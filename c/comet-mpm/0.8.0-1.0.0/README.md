# Comparing `tmp/comet_mpm-0.8.0.tar.gz` & `tmp/comet_mpm-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comet_mpm-0.8.0.tar", last modified: Wed Apr 10 15:10:16 2024, max compression
+gzip compressed data, was "comet_mpm-1.0.0.tar", last modified: Wed May 29 09:27:15 2024, max compression
```

## Comparing `comet_mpm-0.8.0.tar` & `comet_mpm-1.0.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.177246 comet_mpm-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/PACKAGE.md
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-10 15:10:16.177246 comet_mpm-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:10:16.177246 comet_mpm-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.165246 comet_mpm-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm/_json/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/_json/numpy_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm/api_key/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/api_key/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/api_key/base64_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/api_key/comet_api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/aws_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/aws_lambda/lambda_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/batch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    12877 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/comet_mpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/connection_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/data_series.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm/events/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/events/base_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/events/events_from_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/events/label_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/events/prediction_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/logging_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/optional_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm/sender/
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/sender/asyncio_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/sender/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/sender/thread_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/settings_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-10 15:10:16.000000 comet_mpm-0.8.0/src/comet_mpm.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.310628 comet_mpm-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/PACKAGE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-29 09:27:15.310628 comet_mpm-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:27:15.310628 comet_mpm-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.298628 comet_mpm-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm/_json/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/_json/numpy_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm/api_key/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/api_key/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/api_key/base64_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/api_key/comet_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/aws_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/aws_lambda/lambda_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/batch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20451 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/comet_mpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/connection_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/data_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/dataset_upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/events/base_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/events/events_from_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/events/label_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/events/prediction_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/logging_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/optional_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm/sender/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/sender/asyncio_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/sender/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/sender/thread_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/server_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/settings_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-29 09:27:15.000000 comet_mpm-1.0.0/src/comet_mpm.egg-info/SOURCES.txt
```

### Comparing `comet_mpm-0.8.0/MANIFEST.in` & `comet_mpm-1.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/PKG-INFO` & `comet_mpm-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_mpm
-Version: 0.8.0
+Version: 1.0.0
 Summary: Comet MPM SDK
 Home-page: https://www.comet.ml
 Author: Comet ML Inc.
 Author-email: mail@comet.ml
 License: Proprietary
 Keywords: comet_mpm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `comet_mpm-0.8.0/setup.py` & `comet_mpm-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,11 +52,11 @@
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="comet_mpm",
     name="comet_mpm",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://www.comet.ml",
-    version="0.8.0",
+    version="1.0.0",
     zip_safe=False,
     license="Proprietary",
 )
```

### Comparing `comet_mpm-0.8.0/src/comet_mpm/__init__.py` & `comet_mpm-1.0.0/src/comet_mpm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 #  Copyright (C) 2021 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 __author__ = """Comet ML Inc."""
 __email__ = "mail@comet.ml"
-__version__ = "0.8.0"
+__version__ = "1.0.0"
 __all__ = ["CometMPM"]
 
 from ._logging import _setup_comet_mpm_logging
 from .comet_mpm import CometMPM
 
 _setup_comet_mpm_logging()
```

### Comparing `comet_mpm-0.8.0/src/comet_mpm/_json/__init__.py` & `comet_mpm-1.0.0/src/comet_mpm/_json/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/_json/numpy_encoder.py` & `comet_mpm-1.0.0/src/comet_mpm/_json/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/_logging.py` & `comet_mpm-1.0.0/src/comet_mpm/_logging.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/api_key/__init__.py` & `comet_mpm-1.0.0/src/comet_mpm/api_key/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/api_key/base64_helper.py` & `comet_mpm-1.0.0/src/comet_mpm/api_key/base64_helper.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/api_key/comet_api_key.py` & `comet_mpm-1.0.0/src/comet_mpm/api_key/comet_api_key.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/aws_lambda/__init__.py` & `comet_mpm-1.0.0/src/comet_mpm/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/aws_lambda/lambda_helpers.py` & `comet_mpm-1.0.0/src/comet_mpm/aws_lambda/lambda_helpers.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/cli.py` & `comet_mpm-1.0.0/src/comet_mpm/cli.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/constants.py` & `comet_mpm-1.0.0/src/comet_mpm/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 EVENT_PREDICTION_ID = "predictionId"
 EVENT_TIMESTAMP = "timestamp"
 EVENT_FEATURES = "features"
 EVENT_PREDICTION = "prediction"
