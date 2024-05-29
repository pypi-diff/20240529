# Comparing `tmp/znsocket-0.1.2.tar.gz` & `tmp/znsocket-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "znsocket-0.1.2.tar", max compression
+gzip compressed data, was "znsocket-0.1.3.tar", max compression
```

## Comparing `znsocket-0.1.2.tar` & `znsocket-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    13576 2024-05-21 18:30:56.569753 znsocket-0.1.2/LICENSE
--rw-r--r--   0        0        0     2272 2024-05-29 09:17:19.572849 znsocket-0.1.2/README.md
--rw-r--r--   0        0        0      776 2024-05-29 09:17:19.573404 znsocket-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      118 2024-05-29 06:27:24.262336 znsocket-0.1.2/znsocket/__init__.py
--rw-r--r--   0        0        0      804 2024-05-28 19:53:23.205211 znsocket-0.1.2/znsocket/cli.py
--rw-r--r--   0        0        0     3029 2024-05-29 09:17:19.574403 znsocket-0.1.2/znsocket/client.py
--rw-r--r--   0        0        0      157 2024-05-29 09:17:19.574517 znsocket-0.1.2/znsocket/exceptions.py
--rw-r--r--   0        0        0     6342 2024-05-29 09:17:19.574747 znsocket-0.1.2/znsocket/server.py
--rw-r--r--   0        0        0     3262 2024-05-29 08:55:53.618742 znsocket-0.1.2/znsocket/utils.py
--rw-r--r--   0        0        0     2990 1970-01-01 00:00:00.000000 znsocket-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    13576 2024-05-21 18:30:56.569753 znsocket-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2265 2024-05-29 16:52:57.368186 znsocket-0.1.3/README.md
+-rw-r--r--   0        0        0      807 2024-05-29 16:52:57.368563 znsocket-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-05-29 06:27:24.262336 znsocket-0.1.3/znsocket/__init__.py
+-rw-r--r--   0        0        0      804 2024-05-28 19:53:23.205211 znsocket-0.1.3/znsocket/cli.py
+-rw-r--r--   0        0        0     3383 2024-05-29 16:52:57.368904 znsocket-0.1.3/znsocket/client.py
+-rw-r--r--   0        0        0      492 2024-05-29 16:52:57.368999 znsocket-0.1.3/znsocket/exceptions.py
+-rw-r--r--   0        0        0     6342 2024-05-29 09:17:19.574747 znsocket-0.1.3/znsocket/server.py
+-rw-r--r--   0        0        0     3359 2024-05-29 16:52:57.369099 znsocket-0.1.3/znsocket/utils.py
+-rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 znsocket-0.1.3/PKG-INFO
```

### Comparing `znsocket-0.1.2/LICENSE` & `znsocket-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `znsocket-0.1.2/README.md` & `znsocket-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 # Set and get a value
 c.set("name", "Fabian")
 assert c.get("name") == "Fabian"
 ```
 
 > [!NOTE]
-> ZnSocket does not decode strings automatically. Using it is equivalent to using `Redis.from_url(storage, decode_responses=True)` in the Redis client.
+> ZnSocket does not encode/decode strings. Using it is equivalent to using `Redis.from_url(storage, decode_responses=True)` in the Redis client.
 
 
 ## Lists
 ZnSocket provides a synchronized version of the Python `list` implementation. Unlike a regular Python list, the data in `znsocket.List` is not stored locally; instead, it is dynamically pushed to and pulled from the server.
 
 Below is a step-by-step example of how to use `znsocket.List` to interact with a ZnSocket server.
