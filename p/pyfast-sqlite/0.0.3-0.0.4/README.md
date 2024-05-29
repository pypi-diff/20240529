# Comparing `tmp/pyfast_sqlite-0.0.3.tar.gz` & `tmp/pyfast_sqlite-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfast_sqlite-0.0.3.tar", last modified: Wed May 29 12:46:00 2024, max compression
+gzip compressed data, was "pyfast_sqlite-0.0.4.tar", last modified: Wed May 29 12:49:07 2024, max compression
```

## Comparing `pyfast_sqlite-0.0.3.tar` & `pyfast_sqlite-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 12:46:00.000000 pyfast_sqlite-0.0.3/
--rw-rw-rw-   0        0        0     1091 2024-05-28 09:41:46.000000 pyfast_sqlite-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2633 2024-05-29 12:46:02.000000 pyfast_sqlite-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2046 2024-05-29 11:29:56.000000 pyfast_sqlite-0.0.3/README.md
--rw-rw-rw-   0        0        0       70 2024-05-29 12:45:00.000000 pyfast_sqlite-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 12:46:02.000000 pyfast_sqlite-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      923 2024-05-29 12:45:44.000000 pyfast_sqlite-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:46:00.000000 pyfast_sqlite-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-29 12:46:00.000000 pyfast_sqlite-0.0.3/src/pyfast_sqlite.egg-info/
--rw-rw-rw-   0        0        0     2633 2024-05-29 12:46:00.000000 pyfast_sqlite-0.0.3/src/pyfast_sqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-29 12:46:00.000000 pyfast_sqlite-0.0.3/src/pyfast_sqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 12:46:00.000000 pyfast_sqlite-0.0.3/src/pyfast_sqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 12:46:00.000000 pyfast_sqlite-0.0.3/src/pyfast_sqlite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 12:49:08.000000 pyfast_sqlite-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2024-05-28 09:41:46.000000 pyfast_sqlite-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2633 2024-05-29 12:49:08.000000 pyfast_sqlite-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2046 2024-05-29 11:29:56.000000 pyfast_sqlite-0.0.4/README.md
+-rw-rw-rw-   0        0        0       72 2024-05-29 12:49:06.000000 pyfast_sqlite-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 12:49:08.000000 pyfast_sqlite-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      923 2024-05-29 12:49:00.000000 pyfast_sqlite-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:49:08.000000 pyfast_sqlite-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 12:49:08.000000 pyfast_sqlite-0.0.4/src/pyfast_sqlite.egg-info/
+-rw-rw-rw-   0        0        0     2633 2024-05-29 12:49:08.000000 pyfast_sqlite-0.0.4/src/pyfast_sqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-05-29 12:49:08.000000 pyfast_sqlite-0.0.4/src/pyfast_sqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:49:08.000000 pyfast_sqlite-0.0.4/src/pyfast_sqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:49:08.000000 pyfast_sqlite-0.0.4/src/pyfast_sqlite.egg-info/top_level.txt
```

### Comparing `pyfast_sqlite-0.0.3/LICENSE` & `pyfast_sqlite-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfast_sqlite-0.0.3/PKG-INFO` & `pyfast_sqlite-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfast-sqlite
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fast_sqlite is a library to use sqlite database faster and easier.
 Home-page: https://github.com/Unknow-per/Fast_sqlite-lIbrary
 Author: Farbod Parkhooi
 Author-email: farbod.p1390@gmail.com
 Project-URL: Bug Tracker, https://github.com/Unknow-per/Fast_sqlite-lIbrary/~/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyfast_sqlite-0.0.3/README.md` & `pyfast_sqlite-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyfast_sqlite-0.0.3/setup.py` & `pyfast_sqlite-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pyfast-sqlite",
-    version = "0.0.3",
+    version = "0.0.4",
     author = "Farbod Parkhooi",
     author_email = "farbod.p1390@gmail.com",
     description = "Fast_sqlite is a library to use sqlite database faster and easier.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/Unknow-per/Fast_sqlite-lIbrary",
     project_urls = {
```

### Comparing `pyfast_sqlite-0.0.3/src/pyfast_sqlite.egg-info/PKG-INFO` & `pyfast_sqlite-0.0.4/src/pyfast_sqlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfast-sqlite
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fast_sqlite is a library to use sqlite database faster and easier.
 Home-page: https://github.com/Unknow-per/Fast_sqlite-lIbrary
 Author: Farbod Parkhooi
 Author-email: farbod.p1390@gmail.com
 Project-URL: Bug Tracker, https://github.com/Unknow-per/Fast_sqlite-lIbrary/~/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