+LABELS = "labels"
 EVENT_PREDICTION_VALUE = "value"
 EVENT_PREDICTION_PROBABILITY = "probability"
 EVENT_WORKSPACE_NAME = "workspaceName"
 EVENT_MODEL_NAME = "modelName"
 EVENT_MODEL_VERSION = "modelVersion"
```

### Comparing `comet_mpm-0.8.0/src/comet_mpm/data_series.py` & `comet_mpm-1.0.0/src/comet_mpm/data_series.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/environment.py` & `comet_mpm-1.0.0/src/comet_mpm/environment.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/events/__init__.py` & `comet_mpm-1.0.0/src/comet_mpm/events/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/events/base_event.py` & `comet_mpm-1.0.0/src/comet_mpm/events/base_event.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/events/events_from_dataframe.py` & `comet_mpm-1.0.0/src/comet_mpm/events/events_from_dataframe.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,27 +26,29 @@
     model_version: str,
     dataframe,
     prediction_id_column: str,
     feature_columns: Optional[List[str]] = None,
     output_features_columns: Optional[List[str]] = None,
     output_value_column: Optional[str] = None,
     output_probability_column: Optional[str] = None,
+    labels_columns: Optional[List[str]] = None,
     timestamp_column: Optional[str] = None,
 ):
     return (
         _event(
             workspace=workspace,
             model_name=model_name,
             model_version=model_version,
             row=row,
             prediction_id_column=prediction_id_column,
             feature_columns=feature_columns,
             output_features_columns=output_features_columns,
             output_value_column=output_value_column,
             output_probability_column=output_probability_column,
+            labels_columns=labels_columns,
             timestamp_column=timestamp_column,
         )
         for row in dataframe.to_dict(orient="records")
     )
 
 
 def _event(  # type: ignore[no-untyped-def]
@@ -55,14 +57,15 @@
     model_version: str,
     row,
     prediction_id_column,
     feature_columns,
     output_features_columns,
     output_value_column,
     output_probability_column,
+    labels_columns: Optional[List[str]] = None,
     timestamp_column: Optional[str] = None,
 ) -> PredictionEvent:
     prediction_id = str(row[prediction_id_column])
     input_features = None
     if feature_columns is not None:
         input_features = {key: row[key] for key in feature_columns}
 
@@ -77,25 +80,30 @@
     output_features = None
     if output_features_columns is not None:
         output_features = {key: row[key] for key in output_features_columns}
     output_features = _handle_dataframe_output_features(
         output_value, output_probability, output_features
     )
 
