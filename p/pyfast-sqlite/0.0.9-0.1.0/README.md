# Comparing `tmp/pyfast_sqlite-0.0.9.tar.gz` & `tmp/pyfast_sqlite-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfast_sqlite-0.0.9.tar", last modified: Wed May 29 13:46:23 2024, max compression
+gzip compressed data, was "pyfast_sqlite-0.1.0.tar", last modified: Wed May 29 13:51:12 2024, max compression
```

## Comparing `pyfast_sqlite-0.0.9.tar` & `pyfast_sqlite-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 13:46:24.000000 pyfast_sqlite-0.0.9/
--rw-rw-rw-   0        0        0     1091 2024-05-29 12:56:34.000000 pyfast_sqlite-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     2655 2024-05-29 13:46:24.000000 pyfast_sqlite-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2046 2024-05-29 12:56:34.000000 pyfast_sqlite-0.0.9/README.md
--rw-rw-rw-   0        0        0      106 2024-05-29 13:28:04.000000 pyfast_sqlite-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 13:46:24.000000 pyfast_sqlite-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      975 2024-05-29 13:46:08.000000 pyfast_sqlite-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:46:24.000000 pyfast_sqlite-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2024-05-29 13:46:24.000000 pyfast_sqlite-0.0.9/src/pyfast_sqlite/
--rw-rw-rw-   0        0        0      134 2024-05-29 13:46:16.000000 pyfast_sqlite-0.0.9/src/pyfast_sqlite/__init__.py
--rw-rw-rw-   0        0        0     2019 2024-05-29 12:56:34.000000 pyfast_sqlite-0.0.9/src/pyfast_sqlite/fast_sql.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:46:24.000000 pyfast_sqlite-0.0.9/src/pyfast_sqlite.egg-info/
--rw-rw-rw-   0        0        0     2655 2024-05-29 13:46:24.000000 pyfast_sqlite-0.0.9/src/pyfast_sqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-29 13:46:24.000000 pyfast_sqlite-0.0.9/src/pyfast_sqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 13:46:24.000000 pyfast_sqlite-0.0.9/src/pyfast_sqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-29 13:46:24.000000 pyfast_sqlite-0.0.9/src/pyfast_sqlite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-29 13:46:24.000000 pyfast_sqlite-0.0.9/src/pyfast_sqlite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 13:51:12.000000 pyfast_sqlite-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2024-05-29 12:56:34.000000 pyfast_sqlite-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2655 2024-05-29 13:51:14.000000 pyfast_sqlite-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2046 2024-05-29 12:56:34.000000 pyfast_sqlite-0.1.0/README.md
+-rw-rw-rw-   0        0        0      106 2024-05-29 13:28:04.000000 pyfast_sqlite-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 13:51:14.000000 pyfast_sqlite-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      975 2024-05-29 13:51:00.000000 pyfast_sqlite-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:51:12.000000 pyfast_sqlite-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 13:51:12.000000 pyfast_sqlite-0.1.0/src/pyfast_sqlite/
+-rw-rw-rw-   0        0        0      135 2024-05-29 13:50:54.000000 pyfast_sqlite-0.1.0/src/pyfast_sqlite/__init__.py
+-rw-rw-rw-   0        0        0     2019 2024-05-29 12:56:34.000000 pyfast_sqlite-0.1.0/src/pyfast_sqlite/fast_sql.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:51:12.000000 pyfast_sqlite-0.1.0/src/pyfast_sqlite.egg-info/
+-rw-rw-rw-   0        0        0     2655 2024-05-29 13:51:12.000000 pyfast_sqlite-0.1.0/src/pyfast_sqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-29 13:51:12.000000 pyfast_sqlite-0.1.0/src/pyfast_sqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 13:51:12.000000 pyfast_sqlite-0.1.0/src/pyfast_sqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-29 13:51:12.000000 pyfast_sqlite-0.1.0/src/pyfast_sqlite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-29 13:51:12.000000 pyfast_sqlite-0.1.0/src/pyfast_sqlite.egg-info/top_level.txt
```

### Comparing `pyfast_sqlite-0.0.9/LICENSE` & `pyfast_sqlite-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfast_sqlite-0.0.9/PKG-INFO` & `pyfast_sqlite-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfast-sqlite
-Version: 0.0.9
+Version: 0.1.0
 Summary: Fast_sqlite is a library to use sqlite database faster and easier.
 Home-page: https://github.com/Unknow-per/Fast_sqlite-lIbrary
 Author: Farbod Parkhooi
 Author-email: farbod.p1390@gmail.com
 Project-URL: Bug Tracker, https://github.com/Unknow-per/Fast_sqlite-lIbrary/~/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyfast_sqlite-0.0.9/README.md` & `pyfast_sqlite-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyfast_sqlite-0.0.9/setup.py` & `pyfast_sqlite-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pyfast-sqlite",
-    version = "0.0.9",
+    version = "0.1.0",
     author = "Farbod Parkhooi",
     author_email = "farbod.p1390@gmail.com",
     description = "Fast_sqlite is a library to use sqlite database faster and easier.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/Unknow-per/Fast_sqlite-lIbrary",
     project_urls = {
```

### Comparing `pyfast_sqlite-0.0.9/src/pyfast_sqlite/fast_sql.py` & `pyfast_sqlite-0.1.0/src/pyfast_sqlite/fast_sql.py`

 * *Files identical despite different names*

### Comparing `pyfast_sqlite-0.0.9/src/pyfast_sqlite.egg-info/PKG-INFO` & `pyfast_sqlite-0.1.0/src/pyfast_sqlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfast-sqlite
-Version: 0.0.9
+Version: 0.1.0
 Summary: Fast_sqlite is a library to use sqlite database faster and easier.
 Home-page: https://github.com/Unknow-per/Fast_sqlite-lIbrary
 Author: Farbod Parkhooi
 Author-email: farbod.p1390@gmail.com
 Project-URL: Bug Tracker, https://github.com/Unknow-per/Fast_sqlite-lIbrary/~/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

