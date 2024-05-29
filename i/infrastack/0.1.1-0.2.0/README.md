# Comparing `tmp/infrastack-0.1.1.tar.gz` & `tmp/infrastack-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrastack-0.1.1.tar", last modified: Mon May 27 12:12:17 2024, max compression
+gzip compressed data, was "infrastack-0.2.0.tar", last modified: Wed May 29 14:59:48 2024, max compression
```

## Comparing `infrastack-0.1.1.tar` & `infrastack-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:12:17.339905 infrastack-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 12:12:08.000000 infrastack-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 12:12:08.000000 infrastack-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-27 12:12:17.339905 infrastack-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-27 12:12:08.000000 infrastack-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:12:17.339905 infrastack-0.1.1/infrastack/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 12:12:08.000000 infrastack-0.1.1/infrastack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:12:17.339905 infrastack-0.1.1/infrastack/flask/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 12:12:08.000000 infrastack-0.1.1/infrastack/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-27 12:12:08.000000 infrastack-0.1.1/infrastack/flask/flask_instrumentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:12:17.339905 infrastack-0.1.1/infrastack/logs/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-27 12:12:08.000000 infrastack-0.1.1/infrastack/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-27 12:12:08.000000 infrastack-0.1.1/infrastack/logs/log_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:12:17.339905 infrastack-0.1.1/infrastack/tracer/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 12:12:08.000000 infrastack-0.1.1/infrastack/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-27 12:12:08.000000 infrastack-0.1.1/infrastack/tracer/create_tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:12:17.339905 infrastack-0.1.1/infrastack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-27 12:12:16.000000 infrastack-0.1.1/infrastack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-27 12:12:17.000000 infrastack-0.1.1/infrastack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:12:16.000000 infrastack-0.1.1/infrastack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:12:16.000000 infrastack-0.1.1/infrastack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-27 12:12:16.000000 infrastack-0.1.1/infrastack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 12:12:16.000000 infrastack-0.1.1/infrastack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-27 12:12:08.000000 infrastack-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:12:17.339905 infrastack-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-27 12:12:08.000000 infrastack-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:59:48.937849 infrastack-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 14:59:37.000000 infrastack-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 14:59:37.000000 infrastack-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-29 14:59:48.937849 infrastack-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-29 14:59:37.000000 infrastack-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:59:48.933849 infrastack-0.2.0/infrastack/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-29 14:59:37.000000 infrastack-0.2.0/infrastack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:59:48.933849 infrastack-0.2.0/infrastack/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 14:59:37.000000 infrastack-0.2.0/infrastack/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-29 14:59:37.000000 infrastack-0.2.0/infrastack/flask/flask_instrumentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:59:48.937849 infrastack-0.2.0/infrastack/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 14:59:37.000000 infrastack-0.2.0/infrastack/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-29 14:59:37.000000 infrastack-0.2.0/infrastack/logs/log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:59:48.937849 infrastack-0.2.0/infrastack/tracer/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 14:59:37.000000 infrastack-0.2.0/infrastack/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-29 14:59:37.000000 infrastack-0.2.0/infrastack/tracer/create_tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:59:48.933849 infrastack-0.2.0/infrastack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-29 14:59:48.000000 infrastack-0.2.0/infrastack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-29 14:59:48.000000 infrastack-0.2.0/infrastack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:59:48.000000 infrastack-0.2.0/infrastack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:59:48.000000 infrastack-0.2.0/infrastack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-29 14:59:48.000000 infrastack-0.2.0/infrastack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 14:59:48.000000 infrastack-0.2.0/infrastack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-29 14:59:37.000000 infrastack-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:59:48.937849 infrastack-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-29 14:59:37.000000 infrastack-0.2.0/setup.py
```

### Comparing `infrastack-0.1.1/LICENSE` & `infrastack-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `infrastack-0.1.1/PKG-INFO` & `infrastack-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrastack
-Version: 0.1.1
+Version: 0.2.0
 Summary: Empowering Developers with AI-First DevTools
 Home-page: https://github.com/infrastackai/python-sdk
 Author: Infrastack AI
 Author-email: info@infrastack.ai
 License: MIT
 Description: # Introduction
         
@@ -35,15 +35,15 @@
         
         ```python
         from infrastack import FlaskInstrument
         from flask import Flask
         
         app = Flask(__name__)
         
-        FlaskInstrument("your_service_name", app, infrastackai_api_key="your_api_key")
+        FlaskInstrument("your_service_name", app, infrastackai_api_key="your_infrastack_api_key")
         
         @app.route('/')
         def hello_world():
             return 'Hello, World!'
         
         if __name__ == '__main__':
             app.run()
