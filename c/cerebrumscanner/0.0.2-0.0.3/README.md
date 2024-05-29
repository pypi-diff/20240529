# Comparing `tmp/cerebrumscanner-0.0.2.tar.gz` & `tmp/cerebrumscanner-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrumscanner-0.0.2.tar", last modified: Wed May 29 12:30:54 2024, max compression
+gzip compressed data, was "cerebrumscanner-0.0.3.tar", last modified: Wed May 29 14:31:38 2024, max compression
```

## Comparing `cerebrumscanner-0.0.2.tar` & `cerebrumscanner-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 12:30:54.259007 cerebrumscanner-0.0.2/
--rw-rw-rw-   0        0        0    35823 2023-09-10 19:28:05.000000 cerebrumscanner-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       24 2024-05-27 12:55:40.000000 cerebrumscanner-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    45364 2024-05-29 12:30:54.257999 cerebrumscanner-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3382 2024-02-21 06:32:05.000000 cerebrumscanner-0.0.2/README.md
--rw-rw-rw-   0        0        0      230 2024-05-28 10:23:21.000000 cerebrumscanner-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 12:30:54.260006 cerebrumscanner-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-05-29 12:30:00.000000 cerebrumscanner-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:30:54.221342 cerebrumscanner-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-29 12:30:54.233417 cerebrumscanner-0.0.2/src/cerebrumscanner/
--rw-rw-rw-   0        0        0       84 2024-05-28 12:15:56.000000 cerebrumscanner-0.0.2/src/cerebrumscanner/__init__.py
--rw-rw-rw-   0        0        0     5850 2024-05-28 12:05:08.000000 cerebrumscanner-0.0.2/src/cerebrumscanner/database_manager.py
--rw-rw-rw-   0        0        0     1379 2024-05-28 12:11:53.000000 cerebrumscanner-0.0.2/src/cerebrumscanner/image_processor.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:30:54.255495 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/
--rw-rw-rw-   0        0        0    45364 2024-05-29 12:30:54.000000 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2024-05-29 12:30:54.000000 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 12:30:54.000000 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-29 12:29:07.000000 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      192 2024-05-29 12:30:54.000000 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-29 12:30:54.000000 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 14:31:38.127573 cerebrumscanner-0.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-09-10 19:28:05.000000 cerebrumscanner-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       24 2024-05-27 12:55:40.000000 cerebrumscanner-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    45364 2024-05-29 14:31:38.125373 cerebrumscanner-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3382 2024-02-21 06:32:05.000000 cerebrumscanner-0.0.3/README.md
+-rw-rw-rw-   0        0        0      230 2024-05-28 10:23:21.000000 cerebrumscanner-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 14:31:38.127573 cerebrumscanner-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-05-29 14:29:38.000000 cerebrumscanner-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:31:38.077151 cerebrumscanner-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 14:31:38.088184 cerebrumscanner-0.0.3/src/cerebrumscanner/
+-rw-rw-rw-   0        0        0       84 2024-05-28 12:15:56.000000 cerebrumscanner-0.0.3/src/cerebrumscanner/__init__.py
+-rw-rw-rw-   0        0        0     5874 2024-05-29 14:31:26.000000 cerebrumscanner-0.0.3/src/cerebrumscanner/database_manager.py
+-rw-rw-rw-   0        0        0     1379 2024-05-28 12:11:53.000000 cerebrumscanner-0.0.3/src/cerebrumscanner/image_processor.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:31:38.122374 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/
+-rw-rw-rw-   0        0        0    45364 2024-05-29 14:31:37.000000 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2024-05-29 14:31:38.000000 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 14:31:37.000000 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-29 14:31:37.000000 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      192 2024-05-29 14:31:37.000000 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-29 14:31:37.000000 cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/top_level.txt
```

### Comparing `cerebrumscanner-0.0.2/LICENSE` & `cerebrumscanner-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.2/PKG-INFO` & `cerebrumscanner-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrumscanner
-Version: 0.0.2
+Version: 0.0.3
 Summary: Cerebrum Scanner Project
 Home-page: https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner
 Author: Nekodu Technology
 Author-email: info@nekodu.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `cerebrumscanner-0.0.2/README.md` & `cerebrumscanner-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.2/setup.py` & `cerebrumscanner-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ) as readme_file, open("requirements.txt", encoding="utf-8") as requirements_file:
     package_license = license_file.read()
     long_description = readme_file.read()
     install_requires = requirements_file.read().split("\n")[0:]
 
 setup(
     name="cerebrumscanner",
-    version="0.0.2",
+    version="0.0.3",
     url="https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner",
     license=package_license,
     author="Nekodu Technology",
     author_email="info@nekodu.com",
     description=(
         "Cerebrum Scanner Project"
     ),
```

### Comparing `cerebrumscanner-0.0.2/src/cerebrumscanner/database_manager.py` & `cerebrumscanner-0.0.3/src/cerebrumscanner/database_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
         try:
             self.client = pymongo.MongoClient(uri)
         except pymongo.errors.ConfigurationError:
             print(
                 "An Invalid URI host error was received. Is your Atlas host name correct in your connection string?"
             )
+            print(uri)
             sys.exit(1)
 
         # Set self.db as "cerebrum_scanner" database
         self.db = self.client[database_name]
         self.collection = self.db[collection_name]
         
         if not self.sample_document in list(self.collection.find()):
```

### Comparing `cerebrumscanner-0.0.2/src/cerebrumscanner/image_processor.py` & `cerebrumscanner-0.0.3/src/cerebrumscanner/image_processor.py`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/PKG-INFO` & `cerebrumscanner-0.0.3/src/cerebrumscanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrumscanner
-Version: 0.0.2
+Version: 0.0.3
 Summary: Cerebrum Scanner Project
 Home-page: https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner
 Author: Nekodu Technology
 Author-email: info@nekodu.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

