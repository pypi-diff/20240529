# Comparing `tmp/scratchcommunication-2.9.2.tar.gz` & `tmp/scratchcommunication-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.9.2.tar", last modified: Tue May 28 18:06:36 2024, max compression
+gzip compressed data, was "scratchcommunication-2.9.4.tar", last modified: Wed May 29 11:55:25 2024, max compression
```

## Comparing `scratchcommunication-2.9.2.tar` & `scratchcommunication-2.9.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18303 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11441 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-28 18:06:36.000000 scratchcommunication-2.9.2/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-28 18:06:36.000000 scratchcommunication-2.9.2/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:06:36.000000 scratchcommunication-2.9.2/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-28 18:06:36.000000 scratchcommunication-2.9.2/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 18:06:36.000000 scratchcommunication-2.9.2/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/tests/test1.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/tests/test2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:55:25.023272 scratchcommunication-2.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-29 11:55:25.023272 scratchcommunication-2.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:55:25.023272 scratchcommunication-2.9.4/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18247 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15163 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:55:25.023272 scratchcommunication-2.9.4/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:55:25.023272 scratchcommunication-2.9.4/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-29 11:55:25.000000 scratchcommunication-2.9.4/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-29 11:55:25.000000 scratchcommunication-2.9.4/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:55:25.000000 scratchcommunication-2.9.4/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 11:55:25.000000 scratchcommunication-2.9.4/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 11:55:25.000000 scratchcommunication-2.9.4/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 11:55:25.023272 scratchcommunication-2.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:55:25.023272 scratchcommunication-2.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/tests/test1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-29 11:55:21.000000 scratchcommunication-2.9.4/tests/test2.py
```

### Comparing `scratchcommunication-2.9.2/LICENSE` & `scratchcommunication-2.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.9.2/PKG-INFO` & `scratchcommunication-2.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.9.2
+Version: 2.9.4
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.9.2/README.md` & `scratchcommunication-2.9.4/README.md`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.9.2/scratchcommunication/cloud.py` & `scratchcommunication-2.9.4/scratchcommunication/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Literal, Union, Any, Protocol
 from collections.abc import Callable
 from .exceptions import QuickAccessDisabledError, NotSupported, ErrorInEventHandler, StopException, EventExpiredError
 import scratchcommunication
 from func_timeout import StoppableThread
 import json, time, requests, warnings, traceback, secrets, sys
-from websocket import WebSocket
+from websocket import WebSocket, WebSocketConnectionClosedException, WebSocketTimeoutException
 
 NoneType = type(None)
 CloudConnection = None
 
 class EventDispatcher(Protocol):
     def __call__(self, data : dict, **entries) -> None:
         pass
@@ -134,15 +134,15 @@
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.stop_thread()
 
     def stop_thread(self):
         """
         Use for stopping the underlying thread.
-        """
+        """#
         self.thread_running = False
         self.data_reception.stop(StopException, 0.1)
         self.data_reception.join(5)
 
     def enable_quickaccess(self):
         """
         Use for enabling the use of the object as a lookup table.
@@ -328,49 +328,45 @@
         """
         Use for receiving new cloud data.
         """
         data = [json.loads(j) for j in self.websocket.recv().split("\n") if j]
         
         for i in data:
             i["var"] = i["name"]
-            i["name"] = i["name"].replace("☁ ", "", 1)
+            i["name"] = i["name"].removeprefix("☁ ")
             method = i.pop("method")
             if not first:
                 self.emit_event(method, **i)
             if method == "set":
                 self.values[i["var"]] = i["value"]
         return self.values
 
-    def receive_data(self):
-        """
-        Use for receiving cloud data.
-        """
+    def _prepare_connection(self):
         while self.thread_running:
             try:
                 self.receive_new_data(first=True)
                 break
-            except TimeoutError:
+            except WebSocketTimeoutException:
                 pass
-            except Exception:
+            except WebSocketConnectionClosedException:
                 self._connect()
+
+    def receive_data(self):
+        """
+        Use for receiving cloud data.
+        """
+        self._prepare_connection()
         while self.thread_running:
             try:
                 self.receive_new_data()
-            except TimeoutError:
+            except WebSocketTimeoutException:
                 pass
-            except Exception:
+            except WebSocketConnectionClosedException:
                 self._connect()
-                while self.thread_running:
-                    try:
-                        self.receive_new_data(first=True)
-                        break
-                    except TimeoutError:
-                        pass
-                    except Exception:
-                        self._connect()
+                self._prepare_connection()
                     
     def get_age_of_event(self, event : Event) -> int:
         """
         Do not use.
         """
         try:
             return len(self.event_order.get(event.value, {})) - self.event_order.get(event.value, {})[event] - 1
```