@@ -54,37 +54,63 @@
         To send logs to InfraStack AI, use the following code snippet:
         
         ```python
         from infrastack import LogHandler
         import logging
         
         logger = logging.getLogger(__name__)
-        LogHandler("your_service_name", logger, infrastackai_api_key="your_api_key")
+        LogHandler("your_service_name", logger, infrastackai_api_key="your_infrastack_api_key")
         
         logger.info("TEST")
         ```
         
         ### Tracing
         
         To create and use a tracer with InfraStack AI, use the following code snippet:
         
         ```python
         from infrastack import CreateTracer
         
-        my_tracer = CreateTracer("your_service_name", "trace_name", infrastackai_api_key="your_api_key")
+        my_tracer = CreateTracer("your_service_name", "trace_name", infrastackai_api_key="your_infrastack_api_key")
         
         with my_tracer.start_span("scope-create-version") as span:
             span.set_attribute("version", "0.0.0")
             span.set_attribute("scope", "create-version")
             span.set_attribute("author", "Your Name")
             print("hi")
         ```
         
         
         
+        ### OpenAI Instrument
+        
+        To instrument your OpenAI API calls with InfraStack AI, use the following code snippet:
+        
+        ```python
+        from infrastack import OpenAIInstrument
+        from openai import OpenAI
+        
+        # Initialize OpenAIInstrument
+        instrument = OpenAIInstrument("your_service_name", catch_content=False, infrastackai_api_key="your_infrastack_api_key")
+        
+        # Example OpenAI API call
+        client = OpenAI(api_key="your_openai_api_key")
+        
+        response = client.chat.completions.create(
+            model="gpt-4o",
+            messages=[
+                {"role": "user", "content": [{"type": "text", "text": "Hi"}]}
+            ]
+        )
+        
+        print(response)
+        ```
+        
+        
+        
         ## Note on API Key Configuration
         
         The InfraStack AI SDK provides two methods for configuring your API key:
         
         1. **Passing it as a Parameter**: You can directly pass the `infrastackai_api_key` as a parameter when initializing the Flask instrument, log handler, or tracer.
         
         2. **Environment Variable (.env)**: Alternatively, you can set the `INFRASTACKAI_API_KEY` as an environment variable. If this environment variable is set, the SDK will automatically use it, and you do not need to pass the API key as a parameter.
```

### Comparing `infrastack-0.1.1/README.md` & `infrastack-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ```python
 from infrastack import FlaskInstrument
 from flask import Flask
 
 app = Flask(__name__)
 
-FlaskInstrument("your_service_name", app, infrastackai_api_key="your_api_key")
+FlaskInstrument("your_service_name", app, infrastackai_api_key="your_infrastack_api_key")
 
 @app.route('/')
 def hello_world():
     return 'Hello, World!'
 
 if __name__ == '__main__':
     app.run()
@@ -46,37 +46,63 @@
 To send logs to InfraStack AI, use the following code snippet:
 
 ```python
 from infrastack import LogHandler
 import logging
 
 logger = logging.getLogger(__name__)
-LogHandler("your_service_name", logger, infrastackai_api_key="your_api_key")
+LogHandler("your_service_name", logger, infrastackai_api_key="your_infrastack_api_key")
 
 logger.info("TEST")
 ```
 
 ### Tracing
 
 To create and use a tracer with InfraStack AI, use the following code snippet:
 
 ```python
 from infrastack import CreateTracer
 
-my_tracer = CreateTracer("your_service_name", "trace_name", infrastackai_api_key="your_api_key")
+my_tracer = CreateTracer("your_service_name", "trace_name", infrastackai_api_key="your_infrastack_api_key")
 
 with my_tracer.start_span("scope-create-version") as span:
     span.set_attribute("version", "0.0.0")
     span.set_attribute("scope", "create-version")
     span.set_attribute("author", "Your Name")
     print("hi")
 ```
 
 
 
+### OpenAI Instrument
+
+To instrument your OpenAI API calls with InfraStack AI, use the following code snippet:
+
+```python
+from infrastack import OpenAIInstrument
+from openai import OpenAI
+
+# Initialize OpenAIInstrument
+instrument = OpenAIInstrument("your_service_name", catch_content=False, infrastackai_api_key="your_infrastack_api_key")
+
+# Example OpenAI API call
+client = OpenAI(api_key="your_openai_api_key")
+
+response = client.chat.completions.create(
+    model="gpt-4o",
+    messages=[
+        {"role": "user", "content": [{"type": "text", "text": "Hi"}]}
+    ]
+)
+
+print(response)
+```
+
+
+
 ## Note on API Key Configuration
 
 The InfraStack AI SDK provides two methods for configuring your API key:
 
 1. **Passing it as a Parameter**: You can directly pass the `infrastackai_api_key` as a parameter when initializing the Flask instrument, log handler, or tracer.
 
 2. **Environment Variable (.env)**: Alternatively, you can set the `INFRASTACKAI_API_KEY` as an environment variable. If this environment variable is set, the SDK will automatically use it, and you do not need to pass the API key as a parameter.
```

