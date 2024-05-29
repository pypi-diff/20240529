# Comparing `tmp/metabotk-0.1.37.tar.gz` & `tmp/metabotk-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabotk-0.1.37.tar", max compression
+gzip compressed data, was "metabotk-0.1.38.tar", max compression
```

## Comparing `metabotk-0.1.37.tar` & `metabotk-0.1.38.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     4442 2024-05-24 14:51:14.708349 metabotk-0.1.37/README.md
--rw-r--r--   0        0        0      531 2024-05-23 10:28:10.899057 metabotk-0.1.37/metabotk/__init__.py
--rw-r--r--   0        0        0       23 2024-05-24 14:28:38.002332 metabotk-0.1.37/metabotk/_version.py
--rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.37/metabotk/cli.py
--rw-r--r--   0        0        0    26255 2024-05-23 10:33:39.163099 metabotk-0.1.37/metabotk/dataset_manager.py
--rw-r--r--   0        0        0     2388 2024-05-21 18:11:30.585916 metabotk-0.1.37/metabotk/dimensionality_reduction.py
--rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.37/metabotk/feature_selection.py
--rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.37/metabotk/imputation.py
--rw-r--r--   0        0        0     6553 2024-05-24 16:03:17.168372 metabotk-0.1.37/metabotk/interface.py
--rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.37/metabotk/missing_handler.py
--rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.37/metabotk/models_handler.py
--rw-r--r--   0        0        0     9020 2024-05-24 16:03:07.004132 metabotk-0.1.37/metabotk/normalization.py
--rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.37/metabotk/outliers_handler.py
--rw-r--r--   0        0        0     5527 2024-05-24 14:44:47.434686 metabotk-0.1.37/metabotk/providers_handler.py
--rw-r--r--   0        0        0     9052 2024-05-24 14:44:35.050377 metabotk-0.1.37/metabotk/statistics_handler.py
--rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.37/metabotk/utils.py
--rw-r--r--   0        0        0     4658 2024-05-10 15:46:25.623360 metabotk-0.1.37/metabotk/visualization_handler.py
--rw-r--r--   0        0        0      735 2024-05-27 10:58:08.641476 metabotk-0.1.37/pyproject.toml
--rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 metabotk-0.1.37/PKG-INFO
+-rw-r--r--   0        0        0     4442 2024-05-24 14:51:14.708349 metabotk-0.1.38/README.md
+-rw-r--r--   0        0        0      615 2024-05-29 15:36:17.621024 metabotk-0.1.38/metabotk/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-29 15:36:41.997620 metabotk-0.1.38/metabotk/_version.py
+-rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.38/metabotk/cli.py
+-rw-r--r--   0        0        0    26255 2024-05-23 10:33:39.163099 metabotk-0.1.38/metabotk/dataset_manager.py
+-rw-r--r--   0        0        0     2388 2024-05-21 18:11:30.585916 metabotk-0.1.38/metabotk/dimensionality_reduction.py
+-rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.38/metabotk/feature_selection.py
+-rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.38/metabotk/imputation.py
+-rw-r--r--   0        0        0     6821 2024-05-29 15:35:57.768538 metabotk-0.1.38/metabotk/interface.py
+-rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.38/metabotk/missing_handler.py
+-rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.38/metabotk/models_handler.py
+-rw-r--r--   0        0        0     9020 2024-05-27 11:11:09.943429 metabotk-0.1.38/metabotk/normalization.py
+-rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.38/metabotk/outliers_handler.py
+-rw-r--r--   0        0        0     5527 2024-05-24 14:44:47.434686 metabotk-0.1.38/metabotk/providers_handler.py
+-rw-r--r--   0        0        0     1037 2024-05-29 15:34:13.821998 metabotk-0.1.38/metabotk/scaling.py
+-rw-r--r--   0        0        0     9052 2024-05-24 14:44:35.050377 metabotk-0.1.38/metabotk/statistics_handler.py
+-rw-r--r--   0        0        0     3235 2024-05-29 15:08:31.336502 metabotk-0.1.38/metabotk/utils.py
+-rw-r--r--   0        0        0     4658 2024-05-10 15:46:25.623360 metabotk-0.1.38/metabotk/visualization_handler.py
+-rw-r--r--   0        0        0      735 2024-05-29 15:36:37.629513 metabotk-0.1.38/pyproject.toml
+-rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 metabotk-0.1.38/PKG-INFO
```

### Comparing `metabotk-0.1.37/README.md` & `metabotk-0.1.38/README.md`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/metabotk/__init__.py` & `metabotk-0.1.38/metabotk/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from .statistics_handler import StatisticsHandler
 from .dataset_manager import DatasetManager
 from .models_handler import ModelsHandler
 from .visualization_handler import Visualization
 from .dimensionality_reduction import DimensionalityReduction
 from .imputation import ImputationHandler
 from .feature_selection import FeatureSelection
+from .normalization import NormalizationHandler
+from .scaling import ScalingHandler
 
 from ._version import __version__
 from .interface import MetaboTK
 
 __all__ = [
     "__version__",
 ]
```

