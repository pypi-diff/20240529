# Comparing `tmp/teia_sdk-0.1.7.tar.gz` & `tmp/teia_sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teia_sdk-0.1.7.tar", last modified: Wed Mar  6 18:25:31 2024, max compression
+gzip compressed data, was "teia_sdk-0.1.8.tar", last modified: Wed May 29 17:16:49 2024, max compression
```

## Comparing `teia_sdk-0.1.7.tar` & `teia_sdk-0.1.8.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 18:25:31.334885 teia_sdk-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-06 18:25:31.334885 teia_sdk-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 18:25:31.334885 teia_sdk-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 18:25:31.326885 teia_sdk-0.1.7/teia_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 18:25:31.330885 teia_sdk-0.1.7/teia_sdk/melting/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/melting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/melting/chat_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/melting/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/melting/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 18:25:31.330885 teia_sdk-0.1.7/teia_sdk/melting/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/melting/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/melting/services/chat_completions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/melting/services/chat_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/melting/services/fcall_completions.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/melting/services/tcall_completions.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/melting/services/text_encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 18:25:31.330885 teia_sdk-0.1.7/teia_sdk/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/plugins/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/plugins/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/plugins/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 18:25:31.330885 teia_sdk-0.1.7/teia_sdk/private_workspaces/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/private_workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/private_workspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/private_workspaces/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/private_workspaces/private_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/private_workspaces/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 18:25:31.330885 teia_sdk-0.1.7/teia_sdk/search/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/search/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/search/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/search/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/teia_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 18:25:31.330885 teia_sdk-0.1.7/teia_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-06 18:25:31.000000 teia_sdk-0.1.7/teia_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-06 18:25:31.000000 teia_sdk-0.1.7/teia_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 18:25:31.000000 teia_sdk-0.1.7/teia_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-06 18:25:31.000000 teia_sdk-0.1.7/teia_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-06 18:25:31.000000 teia_sdk-0.1.7/teia_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-06 18:25:31.000000 teia_sdk-0.1.7/teia_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 18:25:31.330885 teia_sdk-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-06 18:25:18.000000 teia_sdk-0.1.7/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:16:49.607654 teia_sdk-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-29 17:16:49.607654 teia_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:16:49.607654 teia_sdk-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:16:49.603654 teia_sdk-0.1.8/teia_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:16:49.603654 teia_sdk-0.1.8/teia_sdk/dbsailor/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/dbsailor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/dbsailor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/dbsailor/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:16:49.603654 teia_sdk-0.1.8/teia_sdk/melting/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/melting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/melting/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/melting/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/melting/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:16:49.603654 teia_sdk-0.1.8/teia_sdk/melting/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/melting/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/melting/services/chat_completions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/melting/services/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/melting/services/fcall_completions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/melting/services/tcall_completions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/melting/services/text_encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:16:49.607654 teia_sdk-0.1.8/teia_sdk/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/plugins/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/plugins/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/plugins/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:16:49.607654 teia_sdk-0.1.8/teia_sdk/private_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/private_workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/private_workspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/private_workspaces/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/private_workspaces/private_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/private_workspaces/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:16:49.607654 teia_sdk-0.1.8/teia_sdk/search/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/search/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/search/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/teia_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:16:49.607654 teia_sdk-0.1.8/teia_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-29 17:16:49.000000 teia_sdk-0.1.8/teia_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-29 17:16:49.000000 teia_sdk-0.1.8/teia_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:16:49.000000 teia_sdk-0.1.8/teia_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-29 17:16:49.000000 teia_sdk-0.1.8/teia_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-29 17:16:49.000000 teia_sdk-0.1.8/teia_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 17:16:49.000000 teia_sdk-0.1.8/teia_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:16:49.607654 teia_sdk-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-29 17:16:39.000000 teia_sdk-0.1.8/tests/test_search.py
```

### Comparing `teia_sdk-0.1.7/PKG-INFO` & `teia_sdk-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: teia_sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: Teia SDK
 Home-page: https://github.com/TeiaLabs/teia-sdk
 Author: TeiaLabs
 Author-email: contato@teialabs.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fastapi
+Requires-Dist: fastapi==0.111.0
 Requires-Dist: http_error_schemas==1.0.1
-Requires-Dist: httpx
-Requires-Dist: melting_schemas==1.0.7
-Requires-Dist: python-dotenv
-Requires-Dist: requests
-Requires-Dist: rich
-Requires-Dist: typer[all]
+Requires-Dist: melting_schemas==1.0.9
+Requires-Dist: httpx==0.27.0
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: requests==2.32.2
+Requires-Dist: rich==13.7.1
+Requires-Dist: typer[all]==0.12.3
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # Teia SDK 🕸️
 
 # install 🕷️
 ```bash
```