+    labels = None
+    if labels_columns is not None:
+        labels = {key: row[key] for key in labels_columns}
+
     timestamp = None
     if timestamp_column is not None:
         timestamp = row[timestamp_column]
 
     return PredictionEvent(
         workspace=workspace,
         model_name=model_name,
         model_version=model_version,
         prediction_id=prediction_id,
         input_features=input_features,
         output_features=output_features,
+        labels=labels,
         timestamp=timestamp,
     )
 
 
 def _handle_dataframe_output_features(
     output_value: Any,
     output_probability: Any,
```

### Comparing `comet_mpm-0.8.0/src/comet_mpm/events/label_event.py` & `comet_mpm-1.0.0/src/comet_mpm/events/label_event.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 #  \____\___/|_| |_| |_|\___|\__(_)_| |_| |_|_|
 #
 #  Sign up for free at http://www.comet.ml
 #  Copyright (C) 2021-2023 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
-from typing import Any, Dict
 
-from comet_mpm.constants import EVENT_PREDICTION_VALUE
+from typing import Any, Dict, Optional
+
+from comet_mpm.constants import LABELS
 from comet_mpm.events.base_event import BaseEvent
 
 
-class LabelEvent(BaseEvent):
+class LabelsEvent(BaseEvent):
     """
     This class represents a single ground truth label.
     Args:
         workspace: The project workspace.
         model_name: The name of model
         model_version: The version of model
         prediction_id: The unique prediction ID, could be provided by the
@@ -32,19 +33,21 @@
 
     def __init__(
         self,
         workspace: str,
         model_name: str,
         model_version: str,
         prediction_id: str,
-        label: Any,
+        labels: Dict[str, Any],
+        timestamp: Optional[float] = None,
     ):
-        super(LabelEvent, self).__init__(
+        super(LabelsEvent, self).__init__(
             workspace=workspace,
             model_name=model_name,
             model_version=model_version,
             prediction_id=prediction_id,
+            timestamp=timestamp,
         )
-        self.label = label
+        self.labels = labels
 
     def _get_event_dict(self) -> Dict[str, Any]:
-        return {EVENT_PREDICTION_VALUE: self.label}
+        return {LABELS: self.labels}
```

### Comparing `comet_mpm-0.8.0/src/comet_mpm/events/prediction_event.py` & `comet_mpm-1.0.0/src/comet_mpm/events/prediction_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  Copyright (C) 2021 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 from typing import Any, Dict, Optional
 
-from comet_mpm.constants import EVENT_FEATURES, EVENT_PREDICTION
+from comet_mpm.constants import EVENT_FEATURES, EVENT_PREDICTION, LABELS
 from comet_mpm.events.base_event import BaseEvent
 
 
 class PredictionEvent(BaseEvent):
     """
     This class represents a single prediction event. Events are identified by the
     mandatory prediction_id parameter. Many events can have the same
@@ -42,28 +42,33 @@
         self,
         workspace: str,
         model_name: str,
         model_version: str,
         prediction_id: str,
         input_features: Optional[Dict[str, Any]] = None,
         output_features: Optional[Dict[str, Any]] = None,
+        labels: Optional[Dict[str, Any]] = None,
         timestamp: Optional[float] = None,
     ):
         super(PredictionEvent, self).__init__(
             workspace=workspace,
             model_name=model_name,
             model_version=model_version,
             prediction_id=prediction_id,
             timestamp=timestamp,
         )
         self.input_features = input_features
         self.output_features = output_features
+        self.labels = labels
 
     def _get_event_dict(self) -> Dict[str, Any]:
         event: Dict[str, Any] = {}
         if self.input_features is not None:
             event[EVENT_FEATURES] = self.input_features
 
         if self.output_features:
             event[EVENT_PREDICTION] = self.output_features
 
+        if self.labels:
+            event[LABELS] = self.labels
+
         return event
```

### Comparing `comet_mpm-0.8.0/src/comet_mpm/logging_messages.py` & `comet_mpm-1.0.0/src/comet_mpm/logging_messages.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,24 +8,34 @@
 #
 #  Sign up for free at http://www.comet.ml
 #  Copyright (C) 2021 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
+BACKEND_IS_NOT_AVAILABLE_ERROR = "Comet Production Monitoring don't seems to be installed in your installation. Please contact your Comet Admin."
+
+BACKEND_500_ERROR = "Comet Production Monitoring isn't working as expected, Please contact your Comet admin."
+
 BATCH_SENDING_ERROR = "Error sending batch data to the backend"
 
+UPLOAD_CSV_DATASET_ERROR = "Error on uploading csv dataset"
+
 BATCH_SENDING_EXCEPTION = "Unknown exception happened when sending data to the backend"
 
 LABEL_EVENT_SEND_ERROR = "Error sending label to the backend"
 
 GEVENT_NOT_SUPPORTED = (
     "Using the MPM SDK with gevent is not officially supported, data loss might occurs"
 )
 
