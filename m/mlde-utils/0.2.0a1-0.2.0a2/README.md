# Comparing `tmp/mlde_utils-0.2.0a1.tar.gz` & `tmp/mlde_utils-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlde_utils-0.2.0a1.tar", last modified: Fri Mar 22 11:42:58 2024, max compression
+gzip compressed data, was "mlde_utils-0.2.0a2.tar", last modified: Wed May 29 13:17:39 2024, max compression
```

## Comparing `mlde_utils-0.2.0a1.tar` & `mlde_utils-0.2.0a2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:42:58.533621 mlde_utils-0.2.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-22 11:42:58.533621 mlde_utils-0.2.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 11:42:58.533621 mlde_utils-0.2.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:42:58.529621 mlde_utils-0.2.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:42:58.529621 mlde_utils-0.2.0a1/src/mlde_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:42:58.533621 mlde_utils-0.2.0a1/src/mlde_utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/data/coarsen.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/data/constrain.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/data/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/data/regrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/data/remapcon.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/data/resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/data/select_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/data/select_gcm_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/data/shift_lon_break.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/data/split_by_year.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/data/sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/data/vorticity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:42:58.533621 mlde_utils-0.2.0a1/src/mlde_utils/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/training/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-03-22 11:42:51.000000 mlde_utils-0.2.0a1/src/mlde_utils/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:42:58.533621 mlde_utils-0.2.0a1/src/mlde_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-22 11:42:58.000000 mlde_utils-0.2.0a1/src/mlde_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-22 11:42:58.000000 mlde_utils-0.2.0a1/src/mlde_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 11:42:58.000000 mlde_utils-0.2.0a1/src/mlde_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-22 11:42:58.000000 mlde_utils-0.2.0a1/src/mlde_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:39.257098 mlde_utils-0.2.0a2/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-29 13:17:39.253098 mlde_utils-0.2.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:17:39.257098 mlde_utils-0.2.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:39.249098 mlde_utils-0.2.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:39.249098 mlde_utils-0.2.0a2/src/mlde_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:39.253098 mlde_utils-0.2.0a2/src/mlde_utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/data/coarsen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/data/constrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/data/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/data/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/data/remapcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/data/resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/data/select_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/data/select_gcm_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/data/shift_lon_break.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/data/split_by_year.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/data/sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/data/vorticity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:39.253098 mlde_utils-0.2.0a2/src/mlde_utils/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/training/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13082 2024-05-29 13:17:33.000000 mlde_utils-0.2.0a2/src/mlde_utils/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:39.253098 mlde_utils-0.2.0a2/src/mlde_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-29 13:17:39.000000 mlde_utils-0.2.0a2/src/mlde_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-29 13:17:39.000000 mlde_utils-0.2.0a2/src/mlde_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:17:39.000000 mlde_utils-0.2.0a2/src/mlde_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 13:17:39.000000 mlde_utils-0.2.0a2/src/mlde_utils.egg-info/top_level.txt
```

### Comparing `mlde_utils-0.2.0a1/PKG-INFO` & `mlde_utils-0.2.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlde_utils
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: A package for shared code between ML downscaling repos
 Author-email: Henry Addison <henry.addison@bristol.ac.uk>
 Project-URL: Homepage, https://github.com/henryaddison/mlde_utils
 Project-URL: Bug Tracker, https://github.com/henryaddison/mlde_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlde_utils-0.2.0a1/pyproject.toml` & `mlde_utils-0.2.0a2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlde_utils"
