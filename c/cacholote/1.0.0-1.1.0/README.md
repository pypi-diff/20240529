# Comparing `tmp/cacholote-1.0.0.tar.gz` & `tmp/cacholote-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacholote-1.0.0.tar", last modified: Wed May 22 11:35:24 2024, max compression
+gzip compressed data, was "cacholote-1.1.0.tar", last modified: Wed May 29 09:24:11 2024, max compression
```

## Comparing `cacholote-1.0.0.tar` & `cacholote-1.1.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.951754 cacholote-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-22 11:35:15.000000 cacholote-1.0.0/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.939754 cacholote-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.943754 cacholote-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-22 11:35:15.000000 cacholote-1.0.0/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-05-22 11:35:15.000000 cacholote-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-22 11:35:15.000000 cacholote-1.0.0/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-22 11:35:15.000000 cacholote-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-22 11:35:15.000000 cacholote-1.0.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-22 11:35:15.000000 cacholote-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-22 11:35:15.000000 cacholote-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-22 11:35:24.951754 cacholote-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-22 11:35:15.000000 cacholote-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.943754 cacholote-1.0.0/cacholote/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    12756 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/encode.py
--rw-r--r--   0 runner    (1001) docker     (127)    13947 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/extra_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 11:35:24.000000 cacholote-1.0.0/cacholote/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.951754 cacholote-1.0.0/cacholote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-22 11:35:24.000000 cacholote-1.0.0/cacholote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-22 11:35:24.000000 cacholote-1.0.0/cacholote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:35:24.000000 cacholote-1.0.0/cacholote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-22 11:35:24.000000 cacholote-1.0.0/cacholote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:35:24.000000 cacholote-1.0.0/cacholote.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.947754 cacholote-1.0.0/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-22 11:35:15.000000 cacholote-1.0.0/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-22 11:35:15.000000 cacholote-1.0.0/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.947754 cacholote-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/DESIGN.rst
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/OBJECT-STORAGE-DESIGN.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.947754 cacholote-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.947754 cacholote-1.0.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 11:35:15.000000 cacholote-1.0.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-22 11:35:15.000000 cacholote-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:35:24.951754 cacholote-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.951754 cacholote-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_01_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_02_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_10_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_20_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_30_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_40_xarray_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_50_io_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_60_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:24:11.708755 cacholote-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-29 09:24:02.000000 cacholote-1.1.0/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:24:11.700755 cacholote-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:24:11.704755 cacholote-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-29 09:24:02.000000 cacholote-1.1.0/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-05-29 09:24:02.000000 cacholote-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-29 09:24:02.000000 cacholote-1.1.0/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-29 09:24:02.000000 cacholote-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-29 09:24:02.000000 cacholote-1.1.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-29 09:24:02.000000 cacholote-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-29 09:24:02.000000 cacholote-1.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-29 09:24:11.708755 cacholote-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-29 09:24:02.000000 cacholote-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:24:11.704755 cacholote-1.1.0/cacholote/
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-29 09:24:02.000000 cacholote-1.1.0/cacholote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-29 09:24:02.000000 cacholote-1.1.0/cacholote/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12756 2024-05-29 09:24:02.000000 cacholote-1.1.0/cacholote/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-05-29 09:24:02.000000 cacholote-1.1.0/cacholote/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-29 09:24:02.000000 cacholote-1.1.0/cacholote/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-29 09:24:02.000000 cacholote-1.1.0/cacholote/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-29 09:24:02.000000 cacholote-1.1.0/cacholote/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14333 2024-05-29 09:24:02.000000 cacholote-1.1.0/cacholote/extra_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:24:02.000000 cacholote-1.1.0/cacholote/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-29 09:24:02.000000 cacholote-1.1.0/cacholote/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 09:24:11.000000 cacholote-1.1.0/cacholote/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:24:11.708755 cacholote-1.1.0/cacholote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-29 09:24:11.000000 cacholote-1.1.0/cacholote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-29 09:24:11.000000 cacholote-1.1.0/cacholote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:24:11.000000 cacholote-1.1.0/cacholote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 09:24:11.000000 cacholote-1.1.0/cacholote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 09:24:11.000000 cacholote-1.1.0/cacholote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:24:11.708755 cacholote-1.1.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-29 09:24:02.000000 cacholote-1.1.0/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-29 09:24:02.000000 cacholote-1.1.0/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:24:11.708755 cacholote-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-29 09:24:02.000000 cacholote-1.1.0/docs/DESIGN.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-29 09:24:02.000000 cacholote-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-29 09:24:02.000000 cacholote-1.1.0/docs/OBJECT-STORAGE-DESIGN.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:24:11.708755 cacholote-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:24:02.000000 cacholote-1.1.0/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:24:11.708755 cacholote-1.1.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:24:02.000000 cacholote-1.1.0/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-29 09:24:02.000000 cacholote-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-29 09:24:02.000000 cacholote-1.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-29 09:24:02.000000 cacholote-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-29 09:24:02.000000 cacholote-1.1.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-29 09:24:02.000000 cacholote-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:24:11.708755 cacholote-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:24:11.708755 cacholote-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-29 09:24:02.000000 cacholote-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-29 09:24:02.000000 cacholote-1.1.0/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-29 09:24:02.000000 cacholote-1.1.0/tests/test_01_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-29 09:24:02.000000 cacholote-1.1.0/tests/test_02_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-29 09:24:02.000000 cacholote-1.1.0/tests/test_10_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-29 09:24:02.000000 cacholote-1.1.0/tests/test_20_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-05-29 09:24:02.000000 cacholote-1.1.0/tests/test_30_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-29 09:24:02.000000 cacholote-1.1.0/tests/test_40_xarray_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-29 09:24:02.000000 cacholote-1.1.0/tests/test_50_io_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-29 09:24:02.000000 cacholote-1.1.0/tests/test_60_clean.py
```

### Comparing `cacholote-1.0.0/.cruft.json` & `cacholote-1.1.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/.github/workflows/on-push.yml` & `cacholote-1.1.0/.github/workflows/on-push.yml`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/.gitignore` & `cacholote-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/.pre-commit-config.yaml` & `cacholote-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/LICENSE` & `cacholote-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/Makefile` & `cacholote-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/PKG-INFO` & `cacholote-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 1.0.0
+Version: 1.1.0
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cacholote-1.0.0/README.md` & `cacholote-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/cacholote/__init__.py` & `cacholote-1.1.0/cacholote/__init__.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/cacholote/cache.py` & `cacholote-1.1.0/cacholote/cache.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/cacholote/clean.py` & `cacholote-1.1.0/cacholote/clean.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/cacholote/config.py` & `cacholote-1.1.0/cacholote/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
+import abc
 import datetime
 import logging
 import pathlib
 import tempfile
 from types import TracebackType
 from typing import Any, Literal, Optional, Union
 
@@ -37,14 +38,22 @@
 _DEFAULT_CACHE_DB_URLPATH = f"sqlite:///{_DEFAULT_CACHE_DIR / 'cacholote.db'}"
 _DEFAULT_CACHE_FILES_URLPATH = f"{_DEFAULT_CACHE_DIR / 'cache_files'}"
 _DEFAULT_LOGGER = structlog.get_logger(
     wrapper_class=structlog.make_filtering_bound_logger(logging.WARNING)
 )
 
 
+class Context(abc.ABC):
+    @abc.abstractmethod
+    def __init__(self, *args: Any, **kwargs: Any) -> None: ...
+
+    @abc.abstractmethod
+    def upload_log(self, *args: Any, **kwargs: Any) -> None: ...
+
+
 class Settings(pydantic_settings.BaseSettings):
     use_cache: bool = True
     cache_db_urlpath: Optional[str] = _DEFAULT_CACHE_DB_URLPATH
     create_engine_kwargs: dict[str, Any] = {}
     sessionmaker: Optional[sa.orm.sessionmaker[sa.orm.Session]] = None
     cache_files_urlpath: str = _DEFAULT_CACHE_FILES_URLPATH
     cache_files_urlpath_readonly: Optional[str] = None
@@ -57,14 +66,15 @@
     expiration: Optional[datetime.datetime] = None
     tag: Optional[str] = None
     return_cache_entry: bool = False
     logger: Union[structlog.BoundLogger, structlog._config.BoundLoggerLazyProxy] = (
         _DEFAULT_LOGGER
     )
     lock_timeout: Optional[float] = None
+    context: Optional[Context] = None
 
     @pydantic.field_validator("create_engine_kwargs")
     def validate_create_engine_kwargs(
         cls: pydantic_settings.BaseSettings, create_engine_kwargs: dict[str, Any]
     ) -> dict[str, Any]:
         poolclass = create_engine_kwargs.get("poolclass")
         if isinstance(poolclass, str):
@@ -147,16 +157,18 @@
     expiration: datetime, optional, default: None
         Expiration for cached results.
     tag: str, optional, default: None
         Tag for the cache entry. If None, do NOT tag.
         Note that existing tags are overwritten.
     return_cache_entry: bool, default: False
         Whether to return the cache database entry rather than decoded results.
-    lock_timeout: fload, optional, default: None
+    lock_timeout: float, optional, default: None
         Time to wait before raising an error if a cache file is locked.
+    context: Context, optional, default: None
+        CADS context for internal use.
     """
 
     def __init__(self, **kwargs: Any):
         self._old_settings = get()
 
         model_dump = self._old_settings.model_dump()
         if kwargs.get("cache_db_urlpath"):
```

