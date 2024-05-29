# Comparing `tmp/prophecy-libs-1.9.3.tar.gz` & `tmp/prophecy-libs-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-libs-1.9.3.tar", last modified: Mon May 27 12:24:12 2024, max compression
+gzip compressed data, was "prophecy-libs-1.9.4.tar", last modified: Wed May 29 19:47:08 2024, max compression
```

## Comparing `prophecy-libs-1.9.3.tar` & `prophecy-libs-1.9.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-27 12:24:12.584447 prophecy-libs-1.9.3/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2024-05-27 12:24:12.584447 prophecy-libs-1.9.3/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.9.3/README.md
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-27 12:24:12.576447 prophecy-libs-1.9.3/prophecy/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.9.3/prophecy/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-27 12:24:12.576447 prophecy-libs-1.9.3/prophecy/config/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.9.3/prophecy/config/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     8391 2024-05-14 13:52:47.000000 prophecy-libs-1.9.3/prophecy/config/config_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4442 2023-06-09 08:12:50.000000 prophecy-libs-1.9.3/prophecy/config/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-27 12:24:12.576447 prophecy-libs-1.9.3/prophecy/libs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.9.3/prophecy/libs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1777 2024-05-20 10:14:39.000000 prophecy-libs-1.9.3/prophecy/libs/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-27 12:24:12.576447 prophecy-libs-1.9.3/prophecy/lookups/
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5483 2024-05-07 19:46:40.000000 prophecy-libs-1.9.3/prophecy/lookups/LookupsBase.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.9.3/prophecy/lookups/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.9.3/prophecy/random_data_creator.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-27 12:24:12.576447 prophecy-libs-1.9.3/prophecy/streaming/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.9.3/prophecy/streaming/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.9.3/prophecy/streaming/delta_lake_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-27 12:24:12.580447 prophecy-libs-1.9.3/prophecy/test/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.9.3/prophecy/test/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1944 2023-09-29 15:23:20.000000 prophecy-libs-1.9.3/prophecy/test/base_test_case.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     9645 2023-12-26 06:16:49.000000 prophecy-libs-1.9.3/prophecy/test/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-27 12:24:12.580447 prophecy-libs-1.9.3/prophecy/udfs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.9.3/prophecy/udfs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2306 2024-02-23 07:14:39.000000 prophecy-libs-1.9.3/prophecy/udfs/rest_api_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.9.3/prophecy/udfs/sample_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.9.3/prophecy/udfs/scala_udf_wrapper.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-27 12:24:12.580447 prophecy-libs-1.9.3/prophecy/utils/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      101 2024-05-20 10:20:20.000000 prophecy-libs-1.9.3/prophecy/utils/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1233 2024-05-27 12:24:11.000000 prophecy-libs-1.9.3/prophecy/utils/functions.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      303 2024-01-25 15:47:15.000000 prophecy-libs-1.9.3/prophecy/utils/gems_utils.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2824 2024-01-25 15:47:15.000000 prophecy-libs-1.9.3/prophecy/utils/metagem_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-27 12:24:12.584447 prophecy-libs-1.9.3/prophecy/utils/transpiler/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      143 2023-08-26 18:29:07.000000 prophecy-libs-1.9.3/prophecy/utils/transpiler/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-08-26 18:29:07.000000 prophecy-libs-1.9.3/prophecy/utils/transpiler/abi_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    22842 2023-08-30 12:14:40.000000 prophecy-libs-1.9.3/prophecy/utils/transpiler/abi_core_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4406 2024-01-25 15:47:15.000000 prophecy-libs-1.9.3/prophecy/utils/transpiler/abi_fcn_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     8740 2024-05-27 09:42:37.000000 prophecy-libs-1.9.3/prophecy/utils/transpiler/dataframe_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      692 2023-10-10 05:11:33.000000 prophecy-libs-1.9.3/prophecy/utils/transpiler/dml_schema.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     6399 2023-08-26 18:29:07.000000 prophecy-libs-1.9.3/prophecy/utils/transpiler/fixed_file_schema.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    39212 2024-05-27 09:42:37.000000 prophecy-libs-1.9.3/prophecy/utils/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-27 12:24:12.584447 prophecy-libs-1.9.3/prophecy_libs.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2024-05-27 12:24:12.000000 prophecy-libs-1.9.3/prophecy_libs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1190 2024-05-27 12:24:12.000000 prophecy-libs-1.9.3/prophecy_libs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2024-05-27 12:24:12.000000 prophecy-libs-1.9.3/prophecy_libs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.9.3/prophecy_libs.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2024-05-27 12:24:12.000000 prophecy-libs-1.9.3/prophecy_libs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2024-05-27 12:24:12.000000 prophecy-libs-1.9.3/prophecy_libs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2024-05-27 12:24:12.584447 prophecy-libs-1.9.3/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (114)      497 2024-05-27 12:24:11.000000 prophecy-libs-1.9.3/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-29 19:47:08.007949 prophecy-libs-1.9.4/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2024-05-29 19:47:08.007949 prophecy-libs-1.9.4/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.9.4/README.md
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-29 19:47:07.995948 prophecy-libs-1.9.4/prophecy/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.9.4/prophecy/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-29 19:47:07.999949 prophecy-libs-1.9.4/prophecy/config/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.9.4/prophecy/config/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     8391 2024-05-14 13:52:47.000000 prophecy-libs-1.9.4/prophecy/config/config_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     4442 2023-06-09 08:12:50.000000 prophecy-libs-1.9.4/prophecy/config/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-29 19:47:07.999949 prophecy-libs-1.9.4/prophecy/libs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.9.4/prophecy/libs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1777 2024-05-20 10:14:39.000000 prophecy-libs-1.9.4/prophecy/libs/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-29 19:47:07.999949 prophecy-libs-1.9.4/prophecy/lookups/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5483 2024-05-07 19:46:40.000000 prophecy-libs-1.9.4/prophecy/lookups/LookupsBase.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.9.4/prophecy/lookups/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.9.4/prophecy/random_data_creator.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-29 19:47:07.999949 prophecy-libs-1.9.4/prophecy/streaming/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.9.4/prophecy/streaming/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.9.4/prophecy/streaming/delta_lake_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-29 19:47:07.999949 prophecy-libs-1.9.4/prophecy/test/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.9.4/prophecy/test/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1944 2023-09-29 15:23:20.000000 prophecy-libs-1.9.4/prophecy/test/base_test_case.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     9645 2023-12-26 06:16:49.000000 prophecy-libs-1.9.4/prophecy/test/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-29 19:47:08.003949 prophecy-libs-1.9.4/prophecy/udfs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.9.4/prophecy/udfs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2306 2024-02-23 07:14:39.000000 prophecy-libs-1.9.4/prophecy/udfs/rest_api_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.9.4/prophecy/udfs/sample_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.9.4/prophecy/udfs/scala_udf_wrapper.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-29 19:47:08.003949 prophecy-libs-1.9.4/prophecy/utils/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      101 2024-05-20 10:20:20.000000 prophecy-libs-1.9.4/prophecy/utils/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1233 2024-05-27 12:24:11.000000 prophecy-libs-1.9.4/prophecy/utils/functions.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      303 2024-01-25 15:47:15.000000 prophecy-libs-1.9.4/prophecy/utils/gems_utils.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2824 2024-01-25 15:47:15.000000 prophecy-libs-1.9.4/prophecy/utils/metagem_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-29 19:47:08.007949 prophecy-libs-1.9.4/prophecy/utils/transpiler/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      143 2023-08-26 18:29:07.000000 prophecy-libs-1.9.4/prophecy/utils/transpiler/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-08-26 18:29:07.000000 prophecy-libs-1.9.4/prophecy/utils/transpiler/abi_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    22842 2023-08-30 12:14:40.000000 prophecy-libs-1.9.4/prophecy/utils/transpiler/abi_core_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     4406 2024-01-25 15:47:15.000000 prophecy-libs-1.9.4/prophecy/utils/transpiler/abi_fcn_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     8740 2024-05-27 09:42:37.000000 prophecy-libs-1.9.4/prophecy/utils/transpiler/dataframe_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      692 2023-10-10 05:11:33.000000 prophecy-libs-1.9.4/prophecy/utils/transpiler/dml_schema.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6399 2023-08-26 18:29:07.000000 prophecy-libs-1.9.4/prophecy/utils/transpiler/fixed_file_schema.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    39269 2024-05-29 19:47:06.000000 prophecy-libs-1.9.4/prophecy/utils/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-29 19:47:08.007949 prophecy-libs-1.9.4/prophecy_libs.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2024-05-29 19:47:07.000000 prophecy-libs-1.9.4/prophecy_libs.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1190 2024-05-29 19:47:07.000000 prophecy-libs-1.9.4/prophecy_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2024-05-29 19:47:07.000000 prophecy-libs-1.9.4/prophecy_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.9.4/prophecy_libs.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2024-05-29 19:47:07.000000 prophecy-libs-1.9.4/prophecy_libs.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2024-05-29 19:47:07.000000 prophecy-libs-1.9.4/prophecy_libs.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2024-05-29 19:47:08.007949 prophecy-libs-1.9.4/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      497 2024-05-29 19:47:06.000000 prophecy-libs-1.9.4/setup.py
```

### Comparing `prophecy-libs-1.9.3/prophecy/config/config_base.py` & `prophecy-libs-1.9.4/prophecy/config/config_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/config/utils.py` & `prophecy-libs-1.9.4/prophecy/config/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/libs/utils.py` & `prophecy-libs-1.9.4/prophecy/libs/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/lookups/LookupsBase.py` & `prophecy-libs-1.9.4/prophecy/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/random_data_creator.py` & `prophecy-libs-1.9.4/prophecy/random_data_creator.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/streaming/delta_lake_utils.py` & `prophecy-libs-1.9.4/prophecy/streaming/delta_lake_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/test/base_test_case.py` & `prophecy-libs-1.9.4/prophecy/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/test/utils.py` & `prophecy-libs-1.9.4/prophecy/test/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/udfs/rest_api_udf.py` & `prophecy-libs-1.9.4/prophecy/udfs/rest_api_udf.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/udfs/scala_udf_wrapper.py` & `prophecy-libs-1.9.4/prophecy/udfs/scala_udf_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/utils/functions.py` & `prophecy-libs-1.9.4/prophecy/utils/functions.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/utils/metagem_utils.py` & `prophecy-libs-1.9.4/prophecy/utils/metagem_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/utils/transpiler/abi_base.py` & `prophecy-libs-1.9.4/prophecy/utils/transpiler/abi_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/utils/transpiler/abi_core_fcns.py` & `prophecy-libs-1.9.4/prophecy/utils/transpiler/abi_core_fcns.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/utils/transpiler/abi_fcn_wrapper.py` & `prophecy-libs-1.9.4/prophecy/utils/transpiler/abi_fcn_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/utils/transpiler/dataframe_fcns.py` & `prophecy-libs-1.9.4/prophecy/utils/transpiler/dataframe_fcns.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/utils/transpiler/dml_schema.py` & `prophecy-libs-1.9.4/prophecy/utils/transpiler/dml_schema.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/utils/transpiler/fixed_file_schema.py` & `prophecy-libs-1.9.4/prophecy/utils/transpiler/fixed_file_schema.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.9.3/prophecy/utils/utils.py` & `prophecy-libs-1.9.4/prophecy/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,19 +304,21 @@
             return getattr(self.dataframe, item)
 
 
 class InterimConfig:
     def __init__(self):
         self.isInitialized = False
         self.interimOutput = None