### Comparing `scratchcommunication-2.9.2/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.9.4/scratchcommunication/cloud_socket.py`

 * *Files 8% similar despite different names*

```diff
@@ -160,24 +160,25 @@
         self.clients = {}
         self.new_clients = []
         self.connecting_clients = []
         self.key_parts = {}
         self.last_timestamp = time.time()
         self.packet_size = packet_size
         self.accepting = Lock()
-        self.accepted = Condition()
-        self.received_any = Condition()
-        self.any_update = Condition()
+        self.accepted = Condition(Lock())
+        self.received_any = Condition(Lock())
+        self.any_update = Condition(Lock())
         
     def listen(self):
         """
         Start the cloud socket.
         """
         @self.cloud.on("set")
         def on_packet(event):
+            
             try:
                 assert event.type == "set"
                 assert event.name == "FROM_CLIENT"
                 salt = 0
                 value = event.value.replace("-", "")
                 msg_data = value.split(".", 1)[0]
                 msg_type = int(value[0])
@@ -192,25 +193,28 @@
                     if len(self.key_parts) >= 100:
                         for key_part_id in list(self.key_parts.keys())[:-100]:
                             self.key_parts.pop(key_part_id)
                     return
                             
                 # Non secure message part
                 
-                if (client := value.split(".", 1)[1][:5]) in self.clients and not self.clients[client].secure:
+                client = value.split(".", 1)[1][:5]
+                
+                if not self._decode(msg_data[1:29]).startswith("_connect") and client in self.clients and not self.clients[client].secure:
                     self.clients[client].current_msg.add(msg_data)
                     assert not "-" in event.value
                     self.clients[client].current_msg.finalize()
+                    self.clients[client]._new_msg()
                     self.clients[client].new_msgs.append(self.clients[client].current_msg)
                     self.clients[client].current_msg = CloudSocketMSG()
                     return
                 
                 # Secure message part
                 
-                if client in self.clients and self.clients[client].secure:
+                if not self._decode(msg_data[1:29]).startswith("_connect") and client in self.clients and self.clients[client].secure:
                     salt = int(msg_data[-15:]) / 100
                     assert salt > self.last_timestamp, "Invalid salt(too little)"
                     assert salt < time.time() + 30, "Invalid salt(too big)"
                     self.last_timestamp = salt
                     self.clients[client].current_msg.add(" "+self.clients[client].encrypter.decrypt(self._decode(msg_data[1:-15]), msg_data[-15:]))
                     assert not "-" in event.value
                     self.clients[client].current_msg.finalize(decode=False)
@@ -239,16 +243,18 @@
                 try:
                     client_username = event.user
                 except NotSupported:
                     client_username = None
                 client_obj = CloudSocketConnection(cloud_socket=self, client_id=client, username=client_username, security=key)
                 self.clients[client] = client_obj
                 self.new_clients.append((client_obj, client_username))
-                self.accepted.notify_all()
-                self.any_update.notify_all()
+                with self.accepted:
+                    self.accepted.notify_all()
+                with self.any_update:
+                    self.any_update.notify_all()
                 return
             except AssertionError:
                 pass
             
     def stop(self):
         self.cloud.stop_thread()
 
@@ -283,28 +289,29 @@
                 encoded += char_to_idx["?"]
         return int(encoded)
     
     def accept(self, timeout : Union[float, None] = 10) -> tuple[BaseCloudSocketConnection, str]:
         """
         Returns a new client
         """
-        endtime = (time.time() + timeout) if timeout is not None else None
-        result = self.accepting.acquire(timeout=timeout if timeout is not None else -1)
-        if not result:
-            raise TimeoutError("The timeout expired (consider setting timeout=None)")
-        try:
-            while (not self.new_clients) and (timeout is None or time.time() < endtime): 
-                self.accepted.wait(timeout and endtime - time.time())
-            try:
-                new_client = self.new_clients.pop(0)
-                return new_client
-            except IndexError:
+        with self.accepted:
+            endtime = (time.time() + timeout) if timeout is not None else None
+            result = self.accepting.acquire(timeout=timeout if timeout is not None else -1)
+            if not result:
                 raise TimeoutError("The timeout expired (consider setting timeout=None)")
-        finally:
-            self.accepting.release()
+            try:
+                while (not self.new_clients) and (timeout is None or time.time() < endtime): 
+                    self.accepted.wait(timeout and endtime - time.time())
+                try:
+                    new_client = self.new_clients.pop(0)
+                    return new_client
+                except IndexError:
+                    raise TimeoutError("The timeout expired (consider setting timeout=None)")
+            finally:
+                self.accepting.release()
     
 class CloudSocketConnection(BaseCloudSocketConnection):
     """
     Class for handling incoming connections from a cloud socket
     """
     def __init__(self, *, cloud_socket : BaseCloudSocket, client_id : str, username : str = None, security : str = None):
         self.cloud_socket = cloud_socket
@@ -313,79 +320,81 @@
         self.security = security
         self.encrypter = sec.SymmetricEncryption(self.security)
         self.secure = bool(self.security)
         self.new_msgs = []
         self.current_msg = CloudSocketMSG()
         self.receiving = Lock()
         self.sending = Lock()
-        self.received = Condition()
+        self.received = Condition(Lock())
 
     def __enter__(self):
         return self
     
     def __exit__(self, exc_type, exc_value, traceback):
         pass
     
     def _secure_send(self, data : str):
         """
         Use for sending data to the client if secure
         """
-        packets = ["".join(i) for i in batched(data, self.cloud_socket.packet_size // 2 - 25)]
+        packets = ["".join(i) for i in batched(data, self.cloud_socket.packet_size // 2 - 28)]
         packet_idx = 0
         for packet in packets[:-1]:
             salt = int(time.time() * 100)
             packet = self.cloud_socket._encode(self.encrypter.encrypt(packet, salt=salt))
-            self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"-{packet}{str(salt).zfill(15)}.{self.client_id}{packet_idx}")
+            self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"-{packet}{str(salt).zfill(15)}.{self.client_id}{random.randrange(1000):03}{packet_idx}")
             packet_idx += 1
         salt = int(time.time() * 100)
         packet = self.cloud_socket._encode(self.encrypter.encrypt(packets[-1], salt=salt))
-        self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"{packet}{str(salt).zfill(15)}.{self.client_id}{packet_idx}")
+        self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"{packet}{str(salt).zfill(15)}.{self.client_id}{random.randrange(1000):03}{packet_idx}")
     
     def send(self, data : str):
         """
         Use for sending data to the client
         """
         with self.sending:
             if self.secure:
                 self._secure_send(data)
                 return
             data = str(self.cloud_socket._encode(data))
             packets = ["".join(i) for i in batched(data, self.cloud_socket.packet_size)]
             packet_idx = 0
             for packet in packets[:-1]:
-                self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"-{packet}.{self.client_id}{packet_idx}")
+                self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"-{packet}.{self.client_id}{random.randrange(1000):03}{packet_idx}")
                 packet_idx += 1
-            self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"{packets[-1]}.{self.client_id}{packet_idx}")
+            self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"{packets[-1]}.{self.client_id}{random.randrange(1000):03}{packet_idx}")
 
     def recv(self, timeout : Union[float, None] = 10) -> str:
         """
         Use for receiving data from the client
         timeout defaults to 10 (seconds) but can be set to None if you do not want timeout.
         """
-        endtime = (time.time() + timeout) if timeout is not None else None
-        result = self.receiving.acquire(timeout=timeout if timeout is not None else -1)
-        if not result:
-            raise TimeoutError("The timeout expired (consider setting timeout=None)")
-        try:
-            while (not self.new_msgs) and (timeout is None or time.time() < endtime):
-                self.received.wait(timeout and endtime - time.time())
-            try:
-                return self.new_msgs.pop(0).message
-            except IndexError:
+        with self.received:
+            endtime = (time.time() + timeout) if timeout is not None else None
+            result = self.receiving.acquire(timeout=timeout if timeout is not None else -1)
+            if not result:
                 raise TimeoutError("The timeout expired (consider setting timeout=None)")
-        finally:
-            self.receiving.release()
+            try:
+                while (not self.new_msgs) and (timeout is None or time.time() < endtime):
+                    self.received.wait(timeout and endtime - time.time())
+                try:
+                    return self.new_msgs.pop(0).message
+                except IndexError:
+                    raise TimeoutError("The timeout expired (consider setting timeout=None)")
+            finally:
+                self.receiving.release()
             
     def _new_msg(self):
         """
         Don't use.
         """
-        self.received.notify_all()
-        self.cloud_socket.received_any.notify_all()
-        self.cloud_socket.any_update.notify_all()
+        with self.received, self.cloud_socket.received_any, self.cloud_socket.any_update:
+            self.received.notify_all()
+            self.cloud_socket.received_any.notify_all()
+            self.cloud_socket.any_update.notify_all()
     
 class CloudSocketMSG(BaseCloudSocketMSG):
     """
     Class for cloud socket messages.
     """
     def __init__(self, message : str = "", complete : bool = False):
         self.message = message
```

