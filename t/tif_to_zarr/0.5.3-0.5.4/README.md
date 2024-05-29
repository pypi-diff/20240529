# Comparing `tmp/tif_to_zarr-0.5.3.tar.gz` & `tmp/tif_to_zarr-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tif_to_zarr-0.5.3.tar", max compression
+gzip compressed data, was "tif_to_zarr-0.5.4.tar", max compression
```

## Comparing `tif_to_zarr-0.5.3.tar` & `tif_to_zarr-0.5.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1518 2024-04-29 20:35:53.842078 tif_to_zarr-0.5.3/LICENSE
--rw-r--r--   0        0        0      924 2024-04-29 20:13:11.195310 tif_to_zarr-0.5.3/README.md
--rw-r--r--   0        0        0      631 2024-05-29 14:48:43.540699 tif_to_zarr-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       84 2024-04-30 17:36:20.760280 tif_to_zarr-0.5.3/tif_to_zarr/__init__.py
--rw-r--r--   0        0        0     4695 2024-05-07 15:55:20.018381 tif_to_zarr-0.5.3/tif_to_zarr/conversion_lib.py
--rw-r--r--   0        0        0      326 2024-04-29 20:59:01.518144 tif_to_zarr-0.5.3/tif_to_zarr/n5_attrs_template.json
--rw-r--r--   0        0        0     1418 2024-05-29 14:46:01.628058 tif_to_zarr-0.5.3/tif_to_zarr/tif_to_zarr.py
--rw-r--r--   0        0        0      268 2024-04-29 20:13:11.195310 tif_to_zarr-0.5.3/tif_to_zarr/zarr_attrs_template.json
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 tif_to_zarr-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1518 2024-04-29 20:35:53.842078 tif_to_zarr-0.5.4/LICENSE
+-rw-r--r--   0        0        0      669 2024-05-29 15:05:01.876918 tif_to_zarr-0.5.4/README.md
+-rw-r--r--   0        0        0      631 2024-05-29 15:05:37.853950 tif_to_zarr-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-30 17:36:20.760280 tif_to_zarr-0.5.4/tif_to_zarr/__init__.py
+-rw-r--r--   0        0        0     4695 2024-05-07 15:55:20.018381 tif_to_zarr-0.5.4/tif_to_zarr/conversion_lib.py
+-rw-r--r--   0        0        0      326 2024-04-29 20:59:01.518144 tif_to_zarr-0.5.4/tif_to_zarr/n5_attrs_template.json
+-rw-r--r--   0        0        0     1418 2024-05-29 14:46:01.628058 tif_to_zarr-0.5.4/tif_to_zarr/tif_to_zarr.py
+-rw-r--r--   0        0        0      268 2024-04-29 20:13:11.195310 tif_to_zarr-0.5.4/tif_to_zarr/zarr_attrs_template.json
+-rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 tif_to_zarr-0.5.4/PKG-INFO
```

### Comparing `tif_to_zarr-0.5.3/LICENSE` & `tif_to_zarr-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.5.3/README.md` & `tif_to_zarr-0.5.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 This script could be used for conversion of a .tiff file to .zarr format with OME-NGFF multiscales metadata structure.
 #### How to run
 1. open command line terminal
-2. install poetry tool for dependency management and packaging: https://pypi.org/project/poetry/
-3. switch to the tif_to_zarr directory:
-    ``cd PATH_TO_DIRECTORY/tif_to_zarr``
-4. install python dependencies:
-    ``poetry install``
+2. install tif_to_zarr
+    ``pip install tif_to_zarr``
 5. run script using cli:
-    ``poetry run python src/tif_to_zarr.py --src=PATH_TO_SOURCE_DIRECTORY/input_file.tif --dest=PATH_TO_DEST_DIRECTORY/output_file.zarr``
+    ``tif_to_zarr --src=PATH_TO_SOURCE_DIRECTORY/input_file.tif --dest=PATH_TO_DEST_DIRECTORY/output_file.zarr``
 6. to convert a tiff file to zarr with custom metadata values, you can run smthg similar to this:
-``poetry run python3 src/tif_to_zarr.py --src=path_to_source_tif  --dest=path_to_output_zarr -a x z y -t 1.0 2.0 3.0 -s 4.0 5.0 6.0 -u nanometer nanometer nanometer``
+``tif_to_zarr --src=path_to_source_tif  --dest=path_to_output_zarr -a x z y -t 1.0 2.0 3.0 -s 4.0 5.0 6.0 -u nanometer nanometer nanometer``
 7. To get the list of options, you may run this:
-``poetry run python3 src/tif_to_zarr.py --help``
+``tif_to_zarr --help``
```

### Comparing `tif_to_zarr-0.5.3/pyproject.toml` & `tif_to_zarr-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tif_to_zarr"
-version = "0.5.3"
+version = "0.5.4"
 description = ""
 authors = ["yurii_zubov"]
 license = "BSD 3-Clause License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tif_to_zarr-0.5.3/tif_to_zarr/conversion_lib.py` & `tif_to_zarr-0.5.4/tif_to_zarr/conversion_lib.py`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.5.3/tif_to_zarr/tif_to_zarr.py` & `tif_to_zarr-0.5.4/tif_to_zarr/tif_to_zarr.py`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.5.3/PKG-INFO` & `tif_to_zarr-0.5.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tif_to_zarr
-Version: 0.5.3
+Version: 0.5.4
 Summary: 
 License: BSD 3-Clause License
 Author: yurii_zubov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -15,19 +15,16 @@
 Requires-Dist: imagecodecs (>=2024.1.1,<2025.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 This script could be used for conversion of a .tiff file to .zarr format with OME-NGFF multiscales metadata structure.
 #### How to run
 1. open command line terminal
-2. install poetry tool for dependency management and packaging: https://pypi.org/project/poetry/
-3. switch to the tif_to_zarr directory:
-    ``cd PATH_TO_DIRECTORY/tif_to_zarr``
-4. install python dependencies:
-    ``poetry install``
+2. install tif_to_zarr
+    ``pip install tif_to_zarr``
 5. run script using cli:
-    ``poetry run python src/tif_to_zarr.py --src=PATH_TO_SOURCE_DIRECTORY/input_file.tif --dest=PATH_TO_DEST_DIRECTORY/output_file.zarr``
+    ``tif_to_zarr --src=PATH_TO_SOURCE_DIRECTORY/input_file.tif --dest=PATH_TO_DEST_DIRECTORY/output_file.zarr``
 6. to convert a tiff file to zarr with custom metadata values, you can run smthg similar to this:
-``poetry run python3 src/tif_to_zarr.py --src=path_to_source_tif  --dest=path_to_output_zarr -a x z y -t 1.0 2.0 3.0 -s 4.0 5.0 6.0 -u nanometer nanometer nanometer``
+``tif_to_zarr --src=path_to_source_tif  --dest=path_to_output_zarr -a x z y -t 1.0 2.0 3.0 -s 4.0 5.0 6.0 -u nanometer nanometer nanometer``
 7. To get the list of options, you may run this:
-``poetry run python3 src/tif_to_zarr.py --help``
+``tif_to_zarr --help``
```

