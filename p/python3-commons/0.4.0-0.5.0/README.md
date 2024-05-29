# Comparing `tmp/python3_commons-0.4.0.tar.gz` & `tmp/python3_commons-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3_commons-0.4.0.tar", last modified: Wed May 29 14:58:34 2024, max compression
+gzip compressed data, was "python3_commons-0.5.0.tar", last modified: Wed May 29 18:36:19 2024, max compression
```

## Comparing `python3_commons-0.4.0.tar` & `python3_commons-0.5.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:58:34.819944 python3_commons-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 14:58:29.000000 python3_commons-0.4.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:58:34.811944 python3_commons-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:58:34.815944 python3_commons-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-29 14:58:29.000000 python3_commons-0.4.0/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-29 14:58:29.000000 python3_commons-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 14:58:29.000000 python3_commons-0.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-29 14:58:29.000000 python3_commons-0.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-05-29 14:58:29.000000 python3_commons-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-29 14:58:34.819944 python3_commons-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 14:58:29.000000 python3_commons-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 14:58:29.000000 python3_commons-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:58:34.815944 python3_commons-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 14:58:29.000000 python3_commons-0.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:58:34.815944 python3_commons-0.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 14:58:29.000000 python3_commons-0.4.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 14:58:29.000000 python3_commons-0.4.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 14:58:29.000000 python3_commons-0.4.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-29 14:58:29.000000 python3_commons-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-29 14:58:29.000000 python3_commons-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 14:58:29.000000 python3_commons-0.4.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 14:58:29.000000 python3_commons-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 14:58:29.000000 python3_commons-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 14:58:29.000000 python3_commons-0.4.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 14:58:29.000000 python3_commons-0.4.0/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-29 14:58:34.819944 python3_commons-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 14:58:29.000000 python3_commons-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:58:34.811944 python3_commons-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:58:34.815944 python3_commons-0.4.0/src/python3_commons/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:58:34.819944 python3_commons-0.4.0/src/python3_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/object_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:58:34.819944 python3_commons-0.4.0/src/python3_commons/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/serializers/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 14:58:29.000000 python3_commons-0.4.0/src/python3_commons/serializers/msgspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:58:34.819944 python3_commons-0.4.0/src/python3_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-29 14:58:34.000000 python3_commons-0.4.0/src/python3_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 14:58:34.000000 python3_commons-0.4.0/src/python3_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:58:34.000000 python3_commons-0.4.0/src/python3_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:58:34.000000 python3_commons-0.4.0/src/python3_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-29 14:58:34.000000 python3_commons-0.4.0/src/python3_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 14:58:34.000000 python3_commons-0.4.0/src/python3_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:58:34.819944 python3_commons-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 14:58:29.000000 python3_commons-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-29 14:58:29.000000 python3_commons-0.4.0/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 14:58:29.000000 python3_commons-0.4.0/tests/test_msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:19.405109 python3_commons-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 18:36:10.000000 python3_commons-0.5.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:19.393109 python3_commons-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:19.397109 python3_commons-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-29 18:36:10.000000 python3_commons-0.5.0/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-29 18:36:10.000000 python3_commons-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 18:36:10.000000 python3_commons-0.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-29 18:36:10.000000 python3_commons-0.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-05-29 18:36:10.000000 python3_commons-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 18:36:19.405109 python3_commons-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 18:36:10.000000 python3_commons-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 18:36:10.000000 python3_commons-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:19.397109 python3_commons-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 18:36:10.000000 python3_commons-0.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:19.397109 python3_commons-0.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 18:36:10.000000 python3_commons-0.5.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 18:36:10.000000 python3_commons-0.5.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 18:36:10.000000 python3_commons-0.5.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-29 18:36:10.000000 python3_commons-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-29 18:36:10.000000 python3_commons-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 18:36:10.000000 python3_commons-0.5.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 18:36:10.000000 python3_commons-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 18:36:10.000000 python3_commons-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 18:36:10.000000 python3_commons-0.5.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 18:36:10.000000 python3_commons-0.5.0/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-29 18:36:19.405109 python3_commons-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 18:36:10.000000 python3_commons-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:19.393109 python3_commons-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:19.401109 python3_commons-0.5.0/src/python3_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:19.401109 python3_commons-0.5.0/src/python3_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/object_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:19.401109 python3_commons-0.5.0/src/python3_commons/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/serializers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 18:36:10.000000 python3_commons-0.5.0/src/python3_commons/serializers/msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:19.401109 python3_commons-0.5.0/src/python3_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 18:36:19.000000 python3_commons-0.5.0/src/python3_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 18:36:19.000000 python3_commons-0.5.0/src/python3_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:36:19.000000 python3_commons-0.5.0/src/python3_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:36:19.000000 python3_commons-0.5.0/src/python3_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 18:36:19.000000 python3_commons-0.5.0/src/python3_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 18:36:19.000000 python3_commons-0.5.0/src/python3_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:19.401109 python3_commons-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 18:36:10.000000 python3_commons-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-29 18:36:10.000000 python3_commons-0.5.0/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 18:36:10.000000 python3_commons-0.5.0/tests/test_msgspec.py
```

### Comparing `python3_commons-0.4.0/.coveragerc` & `python3_commons-0.5.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/.github/workflows/python-publish.yaml` & `python3_commons-0.5.0/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/.gitignore` & `python3_commons-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/LICENSE` & `python3_commons-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/PKG-INFO` & `python3_commons-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.4.0
+Version: 0.5.0
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.12
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: asyncpg==0.29.0
+Requires-Dist: lxml==5.2.2
 Requires-Dist: minio==7.2.7
 Requires-Dist: msgpack==1.0.8
 Requires-Dist: msgspec==0.18.6
 Requires-Dist: pydantic[email]==2.7.2
 Requires-Dist: pydantic-settings==2.2.1