### Comparing `infrastack-0.1.1/infrastack/flask/flask_instrumentation.py` & `infrastack-0.2.0/infrastack/flask/flask_instrumentation.py`

 * *Files identical despite different names*

### Comparing `infrastack-0.1.1/infrastack/logs/log_handler.py` & `infrastack-0.2.0/infrastack/logs/log_handler.py`

 * *Files identical despite different names*

### Comparing `infrastack-0.1.1/infrastack/tracer/create_tracer.py` & `infrastack-0.2.0/infrastack/tracer/create_tracer.py`

 * *Files identical despite different names*

### Comparing `infrastack-0.1.1/infrastack.egg-info/PKG-INFO` & `infrastack-0.2.0/infrastack.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrastack
-Version: 0.1.1
+Version: 0.2.0
 Summary: Empowering Developers with AI-First DevTools
 Home-page: https://github.com/infrastackai/python-sdk
 Author: Infrastack AI
 Author-email: info@infrastack.ai
 License: MIT
 Description: # Introduction
         
@@ -35,15 +35,15 @@
         
         ```python
         from infrastack import FlaskInstrument
         from flask import Flask
         
         app = Flask(__name__)
         
-        FlaskInstrument("your_service_name", app, infrastackai_api_key="your_api_key")
+        FlaskInstrument("your_service_name", app, infrastackai_api_key="your_infrastack_api_key")
         
         @app.route('/')
         def hello_world():
             return 'Hello, World!'
         
         if __name__ == '__main__':
             app.run()
@@ -54,37 +54,63 @@
         To send logs to InfraStack AI, use the following code snippet:
         
         ```python
         from infrastack import LogHandler
         import logging
         
         logger = logging.getLogger(__name__)
-        LogHandler("your_service_name", logger, infrastackai_api_key="your_api_key")
+        LogHandler("your_service_name", logger, infrastackai_api_key="your_infrastack_api_key")
         
         logger.info("TEST")
         ```
         
         ### Tracing
         
         To create and use a tracer with InfraStack AI, use the following code snippet:
         
         ```python
         from infrastack import CreateTracer
         
-        my_tracer = CreateTracer("your_service_name", "trace_name", infrastackai_api_key="your_api_key")
+        my_tracer = CreateTracer("your_service_name", "trace_name", infrastackai_api_key="your_infrastack_api_key")
         
         with my_tracer.start_span("scope-create-version") as span:
             span.set_attribute("version", "0.0.0")
             span.set_attribute("scope", "create-version")
             span.set_attribute("author", "Your Name")
             print("hi")
         ```
         
         
         
+        ### OpenAI Instrument
+        
+        To instrument your OpenAI API calls with InfraStack AI, use the following code snippet:
+        
+        ```python
+        from infrastack import OpenAIInstrument
+        from openai import OpenAI
+        
+        # Initialize OpenAIInstrument
+        instrument = OpenAIInstrument("your_service_name", catch_content=False, infrastackai_api_key="your_infrastack_api_key")
+        
+        # Example OpenAI API call
+        client = OpenAI(api_key="your_openai_api_key")
+        
+        response = client.chat.completions.create(
+            model="gpt-4o",
+            messages=[
+                {"role": "user", "content": [{"type": "text", "text": "Hi"}]}
+            ]
+        )
+        
+        print(response)
+        ```
+        
+        
+        
         ## Note on API Key Configuration
         
         The InfraStack AI SDK provides two methods for configuring your API key:
         
         1. **Passing it as a Parameter**: You can directly pass the `infrastackai_api_key` as a parameter when initializing the Flask instrument, log handler, or tracer.
         
         2. **Environment Variable (.env)**: Alternatively, you can set the `INFRASTACKAI_API_KEY` as an environment variable. If this environment variable is set, the SDK will automatically use it, and you do not need to pass the API key as a parameter.
```

### Comparing `infrastack-0.1.1/setup.py` & `infrastack-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 
 with open('requirements.txt') as fp:
     install_requires = fp.read()
 setup(
     name="infrastack",
-    version="0.1.1",
+    version="0.2.0",
     description="""Empowering Developers with AI-First DevTools""",
     long_description="".join(open("README.md", encoding="utf-8").readlines()),
     long_description_content_type="text/markdown",
     url="https://github.com/infrastackai/python-sdk",
     author="Infrastack AI",
     author_email="info@infrastack.ai",
     license="MIT",
```

