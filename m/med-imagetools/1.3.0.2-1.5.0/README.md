# Comparing `tmp/med_imagetools-1.3.0.2.tar.gz` & `tmp/med_imagetools-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "med_imagetools-1.3.0.2.tar", max compression
+gzip compressed data, was "med_imagetools-1.5.0.tar", max compression
```

## Comparing `med_imagetools-1.3.0.2.tar` & `med_imagetools-1.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    35149 2024-05-24 12:49:47.568958 med_imagetools-1.3.0.2/LICENSE
--rw-r--r--   0        0        0     6059 2024-05-24 12:49:47.568958 med_imagetools-1.3.0.2/README.md
--rw-r--r--   0        0        0     1091 2024-05-24 12:49:47.572958 med_imagetools-1.3.0.2/pyproject.toml
--rw-r--r--   0        0        0      108 2024-05-24 12:49:47.572958 med_imagetools-1.3.0.2/src/imgtools/__init__.py
--rw-r--r--   0        0        0    41216 2024-05-24 12:49:47.572958 med_imagetools-1.3.0.2/src/imgtools/autopipeline.py
--rw-r--r--   0        0        0     8396 2024-05-24 12:49:47.572958 med_imagetools-1.3.0.2/src/imgtools/image.py
--rw-r--r--   0        0        0       68 2024-05-24 12:49:47.572958 med_imagetools-1.3.0.2/src/imgtools/io/__init__.py
--rw-r--r--   0        0        0     1714 2024-05-24 12:49:47.572958 med_imagetools-1.3.0.2/src/imgtools/io/common.py
--rw-r--r--   0        0        0     9680 2024-05-24 12:49:47.572958 med_imagetools-1.3.0.2/src/imgtools/io/dataset.py
--rw-r--r--   0        0        0    13185 2024-05-24 12:49:47.572958 med_imagetools-1.3.0.2/src/imgtools/io/loaders.py
--rw-r--r--   0        0        0    11169 2024-05-24 12:49:47.572958 med_imagetools-1.3.0.2/src/imgtools/io/writers.py
--rw-r--r--   0        0        0      166 2024-05-24 12:49:47.572958 med_imagetools-1.3.0.2/src/imgtools/modules/__init__.py
--rw-r--r--   0        0        0    28610 2024-05-24 12:49:47.572958 med_imagetools-1.3.0.2/src/imgtools/modules/datagraph.py
--rw-r--r--   0        0        0     5239 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/modules/dose.py
--rw-r--r--   0        0        0     6925 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/modules/pet.py
--rw-r--r--   0        0        0      217 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/modules/scan.py
--rw-r--r--   0        0        0     7624 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/modules/segmentation.py
--rw-r--r--   0        0        0      221 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/modules/sparsemask.py
--rw-r--r--   0        0        0     9690 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/modules/structureset.py
--rw-r--r--   0        0        0     2066 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/ops/README.md
--rw-r--r--   0        0        0       19 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/ops/__init__.py
--rw-r--r--   0        0        0    22644 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/ops/functional.py
--rw-r--r--   0        0        0    63269 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/ops/ops.py
--rw-r--r--   0        0        0     4768 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/pipeline.py
--rw-r--r--   0        0        0        0 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/transforms/__init__.py
--rw-r--r--   0        0        0      462 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/transforms/intensity.py
--rw-r--r--   0        0        0     6218 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/transforms/spatial.py
--rw-r--r--   0        0        0      169 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/utils/__init__.py
--rw-r--r--   0        0        0     4392 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/utils/args.py
--rw-r--r--   0        0        0      792 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/utils/arrayutils.py
--rw-r--r--   0        0        0     4679 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/utils/autopipeutils.py
--rw-r--r--   0        0        0    11095 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/utils/crawl.py
--rw-r--r--   0        0        0     3094 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/utils/dicomutils.py
--rw-r--r--   0        0        0     1584 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/utils/imageutils.py
--rw-r--r--   0        0        0     1828 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/utils/nifti_to_dicom.py
--rw-r--r--   0        0        0     4675 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/utils/nnunet.py
--rw-r--r--   0        0        0        0 2024-05-24 12:49:47.576958 med_imagetools-1.3.0.2/src/imgtools/utils/report.py
--rw-r--r--   0        0        0     7228 1970-01-01 00:00:00.000000 med_imagetools-1.3.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-29 19:00:21.330288 med_imagetools-1.5.0/LICENSE
+-rw-r--r--   0        0        0     6059 2024-05-29 19:00:21.330288 med_imagetools-1.5.0/README.md
+-rw-r--r--   0        0        0     1421 2024-05-29 19:00:21.334288 med_imagetools-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-05-29 19:00:21.334288 med_imagetools-1.5.0/src/imgtools/__init__.py
+-rw-r--r--   0        0        0    41216 2024-05-29 19:00:21.334288 med_imagetools-1.5.0/src/imgtools/autopipeline.py
+-rw-r--r--   0        0        0     8396 2024-05-29 19:00:21.334288 med_imagetools-1.5.0/src/imgtools/image.py
+-rw-r--r--   0        0        0       68 2024-05-29 19:00:21.334288 med_imagetools-1.5.0/src/imgtools/io/__init__.py
+-rw-r--r--   0        0        0     1714 2024-05-29 19:00:21.334288 med_imagetools-1.5.0/src/imgtools/io/common.py
+-rw-r--r--   0        0        0     9680 2024-05-29 19:00:21.334288 med_imagetools-1.5.0/src/imgtools/io/dataset.py
+-rw-r--r--   0        0        0    13185 2024-05-29 19:00:21.334288 med_imagetools-1.5.0/src/imgtools/io/loaders.py
+-rw-r--r--   0        0        0    11169 2024-05-29 19:00:21.334288 med_imagetools-1.5.0/src/imgtools/io/writers.py
+-rw-r--r--   0        0        0      166 2024-05-29 19:00:21.334288 med_imagetools-1.5.0/src/imgtools/modules/__init__.py
+-rw-r--r--   0        0        0    28610 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/modules/datagraph.py
+-rw-r--r--   0        0        0     5239 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/modules/dose.py
+-rw-r--r--   0        0        0     6925 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/modules/pet.py
+-rw-r--r--   0        0        0      217 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/modules/scan.py
+-rw-r--r--   0        0        0     7624 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/modules/segmentation.py
+-rw-r--r--   0        0        0      221 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/modules/sparsemask.py
+-rw-r--r--   0        0        0     9690 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/modules/structureset.py
+-rw-r--r--   0        0        0     2066 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/ops/README.md
+-rw-r--r--   0        0        0       19 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/ops/__init__.py
+-rw-r--r--   0        0        0    22644 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/ops/functional.py
+-rw-r--r--   0        0        0    63269 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/ops/ops.py
+-rw-r--r--   0        0        0     4768 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/pipeline.py
+-rw-r--r--   0        0        0        0 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/transforms/__init__.py
+-rw-r--r--   0        0        0      462 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/transforms/intensity.py
+-rw-r--r--   0        0        0     6218 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/transforms/spatial.py
+-rw-r--r--   0        0        0      169 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/utils/__init__.py
+-rw-r--r--   0        0        0     4392 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/utils/args.py
+-rw-r--r--   0        0        0      792 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/utils/arrayutils.py
+-rw-r--r--   0        0        0     4679 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/utils/autopipeutils.py
+-rw-r--r--   0        0        0    11095 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/utils/crawl.py
+-rw-r--r--   0        0        0     3094 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/utils/dicomutils.py
+-rw-r--r--   0        0        0     1584 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/utils/imageutils.py
+-rw-r--r--   0        0        0     1828 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/utils/nifti_to_dicom.py
+-rw-r--r--   0        0        0     4675 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/utils/nnunet.py
+-rw-r--r--   0        0        0        0 2024-05-29 19:00:21.338288 med_imagetools-1.5.0/src/imgtools/utils/report.py
+-rw-r--r--   0        0        0     7229 1970-01-01 00:00:00.000000 med_imagetools-1.5.0/PKG-INFO
```

### Comparing `med_imagetools-1.3.0.2/LICENSE` & `med_imagetools-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/README.md` & `med_imagetools-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/pyproject.toml` & `med_imagetools-1.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # shoutout to @jjjermiah for the Poetry crash course
 [tool.poetry]
 name = "med-imagetools"
 packages = [{ include = "imgtools", from = "src" }]
