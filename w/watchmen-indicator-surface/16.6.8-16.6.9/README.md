# Comparing `tmp/watchmen_indicator_surface-16.6.8.tar.gz` & `tmp/watchmen_indicator_surface-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_indicator_surface-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_indicator_surface-16.6.9.tar", max compression
```

## Comparing `watchmen_indicator_surface-16.6.8.tar` & `watchmen_indicator_surface-16.6.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1025 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/pyproject.toml
--rw-r--r--   0        0        0       48 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/data/__init__.py
--rw-r--r--   0        0        0     1662 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/data/convergence_data_router.py
--rw-r--r--   0        0        0    12505 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/data/objective_data_router.py
--rw-r--r--   0        0        0      653 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/main.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/__init__.py
--rw-r--r--   0        0        0     6015 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py
--rw-r--r--   0        0        0     7181 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/bucket_router.py
--rw-r--r--   0        0        0    13226 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/convergence_router.py
--rw-r--r--   0        0        0     8363 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/derived_objective_report_router.py
--rw-r--r--   0        0        0     9156 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/derived_objective_router.py
--rw-r--r--   0        0        0     7904 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/indicator_router.py
--rw-r--r--   0        0        0     2953 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/objective_report_router.py
--rw-r--r--   0        0        0    12730 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/objective_router.py
--rw-r--r--   0        0        0     5673 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/subject_router.py
--rw-r--r--   0        0        0      408 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/settings.py
--rw-r--r--   0        0        0       80 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/util/__init__.py
--rw-r--r--   0        0        0     2135 2024-01-08 07:58:02.508594 watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/util/trans.py
--rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 watchmen_indicator_surface-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1025 2024-02-01 01:32:37.239323 watchmen_indicator_surface-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-02-01 01:32:37.239323 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/data/__init__.py
+-rw-r--r--   0        0        0     1662 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/data/convergence_data_router.py
+-rw-r--r--   0        0        0    12505 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/data/objective_data_router.py
+-rw-r--r--   0        0        0      653 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/main.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/__init__.py
+-rw-r--r--   0        0        0     6015 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py
+-rw-r--r--   0        0        0     7181 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/bucket_router.py
+-rw-r--r--   0        0        0    13226 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/convergence_router.py
+-rw-r--r--   0        0        0     8363 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/derived_objective_report_router.py
+-rw-r--r--   0        0        0     9156 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/derived_objective_router.py
+-rw-r--r--   0        0        0     7904 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/indicator_router.py
+-rw-r--r--   0        0        0     2953 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/objective_report_router.py
+-rw-r--r--   0        0        0    12730 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/objective_router.py
+-rw-r--r--   0        0        0     5673 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/subject_router.py
+-rw-r--r--   0        0        0      408 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/settings.py
+-rw-r--r--   0        0        0       80 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/util/__init__.py
+-rw-r--r--   0        0        0     2135 2024-02-01 01:32:37.243322 watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/util/trans.py
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 watchmen_indicator_surface-16.6.9/PKG-INFO
```

### Comparing `watchmen_indicator_surface-16.6.8/pyproject.toml` & `watchmen_indicator_surface-16.6.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "watchmen-indicator-surface"
-version = "16.6.8"
+version = "16.6.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_indicator_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-indicator-kernel = "16.6.8"
-watchmen-rest = "16.6.8"
-watchmen-storage-mysql = { version = "16.6.8", optional = true }
-watchmen-storage-oracle = { version = "16.6.8", optional = true }
-watchmen-storage-mongodb = { version = "16.6.8", optional = true }
-watchmen-storage-mssql = { version = "16.6.8", optional = true }
-watchmen-storage-postgresql = { version = "16.6.8", optional = true }
+watchmen-indicator-kernel = "16.6.9"
+watchmen-rest = "16.6.9"
+watchmen-storage-mysql = { version = "16.6.9", optional = true }
+watchmen-storage-oracle = { version = "16.6.9", optional = true }
+watchmen-storage-mongodb = { version = "16.6.9", optional = true }
+watchmen-storage-mssql = { version = "16.6.9", optional = true }
+watchmen-storage-postgresql = { version = "16.6.9", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/data/convergence_data_router.py` & `watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/data/convergence_data_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/data/objective_data_router.py` & `watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/data/objective_data_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/main.py` & `watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/main.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py` & `watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/bucket_router.py` & `watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/bucket_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/convergence_router.py` & `watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/convergence_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/derived_objective_report_router.py` & `watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/derived_objective_report_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/derived_objective_router.py` & `watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/derived_objective_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/indicator_router.py` & `watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/indicator_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/objective_report_router.py` & `watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/objective_report_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/objective_router.py` & `watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/objective_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/meta/subject_router.py` & `watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/meta/subject_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.6.8/src/watchmen_indicator_surface/util/trans.py` & `watchmen_indicator_surface-16.6.9/src/watchmen_indicator_surface/util/trans.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.6.8/PKG-INFO` & `watchmen_indicator_surface-16.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-indicator-surface
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: mongodb
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: postgresql
-Requires-Dist: watchmen-indicator-kernel (==16.6.8)
-Requires-Dist: watchmen-rest (==16.6.8)
-Requires-Dist: watchmen-storage-mongodb (==16.6.8) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.6.8) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.6.8) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.6.8) ; extra == "oracle"
-Requires-Dist: watchmen-storage-postgresql (==16.6.8) ; extra == "postgresql"
+Requires-Dist: watchmen-indicator-kernel (==16.6.9)
+Requires-Dist: watchmen-rest (==16.6.9)
+Requires-Dist: watchmen-storage-mongodb (==16.6.9) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.6.9) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.6.9) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.6.9) ; extra == "oracle"
+Requires-Dist: watchmen-storage-postgresql (==16.6.9) ; extra == "postgresql"
```