### Comparing `teia_sdk-0.1.7/setup.py` & `teia_sdk-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk/melting/chat_prompts.py` & `teia_sdk-0.1.8/teia_sdk/melting/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk/melting/schemas.py` & `teia_sdk-0.1.8/teia_sdk/melting/schemas.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk/melting/services/chat_completions.py` & `teia_sdk-0.1.8/teia_sdk/melting/services/chat_completions.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk/melting/services/chat_prompts.py` & `teia_sdk-0.1.8/teia_sdk/melting/services/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk/melting/services/fcall_completions.py` & `teia_sdk-0.1.8/teia_sdk/melting/services/fcall_completions.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk/melting/services/tcall_completions.py` & `teia_sdk-0.1.8/teia_sdk/melting/services/tcall_completions.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk/melting/services/text_encodings.py` & `teia_sdk-0.1.8/teia_sdk/melting/services/text_encodings.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk/plugins/client.py` & `teia_sdk-0.1.8/teia_sdk/plugins/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import json
 import logging
 import os
-from typing import Any, Optional
+from typing import Any, Literal, Optional
 
 import httpx
+import requests
 from melting_schemas.completion.fcall import ChatMLMessage, FCallModelSettings
-
 from starlette import status as http_status
 
 from . import exceptions
 from .schemas import (
     GetPluginExecution,
     GetPluginSelection,
     PluginInfo,
@@ -17,26 +18,24 @@
     SelectPlugin,
 )
 
 logger = logging.getLogger(__name__)
 
 try:
     TEIA_API_KEY = os.environ["TEIA_API_KEY"]
-    PLUGINS_API_URL = os.getenv(
-        "PLUGINS_API_URL", "https://plugins.athena.teialabs.com.br"
-    )
+    PLUGINS_API_URL = os.getenv("PLUGINS_API_URL", "https://plugins.allai.digital")
 except KeyError:
     m = "[red]MissingEnvironmentVariables[/red]: "
     m += "[yellow]'TEIA_API_KEY'[/yellow] cannot be empty."
     print(m)
     exit(1)
 
 
 class PluginClient:
-    client = httpx.Client(timeout=120)
+    client = httpx.Client(timeout=300)
 
     @classmethod
     def get_headers(cls) -> dict[str, str]:
         obj = {
             "Authorization": f"Bearer {TEIA_API_KEY}",
         }
         return obj
@@ -54,14 +53,15 @@
         cls,
         messages: list[ChatMLMessage],
         plugin_names: list[str],
         model_settings: FCallModelSettings,
         plugin_extra_args: Optional[dict[str, dict[str, str]]] = None,
         user_email: Optional[str] = None,
         schemaless: bool = True,
+        tool_choice: Optional[Literal["auto", "required"] | dict] = "auto",
     ) -> PluginResponse:
 
         if not plugin_names:
             return PluginResponse(
                 selector_completion="",
                 plugin_infos=[],
                 error=f"No plugins in plugin_names",
@@ -73,14 +73,15 @@
             plugin_extra_args[plugin]["schemaless"] = schemaless
 
         sp = SelectPlugin(
             messages=messages,
             plugin_names=plugin_names,
             model_settings=model_settings,
             plugin_extra_arguments=plugin_extra_args,
+            tool_choice=tool_choice,
         )
 
         sel_run_url = f"{PLUGINS_API_URL}/select-and-run-plugin"
         headers = cls.get_headers()
         if user_email:
             headers["X-User-Email"] = user_email
 
@@ -115,14 +116,66 @@
             PluginInfo(**p) for p in plugins_data["plugin_infos"]
         ]
         plugins_data = PluginResponse(**plugins_data)
 
         return plugins_data
 
     @classmethod
