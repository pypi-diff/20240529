# Comparing `tmp/knn-tspi-1.0.0.tar.gz` & `tmp/knn_tspi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knn-tspi-1.0.0.tar", last modified: Thu Sep 28 20:16:01 2023, max compression
+gzip compressed data, was "knn_tspi-1.0.1.tar", max compression
```

## Comparing `knn-tspi-1.0.0.tar` & `knn_tspi-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:16:01.163589 knn-tspi-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-09-28 20:16:01.163589 knn-tspi-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:16:01.159589 knn-tspi-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   108038 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/examples/customize-hypothesis-function.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    80613 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/examples/forecasting-with-confidence.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    69962 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/examples/getting-started.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:16:01.163589 knn-tspi-1.0.0/knn_tspi/
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/knn_tspi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/knn_tspi/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/knn_tspi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/knn_tspi/distances.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/knn_tspi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/knn_tspi/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/knn_tspi/scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/knn_tspi/similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/knn_tspi/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:16:01.163589 knn-tspi-1.0.0/knn_tspi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-09-28 20:16:01.000000 knn-tspi-1.0.0/knn_tspi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-09-28 20:16:01.000000 knn-tspi-1.0.0/knn_tspi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-28 20:16:01.000000 knn-tspi-1.0.0/knn_tspi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-28 20:16:01.000000 knn-tspi-1.0.0/knn_tspi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-28 20:16:01.000000 knn-tspi-1.0.0/knn_tspi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-28 20:16:01.163589 knn-tspi-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-09-28 20:15:53.000000 knn-tspi-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:16:01.163589 knn-tspi-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2023-09-28 20:15:31.000000 knn-tspi-1.0.0/tests/test_knn_tspi.py
+-rw-r--r--   0        0        0     1073 2024-05-29 21:14:04.746737 knn_tspi-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     4862 2024-05-29 21:14:04.746737 knn_tspi-1.0.1/README.md
+-rw-r--r--   0        0        0     4650 2024-05-29 21:14:04.966738 knn_tspi-1.0.1/knn_tspi/__init__.py
+-rw-r--r--   0        0        0     1498 2024-05-29 21:14:04.750738 knn_tspi-1.0.1/knn_tspi/bootstrap.py
+-rw-r--r--   0        0        0      124 2024-05-29 21:14:04.750738 knn_tspi-1.0.1/knn_tspi/constants.py
+-rw-r--r--   0        0        0      441 2024-05-29 21:14:04.750738 knn_tspi-1.0.1/knn_tspi/distances.py
+-rw-r--r--   0        0        0      381 2024-05-29 21:14:04.750738 knn_tspi-1.0.1/knn_tspi/exceptions.py
+-rw-r--r--   0        0        0     2099 2024-05-29 21:14:04.750738 knn_tspi-1.0.1/knn_tspi/predict.py
+-rw-r--r--   0        0        0      409 2024-05-29 21:14:04.750738 knn_tspi-1.0.1/knn_tspi/scores.py
+-rw-r--r--   0        0        0     1710 2024-05-29 21:14:04.750738 knn_tspi-1.0.1/knn_tspi/similarity.py
+-rw-r--r--   0        0        0     1587 2024-05-29 21:14:04.750738 knn_tspi-1.0.1/knn_tspi/validation.py
+-rw-r--r--   0        0        0     1575 2024-05-29 21:15:50.486970 knn_tspi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5926 1970-01-01 00:00:00.000000 knn_tspi-1.0.1/PKG-INFO
```

### Comparing `knn-tspi-1.0.0/LICENSE.txt` & `knn_tspi-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `knn-tspi-1.0.0/knn_tspi/__init__.py` & `knn_tspi-1.0.1/knn_tspi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 
 from knn_tspi.bootstrap import bootstrap_residuals, calculate_residuals
 from knn_tspi.predict import predict
 from knn_tspi.validation import validate_hyperparameters, validate_fit, validate_predict
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 
 class KNeighborsTSPI:
     """K-Nearest Neighbors Time Series Prediction with Invariances
 
     Parameters
     ----------
```

### Comparing `knn-tspi-1.0.0/knn_tspi/bootstrap.py` & `knn_tspi-1.0.1/knn_tspi/bootstrap.py`

 * *Files identical despite different names*

### Comparing `knn-tspi-1.0.0/knn_tspi/predict.py` & `knn_tspi-1.0.1/knn_tspi/predict.py`

 * *Files identical despite different names*

### Comparing `knn-tspi-1.0.0/knn_tspi/similarity.py` & `knn_tspi-1.0.1/knn_tspi/similarity.py`

 * *Files identical despite different names*

### Comparing `knn-tspi-1.0.0/knn_tspi/validation.py` & `knn_tspi-1.0.1/knn_tspi/validation.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     InvalidDataException,
 )
 
 
 def validate_hyperparameters(
     k: int, len_query: int, weights: Literal["uniform", "distance"]
 ) -> None:
-    if type(k) != int or k <= 0:
+    if not isinstance(k, int) or k <= 0:
         raise InvalidParameterException(
             f"Number of neighbors must be an integer greater than 1, got {k}!"
         )
-    if type(len_query) != int or len_query <= 2:
+    if not isinstance(len_query, int) or len_query <= 2:
         raise InvalidParameterException(
             f"Query length must be an integer greater than 3, got {len_query}!"
         )
     if weights not in (
         "uniform",
         "distance",
     ):
@@ -37,13 +37,13 @@
     if data.dtype.kind not in ("f", "i"):
         raise InvalidDataException("Data must be numerical!")
     if np.isnan(data).any():
         raise InvalidDataException("Data has missing values on it!")
 
 
 def validate_predict(h: int, is_fitted: bool) -> None:
-    if type(h) != int or h <= 0:
+    if not isinstance(h, int) or h <= 0:
         raise InvalidParameterException(
             f"Horizon must be an integer greater than 0, got {h}!"
         )
     if not is_fitted:
         raise ModelNotFittedException("Model hasn't been fitted yet")
```

