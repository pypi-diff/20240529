# Comparing `tmp/airgradient-0.4.1.tar.gz` & `tmp/airgradient-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airgradient-0.4.1.tar", max compression
+gzip compressed data, was "airgradient-0.4.2.tar", max compression
```

## Comparing `airgradient-0.4.1.tar` & `airgradient-0.4.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-05-23 07:34:37.146370 airgradient-0.4.1/LICENSE.md
--rw-r--r--   0        0        0     4673 2024-05-23 07:34:37.146370 airgradient-0.4.1/README.md
--rw-r--r--   0        0        0     3857 2024-05-23 07:34:51.474289 airgradient-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      540 2024-05-23 07:34:37.150370 airgradient-0.4.1/src/airgradient/__init__.py
--rw-r--r--   0        0        0     3893 2024-05-23 07:34:37.150370 airgradient-0.4.1/src/airgradient/airgradient.py
--rw-r--r--   0        0        0      214 2024-05-23 07:34:37.150370 airgradient-0.4.1/src/airgradient/exceptions.py
--rw-r--r--   0        0        0     2728 2024-05-23 07:34:37.150370 airgradient-0.4.1/src/airgradient/models.py
--rw-r--r--   0        0        0        0 2024-05-23 07:34:37.150370 airgradient-0.4.1/src/airgradient/py.typed
--rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 airgradient-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-29 15:53:56.953089 airgradient-0.4.2/LICENSE.md
+-rw-r--r--   0        0        0     4673 2024-05-29 15:53:56.953089 airgradient-0.4.2/README.md
+-rw-r--r--   0        0        0     3857 2024-05-29 15:54:10.309024 airgradient-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      540 2024-05-29 15:53:56.953089 airgradient-0.4.2/src/airgradient/__init__.py
+-rw-r--r--   0        0        0     3893 2024-05-29 15:53:56.953089 airgradient-0.4.2/src/airgradient/airgradient.py
+-rw-r--r--   0        0        0      214 2024-05-29 15:53:56.953089 airgradient-0.4.2/src/airgradient/exceptions.py
+-rw-r--r--   0        0        0     2728 2024-05-29 15:53:56.953089 airgradient-0.4.2/src/airgradient/models.py
+-rw-r--r--   0        0        0        0 2024-05-29 15:53:56.953089 airgradient-0.4.2/src/airgradient/py.typed
+-rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 airgradient-0.4.2/PKG-INFO
```

### Comparing `airgradient-0.4.1/LICENSE.md` & `airgradient-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `airgradient-0.4.1/README.md` & `airgradient-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `airgradient-0.4.1/pyproject.toml` & `airgradient-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airgradient"
-version = "0.4.1"
+version = "0.4.2"
 description = "Asynchronous Python client for AirGradient."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/airgradienthq/python-airgradient"
 repository = "https://github.com/airgradienthq/python-airgradient"
@@ -28,25 +28,25 @@
 python = "^3.11"
 aiohttp = ">=3.0.0"
 yarl = ">=1.6.0"
 mashumaro = "^3.11"
 orjson = ">=3.9.0"
 
 [tool.poetry.group.dev.dependencies]
-codespell = "2.2.6"
+codespell = "2.3.0"
 covdefaults = "2.3.0"
-coverage = {version = "7.5.1", extras = ["toml"]}
+coverage = {version = "7.5.3", extras = ["toml"]}
 mypy = "1.10.0"
 pre-commit = "3.7.1"
 pre-commit-hooks = "4.6.0"
-pylint = "3.1.0"
+pylint = "3.2.2"
 pytest = "8.2.1"
-pytest-asyncio = "0.23.6"
+pytest-asyncio = "0.23.7"
 pytest-cov = "5.0.0"
-ruff = "0.4.4"
+ruff = "0.4.6"
 safety = "3.2.0"
 yamllint = "1.35.1"
 syrupy = "4.6.1"
 aioresponses = "0.7.6"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/airgradienthq/python-airgradient/issues"
```

### Comparing `airgradient-0.4.1/src/airgradient/__init__.py` & `airgradient-0.4.2/src/airgradient/__init__.py`

 * *Files identical despite different names*

### Comparing `airgradient-0.4.1/src/airgradient/airgradient.py` & `airgradient-0.4.2/src/airgradient/airgradient.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             self._close_session = True
 
         async with timeout(self.request_timeout):
             response = await self.session.request(
                 method,
                 url,
                 headers=headers,
-                data=data,
+                json=data,
             )
 
         if response.status != 200:
             content_type = response.headers.get("Content-Type", "")
             text = await response.text()
             msg = "Unexpected response from AirGradient"
             raise AirGradientConnectionError(
```

### Comparing `airgradient-0.4.1/src/airgradient/models.py` & `airgradient-0.4.2/src/airgradient/models.py`

 * *Files identical despite different names*

### Comparing `airgradient-0.4.1/PKG-INFO` & `airgradient-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgradient
-Version: 0.4.1
+Version: 0.4.2
 Summary: Asynchronous Python client for AirGradient.
 Home-page: https://github.com/airgradienthq/python-airgradient
 License: MIT
 Keywords: Airgradient,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
```

