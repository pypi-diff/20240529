# Comparing `tmp/shinylive-0.4.0.tar.gz` & `tmp/shinylive-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinylive-0.4.0.tar", last modified: Thu May 23 20:35:15 2024, max compression
+gzip compressed data, was "shinylive-0.4.1.tar", last modified: Wed May 29 17:59:43 2024, max compression
```

## Comparing `shinylive-0.4.0.tar` & `shinylive-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:35:15.849802 shinylive-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-23 20:34:59.000000 shinylive-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-23 20:35:15.849802 shinylive-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-23 20:34:59.000000 shinylive-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-23 20:35:15.849802 shinylive-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:34:59.000000 shinylive-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:35:15.849802 shinylive-0.4.0/shinylive/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_app_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)    19230 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    17783 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    25131 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:35:15.849802 shinylive-0.4.0/shinylive/_version/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:35:15.849802 shinylive-0.4.0/shinylive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:59:43.056844 shinylive-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-29 17:59:28.000000 shinylive-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-29 17:59:43.056844 shinylive-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-29 17:59:28.000000 shinylive-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-29 17:59:43.060844 shinylive-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:59:28.000000 shinylive-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:59:43.056844 shinylive-0.4.1/shinylive/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 17:59:28.000000 shinylive-0.4.1/shinylive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-29 17:59:28.000000 shinylive-0.4.1/shinylive/_app_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-05-29 17:59:28.000000 shinylive-0.4.1/shinylive/_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19230 2024-05-29 17:59:28.000000 shinylive-0.4.1/shinylive/_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-29 17:59:28.000000 shinylive-0.4.1/shinylive/_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17783 2024-05-29 17:59:28.000000 shinylive-0.4.1/shinylive/_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25131 2024-05-29 17:59:28.000000 shinylive-0.4.1/shinylive/_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-29 17:59:28.000000 shinylive-0.4.1/shinylive/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:59:43.056844 shinylive-0.4.1/shinylive/_version/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-29 17:59:28.000000 shinylive-0.4.1/shinylive/_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:59:28.000000 shinylive-0.4.1/shinylive/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:59:43.056844 shinylive-0.4.1/shinylive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-29 17:59:43.000000 shinylive-0.4.1/shinylive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-29 17:59:43.000000 shinylive-0.4.1/shinylive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:59:43.000000 shinylive-0.4.1/shinylive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-29 17:59:43.000000 shinylive-0.4.1/shinylive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:59:43.000000 shinylive-0.4.1/shinylive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-29 17:59:43.000000 shinylive-0.4.1/shinylive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 17:59:43.000000 shinylive-0.4.1/shinylive.egg-info/top_level.txt
```

### Comparing `shinylive-0.4.0/LICENSE` & `shinylive-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shinylive-0.4.0/PKG-INFO` & `shinylive-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinylive
-Version: 0.4.0
+Version: 0.4.1
 Summary: Run Shiny applications running Python in the browser.
 Home-page: https://github.com/posit-dev/py-shinylive
 Author: Winston Chang
 Author-email: winston@posit.co
 License: MIT
 Project-URL: Bug Tracker, https://github.com/posit-dev/py-shinylive/issues
 Project-URL: Documentation, https://github.com/posit-dev/py-shinylive
```

### Comparing `shinylive-0.4.0/README.md` & `shinylive-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `shinylive-0.4.0/setup.cfg` & `shinylive-0.4.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 	setuptools
 install_requires = 
 	shiny
 	click>=8.1.7
 	appdirs>=1.4.4
 	lzstring>=1.0.4
 	typing-extensions>=4.0.1
+	setuptools; python_version>='3.12'
 tests_require = 
 	pytest>=3
 zip_safe = False
 
 [options.extras_require]
 test = 
 	pytest>=6.2.4
```

### Comparing `shinylive-0.4.0/shinylive/_app_json.py` & `shinylive-0.4.1/shinylive/_app_json.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.4.0/shinylive/_assets.py` & `shinylive-0.4.1/shinylive/_assets.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.4.0/shinylive/_deps.py` & `shinylive-0.4.1/shinylive/_deps.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.4.0/shinylive/_export.py` & `shinylive-0.4.1/shinylive/_export.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.4.0/shinylive/_main.py` & `shinylive-0.4.1/shinylive/_main.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.4.0/shinylive/_url.py` & `shinylive-0.4.1/shinylive/_url.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.4.0/shinylive/_utils.py` & `shinylive-0.4.1/shinylive/_utils.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.4.0/shinylive.egg-info/PKG-INFO` & `shinylive-0.4.1/shinylive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinylive
-Version: 0.4.0
+Version: 0.4.1
 Summary: Run Shiny applications running Python in the browser.
 Home-page: https://github.com/posit-dev/py-shinylive
 Author: Winston Chang
 Author-email: winston@posit.co
 License: MIT
 Project-URL: Bug Tracker, https://github.com/posit-dev/py-shinylive/issues
 Project-URL: Documentation, https://github.com/posit-dev/py-shinylive
```