+Requires-Dist: zeep==4.2.1
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 Re-usable Python3 code
 ======================
```

### Comparing `python3_commons-0.4.0/docs/Makefile` & `python3_commons-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/docs/conf.py` & `python3_commons-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/docs/index.rst` & `python3_commons-0.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/setup.cfg` & `python3_commons-0.5.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python3-commons
-version = 0.4.0
+version = 0.5.0
 description = Re-usable Python3 code
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/python3-commons
@@ -20,19 +20,21 @@
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
 	asyncpg==0.29.0
+	lxml==5.2.2
 	minio==7.2.7
 	msgpack==1.0.8
 	msgspec==0.18.6
 	pydantic[email]==2.7.2
 	pydantic-settings==2.2.1
+	zeep==4.2.1
 python_requires = >=3.12
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `python3_commons-0.4.0/src/python3_commons/conf.py` & `python3_commons-0.5.0/src/python3_commons/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/src/python3_commons/db.py` & `python3_commons-0.5.0/src/python3_commons/db.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/src/python3_commons/helpers.py` & `python3_commons-0.5.0/src/python3_commons/helpers.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/src/python3_commons/logging/formatter.py` & `python3_commons-0.5.0/src/python3_commons/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/src/python3_commons/object_storage.py` & `python3_commons-0.5.0/src/python3_commons/object_storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -121,21 +121,7 @@
         delete_object_list = map(DeleteObject, object_names)
     else:
         return None
 
     errors = s3_client.remove_objects(bucket_name, delete_object_list)
 
     return errors
-
-
-async def store_bytes_in_s3(settings: S3Settings, data: bytes, key: str):
-    if settings.s3_secret_access_key:
-        try:
-            client = get_s3_client(settings)
-
-            client.put_object(settings.s3_bucket, key, io.BytesIO(data), len(data))
-        except S3Error as e:
-            logger.error(f'Failed storing object in storage: {e}')
-        else:
-            logger.debug(f'Stored object in storage: {key}')
-    else:
-        logger.debug(f'S3 is not configured, not storing object in storage: {key}')
```

### Comparing `python3_commons-0.4.0/src/python3_commons/serializers/json.py` & `python3_commons-0.5.0/src/python3_commons/serializers/json.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/src/python3_commons/serializers/msgpack.py` & `python3_commons-0.5.0/src/python3_commons/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/src/python3_commons/serializers/msgspec.py` & `python3_commons-0.5.0/src/python3_commons/serializers/msgspec.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/src/python3_commons.egg-info/PKG-INFO` & `python3_commons-0.5.0/src/python3_commons.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.4.0
+Version: 0.5.0
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.12
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: asyncpg==0.29.0
+Requires-Dist: lxml==5.2.2
 Requires-Dist: minio==7.2.7
 Requires-Dist: msgpack==1.0.8
 Requires-Dist: msgspec==0.18.6
 Requires-Dist: pydantic[email]==2.7.2
 Requires-Dist: pydantic-settings==2.2.1
+Requires-Dist: zeep==4.2.1
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 Re-usable Python3 code
 ======================
```

### Comparing `python3_commons-0.4.0/src/python3_commons.egg-info/SOURCES.txt` & `python3_commons-0.5.0/src/python3_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/tests/conftest.py` & `python3_commons-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/tests/test_msgpack.py` & `python3_commons-0.5.0/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.4.0/tests/test_msgspec.py` & `python3_commons-0.5.0/tests/test_msgspec.py`

 * *Files identical despite different names*

