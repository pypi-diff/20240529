# Comparing `tmp/realtime-1.0.4.tar.gz` & `tmp/realtime-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realtime-1.0.4.tar", max compression
+gzip compressed data, was "realtime-1.0.5.tar", max compression
```

## Comparing `realtime-1.0.4.tar` & `realtime-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2024-04-13 00:31:43.750297 realtime-1.0.4/LICENSE
--rw-r--r--   0        0        0     1744 2024-04-13 00:31:43.750297 realtime-1.0.4/README.md
--rw-r--r--   0        0        0     1206 2024-04-13 00:31:44.574297 realtime-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      235 2024-04-13 00:31:44.574297 realtime-1.0.4/realtime/__init__.py
--rw-r--r--   0        0        0     2559 2024-04-13 00:31:43.754297 realtime-1.0.4/realtime/channel.py
--rw-r--r--   0        0        0     5744 2024-04-13 00:31:43.754297 realtime-1.0.4/realtime/connection.py
--rw-r--r--   0        0        0      403 2024-04-13 00:31:43.754297 realtime-1.0.4/realtime/exceptions.py
--rw-r--r--   0        0        0      744 2024-04-13 00:31:43.754297 realtime-1.0.4/realtime/message.py
--rw-r--r--   0        0        0     5521 2024-04-13 00:31:43.754297 realtime-1.0.4/realtime/transformers.py
--rw-r--r--   0        0        0      209 2024-04-13 00:31:43.754297 realtime-1.0.4/realtime/types.py
--rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 realtime-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-29 11:00:40.965561 realtime-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1744 2024-05-29 11:00:40.965561 realtime-1.0.5/README.md
+-rw-r--r--   0        0        0     1206 2024-05-29 11:00:42.093555 realtime-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      234 2024-05-29 11:00:42.093555 realtime-1.0.5/realtime/__init__.py
+-rw-r--r--   0        0        0     2544 2024-05-29 11:00:40.965561 realtime-1.0.5/realtime/channel.py
+-rw-r--r--   0        0        0     6030 2024-05-29 11:00:40.965561 realtime-1.0.5/realtime/connection.py
+-rw-r--r--   0        0        0      403 2024-05-29 11:00:40.965561 realtime-1.0.5/realtime/exceptions.py
+-rw-r--r--   0        0        0      767 2024-05-29 11:00:40.965561 realtime-1.0.5/realtime/message.py
+-rw-r--r--   0        0        0     5502 2024-05-29 11:00:40.965561 realtime-1.0.5/realtime/transformers.py
+-rw-r--r--   0        0        0      208 2024-05-29 11:00:40.965561 realtime-1.0.5/realtime/types.py
+-rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 realtime-1.0.5/PKG-INFO
```

### Comparing `realtime-1.0.4/LICENSE` & `realtime-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `realtime-1.0.4/README.md` & `realtime-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `realtime-1.0.4/pyproject.toml` & `realtime-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "realtime"
-version = "1.0.4"
+version = "1.0.5"
 description = ""
 authors = [
     "Joel Lee <joel@joellee.org>",
     "Andrew Smith <a.smith@silentworks.co.uk>"
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `realtime-1.0.4/realtime/channel.py` & `realtime-1.0.5/realtime/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 import asyncio
 import json
-from typing import Any, List, Dict, TYPE_CHECKING, NamedTuple
+from typing import TYPE_CHECKING, Any, Dict, List, NamedTuple
 
 from realtime.types import Callback
 
 if TYPE_CHECKING:
     from realtime.connection import Socket
 
 
 class CallbackListener(NamedTuple):
-    """A tuple with `event` and `callback` """
+    """A tuple with `event` and `callback`"""
+
     event: str
     callback: Callback
 
 
 class Channel:
     """
     `Channel` is an abstraction for a topic listener for an existing socket connection.
@@ -47,16 +48,15 @@
         return self
 
     async def _join(self) -> None:
         """
         Coroutine that attempts to join Phoenix Realtime server via a certain topic
         :return: None
         """
-        join_req = dict(topic=self.topic, event="phx_join",
-                        payload={}, ref=None)
+        join_req = dict(topic=self.topic, event="phx_join", payload={}, ref=None)
 
         try:
             await self.socket.ws_connection.send(json.dumps(join_req))
         except Exception as e:
             print(str(e))  # TODO: better error propagation
             return
 
@@ -72,8 +72,9 @@
 
     def off(self, event: str) -> None:
         """
         :param event: Stop responding to a certain event
         :return: None
         """
         self.listeners = [
-            callback for callback in self.listeners if callback.event != event]
+            callback for callback in self.listeners if callback.event != event
+        ]
```

### Comparing `realtime-1.0.4/realtime/connection.py` & `realtime-1.0.5/realtime/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import asyncio
 import json
 import logging
 from collections import defaultdict
 from functools import wraps
-from typing import Any, Callable, List, Dict, TypeVar, DefaultDict
+from typing import Any, DefaultDict, Dict, List
 
 import websockets
-from typing_extensions import ParamSpec
 
 from realtime.channel import Channel
 from realtime.exceptions import NotConnectedError
 from realtime.message import HEARTBEAT_PAYLOAD, PHOENIX_CHANNEL, ChannelEvents, Message
 from realtime.types import Callback, T_ParamSpec, T_Retval
 
 # logging.basicConfig(
 #     format="%(asctime)s:%(levelname)s - %(message)s", level=logging.INFO
 # )
 
+
 def ensure_connection(func: Callback):
     @wraps(func)
     def wrapper(*args: T_ParamSpec.args, **kwargs: T_ParamSpec.kwargs) -> T_Retval:
         if not args[0].connected:
             raise NotConnectedError(func.__name__)
 
         return func(*args, **kwargs)
@@ -109,14 +109,26 @@
         if ws_connection.open:
             logging.info("Connection was successful")
             self.ws_connection = ws_connection
             self.connected = True
         else:
             raise Exception("Connection Failed")
 
+    @ensure_connection
+    def close(self) -> None:
+        """
+        Wrapper for async def _close() to expose a non-async interface
+        """
+        loop = asyncio.get_event_loop()
+        loop.run_until_complete(self._close())
+        self.connected = False
+
+    async def _close(self) -> None:
+        await self.ws_connection.close()
+
     async def _keep_alive(self) -> None:
         """
         Sending heartbeat to server every 5 seconds
         Ping - pong messages to verify connection is alive
         """
         while True:
             try:
```

### Comparing `realtime-1.0.4/realtime/message.py` & `realtime-1.0.5/realtime/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 
 
 @dataclass
 class Message:
     """
     Dataclass abstraction for message
     """
+
     event: str
     payload: Dict[str, Any]
     ref: Any
     topic: str
 
     def __hash__(self):
-        return hash((self.event, tuple(list(self.payload.values())), self.ref, self.topic))
+        return hash(
+            (self.event, tuple(list(self.payload.values())), self.ref, self.topic)
+        )
 
 
 class ChannelEvents(str, Enum):
     """
     ChannelEvents are a bunch of constant strings that are defined according to
     what the Phoenix realtime server expects.
     """
```

### Comparing `realtime-1.0.4/realtime/transformers.py` & `realtime-1.0.5/realtime/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Converts the change Payload into native Python types.
 """
+
 import json
-from dateutil.parser import parse
 
+from dateutil.parser import parse
 
 abstime = "abstime"
 _bool = "bool"  # bool is a keyword in python
 date = "date"
 daterange = "daterange"
 float4 = "float4"
 float8 = "float8"
@@ -38,19 +39,19 @@
 :param records:
 :param options: The map of various options that can be applied to the mapper
 
 """
 
 
 def convert_change_data(columns, records, options={}):
-    skip_types = options.get("skip_types") if options.get(
-        "skip_types") == "undefined" else []
+    skip_types = (
+        options.get("skip_types") if options.get("skip_types") == "undefined" else []
+    )
     return {
-        key: convert_column(key, columns, records, skip_types)
-        for key in records.keys()
+        key: convert_column(key, columns, records, skip_types) for key in records.keys()
     }
 
 
 def convert_column(column_name, columns, records, skip_types):
     column = next(filter(lambda x: x.get("name") == column_name, columns))
     if not column or column.get("type") in skip_types:
         return noop(records[column_name])
@@ -60,15 +61,15 @@
 
 def convert_cell(_type: str, string_value: str):
     try:
         if string_value is None:
             return None
         # If data type is an array
         if _type[0] == "_":
-            array_value = _type[1:len(_type)]
+            array_value = _type[1 : len(_type)]
             return to_array(string_value, array_value)
         # If it's not null then we need to convert it to the correct type
         if _type == abstime:
             return noop(string_value)
         elif _type == _bool:
             print("converted to bool")
             return to_boolean(string_value)
@@ -119,16 +120,15 @@
         elif _type == tstzrange:
             return to_date_range(string_value)
         else:
             # All the rest will be returned as strings
             return noop(string_value)
 
     except Exception as e:
-        print(
-            f"Could not convert cell of type {_type} and value {string_value}")
+        print(f"Could not convert cell of type {_type} and value {string_value}")
         print(f"This is the error {e}")
         return string_value
 
 
 def noop(string_value: str):
     return string_value
 
@@ -175,20 +175,19 @@
 >>> to_array('{}', 'int4')
     []
 """
 
 
 def to_array(string_value: str, type: str):
     # this takes off the '{' & '}'
-    string_enriched = string_value[1: len(string_value) - 1]
+    string_enriched = string_value[1 : len(string_value) - 1]
 
     # Converts the string into an array
     # if string is empty (meaning the array was empty), an empty array will be immediately returned
-    string_array = string_enriched.split(
-        ",") if len(string_enriched) > 0 else []
+    string_array = string_enriched.split(",") if len(string_enriched) > 0 else []
     return list(map(lambda string: convert_cell(type, string), string_array))
 
 
 """
 Fixes timestamp to be ISO-8601. Swaps the space between the date and time for a 'T'
 >>> to_timestamp_string('2019-09-10 00:00:00')
     '2019-09-10T00:00:00'
```

### Comparing `realtime-1.0.4/PKG-INFO` & `realtime-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtime
-Version: 1.0.4
+Version: 1.0.5
 Summary: 
 Home-page: https://github.com/supabase-community/realtime-py
 License: MIT
 Author: Joel Lee
 Author-email: joel@joellee.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

