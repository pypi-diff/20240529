# Comparing `tmp/spectrum_fundamentals-0.5.3.tar.gz` & `tmp/spectrum_fundamentals-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_fundamentals-0.5.3.tar", max compression
+gzip compressed data, was "spectrum_fundamentals-0.5.4.tar", max compression
```

## Comparing `spectrum_fundamentals-0.5.3.tar` & `spectrum_fundamentals-0.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1102 2024-05-10 06:54:47.221579 spectrum_fundamentals-0.5.3/LICENSE
--rw-r--r--   0        0        0     2611 2024-05-10 06:54:47.221579 spectrum_fundamentals-0.5.3/README.rst
--rw-r--r--   0        0        0     2464 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      939 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/__init__.py
--rw-r--r--   0        0        0      381 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/__main__.py
--rw-r--r--   0        0        0       29 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/annotation/__init__.py
--rw-r--r--   0        0        0    20512 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/annotation/annotation.py
--rw-r--r--   0        0        0     1377 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/charge.py
--rw-r--r--   0        0        0    12541 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/constants.py
--rw-r--r--   0        0        0    19686 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/fragments.py
--rw-r--r--   0        0        0       26 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/__init__.py
--rw-r--r--   0        0        0    34826 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/fragments_ratio.py
--rw-r--r--   0        0        0     1563 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/metric.py
--rw-r--r--   0        0        0    23723 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/percolator.py
--rw-r--r--   0        0        0    26034 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/similarity.py
--rw-r--r--   0        0        0    17026 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/mod_string.py
--rw-r--r--   0        0        0        0 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/py.typed
--rw-r--r--   0        0        0     3700 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-05-29 11:42:28.257124 spectrum_fundamentals-0.5.4/LICENSE
+-rw-r--r--   0        0        0     2611 2024-05-29 11:42:28.257124 spectrum_fundamentals-0.5.4/README.rst
+-rw-r--r--   0        0        0     2468 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      939 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/__main__.py
+-rw-r--r--   0        0        0       29 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/annotation/__init__.py
+-rw-r--r--   0        0        0    20512 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/annotation/annotation.py
+-rw-r--r--   0        0        0     1377 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/charge.py
+-rw-r--r--   0        0        0    12568 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/constants.py
+-rw-r--r--   0        0        0    19686 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/fragments.py
+-rw-r--r--   0        0        0       26 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/metrics/__init__.py
+-rw-r--r--   0        0        0    34826 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/metrics/fragments_ratio.py
+-rw-r--r--   0        0        0     1563 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/metrics/metric.py
+-rw-r--r--   0        0        0    23723 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/metrics/percolator.py
+-rw-r--r--   0        0        0    26034 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/metrics/similarity.py
+-rw-r--r--   0        0        0    17026 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/mod_string.py
+-rw-r--r--   0        0        0        0 2024-05-29 11:42:28.261124 spectrum_fundamentals-0.5.4/spectrum_fundamentals/py.typed
+-rw-r--r--   0        0        0     3696 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.5.4/PKG-INFO
```

### Comparing `spectrum_fundamentals-0.5.3/LICENSE` & `spectrum_fundamentals-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.3/README.rst` & `spectrum_fundamentals-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.3/pyproject.toml` & `spectrum_fundamentals-0.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_fundamentals"
-version = "0.5.3"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.5.4"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Fundamental functions, annotation pipeline and constants for oktoberfest"
 authors = ["Wilhelmlab at Technical University of Munich"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 repository = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 documentation = "https://spectrum_fundamentals.readthedocs.io"
@@ -21,15 +21,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<3.11.0"
 click = ">=8.0.0"
 rich = ">=10.3.0"
 PyYAML = ">=5.4.1"
 numpy = ">=1.24.1,<1.25"
-pandas = "^1.3.0"
+pandas = ">=1.3,<3.0"
 scikit-learn = "^1.0"
 joblib = "^1.0.1"
 moepy = "^1.1.4"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.2.4"
 pytest-cov = "^5.0.0"
```

### Comparing `spectrum_fundamentals-0.5.3/spectrum_fundamentals/__init__.py` & `spectrum_fundamentals-0.5.4/spectrum_fundamentals/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Initialize fundamentals."""
 
 __author__ = "Mario Picciani"
 __email__ = "mario.picciani@tum.de"
-__version__ = "0.5.3"
+__version__ = "0.5.4"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 CONSOLE_LOG_LEVEL = logging.INFO
```

### Comparing `spectrum_fundamentals-0.5.3/spectrum_fundamentals/annotation/annotation.py` & `spectrum_fundamentals-0.5.4/spectrum_fundamentals/annotation/annotation.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.3/spectrum_fundamentals/charge.py` & `spectrum_fundamentals-0.5.4/spectrum_fundamentals/charge.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.3/spectrum_fundamentals/constants.py` & `spectrum_fundamentals-0.5.4/spectrum_fundamentals/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,14 +240,15 @@
     304.2053: "[UNIMOD:730]",
     8.0141: "[UNIMOD:259]",
     10.0082: "[UNIMOD:267]",
     79.9663: "[UNIMOD:21]",
     -18.0105: "[UNIMOD:23]",
     57.0215: "[UNIMOD:4]",
     15.9949: "[UNIMOD:35]",
+    15.994: "[UNIMOD:35]",
     42.0105: "[UNIMOD:1]",
 }
 # these are only used for prosit_grpc, oktoberfest uses the masses from MOD_MASSES
 AA_MOD_MASSES = {
     "K[UNIMOD:737]": AA_MASSES["K"] + MOD_MASSES["[UNIMOD:737]"],
     "M[UNIMOD:35]": AA_MASSES["M"] + MOD_MASSES["[UNIMOD:35]"],
     "C[UNIMOD:4]": AA_MASSES["C"] + MOD_MASSES["[UNIMOD:4]"],
```

### Comparing `spectrum_fundamentals-0.5.3/spectrum_fundamentals/fragments.py` & `spectrum_fundamentals-0.5.4/spectrum_fundamentals/fragments.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/fragments_ratio.py` & `spectrum_fundamentals-0.5.4/spectrum_fundamentals/metrics/fragments_ratio.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/metric.py` & `spectrum_fundamentals-0.5.4/spectrum_fundamentals/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/percolator.py` & `spectrum_fundamentals-0.5.4/spectrum_fundamentals/metrics/percolator.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/similarity.py` & `spectrum_fundamentals-0.5.4/spectrum_fundamentals/metrics/similarity.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.3/spectrum_fundamentals/mod_string.py` & `spectrum_fundamentals-0.5.4/spectrum_fundamentals/mod_string.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.3/PKG-INFO` & `spectrum_fundamentals-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_fundamentals
-Version: 0.5.3
+Version: 0.5.4
 Summary: Fundamental functions, annotation pipeline and constants for oktoberfest
 Home-page: https://github.com/wilhelm-lab/spectrum_fundamentals
 License: MIT
 Author: Wilhelmlab at Technical University of Munich
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: click (>=8.0.0)
 Requires-Dist: joblib (>=1.0.1,<2.0.0)
 Requires-Dist: moepy (>=1.1.4,<2.0.0)
 Requires-Dist: numpy (>=1.24.1,<1.25)
-Requires-Dist: pandas (>=1.3.0,<2.0.0)
+Requires-Dist: pandas (>=1.3,<3.0)
 Requires-Dist: rich (>=10.3.0)
 Requires-Dist: scikit-learn (>=1.0,<2.0)
 Project-URL: Documentation, https://spectrum_fundamentals.readthedocs.io
 Project-URL: Repository, https://github.com/wilhelm-lab/spectrum_fundamentals
 Description-Content-Type: text/x-rst
 
 spectrum_fundamentals
```