### Comparing `scratchcommunication-2.9.2/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.9.4/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.9.2/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.9.4/scratchcommunication/cloudrequests/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,55 +51,56 @@
         """
         self.cloud_socket.listen()
         if thread or (thread is None and self.uses_thread):
             self.uses_thread = True
             self.thread = StoppableThread(target=lambda : self.start(thread=False), daemon=daemon_thread)
             self.thread.start()
             return
-        clients : list[tuple[CloudSocketConnection, str]] = []
-        end_time = duration and (time.time() + duration)
-        while (not end_time) or time.time() < end_time:
-            self.cloud_socket.any_update.wait(30)
-            try:
+        with self.cloud_socket.any_update:
+            clients : list[tuple[CloudSocketConnection, str]] = []
+            end_time = duration and (time.time() + duration)
+            while (not end_time) or time.time() < end_time:
+                success = self.cloud_socket.any_update.wait(30)
                 try:
-                    clients.append(self.cloud_socket.accept(timeout=0))
-                except TimeoutError:
-                    pass
-                for client, username in clients:
                     try:
-                        msg = client.recv(timeout=0)
+                        clients.append(self.cloud_socket.accept(timeout=0))
                     except TimeoutError:
-                        continue
-                    response = "No response."
-                    try:
-                        self.current_client = client
-                        self.current_client_username = username
-                        raw_sub_requests = [raw_request.strip() for raw_request in msg.split(";")]
-                        sub_request_names = [re.match(r"\w+", raw_request).group() for raw_request in raw_sub_requests]
-                        for req_name, raw_req in zip(sub_request_names, raw_sub_requests):
-                            if re.match(r"\w+\(.*\)$", raw_req) and self.requests[req_name].allow_python_syntax:
-                                name, args, kwargs = parse_python_request(raw_req, req_name)
-                            elif not re.match(r"\w+\(.*\)$", raw_req):
-                                name, args, kwargs = parse_normal_request(raw_req, req_name)
-                            else:
-                                raise PermissionError("Python syntax is not allowed for this.")
-                    except Exception:
-                        response = "The command syntax was wrong."
-                        warnings.warn("Received a request with an invalid syntax: \n"+traceback.format_exc(), RuntimeWarning)
-                    else:
+                        pass
+                    for client, username in clients:
+                        try:
+                            msg = client.recv(timeout=0)
+                        except TimeoutError:
+                            continue
+                        response = "No response."
                         try:
-                            self.execute_request(name, args=args, kwargs=kwargs, client=client)
-                            response = None
+                            self.current_client = client
+                            self.current_client_username = username
+                            raw_sub_requests = [raw_request.strip() for raw_request in msg.split(";")]
+                            sub_request_names = [re.match(r"\w+", raw_request).group() for raw_request in raw_sub_requests]
+                            for req_name, raw_req in zip(sub_request_names, raw_sub_requests):
+                                if re.match(r"\w+\(.*\)$", raw_req) and self.requests[req_name].allow_python_syntax:
+                                    name, args, kwargs = parse_python_request(raw_req, req_name)
+                                elif not re.match(r"\w+\(.*\)$", raw_req):
+                                    name, args, kwargs = parse_normal_request(raw_req, req_name)
+                                else:
+                                    raise PermissionError("Python syntax is not allowed for this.")
                         except Exception:
-                            response = "Something went wrong."
-                            warnings.warn("Something went wrong with a request.", RuntimeWarning)
-                    if response:
-                        client.send(response)
-            except Exception:
-                warnings.warn(f"There was an uncaught error in the request handler: {traceback.format_exc()}", RuntimeWarning)
+                            response = "The command syntax was wrong."
+                            warnings.warn("Received a request with an invalid syntax: \n"+traceback.format_exc(), RuntimeWarning)
+                        else:
+                            try:
+                                self.execute_request(name, args=args, kwargs=kwargs, client=client)
+                                response = None
+                            except Exception:
+                                response = "Something went wrong."
+                                warnings.warn(f"Something went wrong with a request: {traceback.format_exc()}", RuntimeWarning)
+                        if response:
+                            client.send(response)
+                except Exception:
+                    warnings.warn(f"There was an uncaught error in the request handler: {traceback.format_exc()}", RuntimeWarning)
                 
     
     def execute_request(self, name, *, args : Sequence[Any], kwargs : Mapping[str, Any], client : CloudSocketConnection) -> None:
         """
         Execute a request.
         """
         request_handling_function = self.requests[name]
@@ -116,18 +117,20 @@
             return
         respond()
     
     def stop(self):
         """
         Stop the request handler.
         """
-        if self.uses_thread:
+        if not self.uses_thread:
             raise NotUsingAThread("Can't stop a request handler that is not using a thread.")
         self.thread.stop(StopRequestHandler)
         self.cloud_socket.stop()
+        with self.cloud_socket.any_update:
+            self.cloud_socket.any_update.notify_all()
         self.thread.join(5)
                    
                    
 KW = Parameter.KEYWORD_ONLY
 KWPS = Parameter.POSITIONAL_OR_KEYWORD
 PS = Parameter.POSITIONAL_ONLY
 MKW = Parameter.VAR_KEYWORD
```

### Comparing `scratchcommunication-2.9.2/scratchcommunication/security.py` & `scratchcommunication-2.9.4/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.9.2/scratchcommunication/session.py` & `scratchcommunication-2.9.4/scratchcommunication/session.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.9.2/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.9.4/scratchcommunication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.9.2
+Version: 2.9.4
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.9.2/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.9.4/scratchcommunication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.9.2/setup.py` & `scratchcommunication-2.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '2.9.2'
+VERSION = '2.9.4'
 
 setup(
     name='scratchcommunication',
     version=VERSION,
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
```

### Comparing `scratchcommunication-2.9.2/tests/test1.py` & `scratchcommunication-2.9.4/tests/test1.py`

 * *Files identical despite different names*

