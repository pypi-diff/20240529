# Comparing `tmp/tscat_gui-0.3.1.tar.gz` & `tmp/tscat_gui-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tscat_gui-0.3.1.tar", last modified: Fri May 24 15:16:50 2024, max compression
+gzip compressed data, was "tscat_gui-0.3.2.tar", last modified: Wed May 29 16:45:43 2024, max compression
```

## Comparing `tscat_gui-0.3.1.tar` & `tscat_gui-0.3.2.tar`

### file list

```diff
@@ -1,57 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.252851 tscat_gui-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-24 15:16:50.252851 tscat_gui-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.248851 tscat_gui-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4891 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-24 15:16:50.256851 tscat_gui-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.248851 tscat_gui-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tests/test_mypy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.252851 tscat_gui-0.3.1/tscat_gui/
--rw-r--r--   0 runner    (1001) docker     (127)    23012 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    21591 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.252851 tscat_gui-0.3.1/tscat_gui/tscat_driver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/catalog_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/tscat_root_model.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    12569 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/undo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.252851 tscat_gui-0.3.1/tscat_gui/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/utils/editable_label.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/utils/flow_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/utils/keyword_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.252851 tscat_gui-0.3.1/tscat_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:45:43.163596 tscat_gui-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-29 16:45:43.163596 tscat_gui-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:45:43.155596 tscat_gui-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4891 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-29 16:45:43.163596 tscat_gui-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:45:43.155596 tscat_gui-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tests/test_mypy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:45:43.159596 tscat_gui-0.3.2/tscat_gui/
+-rw-r--r--   0 runner    (1001) docker     (127)    23045 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:45:43.159596 tscat_gui-0.3.2/tscat_gui/model_base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/model_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/model_base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21591 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:45:43.159596 tscat_gui-0.3.2/tscat_gui/tscat_driver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/tscat_driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/tscat_driver/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/tscat_driver/catalog_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/tscat_driver/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/tscat_driver/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/tscat_driver/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12673 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/tscat_driver/tscat_root_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/tscat_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12569 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/undo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:45:43.163596 tscat_gui-0.3.2/tscat_gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/utils/editable_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/utils/flow_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-29 16:45:36.000000 tscat_gui-0.3.2/tscat_gui/utils/keyword_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:45:43.159596 tscat_gui-0.3.2/tscat_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-29 16:45:43.000000 tscat_gui-0.3.2/tscat_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-29 16:45:43.000000 tscat_gui-0.3.2/tscat_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:45:43.000000 tscat_gui-0.3.2/tscat_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 16:45:43.000000 tscat_gui-0.3.2/tscat_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:45:43.000000 tscat_gui-0.3.2/tscat_gui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 16:45:43.000000 tscat_gui-0.3.2/tscat_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 16:45:43.000000 tscat_gui-0.3.2/tscat_gui.egg-info/top_level.txt
```

### Comparing `tscat_gui-0.3.1/CONTRIBUTING.rst` & `tscat_gui-0.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/LICENSE` & `tscat_gui-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/PKG-INFO` & `tscat_gui-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tscat_gui
-Version: 0.3.1
+Version: 0.3.2
 Summary: Time-series catalogue - graphical user interface library
 Home-page: https://github.com/SciQLop/tscat_gui
 Author: Patrick Boettcher
 Author-email: p@yai.se
 License: GNU General Public License v3
 Keywords: tscat_gui
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `tscat_gui-0.3.1/README.rst` & `tscat_gui-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/docs/Makefile` & `tscat_gui-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/docs/conf.py` & `tscat_gui-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/docs/installation.rst` & `tscat_gui-0.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/docs/make.bat` & `tscat_gui-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/setup.py` & `tscat_gui-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords='tscat_gui',
     name='tscat_gui',
     packages=find_packages(include=['tscat_gui', 'tscat_gui.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/SciQLop/tscat_gui',
-    version='0.3.1',
+    version='0.3.2',
     zip_safe=False
 )
```

### Comparing `tscat_gui-0.3.1/tests/test_mypy.py` & `tscat_gui-0.3.2/tests/test_mypy.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/tscat_gui/__init__.py` & `tscat_gui-0.3.2/tscat_gui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Time series catalogue - GUI."""
 
 __author__ = """Patrick Boettcher"""
 __email__ = 'p@yai.se'
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 
 import datetime as dt
 import os
 from pathlib import Path
 from typing import List, Optional, Sequence, Type, Union, cast
 
 import itertools
@@ -427,14 +427,15 @@
         toolbar.addSeparator()
 
         action = QtGui.QAction(
             self.style().standardIcon(QtWidgets.QStyle.SP_DialogRetryButton), "Refresh",  # type: ignore
             self)
 
         action.triggered.connect(self.__refresh_current_selection)  # type: ignore
