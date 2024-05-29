# Comparing `tmp/aishalib-0.0.1.tar.gz` & `tmp/aishalib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aishalib-0.0.1.tar", last modified: Wed May 29 10:04:03 2024, max compression
+gzip compressed data, was "aishalib-0.0.2.tar", last modified: Wed May 29 10:26:15 2024, max compression
```

## Comparing `aishalib-0.0.1.tar` & `aishalib-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-29 10:04:03.274960 aishalib-0.0.1/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-29 08:46:39.000000 aishalib-0.0.1/LICENSE
--rw-r--r--   0 man4j     (1000) man4j     (1000)      568 2024-05-29 10:04:03.274960 aishalib-0.0.1/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)      640 2024-05-29 09:03:33.000000 aishalib-0.0.1/pyproject.toml
--rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-29 10:04:03.274960 aishalib-0.0.1/setup.cfg
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-29 10:04:03.270960 aishalib-0.0.1/src/
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-29 10:04:03.270960 aishalib-0.0.1/src/aishalib/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     3729 2024-05-29 09:13:50.000000 aishalib-0.0.1/src/aishalib/aishalib.py
--rw-r--r--   0 man4j     (1000) man4j     (1000)      922 2024-05-29 09:10:58.000000 aishalib-0.0.1/src/aishalib/llmbackend.py
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-29 10:04:03.274960 aishalib-0.0.1/src/aishalib.egg-info/
--rw-r--r--   0 man4j     (1000) man4j     (1000)      568 2024-05-29 10:04:03.000000 aishalib-0.0.1/src/aishalib.egg-info/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)      253 2024-05-29 10:04:03.000000 aishalib-0.0.1/src/aishalib.egg-info/SOURCES.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-29 10:04:03.000000 aishalib-0.0.1/src/aishalib.egg-info/dependency_links.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)       21 2024-05-29 10:04:03.000000 aishalib-0.0.1/src/aishalib.egg-info/requires.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        9 2024-05-29 10:04:03.000000 aishalib-0.0.1/src/aishalib.egg-info/top_level.txt
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-29 10:26:15.692142 aishalib-0.0.2/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-29 08:46:39.000000 aishalib-0.0.2/LICENSE
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      597 2024-05-29 10:26:15.692142 aishalib-0.0.2/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      659 2024-05-29 10:25:58.000000 aishalib-0.0.2/pyproject.toml
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-29 10:26:15.692142 aishalib-0.0.2/setup.cfg
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-29 10:26:15.688142 aishalib-0.0.2/src/
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-29 10:26:15.692142 aishalib-0.0.2/src/aishalib/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     3729 2024-05-29 09:13:50.000000 aishalib-0.0.2/src/aishalib/aishalib.py
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      922 2024-05-29 09:10:58.000000 aishalib-0.0.2/src/aishalib/llmbackend.py
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-29 10:26:15.692142 aishalib-0.0.2/src/aishalib.egg-info/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      597 2024-05-29 10:26:15.000000 aishalib-0.0.2/src/aishalib.egg-info/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      253 2024-05-29 10:26:15.000000 aishalib-0.0.2/src/aishalib.egg-info/SOURCES.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-29 10:26:15.000000 aishalib-0.0.2/src/aishalib.egg-info/dependency_links.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       35 2024-05-29 10:26:15.000000 aishalib-0.0.2/src/aishalib.egg-info/requires.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        9 2024-05-29 10:26:15.000000 aishalib-0.0.2/src/aishalib.egg-info/top_level.txt
```

### Comparing `aishalib-0.0.1/LICENSE` & `aishalib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.1/PKG-INFO` & `aishalib-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: aishalib
-Version: 0.0.1
+Version: 0.0.2
 Summary: AI Smart Human Assistant Library
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aishalib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: transformers>=4.41.1
+Requires-Dist: jinja2>=3.1.4
```

### Comparing `aishalib-0.0.1/pyproject.toml` & `aishalib-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aishalib"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Vladimir Petrukhin", email="man4j@ya.ru" },
 ]
 description = "AI Smart Human Assistant Library"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "transformers>=4.41.1"
+  "transformers>=4.41.1",
+  "jinja2>=3.1.4"
 ]
 
 [project.urls]
 Homepage = "https://github.com/Equiron-AI/aishalib"
```

### Comparing `aishalib-0.0.1/src/aishalib/aishalib.py` & `aishalib-0.0.2/src/aishalib/aishalib.py`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.1/src/aishalib/llmbackend.py` & `aishalib-0.0.2/src/aishalib/llmbackend.py`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.1/src/aishalib.egg-info/PKG-INFO` & `aishalib-0.0.2/src/aishalib.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: aishalib
-Version: 0.0.1
+Version: 0.0.2
 Summary: AI Smart Human Assistant Library
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aishalib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: transformers>=4.41.1
+Requires-Dist: jinja2>=3.1.4
```

