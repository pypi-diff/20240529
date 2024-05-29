# Comparing `tmp/sciobject-0.0.1.tar.gz` & `tmp/sciobject-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciobject-0.0.1.tar", max compression
+gzip compressed data, was "sciobject-0.0.2.tar", max compression
```

## Comparing `sciobject-0.0.1.tar` & `sciobject-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1298 2024-05-27 08:59:13.510264 sciobject-0.0.1/LICENSE
--rw-r--r--   0        0        0      200 2024-05-27 08:59:13.514264 sciobject-0.0.1/README.md
--rw-r--r--   0        0        0      647 2024-05-29 11:06:17.949640 sciobject-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 11:04:55.328502 sciobject-0.0.1/sciobject/__init__.py
--rw-r--r--   0        0        0    12931 2024-05-29 11:05:44.229176 sciobject-0.0.1/sciobject/sciobject.py
--rw-r--r--   0        0        0     1006 2024-05-29 09:55:24.615094 sciobject-0.0.1/sciobject/test_sciobject.py
--rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 sciobject-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1298 2024-05-27 08:59:13.510264 sciobject-0.0.2/LICENSE
+-rw-r--r--   0        0        0      200 2024-05-27 08:59:13.514264 sciobject-0.0.2/README.md
+-rw-r--r--   0        0        0      644 2024-05-29 11:28:22.507874 sciobject-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 11:04:55.328502 sciobject-0.0.2/sciobject/__init__.py
+-rw-r--r--   0        0        0    12947 2024-05-29 11:28:02.439598 sciobject-0.0.2/sciobject/sciobject.py
+-rw-r--r--   0        0        0     1006 2024-05-29 09:55:24.615094 sciobject-0.0.2/sciobject/test_sciobject.py
+-rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 sciobject-0.0.2/PKG-INFO
```

### Comparing `sciobject-0.0.1/LICENSE` & `sciobject-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sciobject-0.0.1/pyproject.toml` & `sciobject-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "sciobject"
-version = "0.0.1"
+version = "0.0.2"
 description = "Abstract objects that save and log calculations."
-authors = ["Hana Zupan <hana.zupan@fu-berlin.de>"]
+authors = ["Hana Zupan <h.zupan@fu-berlin.de>"]
 license = "LICENSE"
 readme = "README.md"
 keywords = ["scientific computing", "logging"]
 repository = "https://github.com/hanazupan/sciobject"
 homepage = "https://www.bcp.fu-berlin.de/en/chemie/chemie/forschung/PhysTheoChem/agkeller/index.html"
 
 [tool.poetry.dependencies]
```

### Comparing `sciobject-0.0.1/sciobject/sciobject.py` & `sciobject-0.0.2/sciobject/sciobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 from functools import wraps
 from typing import Callable
 
 import numpy as np
 import pandas as pd
 from pandas.errors import EmptyDataError
 
-PATH_OUTPUT_LOGGING = "../data/logging/"
-PATH_OUTPUT_AUTOSAVE = "../data/autosave/"
-PATH_OUTPUT_LOGBOOK = "../data/logbook/"
-PATH_OUTPUT_METHODBOOK = "../data/methodbook/"
+PATH_OUTPUT_LOGGING = "output/data/logging/"
+PATH_OUTPUT_AUTOSAVE = "output/data/autosave/"
+PATH_OUTPUT_LOGBOOK = "output/data/logbook/"
+PATH_OUTPUT_METHODBOOK = "output/data/methodbook/"
 
 LOGGING_PATHS = [PATH_OUTPUT_LOGGING, PATH_OUTPUT_AUTOSAVE, PATH_OUTPUT_LOGBOOK, PATH_OUTPUT_METHODBOOK]
 
 
 def freshly_create_log_folders():
     for path in LOGGING_PATHS:
         if not os.path.exists(path):
```

### Comparing `sciobject-0.0.1/sciobject/test_sciobject.py` & `sciobject-0.0.2/sciobject/test_sciobject.py`

 * *Files identical despite different names*

### Comparing `sciobject-0.0.1/PKG-INFO` & `sciobject-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sciobject
-Version: 0.0.1
+Version: 0.0.2
 Summary: Abstract objects that save and log calculations.
 Home-page: https://www.bcp.fu-berlin.de/en/chemie/chemie/forschung/PhysTheoChem/agkeller/index.html
 License: LICENSE
 Keywords: scientific computing,logging
 Author: Hana Zupan
-Author-email: hana.zupan@fu-berlin.de
+Author-email: h.zupan@fu-berlin.de
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

