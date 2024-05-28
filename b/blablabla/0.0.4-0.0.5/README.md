# Comparing `tmp/blablabla-0.0.4.tar.gz` & `tmp/blablabla-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blablabla-0.0.4.tar", max compression
+gzip compressed data, was "blablabla-0.0.5.tar", max compression
```

## Comparing `blablabla-0.0.4.tar` & `blablabla-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      239 2024-05-28 22:17:06.641005 blablabla-0.0.4/blablabla/__init__.py
--rw-r--r--   0        0        0    11931 2024-05-28 21:29:20.751572 blablabla-0.0.4/blablabla/actions.py
--rw-r--r--   0        0        0     1958 2024-05-28 21:29:12.703349 blablabla-0.0.4/blablabla/orchestrator.py
--rw-r--r--   0        0        0      912 2024-05-28 21:30:32.732416 blablabla-0.0.4/blablabla/start_all.py
--rw-r--r--   0        0        0     2231 2024-05-21 22:50:55.303198 blablabla-0.0.4/blablabla/typing_server.py
--rw-r--r--   0        0        0    30939 2024-05-21 23:36:38.897204 blablabla-0.0.4/blablabla/whisper_online.py
--rw-r--r--   0        0        0     5493 2024-05-28 21:28:54.698470 blablabla-0.0.4/blablabla/whisper_server.py
--rw-r--r--   0        0        0    11548 2024-05-28 20:45:39.048641 blablabla-0.0.4/LICENSE
--rw-r--r--   0        0        0      957 2024-05-28 22:17:01.874464 blablabla-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1683 2024-05-28 21:45:11.511530 blablabla-0.0.4/README.md
--rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 blablabla-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      239 2024-05-28 22:28:20.756130 blablabla-0.0.5/blablabla/__init__.py
+-rw-r--r--   0        0        0    11862 2024-05-28 22:27:26.816687 blablabla-0.0.5/blablabla/actions.py
+-rw-r--r--   0        0        0     1935 2024-05-28 22:25:06.316007 blablabla-0.0.5/blablabla/orchestrator.py
+-rw-r--r--   0        0        0      912 2024-05-28 21:30:32.732416 blablabla-0.0.5/blablabla/start_all.py
+-rw-r--r--   0        0        0     2208 2024-05-28 22:25:06.306012 blablabla-0.0.5/blablabla/typing_server.py
+-rw-r--r--   0        0        0    30916 2024-05-28 22:25:06.304013 blablabla-0.0.5/blablabla/whisper_online.py
+-rw-r--r--   0        0        0     5470 2024-05-28 22:25:06.305013 blablabla-0.0.5/blablabla/whisper_server.py
+-rw-r--r--   0        0        0    11548 2024-05-28 20:45:39.048641 blablabla-0.0.5/LICENSE
+-rw-r--r--   0        0        0      957 2024-05-28 22:28:15.651908 blablabla-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1683 2024-05-28 21:45:11.511530 blablabla-0.0.5/README.md
+-rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 blablabla-0.0.5/PKG-INFO
```

### Comparing `blablabla-0.0.4/blablabla/actions.py` & `blablabla-0.0.5/blablabla/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,28 +7,24 @@
 
 # import webrtcvad
 import keyboard
 import orjson
 import aiohttp
 from typing import Tuple
 import ssl
-from icecream import ic
+
 import statesman
 import logging
 
 from datetime import datetime
 
-
 def time_format():
     return f"{datetime.now()}|> "
 
 
-ic.configureOutput(prefix=time_format)
-
-
 class ProcessLifecycle(statesman.StateMachine):
     class States(statesman.StateEnum):
         starting = "Starting..."
         recording = "Recording..."
         stopping = "Stopping..."
         stopped = "Terminated."
```

### Comparing `blablabla-0.0.4/blablabla/orchestrator.py` & `blablabla-0.0.5/blablabla/orchestrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import keyboard
 import argparse
 import asyncio
-from icecream import ic
+
 import sounddevice as sd
 import statesman
 
 from .actions import record_producers, whisper_consumer, text_consumer, ProcessLifecycle
 
 
 class AppLifecycle(statesman.StateMachine):
```

### Comparing `blablabla-0.0.4/blablabla/start_all.py` & `blablabla-0.0.5/blablabla/start_all.py`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.4/blablabla/typing_server.py` & `blablabla-0.0.5/blablabla/typing_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import orjson
 import pynput
 from typing import Annotated, List, Optional, Callable
 from pydantic import BaseModel
 from fastapi import FastAPI, File, UploadFile, Request, Body, Depends
 from fastapi.responses import ORJSONResponse
 import uvicorn
-from icecream import ic
+
 
 
 class Output:
     instance = None
     text_output_method: Callable[[str], None]
 
     def __new__(cls):
```

### Comparing `blablabla-0.0.4/blablabla/whisper_online.py` & `blablabla-0.0.5/blablabla/whisper_online.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import librosa  
 from functools import lru_cache
 import time
 import logging
 from dotenv import load_dotenv
 import os
-from icecream import ic
+
 import requests
 
 
 import io
 import soundfile as sf
 import math
```

### Comparing `blablabla-0.0.4/blablabla/whisper_server.py` & `blablabla-0.0.5/blablabla/whisper_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from fastapi.responses import ORJSONResponse, RedirectResponse
 
 import numpy as np
 import logging
 import uvicorn
 import io
 import soundfile as sf
-from icecream import ic
+
 
 
 from .whisper_online import asr_factory, set_logging, OnlineASRProcessor
 
 # Set up logging
 logger = logging.getLogger(__name__)
```

### Comparing `blablabla-0.0.4/LICENSE` & `blablabla-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.4/pyproject.toml` & `blablabla-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blablabla"
-version = "0.0.4"
+version = "0.0.5"
 description = "A simple application to enable voice activated chatbot"
 authors = ["Guillaume Cadot <guillaume.cadot.1990@gmail.com>"]
 readme = "README.md"
 packages = [{include = "blablabla"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4.0"
```

### Comparing `blablabla-0.0.4/README.md` & `blablabla-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `blablabla-0.0.4/PKG-INFO` & `blablabla-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blablabla
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple application to enable voice activated chatbot
 Author: Guillaume Cadot
 Author-email: guillaume.cadot.1990@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

