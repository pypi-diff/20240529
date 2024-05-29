# Comparing `tmp/fridaylabs-0.1.6.tar.gz` & `tmp/fridaylabs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fridaylabs-0.1.6.tar", last modified: Wed May 29 19:30:15 2024, max compression
+gzip compressed data, was "fridaylabs-0.1.7.tar", last modified: Wed May 29 19:34:33 2024, max compression
```

## Comparing `fridaylabs-0.1.6.tar` & `fridaylabs-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 19:30:15.516070 fridaylabs-0.1.6/
--rw-r--r--   0 ricky      (501) staff       (20)     1070 2024-05-21 04:23:26.000000 fridaylabs-0.1.6/LICENSE
--rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-29 19:30:15.515770 fridaylabs-0.1.6/PKG-INFO
--rw-r--r--   0 ricky      (501) staff       (20)      792 2024-05-21 05:35:31.000000 fridaylabs-0.1.6/README.md
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 19:30:15.514372 fridaylabs-0.1.6/fridaylabs/
--rw-r--r--   0 ricky      (501) staff       (20)       61 2024-05-21 05:49:44.000000 fridaylabs-0.1.6/fridaylabs/__init__.py
--rw-r--r--   0 ricky      (501) staff       (20)     4871 2024-05-29 19:29:27.000000 fridaylabs-0.1.6/fridaylabs/fridaylabs.py
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 19:30:15.515502 fridaylabs-0.1.6/fridaylabs.egg-info/
--rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-29 19:30:15.000000 fridaylabs-0.1.6/fridaylabs.egg-info/PKG-INFO
--rw-r--r--   0 ricky      (501) staff       (20)      243 2024-05-29 19:30:15.000000 fridaylabs-0.1.6/fridaylabs.egg-info/SOURCES.txt
--rw-r--r--   0 ricky      (501) staff       (20)        1 2024-05-29 19:30:15.000000 fridaylabs-0.1.6/fridaylabs.egg-info/dependency_links.txt
--rw-r--r--   0 ricky      (501) staff       (20)        9 2024-05-29 19:30:15.000000 fridaylabs-0.1.6/fridaylabs.egg-info/requires.txt
--rw-r--r--   0 ricky      (501) staff       (20)       11 2024-05-29 19:30:15.000000 fridaylabs-0.1.6/fridaylabs.egg-info/top_level.txt
--rw-r--r--   0 ricky      (501) staff       (20)       38 2024-05-29 19:30:15.516122 fridaylabs-0.1.6/setup.cfg
--rw-r--r--   0 ricky      (501) staff       (20)      693 2024-05-29 19:29:54.000000 fridaylabs-0.1.6/setup.py
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 19:34:33.944670 fridaylabs-0.1.7/
+-rw-r--r--   0 ricky      (501) staff       (20)     1070 2024-05-21 04:23:26.000000 fridaylabs-0.1.7/LICENSE
+-rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-29 19:34:33.944423 fridaylabs-0.1.7/PKG-INFO
+-rw-r--r--   0 ricky      (501) staff       (20)      792 2024-05-21 05:35:31.000000 fridaylabs-0.1.7/README.md
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 19:34:33.942972 fridaylabs-0.1.7/fridaylabs/
+-rw-r--r--   0 ricky      (501) staff       (20)       61 2024-05-21 05:49:44.000000 fridaylabs-0.1.7/fridaylabs/__init__.py
+-rw-r--r--   0 ricky      (501) staff       (20)     5613 2024-05-29 19:34:18.000000 fridaylabs-0.1.7/fridaylabs/fridaylabs.py
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 19:34:33.944165 fridaylabs-0.1.7/fridaylabs.egg-info/
+-rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-29 19:34:33.000000 fridaylabs-0.1.7/fridaylabs.egg-info/PKG-INFO
+-rw-r--r--   0 ricky      (501) staff       (20)      243 2024-05-29 19:34:33.000000 fridaylabs-0.1.7/fridaylabs.egg-info/SOURCES.txt
+-rw-r--r--   0 ricky      (501) staff       (20)        1 2024-05-29 19:34:33.000000 fridaylabs-0.1.7/fridaylabs.egg-info/dependency_links.txt
+-rw-r--r--   0 ricky      (501) staff       (20)        9 2024-05-29 19:34:33.000000 fridaylabs-0.1.7/fridaylabs.egg-info/requires.txt
+-rw-r--r--   0 ricky      (501) staff       (20)       11 2024-05-29 19:34:33.000000 fridaylabs-0.1.7/fridaylabs.egg-info/top_level.txt
+-rw-r--r--   0 ricky      (501) staff       (20)       38 2024-05-29 19:34:33.944728 fridaylabs-0.1.7/setup.cfg
+-rw-r--r--   0 ricky      (501) staff       (20)      693 2024-05-29 19:34:33.000000 fridaylabs-0.1.7/setup.py
```

### Comparing `fridaylabs-0.1.6/LICENSE` & `fridaylabs-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.6/PKG-INFO` & `fridaylabs-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fridaylabs
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package to interact with FridayLabs AI API
 Home-page: https://github.com/ImJustRicky/fridaylabs-package
 Author: FridayLabs
 Author-email: fridaylabs@fridaylabs.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fridaylabs-0.1.6/README.md` & `fridaylabs-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.6/fridaylabs/fridaylabs.py` & `fridaylabs-0.1.7/fridaylabs/fridaylabs.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,38 +12,43 @@
 
 class FridayLabs:
     def __init__(self, api_key, api_url, verbose=False):
         self.api_key = api_key
         self.api_url = api_url
         self.verbose = verbose
 
