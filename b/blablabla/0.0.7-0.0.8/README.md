# Comparing `tmp/blablabla-0.0.7.tar.gz` & `tmp/blablabla-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blablabla-0.0.7.tar", max compression
+gzip compressed data, was "blablabla-0.0.8.tar", max compression
```

## Comparing `blablabla-0.0.7.tar` & `blablabla-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      239 2024-05-28 22:53:20.481907 blablabla-0.0.7/blablabla/__init__.py
--rw-r--r--   0        0        0    11862 2024-05-28 22:27:26.816687 blablabla-0.0.7/blablabla/actions.py
--rw-r--r--   0        0        0     1935 2024-05-28 22:25:06.316007 blablabla-0.0.7/blablabla/orchestrator.py
--rw-r--r--   0        0        0      912 2024-05-28 21:30:32.732416 blablabla-0.0.7/blablabla/start_all.py
--rw-r--r--   0        0        0     2208 2024-05-28 22:25:06.306012 blablabla-0.0.7/blablabla/typing_server.py
--rw-r--r--   0        0        0    30941 2024-05-28 22:31:39.932817 blablabla-0.0.7/blablabla/whisper_online.py
--rw-r--r--   0        0        0     5470 2024-05-28 22:25:06.305013 blablabla-0.0.7/blablabla/whisper_server.py
--rw-r--r--   0        0        0    11548 2024-05-28 20:45:39.048641 blablabla-0.0.7/LICENSE
--rw-r--r--   0        0        0      958 2024-05-28 22:53:14.617340 blablabla-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1683 2024-05-28 21:45:11.511530 blablabla-0.0.7/README.md
--rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 blablabla-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      239 2024-05-29 19:55:33.450751 blablabla-0.0.8/blablabla/__init__.py
+-rw-r--r--   0        0        0    11862 2024-05-28 22:27:26.816687 blablabla-0.0.8/blablabla/actions.py
+-rw-r--r--   0        0        0     1935 2024-05-28 22:25:06.316007 blablabla-0.0.8/blablabla/orchestrator.py
+-rw-r--r--   0        0        0      912 2024-05-28 21:30:32.732416 blablabla-0.0.8/blablabla/start_all.py
+-rw-r--r--   0        0        0     2208 2024-05-28 22:25:06.306012 blablabla-0.0.8/blablabla/typing_server.py
+-rw-r--r--   0        0        0    30941 2024-05-28 22:31:39.932817 blablabla-0.0.8/blablabla/whisper_online.py
+-rw-r--r--   0        0        0     5470 2024-05-28 22:25:06.305013 blablabla-0.0.8/blablabla/whisper_server.py
+-rw-r--r--   0        0        0    11548 2024-05-28 20:45:39.048641 blablabla-0.0.8/LICENSE
+-rw-r--r--   0        0        0      958 2024-05-29 19:55:36.653668 blablabla-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1683 2024-05-28 21:45:11.511530 blablabla-0.0.8/README.md
+-rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 blablabla-0.0.8/PKG-INFO
```

### Comparing `blablabla-0.0.7/blablabla/actions.py` & `blablabla-0.0.8/blablabla/actions.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.7/blablabla/orchestrator.py` & `blablabla-0.0.8/blablabla/orchestrator.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.7/blablabla/start_all.py` & `blablabla-0.0.8/blablabla/start_all.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.7/blablabla/typing_server.py` & `blablabla-0.0.8/blablabla/typing_server.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.7/blablabla/whisper_online.py` & `blablabla-0.0.8/blablabla/whisper_online.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.7/blablabla/whisper_server.py` & `blablabla-0.0.8/blablabla/whisper_server.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.7/LICENSE` & `blablabla-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.7/pyproject.toml` & `blablabla-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blablabla"
-version = "0.0.7"
+version = "0.0.8"
 description = "A simple application to enable voice activated chatbot"
 authors = ["Guillaume Cadot <guillaume.cadot.1990@gmail.com>"]
 readme = "README.md"
 packages = [{include = "blablabla"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4.0"
```

### Comparing `blablabla-0.0.7/README.md` & `blablabla-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.7/PKG-INFO` & `blablabla-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blablabla
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple application to enable voice activated chatbot
 Author: Guillaume Cadot
 Author-email: guillaume.cadot.1990@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

