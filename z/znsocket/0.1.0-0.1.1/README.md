# Comparing `tmp/znsocket-0.1.0.tar.gz` & `tmp/znsocket-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "znsocket-0.1.0.tar", max compression
+gzip compressed data, was "znsocket-0.1.1.tar", max compression
```

## Comparing `znsocket-0.1.0.tar` & `znsocket-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    13576 2024-05-21 18:30:56.569753 znsocket-0.1.0/LICENSE
--rw-r--r--   0        0        0     1429 2024-05-28 19:11:48.263068 znsocket-0.1.0/README.md
--rw-r--r--   0        0        0      777 2024-05-28 19:11:48.263469 znsocket-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      130 2024-05-28 19:11:48.263828 znsocket-0.1.0/znsocket/__init__.py
--rw-r--r--   0        0        0      694 2024-05-28 19:11:48.263992 znsocket-0.1.0/znsocket/cli.py
--rw-r--r--   0        0        0     2521 2024-05-28 19:11:48.264166 znsocket-0.1.0/znsocket/client.py
--rw-r--r--   0        0        0     4273 2024-05-28 19:11:48.264345 znsocket-0.1.0/znsocket/server.py
--rw-r--r--   0        0        0     2148 1970-01-01 00:00:00.000000 znsocket-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    13576 2024-05-21 18:30:56.569753 znsocket-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1429 2024-05-28 19:11:48.263068 znsocket-0.1.1/README.md
+-rw-r--r--   0        0        0      777 2024-05-28 19:42:18.959908 znsocket-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       86 2024-05-28 19:53:22.847159 znsocket-0.1.1/znsocket/__init__.py
+-rw-r--r--   0        0        0      804 2024-05-28 19:53:23.205211 znsocket-0.1.1/znsocket/cli.py
+-rw-r--r--   0        0        0     2624 2024-05-28 19:42:34.598325 znsocket-0.1.1/znsocket/client.py
+-rw-r--r--   0        0        0     5294 2024-05-28 19:54:02.627528 znsocket-0.1.1/znsocket/server.py
+-rw-r--r--   0        0        0     2148 1970-01-01 00:00:00.000000 znsocket-0.1.1/PKG-INFO
```

### Comparing `znsocket-0.1.0/LICENSE` & `znsocket-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `znsocket-0.1.0/README.md` & `znsocket-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `znsocket-0.1.0/pyproject.toml` & `znsocket-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "znsocket"
-version = "0.1.0"
+version = "0.1.1"
 description = "Create objects with shared attributes through a socket connection."
 authors = ["Fabian Zills <fzills@icp.uni-stuttgart.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `znsocket-0.1.0/znsocket/client.py` & `znsocket-0.1.1/znsocket/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,9 +74,12 @@
 
     def lrem(self, name: str, count: int, value: str):
         return self.sio.call("lrem", {"name": name, "count": count, "value": value})
 
     def sadd(self, name, value):
         return self.sio.call("sadd", {"name": name, "value": value})
 
+    def srem(self, name, value):
+        return self.sio.call("srem", {"name": name, "value": value})
+
     def flushall(self):
         return self.sio.call("flushall", {})
```

### Comparing `znsocket-0.1.0/PKG-INFO` & `znsocket-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: znsocket
-Version: 0.1.0
+Version: 0.1.1
 Summary: Create objects with shared attributes through a socket connection.
 License: Apache-2.0
 Author: Fabian Zills
 Author-email: fzills@icp.uni-stuttgart.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

