# Comparing `tmp/barcode_server-2.4.0.tar.gz` & `tmp/barcode_server-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barcode_server-2.4.0.tar", max compression
+gzip compressed data, was "barcode_server-2.4.1.tar", max compression
```

## Comparing `barcode_server-2.4.0.tar` & `barcode_server-2.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    34523 2023-09-09 13:49:17.520884 barcode_server-2.4.0/LICENSE
--rw-r--r--   0        0        0     9784 2023-09-09 13:49:17.520884 barcode_server-2.4.0/README.md
--rw-r--r--   0        0        0        0 2023-09-09 13:49:17.520884 barcode_server-2.4.0/barcode_server/__init__.py
--rw-r--r--   0        0        0     5796 2023-09-09 13:49:17.520884 barcode_server-2.4.0/barcode_server/barcode.py
--rw-r--r--   0        0        0     2335 2023-09-09 13:49:17.520884 barcode_server-2.4.0/barcode_server/cli.py
--rw-r--r--   0        0        0     6322 2023-09-09 13:49:17.520884 barcode_server-2.4.0/barcode_server/config.py
--rw-r--r--   0        0        0     1064 2023-09-09 13:49:17.520884 barcode_server-2.4.0/barcode_server/const.py
--rw-r--r--   0        0        0     6113 2023-09-09 13:49:17.520884 barcode_server-2.4.0/barcode_server/keyevent_reader.py
--rw-r--r--   0        0        0     2963 2023-09-09 13:49:17.520884 barcode_server-2.4.0/barcode_server/notifier/__init__.py
--rw-r--r--   0        0        0     1102 2023-09-09 13:49:17.520884 barcode_server-2.4.0/barcode_server/notifier/http.py
--rw-r--r--   0        0        0     1400 2023-09-09 13:49:17.520884 barcode_server-2.4.0/barcode_server/notifier/mqtt.py
--rw-r--r--   0        0        0      877 2023-09-09 13:49:17.520884 barcode_server-2.4.0/barcode_server/notifier/ws.py
--rw-r--r--   0        0        0      926 2023-09-09 13:49:17.520884 barcode_server-2.4.0/barcode_server/stats.py
--rw-r--r--   0        0        0     1022 2023-09-09 13:49:17.520884 barcode_server-2.4.0/barcode_server/util.py
--rw-r--r--   0        0        0     6977 2023-09-09 13:49:17.520884 barcode_server-2.4.0/barcode_server/webserver.py
--rw-r--r--   0        0        0     1445 2023-09-09 13:49:17.524884 barcode_server-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    11051 1970-01-01 00:00:00.000000 barcode_server-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-29 15:26:53.451065 barcode_server-2.4.1/LICENSE
+-rw-r--r--   0        0        0     9784 2024-05-29 15:26:53.451065 barcode_server-2.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 15:26:53.451065 barcode_server-2.4.1/barcode_server/__init__.py
+-rw-r--r--   0        0        0     5796 2024-05-29 15:26:53.451065 barcode_server-2.4.1/barcode_server/barcode.py
+-rw-r--r--   0        0        0     2335 2024-05-29 15:26:53.451065 barcode_server-2.4.1/barcode_server/cli.py
+-rw-r--r--   0        0        0     6322 2024-05-29 15:26:53.451065 barcode_server-2.4.1/barcode_server/config.py
+-rw-r--r--   0        0        0     1064 2024-05-29 15:26:53.451065 barcode_server-2.4.1/barcode_server/const.py
+-rw-r--r--   0        0        0     6113 2024-05-29 15:26:53.451065 barcode_server-2.4.1/barcode_server/keyevent_reader.py
+-rw-r--r--   0        0        0     2963 2024-05-29 15:26:53.451065 barcode_server-2.4.1/barcode_server/notifier/__init__.py
+-rw-r--r--   0        0        0     1102 2024-05-29 15:26:53.451065 barcode_server-2.4.1/barcode_server/notifier/http.py
+-rw-r--r--   0        0        0     1396 2024-05-29 15:26:53.451065 barcode_server-2.4.1/barcode_server/notifier/mqtt.py
+-rw-r--r--   0        0        0      877 2024-05-29 15:26:53.451065 barcode_server-2.4.1/barcode_server/notifier/ws.py
+-rw-r--r--   0        0        0      926 2024-05-29 15:26:53.451065 barcode_server-2.4.1/barcode_server/stats.py
+-rw-r--r--   0        0        0     1022 2024-05-29 15:26:53.451065 barcode_server-2.4.1/barcode_server/util.py
+-rw-r--r--   0        0        0     6977 2024-05-29 15:26:53.451065 barcode_server-2.4.1/barcode_server/webserver.py
+-rw-r--r--   0        0        0     1440 2024-05-29 15:26:53.451065 barcode_server-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0    11097 1970-01-01 00:00:00.000000 barcode_server-2.4.1/PKG-INFO
```

### Comparing `barcode_server-2.4.0/LICENSE` & `barcode_server-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `barcode_server-2.4.0/README.md` & `barcode_server-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `barcode_server-2.4.0/barcode_server/barcode.py` & `barcode_server-2.4.1/barcode_server/barcode.py`

 * *Files identical despite different names*

### Comparing `barcode_server-2.4.0/barcode_server/cli.py` & `barcode_server-2.4.1/barcode_server/cli.py`

 * *Files identical despite different names*

### Comparing `barcode_server-2.4.0/barcode_server/config.py` & `barcode_server-2.4.1/barcode_server/config.py`

 * *Files identical despite different names*

### Comparing `barcode_server-2.4.0/barcode_server/const.py` & `barcode_server-2.4.1/barcode_server/const.py`

 * *Files identical despite different names*

### Comparing `barcode_server-2.4.0/barcode_server/keyevent_reader.py` & `barcode_server-2.4.1/barcode_server/keyevent_reader.py`

 * *Files identical despite different names*

### Comparing `barcode_server-2.4.0/barcode_server/notifier/__init__.py` & `barcode_server-2.4.1/barcode_server/notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `barcode_server-2.4.0/barcode_server/notifier/http.py` & `barcode_server-2.4.1/barcode_server/notifier/http.py`

 * *Files identical despite different names*