-    def chat_completion(self, model, messages, temperature=1.0, max_tokens=256, top_p=1.0, frequency_penalty=0.0, presence_penalty=0.0):
+    def chat_completion(self, model, messages, temperature=1.0, max_tokens=256, top_p=1.0, frequency_penalty=0.0, presence_penalty=0.0, stream=False):
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json"
         }
         payload = {
             "model": model,
             "messages": messages,
             "temperature": temperature,
             "max_tokens": max_tokens,
             "top_p": top_p,
             "frequency_penalty": frequency_penalty,
-            "presence_penalty": presence_penalty
+            "presence_penalty": presence_penalty,
+            "stream": stream
         }
 
         if self.verbose:
             print(f"{Colors.HEADER}{Colors.BOLD}Sending Request to FridayLabs API...{Colors.ENDC}")
 
         try:
-            response = requests.post(self.api_url, headers=headers, json=payload)
+            response = requests.post(self.api_url, headers=headers, json=payload, stream=stream)
             response.raise_for_status()
             if self.verbose:
                 print(f"{Colors.OKGREEN}{Colors.BOLD}Request successful!{Colors.ENDC}")
-            return response.json()
+
+            if stream:
+                return self._handle_streaming_response(response)
+            else:
+                return response.json()
 
         except requests.exceptions.HTTPError as http_err:
             if self.verbose:
                 print(f"{Colors.FAIL}{Colors.BOLD}HTTP error occurred: {Colors.ENDC}{http_err}")
                 self.suggest_solution(response)
             if response.status_code == 403:
                 return {"error": "Access to this model is restricted. Please check your access rights."}
@@ -63,14 +68,28 @@
                 print(f"{Colors.FAIL}{Colors.BOLD}An unexpected error occurred: {Colors.ENDC}{err}")
                 print(f"{Colors.WARNING}Possible solutions:{Colors.ENDC}")
                 print(f"{Colors.WARNING}1. Check the payload for correctness.{Colors.ENDC}")
                 print(f"{Colors.WARNING}2. Verify the API endpoint is correct.{Colors.ENDC}")
                 print(f"{Colors.WARNING}3. Ensure the server is running and accessible.{Colors.ENDC}")
             raise
 
+    def _handle_streaming_response(self, response):
+        response_text = ""
+        try:
+            for chunk in response.iter_lines():
+                if chunk:
+                    decoded_chunk = chunk.decode('utf-8')
+                    response_text += decoded_chunk
+                    print(f"{Colors.OKBLUE}{decoded_chunk}{Colors.ENDC}", end='', flush=True)
+        except Exception as e:
+            if self.verbose:
+                print(f"{Colors.FAIL}{Colors.BOLD}Streaming error occurred: {Colors.ENDC}{e}")
+            raise
+        return response_text
+
     def suggest_solution(self, response):
         if self.verbose:
             print(f"{Colors.FAIL}Response content: {response.content}{Colors.ENDC}")
 
             status_code = response.status_code
             if status_code == 400:
                 print(f"{Colors.WARNING}Possible solutions:{Colors.ENDC}")
```

### Comparing `fridaylabs-0.1.6/fridaylabs.egg-info/PKG-INFO` & `fridaylabs-0.1.7/fridaylabs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fridaylabs
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package to interact with FridayLabs AI API
 Home-page: https://github.com/ImJustRicky/fridaylabs-package
 Author: FridayLabs
 Author-email: fridaylabs@fridaylabs.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fridaylabs-0.1.6/setup.py` & `fridaylabs-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name="fridaylabs",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     install_requires=["requests"],  # Add any dependencies here
     author="FridayLabs",
     author_email="fridaylabs@fridaylabs.ai",
     description="A package to interact with FridayLabs AI API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

