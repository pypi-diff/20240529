# Comparing `tmp/fms_robot_plugin-0.3.0rc5.tar.gz` & `tmp/fms_robot_plugin-0.3.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fms_robot_plugin-0.3.0rc5.tar", max compression
+gzip compressed data, was "fms_robot_plugin-0.3.0rc6.tar", max compression
```

## Comparing `fms_robot_plugin-0.3.0rc5.tar` & `fms_robot_plugin-0.3.0rc6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       26 2024-05-28 01:41:02.626855 fms_robot_plugin-0.3.0rc5/README.md
--rw-r--r--   0        0        0       49 2024-05-28 01:41:02.626855 fms_robot_plugin-0.3.0rc5/fms_robot_plugin/__init__.py
--rw-r--r--   0        0        0     1601 2024-05-28 01:41:02.626855 fms_robot_plugin-0.3.0rc5/fms_robot_plugin/constants.py
--rw-r--r--   0        0        0     1824 2024-05-28 01:41:02.626855 fms_robot_plugin-0.3.0rc5/fms_robot_plugin/mqtt.py
--rw-r--r--   0        0        0     9461 2024-05-28 01:41:02.626855 fms_robot_plugin-0.3.0rc5/fms_robot_plugin/robot.py
--rw-r--r--   0        0        0     4033 2024-05-28 01:41:02.626855 fms_robot_plugin-0.3.0rc5/fms_robot_plugin/typings.py
--rw-r--r--   0        0        0      657 2024-05-28 01:41:02.626855 fms_robot_plugin-0.3.0rc5/pyproject.toml
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc5/setup.py
--rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc5/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-05-29 08:36:21.153163 fms_robot_plugin-0.3.0rc6/README.md
+-rw-r--r--   0        0        0       49 2024-05-29 08:36:21.157163 fms_robot_plugin-0.3.0rc6/fms_robot_plugin/__init__.py
+-rw-r--r--   0        0        0     1601 2024-05-29 08:36:21.157163 fms_robot_plugin-0.3.0rc6/fms_robot_plugin/constants.py
+-rw-r--r--   0        0        0     1886 2024-05-29 08:36:21.157163 fms_robot_plugin-0.3.0rc6/fms_robot_plugin/mqtt.py
+-rw-r--r--   0        0        0    10139 2024-05-29 08:36:21.157163 fms_robot_plugin-0.3.0rc6/fms_robot_plugin/robot.py
+-rw-r--r--   0        0        0     4213 2024-05-29 08:36:21.157163 fms_robot_plugin-0.3.0rc6/fms_robot_plugin/typings.py
+-rw-r--r--   0        0        0      657 2024-05-29 08:36:21.157163 fms_robot_plugin-0.3.0rc6/pyproject.toml
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc6/setup.py
+-rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc6/PKG-INFO
```

### Comparing `fms_robot_plugin-0.3.0rc5/fms_robot_plugin/constants.py` & `fms_robot_plugin-0.3.0rc6/fms_robot_plugin/constants.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.3.0rc5/fms_robot_plugin/mqtt.py` & `fms_robot_plugin-0.3.0rc6/fms_robot_plugin/mqtt.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 
 
 class MqttClient:
     def __init__(self, host: str, port: int):
         self.client = mqtt.Client()
         self.client.connect(host, port)
 
-    def publish(self, topic: str, data: Any, serialize: bool = True):
+    def publish(self, topic: str, data: Any, serialize: bool = True, qos: int = 0):
         if serialize:
             data = json.dumps(data, default=str)
 
-        self.client.publish(topic, data)
+        self.client.publish(topic, data, qos)
 
 
 class MqttConsumer:
-    def __init__(self, topic: str, host: str, port: int):
+    def __init__(self, topic: str, qos: int, host: str, port: int):
         self.topic = topic
+        self.qos = qos
         self.url_params: list[tuple[int, str]] = []
         self.host = host
         self.port = port
 
     def consume(self, cb: Callable[[dict, dict], None], serialize: bool = True):
         self.cb = cb
 
@@ -35,15 +36,15 @@
         client.on_connect = self.on_connect
         client.on_message = self.on_message_callback(serialize)
 
         client.connect(self.host, self.port)
         client.loop_start()
 
     def on_connect(self, client, userdata, flags, rc):
-        client.subscribe(self.topic)
+        client.subscribe(self.topic, self.qos)
 
     def on_message_callback(self, serialize: bool = True):
         def on_message(client, userdata, msg):
             msg.topic.split("/")
 
             payload = msg.payload
             if serialize:
```

### Comparing `fms_robot_plugin-0.3.0rc5/fms_robot_plugin/robot.py` & `fms_robot_plugin-0.3.0rc6/fms_robot_plugin/robot.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     Map,
     RobotInfo,
     Task,
     DecimatedPlan,
     Result,
     AcquireLockRequest,
     AcquireLockResponse,