+        action.setEnabled(False)
         toolbar.addAction(action)
 
         self.refresh_action = action
 
         toolbar.addSeparator()
 
         action = QtGui.QAction(
```

### Comparing `tscat_gui-0.3.1/tscat_gui/edit.py` & `tscat_gui-0.3.2/tscat_gui/edit.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/tscat_gui/metadata.py` & `tscat_gui-0.3.2/tscat_gui/metadata.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/tscat_gui/predicate.py` & `tscat_gui-0.3.2/tscat_gui/predicate.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/tscat_gui/state.py` & `tscat_gui-0.3.2/tscat_gui/state.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/tscat_gui/tscat_driver/actions.py` & `tscat_gui-0.3.2/tscat_gui/tscat_driver/actions.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/tscat_gui/tscat_driver/catalog_model.py` & `tscat_gui-0.3.2/tscat_gui/tscat_driver/catalog_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pickle
 from typing import Any, List, Optional, Sequence, Union
 
 from PySide6.QtCore import QAbstractTableModel, QMimeData, QModelIndex, QPersistentModelIndex, Qt
 from PySide6.QtGui import QColor
 
-from tscat import _Event
+from tscat import _Event, _Catalogue
 from .actions import Action, AddEventsToCatalogueAction, DeleteAttributeAction, DeletePermanentlyAction, \
     GetCatalogueAction, MoveToTrashAction, RemoveEntitiesAction, RemoveEventsFromCatalogueAction, \
     RestoreFromTrashAction, RestorePermanentlyDeletedAction, SetAttributeAction
 from .driver import tscat_driver
 from .nodes import CatalogNode, EventNode, TrashNode
 from ..model_base.constants import EntityRole, UUIDDataRole
 
@@ -16,15 +16,15 @@
 class CatalogModel(QAbstractTableModel):
     _columns = ['start', 'stop', 'author', 'tags', 'products', 'rating']
 
     def __init__(self, root: CatalogNode):
         super().__init__()
         self._root = root
         self._trash = TrashNode()
-        tscat_driver.action_done_prioritised.connect(self._driver_action_done)
+        tscat_driver.action_done_prioritised.connect(self._driver_action_done, Qt.QueuedConnection)
 
     def _driver_action_done(self, action: Action) -> None:
         if isinstance(action, GetCatalogueAction):
             if action.uuid == self._root.uuid:
                 children = [EventNode(e, i.assigned) for e, i in zip(action.events, action.query_info)]
                 if action.removed_items:
                     # unused for now
@@ -42,14 +42,19 @@
                             child.node = e
 
                             if node == self._root:  # update model only for visible nodes
                                 index_left = self.index(row, 0, QModelIndex())
                                 index_right = self.index(row, self.columnCount() - 1, QModelIndex())
                                 self.dataChanged.emit(index_left, index_right)  # type: ignore
 
+            if action.name == 'predicate':
+                for c in filter(lambda x: isinstance(x, _Catalogue), action.entities):
+                    if c.uuid == self._root.uuid:
+                        self.refresh()
+
         elif isinstance(action, AddEventsToCatalogueAction):
             if action.catalogue_uuid == self._root.uuid:
                 nodes = list(map(lambda x: EventNode(x, True), map(tscat_driver.event_from_uuid, action.uuids)))
 
                 removed_nodes = list(filter(lambda x: x.node.is_removed(), nodes))
                 nodes = list(filter(lambda x: not x.node.is_removed(), nodes))
 
@@ -116,14 +121,17 @@
                     nodes.append(c)  # type: ignore
 
             if nodes:
                 self.beginInsertRows(QModelIndex(), self.rowCount(), self.rowCount() + len(nodes) - 1)
                 self._root.append_children(nodes)
                 self.endInsertRows()
 
+    def refresh(self):
+        tscat_driver.do(GetCatalogueAction(None, self._root.uuid))
+
     def headerData(self, section: int, orientation: Qt.Orientation,
                    role: int = Qt.DisplayRole) -> Any:  # type: ignore
         if orientation == Qt.Orientation.Horizontal:
             if role == Qt.DisplayRole:  # type: ignore
                 if section < len(self._columns):
                     return self._columns[section].title()
                 else:
```

### Comparing `tscat_gui-0.3.1/tscat_gui/tscat_driver/driver.py` & `tscat_gui-0.3.2/tscat_gui/tscat_driver/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import atexit
 from typing import Dict, Union, Optional
 
-from PySide6.QtCore import QObject, QThread, Slot, Signal
+from PySide6.QtCore import QObject, QThread, Slot, Signal, Qt
 from tscat import _Catalogue, _Event
 
 from .actions import Action, GetCataloguesAction, GetCatalogueAction, CreateEntityAction, RemoveEntitiesAction, \
     SetAttributeAction, DeleteAttributeAction, ImportCanonicalizedDictAction
 
 
 class _TscatDriverWorker(QThread):
@@ -30,16 +30,16 @@
     action_done = Signal(Action)
 
     def __init__(self, parent: Optional[QObject] = None):
         super().__init__(parent=parent)
 
         self._worker = _TscatDriverWorker()
 
-        self._do_action.connect(self._worker.do_action)
-        self._worker.action_done.connect(self._worker_action_done)
+        self._do_action.connect(self._worker.do_action, Qt.QueuedConnection)
+        self._worker.action_done.connect(self._worker_action_done, Qt.QueuedConnection)
 
         self._entity_cache: Dict[str, Union[_Event, _Catalogue]] = {}
         self.destroyed.connect(self.stop)  # type: ignore
 
     def do(self, action: Action) -> None:
         self._do_action.emit(action)
```

### Comparing `tscat_gui-0.3.1/tscat_gui/tscat_driver/model.py` & `tscat_gui-0.3.2/tscat_gui/tscat_driver/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union, Sequence, List
 
-from PySide6.QtCore import QObject, QAbstractItemModel, Signal
+from PySide6.QtCore import QObject, QAbstractItemModel, Signal, Qt
 from tscat import _Event, _Catalogue
 
 from .actions import Action
 from .tscat_root_model import TscatRootModel
 
 
 class _Model(QObject):
@@ -12,15 +12,15 @@
 
     def __init__(self):
         super().__init__(None)
 
         self._tscat_root = TscatRootModel()
 
         from .driver import tscat_driver
-        tscat_driver.action_done.connect(self._action_done)
+        tscat_driver.action_done.connect(self._action_done, Qt.QueuedConnection)
 
     def _action_done(self, action: Action) -> None:
         self.action_done.emit(action)
         if action.user_callback:
             action.user_callback(action)
 
     def catalog(self, uid: str) -> QAbstractItemModel:
```

### Comparing `tscat_gui-0.3.1/tscat_gui/tscat_driver/nodes.py` & `tscat_gui-0.3.2/tscat_gui/tscat_driver/nodes.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/tscat_gui/tscat_driver/tscat_root_model.py` & `tscat_gui-0.3.2/tscat_gui/tscat_driver/tscat_root_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self._root = RootNode()
         self._trash = TrashNode()
 
         self._root.append_child(self._trash)
 
         self._catalogues: Dict[str, CatalogModel] = {}
 
-        tscat_driver.action_done_prioritised.connect(self._driver_action_done)
+        tscat_driver.action_done_prioritised.connect(self._driver_action_done, Qt.QueuedConnection)
 
         tscat_driver.do(GetCataloguesAction(None, False))
         tscat_driver.do(GetCataloguesAction(None, True))
 
     def _trash_index(self) -> QModelIndex:
         return self.index(0, 0, QModelIndex())
 
@@ -203,15 +203,15 @@
             parent_node = cast(Node, parent.internalPointer())
 
         if isinstance(parent_node, CatalogNode):
             return 0
         else:
             return len(parent_node.children)
 
-    def columnCount(self, parent: Union[QModelIndex, QPersistentModelIndex]) -> int:  # type: ignore
+    def columnCount(self, parent: Union[QModelIndex, QPersistentModelIndex] = None) -> int:  # type: ignore
         return 1
 
     def data(self, index: Union[QModelIndex, QPersistentModelIndex],
              role: Qt.ItemDataRole = Qt.DisplayRole) -> Any:  # type: ignore
         if index.isValid():
             item = cast(NamedNode, index.internalPointer())
             if role == Qt.ItemDataRole.DisplayRole:
```

### Comparing `tscat_gui-0.3.1/tscat_gui/undo.py` & `tscat_gui-0.3.2/tscat_gui/undo.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/tscat_gui/utils/editable_label.py` & `tscat_gui-0.3.2/tscat_gui/utils/editable_label.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/tscat_gui/utils/export.py` & `tscat_gui-0.3.2/tscat_gui/utils/export.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/tscat_gui/utils/flow_layout.py` & `tscat_gui-0.3.2/tscat_gui/utils/flow_layout.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/tscat_gui/utils/helper.py` & `tscat_gui-0.3.2/tscat_gui/utils/helper.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/tscat_gui/utils/keyword_list.py` & `tscat_gui-0.3.2/tscat_gui/utils/keyword_list.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.3.1/tscat_gui.egg-info/PKG-INFO` & `tscat_gui-0.3.2/tscat_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tscat-gui
-Version: 0.3.1
+Version: 0.3.2
 Summary: Time-series catalogue - graphical user interface library
 Home-page: https://github.com/SciQLop/tscat_gui
 Author: Patrick Boettcher
 Author-email: p@yai.se
 License: GNU General Public License v3
 Keywords: tscat_gui
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `tscat_gui-0.3.1/tscat_gui.egg-info/SOURCES.txt` & `tscat_gui-0.3.2/tscat_gui.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 tscat_gui.egg-info/PKG-INFO
 tscat_gui.egg-info/SOURCES.txt
 tscat_gui.egg-info/dependency_links.txt
 tscat_gui.egg-info/entry_points.txt
 tscat_gui.egg-info/not-zip-safe
 tscat_gui.egg-info/requires.txt
 tscat_gui.egg-info/top_level.txt
+tscat_gui/model_base/__init__.py
+tscat_gui/model_base/constants.py
 tscat_gui/tscat_driver/__init__.py
 tscat_gui/tscat_driver/actions.py
 tscat_gui/tscat_driver/catalog_model.py
 tscat_gui/tscat_driver/driver.py
 tscat_gui/tscat_driver/model.py
 tscat_gui/tscat_driver/nodes.py
 tscat_gui/tscat_driver/tscat_root_model.py
```