### Comparing `cacholote-1.0.0/cacholote/database.py` & `cacholote-1.1.0/cacholote/database.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/cacholote/decode.py` & `cacholote-1.1.0/cacholote/decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/cacholote/encode.py` & `cacholote-1.1.0/cacholote/encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/cacholote/extra_encoders.py` & `cacholote-1.1.0/cacholote/extra_encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,23 +107,34 @@
     return cast(F, wrapper)
 
 
 def _filesystem_is_local(fs: fsspec.AbstractFileSystem) -> bool:
     return isinstance(fs, fsspec.get_filesystem_class("file"))
 
 
+def _kwargs_to_str(**kwargs: Any) -> str:
+    return " ".join([f"{k}={v}" for k, v in kwargs.items()])
+
+
 @contextlib.contextmanager
 def _logging_timer(event: str, **kwargs: Any) -> Generator[float, None, None]:
     logger = config.get().logger
+    context = config.get().context
     logger.info(f"start {event}", **kwargs)
+    if event == "upload" and context is not None:
+        context.upload_log(f"start {event}. {_kwargs_to_str(**kwargs)}")
+
     tic = time.perf_counter()
     yield tic
     toc = time.perf_counter()
+
     kwargs["_".join(event.split() + ["time"])] = toc - tic  # elapsed time
     logger.info(f"end {event}", **kwargs)
