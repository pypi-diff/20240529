# Comparing `tmp/watchmen_storage_rds-16.6.8.tar.gz` & `tmp/watchmen_storage_rds-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_rds-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_storage_rds-16.6.9.tar", max compression
```

## Comparing `watchmen_storage_rds-16.6.8.tar` & `watchmen_storage_rds-16.6.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      455 2024-01-08 07:58:02.560594 watchmen_storage_rds-16.6.8/pyproject.toml
--rw-r--r--   0        0        0      643 2024-01-08 07:58:02.560594 watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/__init__.py
--rw-r--r--   0        0        0      652 2024-01-08 07:58:02.560594 watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/dbscript_builder.py
--rw-r--r--   0        0        0      518 2024-01-08 07:58:02.560594 watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/ext_types.py
--rw-r--r--   0        0        0      674 2024-01-08 07:58:02.560594 watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/settings.py
--rw-r--r--   0        0        0      941 2024-01-08 07:58:02.560594 watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/sort_build.py
--rw-r--r--   0        0        0    18405 2024-01-08 07:58:02.560594 watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/storage_rds.py
--rw-r--r--   0        0        0    24705 2024-01-08 07:58:02.560594 watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/table_defs.py
--rw-r--r--   0        0        0     2249 2024-01-08 07:58:02.560594 watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/table_defs_helper.py
--rw-r--r--   0        0        0      953 2024-01-08 07:58:02.560594 watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/table_reflector.py
--rw-r--r--   0        0        0    24388 2024-01-08 07:58:02.560594 watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/topic_data_storage_rds.py
--rw-r--r--   0        0        0     8191 2024-01-08 07:58:02.560594 watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/topic_table_generate.py
--rw-r--r--   0        0        0      916 2024-01-08 07:58:02.560594 watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/types.py
--rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 watchmen_storage_rds-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0      455 2024-02-01 01:32:37.291323 watchmen_storage_rds-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0      643 2024-02-01 01:32:37.291323 watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/__init__.py
+-rw-r--r--   0        0        0      652 2024-02-01 01:32:37.291323 watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/dbscript_builder.py
+-rw-r--r--   0        0        0      518 2024-02-01 01:32:37.291323 watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/ext_types.py
+-rw-r--r--   0        0        0      674 2024-02-01 01:32:37.291323 watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/settings.py
+-rw-r--r--   0        0        0      941 2024-02-01 01:32:37.291323 watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/sort_build.py
+-rw-r--r--   0        0        0    18405 2024-02-01 01:32:37.291323 watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/storage_rds.py
+-rw-r--r--   0        0        0    24705 2024-02-01 01:32:37.295323 watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/table_defs.py
+-rw-r--r--   0        0        0     2249 2024-02-01 01:32:37.295323 watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/table_defs_helper.py
+-rw-r--r--   0        0        0      953 2024-02-01 01:32:37.295323 watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/table_reflector.py
+-rw-r--r--   0        0        0    24388 2024-02-01 01:32:37.295323 watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/topic_data_storage_rds.py
+-rw-r--r--   0        0        0     8191 2024-02-01 01:32:37.295323 watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/topic_table_generate.py
+-rw-r--r--   0        0        0      916 2024-02-01 01:32:37.295323 watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/types.py
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 watchmen_storage_rds-16.6.9/PKG-INFO
```

### Comparing `watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/__init__.py` & `watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/dbscript_builder.py` & `watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/dbscript_builder.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/ext_types.py` & `watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/ext_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/settings.py` & `watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/sort_build.py` & `watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/sort_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/storage_rds.py` & `watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/storage_rds.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/table_defs.py` & `watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/table_defs.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/table_defs_helper.py` & `watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/table_defs_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/table_reflector.py` & `watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/table_reflector.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/topic_data_storage_rds.py` & `watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/topic_data_storage_rds.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/topic_table_generate.py` & `watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/topic_table_generate.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.6.8/src/watchmen_storage_rds/types.py` & `watchmen_storage_rds-16.6.9/src/watchmen_storage_rds/types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.6.8/PKG-INFO` & `watchmen_storage_rds-16.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-rds
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: SQLAlchemy (==1.4.35)
-Requires-Dist: watchmen-storage (==16.6.8)
+Requires-Dist: watchmen-storage (==16.6.9)
```

