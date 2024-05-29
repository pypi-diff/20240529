# Comparing `tmp/invenio-imoox-0.2.0.tar.gz` & `tmp/invenio-imoox-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-imoox-0.2.0.tar", last modified: Fri Oct 14 06:41:46 2022, max compression
+gzip compressed data, was "invenio-imoox-0.3.0.tar", last modified: Wed May 29 09:25:40 2024, max compression
```

## Comparing `invenio-imoox-0.2.0.tar` & `invenio-imoox-0.3.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:41:46.908046 invenio-imoox-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3512 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-10-14 06:41:46.908046 invenio-imoox-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:41:46.908046 invenio-imoox-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10090 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6995 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:41:46.908046 invenio-imoox-0.2.0/invenio_imoox/
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/invenio_imoox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2221 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/invenio_imoox/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/invenio_imoox/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    10222 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/invenio_imoox/converter.py
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/invenio_imoox/ext.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/invenio_imoox/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/invenio_imoox/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:41:46.908046 invenio-imoox-0.2.0/invenio_imoox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-10-14 06:41:46.000000 invenio-imoox-0.2.0/invenio_imoox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-10-14 06:41:46.000000 invenio-imoox-0.2.0/invenio_imoox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 06:41:46.000000 invenio-imoox-0.2.0/invenio_imoox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-14 06:41:46.000000 invenio-imoox-0.2.0/invenio_imoox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 06:41:46.000000 invenio-imoox-0.2.0/invenio_imoox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-10-14 06:41:46.000000 invenio-imoox-0.2.0/invenio_imoox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-14 06:41:46.000000 invenio-imoox-0.2.0/invenio_imoox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)      783 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-10-14 06:41:46.908046 invenio-imoox-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:41:46.908046 invenio-imoox-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-10-14 06:41:39.000000 invenio-imoox-0.2.0/tests/test_invenio_imoox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:25:40.503506 invenio-imoox-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-29 09:25:40.503506 invenio-imoox-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:25:40.503506 invenio-imoox-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:25:40.503506 invenio-imoox-0.3.0/invenio_imoox/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/invenio_imoox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/invenio_imoox/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/invenio_imoox/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/invenio_imoox/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/invenio_imoox/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/invenio_imoox/records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/invenio_imoox/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/invenio_imoox/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:25:40.503506 invenio-imoox-0.3.0/invenio_imoox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-29 09:25:40.000000 invenio-imoox-0.3.0/invenio_imoox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-29 09:25:40.000000 invenio-imoox-0.3.0/invenio_imoox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:25:40.000000 invenio-imoox-0.3.0/invenio_imoox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-29 09:25:40.000000 invenio-imoox-0.3.0/invenio_imoox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:25:40.000000 invenio-imoox-0.3.0/invenio_imoox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-29 09:25:40.000000 invenio-imoox-0.3.0/invenio_imoox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 09:25:40.000000 invenio-imoox-0.3.0/invenio_imoox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1102 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-29 09:25:40.507506 invenio-imoox-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:25:40.503506 invenio-imoox-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-29 09:25:36.000000 invenio-imoox-0.3.0/tests/test_invenio_imoox.py
```

### Comparing `invenio-imoox-0.2.0/.editorconfig` & `invenio-imoox-0.3.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-imoox-0.2.0/CONTRIBUTING.rst` & `invenio-imoox-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-imoox-0.2.0/LICENSE` & `invenio-imoox-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-imoox-0.2.0/PKG-INFO` & `invenio-imoox-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-imoox
-Version: 0.2.0
+Version: 0.3.0
 Summary: "Provides API for iMooX."
 Home-page: https://github.com/tu-graz-library/invenio-imoox
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2021 Graz University of Technology.
@@ -40,26 +40,36 @@
             invenio-imoox is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version v0.3.0 (release 2024-05-29)
+        
+        - cli: improve success output
+        - fix: for global search
+        - cli: give clean message for not existing user
+        - cli: improve shown error by color
+        - setup: use ruff
+        - cli: add dry_run option
+        - refactor: implement service approach
+        
+        
         Version v0.2.0 (release 2022-10-14)
         
         - setup: remove packages coming from pytest-invenio
         - change: improve function
         - pylint: changes
         - global: pin flake8
         - fix: install invenio_search[opensearch2] for tests
         - fix: sphinx language should not set to None
         - global: migrate to reusable workflows
         - global: remove explicit install of db and search
         
         
 Platform: any
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Provides-Extra: tests
```

### Comparing `invenio-imoox-0.2.0/README.rst` & `invenio-imoox-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-imoox-0.2.0/docs/conf.py` & `invenio-imoox-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-imoox-0.2.0/docs/index.rst` & `invenio-imoox-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-imoox-0.2.0/docs/make.bat` & `invenio-imoox-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-imoox-0.2.0/invenio_imoox/ext.py` & `invenio-imoox-0.3.0/tests/test_invenio_imoox.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 Graz University of Technology.
+# Copyright (C) 2021-2024 Graz University of Technology.
 #
 # invenio-imoox is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
