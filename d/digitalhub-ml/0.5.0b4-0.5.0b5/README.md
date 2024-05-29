# Comparing `tmp/digitalhub_ml-0.5.0b4.tar.gz` & `tmp/digitalhub_ml-0.5.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_ml-0.5.0b4.tar", last modified: Mon May 27 13:53:57 2024, max compression
+gzip compressed data, was "digitalhub_ml-0.5.0b5.tar", last modified: Wed May 29 09:49:00 2024, max compression
```

## Comparing `digitalhub_ml-0.5.0b4.tar` & `digitalhub_ml-0.5.0b5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:57.034887 digitalhub_ml-0.5.0b4/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      942 2024-05-27 13:53:57.030887 digitalhub_ml-0.5.0b4/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      462 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b4/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:57.026888 digitalhub_ml-0.5.0b4/digitalhub_ml/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-05-27 13:03:31.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:57.030887 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      436 2024-05-06 11:22:14.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/entity_types.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:57.030887 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/models/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/models/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6328 2024-05-27 13:03:31.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/models/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    12455 2024-05-27 13:03:31.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/models/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/models/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1029 2024-05-21 12:34:21.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/models/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      209 2024-02-15 10:15:41.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/models/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:57.030887 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-05-27 13:03:31.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5869 2024-05-27 13:03:31.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-05-27 13:03:31.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      730 2024-05-06 11:19:46.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:57.030887 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-05-27 13:03:31.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.5.0b4/digitalhub_ml/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:57.030887 digitalhub_ml-0.5.0b4/digitalhub_ml.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      942 2024-05-27 13:53:57.000000 digitalhub_ml-0.5.0b4/digitalhub_ml.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      903 2024-05-27 13:53:57.000000 digitalhub_ml-0.5.0b4/digitalhub_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-27 13:53:57.000000 digitalhub_ml-0.5.0b4/digitalhub_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       25 2024-05-27 13:53:57.000000 digitalhub_ml-0.5.0b4/digitalhub_ml.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-05-27 13:53:57.000000 digitalhub_ml-0.5.0b4/digitalhub_ml.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1058 2024-05-27 12:34:24.000000 digitalhub_ml-0.5.0b4/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-27 13:53:57.034887 digitalhub_ml-0.5.0b4/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      462 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b5/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/digitalhub_ml/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-05-27 14:03:58.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      436 2024-05-06 11:22:14.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/entity_types.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6328 2024-05-27 14:03:58.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    12482 2024-05-28 10:51:37.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1427 2024-05-28 09:49:46.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-05-28 09:45:24.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-05-27 14:03:58.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5869 2024-05-27 14:03:58.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-05-27 14:03:58.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      730 2024-05-06 11:19:46.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-05-27 14:03:58.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-05-29 09:49:00.000000 digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      903 2024-05-29 09:49:00.000000 digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-29 09:49:00.000000 digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       29 2024-05-29 09:49:00.000000 digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-05-29 09:49:00.000000 digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1063 2024-05-28 11:34:48.000000 digitalhub_ml-0.5.0b5/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/setup.cfg
```

### Comparing `digitalhub_ml-0.5.0b4/PKG-INFO` & `digitalhub_ml-0.5.0b5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
-Version: 0.5.0b4
+Version: 0.5.0b5
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: digitalhub-data==0.5.0b4
+Requires-Dist: digitalhub-data<0.6,~=0.5.0b
 
 # Digitalhub-ml Library
 
 The Digitalhub-ml SDK library is used to manage entities and executions in Digitalhub from Python.
 The Digitalhub-ml layer is the third layer of the Digitalhub ml platform, focused on machine learning functions.
 It contains the ml entities and objects (Models) and the methods to manage them.
```

### Comparing `digitalhub_ml-0.5.0b4/digitalhub_ml/entities/models/crud.py` & `digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b4/digitalhub_ml/entities/models/entity.py` & `digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,24 +223,25 @@
             Path of the uploaded model.
         """
         # Check if target path is provided and if it is remote
         trg = self._parameter_or_default(target, self.spec.path)
         self._check_remote(trg)
 
         # Check if source path is provided and if it is local
-        src = self._parameter_or_default(source, self.spec.src_path)
-        self._check_local(src)
+        if source is None:
+            raise EntityError("Source path is not specified.")
+        self._check_local(source)
 
         # Get store
         store = get_store(trg)
         if store.is_local():
             raise EntityError("Cannot target local store for upload.")
 
         # Upload model and return remote path
-        return store.upload(src, trg)
+        return store.upload(source, trg)
 
     #############################
     #  Private Helpers
     #############################
 
     @staticmethod
     def _parameter_or_default(parameter: str | None = None, default: str | None = None) -> str:
```

### Comparing `digitalhub_ml-0.5.0b4/digitalhub_ml/entities/projects/crud.py` & `digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b4/digitalhub_ml/entities/projects/entity.py` & `digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b4/digitalhub_ml/entities/projects/spec.py` & `digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b4/digitalhub_ml/entities/registries.py` & `digitalhub_ml-0.5.0b5/digitalhub_ml/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b4/digitalhub_ml.egg-info/PKG-INFO` & `digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
-Version: 0.5.0b4
+Version: 0.5.0b5
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: digitalhub-data==0.5.0b4
+Requires-Dist: digitalhub-data<0.6,~=0.5.0b
 
 # Digitalhub-ml Library
 
 The Digitalhub-ml SDK library is used to manage entities and executions in Digitalhub from Python.
 The Digitalhub-ml layer is the third layer of the Digitalhub ml platform, focused on machine learning functions.
 It contains the ml entities and objects (Models) and the methods to manage them.
```

### Comparing `digitalhub_ml-0.5.0b4/digitalhub_ml.egg-info/SOURCES.txt` & `digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b4/pyproject.toml` & `digitalhub_ml-0.5.0b5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-ml"
-version = "0.5.0b4"
+version = "0.5.0b5"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -16,22 +16,22 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 keywords = ["data", "dataops", "kubernetes"]
 requires-python = ">=3.9"
 dependencies = [
-    "digitalhub-data==0.5.0b4",
+    "digitalhub-data~=0.5.0b, <0.6",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
 [tool.bumpver]
-current_version = "0.5.0b4"
+current_version = "0.5.0b5"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

