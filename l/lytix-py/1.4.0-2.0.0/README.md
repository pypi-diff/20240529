# Comparing `tmp/lytix_py-1.4.0.tar.gz` & `tmp/lytix_py-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytix_py-1.4.0.tar", last modified: Thu May 16 18:27:57 2024, max compression
+gzip compressed data, was "lytix_py-2.0.0.tar", last modified: Wed May 29 03:14:35 2024, max compression
```

## Comparing `lytix_py-1.4.0.tar` & `lytix_py-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-16 18:27:57.167312 lytix_py-1.4.0/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-1.4.0/LICENSE.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-16 18:27:57.167096 lytix_py-1.4.0/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-1.4.0/README.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-16 18:27:02.000000 lytix_py-1.4.0/pyproject.toml
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-16 18:27:57.167377 lytix_py-1.4.0/setup.cfg
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-16 18:27:57.164723 lytix_py-1.4.0/src/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-16 18:27:57.165586 lytix_py-1.4.0/src/lytix_py/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-16 18:27:57.166472 lytix_py-1.4.0/src/lytix_py/LLLogger/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      886 2024-05-06 00:20:17.000000 lytix_py-1.4.0/src/lytix_py/LLLogger/LLLogger.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-16 18:27:57.166686 lytix_py-1.4.0/src/lytix_py/MetricCollector/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     3012 2024-05-16 18:27:48.000000 lytix_py-1.4.0/src/lytix_py/MetricCollector/MetricCollector.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      133 2024-05-13 18:41:07.000000 lytix_py-1.4.0/src/lytix_py/__init__.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      658 2024-05-13 18:47:25.000000 lytix_py-1.4.0/src/lytix_py/envVars.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-16 18:27:57.166875 lytix_py-1.4.0/src/lytix_py.egg-info/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-16 18:27:57.000000 lytix_py-1.4.0/src/lytix_py.egg-info/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      345 2024-05-16 18:27:57.000000 lytix_py-1.4.0/src/lytix_py.egg-info/SOURCES.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-16 18:27:57.000000 lytix_py-1.4.0/src/lytix_py.egg-info/dependency_links.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-16 18:27:57.000000 lytix_py-1.4.0/src/lytix_py.egg-info/requires.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-16 18:27:57.000000 lytix_py-1.4.0/src/lytix_py.egg-info/top_level.txt
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.103899 lytix_py-2.0.0/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-2.0.0/LICENSE.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-29 03:14:35.103693 lytix_py-2.0.0/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-2.0.0/README.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-29 03:14:14.000000 lytix_py-2.0.0/pyproject.toml
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-29 03:14:35.103942 lytix_py-2.0.0/setup.cfg
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.099528 lytix_py-2.0.0/src/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.100820 lytix_py-2.0.0/src/lytix_py/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.101679 lytix_py-2.0.0/src/lytix_py/LAsyncStore/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      641 2024-05-29 01:10:56.000000 lytix_py-2.0.0/src/lytix_py/LAsyncStore/LAsyncStore.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.102409 lytix_py-2.0.0/src/lytix_py/LError/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1284 2024-05-29 02:52:56.000000 lytix_py-2.0.0/src/lytix_py/LError/LError.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      988 2024-05-29 03:05:15.000000 lytix_py-2.0.0/src/lytix_py/LError/LErrorIncrement.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       73 2024-05-29 01:24:22.000000 lytix_py-2.0.0/src/lytix_py/LError/__init__.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.102875 lytix_py-2.0.0/src/lytix_py/LLogger/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     2452 2024-05-29 03:13:57.000000 lytix_py-2.0.0/src/lytix_py/LLogger/LLogger.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      309 2024-05-29 03:12:54.000000 lytix_py-2.0.0/src/lytix_py/LLogger/LLoggerStreamWrapper.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.103147 lytix_py-2.0.0/src/lytix_py/MetricCollector/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     3595 2024-05-29 01:55:23.000000 lytix_py-2.0.0/src/lytix_py/MetricCollector/MetricCollector.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      175 2024-05-29 01:24:47.000000 lytix_py-2.0.0/src/lytix_py/__init__.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      658 2024-05-13 18:47:25.000000 lytix_py-2.0.0/src/lytix_py/envVars.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.103464 lytix_py-2.0.0/src/lytix_py.egg-info/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-29 03:14:35.000000 lytix_py-2.0.0/src/lytix_py.egg-info/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      529 2024-05-29 03:14:35.000000 lytix_py-2.0.0/src/lytix_py.egg-info/SOURCES.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-29 03:14:35.000000 lytix_py-2.0.0/src/lytix_py.egg-info/dependency_links.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-29 03:14:35.000000 lytix_py-2.0.0/src/lytix_py.egg-info/requires.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-29 03:14:35.000000 lytix_py-2.0.0/src/lytix_py.egg-info/top_level.txt
```

### Comparing `lytix_py-1.4.0/LICENSE.md` & `lytix_py-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lytix_py-1.4.0/PKG-INFO` & `lytix_py-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.4.0
+Version: 2.0.0
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lytix_py-1.4.0/pyproject.toml` & `lytix_py-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lytix-py"
-version = "1.4.0"
+version = "2.0.0"
 authors = [
   { name="Lytix", email="support@lytix.com" },
 ]
 description = "Official Lytix Client Packages"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `lytix_py-1.4.0/src/lytix_py/MetricCollector/MetricCollector.py` & `lytix_py-2.0.0/src/lytix_py/MetricCollector/MetricCollector.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 
 """
  Main class to collect and report metrics
  back to HQ
 """
 class _MetricCollector:
     _baseURL: str = None
-    # _logger: str = None
+    processing_metric_mutex: int = 0
 
     def __init__(self):
         self._baseURL = urljoin(LytixCreds.LX_BASE_URL, "/v1/metrics")
+        self.processing_metric_mutex = 0
         pass
 
 
     """
     Interal wrapper to send a post request
     """
     def _sendPostRequest(self, endpoint: str, body: dict):
@@ -81,9 +82,27 @@
             self.increment("model.responseTime", responseTime, {"modelName": modelName}.update(metricMetadata))
         except Exception as err:
             self.logger.error(f"Failed to capture model trace: {err}", err, modelName, modelInput)
             raise err
         finally:
             return modelOutput
 
+    """
+    Capture a metric trace event
+    @note You likeley never need to call this directly
+    """
+    def _captureMetricTrace(self, metricName: str, metricValue: int, metricMetadata: dict = {}, logs: list = []):
+        self.processing_metric_mutex += 1
+
+        body = {
+            "metricName": metricName,
+            "metricValue": metricValue,
+            "metricMetadata": metricMetadata,
+            "logs": logs
+        }
+
+        self._sendPostRequest("increment", body)
+
+        self.processing_metric_mutex -= 1
+
 MetricCollector = _MetricCollector()
```

### Comparing `lytix_py-1.4.0/src/lytix_py/envVars.py` & `lytix_py-2.0.0/src/lytix_py/envVars.py`

 * *Files identical despite different names*

### Comparing `lytix_py-1.4.0/src/lytix_py.egg-info/PKG-INFO` & `lytix_py-2.0.0/src/lytix_py.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.4.0
+Version: 2.0.0
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

