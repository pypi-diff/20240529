# Comparing `tmp/dj-dynamic-settings-0.2.6.tar.gz` & `tmp/dj-dynamic-settings-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-dynamic-settings-0.2.6.tar", last modified: Sun May 12 22:34:09 2024, max compression
+gzip compressed data, was "dj-dynamic-settings-0.2.7.tar", last modified: Tue May 28 13:56:10 2024, max compression
```

## Comparing `dj-dynamic-settings-0.2.6.tar` & `dj-dynamic-settings-0.2.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:34:09.012124 dj-dynamic-settings-0.2.6/
--rw-rw-rw-   0 root         (0) root         (0)     1304 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/.isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1050 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     4765 2024-05-12 22:34:09.012124 dj-dynamic-settings-0.2.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3305 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:34:09.008124 dj-dynamic-settings-0.2.6/dj_dynamic_settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/compat.py
--rw-rw-rw-   0 root         (0) root         (0)     3093 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/metadata.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:34:09.012124 dj-dynamic-settings-0.2.6/dj_dynamic_settings/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      970 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1215 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/registry.py
--rw-rw-rw-   0 root         (0) root         (0)     2515 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/serializers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:34:09.012124 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     4250 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_dynamic_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2377 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_override_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     4014 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3550 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/views.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:34:09.012124 dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4765 2024-05-12 22:34:08.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1176 2024-05-12 22:34:08.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-12 22:34:08.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-12 22:34:08.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-12 22:34:08.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/runtests.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-12 22:34:09.012124 dj-dynamic-settings-0.2.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2257 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:56:10.925315 dj-dynamic-settings-0.2.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/.isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4815 2024-05-28 13:56:10.925315 dj-dynamic-settings-0.2.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3305 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2942 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:56:10.925315 dj-dynamic-settings-0.2.7/dj_dynamic_settings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/compat.py
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/metadata.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:56:10.925315 dj-dynamic-settings-0.2.7/dj_dynamic_settings/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      970 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/serializers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:56:10.925315 dj-dynamic-settings-0.2.7/dj_dynamic_settings/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/tests/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4250 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/tests/test_dynamic_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/tests/test_override_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/tests/test_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     4014 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/tests/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3550 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings/views.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:56:10.925315 dj-dynamic-settings-0.2.7/dj_dynamic_settings.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4815 2024-05-28 13:56:10.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2024-05-28 13:56:10.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-28 13:56:10.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-28 13:56:10.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-28 13:56:10.000000 dj-dynamic-settings-0.2.7/dj_dynamic_settings.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/runtests.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-28 13:56:10.925315 dj-dynamic-settings-0.2.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1438 2024-05-28 13:55:42.000000 dj-dynamic-settings-0.2.7/tox.ini
```

### Comparing `dj-dynamic-settings-0.2.6/.gitignore` & `dj-dynamic-settings-0.2.7/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -106,7 +106,9 @@
 media
 static_core/package-lock.json
 
 .pytest_cache/*
 
 # Prevent committing editable requirements in src directory
 src/
+
+dist/
```

### Comparing `dj-dynamic-settings-0.2.6/LICENSE.txt` & `dj-dynamic-settings-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/PKG-INFO` & `dj-dynamic-settings-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-dynamic-settings
-Version: 0.2.6
+Version: 0.2.7
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-dynamic-settings/
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
```

### Comparing `dj-dynamic-settings-0.2.6/README.md` & `dj-dynamic-settings-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/bitbucket-pipelines.yml` & `dj-dynamic-settings-0.2.7/bitbucket-pipelines.yml`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,23 @@
           image: python:3.8-alpine
           script:
             - apk add postgresql-dev gcc git python3-dev musl-dev
             - pip install tox
             - tox -e py38-django22,py38-django30,py38-django32,py38-django40,py38-django41,py38-django42
           services:
             - postgres
+      - step:
+          name: py39
+          image: python:3.9-alpine
+          script:
+            - apk add postgresql-dev gcc git python3-dev musl-dev
+            - pip install tox
+            - tox -e py389-django32,py39-django40,py39-django41,py39-django42
+          services:
+            - postgres
   tags:
     '*':
       - step:
           name: Publish to PyPI
           image: python:3.8-alpine
           script:
             - apk add gcc git libffi-dev musl-dev openssl-dev python3-dev
```

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/app_settings.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/app_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/compat.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/compat.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/conf.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/conf.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/metadata.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/metadata.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/migrations/0001_initial.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/models.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/models.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/registry.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/registry.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/serializers.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/serializers.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/definitions.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/tests/definitions.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_dynamic_settings.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/tests/test_dynamic_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_override_settings.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/tests/test_override_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_settings.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_views.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/utils.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/utils.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/validators.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/validators.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings/views.py` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings/views.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/PKG-INFO` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-dynamic-settings
-Version: 0.2.6
+Version: 0.2.7
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-dynamic-settings/
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
```

### Comparing `dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/SOURCES.txt` & `dj-dynamic-settings-0.2.7/dj_dynamic_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.6/setup.py` & `dj-dynamic-settings-0.2.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Framework :: Django",
         "Framework :: Django :: 1.10",
         "Framework :: Django :: 1.11",
         "Framework :: Django :: 2.0",
         "Framework :: Django :: 2.1",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
```

### Comparing `dj-dynamic-settings-0.2.6/tox.ini` & `dj-dynamic-settings-0.2.7/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 isolated_build = True
 skip_missing_interpreters = True
 envlist = py27-{django110,django111}
           py34-{django110,django111,django20}
           py35-{django110,django111,django20,django21,django22}
           {py36,py37}-{django111,django20,django21,django22,django30,django31,django32}
           py38-{django22,django30,django31,django32, django40, django41, django42}
+          py39-{django32,django40,django41,django42}
           linting
 
 [testenv]
 deps = django110: Django>=1.10,<1.11
        django111: Django>=1.11.7,<2.0
        django20: Django>=2.0,<2.1
        django21: Django>=2.1,<2.2
```

