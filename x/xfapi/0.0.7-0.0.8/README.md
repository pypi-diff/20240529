# Comparing `tmp/xfapi-0.0.7.tar.gz` & `tmp/xfapi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfapi-0.0.7.tar", last modified: Wed May 29 07:54:38 2024, max compression
+gzip compressed data, was "xfapi-0.0.8.tar", last modified: Wed May 29 08:01:29 2024, max compression
```

## Comparing `xfapi-0.0.7.tar` & `xfapi-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 07:54:38.424931 xfapi-0.0.7/
--rw-r--r--   0 asia       (501) staff       (20)     1334 2024-05-29 07:54:38.424657 xfapi-0.0.7/PKG-INFO
--rw-r--r--   0 asia       (501) staff       (20)      883 2024-05-29 05:46:51.000000 xfapi-0.0.7/README.md
--rw-r--r--   0 asia       (501) staff       (20)       26 2024-05-29 07:54:23.000000 xfapi-0.0.7/requirements.txt
--rw-r--r--   0 asia       (501) staff       (20)       38 2024-05-29 07:54:38.424986 xfapi-0.0.7/setup.cfg
--rw-r--r--   0 asia       (501) staff       (20)     1393 2024-05-29 07:54:33.000000 xfapi-0.0.7/setup.py
-drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 07:54:38.421997 xfapi-0.0.7/xfapi/
--rw-r--r--   0 asia       (501) staff       (20)       45 2024-05-29 07:44:34.000000 xfapi-0.0.7/xfapi/__init__.py
--rw-r--r--   0 asia       (501) staff       (20)     2980 2024-05-29 07:45:01.000000 xfapi-0.0.7/xfapi/server.py
-drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 07:54:38.423902 xfapi-0.0.7/xfapi/utils/
--rw-r--r--   0 asia       (501) staff       (20)       18 2024-05-29 07:44:50.000000 xfapi-0.0.7/xfapi/utils/__init__.py
--rw-r--r--   0 asia       (501) staff       (20)     1467 2024-05-29 03:49:23.000000 xfapi-0.0.7/xfapi/utils/auth.py
--rw-r--r--   0 asia       (501) staff       (20)     1096 2024-05-29 03:52:36.000000 xfapi-0.0.7/xfapi/utils/load_yaml.py
-drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 07:54:38.424264 xfapi-0.0.7/xfapi.egg-info/
--rw-r--r--   0 asia       (501) staff       (20)     1334 2024-05-29 07:54:38.000000 xfapi-0.0.7/xfapi.egg-info/PKG-INFO
--rw-r--r--   0 asia       (501) staff       (20)      282 2024-05-29 07:54:38.000000 xfapi-0.0.7/xfapi.egg-info/SOURCES.txt
--rw-r--r--   0 asia       (501) staff       (20)        1 2024-05-29 07:54:38.000000 xfapi-0.0.7/xfapi.egg-info/dependency_links.txt
--rw-r--r--   0 asia       (501) staff       (20)       27 2024-05-29 07:54:38.000000 xfapi-0.0.7/xfapi.egg-info/requires.txt
--rw-r--r--   0 asia       (501) staff       (20)        6 2024-05-29 07:54:38.000000 xfapi-0.0.7/xfapi.egg-info/top_level.txt
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 08:01:29.852107 xfapi-0.0.8/
+-rw-r--r--   0 asia       (501) staff       (20)     1327 2024-05-29 08:01:29.851820 xfapi-0.0.8/PKG-INFO
+-rw-r--r--   0 asia       (501) staff       (20)      876 2024-05-29 08:01:15.000000 xfapi-0.0.8/README.md
+-rw-r--r--   0 asia       (501) staff       (20)       26 2024-05-29 07:54:23.000000 xfapi-0.0.8/requirements.txt
+-rw-r--r--   0 asia       (501) staff       (20)       38 2024-05-29 08:01:29.852158 xfapi-0.0.8/setup.cfg
+-rw-r--r--   0 asia       (501) staff       (20)     1393 2024-05-29 08:01:27.000000 xfapi-0.0.8/setup.py
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 08:01:29.849689 xfapi-0.0.8/xfapi/
+-rw-r--r--   0 asia       (501) staff       (20)       45 2024-05-29 07:44:34.000000 xfapi-0.0.8/xfapi/__init__.py
+-rw-r--r--   0 asia       (501) staff       (20)     2980 2024-05-29 07:45:01.000000 xfapi-0.0.8/xfapi/server.py
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 08:01:29.851156 xfapi-0.0.8/xfapi/utils/
+-rw-r--r--   0 asia       (501) staff       (20)       18 2024-05-29 07:44:50.000000 xfapi-0.0.8/xfapi/utils/__init__.py
+-rw-r--r--   0 asia       (501) staff       (20)     1467 2024-05-29 03:49:23.000000 xfapi-0.0.8/xfapi/utils/auth.py
+-rw-r--r--   0 asia       (501) staff       (20)     1096 2024-05-29 03:52:36.000000 xfapi-0.0.8/xfapi/utils/load_yaml.py
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 08:01:29.851552 xfapi-0.0.8/xfapi.egg-info/
+-rw-r--r--   0 asia       (501) staff       (20)     1327 2024-05-29 08:01:29.000000 xfapi-0.0.8/xfapi.egg-info/PKG-INFO
+-rw-r--r--   0 asia       (501) staff       (20)      282 2024-05-29 08:01:29.000000 xfapi-0.0.8/xfapi.egg-info/SOURCES.txt
+-rw-r--r--   0 asia       (501) staff       (20)        1 2024-05-29 08:01:29.000000 xfapi-0.0.8/xfapi.egg-info/dependency_links.txt
+-rw-r--r--   0 asia       (501) staff       (20)       27 2024-05-29 08:01:29.000000 xfapi-0.0.8/xfapi.egg-info/requires.txt
+-rw-r--r--   0 asia       (501) staff       (20)        6 2024-05-29 08:01:29.000000 xfapi-0.0.8/xfapi.egg-info/top_level.txt
```

### Comparing `xfapi-0.0.7/PKG-INFO` & `xfapi-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Apis tool base fastapi
 Home-page: https://pypi.org/project/xfapi/
 Author: Alex_M
 Author-email: asiaier@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,48 +14,47 @@
 Requires-Dist: pyyaml
 Requires-Dist: python-jose
 
 配置文件示例
 
 ```yaml
 apis:
-- name: "token"
-  path: "/token"
-  method: "POST"
-  handler: "apis.handler_token"
+- name: "index"
+  path: "/index"
+  method: "Get"
+  handler: "apis.index"
 
-- name: "p"
-  path: "/p"
-  method: "GET"
-  handler: "apis.p"
+- name: "save"
+  path: "/save"
+  method: "POST"
+  handler: "apis.save"
 
 ```
 
 回调函数示例
 
 ```python
-
 from fastapi import Request
-def handler_token(data:dict):
-    print(data)
-    return {"token": "your_token_here"}
 
-def p(request:Request):
+
+def index(request:Request):
     print(request._query_params._dict)
-    return {"data": "your_token_here"}
+    return {"msg": "this is index msg"}
+
+def save(data:dict):
+    return {"msg": "this is save msg", "data":data}
 ```
 
 
 调用示例
 
 ```python
 from xapi.server import HTTPServer
 
 server = HTTPServer()
-
 server.start()
 
 ```
 
 调用成功 日志
 
 ```log
```

