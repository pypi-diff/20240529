# Comparing `tmp/nbappinator-0.1.5b1.tar.gz` & `tmp/nbappinator-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbappinator-0.1.5b1.tar", last modified: Tue May  7 20:58:41 2024, max compression
+gzip compressed data, was "nbappinator-0.1.6.tar", last modified: Tue May  7 22:48:49 2024, max compression
```

## Comparing `nbappinator-0.1.5b1.tar` & `nbappinator-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:58:41.625769 nbappinator-0.1.5b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-07 20:58:41.621769 nbappinator-0.1.5b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:58:41.621769 nbappinator-0.1.5b1/nbappinator/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/aggridhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/appinator.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/browser_title.py
--rw-r--r--   0 runner    (1001) docker     (127)    15437 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/jinjamagic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/plotly_charts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/treew.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:58:41.621769 nbappinator-0.1.5b1/nbappinator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-07 20:58:41.000000 nbappinator-0.1.5b1/nbappinator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 20:58:41.000000 nbappinator-0.1.5b1/nbappinator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:58:41.000000 nbappinator-0.1.5b1/nbappinator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 20:58:41.000000 nbappinator-0.1.5b1/nbappinator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 20:58:41.000000 nbappinator-0.1.5b1/nbappinator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:58:41.625769 nbappinator-0.1.5b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:58:41.621769 nbappinator-0.1.5b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/tests/test_fails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/tests/test_nb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:48:49.831341 nbappinator-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 22:47:54.000000 nbappinator-0.1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-07 22:48:49.831341 nbappinator-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-07 22:47:54.000000 nbappinator-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:48:49.831341 nbappinator-0.1.6/nbappinator/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-07 22:47:54.000000 nbappinator-0.1.6/nbappinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 22:47:54.000000 nbappinator-0.1.6/nbappinator/aggridhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-07 22:47:54.000000 nbappinator-0.1.6/nbappinator/appinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 22:47:54.000000 nbappinator-0.1.6/nbappinator/browser_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15437 2024-05-07 22:47:54.000000 nbappinator-0.1.6/nbappinator/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:47:54.000000 nbappinator-0.1.6/nbappinator/jinjamagic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-07 22:47:54.000000 nbappinator-0.1.6/nbappinator/plotly_charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 22:47:54.000000 nbappinator-0.1.6/nbappinator/treew.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 22:47:54.000000 nbappinator-0.1.6/nbappinator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:48:49.831341 nbappinator-0.1.6/nbappinator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-07 22:48:49.000000 nbappinator-0.1.6/nbappinator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 22:48:49.000000 nbappinator-0.1.6/nbappinator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:48:49.000000 nbappinator-0.1.6/nbappinator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 22:48:49.000000 nbappinator-0.1.6/nbappinator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 22:48:49.000000 nbappinator-0.1.6/nbappinator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-07 22:47:54.000000 nbappinator-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:48:49.831341 nbappinator-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:48:49.831341 nbappinator-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-07 22:47:54.000000 nbappinator-0.1.6/tests/test_fails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 22:47:54.000000 nbappinator-0.1.6/tests/test_nb.py
```

### Comparing `nbappinator-0.1.5b1/LICENSE.md` & `nbappinator-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.5b1/PKG-INFO` & `nbappinator-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbappinator
-Version: 0.1.5b1
+Version: 0.1.6
 Summary: Jupyter Notebook Application Builder
 Author-email: Paul T <paul@iqmo.com>
 Maintainer-email: Paul T <paul@iqmo.com>
 Project-URL: Homepage, https://github.com/iqmo-org/nbappinator
 Project-URL: Repository, https://github.com/iqmo-org/nbappinator
 Project-URL: Issues, https://github.com/iqmo-org/nbappinator/issues
 Requires-Python: >=3.9