+    ReleaseLockRequest,
+    ReleaseLockResponse,
 )
 from fms_robot_plugin.mqtt import MqttClient, MqttConsumer
 
 
 class Robot:
     robot_key: Optional[str]
 
@@ -37,14 +39,17 @@
     ):
         self.plugin_name = plugin_name
         self.plugin_version = plugin_version
         self.capabilities = capabilities
         self.robot_key = robot_key
         self.priority: int = 0
         self.acquire_lock_message_id: Optional[str] = None
+        self.release_lock_message_id: Optional[str] = None
+        self.traffic_task: Optional[Task] = None
+        self.node_ids: List[str] = []
 
         self.api_hostname = api_hostname
         self.broker_host = broker_host
         self.broker_port = broker_port
         self.mqtt = MqttClient(broker_host, broker_port)
 
     def run(self):
@@ -119,15 +124,19 @@
 
     def on_preview_map(self, cb: Callable[[], None]):
         topic = f"robots/{self.robot_key}/mapping/import"
         self.consumer(topic).consume(lambda _: cb(), serialize=False)
 
     def on_acquire_lock_response(self, cb: Callable[[AcquireLockResponse], None]):
         topic = f"robots/{self.robot_key}/locks/acquire/response"
-        self.consumer(topic).consume(lambda data: cb(AcquireLockResponse(**data)))
+        self.consumer(topic, 2).consume(lambda data: cb(AcquireLockResponse(**data)))
+
+    def on_release_lock_response(self, cb: Callable[[ReleaseLockResponse], None]):
+        topic = f"robots/{self.robot_key}/locks/release/response"
+        self.consumer(topic, 2).consume(lambda data: cb(ReleaseLockResponse(**data)))
 
     """
     Publishers
 
     These methods are called to publish data to the FMS server.
     """
 
@@ -201,22 +210,26 @@
         self.mqtt.publish(f"robots/{self.robot_key}/obstacle", data, serialize=False)
 
     def set_notification_message(self, data: str):
         self.mqtt.publish(f"robots/{self.robot_key}/notification", data, serialize=False)
 
     def set_acquire_lock_request(self, data: AcquireLockRequest):
         self.acquire_lock_message_id = data.message_id
-        self.mqtt.publish(f"robots/{self.robot_key}/locks/acquire/request", data.dict())
+        self.mqtt.publish(f"robots/{self.robot_key}/locks/acquire/request", data.dict(), qos=2)
+
+    def set_release_lock_request(self, data: ReleaseLockRequest):
+        self.release_lock_message_id = data.message_id
+        self.mqtt.publish(f"robots/{self.robot_key}/locks/release/request", data.dict(), qos=2)
 
     """
     Utilities
     """
 
-    def consumer(self, topic: str):
-        return MqttConsumer(topic, self.broker_host, self.broker_port)
+    def consumer(self, topic: str, qos: int = 0):
+        return MqttConsumer(topic, qos, self.broker_host, self.broker_port)
 
     def register_default_callbacks(self):
         self.on_set_priority(self.set_priority)
 
     def set_priority(self, priority):
         self.priority = int(priority.decode("utf-8"))
```

### Comparing `fms_robot_plugin-0.3.0rc5/fms_robot_plugin/typings.py` & `fms_robot_plugin-0.3.0rc6/fms_robot_plugin/typings.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,7 +215,18 @@
     node_ids: List[str]
 
 
 class AcquireLockResponse(BaseModel):
     message_id: str
     result: bool
     error: str = ""
+
+
+class ReleaseLockRequest(BaseModel):
+    message_id: str
+    node_ids: List[str]
+
+
+class ReleaseLockResponse(BaseModel):
+    message_id: str
+    result: bool
+    error: str = ""
```

### Comparing `fms_robot_plugin-0.3.0rc5/pyproject.toml` & `fms_robot_plugin-0.3.0rc6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fms-robot-plugin"
-version = "0.3.0rc5"
+version = "0.3.0rc6"
 description = ""
 authors = [
   "Dionesius Agung <dionesius@movel.ai>",
   "Steven Hansel <steven@movel.ai>"
 ]
 readme = "README.md"
 packages = [{include = "fms_robot_plugin"}]
```

### Comparing `fms_robot_plugin-0.3.0rc5/setup.py` & `fms_robot_plugin-0.3.0rc6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['paho-mqtt>=1.6.1,<2.0.0', 'pydantic>=2.3.0,<3.0.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'fms-robot-plugin',
-    'version': '0.3.0rc5',
+    'version': '0.3.0rc6',
     'description': '',
     'long_description': '# FMS Robot Plugin Library',
     'author': 'Dionesius Agung',
     'author_email': 'dionesius@movel.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