-version = "1.3.0.2"
+version = "1.5.0"
 description = "Med-Imagetools: Transparent and Reproducible Medical Image Processing Pipelines in Python"
 authors = ["Sejin Kim, Benjamin Haibe-Kains"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.dependencies]
-python = ">=3.10 || 3.12"
+python = ">=3.10,<4"
 h5py = "^3.11.0"
 joblib = "^1.4.2"
 numpy = "^1.26.4"
 matplotlib = "^3.8.4"
 pandas = "^2.2.2"
 pydicom = "^2.4.4"
 pynrrd = "^1.0.0"
@@ -32,15 +32,27 @@
 autopipeline = "imgtools.autopipeline:main"
 betapipeline = "imgtools.autopipeline_refactored:main"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 ruff = "^0.4.4"
 pytest-cov = ">=4.0.0"
+python-semantic-release = "^9.8.0"
 
 [tool.poetry.extras]
 torch = ["torch", "torchio"]
 debug = ["pyvis"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.semantic_release]
+version_variables = ["setup.py:__version__"]
+version_toml = ["pyproject.toml:tool.poetry.version"]
+upload_to_release = true
+remove_dist = false
+commit_message = "chore(sem-ver): {version}"
+patch_without_tag = true
+
+[tool.semantic_release.branches.main]
+match = "(main|master)"
```

### Comparing `med_imagetools-1.3.0.2/src/imgtools/autopipeline.py` & `med_imagetools-1.5.0/src/imgtools/autopipeline.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/image.py` & `med_imagetools-1.5.0/src/imgtools/image.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/io/common.py` & `med_imagetools-1.5.0/src/imgtools/io/common.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/io/dataset.py` & `med_imagetools-1.5.0/src/imgtools/io/dataset.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/io/loaders.py` & `med_imagetools-1.5.0/src/imgtools/io/loaders.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/io/writers.py` & `med_imagetools-1.5.0/src/imgtools/io/writers.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/modules/datagraph.py` & `med_imagetools-1.5.0/src/imgtools/modules/datagraph.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/modules/dose.py` & `med_imagetools-1.5.0/src/imgtools/modules/dose.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/modules/pet.py` & `med_imagetools-1.5.0/src/imgtools/modules/pet.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/modules/segmentation.py` & `med_imagetools-1.5.0/src/imgtools/modules/segmentation.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/modules/structureset.py` & `med_imagetools-1.5.0/src/imgtools/modules/structureset.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/ops/README.md` & `med_imagetools-1.5.0/src/imgtools/ops/README.md`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/ops/functional.py` & `med_imagetools-1.5.0/src/imgtools/ops/functional.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/ops/ops.py` & `med_imagetools-1.5.0/src/imgtools/ops/ops.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/pipeline.py` & `med_imagetools-1.5.0/src/imgtools/pipeline.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/transforms/spatial.py` & `med_imagetools-1.5.0/src/imgtools/transforms/spatial.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/utils/args.py` & `med_imagetools-1.5.0/src/imgtools/utils/args.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/utils/arrayutils.py` & `med_imagetools-1.5.0/src/imgtools/utils/arrayutils.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/utils/autopipeutils.py` & `med_imagetools-1.5.0/src/imgtools/utils/autopipeutils.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/utils/crawl.py` & `med_imagetools-1.5.0/src/imgtools/utils/crawl.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/utils/dicomutils.py` & `med_imagetools-1.5.0/src/imgtools/utils/dicomutils.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/utils/imageutils.py` & `med_imagetools-1.5.0/src/imgtools/utils/imageutils.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/utils/nifti_to_dicom.py` & `med_imagetools-1.5.0/src/imgtools/utils/nifti_to_dicom.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/src/imgtools/utils/nnunet.py` & `med_imagetools-1.5.0/src/imgtools/utils/nnunet.py`

 * *Files identical despite different names*

### Comparing `med_imagetools-1.3.0.2/PKG-INFO` & `med_imagetools-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: med-imagetools
-Version: 1.3.0.2
+Version: 1.5.0
 Summary: Med-Imagetools: Transparent and Reproducible Medical Image Processing Pipelines in Python
 License: GPL-3.0
 Author: Sejin Kim, Benjamin Haibe-Kains
-Requires-Python: >=3.10
+Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: debug
 Provides-Extra: torch
```

