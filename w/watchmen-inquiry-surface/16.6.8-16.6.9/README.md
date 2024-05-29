# Comparing `tmp/watchmen_inquiry_surface-16.6.8.tar.gz` & `tmp/watchmen_inquiry_surface-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_surface-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_inquiry_surface-16.6.9.tar", max compression
```

## Comparing `watchmen_inquiry_surface-16.6.8.tar` & `watchmen_inquiry_surface-16.6.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.508594 watchmen_inquiry_surface-16.6.8/LICENSE
--rw-r--r--   0        0        0     1304 2024-01-08 07:58:02.512594 watchmen_inquiry_surface-16.6.8/pyproject.toml
--rw-r--r--   0        0        0       46 2024-01-08 07:58:02.512594 watchmen_inquiry_surface-16.6.8/src/watchmen_inquiry_surface/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.512594 watchmen_inquiry_surface-16.6.8/src/watchmen_inquiry_surface/data/__init__.py
--rw-r--r--   0        0        0    17842 2024-01-08 07:58:02.512594 watchmen_inquiry_surface-16.6.8/src/watchmen_inquiry_surface/data/data_router.py
--rw-r--r--   0        0        0      176 2024-01-08 07:58:02.512594 watchmen_inquiry_surface-16.6.8/src/watchmen_inquiry_surface/main.py
--rw-r--r--   0        0        0      478 2024-01-08 07:58:02.512594 watchmen_inquiry_surface-16.6.8/src/watchmen_inquiry_surface/settings.py
--rw-r--r--   0        0        0     1318 1970-01-01 00:00:00.000000 watchmen_inquiry_surface-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.243322 watchmen_inquiry_surface-16.6.9/LICENSE
+-rw-r--r--   0        0        0     1304 2024-02-01 01:32:37.243322 watchmen_inquiry_surface-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0       46 2024-02-01 01:32:37.243322 watchmen_inquiry_surface-16.6.9/src/watchmen_inquiry_surface/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.243322 watchmen_inquiry_surface-16.6.9/src/watchmen_inquiry_surface/data/__init__.py
+-rw-r--r--   0        0        0    17842 2024-02-01 01:32:37.243322 watchmen_inquiry_surface-16.6.9/src/watchmen_inquiry_surface/data/data_router.py
+-rw-r--r--   0        0        0      176 2024-02-01 01:32:37.243322 watchmen_inquiry_surface-16.6.9/src/watchmen_inquiry_surface/main.py
+-rw-r--r--   0        0        0      478 2024-02-01 01:32:37.243322 watchmen_inquiry_surface-16.6.9/src/watchmen_inquiry_surface/settings.py
+-rw-r--r--   0        0        0     1318 1970-01-01 00:00:00.000000 watchmen_inquiry_surface-16.6.9/PKG-INFO
```

### Comparing `watchmen_inquiry_surface-16.6.8/LICENSE` & `watchmen_inquiry_surface-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_surface-16.6.8/pyproject.toml` & `watchmen_inquiry_surface-16.6.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-inquiry-surface"
-version = "16.6.8"
+version = "16.6.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_inquiry_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-inquiry-kernel = "16.6.8"
-watchmen-rest = "16.6.8"
-watchmen-inquiry-trino = { version = "16.6.8", optional = true }
-watchmen-storage-mysql = { version = "16.6.8", optional = true }
-watchmen-storage-oracle = { version = "16.6.8", optional = true }
-watchmen-storage-mongodb = { version = "16.6.8", optional = true }
-watchmen-storage-mssql = { version = "16.6.8", optional = true }
-watchmen-storage-postgresql = { version = "16.6.8", optional = true }
-watchmen-storage-oss = { version = "16.6.8", optional = true }
-watchmen-storage-s3 = { version = "16.6.8", optional = true }
+watchmen-inquiry-kernel = "16.6.9"
+watchmen-rest = "16.6.9"
+watchmen-inquiry-trino = { version = "16.6.9", optional = true }
+watchmen-storage-mysql = { version = "16.6.9", optional = true }
+watchmen-storage-oracle = { version = "16.6.9", optional = true }
+watchmen-storage-mongodb = { version = "16.6.9", optional = true }
+watchmen-storage-mssql = { version = "16.6.9", optional = true }
+watchmen-storage-postgresql = { version = "16.6.9", optional = true }
+watchmen-storage-oss = { version = "16.6.9", optional = true }
+watchmen-storage-s3 = { version = "16.6.9", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 trino = ["watchmen-inquiry-trino"]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
```

### Comparing `watchmen_inquiry_surface-16.6.8/src/watchmen_inquiry_surface/data/data_router.py` & `watchmen_inquiry_surface-16.6.9/src/watchmen_inquiry_surface/data/data_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_surface-16.6.8/PKG-INFO` & `watchmen_inquiry_surface-16.6.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-surface
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,17 +16,17 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Provides-Extra: trino
-Requires-Dist: watchmen-inquiry-kernel (==16.6.8)
-Requires-Dist: watchmen-inquiry-trino (==16.6.8) ; extra == "trino"
-Requires-Dist: watchmen-rest (==16.6.8)
-Requires-Dist: watchmen-storage-mongodb (==16.6.8) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.6.8) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.6.8) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.6.8) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.6.8) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.6.8) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.6.8) ; extra == "s3"
+Requires-Dist: watchmen-inquiry-kernel (==16.6.9)
+Requires-Dist: watchmen-inquiry-trino (==16.6.9) ; extra == "trino"
+Requires-Dist: watchmen-rest (==16.6.9)
+Requires-Dist: watchmen-storage-mongodb (==16.6.9) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.6.9) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.6.9) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.6.9) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.6.9) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.6.9) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.6.9) ; extra == "s3"
```

