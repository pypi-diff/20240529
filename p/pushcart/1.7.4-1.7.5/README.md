# Comparing `tmp/pushcart-1.7.4.tar.gz` & `tmp/pushcart-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushcart-1.7.4.tar", max compression
+gzip compressed data, was "pushcart-1.7.5.tar", max compression
```

## Comparing `pushcart-1.7.4.tar` & `pushcart-1.7.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11358 2024-05-15 13:46:20.244227 pushcart-1.7.4/LICENSE.txt
--rw-r--r--   0        0        0     1261 2024-05-15 13:46:20.244227 pushcart-1.7.4/README.md
--rw-r--r--   0        0        0     4110 2024-05-16 08:10:55.356923 pushcart-1.7.4/pyproject.toml
--rw-r--r--   0        0        0       51 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/__init__.py
--rw-r--r--   0        0        0      599 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/log_handlers/__init__.py
--rw-r--r--   0        0        0     1077 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/log_handlers/app_insights_handler.py
--rw-r--r--   0        0        0      124 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/metadata/__init__.py
--rw-r--r--   0        0        0    17893 2024-05-16 07:08:22.680127 pushcart-1.7.4/src/pushcart/metadata/metadata.py
--rw-r--r--   0        0        0     6873 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/metadata/spark.py
--rw-r--r--   0        0        0        0 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/py.typed
--rw-r--r--   0        0        0      109 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/sources/__init__.py
--rw-r--r--   0        0        0    19054 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/sources/rest_api.py
--rw-r--r--   0        0        0     2615 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/utils.py
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 pushcart-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-16 12:27:56.670788 pushcart-1.7.5/LICENSE.txt
+-rw-r--r--   0        0        0     1261 2024-05-16 12:27:56.670788 pushcart-1.7.5/README.md
+-rw-r--r--   0        0        0     4502 2024-05-29 09:56:57.196716 pushcart-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0       51 2024-05-16 12:27:56.677455 pushcart-1.7.5/src/pushcart/__init__.py
+-rw-r--r--   0        0        0      599 2024-05-16 12:27:56.677455 pushcart-1.7.5/src/pushcart/log_handlers/__init__.py
+-rw-r--r--   0        0        0     1077 2024-05-16 12:27:56.677455 pushcart-1.7.5/src/pushcart/log_handlers/app_insights_handler.py
+-rw-r--r--   0        0        0      124 2024-05-16 12:27:56.677455 pushcart-1.7.5/src/pushcart/metadata/__init__.py
+-rw-r--r--   0        0        0    17893 2024-05-16 12:27:56.677455 pushcart-1.7.5/src/pushcart/metadata/metadata.py
+-rw-r--r--   0        0        0     6873 2024-05-16 12:27:56.677455 pushcart-1.7.5/src/pushcart/metadata/spark.py
+-rw-r--r--   0        0        0        0 2024-05-16 12:27:56.677455 pushcart-1.7.5/src/pushcart/py.typed
+-rw-r--r--   0        0        0      109 2024-05-16 12:27:56.677455 pushcart-1.7.5/src/pushcart/sources/__init__.py
+-rw-r--r--   0        0        0    19079 2024-05-16 12:27:56.677455 pushcart-1.7.5/src/pushcart/sources/rest_api.py
+-rw-r--r--   0        0        0     2615 2024-05-16 12:27:56.677455 pushcart-1.7.5/src/pushcart/utils.py
+-rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 pushcart-1.7.5/PKG-INFO
```

### Comparing `pushcart-1.7.4/LICENSE.txt` & `pushcart-1.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pushcart-1.7.4/README.md` & `pushcart-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pushcart-1.7.4/pyproject.toml` & `pushcart-1.7.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.pyright]
 include = ["src", "tests"]
 ignore = ["**/.pyenv"]
 exclude = ["**/.pyenv"]
 
 [tool.black]
 line-length = 88