-"""Provides API for iMooX."""
+"""Module tests."""
 
-from . import config
+from flask import Flask
 
+from invenio_imoox import InvenioIMooX, __version__
 
-class InvenioIMooX:
-    """invenio-imoox extension."""
 
-    def __init__(self, app=None):
-        """Extension initialization."""
-        if app:
-            self.init_app(app)
+def test_version() -> None:
+    """Test version import."""
+    assert __version__
 
-    def init_app(self, app):
-        """Flask application initialization."""
-        self.init_config(app)
-        app.extensions["invenio-imoox"] = self
 
-    def init_config(self, app):
-        """Initialize configuration."""
-        for k in dir(config):
-            if k.startswith("INVENIO_IMOOX_"):
-                app.config.setdefault(k, getattr(config, k))
+def test_init() -> None:
+    """Test extension initialization."""
+    app = Flask("testapp")
+    ext = InvenioIMooX(app)
+    assert "invenio-imoox" in app.extensions
+
+    app = Flask("testapp")
+    ext = InvenioIMooX()
+    assert "invenio-imoox" not in app.extensions
+
+    ext.init_app(app)
+    assert "invenio-imoox" in app.extensions
```

### Comparing `invenio-imoox-0.2.0/invenio_imoox.egg-info/PKG-INFO` & `invenio-imoox-0.3.0/invenio_imoox.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-imoox
-Version: 0.2.0
+Version: 0.3.0
 Summary: "Provides API for iMooX."
 Home-page: https://github.com/tu-graz-library/invenio-imoox
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2021 Graz University of Technology.
@@ -40,26 +40,36 @@
             invenio-imoox is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version v0.3.0 (release 2024-05-29)
+        
+        - cli: improve success output
+        - fix: for global search
+        - cli: give clean message for not existing user
+        - cli: improve shown error by color
+        - setup: use ruff
+        - cli: add dry_run option
+        - refactor: implement service approach
+        
+        
         Version v0.2.0 (release 2022-10-14)
         
         - setup: remove packages coming from pytest-invenio
         - change: improve function
         - pylint: changes
         - global: pin flake8
         - fix: install invenio_search[opensearch2] for tests
         - fix: sphinx language should not set to None
         - global: migrate to reusable workflows
         - global: remove explicit install of db and search
         
         
 Platform: any
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Provides-Extra: tests
```

### Comparing `invenio-imoox-0.2.0/invenio_imoox.egg-info/SOURCES.txt` & `invenio-imoox-0.3.0/invenio_imoox.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -22,18 +22,19 @@
 docs/license.rst
 docs/make.bat
 docs/requirements.txt
 docs/usage.rst
 invenio_imoox/__init__.py
 invenio_imoox/cli.py
 invenio_imoox/config.py
-invenio_imoox/converter.py
 invenio_imoox/ext.py
+invenio_imoox/proxies.py
+invenio_imoox/records.py
+invenio_imoox/services.py
 invenio_imoox/tasks.py
-invenio_imoox/utils.py
 invenio_imoox.egg-info/PKG-INFO
 invenio_imoox.egg-info/SOURCES.txt
 invenio_imoox.egg-info/dependency_links.txt
 invenio_imoox.egg-info/entry_points.txt
 invenio_imoox.egg-info/not-zip-safe
 invenio_imoox.egg-info/requires.txt
 invenio_imoox.egg-info/top_level.txt
```

### Comparing `invenio-imoox-0.2.0/tests/conftest.py` & `invenio-imoox-0.3.0/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 Graz University of Technology.
+# Copyright (C) 2021-2024 Graz University of Technology.
 #
 # invenio-imoox is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Pytest configuration.
 
 See https://pytest-invenio.readthedocs.io/ for documentation on which test
 fixtures are available.
 """
 
+from collections.abc import Callable
+
 import pytest
 from flask import Flask
 
 from invenio_imoox import InvenioIMooX
 
 
 @pytest.fixture(scope="module")
-def celery_config():
-    """Override pytest-invenio fixture.
-
-    TODO: Remove this fixture if you add Celery support.
-    """
-    return {}
-
-
-@pytest.fixture(scope="module")
-def create_app(instance_path):
+def create_app(instance_path: str) -> Callable:
     """Application factory fixture."""
 
-    def factory(**config):
+    def factory(**config: dict) -> Flask:
         app = Flask("testapp", instance_path=instance_path)
         app.config.update(**config)
         InvenioIMooX(app)
         return app
 
     return factory
```

