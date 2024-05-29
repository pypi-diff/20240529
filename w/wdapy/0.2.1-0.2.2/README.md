# Comparing `tmp/wdapy-0.2.1.tar.gz` & `tmp/wdapy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wdapy-0.2.1.tar", last modified: Mon Jan  8 09:18:28 2024, max compression
+gzip compressed data, was "wdapy-0.2.2.tar", last modified: Wed May 29 09:04:18 2024, max compression
```

## Comparing `wdapy-0.2.1.tar` & `wdapy-0.2.2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:18:28.269366 wdapy-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-08 09:18:14.000000 wdapy-0.2.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:18:28.265366 wdapy-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:18:28.265366 wdapy-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-01-08 09:18:14.000000 wdapy-0.2.1/.github/workflows/publish_to_pypi.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:18:28.265366 wdapy-0.2.1/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-01-08 09:18:14.000000 wdapy-0.2.1/.idea/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:18:28.265366 wdapy-0.2.1/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-08 09:18:14.000000 wdapy-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-01-08 09:18:14.000000 wdapy-0.2.1/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-08 09:18:14.000000 wdapy-0.2.1/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-08 09:18:14.000000 wdapy-0.2.1/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-01-08 09:18:14.000000 wdapy-0.2.1/.idea/wdapy.iml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-08 09:18:27.000000 wdapy-0.2.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-08 09:18:27.000000 wdapy-0.2.1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-08 09:18:14.000000 wdapy-0.2.1/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-01-08 09:18:14.000000 wdapy-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-01-08 09:18:28.269366 wdapy-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-01-08 09:18:14.000000 wdapy-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-01-08 09:18:14.000000 wdapy-0.2.1/README_CN.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-08 09:18:14.000000 wdapy-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-08 09:18:28.269366 wdapy-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-08 09:18:14.000000 wdapy-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:18:28.265366 wdapy-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-01-08 09:18:14.000000 wdapy-0.2.1/tests/test_common_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-01-08 09:18:14.000000 wdapy-0.2.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:18:28.269366 wdapy-0.2.1/wdapy/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-08 09:18:14.000000 wdapy-0.2.1/wdapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-01-08 09:18:14.000000 wdapy-0.2.1/wdapy/_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-01-08 09:18:14.000000 wdapy-0.2.1/wdapy/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-08 09:18:14.000000 wdapy-0.2.1/wdapy/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-01-08 09:18:14.000000 wdapy-0.2.1/wdapy/_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-01-08 09:18:14.000000 wdapy-0.2.1/wdapy/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-08 09:18:14.000000 wdapy-0.2.1/wdapy/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13049 2024-01-08 09:18:14.000000 wdapy-0.2.1/wdapy/_wdapy.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-08 09:18:14.000000 wdapy-0.2.1/wdapy/_wrap.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-08 09:18:14.000000 wdapy-0.2.1/wdapy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:18:28.269366 wdapy-0.2.1/wdapy/usbmux/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-08 09:18:14.000000 wdapy-0.2.1/wdapy/usbmux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-01-08 09:18:14.000000 wdapy-0.2.1/wdapy/usbmux/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-01-08 09:18:14.000000 wdapy-0.2.1/wdapy/usbmux/usbmux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:18:28.269366 wdapy-0.2.1/wdapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-01-08 09:18:27.000000 wdapy-0.2.1/wdapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-01-08 09:18:28.000000 wdapy-0.2.1/wdapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 09:18:27.000000 wdapy-0.2.1/wdapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 09:18:27.000000 wdapy-0.2.1/wdapy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-08 09:18:27.000000 wdapy-0.2.1/wdapy.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-08 09:18:27.000000 wdapy-0.2.1/wdapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-08 09:18:27.000000 wdapy-0.2.1/wdapy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:18.548462 wdapy-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-29 09:04:08.000000 wdapy-0.2.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:18.544462 wdapy-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:18.544462 wdapy-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-29 09:04:08.000000 wdapy-0.2.2/.github/workflows/publish_to_pypi.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:18.548462 wdapy-0.2.2/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 09:04:08.000000 wdapy-0.2.2/.idea/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:18.548462 wdapy-0.2.2/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-29 09:04:08.000000 wdapy-0.2.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 09:04:08.000000 wdapy-0.2.2/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-29 09:04:08.000000 wdapy-0.2.2/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 09:04:08.000000 wdapy-0.2.2/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-29 09:04:08.000000 wdapy-0.2.2/.idea/wdapy.iml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 09:04:18.000000 wdapy-0.2.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-29 09:04:18.000000 wdapy-0.2.2/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-29 09:04:08.000000 wdapy-0.2.2/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-29 09:04:08.000000 wdapy-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-29 09:04:18.548462 wdapy-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-29 09:04:08.000000 wdapy-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-29 09:04:08.000000 wdapy-0.2.2/README_CN.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:18.548462 wdapy-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-29 09:04:08.000000 wdapy-0.2.2/examples/swipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 09:04:08.000000 wdapy-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-29 09:04:18.552462 wdapy-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-29 09:04:08.000000 wdapy-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:18.548462 wdapy-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-29 09:04:08.000000 wdapy-0.2.2/tests/test_common_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-29 09:04:08.000000 wdapy-0.2.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:18.548462 wdapy-0.2.2/wdapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-29 09:04:08.000000 wdapy-0.2.2/wdapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-29 09:04:08.000000 wdapy-0.2.2/wdapy/_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-29 09:04:08.000000 wdapy-0.2.2/wdapy/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-29 09:04:08.000000 wdapy-0.2.2/wdapy/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-29 09:04:08.000000 wdapy-0.2.2/wdapy/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-29 09:04:08.000000 wdapy-0.2.2/wdapy/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-05-29 09:04:08.000000 wdapy-0.2.2/wdapy/_wdapy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-29 09:04:08.000000 wdapy-0.2.2/wdapy/_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-29 09:04:08.000000 wdapy-0.2.2/wdapy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:18.548462 wdapy-0.2.2/wdapy/usbmux/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-29 09:04:08.000000 wdapy-0.2.2/wdapy/usbmux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-29 09:04:08.000000 wdapy-0.2.2/wdapy/usbmux/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-05-29 09:04:08.000000 wdapy-0.2.2/wdapy/usbmux/pyusbmux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:18.548462 wdapy-0.2.2/wdapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-29 09:04:18.000000 wdapy-0.2.2/wdapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-29 09:04:18.000000 wdapy-0.2.2/wdapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:04:18.000000 wdapy-0.2.2/wdapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:04:18.000000 wdapy-0.2.2/wdapy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-29 09:04:18.000000 wdapy-0.2.2/wdapy.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 09:04:18.000000 wdapy-0.2.2/wdapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 09:04:18.000000 wdapy-0.2.2/wdapy.egg-info/top_level.txt
```

### Comparing `wdapy-0.2.1/.github/workflows/publish_to_pypi.yml` & `wdapy-0.2.2/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `wdapy-0.2.1/.idea/wdapy.iml` & `wdapy-0.2.2/.idea/wdapy.iml`

 * *Files identical despite different names*

