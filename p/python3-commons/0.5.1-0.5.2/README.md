# Comparing `tmp/python3_commons-0.5.1.tar.gz` & `tmp/python3_commons-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3_commons-0.5.1.tar", last modified: Wed May 29 18:42:34 2024, max compression
+gzip compressed data, was "python3_commons-0.5.2.tar", last modified: Wed May 29 19:27:15 2024, max compression
```

## Comparing `python3_commons-0.5.1.tar` & `python3_commons-0.5.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:34.207411 python3_commons-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 18:42:29.000000 python3_commons-0.5.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:34.199411 python3_commons-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:34.203410 python3_commons-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 18:42:29.000000 python3_commons-0.5.1/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-29 18:42:29.000000 python3_commons-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 18:42:29.000000 python3_commons-0.5.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-29 18:42:29.000000 python3_commons-0.5.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-05-29 18:42:29.000000 python3_commons-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 18:42:34.207411 python3_commons-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 18:42:29.000000 python3_commons-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 18:42:29.000000 python3_commons-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:34.203410 python3_commons-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 18:42:29.000000 python3_commons-0.5.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:34.203410 python3_commons-0.5.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 18:42:29.000000 python3_commons-0.5.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 18:42:29.000000 python3_commons-0.5.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 18:42:29.000000 python3_commons-0.5.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-29 18:42:29.000000 python3_commons-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-29 18:42:29.000000 python3_commons-0.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 18:42:29.000000 python3_commons-0.5.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 18:42:29.000000 python3_commons-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 18:42:29.000000 python3_commons-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 18:42:29.000000 python3_commons-0.5.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 18:42:29.000000 python3_commons-0.5.1/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-29 18:42:34.207411 python3_commons-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 18:42:29.000000 python3_commons-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:34.199411 python3_commons-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:34.203410 python3_commons-0.5.1/src/python3_commons/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:34.207411 python3_commons-0.5.1/src/python3_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/object_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:34.207411 python3_commons-0.5.1/src/python3_commons/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/serializers/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 18:42:29.000000 python3_commons-0.5.1/src/python3_commons/serializers/msgspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:34.207411 python3_commons-0.5.1/src/python3_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 18:42:34.000000 python3_commons-0.5.1/src/python3_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 18:42:34.000000 python3_commons-0.5.1/src/python3_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:42:34.000000 python3_commons-0.5.1/src/python3_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:42:34.000000 python3_commons-0.5.1/src/python3_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 18:42:34.000000 python3_commons-0.5.1/src/python3_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 18:42:34.000000 python3_commons-0.5.1/src/python3_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:34.207411 python3_commons-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 18:42:29.000000 python3_commons-0.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-29 18:42:29.000000 python3_commons-0.5.1/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 18:42:29.000000 python3_commons-0.5.1/tests/test_msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.837325 python3_commons-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 19:27:10.000000 python3_commons-0.5.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.829326 python3_commons-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.833325 python3_commons-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 19:27:10.000000 python3_commons-0.5.2/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-29 19:27:10.000000 python3_commons-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 19:27:10.000000 python3_commons-0.5.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-29 19:27:10.000000 python3_commons-0.5.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-05-29 19:27:10.000000 python3_commons-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 19:27:15.837325 python3_commons-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 19:27:10.000000 python3_commons-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 19:27:10.000000 python3_commons-0.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.833325 python3_commons-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.833325 python3_commons-0.5.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 19:27:10.000000 python3_commons-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 19:27:10.000000 python3_commons-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 19:27:10.000000 python3_commons-0.5.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 19:27:10.000000 python3_commons-0.5.2/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-29 19:27:15.841325 python3_commons-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 19:27:10.000000 python3_commons-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.829326 python3_commons-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.837325 python3_commons-0.5.2/src/python3_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.837325 python3_commons-0.5.2/src/python3_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/object_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.837325 python3_commons-0.5.2/src/python3_commons/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/serializers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/serializers/msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.837325 python3_commons-0.5.2/src/python3_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 19:27:15.000000 python3_commons-0.5.2/src/python3_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 19:27:15.000000 python3_commons-0.5.2/src/python3_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:27:15.000000 python3_commons-0.5.2/src/python3_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:27:15.000000 python3_commons-0.5.2/src/python3_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 19:27:15.000000 python3_commons-0.5.2/src/python3_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 19:27:15.000000 python3_commons-0.5.2/src/python3_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.837325 python3_commons-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 19:27:10.000000 python3_commons-0.5.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-29 19:27:10.000000 python3_commons-0.5.2/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 19:27:10.000000 python3_commons-0.5.2/tests/test_msgspec.py
```

### Comparing `python3_commons-0.5.1/.coveragerc` & `python3_commons-0.5.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/.github/workflows/python-publish.yaml` & `python3_commons-0.5.2/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/.gitignore` & `python3_commons-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/LICENSE` & `python3_commons-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/PKG-INFO` & `python3_commons-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.1
+Version: 0.5.2
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.1/docs/Makefile` & `python3_commons-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/docs/conf.py` & `python3_commons-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/docs/index.rst` & `python3_commons-0.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/setup.cfg` & `python3_commons-0.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python3-commons
-version = 0.5.1
+version = 0.5.2
 description = Re-usable Python3 code
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/python3-commons
```

### Comparing `python3_commons-0.5.1/src/python3_commons/audit.py` & `python3_commons-0.5.2/src/python3_commons/audit.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from zoneinfo import ZoneInfo
 
 from lxml import etree
 from zeep.plugins import Plugin
 from zeep.wsdl.definitions import AbstractOperation
 
 from python3_commons import object_storage
-from python3_commons.conf import s3_settings
+from python3_commons.conf import S3Settings, s3_settings
 
 logger = logging.getLogger(__name__)
 
 
 class ZeepAuditPlugin(Plugin):
     def __init__(self, audit_name: str = 'zeep'):
         super().__init__()
```

### Comparing `python3_commons-0.5.1/src/python3_commons/conf.py` & `python3_commons-0.5.2/src/python3_commons/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/src/python3_commons/db.py` & `python3_commons-0.5.2/src/python3_commons/db.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/src/python3_commons/helpers.py` & `python3_commons-0.5.2/src/python3_commons/helpers.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/src/python3_commons/logging/formatter.py` & `python3_commons-0.5.2/src/python3_commons/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/src/python3_commons/object_storage.py` & `python3_commons-0.5.2/src/python3_commons/object_storage.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/src/python3_commons/serializers/json.py` & `python3_commons-0.5.2/src/python3_commons/serializers/json.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/src/python3_commons/serializers/msgpack.py` & `python3_commons-0.5.2/src/python3_commons/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/src/python3_commons/serializers/msgspec.py` & `python3_commons-0.5.2/src/python3_commons/serializers/msgspec.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/src/python3_commons.egg-info/PKG-INFO` & `python3_commons-0.5.2/src/python3_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.1
+Version: 0.5.2
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.1/src/python3_commons.egg-info/SOURCES.txt` & `python3_commons-0.5.2/src/python3_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/tests/conftest.py` & `python3_commons-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/tests/test_msgpack.py` & `python3_commons-0.5.2/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.1/tests/test_msgspec.py` & `python3_commons-0.5.2/tests/test_msgspec.py`

 * *Files identical despite different names*

