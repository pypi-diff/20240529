# Comparing `tmp/xfapi-0.0.8.tar.gz` & `tmp/xfapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfapi-0.0.8.tar", last modified: Wed May 29 08:01:29 2024, max compression
+gzip compressed data, was "xfapi-0.0.9.tar", last modified: Wed May 29 09:04:07 2024, max compression
```

## Comparing `xfapi-0.0.8.tar` & `xfapi-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 08:01:29.852107 xfapi-0.0.8/
--rw-r--r--   0 asia       (501) staff       (20)     1327 2024-05-29 08:01:29.851820 xfapi-0.0.8/PKG-INFO
--rw-r--r--   0 asia       (501) staff       (20)      876 2024-05-29 08:01:15.000000 xfapi-0.0.8/README.md
--rw-r--r--   0 asia       (501) staff       (20)       26 2024-05-29 07:54:23.000000 xfapi-0.0.8/requirements.txt
--rw-r--r--   0 asia       (501) staff       (20)       38 2024-05-29 08:01:29.852158 xfapi-0.0.8/setup.cfg
--rw-r--r--   0 asia       (501) staff       (20)     1393 2024-05-29 08:01:27.000000 xfapi-0.0.8/setup.py
-drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 08:01:29.849689 xfapi-0.0.8/xfapi/
--rw-r--r--   0 asia       (501) staff       (20)       45 2024-05-29 07:44:34.000000 xfapi-0.0.8/xfapi/__init__.py
--rw-r--r--   0 asia       (501) staff       (20)     2980 2024-05-29 07:45:01.000000 xfapi-0.0.8/xfapi/server.py
-drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 08:01:29.851156 xfapi-0.0.8/xfapi/utils/
--rw-r--r--   0 asia       (501) staff       (20)       18 2024-05-29 07:44:50.000000 xfapi-0.0.8/xfapi/utils/__init__.py
--rw-r--r--   0 asia       (501) staff       (20)     1467 2024-05-29 03:49:23.000000 xfapi-0.0.8/xfapi/utils/auth.py
--rw-r--r--   0 asia       (501) staff       (20)     1096 2024-05-29 03:52:36.000000 xfapi-0.0.8/xfapi/utils/load_yaml.py
-drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 08:01:29.851552 xfapi-0.0.8/xfapi.egg-info/
--rw-r--r--   0 asia       (501) staff       (20)     1327 2024-05-29 08:01:29.000000 xfapi-0.0.8/xfapi.egg-info/PKG-INFO
--rw-r--r--   0 asia       (501) staff       (20)      282 2024-05-29 08:01:29.000000 xfapi-0.0.8/xfapi.egg-info/SOURCES.txt
--rw-r--r--   0 asia       (501) staff       (20)        1 2024-05-29 08:01:29.000000 xfapi-0.0.8/xfapi.egg-info/dependency_links.txt
--rw-r--r--   0 asia       (501) staff       (20)       27 2024-05-29 08:01:29.000000 xfapi-0.0.8/xfapi.egg-info/requires.txt
--rw-r--r--   0 asia       (501) staff       (20)        6 2024-05-29 08:01:29.000000 xfapi-0.0.8/xfapi.egg-info/top_level.txt
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 09:04:07.550995 xfapi-0.0.9/
+-rw-r--r--   0 asia       (501) staff       (20)     3389 2024-05-29 09:04:07.550778 xfapi-0.0.9/PKG-INFO
+-rw-r--r--   0 asia       (501) staff       (20)     2937 2024-05-29 09:03:43.000000 xfapi-0.0.9/README.md
+-rw-r--r--   0 asia       (501) staff       (20)       26 2024-05-29 07:54:23.000000 xfapi-0.0.9/requirements.txt
+-rw-r--r--   0 asia       (501) staff       (20)       38 2024-05-29 09:04:07.551044 xfapi-0.0.9/setup.cfg
+-rw-r--r--   0 asia       (501) staff       (20)     1393 2024-05-29 09:03:50.000000 xfapi-0.0.9/setup.py
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 09:04:07.548544 xfapi-0.0.9/xfapi/
+-rw-r--r--   0 asia       (501) staff       (20)       45 2024-05-29 07:44:34.000000 xfapi-0.0.9/xfapi/__init__.py
+-rw-r--r--   0 asia       (501) staff       (20)     3371 2024-05-29 08:51:09.000000 xfapi-0.0.9/xfapi/server.py
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 09:04:07.550180 xfapi-0.0.9/xfapi/utils/
+-rw-r--r--   0 asia       (501) staff       (20)       18 2024-05-29 07:44:50.000000 xfapi-0.0.9/xfapi/utils/__init__.py
+-rw-r--r--   0 asia       (501) staff       (20)     3006 2024-05-29 08:54:05.000000 xfapi-0.0.9/xfapi/utils/auth.py
+-rw-r--r--   0 asia       (501) staff       (20)     1096 2024-05-29 03:52:36.000000 xfapi-0.0.9/xfapi/utils/load_yaml.py
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 09:04:07.550536 xfapi-0.0.9/xfapi.egg-info/
+-rw-r--r--   0 asia       (501) staff       (20)     3389 2024-05-29 09:04:07.000000 xfapi-0.0.9/xfapi.egg-info/PKG-INFO
+-rw-r--r--   0 asia       (501) staff       (20)      282 2024-05-29 09:04:07.000000 xfapi-0.0.9/xfapi.egg-info/SOURCES.txt
+-rw-r--r--   0 asia       (501) staff       (20)        1 2024-05-29 09:04:07.000000 xfapi-0.0.9/xfapi.egg-info/dependency_links.txt
+-rw-r--r--   0 asia       (501) staff       (20)       27 2024-05-29 09:04:07.000000 xfapi-0.0.9/xfapi.egg-info/requires.txt
+-rw-r--r--   0 asia       (501) staff       (20)        6 2024-05-29 09:04:07.000000 xfapi-0.0.9/xfapi.egg-info/top_level.txt
```

### Comparing `xfapi-0.0.8/setup.py` & `xfapi-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
  
 package_name = "xfapi"
  
 
 def get_version():
