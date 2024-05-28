# Comparing `tmp/blablabla-0.0.3.tar.gz` & `tmp/blablabla-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blablabla-0.0.3.tar", max compression
+gzip compressed data, was "blablabla-0.0.4.tar", max compression
```

## Comparing `blablabla-0.0.3.tar` & `blablabla-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      239 2024-05-28 22:06:18.910080 blablabla-0.0.3/blablabla/__init__.py
--rw-r--r--   0        0        0    11931 2024-05-28 21:29:20.751572 blablabla-0.0.3/blablabla/actions.py
--rw-r--r--   0        0        0     1958 2024-05-28 21:29:12.703349 blablabla-0.0.3/blablabla/orchestrator.py
--rw-r--r--   0        0        0      912 2024-05-28 21:30:32.732416 blablabla-0.0.3/blablabla/start_all.py
--rw-r--r--   0        0        0     2231 2024-05-21 22:50:55.303198 blablabla-0.0.3/blablabla/typing_server.py
--rw-r--r--   0        0        0    30939 2024-05-21 23:36:38.897204 blablabla-0.0.3/blablabla/whisper_online.py
--rw-r--r--   0        0        0     5493 2024-05-28 21:28:54.698470 blablabla-0.0.3/blablabla/whisper_server.py
--rw-r--r--   0        0        0    11548 2024-05-28 20:45:39.048641 blablabla-0.0.3/LICENSE
--rw-r--r--   0        0        0      957 2024-05-28 22:07:40.482781 blablabla-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1683 2024-05-28 21:45:11.511530 blablabla-0.0.3/README.md
--rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 blablabla-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      239 2024-05-28 22:17:06.641005 blablabla-0.0.4/blablabla/__init__.py
+-rw-r--r--   0        0        0    11931 2024-05-28 21:29:20.751572 blablabla-0.0.4/blablabla/actions.py
+-rw-r--r--   0        0        0     1958 2024-05-28 21:29:12.703349 blablabla-0.0.4/blablabla/orchestrator.py
+-rw-r--r--   0        0        0      912 2024-05-28 21:30:32.732416 blablabla-0.0.4/blablabla/start_all.py
+-rw-r--r--   0        0        0     2231 2024-05-21 22:50:55.303198 blablabla-0.0.4/blablabla/typing_server.py
+-rw-r--r--   0        0        0    30939 2024-05-21 23:36:38.897204 blablabla-0.0.4/blablabla/whisper_online.py
+-rw-r--r--   0        0        0     5493 2024-05-28 21:28:54.698470 blablabla-0.0.4/blablabla/whisper_server.py
+-rw-r--r--   0        0        0    11548 2024-05-28 20:45:39.048641 blablabla-0.0.4/LICENSE
+-rw-r--r--   0        0        0      957 2024-05-28 22:17:01.874464 blablabla-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1683 2024-05-28 21:45:11.511530 blablabla-0.0.4/README.md
+-rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 blablabla-0.0.4/PKG-INFO
```

### Comparing `blablabla-0.0.3/blablabla/actions.py` & `blablabla-0.0.4/blablabla/actions.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.3/blablabla/orchestrator.py` & `blablabla-0.0.4/blablabla/orchestrator.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.3/blablabla/start_all.py` & `blablabla-0.0.4/blablabla/start_all.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.3/blablabla/typing_server.py` & `blablabla-0.0.4/blablabla/typing_server.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.3/blablabla/whisper_online.py` & `blablabla-0.0.4/blablabla/whisper_online.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.3/blablabla/whisper_server.py` & `blablabla-0.0.4/blablabla/whisper_server.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.3/LICENSE` & `blablabla-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.3/pyproject.toml` & `blablabla-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blablabla"
-version = "0.0.3"
+version = "0.0.4"
 description = "A simple application to enable voice activated chatbot"
 authors = ["Guillaume Cadot <guillaume.cadot.1990@gmail.com>"]
 readme = "README.md"
 packages = [{include = "blablabla"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4.0"
@@ -12,15 +12,15 @@
 librosa = "^0.8.1"
 openai = "^0.12.0"
 pynput = "^1.7.3"
 pyperclip = "^1.8.2"
 keyboard = "^0.13.5"
 orjson = "^3.6.5"
 fastapi = "^0.111.0"
-uvicorn = "^0.15.0"
+uvicorn = "^0.30.0"
 aiohttp = "^3.7.4"
 sounddevice = "^0.4.1"
 statesman = "^1.0"
 faster-whisper=">=0.10.1"
 
 [tool.poetry.dev-dependencies]
 icecream = "^2.1.3"
```

### Comparing `blablabla-0.0.3/README.md` & `blablabla-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.3/PKG-INFO` & `blablabla-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blablabla
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple application to enable voice activated chatbot
 Author: Guillaume Cadot
 Author-email: guillaume.cadot.1990@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -16,15 +16,15 @@
 Requires-Dist: openai (>=0.12.0,<0.13.0)
 Requires-Dist: orjson (>=3.6.5,<4.0.0)
 Requires-Dist: pynput (>=1.7.3,<2.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: pysoundfile (>=0.9,<0.10)
 Requires-Dist: sounddevice (>=0.4.1,<0.5.0)
 Requires-Dist: statesman (>=1.0,<2.0)
-Requires-Dist: uvicorn (>=0.15.0,<0.16.0)
+Requires-Dist: uvicorn (>=0.30.0,<0.31.0)
 Description-Content-Type: text/markdown
 
 **Project Blablabla: Conversational AI for the Modern Era**
 
 Imagine a world where interacting with artificial intelligence is as natural as chatting with a friend 🤖. Welcome to Blablabla, a pioneering voice-activated chat interface that's taking the first step towards making human-AI conversations a reality 💬.
 
 **Current Focus: Live Transcription**
```

