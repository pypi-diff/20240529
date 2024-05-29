# Comparing `tmp/pyfast_sqlite-0.0.1.tar.gz` & `tmp/pyfast_sqlite-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfast_sqlite-0.0.1.tar", last modified: Wed May 29 12:37:12 2024, max compression
+gzip compressed data, was "pyfast_sqlite-0.0.2.tar", last modified: Wed May 29 12:43:45 2024, max compression
```

## Comparing `pyfast_sqlite-0.0.1.tar` & `pyfast_sqlite-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 12:37:14.000000 pyfast_sqlite-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-05-28 09:41:46.000000 pyfast_sqlite-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2633 2024-05-29 12:37:14.000000 pyfast_sqlite-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2046 2024-05-29 11:29:56.000000 pyfast_sqlite-0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2024-05-29 12:20:54.000000 pyfast_sqlite-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 12:37:14.000000 pyfast_sqlite-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      923 2024-05-29 12:35:22.000000 pyfast_sqlite-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:37:14.000000 pyfast_sqlite-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-29 12:37:14.000000 pyfast_sqlite-0.0.1/src/pyfast_sqlite.egg-info/
--rw-rw-rw-   0        0        0     2633 2024-05-29 12:37:14.000000 pyfast_sqlite-0.0.1/src/pyfast_sqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-29 12:37:14.000000 pyfast_sqlite-0.0.1/src/pyfast_sqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 12:37:14.000000 pyfast_sqlite-0.0.1/src/pyfast_sqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 12:37:14.000000 pyfast_sqlite-0.0.1/src/pyfast_sqlite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 12:43:46.000000 pyfast_sqlite-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-05-28 09:41:46.000000 pyfast_sqlite-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2633 2024-05-29 12:43:46.000000 pyfast_sqlite-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2046 2024-05-29 11:29:56.000000 pyfast_sqlite-0.0.2/README.md
+-rw-rw-rw-   0        0        0       88 2024-05-29 12:43:36.000000 pyfast_sqlite-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 12:43:46.000000 pyfast_sqlite-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      923 2024-05-29 12:43:32.000000 pyfast_sqlite-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:43:46.000000 pyfast_sqlite-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 12:43:46.000000 pyfast_sqlite-0.0.2/src/pyfast_sqlite.egg-info/
+-rw-rw-rw-   0        0        0     2633 2024-05-29 12:43:46.000000 pyfast_sqlite-0.0.2/src/pyfast_sqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-05-29 12:43:46.000000 pyfast_sqlite-0.0.2/src/pyfast_sqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:43:46.000000 pyfast_sqlite-0.0.2/src/pyfast_sqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:43:46.000000 pyfast_sqlite-0.0.2/src/pyfast_sqlite.egg-info/top_level.txt
```

### Comparing `pyfast_sqlite-0.0.1/LICENSE` & `pyfast_sqlite-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfast_sqlite-0.0.1/PKG-INFO` & `pyfast_sqlite-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfast-sqlite
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fast_sqlite is a library to use sqlite database faster and easier.
 Home-page: https://github.com/Unknow-per/Fast_sqlite-lIbrary
 Author: Farbod Parkhooi
 Author-email: farbod.p1390@gmail.com
 Project-URL: Bug Tracker, https://github.com/Unknow-per/Fast_sqlite-lIbrary/~/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyfast_sqlite-0.0.1/README.md` & `pyfast_sqlite-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyfast_sqlite-0.0.1/setup.py` & `pyfast_sqlite-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pyfast-sqlite",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "Farbod Parkhooi",
     author_email = "farbod.p1390@gmail.com",
     description = "Fast_sqlite is a library to use sqlite database faster and easier.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/Unknow-per/Fast_sqlite-lIbrary",
     project_urls = {
```

### Comparing `pyfast_sqlite-0.0.1/src/pyfast_sqlite.egg-info/PKG-INFO` & `pyfast_sqlite-0.0.2/src/pyfast_sqlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfast-sqlite
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fast_sqlite is a library to use sqlite database faster and easier.
 Home-page: https://github.com/Unknow-per/Fast_sqlite-lIbrary
 Author: Farbod Parkhooi
 Author-email: farbod.p1390@gmail.com
 Project-URL: Bug Tracker, https://github.com/Unknow-per/Fast_sqlite-lIbrary/~/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

