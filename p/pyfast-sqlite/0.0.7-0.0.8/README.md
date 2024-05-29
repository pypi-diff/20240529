# Comparing `tmp/pyfast_sqlite-0.0.7.tar.gz` & `tmp/pyfast_sqlite-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfast_sqlite-0.0.7.tar", last modified: Wed May 29 13:28:11 2024, max compression
+gzip compressed data, was "pyfast_sqlite-0.0.8.tar", last modified: Wed May 29 13:39:47 2024, max compression
```

## Comparing `pyfast_sqlite-0.0.7.tar` & `pyfast_sqlite-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 13:28:12.000000 pyfast_sqlite-0.0.7/
--rw-rw-rw-   0        0        0     1091 2024-05-29 12:56:34.000000 pyfast_sqlite-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2633 2024-05-29 13:28:12.000000 pyfast_sqlite-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2046 2024-05-29 12:56:34.000000 pyfast_sqlite-0.0.7/README.md
--rw-rw-rw-   0        0        0      106 2024-05-29 13:28:04.000000 pyfast_sqlite-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 13:28:12.000000 pyfast_sqlite-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      925 2024-05-29 13:24:12.000000 pyfast_sqlite-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:28:12.000000 pyfast_sqlite-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-29 13:28:12.000000 pyfast_sqlite-0.0.7/src/pyfast_sqlite.egg-info/
--rw-rw-rw-   0        0        0     2633 2024-05-29 13:28:12.000000 pyfast_sqlite-0.0.7/src/pyfast_sqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-29 13:28:12.000000 pyfast_sqlite-0.0.7/src/pyfast_sqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 13:28:12.000000 pyfast_sqlite-0.0.7/src/pyfast_sqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 13:28:12.000000 pyfast_sqlite-0.0.7/src/pyfast_sqlite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 13:39:48.000000 pyfast_sqlite-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2024-05-29 12:56:34.000000 pyfast_sqlite-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2655 2024-05-29 13:39:48.000000 pyfast_sqlite-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2046 2024-05-29 12:56:34.000000 pyfast_sqlite-0.0.8/README.md
+-rw-rw-rw-   0        0        0      106 2024-05-29 13:28:04.000000 pyfast_sqlite-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 13:39:48.000000 pyfast_sqlite-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      975 2024-05-29 13:39:24.000000 pyfast_sqlite-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:39:48.000000 pyfast_sqlite-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 13:39:48.000000 pyfast_sqlite-0.0.8/src/pyfast-sqlite/
+-rw-rw-rw-   0        0        0      134 2024-05-29 13:39:32.000000 pyfast_sqlite-0.0.8/src/pyfast-sqlite/__init__.py
+-rw-rw-rw-   0        0        0     2019 2024-05-29 12:56:34.000000 pyfast_sqlite-0.0.8/src/pyfast-sqlite/fast_sql.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:39:48.000000 pyfast_sqlite-0.0.8/src/pyfast_sqlite.egg-info/
+-rw-rw-rw-   0        0        0     2655 2024-05-29 13:39:48.000000 pyfast_sqlite-0.0.8/src/pyfast_sqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-29 13:39:48.000000 pyfast_sqlite-0.0.8/src/pyfast_sqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 13:39:48.000000 pyfast_sqlite-0.0.8/src/pyfast_sqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-29 13:39:48.000000 pyfast_sqlite-0.0.8/src/pyfast_sqlite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-29 13:39:48.000000 pyfast_sqlite-0.0.8/src/pyfast_sqlite.egg-info/top_level.txt
```

### Comparing `pyfast_sqlite-0.0.7/LICENSE` & `pyfast_sqlite-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfast_sqlite-0.0.7/PKG-INFO` & `pyfast_sqlite-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pyfast-sqlite
-Version: 0.0.7
+Version: 0.0.8
 Summary: Fast_sqlite is a library to use sqlite database faster and easier.
 Home-page: https://github.com/Unknow-per/Fast_sqlite-lIbrary
 Author: Farbod Parkhooi
 Author-email: farbod.p1390@gmail.com
 Project-URL: Bug Tracker, https://github.com/Unknow-per/Fast_sqlite-lIbrary/~/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 
 # Fast_sqlite
 
 <b>Fast SQL</b> is a Python library to make and use a sqlite3 database. For use this library you can copy the file in your code directory and use below codes or read <b>src/example/write_and_read_data.py</b> file
 
 # Create values to use library
 ```python
```

### Comparing `pyfast_sqlite-0.0.7/README.md` & `pyfast_sqlite-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyfast_sqlite-0.0.7/setup.py` & `pyfast_sqlite-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pyfast-sqlite",
-    version = "0.0.7",
+    version = "0.0.8",
     author = "Farbod Parkhooi",
     author_email = "farbod.p1390@gmail.com",
     description = "Fast_sqlite is a library to use sqlite database faster and easier.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/Unknow-per/Fast_sqlite-lIbrary",
     project_urls = {
         "Bug Tracker": "https://github.com/Unknow-per/Fast_sqlite-lIbrary/~/issues",
     },
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    install_requires=[
+        'numpy',
+    ],
     package_dir = {"": "src"},
     packages = setuptools.find_packages(where="src"),
     python_requires = ">=3.8"
 )
```

### Comparing `pyfast_sqlite-0.0.7/src/pyfast_sqlite.egg-info/PKG-INFO` & `pyfast_sqlite-0.0.8/src/pyfast_sqlite.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pyfast-sqlite
-Version: 0.0.7
+Version: 0.0.8
 Summary: Fast_sqlite is a library to use sqlite database faster and easier.
 Home-page: https://github.com/Unknow-per/Fast_sqlite-lIbrary
 Author: Farbod Parkhooi
 Author-email: farbod.p1390@gmail.com
 Project-URL: Bug Tracker, https://github.com/Unknow-per/Fast_sqlite-lIbrary/~/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 
 # Fast_sqlite
 
 <b>Fast SQL</b> is a Python library to make and use a sqlite3 database. For use this library you can copy the file in your code directory and use below codes or read <b>src/example/write_and_read_data.py</b> file
 
 # Create values to use library
 ```python
```