+        self.session = None
 
     def initialize(self, spark: SparkSession, sessionForInteractive: str = ""):
         from py4j.java_gateway import JavaPackage
 
         self.isInitialized = True
+        self.session = sessionForInteractive
         # It's `JavaClass` when scala-libs are present, and `JavaPackage` when they are not present.
         if (
                 type(spark.sparkContext._jvm.org.apache.spark.sql.InterimOutputHive2)
                 == JavaPackage
         ):
             raise Exception(
                 "Scala Prophecy Libs jar was not found in the classpath. Please add Scala Prophecy Libs and retry the operation"
@@ -907,16 +909,16 @@
     return spark.sparkContext._jvm.org.apache.spark.sql.ProphecySparkSession.getProcessFromGem(
         spark._jsparkSession, gemName, userSession)
 
 
 def instrument(function):
     def inner_wrapper(spark, *args, **kwargs):
         global interimConfig
-        if interimConfig.interimOutput:
-            user_session = interimConfig.interimOutput.session()
+        if interimConfig.isInitialized:
+            user_session = interimConfig.session
         else:
             user_session = ""
         start_time = currentTimeString()
         state = TaskState.LAUNCHING
         gem_name = extractHierarchicalGemName(inspect.stack(), function)
         process_id = getProcessFromGem(spark, gem_name, user_session)
         sendGemProgressEvent(spark, user_session, process_id, state, start_time)
```

### Comparing `prophecy-libs-1.9.3/prophecy_libs.egg-info/SOURCES.txt` & `prophecy-libs-1.9.4/prophecy_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