-   return "0.0.8"
+   return "0.0.9"
  
  
 def upload():
     with open("README.md", "r") as fh:
         long_description = fh.read()
     with open('requirements.txt') as f:
         required = f.read().splitlines()
```

### Comparing `xfapi-0.0.8/xfapi/server.py` & `xfapi-0.0.9/xfapi/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,53 @@
-from fastapi import FastAPI, APIRouter  
+from fastapi import FastAPI, APIRouter ,Request
+from fastapi.responses import JSONResponse
 import uvicorn  
 from .utils.load_yaml import YamlConfig  
 import os  
 import importlib  
 import logging  
-  
+
 logging.basicConfig(level=logging.INFO)  
 logger = logging.getLogger(__name__)  
   
 class HTTPServer:  
-    def __init__(self, host="0.0.0.0", port=8000, config_path="api.yaml"):  
+    def __init__(self, host="0.0.0.0", port=8000, config_path="api.yaml", auth_middleware=None):  
         self.host = host  
         self.port = port  
         self.app = FastAPI()  
         self.router = APIRouter()  
-        self.config_path = config_path  
+        self.config_path = config_path 
+        self.auth_middleware = auth_middleware
   
     def call_func(self, modle_name: str, func_name: str) -> callable:  
         try:  
             module = importlib.import_module(modle_name)  
             func = getattr(module, func_name)  
             if callable(func):  
                 return func  
             else:  
                 raise ValueError(f"函数 {func_name} 在模块 {modle_name} 中不可调用")  
         except Exception as e:  
             raise ImportError(f"导入模块 {modle_name} 或获取函数 {func_name} 时出错: {e}")  
-  
+    
     def register_routes(self):  
         if not os.path.exists(self.config_path):  
             logger.error("api.yaml文件不存在，请先创建该文件")  
             return  
-          
         try:  
             self.apis = YamlConfig(self.config_path).get_configs().get("apis")  
             if not self.apis:  
                 logger.error("api.yaml文件格式错误，请检查")  
                 return  
-              
+            # 注册中间件
+            if self.auth_middleware:
+                if callable(self.auth_middleware):  
+                    self.app.middleware("http")(self.auth_middleware)
+                else:
+                    logger.error("auth_middleware 必须是一个可调用的函数")
             for api in self.apis:  
                 logger.info(f"""注册路由: {api.get("path")} {api.get("method")} -> {api.get("handler")}""")
                 modle_path = ".".join(api.get("handler").split(".")[:-1])  
                 func_name = api.get("handler").split(".")[-1]  
                 try:  
                     func = self.call_func(modle_path, func_name)  
                 except Exception as e:  
@@ -65,7 +71,8 @@
         except Exception as e:  
             logger.error(f"注册路由时出错: {e}")  
   
     def start(self):  
         self.register_routes()  
         uvicorn.run(self.app, host=self.host, port=self.port)  
   
+
```

### Comparing `xfapi-0.0.8/xfapi/utils/load_yaml.py` & `xfapi-0.0.9/xfapi/utils/load_yaml.py`

 * *Files identical despite different names*

