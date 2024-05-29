# Comparing `tmp/direnumerate-4.0rc3.tar.gz` & `tmp/direnumerate-4.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direnumerate-4.0rc3.tar", last modified: Wed May 29 14:00:07 2024, max compression
+gzip compressed data, was "direnumerate-4.0rc4.tar", last modified: Wed May 29 14:32:13 2024, max compression
```

## Comparing `direnumerate-4.0rc3.tar` & `direnumerate-4.0rc4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-29 14:00:07.362926 direnumerate-4.0rc3/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-05-29 11:49:39.000000 direnumerate-4.0rc3/LICENSE
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3282 2024-05-29 14:00:07.362926 direnumerate-4.0rc3/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1856 2024-05-29 11:52:24.000000 direnumerate-4.0rc3/README.md
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-29 14:00:07.358926 direnumerate-4.0rc3/direnumerate/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      421 2024-05-29 11:52:24.000000 direnumerate-4.0rc3/direnumerate/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    10702 2024-05-29 13:59:09.000000 direnumerate-4.0rc3/direnumerate/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-05-29 11:49:39.000000 direnumerate-4.0rc3/direnumerate/banner.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2673 2024-05-29 13:32:28.000000 direnumerate-4.0rc3/direnumerate/cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-05-29 11:49:39.000000 direnumerate-4.0rc3/direnumerate/colors.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-05-29 11:49:39.000000 direnumerate-4.0rc3/direnumerate/createlist.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      229 2024-05-29 11:49:39.000000 direnumerate-4.0rc3/direnumerate/exceptions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      981 2024-05-29 11:49:39.000000 direnumerate-4.0rc3/direnumerate/help.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2021 2024-05-29 12:07:50.000000 direnumerate-4.0rc3/direnumerate/port_scan.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-05-29 13:44:34.000000 direnumerate-4.0rc3/direnumerate/version.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      334 2024-05-29 11:49:39.000000 direnumerate-4.0rc3/direnumerate/warning.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-29 14:00:07.362926 direnumerate-4.0rc3/direnumerate.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3282 2024-05-29 14:00:07.000000 direnumerate-4.0rc3/direnumerate.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      515 2024-05-29 14:00:07.000000 direnumerate-4.0rc3/direnumerate.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-29 14:00:07.000000 direnumerate-4.0rc3/direnumerate.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-05-29 14:00:07.000000 direnumerate-4.0rc3/direnumerate.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-05-29 14:00:07.000000 direnumerate-4.0rc3/direnumerate.egg-info/requires.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-05-29 14:00:07.000000 direnumerate-4.0rc3/direnumerate.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-05-29 13:44:23.000000 direnumerate-4.0rc3/pyproject.toml
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-29 14:00:07.362926 direnumerate-4.0rc3/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-29 14:32:13.706587 direnumerate-4.0rc4/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-05-29 14:25:26.000000 direnumerate-4.0rc4/LICENSE
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3282 2024-05-29 14:32:13.706587 direnumerate-4.0rc4/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1856 2024-05-29 14:26:18.000000 direnumerate-4.0rc4/README.md
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-29 14:32:13.702587 direnumerate-4.0rc4/direnumerate/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      421 2024-05-29 14:26:18.000000 direnumerate-4.0rc4/direnumerate/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    10702 2024-05-29 14:29:45.000000 direnumerate-4.0rc4/direnumerate/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-05-29 14:25:26.000000 direnumerate-4.0rc4/direnumerate/banner.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2673 2024-05-29 14:26:18.000000 direnumerate-4.0rc4/direnumerate/cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-05-29 14:25:26.000000 direnumerate-4.0rc4/direnumerate/colors.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-05-29 14:25:26.000000 direnumerate-4.0rc4/direnumerate/createlist.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      229 2024-05-29 14:25:26.000000 direnumerate-4.0rc4/direnumerate/exceptions.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      981 2024-05-29 14:25:26.000000 direnumerate-4.0rc4/direnumerate/help.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2021 2024-05-29 14:26:18.000000 direnumerate-4.0rc4/direnumerate/port_scan.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-05-29 14:30:08.000000 direnumerate-4.0rc4/direnumerate/version.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      334 2024-05-29 14:25:26.000000 direnumerate-4.0rc4/direnumerate/warning.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-29 14:32:13.706587 direnumerate-4.0rc4/direnumerate.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3282 2024-05-29 14:32:13.000000 direnumerate-4.0rc4/direnumerate.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      515 2024-05-29 14:32:13.000000 direnumerate-4.0rc4/direnumerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-29 14:32:13.000000 direnumerate-4.0rc4/direnumerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-05-29 14:32:13.000000 direnumerate-4.0rc4/direnumerate.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-05-29 14:32:13.000000 direnumerate-4.0rc4/direnumerate.egg-info/requires.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-05-29 14:32:13.000000 direnumerate-4.0rc4/direnumerate.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-05-29 14:29:02.000000 direnumerate-4.0rc4/pyproject.toml
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-29 14:32:13.706587 direnumerate-4.0rc4/setup.cfg
```

### Comparing `direnumerate-4.0rc3/LICENSE` & `direnumerate-4.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0rc3/PKG-INFO` & `direnumerate-4.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 4.0rc3
+Version: 4.0rc4
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
-Metadata-Version: 2.1 Name: direnumerate Version: 4.0rc3 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0rc4 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-4.0rc3/README.md` & `direnumerate-4.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0rc3/direnumerate/__main__.py` & `direnumerate-4.0rc4/direnumerate/__main__.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0rc3/direnumerate/cli.py` & `direnumerate-4.0rc4/direnumerate/cli.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0rc3/direnumerate/createlist.py` & `direnumerate-4.0rc4/direnumerate/createlist.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0rc3/direnumerate/help.py` & `direnumerate-4.0rc4/direnumerate/help.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0rc3/direnumerate/port_scan.py` & `direnumerate-4.0rc4/direnumerate/port_scan.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0rc3/direnumerate.egg-info/PKG-INFO` & `direnumerate-4.0rc4/direnumerate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 4.0rc3
+Version: 4.0rc4
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
-Metadata-Version: 2.1 Name: direnumerate Version: 4.0rc3 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0rc4 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-4.0rc3/direnumerate.egg-info/SOURCES.txt` & `direnumerate-4.0rc4/direnumerate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0rc3/pyproject.toml` & `direnumerate-4.0rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "direnumerate"
-version = "4.0-rc3"
+version = "4.0-rc4"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for directory enumeration tool in web applications."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

