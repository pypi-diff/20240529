# Comparing `tmp/vaul-0.1.1.tar.gz` & `tmp/vaul-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaul-0.1.1.tar", last modified: Wed May 29 00:59:40 2024, max compression
+gzip compressed data, was "vaul-0.1.2.tar", last modified: Wed May 29 15:36:35 2024, max compression
```

## Comparing `vaul-0.1.1.tar` & `vaul-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-29 00:59:40.011466 vaul-0.1.1/
--rw-r--r--   0 sporter    (501) staff       (20)    34599 2024-05-29 00:30:50.000000 vaul-0.1.1/LICENSE.txt
--rw-r--r--   0 sporter    (501) staff       (20)       33 2024-05-29 00:36:56.000000 vaul-0.1.1/MANIFEST.in
--rw-r--r--   0 sporter    (501) staff       (20)     3871 2024-05-29 00:59:40.011402 vaul-0.1.1/PKG-INFO
--rw-r--r--   0 sporter    (501) staff       (20)     3579 2024-05-29 00:33:47.000000 vaul-0.1.1/README.md
--rw-r--r--   0 sporter    (501) staff       (20)       79 2024-05-29 00:59:40.011676 vaul-0.1.1/setup.cfg
--rw-r--r--   0 sporter    (501) staff       (20)      524 2024-05-29 00:56:32.000000 vaul-0.1.1/setup.py
-drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-29 00:59:40.010550 vaul-0.1.1/vaul/
--rw-r--r--   0 sporter    (501) staff       (20)     5013 2024-05-29 00:56:32.000000 vaul-0.1.1/vaul/__init__.py
--rw-r--r--   0 sporter    (501) staff       (20)     1312 2024-05-28 23:32:45.000000 vaul-0.1.1/vaul/ctx.py
--rw-r--r--   0 sporter    (501) staff       (20)      228 2024-05-28 17:31:12.000000 vaul-0.1.1/vaul/enums.py
--rw-r--r--   0 sporter    (501) staff       (20)     1235 2024-05-28 18:02:10.000000 vaul-0.1.1/vaul/helpers.py
--rw-r--r--   0 sporter    (501) staff       (20)      987 2024-05-28 15:31:29.000000 vaul-0.1.1/vaul/logging.py
--rw-r--r--   0 sporter    (501) staff       (20)     3211 2024-05-28 23:55:58.000000 vaul-0.1.1/vaul/models.py
--rw-r--r--   0 sporter    (501) staff       (20)     1119 2024-05-28 14:55:24.000000 vaul-0.1.1/vaul/request.py
-drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-29 00:59:40.011176 vaul-0.1.1/vaul.egg-info/
--rw-r--r--   0 sporter    (501) staff       (20)     3871 2024-05-29 00:59:39.000000 vaul-0.1.1/vaul.egg-info/PKG-INFO
--rw-r--r--   0 sporter    (501) staff       (20)      297 2024-05-29 00:59:39.000000 vaul-0.1.1/vaul.egg-info/SOURCES.txt
--rw-r--r--   0 sporter    (501) staff       (20)        1 2024-05-29 00:59:39.000000 vaul-0.1.1/vaul.egg-info/dependency_links.txt
--rw-r--r--   0 sporter    (501) staff       (20)       16 2024-05-29 00:59:39.000000 vaul-0.1.1/vaul.egg-info/requires.txt
--rw-r--r--   0 sporter    (501) staff       (20)        5 2024-05-29 00:59:39.000000 vaul-0.1.1/vaul.egg-info/top_level.txt
+drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-29 15:36:35.685207 vaul-0.1.2/
+-rw-r--r--   0 sporter    (501) staff       (20)    34599 2024-05-29 00:30:50.000000 vaul-0.1.2/LICENSE.txt
+-rw-r--r--   0 sporter    (501) staff       (20)       33 2024-05-29 00:36:56.000000 vaul-0.1.2/MANIFEST.in
+-rw-r--r--   0 sporter    (501) staff       (20)     3859 2024-05-29 15:36:35.685138 vaul-0.1.2/PKG-INFO
+-rw-r--r--   0 sporter    (501) staff       (20)     3567 2024-05-29 13:35:57.000000 vaul-0.1.2/README.md
+-rw-r--r--   0 sporter    (501) staff       (20)       79 2024-05-29 15:36:35.685411 vaul-0.1.2/setup.cfg
+-rw-r--r--   0 sporter    (501) staff       (20)      524 2024-05-29 15:36:33.000000 vaul-0.1.2/setup.py
+drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-29 15:36:35.684218 vaul-0.1.2/vaul/
+-rw-r--r--   0 sporter    (501) staff       (20)     5018 2024-05-29 13:30:39.000000 vaul-0.1.2/vaul/__init__.py
+-rw-r--r--   0 sporter    (501) staff       (20)     1312 2024-05-28 23:32:45.000000 vaul-0.1.2/vaul/ctx.py
+-rw-r--r--   0 sporter    (501) staff       (20)      228 2024-05-28 17:31:12.000000 vaul-0.1.2/vaul/enums.py
+-rw-r--r--   0 sporter    (501) staff       (20)     1235 2024-05-28 18:02:10.000000 vaul-0.1.2/vaul/helpers.py
+-rw-r--r--   0 sporter    (501) staff       (20)      987 2024-05-28 15:31:29.000000 vaul-0.1.2/vaul/logging.py
+-rw-r--r--   0 sporter    (501) staff       (20)     5891 2024-05-29 15:34:29.000000 vaul-0.1.2/vaul/models.py
+-rw-r--r--   0 sporter    (501) staff       (20)     1119 2024-05-28 14:55:24.000000 vaul-0.1.2/vaul/request.py
+drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-29 15:36:35.684918 vaul-0.1.2/vaul.egg-info/
+-rw-r--r--   0 sporter    (501) staff       (20)     3859 2024-05-29 15:36:35.000000 vaul-0.1.2/vaul.egg-info/PKG-INFO
+-rw-r--r--   0 sporter    (501) staff       (20)      297 2024-05-29 15:36:35.000000 vaul-0.1.2/vaul.egg-info/SOURCES.txt
+-rw-r--r--   0 sporter    (501) staff       (20)        1 2024-05-29 15:36:35.000000 vaul-0.1.2/vaul.egg-info/dependency_links.txt
+-rw-r--r--   0 sporter    (501) staff       (20)       16 2024-05-29 15:36:35.000000 vaul-0.1.2/vaul.egg-info/requires.txt
+-rw-r--r--   0 sporter    (501) staff       (20)        5 2024-05-29 15:36:35.000000 vaul-0.1.2/vaul.egg-info/top_level.txt
```

### Comparing `vaul-0.1.1/LICENSE.txt` & `vaul-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vaul-0.1.1/PKG-INFO` & `vaul-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: vaul
-Version: 0.1.1
-Summary: A nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs.
-Author: Spencer Porter
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: pydantic==2.6.4
-
 # Vaul
 
 Vaul is a nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs. It provides seamless integration with OpenAPI Schema and allows for monitoring and managing microservices with ease.
 
 ## Table of Contents
 
 - [Introduction](#introduction)
@@ -58,27 +48,30 @@
 
 app = Vaul()
 
 @app.action(path='/hello', method="GET")
 def hello(name: str) -> str:
     return f"Hello, {name}!"
 
-@app.action(path='/echo', method="POST)
+@app.action(path='/echo', method="POST")
 def echo(data: dict) -> dict:
     return data
 
 def handler(event, context):
-    return app.handler(event, context)
+    return app.handler(event)
 ```
 
+### Deploying to AWS Lambda
+To deploy your Vaul application to AWS Lambda, use the AWS CLI or AWS Management Console. Ensure that your Lambda function's handler is set to the appropriate entry point (e.g., handler).
+
 ### Using OpenAPI Schema
 Vaul automatically generates an OpenAPI schema for your API based on the defined actions. You can access the schema by visiting the `/openapi` endpoint.
 
 ```curl
-curl -X GET https://your-function-url/openapi
+curl -X GET https://your-function-url/openapi.json
 ```
 
 ### Accessing Request Data
 You can access the request data (e.g., query parameters, headers, body) using the `get_request` function:
 
 ```python
 from vaul import Vaul, get_request
@@ -88,20 +81,17 @@
 @app.action(path='/hello', method="GET")
 def hello() -> str:
     request = get_request()
     user_agent = request.headers.get('User-Agent')
     return f"Hello, {user_agent}!"
     
 def handler(event, context):
-    return app.handler(event, context)
+    return app.handler(event)
 ```
 
-### Deploying to AWS Lambda
-To deploy your Vaul application to AWS Lambda, use the AWS CLI or AWS Management Console. Ensure that your Lambda function's handler is set to the appropriate entry point (e.g., handler).
-
 ### Handling Requests
 Vaul's middleware automatically handles incoming requests, validates them, and routes them to the appropriate action based on the request path and method.
 
 ## Contributing
 We welcome contributions from the community! If you would like to contribute to Vaul, please follow these steps:
 
 1. Fork the repository.
```

### Comparing `vaul-0.1.1/README.md` & `vaul-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: vaul
+Version: 0.1.2
+Summary: A nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs.
+Author: Spencer Porter
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: pydantic==2.6.4
+
 # Vaul
 
 Vaul is a nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs. It provides seamless integration with OpenAPI Schema and allows for monitoring and managing microservices with ease.
 
 ## Table of Contents
 
 - [Introduction](#introduction)
@@ -48,27 +58,30 @@
 
 app = Vaul()
 
 @app.action(path='/hello', method="GET")
 def hello(name: str) -> str:
     return f"Hello, {name}!"
 
-@app.action(path='/echo', method="POST)
+@app.action(path='/echo', method="POST")
 def echo(data: dict) -> dict:
     return data
 
 def handler(event, context):
-    return app.handler(event, context)
+    return app.handler(event)
 ```
 
+### Deploying to AWS Lambda
+To deploy your Vaul application to AWS Lambda, use the AWS CLI or AWS Management Console. Ensure that your Lambda function's handler is set to the appropriate entry point (e.g., handler).
+
 ### Using OpenAPI Schema
 Vaul automatically generates an OpenAPI schema for your API based on the defined actions. You can access the schema by visiting the `/openapi` endpoint.
 
 ```curl
-curl -X GET https://your-function-url/openapi
+curl -X GET https://your-function-url/openapi.json
 ```
 
 ### Accessing Request Data
 You can access the request data (e.g., query parameters, headers, body) using the `get_request` function:
 
 ```python
 from vaul import Vaul, get_request
@@ -78,20 +91,17 @@
 @app.action(path='/hello', method="GET")
 def hello() -> str:
     request = get_request()
     user_agent = request.headers.get('User-Agent')
     return f"Hello, {user_agent}!"
     
 def handler(event, context):
-    return app.handler(event, context)
+    return app.handler(event)
 ```
 
-### Deploying to AWS Lambda
-To deploy your Vaul application to AWS Lambda, use the AWS CLI or AWS Management Console. Ensure that your Lambda function's handler is set to the appropriate entry point (e.g., handler).
-
 ### Handling Requests
 Vaul's middleware automatically handles incoming requests, validates them, and routes them to the appropriate action based on the request path and method.
 
 ## Contributing
 We welcome contributions from the community! If you would like to contribute to Vaul, please follow these steps:
 
 1. Fork the repository.
```

### Comparing `vaul-0.1.1/setup.py` & `vaul-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="vaul",
-    version="0.1.1",
+    version="0.1.2",
     description="A nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs.",
     author="Spencer Porter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'pydantic==2.6.4',
     ],
```

### Comparing `vaul-0.1.1/vaul/__init__.py` & `vaul-0.1.2/vaul/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             return self._response(404, f"Path or method not found: {path}, {method}", method)
 
         return route_handler(request)
 
     def _get_route_handler(self, path, method, domain_name):
         if path == '/' and method == RequestMethod.GET:
             return lambda _: self._response(200, self.handle_base_path(), method)
-        if path == '/openapi' and method == RequestMethod.GET:
+        if path == '/openapi.json' and method == RequestMethod.GET:
             return lambda _: self._response(200, self.handle_openapi_request(domain_name), method)
         if method == RequestMethod.OPTIONS:
             return lambda _: self._response(200, self.handle_options_request(), method)
         if path in self.routes and method in self.routes[path]:
             return lambda request: self._run_action(request, path, method)
         return None
```

### Comparing `vaul-0.1.1/vaul/ctx.py` & `vaul-0.1.2/vaul/ctx.py`

 * *Files identical despite different names*

### Comparing `vaul-0.1.1/vaul/helpers.py` & `vaul-0.1.2/vaul/helpers.py`

 * *Files identical despite different names*

### Comparing `vaul-0.1.1/vaul/logging.py` & `vaul-0.1.2/vaul/logging.py`

 * *Files identical despite different names*

### Comparing `vaul-0.1.1/vaul/request.py` & `vaul-0.1.2/vaul/request.py`

 * *Files identical despite different names*

### Comparing `vaul-0.1.1/vaul.egg-info/PKG-INFO` & `vaul-0.1.2/vaul.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaul
-Version: 0.1.1
+Version: 0.1.2
 Summary: A nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs.
 Author: Spencer Porter
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pydantic==2.6.4
 
@@ -58,27 +58,30 @@
 
 app = Vaul()
 
 @app.action(path='/hello', method="GET")
 def hello(name: str) -> str:
     return f"Hello, {name}!"
 
-@app.action(path='/echo', method="POST)
+@app.action(path='/echo', method="POST")
 def echo(data: dict) -> dict:
     return data
 
 def handler(event, context):
-    return app.handler(event, context)
+    return app.handler(event)
 ```
 
+### Deploying to AWS Lambda
+To deploy your Vaul application to AWS Lambda, use the AWS CLI or AWS Management Console. Ensure that your Lambda function's handler is set to the appropriate entry point (e.g., handler).
+
 ### Using OpenAPI Schema
 Vaul automatically generates an OpenAPI schema for your API based on the defined actions. You can access the schema by visiting the `/openapi` endpoint.
 
 ```curl
-curl -X GET https://your-function-url/openapi
+curl -X GET https://your-function-url/openapi.json
 ```
 
 ### Accessing Request Data
 You can access the request data (e.g., query parameters, headers, body) using the `get_request` function:
 
 ```python
 from vaul import Vaul, get_request
@@ -88,20 +91,17 @@
 @app.action(path='/hello', method="GET")
 def hello() -> str:
     request = get_request()
     user_agent = request.headers.get('User-Agent')
     return f"Hello, {user_agent}!"
     
 def handler(event, context):
-    return app.handler(event, context)
+    return app.handler(event)
 ```
 
-### Deploying to AWS Lambda
-To deploy your Vaul application to AWS Lambda, use the AWS CLI or AWS Management Console. Ensure that your Lambda function's handler is set to the appropriate entry point (e.g., handler).
-
 ### Handling Requests
 Vaul's middleware automatically handles incoming requests, validates them, and routes them to the appropriate action based on the request path and method.
 
 ## Contributing
 We welcome contributions from the community! If you would like to contribute to Vaul, please follow these steps:
 
 1. Fork the repository.
```