```

### Comparing `znsocket-0.1.2/pyproject.toml` & `znsocket-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [tool.poetry]
 name = "znsocket"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python implementation of a Redis-compatible API using websockets."
 authors = ["Fabian Zills <fzills@icp.uni-stuttgart.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 python-socketio = {extras = ["client"], version = "^5"}
 eventlet = "^0"
 typer = "^0"
+znjson = "^0.2.3"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.4"
 pytest = "^8.2"
 coverage = "^7.5.1"
 redis = "^5"
+numpy = "^1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 znsocket = "znsocket.cli:app"
```

### Comparing `znsocket-0.1.2/znsocket/cli.py` & `znsocket-0.1.3/znsocket/cli.py`

 * *Files identical despite different names*

### Comparing `znsocket-0.1.2/znsocket/client.py` & `znsocket-0.1.3/znsocket/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 import dataclasses
 
-import socketio
+import socketio.exceptions
 
 from znsocket import exceptions
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Client:
     address: str
-    sio: socketio.SimpleClient = dataclasses.field(default=None, repr=False, init=False)
+    decode_responses: bool = True
+    sio: socketio.SimpleClient = dataclasses.field(
+        default_factory=socketio.SimpleClient, repr=False, init=False
+    )
 
     @classmethod
-    def from_url(cls, url):
+    def from_url(cls, url, **kwargs) -> "Client":
         """Connect to a znsocket server using a URL.
 
         Parameters
         ----------
         url : str
             The URL of the znsocket server. Should be in the format
             "znsocket://127.0.0.1:5000".
         """
-        return cls(address=url.replace("znsocket://", "http://"))
+        return cls(address=url.replace("znsocket://", "http://"), **kwargs)
 
     def __post_init__(self):
-        self.sio = socketio.SimpleClient()
-        self.sio.connect(self.address)
+        try:
+            self.sio.connect(self.address)
+        except socketio.exceptions.ConnectionError as err:
+            raise exceptions.ConnectionError(self.address) from err
+
+        if not self.decode_responses:
+            raise NotImplementedError("decode_responses=False is not supported yet")
 
     def delete(self, name):
         return self.sio.call("delete", {"name": name})
 
     def hget(self, name, key):
         return self.sio.call("hget", {"name": name, "key": key})
```

### Comparing `znsocket-0.1.2/znsocket/server.py` & `znsocket-0.1.3/znsocket/server.py`

 * *Files identical despite different names*

### Comparing `znsocket-0.1.2/znsocket/utils.py` & `znsocket-0.1.3/znsocket/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import json
 import typing as t
 from collections.abc import MutableSequence
 
+import znjson
+
 from .client import Client
 
 
 class List(MutableSequence):
     def __init__(self, r: Client | t.Any, key: str):
         """Synchronized list object.
 
@@ -34,25 +37,28 @@
         if single_item:
             index = [index]
         if isinstance(index, slice):
             index = list(range(*index.indices(len(self))))
 
         items = []
         for i in index:
-            item = self.redis.lindex(self.key, i)
+            value = self.redis.lindex(self.key, i)
+            try:
+                item = znjson.loads(value)
+            except TypeError:
+                item = value
             if item is None:
                 raise IndexError("list index out of range")
             items.append(item)
         return items[0] if single_item else items
 
     def __setitem__(self, index: int | list | slice, value: str | list[str]):
         single_item = isinstance(index, int)
         if single_item:
             index = [index]
-            assert isinstance(value, str), "single index requires single value"
             value = [value]
 
         if isinstance(index, slice):
             index = list(range(*index.indices(len(self))))
 
         index = [int(i) for i in index]
 
@@ -60,41 +66,41 @@
             raise ValueError(
                 f"attempt to assign sequence of size {len(value)} to extended slice of size {len(index)}"
             )
 
         for i, v in zip(index, value):
             if i >= self.__len__() or i < -self.__len__():
                 raise IndexError("list index out of range")
-            self.redis.lset(self.key, i, v)
+            self.redis.lset(self.key, i, znjson.dumps(v))
 
     def __delitem__(self, index: int | list | slice):
         single_item = isinstance(index, int)
         if single_item:
             index = [index]
         if isinstance(index, slice):
             index = list(range(*index.indices(len(self))))
 
         for i in index:
             self.redis.lset(self.key, i, "__DELETED__")
         self.redis.lrem(self.key, 0, "__DELETED__")
 
     def insert(self, index, value):
         if index >= self.__len__():
-            self.redis.rpush(self.key, value)
+            self.redis.rpush(self.key, znjson.dumps(value))
         elif index == 0:
-            self.redis.lpush(self.key, value)
+            self.redis.lpush(self.key, znjson.dumps(value))
         else:
             pivot = self.redis.lindex(self.key, index)
-            self.redis.linsert(self.key, "BEFORE", pivot, value)
-
-    def __iter__(self):
-        return (item for item in self.redis.lrange(self.key, 0, -1))
+            self.redis.linsert(self.key, "BEFORE", pivot, znjson.dumps(value))
 
     def __eq__(self, value: object) -> bool:
         if isinstance(value, List):
             return self[:] == value[:]
         elif isinstance(value, list):
             return self[:] == value
         return False
 
     def __repr__(self):
-        return f"List({self.redis.lrange(self.key, 0, -1)})"
+        data = self.redis.lrange(self.key, 0, -1)
+        data = [znjson.loads(i) for i in data]
+
+        return f"List({data})"
```

### Comparing `znsocket-0.1.2/PKG-INFO` & `znsocket-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: znsocket
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python implementation of a Redis-compatible API using websockets.
 License: Apache-2.0
 Author: Fabian Zills
 Author-email: fzills@icp.uni-stuttgart.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: eventlet (>=0,<1)
 Requires-Dist: python-socketio[client] (>=5,<6)
 Requires-Dist: typer (>=0,<1)
+Requires-Dist: znjson (>=0.2.3,<0.3.0)
 Project-URL: repository, https://github.com/zincware/ZnSocket
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/znsocket.svg)](https://badge.fury.io/py/znsocket)
 [![Coverage Status](https://coveralls.io/repos/github/zincware/ZnSocket/badge.svg?branch=main)](https://coveralls.io/github/zincware/ZnSocket?branch=main)
 ![PyTest](https://github.com/zincware/ZnSocket/actions/workflows/pytest.yaml/badge.svg)
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
@@ -53,15 +54,15 @@
 
 # Set and get a value
 c.set("name", "Fabian")
 assert c.get("name") == "Fabian"
 ```
 
 > [!NOTE]
-> ZnSocket does not decode strings automatically. Using it is equivalent to using `Redis.from_url(storage, decode_responses=True)` in the Redis client.
+> ZnSocket does not encode/decode strings. Using it is equivalent to using `Redis.from_url(storage, decode_responses=True)` in the Redis client.
 
 
 ## Lists
 ZnSocket provides a synchronized version of the Python `list` implementation. Unlike a regular Python list, the data in `znsocket.List` is not stored locally; instead, it is dynamically pushed to and pulled from the server.
 
 Below is a step-by-step example of how to use `znsocket.List` to interact with a ZnSocket server.
```