### Comparing `wdapy-0.2.1/LICENSE` & `wdapy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wdapy-0.2.1/PKG-INFO` & `wdapy-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: wdapy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Client for Facebook WebDriverAgent
 Home-page: https://github.com/openatx/wdapy
 Author: "codeskyblue"
-Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.8
```

### Comparing `wdapy-0.2.1/README.md` & `wdapy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `wdapy-0.2.1/README_CN.md` & `wdapy-0.2.2/README_CN.md`

 * *Files identical despite different names*

### Comparing `wdapy-0.2.1/setup.cfg` & `wdapy-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `wdapy-0.2.1/tests/test_common_client.py` & `wdapy-0.2.2/tests/test_common_client.py`

 * *Files identical despite different names*

### Comparing `wdapy-0.2.1/tests/test_utils.py` & `wdapy-0.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wdapy-0.2.1/wdapy/_alert.py` & `wdapy-0.2.2/wdapy/_alert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """Created on Tue Sep 14 2021 15:24:46 by codeskyblue
 """
 
+import logging
 import typing
 from wdapy.exceptions import RequestError
 from wdapy._proto import *
 from wdapy._base import BaseClient
-from wdapy._logger import logger
 
+logger = logging.getLogger(__name__)
 
 class Alert:
     def __init__(self, client: BaseClient):
         self._client = client
         
     @property
     def exists(self) -> bool:
```

### Comparing `wdapy-0.2.1/wdapy/_proto.py` & `wdapy-0.2.2/wdapy/_proto.py`

 * *Files identical despite different names*

### Comparing `wdapy-0.2.1/wdapy/_types.py` & `wdapy-0.2.2/wdapy/_types.py`

 * *Files identical despite different names*

### Comparing `wdapy-0.2.1/wdapy/_utils.py` & `wdapy-0.2.2/wdapy/_utils.py`

 * *Files identical despite different names*

### Comparing `wdapy-0.2.1/wdapy/_wdapy.py` & `wdapy-0.2.2/wdapy/_wdapy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,47 @@
 # coding: utf-8
 
 from __future__ import annotations
 
 import atexit
 import base64
 import io
-import json
-import logging
 import queue
 import subprocess
 import sys
 import threading
 import time
 import typing
 
-import requests
-from cached_property import cached_property
-from logzero import setup_logger
+from functools import cached_property
 from PIL import Image
 
 from wdapy._alert import Alert
 from wdapy._base import BaseClient
-from wdapy._logger import logger
 from wdapy._proto import *
 from wdapy._types import *
 from wdapy.exceptions import *
 from wdapy._utils import omit_empty
-from wdapy.usbmux import requests_usbmux, usbmux
+from wdapy.usbmux.pyusbmux import list_devices
 
 
-class HTTPResponse:
-    def __init__(self, resp: requests.Response, err: requests.RequestException):
-        self._resp = resp
-        self._err = err
-
-    def is_success(self) -> bool:
-        return self._err is None and self._resp.status_code == 200
-
-    def json(self) -> dict:
-        assert self._resp is not None
-        try:
-            return self._resp.json()
-        except json.JSONDecodeError:
-            return RequestError("JSON decode error", self._resp.text)
-
-    def get_error_message(self) -> str:
-        if self._resp:
-            return self._resp.text
-        return str(self._err)
-
-    def raise_if_failed(self):
-        if self._err:
-            raise RequestError("HTTP request error", self._err)
-        if self._resp.status_code != 200:
-            raise RequestError(self._resp.status_code, self._resp.text)
-
 
 class CommonClient(BaseClient):
     def __init__(self, wda_url: str):
         super().__init__(wda_url)
         self.__ui_size = None
         self.__debug = False
 
     @property
     def debug(self) -> bool:
         return self.__debug
 
     @debug.setter
     def debug(self, v: bool):
-        if v:
-            setup_logger(NAME)
-        else:
-            setup_logger(NAME, level=logging.INFO)
+        self.__debug = v
 
     def app_start(self, bundle_id: str, arguments: typing.List[str] = [], environment: typing.Dict[str, str] = {}):
         self.session_request(POST, "/wda/apps/launch", {
             "bundleId": bundle_id,
             "arguments": arguments,
             "environment": environment,
         })
@@ -189,15 +155,18 @@
         #     return self.__ui_size
 
     def send_keys(self, value: str):
         """ input with some text """
         self.session_request(POST, "/wda/keys", {"value": list(value)})
 
     def tap(self, x: int, y: int):
-        self.session_request(POST, "/wda/tap/0", {"x": x, "y": y})
+        try:
+            self.session_request(POST, "/wda/tap", {"x": x, "y": y})
+        except RequestError:
+            self.session_request(POST, "/wda/tap/0", {"x": x, "y": y})
     
     def touch_and_hold(self, x: int, y: int, duration: float):
         """ touch and hold
         
         Ref:
             FBElementCommands.m
         """
@@ -357,20 +326,28 @@
     client for https://github.com/appium/WebDriverAgent
     """
 
     def __init__(self, wda_url: str = DEFAULT_WDA_URL):
         super().__init__(wda_url)
 
 