### Comparing `xfapi-0.0.7/README.md` & `xfapi-0.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 配置文件示例
 
 ```yaml
 apis:
-- name: "token"
-  path: "/token"
-  method: "POST"
-  handler: "apis.handler_token"
+- name: "index"
+  path: "/index"
+  method: "Get"
+  handler: "apis.index"
 
-- name: "p"
-  path: "/p"
-  method: "GET"
-  handler: "apis.p"
+- name: "save"
+  path: "/save"
+  method: "POST"
+  handler: "apis.save"
 
 ```
 
 回调函数示例
 
 ```python
-
 from fastapi import Request
-def handler_token(data:dict):
-    print(data)
-    return {"token": "your_token_here"}
 
-def p(request:Request):
+
+def index(request:Request):
     print(request._query_params._dict)
-    return {"data": "your_token_here"}
+    return {"msg": "this is index msg"}
+
+def save(data:dict):
+    return {"msg": "this is save msg", "data":data}
 ```
 
 
 调用示例
 
 ```python
 from xapi.server import HTTPServer
 
 server = HTTPServer()
-
 server.start()
 
 ```
 
 调用成功 日志
 
 ```log
```

### Comparing `xfapi-0.0.7/setup.py` & `xfapi-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
  
 package_name = "xfapi"
  
 
 def get_version():
-   return "0.0.7"
+   return "0.0.8"
  
  
 def upload():
     with open("README.md", "r") as fh:
         long_description = fh.read()
     with open('requirements.txt') as f:
         required = f.read().splitlines()
```

### Comparing `xfapi-0.0.7/xfapi/server.py` & `xfapi-0.0.8/xfapi/server.py`

 * *Files identical despite different names*

### Comparing `xfapi-0.0.7/xfapi/utils/auth.py` & `xfapi-0.0.8/xfapi/utils/auth.py`

 * *Files identical despite different names*

### Comparing `xfapi-0.0.7/xfapi/utils/load_yaml.py` & `xfapi-0.0.8/xfapi/utils/load_yaml.py`

 * *Files identical despite different names*

### Comparing `xfapi-0.0.7/xfapi.egg-info/PKG-INFO` & `xfapi-0.0.8/xfapi.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Apis tool base fastapi
 Home-page: https://pypi.org/project/xfapi/
 Author: Alex_M
 Author-email: asiaier@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,48 +14,47 @@
 Requires-Dist: pyyaml
 Requires-Dist: python-jose
 
 配置文件示例
 
 ```yaml
 apis:
-- name: "token"
-  path: "/token"
-  method: "POST"
-  handler: "apis.handler_token"
+- name: "index"
+  path: "/index"
+  method: "Get"
+  handler: "apis.index"
 
-- name: "p"
-  path: "/p"
-  method: "GET"
-  handler: "apis.p"
+- name: "save"
+  path: "/save"
+  method: "POST"
+  handler: "apis.save"
 
 ```
 
 回调函数示例
 
 ```python
-
 from fastapi import Request
-def handler_token(data:dict):
-    print(data)
-    return {"token": "your_token_here"}
 
-def p(request:Request):
+
+def index(request:Request):
     print(request._query_params._dict)
-    return {"data": "your_token_here"}
+    return {"msg": "this is index msg"}
+
+def save(data:dict):
+    return {"msg": "this is save msg", "data":data}
 ```
 
 
 调用示例
 
 ```python
 from xapi.server import HTTPServer
 
 server = HTTPServer()
-
 server.start()
 
 ```
 
 调用成功 日志
 
 ```log
```

