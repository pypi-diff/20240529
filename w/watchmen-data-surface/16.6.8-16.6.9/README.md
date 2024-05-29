# Comparing `tmp/watchmen_data_surface-16.6.8.tar.gz` & `tmp/watchmen_data_surface-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_data_surface-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_data_surface-16.6.9.tar", max compression
```

## Comparing `watchmen_data_surface-16.6.8.tar` & `watchmen_data_surface-16.6.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.500594 watchmen_data_surface-16.6.8/LICENSE
--rw-r--r--   0        0        0     1195 2024-01-08 07:58:02.500594 watchmen_data_surface-16.6.8/pyproject.toml
--rw-r--r--   0        0        0       43 2024-01-08 07:58:02.500594 watchmen_data_surface-16.6.8/src/watchmen_data_surface/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.500594 watchmen_data_surface-16.6.8/src/watchmen_data_surface/cache/__init__.py
--rw-r--r--   0        0        0     2237 2024-01-08 07:58:02.500594 watchmen_data_surface-16.6.8/src/watchmen_data_surface/cache/cache_router.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.500594 watchmen_data_surface-16.6.8/src/watchmen_data_surface/data/__init__.py
--rw-r--r--   0        0        0     9814 2024-01-08 07:58:02.500594 watchmen_data_surface-16.6.8/src/watchmen_data_surface/data/topic_data_router.py
--rw-r--r--   0        0        0      240 2024-01-08 07:58:02.500594 watchmen_data_surface-16.6.8/src/watchmen_data_surface/main.py
--rw-r--r--   0        0        0      404 2024-01-08 07:58:02.500594 watchmen_data_surface-16.6.8/src/watchmen_data_surface/settings.py
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 watchmen_data_surface-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.235322 watchmen_data_surface-16.6.9/LICENSE
+-rw-r--r--   0        0        0     1195 2024-02-01 01:32:37.235322 watchmen_data_surface-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-02-01 01:32:37.235322 watchmen_data_surface-16.6.9/src/watchmen_data_surface/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.235322 watchmen_data_surface-16.6.9/src/watchmen_data_surface/cache/__init__.py
+-rw-r--r--   0        0        0     2237 2024-02-01 01:32:37.235322 watchmen_data_surface-16.6.9/src/watchmen_data_surface/cache/cache_router.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.235322 watchmen_data_surface-16.6.9/src/watchmen_data_surface/data/__init__.py
+-rw-r--r--   0        0        0     9814 2024-02-01 01:32:37.235322 watchmen_data_surface-16.6.9/src/watchmen_data_surface/data/topic_data_router.py
+-rw-r--r--   0        0        0      240 2024-02-01 01:32:37.235322 watchmen_data_surface-16.6.9/src/watchmen_data_surface/main.py
+-rw-r--r--   0        0        0      404 2024-02-01 01:32:37.235322 watchmen_data_surface-16.6.9/src/watchmen_data_surface/settings.py
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 watchmen_data_surface-16.6.9/PKG-INFO
```

### Comparing `watchmen_data_surface-16.6.8/LICENSE` & `watchmen_data_surface-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_data_surface-16.6.8/pyproject.toml` & `watchmen_data_surface-16.6.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "watchmen-data-surface"
-version = "16.6.8"
+version = "16.6.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_data_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-data-kernel = "16.6.8"
-watchmen-rest = "16.6.8"
-watchmen-storage-mysql = { version = "16.6.8", optional = true }
-watchmen-storage-oracle = { version = "16.6.8", optional = true }
-watchmen-storage-mongodb = { version = "16.6.8", optional = true }
-watchmen-storage-mssql = { version = "16.6.8", optional = true }
-watchmen-storage-postgresql = { version = "16.6.8", optional = true }
-watchmen-storage-oss = { version = "16.6.8", optional = true }
-watchmen-storage-s3 = { version = "16.6.8", optional = true }
+watchmen-data-kernel = "16.6.9"
+watchmen-rest = "16.6.9"
+watchmen-storage-mysql = { version = "16.6.9", optional = true }
+watchmen-storage-oracle = { version = "16.6.9", optional = true }
+watchmen-storage-mongodb = { version = "16.6.9", optional = true }
+watchmen-storage-mssql = { version = "16.6.9", optional = true }
+watchmen-storage-postgresql = { version = "16.6.9", optional = true }
+watchmen-storage-oss = { version = "16.6.9", optional = true }
+watchmen-storage-s3 = { version = "16.6.9", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_data_surface-16.6.8/src/watchmen_data_surface/cache/cache_router.py` & `watchmen_data_surface-16.6.9/src/watchmen_data_surface/cache/cache_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_surface-16.6.8/src/watchmen_data_surface/data/topic_data_router.py` & `watchmen_data_surface-16.6.9/src/watchmen_data_surface/data/topic_data_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_surface-16.6.8/PKG-INFO` & `watchmen_data_surface-16.6.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-data-surface
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,16 +15,16 @@
 Provides-Extra: mongodb
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
-Requires-Dist: watchmen-data-kernel (==16.6.8)
-Requires-Dist: watchmen-rest (==16.6.8)
-Requires-Dist: watchmen-storage-mongodb (==16.6.8) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.6.8) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.6.8) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.6.8) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.6.8) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.6.8) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.6.8) ; extra == "s3"
+Requires-Dist: watchmen-data-kernel (==16.6.9)
+Requires-Dist: watchmen-rest (==16.6.9)
+Requires-Dist: watchmen-storage-mongodb (==16.6.9) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.6.9) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.6.9) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.6.9) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.6.9) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.6.9) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.6.9) ; extra == "s3"
```