### Comparing `barcode_server-2.4.0/barcode_server/notifier/mqtt.py` & `barcode_server-2.4.1/barcode_server/notifier/mqtt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from asyncio_mqtt import Client
+from aiomqtt import Client
 from prometheus_async.aio import time
 
 from barcode_server.barcode import BarcodeEvent
 from barcode_server.notifier import BarcodeNotifier
 from barcode_server.stats import MQTT_NOTIFIER_TIME
 from barcode_server.util import barcode_event_to_json
 
@@ -29,10 +29,10 @@
         self.retain = retain
 
     @time(MQTT_NOTIFIER_TIME)
     async def _send_event(self, event: BarcodeEvent):
         json = barcode_event_to_json(self.config.INSTANCE_ID.value, event)
         async with Client(hostname=self.host, port=self.port,
                           username=self.user, password=self.password,
-                          client_id=self.client_id) as client:
+                          identifier=self.client_id) as client:
             await client.publish(self.topic, json, self.qos, self.retain)
             LOGGER.debug(f"Notified {self.host}:{self.port}: {event.barcode}")
```

### Comparing `barcode_server-2.4.0/barcode_server/notifier/ws.py` & `barcode_server-2.4.1/barcode_server/notifier/ws.py`

 * *Files identical despite different names*

### Comparing `barcode_server-2.4.0/barcode_server/stats.py` & `barcode_server-2.4.1/barcode_server/stats.py`

 * *Files identical despite different names*

### Comparing `barcode_server-2.4.0/barcode_server/util.py` & `barcode_server-2.4.1/barcode_server/util.py`

 * *Files identical despite different names*

### Comparing `barcode_server-2.4.0/barcode_server/webserver.py` & `barcode_server-2.4.1/barcode_server/webserver.py`

 * *Files identical despite different names*

### Comparing `barcode_server-2.4.0/pyproject.toml` & `barcode_server-2.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "barcode-server"
-version = "2.4.0"
+version = "2.4.1"
 description = "A simple daemon to expose USB Barcode Scanner data to other services using Websockets, Webhooks or MQTT."
 
 license = "AGPL-3.0-or-later"
 
 authors = [
     "Markus Ressel <mail@markusressel.de>",
 ]
@@ -33,15 +33,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"  # Compatible python versions must be declared here
 
 container-app-conf = ">=5.0.0"
 evdev = "*"
 orjson = ">=3,<4"
 aiohttp = "*"
-asyncio-mqtt = "*"
+aiomqtt = "*"
 prometheus-client = "*"
 prometheus_async = "*"
 click = "*"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
```

### Comparing `barcode_server-2.4.0/PKG-INFO` & `barcode_server-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: barcode-server
-Version: 2.4.0
+Version: 2.4.1
 Summary: A simple daemon to expose USB Barcode Scanner data to other services using Websockets, Webhooks or MQTT.
 Home-page: https://github.com/markusressel/barcode-server
 License: AGPL-3.0-or-later
 Keywords: barcode,asyncio,qrcode,http,mqtt,server,websocket,websocket
 Author: Markus Ressel
 Author-email: mail@markusressel.de
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp
-Requires-Dist: asyncio-mqtt
+Requires-Dist: aiomqtt
 Requires-Dist: click
 Requires-Dist: container-app-conf (>=5.0.0)
 Requires-Dist: evdev
 Requires-Dist: orjson (>=3,<4)
 Requires-Dist: prometheus-client
 Requires-Dist: prometheus_async
 Project-URL: Repository, https://github.com/markusressel/barcode-server
```