-version = "0.2.0a1"
+version = "0.2.0a2"
 authors = [
   { name="Henry Addison", email="henry.addison@bristol.ac.uk" },
 ]
 description = "A package for shared code between ML downscaling repos"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mlde_utils-0.2.0a1/src/mlde_utils/__init__.py` & `mlde_utils-0.2.0a2/src/mlde_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlde_utils-0.2.0a1/src/mlde_utils/data/regrid.py` & `mlde_utils-0.2.0a2/src/mlde_utils/data/regrid.py`

 * *Files identical despite different names*

### Comparing `mlde_utils-0.2.0a1/src/mlde_utils/data/remapcon.py` & `mlde_utils-0.2.0a2/src/mlde_utils/data/remapcon.py`

 * *Files identical despite different names*

### Comparing `mlde_utils-0.2.0a1/src/mlde_utils/data/resample.py` & `mlde_utils-0.2.0a2/src/mlde_utils/data/resample.py`

 * *Files identical despite different names*

### Comparing `mlde_utils-0.2.0a1/src/mlde_utils/data/select_domain.py` & `mlde_utils-0.2.0a2/src/mlde_utils/data/select_domain.py`

 * *Files identical despite different names*

### Comparing `mlde_utils-0.2.0a1/src/mlde_utils/data/select_gcm_domain.py` & `mlde_utils-0.2.0a2/src/mlde_utils/data/select_gcm_domain.py`

 * *Files identical despite different names*

### Comparing `mlde_utils-0.2.0a1/src/mlde_utils/data/split_by_year.py` & `mlde_utils-0.2.0a2/src/mlde_utils/data/split_by_year.py`

 * *Files identical despite different names*

### Comparing `mlde_utils-0.2.0a1/src/mlde_utils/data/vorticity.py` & `mlde_utils-0.2.0a2/src/mlde_utils/data/vorticity.py`

 * *Files identical despite different names*

### Comparing `mlde_utils-0.2.0a1/src/mlde_utils/training/dataset.py` & `mlde_utils-0.2.0a2/src/mlde_utils/training/dataset.py`

 * *Files identical despite different names*

### Comparing `mlde_utils-0.2.0a1/src/mlde_utils/transforms.py` & `mlde_utils-0.2.0a2/src/mlde_utils/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,20 @@
 
     def transform(self, ds):
         for var in self.variables:
             ds[var] = (ds[var] - self.means[var]) / self.stds[var]
 
         return ds
 
+    def invert(self, ds):
+        for var in self.variables:
+            ds[var] = (ds[var] * self.stds[var]) + self.means[var]
+
+        return ds
+
 
 class PixelStandardize:
     def __init__(self, variables):
         self.variables = variables
 
     def fit(self, target_ds, model_src_ds):
         self.means = {
@@ -196,14 +202,34 @@
             nclipped = (ds[var] < min).sum().item()
             logger.debug(f"Clipping {var} to {min}: {nclipped}")
             ds[var] = ds[var].clip(min=min)
 
         return ds
 
 
+class PercentToPropT:
+    def __init__(self, variables):
+        self.variables = variables
+
+    def fit(self, target_ds, _model_src_ds):
+        return self
+
+    def transform(self, ds):
+        for var in self.variables:
+            ds[var] = ds[var] / 100.0
+
+        return ds
+
+    def invert(self, ds):
+        for var in self.variables:
+            ds[var] = ds[var] * 100.0
+
+        return ds
+
+
 class RecentreT:
     def __init__(self, variables):
         self.variables = variables
 
     def fit(self, target_ds, model_src_ds):
         return self
 
@@ -468,8 +494,40 @@
                 ClipT(target_variables),
                 LogT(target_variables),
                 UnitRangeT(target_variables),
                 RecentreT(target_variables),
             ]
         )
 
+    if key == "stanurrecen":
+        return ComposeT(
+            [
+                Standardize(target_variables),
+                UnitRangeT(target_variables),
+                RecentreT(target_variables),
+            ]
+        )
+
+    if key == "urrecen":
+        return ComposeT(
+            [
+                UnitRangeT(target_variables),
+                RecentreT(target_variables),
+            ]
+        )
+
+    if key == "pcrecen":
+        return ComposeT(
+            [
+                PercentToPropT(target_variables),
+                RecentreT(target_variables),
+            ]
+        )
+
+    if key == "recen":
+        return ComposeT(
+            [
+                RecentreT(target_variables),
+            ]
+        )
+
     raise RuntimeError(f"Unknown input transform {key}")
```

### Comparing `mlde_utils-0.2.0a1/src/mlde_utils.egg-info/PKG-INFO` & `mlde_utils-0.2.0a2/src/mlde_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlde_utils
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: A package for shared code between ML downscaling repos
 Author-email: Henry Addison <henry.addison@bristol.ac.uk>
 Project-URL: Homepage, https://github.com/henryaddison/mlde_utils
 Project-URL: Bug Tracker, https://github.com/henryaddison/mlde_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlde_utils-0.2.0a1/src/mlde_utils.egg-info/SOURCES.txt` & `mlde_utils-0.2.0a2/src/mlde_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