+    if event == "upload" and context is not None:
+        context.upload_log(f"end {event}. {_kwargs_to_str(**kwargs)}")
 
 
 class FileInfoModel(pydantic.BaseModel):
     type: str
     href: str
     file_checksum: str = pydantic.Field(..., alias="file:checksum")
     file_size: int = pydantic.Field(..., alias="file:size")
```

### Comparing `cacholote-1.0.0/cacholote/utils.py` & `cacholote-1.1.0/cacholote/utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/cacholote.egg-info/PKG-INFO` & `cacholote-1.1.0/cacholote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 1.0.0
+Version: 1.1.0
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cacholote-1.0.0/cacholote.egg-info/SOURCES.txt` & `cacholote-1.1.0/cacholote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/ci/environment-ci.yml` & `cacholote-1.1.0/ci/environment-ci.yml`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/docs/DESIGN.rst` & `cacholote-1.1.0/docs/DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/docs/Makefile` & `cacholote-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/docs/OBJECT-STORAGE-DESIGN.rst` & `cacholote-1.1.0/docs/OBJECT-STORAGE-DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/docs/conf.py` & `cacholote-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/docs/make.bat` & `cacholote-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/pyproject.toml` & `cacholote-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/tests/conftest.py` & `cacholote-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/tests/test_01_settings.py` & `cacholote-1.1.0/tests/test_01_settings.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/tests/test_02_utils.py` & `cacholote-1.1.0/tests/test_02_utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/tests/test_10_decode.py` & `cacholote-1.1.0/tests/test_10_decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/tests/test_20_encode.py` & `cacholote-1.1.0/tests/test_20_encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/tests/test_30_cache.py` & `cacholote-1.1.0/tests/test_30_cache.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/tests/test_40_xarray_encoder.py` & `cacholote-1.1.0/tests/test_40_xarray_encoder.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/tests/test_50_io_encoder.py` & `cacholote-1.1.0/tests/test_50_io_encoder.py`

 * *Files identical despite different names*

### Comparing `cacholote-1.0.0/tests/test_60_clean.py` & `cacholote-1.1.0/tests/test_60_clean.py`

 * *Files identical despite different names*