+    def select_and_run_plugins_stream(
+        cls,
+        messages: list[ChatMLMessage],
+        plugin_names: list[str],
+        model_settings: FCallModelSettings,
+        plugin_extra_args: Optional[dict[str, dict[str, str]]] = None,
+        user_email: Optional[str] = None,
+        schemaless: bool = True,
+    ):
+        if not plugin_names:
+            return PluginResponse(
+                selector_completion="",
+                plugin_infos=[],
+                error=f"No plugins in plugin_names",
+            )
+
+        if plugin_extra_args is None:
+            plugin_extra_args = {}
+        for plugin in plugin_extra_args:
+            plugin_extra_args[plugin]["schemaless"] = schemaless
+
+        sp = SelectPlugin(
+            messages=messages,
+            plugin_names=plugin_names,
+            model_settings=model_settings,
+            plugin_extra_arguments=plugin_extra_args,
+        )
+        sel_run_url = f"{PLUGINS_API_URL}/select-and-run-stream-plugin"
+        headers = cls.get_headers()
+        if user_email:
+            headers["X-User-Email"] = user_email
+
+        headers["X-Selection-Id"] = "True"
+        headers["X-Execution-Id"] = "True"
+
+        logger.debug(f"Requesting {sel_run_url}. Args: {sp}. Headers: {headers}.")
+
+        res = requests.post(
+            sel_run_url,
+            json=sp,
+            headers=headers,
+            stream=True,
+        )
+        try:
+            res.raise_for_status()
+        except requests.HTTPError as e:
+            raise exceptions.ErrorPluginAPISelectAndRun(
+                f"Request to {sel_run_url} did not work\nError: {e}. "
+            )
+        return map(json.loads, res.iter_lines())
+
+    @classmethod
     def run_selector(
         cls,
         messages: list[ChatMLMessage],
         plugin_names: list[str],
         model_settings: FCallModelSettings,
     ) -> PluginUsage:
         sp = SelectPlugin(
```

### Comparing `teia_sdk-0.1.7/teia_sdk/plugins/exceptions.py` & `teia_sdk-0.1.8/teia_sdk/plugins/exceptions.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk/plugins/schemas.py` & `teia_sdk-0.1.8/teia_sdk/plugins/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Optional, TypedDict
+from typing import Any, Literal, Optional, TypedDict
+
 from melting_schemas.completion.fcall import ChatMLMessage, FCallModelSettings
 
 
 class PluginInfo(TypedDict):
     name: str
     method: str
     params: dict[str, Any]
@@ -20,14 +21,15 @@
 
 
 class SelectPlugin(TypedDict):
     messages: list[ChatMLMessage]
     plugin_names: list[str]
     model_settings: FCallModelSettings
     plugin_extra_arguments: dict[str, dict[str, str]]
+    tool_choice: Optional[Literal["auto", "required"] | dict]
 
 
 class PluginUsage(TypedDict):
     plugin: str
     method: str
     arguments: dict[str, Any]
```

### Comparing `teia_sdk-0.1.7/teia_sdk/private_workspaces/client.py` & `teia_sdk-0.1.8/teia_sdk/private_workspaces/client.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk/private_workspaces/schemas.py` & `teia_sdk-0.1.8/teia_sdk/private_workspaces/schemas.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk/search/client.py` & `teia_sdk-0.1.8/teia_sdk/search/client.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk/search/search.py` & `teia_sdk-0.1.8/teia_sdk/search/search.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk/utils.py` & `teia_sdk-0.1.8/teia_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `teia_sdk-0.1.7/teia_sdk.egg-info/PKG-INFO` & `teia_sdk-0.1.8/teia_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: teia_sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: Teia SDK
 Home-page: https://github.com/TeiaLabs/teia-sdk
 Author: TeiaLabs
 Author-email: contato@teialabs.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fastapi
+Requires-Dist: fastapi==0.111.0
 Requires-Dist: http_error_schemas==1.0.1
-Requires-Dist: httpx
-Requires-Dist: melting_schemas==1.0.7
-Requires-Dist: python-dotenv
-Requires-Dist: requests
-Requires-Dist: rich
-Requires-Dist: typer[all]
+Requires-Dist: melting_schemas==1.0.9
+Requires-Dist: httpx==0.27.0
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: requests==2.32.2
+Requires-Dist: rich==13.7.1
+Requires-Dist: typer[all]==0.12.3
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # Teia SDK 🕸️
 
 # install 🕷️
 ```bash
```

### Comparing `teia_sdk-0.1.7/teia_sdk.egg-info/SOURCES.txt` & `teia_sdk-0.1.8/teia_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 teia_sdk/utils.py
 teia_sdk.egg-info/PKG-INFO
 teia_sdk.egg-info/SOURCES.txt
 teia_sdk.egg-info/dependency_links.txt
 teia_sdk.egg-info/entry_points.txt
 teia_sdk.egg-info/requires.txt
 teia_sdk.egg-info/top_level.txt
+teia_sdk/dbsailor/__init__.py
+teia_sdk/dbsailor/client.py
+teia_sdk/dbsailor/schemas.py
 teia_sdk/melting/__init__.py
 teia_sdk/melting/chat_prompts.py
 teia_sdk/melting/client.py
 teia_sdk/melting/schemas.py
 teia_sdk/melting/services/__init__.py
 teia_sdk/melting/services/chat_completions.py
 teia_sdk/melting/services/chat_prompts.py
```

### Comparing `teia_sdk-0.1.7/tests/test_plugins.py` & `teia_sdk-0.1.8/tests/test_plugins.py`

 * *Files identical despite different names*