@@ -34,15 +34,15 @@
 
 - Simplify UI development for Notebook developers by reducing the surface area of APIs to learn.
 - Abstract the underlying UI components, allowing nbappinator to plug in different frameworks to achieve equivalent behavior.
 - Provide a foundation to develop reusable and portable themes to improve app styling.
 
 # Example
 
-![Example](readme_example.png)
+<!--![Example](readme_example.png)-->
 
 # Getting Started
 
 ```py
 import nbappinator as nbapp
 
 def my_action(component, action, args, app: nbapp.UiModel, caller: str):
```

### Comparing `nbappinator-0.1.5b1/README.md` & `nbappinator-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 - Simplify UI development for Notebook developers by reducing the surface area of APIs to learn.
 - Abstract the underlying UI components, allowing nbappinator to plug in different frameworks to achieve equivalent behavior.
 - Provide a foundation to develop reusable and portable themes to improve app styling.
 
 # Example
 
-![Example](readme_example.png)
+<!--![Example](readme_example.png)-->
 
 # Getting Started
 
 ```py
 import nbappinator as nbapp
 
 def my_action(component, action, args, app: nbapp.UiModel, caller: str):
```

### Comparing `nbappinator-0.1.5b1/nbappinator/aggridhelper.py` & `nbappinator-0.1.6/nbappinator/aggridhelper.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.5b1/nbappinator/appinator.py` & `nbappinator-0.1.6/nbappinator/appinator.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.5b1/nbappinator/browser_title.py` & `nbappinator-0.1.6/nbappinator/browser_title.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.5b1/nbappinator/datagrid.py` & `nbappinator-0.1.6/nbappinator/datagrid.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.5b1/nbappinator/plotly_charts.py` & `nbappinator-0.1.6/nbappinator/plotly_charts.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.5b1/nbappinator/treew.py` & `nbappinator-0.1.6/nbappinator/treew.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.5b1/nbappinator.egg-info/PKG-INFO` & `nbappinator-0.1.6/nbappinator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbappinator
-Version: 0.1.5b1
+Version: 0.1.6
 Summary: Jupyter Notebook Application Builder
 Author-email: Paul T <paul@iqmo.com>
 Maintainer-email: Paul T <paul@iqmo.com>
 Project-URL: Homepage, https://github.com/iqmo-org/nbappinator
 Project-URL: Repository, https://github.com/iqmo-org/nbappinator
 Project-URL: Issues, https://github.com/iqmo-org/nbappinator/issues
 Requires-Python: >=3.9
@@ -34,15 +34,15 @@
 
 - Simplify UI development for Notebook developers by reducing the surface area of APIs to learn.
 - Abstract the underlying UI components, allowing nbappinator to plug in different frameworks to achieve equivalent behavior.
 - Provide a foundation to develop reusable and portable themes to improve app styling.
 
 # Example
 
-![Example](readme_example.png)
+<!--![Example](readme_example.png)-->
 
 # Getting Started
 
 ```py
 import nbappinator as nbapp
 
 def my_action(component, action, args, app: nbapp.UiModel, caller: str):
```

### Comparing `nbappinator-0.1.5b1/pyproject.toml` & `nbappinator-0.1.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -24,15 +24,12 @@
 ignore-init-module-imports = true
 
 [tool.pyright]
 typeCheckingMode = "basic"
 reportGeneralTypeIssues = false
 reportPrivateImportUsage = false
 
-#[tools.setuptools]
-#packages = ["nbappinator"]
-
 [tool.setuptools.dynamic]
 version = {attr = "nbappinator.version.__version__"}
 
-[tool.setuptools.package-dir]
-mypkg = "nbappinator"
+[tool.setuptools]
+packages = ["nbappinator"]
```

### Comparing `nbappinator-0.1.5b1/tests/test_fails.py` & `nbappinator-0.1.6/tests/test_fails.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.5b1/tests/test_nb.py` & `nbappinator-0.1.6/tests/test_nb.py`

 * *Files identical despite different names*

