# Comparing `tmp/python3_commons-0.5.2.tar.gz` & `tmp/python3_commons-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3_commons-0.5.2.tar", last modified: Wed May 29 19:27:15 2024, max compression
+gzip compressed data, was "python3_commons-0.5.3.tar", last modified: Wed May 29 20:49:10 2024, max compression
```

## Comparing `python3_commons-0.5.2.tar` & `python3_commons-0.5.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.837325 python3_commons-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 19:27:10.000000 python3_commons-0.5.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.829326 python3_commons-0.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.833325 python3_commons-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 19:27:10.000000 python3_commons-0.5.2/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-29 19:27:10.000000 python3_commons-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 19:27:10.000000 python3_commons-0.5.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-29 19:27:10.000000 python3_commons-0.5.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-05-29 19:27:10.000000 python3_commons-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 19:27:15.837325 python3_commons-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 19:27:10.000000 python3_commons-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 19:27:10.000000 python3_commons-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.833325 python3_commons-0.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.833325 python3_commons-0.5.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 19:27:10.000000 python3_commons-0.5.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 19:27:10.000000 python3_commons-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 19:27:10.000000 python3_commons-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 19:27:10.000000 python3_commons-0.5.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 19:27:10.000000 python3_commons-0.5.2/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-29 19:27:15.841325 python3_commons-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 19:27:10.000000 python3_commons-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.829326 python3_commons-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.837325 python3_commons-0.5.2/src/python3_commons/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.837325 python3_commons-0.5.2/src/python3_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/object_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.837325 python3_commons-0.5.2/src/python3_commons/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/serializers/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 19:27:10.000000 python3_commons-0.5.2/src/python3_commons/serializers/msgspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.837325 python3_commons-0.5.2/src/python3_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 19:27:15.000000 python3_commons-0.5.2/src/python3_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 19:27:15.000000 python3_commons-0.5.2/src/python3_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:27:15.000000 python3_commons-0.5.2/src/python3_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:27:15.000000 python3_commons-0.5.2/src/python3_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 19:27:15.000000 python3_commons-0.5.2/src/python3_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 19:27:15.000000 python3_commons-0.5.2/src/python3_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:27:15.837325 python3_commons-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 19:27:10.000000 python3_commons-0.5.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-29 19:27:10.000000 python3_commons-0.5.2/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 19:27:10.000000 python3_commons-0.5.2/tests/test_msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.262893 python3_commons-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 20:49:02.000000 python3_commons-0.5.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.254893 python3_commons-0.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.254893 python3_commons-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 20:49:02.000000 python3_commons-0.5.3/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-29 20:49:02.000000 python3_commons-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 20:49:02.000000 python3_commons-0.5.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-29 20:49:02.000000 python3_commons-0.5.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-05-29 20:49:02.000000 python3_commons-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 20:49:10.262893 python3_commons-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 20:49:02.000000 python3_commons-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 20:49:02.000000 python3_commons-0.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.258893 python3_commons-0.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.258893 python3_commons-0.5.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 20:49:02.000000 python3_commons-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 20:49:02.000000 python3_commons-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 20:49:02.000000 python3_commons-0.5.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 20:49:02.000000 python3_commons-0.5.3/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-29 20:49:10.262893 python3_commons-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 20:49:02.000000 python3_commons-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.254893 python3_commons-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.258893 python3_commons-0.5.3/src/python3_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.258893 python3_commons-0.5.3/src/python3_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/object_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.262893 python3_commons-0.5.3/src/python3_commons/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/serializers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/serializers/msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.262893 python3_commons-0.5.3/src/python3_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 20:49:10.000000 python3_commons-0.5.3/src/python3_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 20:49:10.000000 python3_commons-0.5.3/src/python3_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:49:10.000000 python3_commons-0.5.3/src/python3_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:49:10.000000 python3_commons-0.5.3/src/python3_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 20:49:10.000000 python3_commons-0.5.3/src/python3_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 20:49:10.000000 python3_commons-0.5.3/src/python3_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.262893 python3_commons-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 20:49:02.000000 python3_commons-0.5.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-29 20:49:02.000000 python3_commons-0.5.3/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 20:49:02.000000 python3_commons-0.5.3/tests/test_msgspec.py
```

### Comparing `python3_commons-0.5.2/.coveragerc` & `python3_commons-0.5.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/.github/workflows/python-publish.yaml` & `python3_commons-0.5.3/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/.gitignore` & `python3_commons-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/LICENSE` & `python3_commons-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/PKG-INFO` & `python3_commons-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.2
+Version: 0.5.3
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.2/docs/Makefile` & `python3_commons-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/docs/conf.py` & `python3_commons-0.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/docs/index.rst` & `python3_commons-0.5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/setup.cfg` & `python3_commons-0.5.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python3-commons
-version = 0.5.2
+version = 0.5.3
 description = Re-usable Python3 code
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/python3-commons
```

### Comparing `python3_commons-0.5.2/src/python3_commons/audit.py` & `python3_commons-0.5.3/src/python3_commons/audit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,33 @@
 import asyncio
+import io
 import logging
 import tarfile
-from datetime import date, datetime, timedelta, UTC
+from datetime import datetime, timedelta, UTC
 from io import BytesIO
 from uuid import uuid4
-from zoneinfo import ZoneInfo
 
 from lxml import etree
+from minio import S3Error
 from zeep.plugins import Plugin
 from zeep.wsdl.definitions import AbstractOperation
 
 from python3_commons import object_storage
 from python3_commons.conf import S3Settings, s3_settings
