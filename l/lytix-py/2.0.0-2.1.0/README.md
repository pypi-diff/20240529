# Comparing `tmp/lytix_py-2.0.0.tar.gz` & `tmp/lytix_py-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytix_py-2.0.0.tar", last modified: Wed May 29 03:14:35 2024, max compression
+gzip compressed data, was "lytix_py-2.1.0.tar", last modified: Wed May 29 13:37:00 2024, max compression
```

## Comparing `lytix_py-2.0.0.tar` & `lytix_py-2.1.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.103899 lytix_py-2.0.0/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-2.0.0/LICENSE.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-29 03:14:35.103693 lytix_py-2.0.0/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-2.0.0/README.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-29 03:14:14.000000 lytix_py-2.0.0/pyproject.toml
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-29 03:14:35.103942 lytix_py-2.0.0/setup.cfg
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.099528 lytix_py-2.0.0/src/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.100820 lytix_py-2.0.0/src/lytix_py/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.101679 lytix_py-2.0.0/src/lytix_py/LAsyncStore/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      641 2024-05-29 01:10:56.000000 lytix_py-2.0.0/src/lytix_py/LAsyncStore/LAsyncStore.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.102409 lytix_py-2.0.0/src/lytix_py/LError/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1284 2024-05-29 02:52:56.000000 lytix_py-2.0.0/src/lytix_py/LError/LError.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      988 2024-05-29 03:05:15.000000 lytix_py-2.0.0/src/lytix_py/LError/LErrorIncrement.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       73 2024-05-29 01:24:22.000000 lytix_py-2.0.0/src/lytix_py/LError/__init__.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.102875 lytix_py-2.0.0/src/lytix_py/LLogger/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     2452 2024-05-29 03:13:57.000000 lytix_py-2.0.0/src/lytix_py/LLogger/LLogger.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      309 2024-05-29 03:12:54.000000 lytix_py-2.0.0/src/lytix_py/LLogger/LLoggerStreamWrapper.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.103147 lytix_py-2.0.0/src/lytix_py/MetricCollector/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     3595 2024-05-29 01:55:23.000000 lytix_py-2.0.0/src/lytix_py/MetricCollector/MetricCollector.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      175 2024-05-29 01:24:47.000000 lytix_py-2.0.0/src/lytix_py/__init__.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      658 2024-05-13 18:47:25.000000 lytix_py-2.0.0/src/lytix_py/envVars.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 03:14:35.103464 lytix_py-2.0.0/src/lytix_py.egg-info/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-29 03:14:35.000000 lytix_py-2.0.0/src/lytix_py.egg-info/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      529 2024-05-29 03:14:35.000000 lytix_py-2.0.0/src/lytix_py.egg-info/SOURCES.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-29 03:14:35.000000 lytix_py-2.0.0/src/lytix_py.egg-info/dependency_links.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-29 03:14:35.000000 lytix_py-2.0.0/src/lytix_py.egg-info/requires.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-29 03:14:35.000000 lytix_py-2.0.0/src/lytix_py.egg-info/top_level.txt
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 13:37:00.155188 lytix_py-2.1.0/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-2.1.0/LICENSE.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-29 13:37:00.154945 lytix_py-2.1.0/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-2.1.0/README.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-29 13:36:38.000000 lytix_py-2.1.0/pyproject.toml
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-29 13:37:00.155235 lytix_py-2.1.0/setup.cfg
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 13:37:00.148542 lytix_py-2.1.0/src/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 13:37:00.150351 lytix_py-2.1.0/src/lytix_py/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 13:37:00.151945 lytix_py-2.1.0/src/lytix_py/FastAPIMiddleware/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      686 2024-05-29 13:26:48.000000 lytix_py-2.1.0/src/lytix_py/FastAPIMiddleware/LytixMiddleware.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      217 2024-05-29 13:25:03.000000 lytix_py-2.1.0/src/lytix_py/FastAPIMiddleware/MiddlewareState.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 13:37:00.152387 lytix_py-2.1.0/src/lytix_py/LAsyncStore/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1227 2024-05-29 13:30:16.000000 lytix_py-2.1.0/src/lytix_py/LAsyncStore/LAsyncStore.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 13:37:00.153198 lytix_py-2.1.0/src/lytix_py/LError/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1284 2024-05-29 02:52:56.000000 lytix_py-2.1.0/src/lytix_py/LError/LError.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      988 2024-05-29 03:05:15.000000 lytix_py-2.1.0/src/lytix_py/LError/LErrorIncrement.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       73 2024-05-29 01:24:22.000000 lytix_py-2.1.0/src/lytix_py/LError/__init__.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 13:37:00.153789 lytix_py-2.1.0/src/lytix_py/LLogger/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     2558 2024-05-29 13:33:33.000000 lytix_py-2.1.0/src/lytix_py/LLogger/LLogger.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      309 2024-05-29 03:12:54.000000 lytix_py-2.1.0/src/lytix_py/LLogger/LLoggerStreamWrapper.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 13:37:00.154237 lytix_py-2.1.0/src/lytix_py/MetricCollector/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     3595 2024-05-29 01:55:23.000000 lytix_py-2.1.0/src/lytix_py/MetricCollector/MetricCollector.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      175 2024-05-29 01:24:47.000000 lytix_py-2.1.0/src/lytix_py/__init__.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      658 2024-05-13 18:47:25.000000 lytix_py-2.1.0/src/lytix_py/envVars.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-29 13:37:00.154568 lytix_py-2.1.0/src/lytix_py.egg-info/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-29 13:37:00.000000 lytix_py-2.1.0/src/lytix_py.egg-info/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      629 2024-05-29 13:37:00.000000 lytix_py-2.1.0/src/lytix_py.egg-info/SOURCES.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-29 13:37:00.000000 lytix_py-2.1.0/src/lytix_py.egg-info/dependency_links.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-29 13:37:00.000000 lytix_py-2.1.0/src/lytix_py.egg-info/requires.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-29 13:37:00.000000 lytix_py-2.1.0/src/lytix_py.egg-info/top_level.txt
```

### Comparing `lytix_py-2.0.0/LICENSE.md` & `lytix_py-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lytix_py-2.0.0/PKG-INFO` & `lytix_py-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 2.0.0
+Version: 2.1.0
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lytix_py-2.0.0/pyproject.toml` & `lytix_py-2.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lytix-py"
-version = "2.0.0"
+version = "2.1.0"
 authors = [
   { name="Lytix", email="support@lytix.com" },
 ]
 description = "Official Lytix Client Packages"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `lytix_py-2.0.0/src/lytix_py/LError/LError.py` & `lytix_py-2.1.0/src/lytix_py/LError/LError.py`

 * *Files identical despite different names*

