# Comparing `tmp/blablabla-0.0.1.tar.gz` & `tmp/blablabla-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blablabla-0.0.1.tar", max compression
+gzip compressed data, was "blablabla-0.0.2.tar", max compression
```

## Comparing `blablabla-0.0.1.tar` & `blablabla-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      235 2024-05-21 23:38:13.546337 blablabla-0.0.1/blablabla/__init__.py
--rw-r--r--   0        0        0    11931 2024-05-21 23:36:38.894206 blablabla-0.0.1/blablabla/actions.py
--rw-r--r--   0        0        0     1957 2024-05-21 23:36:38.895205 blablabla-0.0.1/blablabla/orchestrator.py
--rw-r--r--   0        0        0      824 2024-05-21 22:50:51.783876 blablabla-0.0.1/blablabla/start_all.py
--rw-r--r--   0        0        0     2231 2024-05-21 22:50:55.303198 blablabla-0.0.1/blablabla/typing_server.py
--rw-r--r--   0        0        0    30939 2024-05-21 23:36:38.897204 blablabla-0.0.1/blablabla/whisper_online.py
--rw-r--r--   0        0        0     5541 2024-05-21 23:36:38.898204 blablabla-0.0.1/blablabla/whisper_server.py
--rw-r--r--   0        0        0    11548 2024-05-28 20:45:39.048641 blablabla-0.0.1/LICENSE
--rw-r--r--   0        0        0      855 2024-05-28 20:45:51.274773 blablabla-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       73 2024-05-21 23:02:05.373930 blablabla-0.0.1/README.md
--rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 blablabla-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      239 2024-05-28 21:28:10.489726 blablabla-0.0.2/blablabla/__init__.py
+-rw-r--r--   0        0        0    11931 2024-05-28 21:29:20.751572 blablabla-0.0.2/blablabla/actions.py
+-rw-r--r--   0        0        0     1958 2024-05-28 21:29:12.703349 blablabla-0.0.2/blablabla/orchestrator.py
+-rw-r--r--   0        0        0      912 2024-05-28 21:30:32.732416 blablabla-0.0.2/blablabla/start_all.py
+-rw-r--r--   0        0        0     2231 2024-05-21 22:50:55.303198 blablabla-0.0.2/blablabla/typing_server.py
+-rw-r--r--   0        0        0    30939 2024-05-21 23:36:38.897204 blablabla-0.0.2/blablabla/whisper_online.py
+-rw-r--r--   0        0        0     5493 2024-05-28 21:28:54.698470 blablabla-0.0.2/blablabla/whisper_server.py
+-rw-r--r--   0        0        0    11548 2024-05-28 20:45:39.048641 blablabla-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1034 2024-05-28 21:12:35.412981 blablabla-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1683 2024-05-28 21:45:11.511530 blablabla-0.0.2/README.md
+-rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 blablabla-0.0.2/PKG-INFO
```

### Comparing `blablabla-0.0.1/blablabla/actions.py` & `blablabla-0.0.2/blablabla/actions.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.1/blablabla/orchestrator.py` & `blablabla-0.0.2/blablabla/orchestrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import keyboard
 import argparse
 import asyncio
 from icecream import ic
 import sounddevice as sd
 import statesman
 
-from actions import record_producers, whisper_consumer, text_consumer, ProcessLifecycle
+from .actions import record_producers, whisper_consumer, text_consumer, ProcessLifecycle
 
 
 class AppLifecycle(statesman.StateMachine):
     class States(statesman.StateEnum):
         starting = "Starting..."
         recording = "Recording..."
         stopping = "Stopping..."
```

### Comparing `blablabla-0.0.1/blablabla/start_all.py` & `blablabla-0.0.2/blablabla/start_all.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from __init__ import start_typing_server, start_whisper_server, start_orchestrator
+
 from multiprocessing import Process
 import requests
 import argparse
 
+from .whisper_server import main as start_whisper_server
+from .typing_server import main as start_typing_server
+from .orchestrator import main as start_orchestrator
+
 
 def main():
     p_whisper = Process(target=start_whisper_server, args=())
     p_whisper.start()
 
     parser = argparse.ArgumentParser()
     parser.add_argument(
```

### Comparing `blablabla-0.0.1/blablabla/typing_server.py` & `blablabla-0.0.2/blablabla/typing_server.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.1/blablabla/whisper_online.py` & `blablabla-0.0.2/blablabla/whisper_online.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.1/blablabla/whisper_server.py` & `blablabla-0.0.2/blablabla/whisper_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import argparse
 import logging
 import orjson
 from typing import Annotated, List, Optional
 from pydantic import BaseModel
 from fastapi import FastAPI, File, UploadFile, Request, Body, Depends
 from fastapi.responses import ORJSONResponse, RedirectResponse
-from whisper_online import asr_factory, set_logging
+
 import numpy as np
 import logging
 import uvicorn
 import io
 import soundfile as sf
 from icecream import ic
 
-from whisper_online import asr_factory, set_logging, OnlineASRProcessor
+
+from .whisper_online import asr_factory, set_logging, OnlineASRProcessor
 
 # Set up logging
 logger = logging.getLogger(__name__)
 
 
 class ASR:
     instance = None
```

### Comparing `blablabla-0.0.1/LICENSE` & `blablabla-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.1/pyproject.toml` & `blablabla-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "blablabla"
-version = "0.0.1"
+version = "0.0.2"
 description = "A simple application to enable voice activated chatbot"
 authors = ["Guillaume Cadot <guillaume.cadot.1990@gmail.com>"]
 readme = "README.md"
 packages = [{include = "blablabla"}]
 
 [tool.poetry.dependencies]
-python = ">3.11,<4.0"
+python = ">=3.11,<4.0"
 pysoundfile = "^0.9"
 librosa = "^0.8.1"
 openai = "^0.12.0"
 pynput = "^1.7.3"
 pyperclip = "^1.8.2"
 keyboard = "^0.13.5"
 orjson = "^3.6.5"
@@ -26,11 +26,16 @@
 faster-whisper=">=0.10.1"
 
 [tool.poetry.dev-dependencies]
 icecream = "^2.1.3"
 pytest = "^6.2.5"
 poetry = "^1.8"
 logfire = "^0.35"
+poetry-bumpversion = "^0.3.2"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry_bumpversion.file."blablabla/__init__.py"]
+search = '__version__ = "{current_version}"'
+replace = '__version__ = "{new_version}"'
```

