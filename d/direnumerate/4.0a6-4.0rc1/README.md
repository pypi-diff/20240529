# Comparing `tmp/direnumerate-4.0a6.tar.gz` & `tmp/direnumerate-4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direnumerate-4.0a6.tar", last modified: Sun May 26 15:50:14 2024, max compression
+gzip compressed data, was "direnumerate-4.0rc1.tar", last modified: Wed May 29 13:13:48 2024, max compression
```

## Comparing `direnumerate-4.0a6.tar` & `direnumerate-4.0rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-26 15:50:14.919219 direnumerate-4.0a6/
--rw-rw-r--   0 juan      (1000) juan      (1000)    18092 2024-05-26 15:20:14.000000 direnumerate-4.0a6/LICENSE
--rw-r--r--   0 juan      (1000) juan      (1000)     3281 2024-05-26 15:50:14.919219 direnumerate-4.0a6/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     1856 2024-05-26 15:45:06.000000 direnumerate-4.0a6/README.md
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-26 15:50:14.919219 direnumerate-4.0a6/direnumerate/
--rw-rw-r--   0 juan      (1000) juan      (1000)      421 2024-05-26 15:22:27.000000 direnumerate-4.0a6/direnumerate/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     7889 2024-05-26 15:46:43.000000 direnumerate-4.0a6/direnumerate/__main__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      125 2024-05-26 15:20:14.000000 direnumerate-4.0a6/direnumerate/banner.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2605 2024-05-26 15:47:09.000000 direnumerate-4.0a6/direnumerate/cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      394 2024-05-26 15:20:14.000000 direnumerate-4.0a6/direnumerate/colors.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    23461 2024-05-26 15:20:14.000000 direnumerate-4.0a6/direnumerate/createlist.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      229 2024-05-26 15:20:14.000000 direnumerate-4.0a6/direnumerate/exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      981 2024-05-26 15:20:14.000000 direnumerate-4.0a6/direnumerate/help.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2021 2024-05-26 15:22:27.000000 direnumerate-4.0a6/direnumerate/port_scan.py
--rw-rw-r--   0 juan      (1000) juan      (1000)       73 2024-05-26 15:24:55.000000 direnumerate-4.0a6/direnumerate/version.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      334 2024-05-26 15:20:14.000000 direnumerate-4.0a6/direnumerate/warning.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-26 15:50:14.919219 direnumerate-4.0a6/direnumerate.egg-info/
--rw-r--r--   0 juan      (1000) juan      (1000)     3281 2024-05-26 15:50:14.000000 direnumerate-4.0a6/direnumerate.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)      515 2024-05-26 15:50:14.000000 direnumerate-4.0a6/direnumerate.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-26 15:50:14.000000 direnumerate-4.0a6/direnumerate.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       55 2024-05-26 15:50:14.000000 direnumerate-4.0a6/direnumerate.egg-info/entry_points.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        9 2024-05-26 15:50:14.000000 direnumerate-4.0a6/direnumerate.egg-info/requires.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       13 2024-05-26 15:50:14.000000 direnumerate-4.0a6/direnumerate.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)     1567 2024-05-26 15:25:02.000000 direnumerate-4.0a6/pyproject.toml
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-26 15:50:14.919219 direnumerate-4.0a6/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-29 13:13:48.205270 direnumerate-4.0rc1/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-05-29 11:49:39.000000 direnumerate-4.0rc1/LICENSE
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3282 2024-05-29 13:13:48.205270 direnumerate-4.0rc1/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1856 2024-05-29 11:52:24.000000 direnumerate-4.0rc1/README.md
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-29 13:13:48.197270 direnumerate-4.0rc1/direnumerate/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      421 2024-05-29 11:52:24.000000 direnumerate-4.0rc1/direnumerate/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    10710 2024-05-29 13:12:31.000000 direnumerate-4.0rc1/direnumerate/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-05-29 11:49:39.000000 direnumerate-4.0rc1/direnumerate/banner.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2605 2024-05-29 12:47:49.000000 direnumerate-4.0rc1/direnumerate/cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-05-29 11:49:39.000000 direnumerate-4.0rc1/direnumerate/colors.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-05-29 11:49:39.000000 direnumerate-4.0rc1/direnumerate/createlist.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      229 2024-05-29 11:49:39.000000 direnumerate-4.0rc1/direnumerate/exceptions.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      981 2024-05-29 11:49:39.000000 direnumerate-4.0rc1/direnumerate/help.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2021 2024-05-29 12:07:50.000000 direnumerate-4.0rc1/direnumerate/port_scan.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-05-29 12:24:09.000000 direnumerate-4.0rc1/direnumerate/version.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      334 2024-05-29 11:49:39.000000 direnumerate-4.0rc1/direnumerate/warning.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-29 13:13:48.201270 direnumerate-4.0rc1/direnumerate.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3282 2024-05-29 13:13:47.000000 direnumerate-4.0rc1/direnumerate.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      515 2024-05-29 13:13:48.000000 direnumerate-4.0rc1/direnumerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-29 13:13:48.000000 direnumerate-4.0rc1/direnumerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-05-29 13:13:48.000000 direnumerate-4.0rc1/direnumerate.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-05-29 13:13:48.000000 direnumerate-4.0rc1/direnumerate.egg-info/requires.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-05-29 13:13:48.000000 direnumerate-4.0rc1/direnumerate.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-05-29 12:47:52.000000 direnumerate-4.0rc1/pyproject.toml
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-29 13:13:48.205270 direnumerate-4.0rc1/setup.cfg
```

### Comparing `direnumerate-4.0a6/LICENSE` & `direnumerate-4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a6/PKG-INFO` & `direnumerate-4.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 4.0a6
+Version: 4.0rc1
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 4.0a6 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0rc1 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-4.0a6/README.md` & `direnumerate-4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a6/direnumerate/cli.py` & `direnumerate-4.0rc1/direnumerate/cli.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a6/direnumerate/createlist.py` & `direnumerate-4.0rc1/direnumerate/createlist.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a6/direnumerate/help.py` & `direnumerate-4.0rc1/direnumerate/help.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a6/direnumerate/port_scan.py` & `direnumerate-4.0rc1/direnumerate/port_scan.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a6/direnumerate.egg-info/PKG-INFO` & `direnumerate-4.0rc1/direnumerate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 4.0a6
+Version: 4.0rc1
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 4.0a6 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0rc1 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-4.0a6/direnumerate.egg-info/SOURCES.txt` & `direnumerate-4.0rc1/direnumerate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a6/pyproject.toml` & `direnumerate-4.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "direnumerate"
-version = "4.0a6"
+version = "4.0-rc1"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for directory enumeration tool in web applications."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

