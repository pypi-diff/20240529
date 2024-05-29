# Comparing `tmp/tif_to_zarr-0.5.1.tar.gz` & `tmp/tif_to_zarr-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tif_to_zarr-0.5.1.tar", max compression
+gzip compressed data, was "tif_to_zarr-0.5.3.tar", max compression
```

## Comparing `tif_to_zarr-0.5.1.tar` & `tif_to_zarr-0.5.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1518 2024-04-29 20:35:53.842078 tif_to_zarr-0.5.1/LICENSE
--rw-r--r--   0        0        0      924 2024-04-29 20:13:11.195310 tif_to_zarr-0.5.1/README.md
--rw-r--r--   0        0        0      554 2024-05-29 14:13:59.410156 tif_to_zarr-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       84 2024-04-30 17:36:20.760280 tif_to_zarr-0.5.1/tif_to_zarr/__init__.py
--rw-r--r--   0        0        0     4695 2024-05-07 15:55:20.018381 tif_to_zarr-0.5.1/tif_to_zarr/conversion_lib.py
--rw-r--r--   0        0        0      326 2024-04-29 20:59:01.518144 tif_to_zarr-0.5.1/tif_to_zarr/n5_attrs_template.json
--rw-r--r--   0        0        0     1349 2024-05-07 15:12:17.576959 tif_to_zarr-0.5.1/tif_to_zarr/tif_to_zarr.py
--rw-r--r--   0        0        0      268 2024-04-29 20:13:11.195310 tif_to_zarr-0.5.1/tif_to_zarr/zarr_attrs_template.json
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 tif_to_zarr-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1518 2024-04-29 20:35:53.842078 tif_to_zarr-0.5.3/LICENSE
+-rw-r--r--   0        0        0      924 2024-04-29 20:13:11.195310 tif_to_zarr-0.5.3/README.md
+-rw-r--r--   0        0        0      631 2024-05-29 14:48:43.540699 tif_to_zarr-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-30 17:36:20.760280 tif_to_zarr-0.5.3/tif_to_zarr/__init__.py
+-rw-r--r--   0        0        0     4695 2024-05-07 15:55:20.018381 tif_to_zarr-0.5.3/tif_to_zarr/conversion_lib.py
+-rw-r--r--   0        0        0      326 2024-04-29 20:59:01.518144 tif_to_zarr-0.5.3/tif_to_zarr/n5_attrs_template.json
+-rw-r--r--   0        0        0     1418 2024-05-29 14:46:01.628058 tif_to_zarr-0.5.3/tif_to_zarr/tif_to_zarr.py
+-rw-r--r--   0        0        0      268 2024-04-29 20:13:11.195310 tif_to_zarr-0.5.3/tif_to_zarr/zarr_attrs_template.json
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 tif_to_zarr-0.5.3/PKG-INFO
```

### Comparing `tif_to_zarr-0.5.1/LICENSE` & `tif_to_zarr-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.5.1/README.md` & `tif_to_zarr-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.5.1/pyproject.toml` & `tif_to_zarr-0.5.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tif_to_zarr"
-version = "0.5.1"
+version = "0.5.3"
 description = ""
 authors = ["yurii_zubov"]
 license = "BSD 3-Clause License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -18,10 +18,13 @@
 dask = "^2023.10.1"
 dask-jobqueue = "^0.8.2"
 numpy = "^1.25.1"
 tifffile = "^2023.9.26"
 logging = "^0.4.9.6"
 xarray-multiscale = "^2.1.0"
 
+[tool.poetry.scripts]
+tiff_to_zarr = 'tif_to_zarr.tif_to_zarr:tiff_to_zarr'
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tif_to_zarr-0.5.1/tif_to_zarr/conversion_lib.py` & `tif_to_zarr-0.5.3/tif_to_zarr/conversion_lib.py`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.5.1/PKG-INFO` & `tif_to_zarr-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tif_to_zarr
-Version: 0.5.1
+Version: 0.5.3
 Summary: 
 License: BSD 3-Clause License
 Author: yurii_zubov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