+from python3_commons.object_storage import get_s3_client
 
 logger = logging.getLogger(__name__)
 
 
-class ZeepAuditPlugin(Plugin):
-    def __init__(self, audit_name: str = 'zeep'):
-        super().__init__()
-        self.audit_name = audit_name
-
-    @staticmethod
-    def store_audit_in_s3(envelope, operation: AbstractOperation, direction: str):
-        xml = etree.tostring(envelope, encoding='UTF-8', pretty_print=True)
-        now = datetime.now(tz=UTC)
-        date_path = now.strftime('%Y/%m/%d')
-        timestamp = now.strftime('%H%M%S')
-        coro = object_storage.store_bytes_in_s3(
-            settings, xml,
-            f'audit/{date_path}/{self.audit_name}/{operation.name}/{timestamp}_{str(uuid4())[-12:]}_{direction}.xml'
-        )
-
-        try:
-            loop = asyncio.get_running_loop()
-        except RuntimeError:
-            loop = None
-
-        if loop and loop.is_running():
-            loop.create_task(coro)
-        else:
-            asyncio.run(coro)
-
-    def ingress(self, envelope, http_headers, operation: AbstractOperation):
-        self.store_audit_in_s3(envelope, operation, 'ingress')
-
-        return envelope, http_headers
-
-    def egress(self, envelope, http_headers, operation: AbstractOperation, binding_options):
-        self.store_audit_in_s3(envelope, operation, 'egress')
-
-        return envelope, http_headers
-
-
 async def write_audit_data(settings: S3Settings, key: str, data: bytes):
     if settings.s3_secret_access_key:
         try:
             client = get_s3_client(settings)
 
-            client.put_object(settings.s3_bucket, key, io.BytesIO(data), len(data))
+            client.put_object(settings.s3_bucket, f'audit/{key}', io.BytesIO(data), len(data))
         except S3Error as e:
             logger.error(f'Failed storing object in storage: {e}')
         else:
             logger.debug(f'Stored object in storage: {key}')
     else:
         logger.debug(f'S3 is not configured, not storing object in storage: {key}')
 
@@ -88,15 +53,51 @@
                 archive.addfile(info, BytesIO(content))
                 object_names.append(name)
 
     fo.seek(0)
 
     if object_names:
         archive_path = object_storage.get_absolute_path(
-            f'.archive/{year}_{month:02}/{year}_{month:02}_{day:02}.tar.bz2')
+            f'.archive/{year}_{month:02}_{day:02}.tar.bz2')
         object_storage.put_object(bucket_name, archive_path, fo, fo.getbuffer().nbytes)
 
         if errors := object_storage.remove_objects(bucket_name, object_names=object_names):
             for error in errors:
                 logger.error(f'Failed to delete object in {bucket_name=}: {error}')
     else:
         logger.info('No objects to archive found.')
+
+
+class ZeepAuditPlugin(Plugin):
+    def __init__(self, audit_name: str = 'zeep'):
+        super().__init__()
+        self.audit_name = audit_name
+
+    def store_audit_in_s3(self, envelope, operation: AbstractOperation, direction: str):
+        xml = etree.tostring(envelope, encoding='UTF-8', pretty_print=True)
+        now = datetime.now(tz=UTC)
+        date_path = now.strftime('%Y/%m/%d')
+        timestamp = now.strftime('%H%M%S')
+        coro = write_audit_data(
+            s3_settings,
+            f'{date_path}/{self.audit_name}/{operation.name}/{timestamp}_{str(uuid4())[-12:]}_{direction}.xml', xml
+        )
+
+        try:
+            loop = asyncio.get_running_loop()
+        except RuntimeError:
+            loop = None
+
+        if loop and loop.is_running():
+            loop.create_task(coro)
+        else:
+            asyncio.run(coro)
+
+    def ingress(self, envelope, http_headers, operation: AbstractOperation):
+        self.store_audit_in_s3(envelope, operation, 'ingress')
+
+        return envelope, http_headers
+
+    def egress(self, envelope, http_headers, operation: AbstractOperation, binding_options):
+        self.store_audit_in_s3(envelope, operation, 'egress')
+
+        return envelope, http_headers
```

### Comparing `python3_commons-0.5.2/src/python3_commons/conf.py` & `python3_commons-0.5.3/src/python3_commons/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/src/python3_commons/db.py` & `python3_commons-0.5.3/src/python3_commons/db.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/src/python3_commons/helpers.py` & `python3_commons-0.5.3/src/python3_commons/helpers.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/src/python3_commons/logging/formatter.py` & `python3_commons-0.5.3/src/python3_commons/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/src/python3_commons/object_storage.py` & `python3_commons-0.5.3/src/python3_commons/object_storage.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/src/python3_commons/serializers/json.py` & `python3_commons-0.5.3/src/python3_commons/serializers/json.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/src/python3_commons/serializers/msgpack.py` & `python3_commons-0.5.3/src/python3_commons/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/src/python3_commons/serializers/msgspec.py` & `python3_commons-0.5.3/src/python3_commons/serializers/msgspec.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/src/python3_commons.egg-info/PKG-INFO` & `python3_commons-0.5.3/src/python3_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.2
+Version: 0.5.3
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.2/src/python3_commons.egg-info/SOURCES.txt` & `python3_commons-0.5.3/src/python3_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/tests/conftest.py` & `python3_commons-0.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/tests/test_msgpack.py` & `python3_commons-0.5.3/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.2/tests/test_msgspec.py` & `python3_commons-0.5.3/tests/test_msgspec.py`

 * *Files identical despite different names*

