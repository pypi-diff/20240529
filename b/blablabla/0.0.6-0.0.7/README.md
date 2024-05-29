# Comparing `tmp/blablabla-0.0.6.tar.gz` & `tmp/blablabla-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blablabla-0.0.6.tar", max compression
+gzip compressed data, was "blablabla-0.0.7.tar", max compression
```

## Comparing `blablabla-0.0.6.tar` & `blablabla-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      239 2024-05-28 22:49:43.880807 blablabla-0.0.6/blablabla/__init__.py
--rw-r--r--   0        0        0    11862 2024-05-28 22:27:26.816687 blablabla-0.0.6/blablabla/actions.py
--rw-r--r--   0        0        0     1935 2024-05-28 22:25:06.316007 blablabla-0.0.6/blablabla/orchestrator.py
--rw-r--r--   0        0        0      912 2024-05-28 21:30:32.732416 blablabla-0.0.6/blablabla/start_all.py
--rw-r--r--   0        0        0     2208 2024-05-28 22:25:06.306012 blablabla-0.0.6/blablabla/typing_server.py
--rw-r--r--   0        0        0    30941 2024-05-28 22:31:39.932817 blablabla-0.0.6/blablabla/whisper_online.py
--rw-r--r--   0        0        0     5470 2024-05-28 22:25:06.305013 blablabla-0.0.6/blablabla/whisper_server.py
--rw-r--r--   0        0        0    11548 2024-05-28 20:45:39.048641 blablabla-0.0.6/LICENSE
--rw-r--r--   0        0        0      958 2024-05-28 22:49:47.746648 blablabla-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1683 2024-05-28 21:45:11.511530 blablabla-0.0.6/README.md
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 blablabla-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      239 2024-05-28 22:53:20.481907 blablabla-0.0.7/blablabla/__init__.py
+-rw-r--r--   0        0        0    11862 2024-05-28 22:27:26.816687 blablabla-0.0.7/blablabla/actions.py
+-rw-r--r--   0        0        0     1935 2024-05-28 22:25:06.316007 blablabla-0.0.7/blablabla/orchestrator.py
+-rw-r--r--   0        0        0      912 2024-05-28 21:30:32.732416 blablabla-0.0.7/blablabla/start_all.py
+-rw-r--r--   0        0        0     2208 2024-05-28 22:25:06.306012 blablabla-0.0.7/blablabla/typing_server.py
+-rw-r--r--   0        0        0    30941 2024-05-28 22:31:39.932817 blablabla-0.0.7/blablabla/whisper_online.py
+-rw-r--r--   0        0        0     5470 2024-05-28 22:25:06.305013 blablabla-0.0.7/blablabla/whisper_server.py
+-rw-r--r--   0        0        0    11548 2024-05-28 20:45:39.048641 blablabla-0.0.7/LICENSE
+-rw-r--r--   0        0        0      958 2024-05-28 22:53:14.617340 blablabla-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1683 2024-05-28 21:45:11.511530 blablabla-0.0.7/README.md
+-rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 blablabla-0.0.7/PKG-INFO
```

### Comparing `blablabla-0.0.6/blablabla/actions.py` & `blablabla-0.0.7/blablabla/actions.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.6/blablabla/orchestrator.py` & `blablabla-0.0.7/blablabla/orchestrator.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.6/blablabla/start_all.py` & `blablabla-0.0.7/blablabla/start_all.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.6/blablabla/typing_server.py` & `blablabla-0.0.7/blablabla/typing_server.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.6/blablabla/whisper_online.py` & `blablabla-0.0.7/blablabla/whisper_online.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.6/blablabla/whisper_server.py` & `blablabla-0.0.7/blablabla/whisper_server.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.6/LICENSE` & `blablabla-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.6/pyproject.toml` & `blablabla-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "blablabla"
-version = "0.0.6"
+version = "0.0.7"
 description = "A simple application to enable voice activated chatbot"
 authors = ["Guillaume Cadot <guillaume.cadot.1990@gmail.com>"]
 readme = "README.md"
 packages = [{include = "blablabla"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4.0"
 pysoundfile = "^0.9"
 librosa = "^0.10.2"
-openai = "^0.12.0"
+openai = "^1.30.4"
 pynput = "^1.7.3"
 pyperclip = "^1.8.2"
 keyboard = "^0.13.5"
 orjson = "^3.6.5"
 fastapi = "^0.111.0"
 uvicorn = "^0.30.0"
 aiohttp = "^3.7.4"
```

### Comparing `blablabla-0.0.6/README.md` & `blablabla-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.6/PKG-INFO` & `blablabla-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: blablabla
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple application to enable voice activated chatbot
 Author: Guillaume Cadot
 Author-email: guillaume.cadot.1990@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
 Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Requires-Dist: faster-whisper (>=0.10.1)
 Requires-Dist: keyboard (>=0.13.5,<0.14.0)
 Requires-Dist: librosa (>=0.10.2,<0.11.0)
-Requires-Dist: openai (>=0.12.0,<0.13.0)
+Requires-Dist: openai (>=1.30.4,<2.0.0)
 Requires-Dist: orjson (>=3.6.5,<4.0.0)
 Requires-Dist: pynput (>=1.7.3,<2.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: pysoundfile (>=0.9,<0.10)
 Requires-Dist: sounddevice (>=0.4.1,<0.5.0)
 Requires-Dist: statesman (>=1.0,<2.0)
 Requires-Dist: uvicorn (>=0.30.0,<0.31.0)
```