### Comparing `metabotk-0.1.37/metabotk/cli.py` & `metabotk-0.1.38/metabotk/cli.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/metabotk/dataset_manager.py` & `metabotk-0.1.38/metabotk/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/metabotk/dimensionality_reduction.py` & `metabotk-0.1.38/metabotk/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/metabotk/feature_selection.py` & `metabotk-0.1.38/metabotk/feature_selection.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/metabotk/imputation.py` & `metabotk-0.1.38/metabotk/imputation.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/metabotk/interface.py` & `metabotk-0.1.38/metabotk/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from typing import List, Dict
+
 from metabotk.outliers_handler import OutlierHandler
 from metabotk.missing_handler import MissingDataHandler
 from metabotk.statistics_handler import StatisticsHandler
 from metabotk.dataset_manager import DatasetManager
 from metabotk.models_handler import ModelsHandler
 from metabotk.visualization_handler import Visualization
 from metabotk.dimensionality_reduction import DimensionalityReduction
 from metabotk.imputation import ImputationHandler
 from metabotk.feature_selection import FeatureSelection
 from metabotk.normalization import NormalizationHandler
-from typing import List, Dict
+from metabotk.scaling import ScalingHandler
 
 
 class MetaboTK(DatasetManager):
     """
     Class for working with metabolomics data
     """
 
@@ -84,14 +86,21 @@
     def normalization(self):
         """Lazy initialization of NormalizationHandler instance."""
         if not hasattr(self, "_normalization_"):
             self._normalization_ = NormalizationHandler(self)
         return self._normalization_
 
     @property
+    def scaling(self):
+        """Lazy initialization of ScalingHandler instance."""
+        if not hasattr(self, "_scaling_"):
+            self._scaling_ = ScalingHandler(self)
+        return self._scaling_
+
+    @property
     def feature_selection(self):
         """Lazy initialization of FeatureSelection instance."""
         if not hasattr(self, "_feature_selection_"):
             self._feature_selection_ = FeatureSelection(self)
         return self._feature_selection_
 
     ###FUNCTIONS###
```

### Comparing `metabotk-0.1.37/metabotk/missing_handler.py` & `metabotk-0.1.38/metabotk/missing_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/metabotk/models_handler.py` & `metabotk-0.1.38/metabotk/models_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/metabotk/normalization.py` & `metabotk-0.1.38/metabotk/normalization.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/metabotk/outliers_handler.py` & `metabotk-0.1.38/metabotk/outliers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/metabotk/providers_handler.py` & `metabotk-0.1.38/metabotk/providers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/metabotk/statistics_handler.py` & `metabotk-0.1.38/metabotk/statistics_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/metabotk/utils.py` & `metabotk-0.1.38/metabotk/utils.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/metabotk/visualization_handler.py` & `metabotk-0.1.38/metabotk/visualization_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.37/pyproject.toml` & `metabotk-0.1.38/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metabotk"
-version = "0.1.37"
+version = "0.1.38"
 description = "Python toolkit for working with metabolomics data"
 authors = ["matteobolner <matteo.bolner2@unibo.it>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4"
 requests = "^2.31.0"
```

### Comparing `metabotk-0.1.37/PKG-INFO` & `metabotk-0.1.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabotk
-Version: 0.1.37
+Version: 0.1.38
 Summary: Python toolkit for working with metabolomics data
 Author: matteobolner
 Author-email: matteo.bolner2@unibo.it
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