+def get_single_device_udid() -> str:
+    devices = list_devices()
+    if len(devices) == 0:
+        raise WDAException("No device connected")
+    if len(devices) > 1:
+        raise WDAException("More than one device connected")
+    return devices[0].serial
+
+
 class AppiumUSBClient(AppiumClient):
     def __init__(self, udid: str = None, port: int = 8100):
         if udid is None:
-            _usbmux = usbmux.Usbmux()
-            udid = _usbmux.get_single_device_udid()
-        super().__init__(requests_usbmux.DEFAULT_SCHEME+udid+f":{port}")
+            udid = get_single_device_udid()
+        super().__init__(f"http+usbmux://{udid}:{port}")
         self.set_recover_handler(XCUITestRecover(udid))
 
 
 class NanoClient(AppiumClient):
     """
     Repo: https://github.com/nanoscopic/WebDriverAgent
 
@@ -400,11 +377,10 @@
             "y2": to_y,
             "delay": duration})
 
 
 class NanoUSBClient(NanoClient):
     def __init__(self, udid: str = None, port: int = 8100):
         if udid is None:
-            _usbmux = usbmux.Usbmux()
-            udid = _usbmux.get_single_device_udid()
-        super().__init__(requests_usbmux.DEFAULT_SCHEME+udid+f":{port}")
+            udid = get_single_device_udid()
+        super().__init__(f"http+usbmux://{udid}:{port}")
         self.set_recover_handler(XCUITestRecover(udid))
```

### Comparing `wdapy-0.2.1/wdapy/_wrap.py` & `wdapy-0.2.2/wdapy/_wrap.py`

 * *Files identical despite different names*

### Comparing `wdapy-0.2.1/wdapy.egg-info/PKG-INFO` & `wdapy-0.2.2/wdapy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: wdapy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Client for Facebook WebDriverAgent
 Home-page: https://github.com/openatx/wdapy
 Author: "codeskyblue"
-Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.8
```

### Comparing `wdapy-0.2.1/wdapy.egg-info/SOURCES.txt` & `wdapy-0.2.2/wdapy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 .github/workflows/publish_to_pypi.yml
 .idea/.gitignore
 .idea/misc.xml
 .idea/modules.xml
 .idea/vcs.xml
 .idea/wdapy.iml
 .idea/inspectionProfiles/profiles_settings.xml
+examples/swipe.py
 tests/test_common_client.py
 tests/test_utils.py
 wdapy/__init__.py
 wdapy/_alert.py
 wdapy/_base.py
-wdapy/_logger.py
 wdapy/_proto.py
 wdapy/_types.py
 wdapy/_utils.py
 wdapy/_wdapy.py
 wdapy/_wrap.py
 wdapy/exceptions.py
 wdapy.egg-info/PKG-INFO
 wdapy.egg-info/SOURCES.txt
 wdapy.egg-info/dependency_links.txt
 wdapy.egg-info/not-zip-safe
 wdapy.egg-info/pbr.json
 wdapy.egg-info/requires.txt
 wdapy.egg-info/top_level.txt
 wdapy/usbmux/__init__.py
-wdapy/usbmux/requests_usbmux.py
-wdapy/usbmux/usbmux.py
+wdapy/usbmux/exceptions.py
+wdapy/usbmux/pyusbmux.py
```