+ASYNCIO_SENDER_NOT_CONNECTED_ERROR = (
+    "You need to call CometMPM.connect before sending events with CometMPM.log_event"
+)
+
 ASYNCIO_SENDER_HARD_SHUTDOWN = "There are still some data in-flight and might be missing. Make sure to call CometMPM.join() manually to guarantee that all data has been sent to the Backend"
 
 ERROR_QUANTILES_LIST_EMPTY = (
     "Error cannot compute distribution summary because the quantiles list is empty."
 )
 ERROR_QUANTILES_INVALID_VALUE = (
     "The quantile must be within [0,1]. The current min value %f and max %f"
@@ -47,14 +57,18 @@
 
 MPM_ALREADY_CLOSED_LOG_DATA_WARNING = "This MPM instance has already been closed. Create a new instance to log additional data."
 
 MPM_IN_AWS_LAMBDA_NEEDS_END = "As you are running in a Lambda function, you will need to call 'mpm.end()' when finished to ensure all data is logged before exiting."
 
 MPM_JOIN_DEPRECATED_WARNING = "MPM.join is deprecated, use MPM.end instead."
 
+MPM_LABEL_DEPRECATED_WARNING = (
+    "label parameter deprecated, use labels parameter instead."
+)
+
 PARSE_API_KEY_EMPTY_KEY = "Can not parse empty Comet API key"
 
 PARSE_API_KEY_EMPTY_EXPECTED_ATTRIBUTES = (
     "Expected attributes not found in the Comet API key: %r"
 )
 
 PARSE_API_KEY_TOO_MANY_PARTS = "Too many parts (%d) found in the Comet API key: %r"
```

### Comparing `comet_mpm-0.8.0/src/comet_mpm/optional_update.py` & `comet_mpm-1.0.0/src/comet_mpm/optional_update.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/sender/__init__.py` & `comet_mpm-1.0.0/src/comet_mpm/sender/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 #  permission of Comet ML Inc.
 # *******************************************************
 
 import logging
 import sys
 
 from ..logging_messages import GEVENT_NOT_SUPPORTED
+from ..server_address import ServerAddress
 from .asyncio_sender import get_asyncio_sender
 from .base import BaseSender
 from .thread_sender import get_thread_sender
 
 LOGGER = logging.getLogger(__name__)
 
 
 def get_sender(
     api_key: str,
-    server_address: str,
+    server_address: ServerAddress,
     max_batch_size: int,
     max_batch_time: int,
     batch_sending_timeout: int,
     asyncio: bool = False,
 ) -> "BaseSender":
 
     if "gevent" in sys.modules:
```

### Comparing `comet_mpm-0.8.0/src/comet_mpm/sender/asyncio_sender.py` & `comet_mpm-1.0.0/src/comet_mpm/sender/asyncio_sender.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,34 +14,31 @@
 
 import asyncio
 import logging
 from typing import Any, Optional, Tuple
 
 import aiohttp
 
-from ..batch_utils import Batch
-from ..connection import send_asyncio_batch_requests
-from ..events.label_event import LabelEvent
-from ..events.prediction_event import PredictionEvent
+from ..batch_utils import Batch, split_batch
+from ..connection import send_asyncio_batch_requests, send_asyncio_is_alive
 from ..exceptions import AsyncioSenderNoConnected
 from ..logging_messages import (
     ASYNCIO_SENDER_HARD_SHUTDOWN,
     BATCH_SENDING_EXCEPTION,
-    LABEL_EVENT_SEND_ERROR,
     MPM_ALREADY_CLOSED_LOG_DATA_WARNING,
-    UNEXPECTED_EVENT_TYPE,
 )
-from .base import CLOSE_MESSAGE, BaseSender, batch_endpoint_url, labels_endpoint_url
+from ..server_address import ServerAddress
+from .base import CLOSE_MESSAGE, BaseSender
 
 LOGGER = logging.getLogger(__name__)
 
 
 def get_asyncio_sender(
     api_key: str,
-    server_address: str,
+    server_address: ServerAddress,
     max_batch_size: int,
     max_batch_time: int,
     batch_sending_timeout: int,
 ) -> "AsyncioSender":
     sender = AsyncioSender(
         api_key=api_key,
         server_address=server_address,
@@ -53,15 +50,15 @@
     return sender
 
 
 class AsyncioBackgroundSender:
     def __init__(
         self,
         api_key: str,
-        server_address: str,
+        server_address: ServerAddress,
         queue: "asyncio.Queue[Any]",
         max_batch_size: int,
         max_batch_time: int,
         batch_sending_timeout: int,
     ):
         """A background coroutine that reads from the queue, add the items to the batch and sends
         them whenever the batch is ready to be sent. Can only be created only when an event loop is running.
@@ -73,16 +70,16 @@
         self.max_batch_time = max_batch_time
         self.batch = Batch(max_batch_size, self.max_batch_time)
         self.batch_sending_timeout = batch_sending_timeout
 
         self.stop_processing = False
 
         # Pre-compute URLs
-        self.batch_endpoint = batch_endpoint_url(self.server_address)
-        self.labels_endpoint = labels_endpoint_url(self.server_address)
+        self.batch_endpoint = self.server_address.batch_endpoint_url()
+        self.labels_endpoint = self.server_address.batch_endpoint_url()
 
     async def run(self) -> None:
         while True:
             stop = await self._loop()
 
             if stop is True:
                 break
@@ -97,96 +94,99 @@
             if data is None:
                 return False
 
             if data is CLOSE_MESSAGE:
                 self.stop_processing = True
                 return True
 
-            if isinstance(data, PredictionEvent):
-                self._process_prediction_event(data)
-            elif isinstance(data, LabelEvent):
-                await self._process_label_event(data)
-            else:
-                LOGGER.error(UNEXPECTED_EVENT_TYPE, data)
+            self.batch.append(data)
         except asyncio.TimeoutError:
             pass
 
         await self._check_batch_sending()
 
         return False
 
-    async def _process_label_event(self, event: LabelEvent) -> None:
-        try:
-            await send_asyncio_batch_requests(
-                session=self.session,
-                url_endpoint=self.labels_endpoint,
-                api_key=self.api_key,
-                batch_sending_timeout=self.batch_sending_timeout,
-                batch=event.create_event_dict(),
-            )
-        except Exception:
-            LOGGER.error(LABEL_EVENT_SEND_ERROR, exc_info=True)
+    async def _send_batch(self, batch_to_send: Any) -> None:
+        async with aiohttp.ClientSession() as session:
+            predictions_batch, labels_batch = split_batch(batch_to_send)
 
-    def _process_prediction_event(self, event: PredictionEvent) -> None:
-        to_send = event.create_event_dict()
-        self.batch.append(to_send)
+            if predictions_batch:
+                await send_asyncio_batch_requests(
+                    session=session,
+                    url_endpoint=self.batch_endpoint,
+                    api_key=self.api_key,
+                    batch_sending_timeout=self.batch_sending_timeout,
+                    batch=predictions_batch,
+                )
 
-    async def _send_batch(self, batch: Any) -> None:
-        async with aiohttp.ClientSession() as session:
-            await send_asyncio_batch_requests(
-                session=session,
-                url_endpoint=self.batch_endpoint,
-                api_key=self.api_key,
-                batch_sending_timeout=self.batch_sending_timeout,
-                batch=batch,
-            )
+            if labels_batch:
+                await send_asyncio_batch_requests(
+                    session=session,
+                    url_endpoint=self.labels_endpoint,
+                    api_key=self.api_key,
+                    batch_sending_timeout=self.batch_sending_timeout,
+                    batch=labels_batch,
+                )
 
     async def _check_batch_sending(self) -> None:
         # This should only be called by the background sender coroutine, if not the batch could
         # become corrupted as its access not protected by a lock
         try:
             if self.batch.should_be_uploaded(self.stop_processing):
-                batch = self.batch.get_and_clear()
+                batch_to_send = self.batch.get_and_clear()
 
-                await send_asyncio_batch_requests(
-                    session=self.session,
-                    url_endpoint=self.batch_endpoint,
-                    api_key=self.api_key,
-                    batch_sending_timeout=self.batch_sending_timeout,
-                    batch=batch,
-                )
+                predictions_batch, labels_batch = split_batch(batch_to_send)
+
+                if predictions_batch:
+                    await send_asyncio_batch_requests(
+                        session=self.session,
+                        url_endpoint=self.batch_endpoint,
+                        api_key=self.api_key,
+                        batch_sending_timeout=self.batch_sending_timeout,
+                        batch=predictions_batch,
+                    )
+
+                if labels_batch:
+                    await send_asyncio_batch_requests(
+                        session=self.session,
+                        url_endpoint=self.labels_endpoint,
+                        api_key=self.api_key,
+                        batch_sending_timeout=self.batch_sending_timeout,
+                        batch=labels_batch,
+                    )
         except Exception:
             LOGGER.error(BATCH_SENDING_EXCEPTION, exc_info=True)
 
     def close(self, timeout: int = 10) -> None:
         """Force the AsyncioBackgroundSender to stop processing messages"""
         #
         self.stop_processing = True
 
         async def flush_queue() -> None:
             while True:
                 try:
                     data = self.queue.get_nowait()
                     if data is not None and data is not CLOSE_MESSAGE:
-                        self._process_prediction_event(data)
+                        self.batch.append(data)
                 except asyncio.QueueEmpty:
                     break
 
             batch = self.batch.get_and_clear()
             await asyncio.wait_for(self._send_batch(batch), timeout)
             await self.session.close()
 
         asyncio.run(flush_queue())
 
 
 class AsyncioSender(BaseSender):
     def __init__(
         self,
         api_key: str,
-        server_address: str,
+        server_address: ServerAddress,
         max_batch_size: int,
         max_batch_time: int,
         batch_sending_timeout: int,
     ) -> None:
         self.sender_queue: Optional["asyncio.Queue[Any]"] = None
         # We need to wait for the asyncio event loop to be created
         self.background_sender: Optional[AsyncioBackgroundSender] = None
@@ -196,15 +196,15 @@
 
         self.api_key = api_key
         self.server_address = server_address
         self.max_batch_time = max_batch_time
         self.max_batch_size = max_batch_size
         self.batch_sending_timeout = batch_sending_timeout
 
-    def connect(self) -> None:
+    async def connect(self) -> None:
         if self.sender_queue is None:
             sender_queue: "asyncio.Queue[Any]" = asyncio.Queue()
             self.sender_queue = sender_queue
             self.background_sender = AsyncioBackgroundSender(
                 api_key=self.api_key,
                 server_address=self.server_address,
                 queue=self.sender_queue,
@@ -217,14 +217,24 @@
         if self.background_task is None:
             assert self.background_sender is not None
             self.background_task = asyncio.create_task(self.background_sender.run())
 
         if self.lock is None:
             self.lock = asyncio.Lock()
 
+        await self.ping_backend()
+
+    async def ping_backend(self) -> None:
+        assert self.background_sender is not None
+        await send_asyncio_is_alive(
+            session=self.background_sender.session,
+            url_endpoint=self.server_address.is_alive_endpoint_url(),
+            api_key=self.api_key,
+        )
+
     def _check_connected(self) -> Tuple[asyncio.Lock, "asyncio.Queue[Any]"]:
         if self.lock is None or self.sender_queue is None:
             raise AsyncioSenderNoConnected()
 
         return self.lock, self.sender_queue
 
     async def put(self, item: Any) -> None:
```

### Comparing `comet_mpm-0.8.0/src/comet_mpm/sender/thread_sender.py` & `comet_mpm-1.0.0/src/comet_mpm/sender/thread_sender.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,40 +7,41 @@
 #  \____\___/|_| |_| |_|\___|\__(_)_| |_| |_|_|
 #
 #  Sign up for free at http://www.comet.ml
 #  Copyright (C) 2021 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
-
 import logging
 import queue
 from threading import Lock, Thread
 from typing import Any, Optional, Tuple
 
-from ..batch_utils import ThreadSafeBatch
-from ..connection import get_http_session, get_retry_strategy, send_batch_requests
-from ..events.label_event import LabelEvent
-from ..events.prediction_event import PredictionEvent
+from ..batch_utils import ThreadSafeBatch, split_batch
+from ..connection import (
+    get_http_session,
+    get_retry_strategy,
+    send_batch_requests,
+    send_is_alive,
+)
 from ..logging_messages import (
     BATCH_SENDING_EXCEPTION,
-    LABEL_EVENT_SEND_ERROR,
     MPM_ALREADY_CLOSED_LOG_DATA_WARNING,
-    UNEXPECTED_EVENT_TYPE,
 )
-from .base import CLOSE_MESSAGE, BaseSender, batch_endpoint_url, labels_endpoint_url
+from ..server_address import ServerAddress
+from .base import CLOSE_MESSAGE, BaseSender
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ThreadBackgroundSender:
     def __init__(
         self,
         api_key: str,
-        server_address: str,
+        server_address: ServerAddress,
         sender_queue: "queue.Queue[Any]",
         max_batch_size: int,
         max_batch_time: int,
         batch_sending_timeout: int,
     ):
         self.api_key = api_key
         self.server_address = server_address
@@ -49,16 +50,16 @@
         self.batch = ThreadSafeBatch(max_batch_size, self.max_batch_time)
         self.session = get_http_session(retry_strategy=get_retry_strategy())
         self.batch_sending_timeout = batch_sending_timeout
 
         self.stop_processing = False
 
         # Pre-compute URLs
-        self.batch_endpoint = batch_endpoint_url(self.server_address)
-        self.labels_endpoint = labels_endpoint_url(self.server_address)
+        self.batch_endpoint = self.server_address.batch_endpoint_url()
+        self.labels_endpoint = self.server_address.labels_endpoint_url()
 
     def run(self) -> None:
         """This is meant to be run in an independent Thread"""
         while self.stop_processing is False:
             stop = self._loop()
 
             if stop is True:
@@ -74,55 +75,46 @@
             if data is None:
                 return False
 
             if data is CLOSE_MESSAGE:
                 self.stop_processing = True
                 return True
 
-            if isinstance(data, PredictionEvent):
-                self._process_prediction_event(event=data)
-            elif isinstance(data, LabelEvent):
-                self._process_label_event(event=data)
-            else:
-                LOGGER.error(UNEXPECTED_EVENT_TYPE, data)
+            self.batch.append(data)
         except queue.Empty:
             pass
 
         self._check_batch_sending()
 
         return False
 
-    def _process_label_event(self, event: LabelEvent) -> None:
-        try:
-            send_batch_requests(
-                self.session,
-                self.labels_endpoint,
-                api_key=self.api_key,
-                batch=event.create_event_dict(),
-                batch_sending_timeout=self.batch_sending_timeout,
-            )
-        except Exception:
-            LOGGER.error(LABEL_EVENT_SEND_ERROR, exc_info=True)
-
-    def _process_prediction_event(self, event: PredictionEvent) -> None:
-        to_send = event.create_event_dict()
-        self.batch.append(to_send)
-
     def _check_batch_sending(self) -> None:
         try:
             if self.batch.should_be_uploaded(self.stop_processing):
-                batch = self.batch.get_and_clear()
+                batch_to_send = self.batch.get_and_clear()
 
-                send_batch_requests(
-                    self.session,
-                    self.batch_endpoint,
-                    api_key=self.api_key,
-                    batch=batch,
-                    batch_sending_timeout=self.batch_sending_timeout,
-                )
+                predictions_batch, labels_batch = split_batch(batch_to_send)
+
+                if predictions_batch:
+                    send_batch_requests(
+                        self.session,
+                        self.batch_endpoint,
+                        api_key=self.api_key,
+                        batch=predictions_batch,
+                        batch_sending_timeout=self.batch_sending_timeout,
+                    )
+
+                if labels_batch:
+                    send_batch_requests(
+                        self.session,
+                        self.labels_endpoint,
+                        api_key=self.api_key,
+                        batch=labels_batch,
+                        batch_sending_timeout=self.batch_sending_timeout,
+                    )
         except Exception:
             LOGGER.error(BATCH_SENDING_EXCEPTION, exc_info=True)
 
     def close(self) -> None:
         """For the BackgroundSender to stop processing messages"""
         self.stop_processing = True
         # This shouldn't happen outside of the background sender thread
@@ -131,15 +123,15 @@
         self.session.close()
 
 
 class ThreadSender(BaseSender):
     def __init__(
         self,
         api_key: str,
-        server_address: str,
+        server_address: ServerAddress,
         max_batch_size: int,
         max_batch_time: int,
         batch_sending_timeout: int,
     ) -> None:
         self.lock = Lock()
         self.sender_queue: Optional["queue.Queue[Any]"] = None
         self.background_sender: Optional[ThreadBackgroundSender] = None
@@ -208,20 +200,31 @@
         """There is no easy way to plug a shutdown callback with Flask, the "normal" cleaning
         process for Flask is to use the close method"""
         return None
 
     def connect(self) -> None:
         """There is no easy way nor need to plug a startup callback as we can create everything and
         do the handshake during Python import"""
-        return None
+        self.ping_backend()
+
+    def ping_backend(self) -> None:
+        if self.background_sender is None:
+            session = get_http_session(get_retry_strategy())
+        else:
+            session = self.background_sender.session
+        send_is_alive(
+            session=session,
+            url_endpoint=self.server_address.is_alive_endpoint_url(),
+            api_key=self.api_key,
+        )
 
 
 def get_thread_sender(
     api_key: str,
-    server_address: str,
+    server_address: ServerAddress,
     max_batch_size: int,
     max_batch_time: int,
     batch_sending_timeout: int,
 ) -> "ThreadSender":
     sender = ThreadSender(
         api_key=api_key,
         server_address=server_address,
@@ -231,15 +234,15 @@
     )
 
     return sender
 
 
 def _get_thread_background_sender(
     api_key: str,
-    server_address: str,
+    server_address: ServerAddress,
     max_batch_size: int,
     max_batch_time: int,
     batch_sending_timeout: int,
 ) -> Tuple["queue.Queue[Any]", "ThreadBackgroundSender"]:
     sender_queue: queue.Queue[Any] = queue.Queue()
     background_sender = ThreadBackgroundSender(
         api_key=api_key,
```

### Comparing `comet_mpm-0.8.0/src/comet_mpm/settings.py` & `comet_mpm-1.0.0/src/comet_mpm/settings.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm/settings_helper.py` & `comet_mpm-1.0.0/src/comet_mpm/settings_helper.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.8.0/src/comet_mpm.egg-info/SOURCES.txt` & `comet_mpm-1.0.0/src/comet_mpm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 src/comet_mpm/batch_utils.py
 src/comet_mpm/cli.py
 src/comet_mpm/comet_mpm.py
 src/comet_mpm/connection.py
 src/comet_mpm/connection_helpers.py
 src/comet_mpm/constants.py
 src/comet_mpm/data_series.py
+src/comet_mpm/dataset_upload_helpers.py
 src/comet_mpm/environment.py
 src/comet_mpm/exceptions.py
 src/comet_mpm/logging_messages.py
 src/comet_mpm/optional_update.py
+src/comet_mpm/server_address.py
 src/comet_mpm/settings.py
 src/comet_mpm/settings_helper.py
 src/comet_mpm/_json/__init__.py
 src/comet_mpm/_json/numpy_encoder.py
 src/comet_mpm/api_key/__init__.py
 src/comet_mpm/api_key/base64_helper.py
 src/comet_mpm/api_key/comet_api_key.py
```