### Comparing `lytix_py-2.0.0/src/lytix_py/LError/LErrorIncrement.py` & `lytix_py-2.1.0/src/lytix_py/LError/LErrorIncrement.py`

 * *Files identical despite different names*

### Comparing `lytix_py-2.0.0/src/lytix_py/LLogger/LLogger.py` & `lytix_py-2.1.0/src/lytix_py/LLogger/LLogger.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,38 +11,39 @@
     metadata: dict = None
 
     """
     @param config: Optional dict of the following shape: { console: boolean }
     """
     def __init__(self, loggerName: str, metadata: dict = None):
         self.logger = logging.getLogger(loggerName)
+        if not len(self.logger.handlers):
+            hostname = socket.gethostname()
+
+            """
+            Setup formatting and logging config
+            """
+            self.logger.setLevel('INFO')
+            fmt = '{"time": "%(asctime)s.%(msecs)03d",  "hostname": "' + hostname + '",  "level": "%(levelname)s", "msg": "%(message)s",  "name": "%(name)s", "pid": "%(process)d"}'
+
+            datefmt="%Y-%m-%d,%H:%M:%S"
+            formatter = logging.Formatter(fmt, datefmt)
+            handler = logging.StreamHandler(stream=sys.stdout)
+            handler.setFormatter(formatter)
+            self.logger.addHandler(handler)
+
+            progress = LLoggerStreamWrapper()
+            progress.setFormatter(formatter)
+            self.logger.addHandler(progress)
+        
 
         """
         Define our async store to store recent logs
         """
         self.asyncStore = LAsyncStore
 
-        hostname = socket.gethostname()
-
-        """
-        Setup formatting and logging config
-        """
-        self.logger.setLevel('INFO')
-        fmt = '{"time": "%(asctime)s.%(msecs)03d",  "hostname": "' + hostname + '",  "level": "%(levelname)s", "msg": "%(message)s",  "name": "%(name)s", "pid": "%(process)d"}'
-
-        datefmt="%Y-%m-%d,%H:%M:%S"
-        formatter = logging.Formatter(fmt, datefmt)
-        handler = logging.StreamHandler(stream=sys.stdout)
-        handler.setFormatter(formatter)
-        self.logger.addHandler(handler)
-
-        progress = LLoggerStreamWrapper()
-        progress.setFormatter(formatter)
-        self.logger.addHandler(progress)
-
         if (metadata): 
             self.metadata = metadata
 
     def info(self, msg: object):
         toLog = f'{self.getMetadataLoggerString()}{msg}'
         self.logger.info(toLog)
```

### Comparing `lytix_py-2.0.0/src/lytix_py/MetricCollector/MetricCollector.py` & `lytix_py-2.1.0/src/lytix_py/MetricCollector/MetricCollector.py`

 * *Files identical despite different names*

### Comparing `lytix_py-2.0.0/src/lytix_py/envVars.py` & `lytix_py-2.1.0/src/lytix_py/envVars.py`

 * *Files identical despite different names*

### Comparing `lytix_py-2.0.0/src/lytix_py.egg-info/PKG-INFO` & `lytix_py-2.1.0/src/lytix_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 2.0.0
+Version: 2.1.0
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lytix_py-2.0.0/src/lytix_py.egg-info/SOURCES.txt` & `lytix_py-2.1.0/src/lytix_py.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 src/lytix_py/__init__.py
 src/lytix_py/envVars.py
 src/lytix_py.egg-info/PKG-INFO
 src/lytix_py.egg-info/SOURCES.txt
 src/lytix_py.egg-info/dependency_links.txt
 src/lytix_py.egg-info/requires.txt
 src/lytix_py.egg-info/top_level.txt
+src/lytix_py/FastAPIMiddleware/LytixMiddleware.py
+src/lytix_py/FastAPIMiddleware/MiddlewareState.py
 src/lytix_py/LAsyncStore/LAsyncStore.py
 src/lytix_py/LError/LError.py
 src/lytix_py/LError/LErrorIncrement.py
 src/lytix_py/LError/__init__.py
 src/lytix_py/LLogger/LLogger.py
 src/lytix_py/LLogger/LLoggerStreamWrapper.py
 src/lytix_py/MetricCollector/MetricCollector.py
```