-target-version = ["py311"]
+target-version = ["py310", "py311"]
 exclude = '''
 (
   /(
       \.git
     | \.github
     | \.venv
   )/
@@ -27,15 +27,15 @@
     "E501",   # Line too long
     "FBT001", # Boolean positional arg in function definition
     "FBT002", # Boolean default value in function definition
     "G004",   # Logging statement uses f-string
     "N812",   # Checks for lowercase imports that are aliased to non-lowercase names
     "S101",   # Use of `assert` detected
 ]
-target-version = "py311"
+target-version = "py310"
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 lint.fixable = [
     "A",
     "B",
     "C",
     "D",
@@ -86,56 +86,60 @@
 
 [tool.ruff.lint.per-file-ignores]
 "scratch/*" = ["D100", "E402", "ERA001", "INP001"]
 ".vscode/__builtins__.pyi" = ["D100", "INP001"]
 
 [tool.poetry]
 name = "pushcart"
-version = "1.7.4"
+version = "1.7.5"
 description = "Metadata transformations for Spark"
 authors = ["Victor Blaga <victor.blaga@revodata.nl>"]
 license = "Apache-2.0"
 readme = "README.md"
 classifiers = [
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Topic :: Database :: Database Engines/Servers",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [{ include = "pushcart", from = "src" }]
 
 [tool.poetry.dependencies]
 python-dotenv = "^1.0.1"
-python = "^3.11"
+python = "^3.10"
 loguru = "^0.7.2"
 azure-monitor-opentelemetry = "^1.4.0"
 opentelemetry-sdk = "^1.24.0"
 delta-spark = "^3.1.0"
 validators = "^0.28.1"
 httpx = "^0.27.0"
 authlib = "^1.3.0"
+mkdocstrings = { extras = ["python"], version = "^0.25.1" }
 
 [tool.poetry.group.dev.dependencies]
-# Matching DBR 15.0
-black = { version = "23.3.0", allow-prereleases = true }
-databricks-sdk = "0.20.0"
-ipykernel = "6.25.1"
-ipywidgets = "8.0.4"
-mypy-extensions = "^1.0.0"
-pandas = "2.0.3"
-pyarrow = "^14.0.1"
-pydantic = "1.10.6"
+# Matching >= DBR 14.3
+black = { version = "^22.6.0", allow-prereleases = true }
+databricks-sdk = "^0.1.6"
+ipykernel = "^6.25.0"
+ipywidgets = "^7.7.2"
+mypy-extensions = "*"                                     # ^0.4.3 in DBR 14.3 but local setup requires ^1.0.0
+pandas = "^1.5.3"
+pyarrow = "*"                                             # ^8.0.0 in DBR 14.3 but local setup fails without ^14.0.0
+pydantic = "^1.10.6"
 
 # Not in DBR
 bumpver = "^2023.1129"
 coverage = "^7.5.0"
 databricks-labs-pylint = "^0.4.0"
 ipydatagrid = "^1.3.1"
+mkdocs-material = "^9.5.23"
+mkdocstrings = { extras = ["python"], version = "^0.25.1" }
 mypy = "^1.5.1"
 pandas-stubs = "^2.2.0.240218"
 pre-commit = "^3.5.0"
 pylint = "^3.1.0"
 pyspark = "^3.5.1"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
@@ -151,29 +155,29 @@
 types-ujson = "^5.9.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "1.7.4"
+current_version = "1.7.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     '^version = "{version}"$',
     '^current_version = "{version}"$',
 ]
 
 [tool.mypy]
-python_version = "3.11"
+python_version = "3.10"
 ignore_missing_imports = true
 mypy_path = "./stubs"
 files = "src/**/*.py, tests/**/*.py"
 exclude = [".venv/"]
 pretty = true
 
 [[tool.mypy.overrides]]
```

### Comparing `pushcart-1.7.4/src/pushcart/log_handlers/__init__.py` & `pushcart-1.7.5/src/pushcart/log_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pushcart-1.7.4/src/pushcart/log_handlers/app_insights_handler.py` & `pushcart-1.7.5/src/pushcart/log_handlers/app_insights_handler.py`

 * *Files identical despite different names*

### Comparing `pushcart-1.7.4/src/pushcart/metadata/metadata.py` & `pushcart-1.7.5/src/pushcart/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `pushcart-1.7.4/src/pushcart/metadata/spark.py` & `pushcart-1.7.5/src/pushcart/metadata/spark.py`

 * *Files identical despite different names*

### Comparing `pushcart-1.7.4/src/pushcart/sources/rest_api.py` & `pushcart-1.7.5/src/pushcart/sources/rest_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""A custom DataSource implementation for reading data from a REST API."""
+"""A custom DataSource implementation for reading data from a REST API. Requires PySpark >= 4.0."""
 
 import contextlib
 import json
 from ast import literal_eval
 from collections.abc import Generator, Hashable
 from typing import Any
 from urllib.parse import parse_qs, urlparse, urlunparse
```

### Comparing `pushcart-1.7.4/src/pushcart/utils.py` & `pushcart-1.7.5/src/pushcart/utils.py`

 * *Files identical despite different names*

### Comparing `pushcart-1.7.4/PKG-INFO` & `pushcart-1.7.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: pushcart
-Version: 1.7.4
+Version: 1.7.5
 Summary: Metadata transformations for Spark
 License: Apache-2.0
 Author: Victor Blaga
 Author-email: victor.blaga@revodata.nl
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: authlib (>=1.3.0,<2.0.0)
 Requires-Dist: azure-monitor-opentelemetry (>=1.4.0,<2.0.0)
 Requires-Dist: delta-spark (>=3.1.0,<4.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: mkdocstrings[python] (>=0.25.1,<0.26.0)
 Requires-Dist: opentelemetry-sdk (>=1.24.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: validators (>=0.28.1,<0.29.0)
 Description-Content-Type: text/markdown
 
 # pushcart
```

