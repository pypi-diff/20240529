# Comparing `tmp/fridaylabs-0.1.5.tar.gz` & `tmp/fridaylabs-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fridaylabs-0.1.5.tar", last modified: Tue May 21 20:05:48 2024, max compression
+gzip compressed data, was "fridaylabs-0.1.6.tar", last modified: Wed May 29 19:30:15 2024, max compression
```

## Comparing `fridaylabs-0.1.5.tar` & `fridaylabs-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 20:05:48.459944 fridaylabs-0.1.5/
--rw-r--r--   0 ricky      (501) staff       (20)     1070 2024-05-21 04:23:26.000000 fridaylabs-0.1.5/LICENSE
--rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 20:05:48.459690 fridaylabs-0.1.5/PKG-INFO
--rw-r--r--   0 ricky      (501) staff       (20)      792 2024-05-21 05:35:31.000000 fridaylabs-0.1.5/README.md
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 20:05:48.458251 fridaylabs-0.1.5/fridaylabs/
--rw-r--r--   0 ricky      (501) staff       (20)       61 2024-05-21 05:49:44.000000 fridaylabs-0.1.5/fridaylabs/__init__.py
--rw-r--r--   0 ricky      (501) staff       (20)     4891 2024-05-21 20:05:31.000000 fridaylabs-0.1.5/fridaylabs/fridaylabs.py
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 20:05:48.459437 fridaylabs-0.1.5/fridaylabs.egg-info/
--rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 20:05:48.000000 fridaylabs-0.1.5/fridaylabs.egg-info/PKG-INFO
--rw-r--r--   0 ricky      (501) staff       (20)      243 2024-05-21 20:05:48.000000 fridaylabs-0.1.5/fridaylabs.egg-info/SOURCES.txt
--rw-r--r--   0 ricky      (501) staff       (20)        1 2024-05-21 20:05:48.000000 fridaylabs-0.1.5/fridaylabs.egg-info/dependency_links.txt
--rw-r--r--   0 ricky      (501) staff       (20)        9 2024-05-21 20:05:48.000000 fridaylabs-0.1.5/fridaylabs.egg-info/requires.txt
--rw-r--r--   0 ricky      (501) staff       (20)       11 2024-05-21 20:05:48.000000 fridaylabs-0.1.5/fridaylabs.egg-info/top_level.txt
--rw-r--r--   0 ricky      (501) staff       (20)       38 2024-05-21 20:05:48.459998 fridaylabs-0.1.5/setup.cfg
--rw-r--r--   0 ricky      (501) staff       (20)      693 2024-05-21 20:05:45.000000 fridaylabs-0.1.5/setup.py
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 19:30:15.516070 fridaylabs-0.1.6/
+-rw-r--r--   0 ricky      (501) staff       (20)     1070 2024-05-21 04:23:26.000000 fridaylabs-0.1.6/LICENSE
+-rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-29 19:30:15.515770 fridaylabs-0.1.6/PKG-INFO
+-rw-r--r--   0 ricky      (501) staff       (20)      792 2024-05-21 05:35:31.000000 fridaylabs-0.1.6/README.md
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 19:30:15.514372 fridaylabs-0.1.6/fridaylabs/
+-rw-r--r--   0 ricky      (501) staff       (20)       61 2024-05-21 05:49:44.000000 fridaylabs-0.1.6/fridaylabs/__init__.py
+-rw-r--r--   0 ricky      (501) staff       (20)     4871 2024-05-29 19:29:27.000000 fridaylabs-0.1.6/fridaylabs/fridaylabs.py
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 19:30:15.515502 fridaylabs-0.1.6/fridaylabs.egg-info/
+-rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-29 19:30:15.000000 fridaylabs-0.1.6/fridaylabs.egg-info/PKG-INFO
+-rw-r--r--   0 ricky      (501) staff       (20)      243 2024-05-29 19:30:15.000000 fridaylabs-0.1.6/fridaylabs.egg-info/SOURCES.txt
+-rw-r--r--   0 ricky      (501) staff       (20)        1 2024-05-29 19:30:15.000000 fridaylabs-0.1.6/fridaylabs.egg-info/dependency_links.txt
+-rw-r--r--   0 ricky      (501) staff       (20)        9 2024-05-29 19:30:15.000000 fridaylabs-0.1.6/fridaylabs.egg-info/requires.txt
+-rw-r--r--   0 ricky      (501) staff       (20)       11 2024-05-29 19:30:15.000000 fridaylabs-0.1.6/fridaylabs.egg-info/top_level.txt
+-rw-r--r--   0 ricky      (501) staff       (20)       38 2024-05-29 19:30:15.516122 fridaylabs-0.1.6/setup.cfg
+-rw-r--r--   0 ricky      (501) staff       (20)      693 2024-05-29 19:29:54.000000 fridaylabs-0.1.6/setup.py
```

### Comparing `fridaylabs-0.1.5/LICENSE` & `fridaylabs-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.5/PKG-INFO` & `fridaylabs-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fridaylabs
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package to interact with FridayLabs AI API
 Home-page: https://github.com/ImJustRicky/fridaylabs-package
 Author: FridayLabs
 Author-email: fridaylabs@fridaylabs.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fridaylabs-0.1.5/README.md` & `fridaylabs-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.5/fridaylabs/fridaylabs.py` & `fridaylabs-0.1.6/fridaylabs/fridaylabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# fridaylabs/fridaylabs.py
-
 import requests
 
 class Colors:
     HEADER = "\033[95m"
     OKBLUE = "\033[94m"
     OKGREEN = "\033[92m"
     WARNING = "\033[93m"
@@ -14,15 +12,15 @@
 
 class FridayLabs:
     def __init__(self, api_key, api_url, verbose=False):
         self.api_key = api_key
         self.api_url = api_url
         self.verbose = verbose
 
-    def chat_completion(self, model, messages, temperature=1, max_tokens=256, top_p=1, frequency_penalty=0, presence_penalty=0):
+    def chat_completion(self, model, messages, temperature=1.0, max_tokens=256, top_p=1.0, frequency_penalty=0.0, presence_penalty=0.0):
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json"
         }
         payload = {
             "model": model,
             "messages": messages,
```

### Comparing `fridaylabs-0.1.5/fridaylabs.egg-info/PKG-INFO` & `fridaylabs-0.1.6/fridaylabs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fridaylabs
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package to interact with FridayLabs AI API
 Home-page: https://github.com/ImJustRicky/fridaylabs-package
 Author: FridayLabs
 Author-email: fridaylabs@fridaylabs.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fridaylabs-0.1.5/setup.py` & `fridaylabs-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name="fridaylabs",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=["requests"],  # Add any dependencies here
     author="FridayLabs",
     author_email="fridaylabs@fridaylabs.ai",
     description="A package to interact with FridayLabs AI API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

