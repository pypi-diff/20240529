# Comparing `tmp/strangeworks_hybrid_optimize-0.1.5.tar.gz` & `tmp/strangeworks_hybrid_optimize-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_hybrid_optimize-0.1.5.tar", max compression
+gzip compressed data, was "strangeworks_hybrid_optimize-0.1.6.tar", max compression
```

## Comparing `strangeworks_hybrid_optimize-0.1.5.tar` & `strangeworks_hybrid_optimize-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       61 2023-11-29 15:16:36.168921 strangeworks_hybrid_optimize-0.1.5/README.md
--rw-r--r--   0        0        0      883 2023-11-29 15:16:48.825127 strangeworks_hybrid_optimize-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      346 2023-11-29 15:16:36.172921 strangeworks_hybrid_optimize-0.1.5/strangeworks_hybrid_optimize/__init__.py
--rw-r--r--   0        0        0    24931 2023-11-29 15:16:36.172921 strangeworks_hybrid_optimize-0.1.5/strangeworks_hybrid_optimize/sdk.py
--rw-r--r--   0        0        0    12428 2023-11-29 15:16:36.172921 strangeworks_hybrid_optimize-0.1.5/strangeworks_hybrid_optimize/utils.py
--rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 strangeworks_hybrid_optimize-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       61 2024-05-29 14:00:19.751355 strangeworks_hybrid_optimize-0.1.6/README.md
+-rw-r--r--   0        0        0      883 2024-05-29 14:00:29.067377 strangeworks_hybrid_optimize-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      346 2024-05-29 14:00:19.755355 strangeworks_hybrid_optimize-0.1.6/strangeworks_hybrid_optimize/__init__.py
+-rw-r--r--   0        0        0    25066 2024-05-29 14:00:19.755355 strangeworks_hybrid_optimize-0.1.6/strangeworks_hybrid_optimize/sdk.py
+-rw-r--r--   0        0        0    12428 2024-05-29 14:00:19.755355 strangeworks_hybrid_optimize-0.1.6/strangeworks_hybrid_optimize/utils.py
+-rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 strangeworks_hybrid_optimize-0.1.6/PKG-INFO
```

### Comparing `strangeworks_hybrid_optimize-0.1.5/pyproject.toml` & `strangeworks_hybrid_optimize-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-hybrid-optimize"
-version = "0.1.5"
+version = "0.1.6"
 description = "Extension to strangeworks sdk to allow user to run the hybrid optimization service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_hybrid_optimize"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `strangeworks_hybrid_optimize-0.1.5/strangeworks_hybrid_optimize/sdk.py` & `strangeworks_hybrid_optimize-0.1.6/strangeworks_hybrid_optimize/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,17 @@
             raise StrangeworksError(
                 f"Unable to find resource. Please add resource on platform https://portal.strangeworks.com/products: {e}"  # noqa: E501
             )
 
         self.backend_list = " "
 
     def backends(self):
-        all_backends = strangeworks.backends(backend_type_slugs=["sw-qaoa"])
+        ibm_backends = strangeworks.backends(product_slugs=["ibm-qiskit-runtime"])
+        aws_backends = strangeworks.backends(product_slugs=["amazon-braket"])
+        all_backends = ibm_backends + aws_backends
 
         aws_backends = []
         aws_sim_backends = []
         ibmq_backends = []
         ibm_cloud_backends = []
         ibm_sim_backends = []
         for bb in range(len(all_backends)):
```

### Comparing `strangeworks_hybrid_optimize-0.1.5/strangeworks_hybrid_optimize/utils.py` & `strangeworks_hybrid_optimize-0.1.6/strangeworks_hybrid_optimize/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_hybrid_optimize-0.1.5/PKG-INFO` & `strangeworks_hybrid_optimize-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-hybrid-optimize
-Version: 0.1.5
+Version: 0.1.6
 Summary: Extension to strangeworks sdk to allow user to run the hybrid optimization service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

