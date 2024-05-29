# Comparing `tmp/pratlib-0.1.0.tar.gz` & `tmp/pratlib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pratlib-0.1.0.tar", last modified: Tue May 28 04:01:21 2024, max compression
+gzip compressed data, was "pratlib-1.0.1.tar", last modified: Wed May 29 17:28:49 2024, max compression
```

## Comparing `pratlib-0.1.0.tar` & `pratlib-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:01:21.027882 pratlib-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-28 04:01:13.000000 pratlib-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-28 04:01:21.027882 pratlib-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-28 04:01:13.000000 pratlib-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:01:21.023882 pratlib-0.1.0/models/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-28 04:01:13.000000 pratlib-0.1.0/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:01:21.027882 pratlib-0.1.0/models/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-28 04:01:13.000000 pratlib-0.1.0/models/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-28 04:01:13.000000 pratlib-0.1.0/models/classification/decision_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-28 04:01:13.000000 pratlib-0.1.0/models/classification/gradient_boosting.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-28 04:01:13.000000 pratlib-0.1.0/models/classification/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-28 04:01:13.000000 pratlib-0.1.0/models/classification/naive_bayes.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-28 04:01:13.000000 pratlib-0.1.0/models/classification/random_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:01:21.027882 pratlib-0.1.0/models/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-28 04:01:13.000000 pratlib-0.1.0/models/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-28 04:01:13.000000 pratlib-0.1.0/models/regression/decision_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-28 04:01:13.000000 pratlib-0.1.0/models/regression/gradient_boosting.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-28 04:01:13.000000 pratlib-0.1.0/models/regression/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-28 04:01:13.000000 pratlib-0.1.0/models/regression/random_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:01:21.027882 pratlib-0.1.0/pratlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-28 04:01:20.000000 pratlib-0.1.0/pratlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-28 04:01:20.000000 pratlib-0.1.0/pratlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 04:01:20.000000 pratlib-0.1.0/pratlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 04:01:20.000000 pratlib-0.1.0/pratlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 04:01:20.000000 pratlib-0.1.0/pratlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:01:21.027882 pratlib-0.1.0/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-28 04:01:13.000000 pratlib-0.1.0/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-28 04:01:13.000000 pratlib-0.1.0/preprocessing/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-28 04:01:13.000000 pratlib-0.1.0/preprocessing/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-28 04:01:13.000000 pratlib-0.1.0/preprocessing/imputer.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-28 04:01:13.000000 pratlib-0.1.0/preprocessing/scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:01:13.000000 pratlib-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 04:01:21.027882 pratlib-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-28 04:01:13.000000 pratlib-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:28:49.453565 pratlib-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 17:28:42.000000 pratlib-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-29 17:28:49.453565 pratlib-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-29 17:28:42.000000 pratlib-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:28:49.449565 pratlib-1.0.1/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-29 17:28:42.000000 pratlib-1.0.1/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:28:49.449565 pratlib-1.0.1/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-29 17:28:42.000000 pratlib-1.0.1/models/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-29 17:28:42.000000 pratlib-1.0.1/models/classification/decision_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-29 17:28:42.000000 pratlib-1.0.1/models/classification/gradient_boosting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-29 17:28:42.000000 pratlib-1.0.1/models/classification/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-29 17:28:42.000000 pratlib-1.0.1/models/classification/naive_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-29 17:28:42.000000 pratlib-1.0.1/models/classification/random_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:28:49.449565 pratlib-1.0.1/models/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-29 17:28:42.000000 pratlib-1.0.1/models/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-29 17:28:42.000000 pratlib-1.0.1/models/regression/decision_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-29 17:28:42.000000 pratlib-1.0.1/models/regression/gradient_boosting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-29 17:28:42.000000 pratlib-1.0.1/models/regression/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-29 17:28:42.000000 pratlib-1.0.1/models/regression/random_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:28:49.453565 pratlib-1.0.1/pratlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-29 17:28:49.000000 pratlib-1.0.1/pratlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-29 17:28:49.000000 pratlib-1.0.1/pratlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:28:49.000000 pratlib-1.0.1/pratlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 17:28:49.000000 pratlib-1.0.1/pratlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 17:28:49.000000 pratlib-1.0.1/pratlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:28:49.453565 pratlib-1.0.1/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-29 17:28:42.000000 pratlib-1.0.1/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-29 17:28:42.000000 pratlib-1.0.1/preprocessing/dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-29 17:28:42.000000 pratlib-1.0.1/preprocessing/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-29 17:28:42.000000 pratlib-1.0.1/preprocessing/imputer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-29 17:28:42.000000 pratlib-1.0.1/preprocessing/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:28:42.000000 pratlib-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:28:49.453565 pratlib-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-29 17:28:42.000000 pratlib-1.0.1/setup.py
```

### Comparing `pratlib-0.1.0/LICENSE` & `pratlib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pratlib-0.1.0/PKG-INFO` & `pratlib-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pratlib
-Version: 0.1.0
+Version: 1.0.1
 Summary: A PySpark library for machine learning, similar to scikit-learn.
 Home-page: https://github.com/pratiush1234/pratlib
 Author: Pratiush
 Author-email: pratiushanand1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pratlib-0.1.0/models/__init__.py` & `pratlib-1.0.1/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pratlib-0.1.0/models/classification/decision_tree.py` & `pratlib-1.0.1/models/classification/decision_tree.py`

 * *Files identical despite different names*

### Comparing `pratlib-0.1.0/models/classification/gradient_boosting.py` & `pratlib-1.0.1/models/classification/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `pratlib-0.1.0/models/classification/logistic_regression.py` & `pratlib-1.0.1/models/classification/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `pratlib-0.1.0/models/classification/random_forest.py` & `pratlib-1.0.1/models/classification/random_forest.py`

 * *Files identical despite different names*

### Comparing `pratlib-0.1.0/models/regression/decision_tree.py` & `pratlib-1.0.1/models/regression/decision_tree.py`

 * *Files identical despite different names*

### Comparing `pratlib-0.1.0/models/regression/gradient_boosting.py` & `pratlib-1.0.1/models/regression/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `pratlib-0.1.0/models/regression/linear_regression.py` & `pratlib-1.0.1/models/regression/linear_regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,7 +8,8 @@
     def fit(self, df, features_col='features', label_col='label'):
         self.model.setFeaturesCol(features_col).setLabelCol(label_col)
         self.fitted_model = self.model.fit(df)
         return self
 
     def predict(self, df):
         return self.fitted_model.transform(df)
+
```

### Comparing `pratlib-0.1.0/models/regression/random_forest.py` & `pratlib-1.0.1/models/regression/random_forest.py`

 * *Files identical despite different names*

### Comparing `pratlib-0.1.0/pratlib.egg-info/PKG-INFO` & `pratlib-1.0.1/pratlib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pratlib
-Version: 0.1.0
+Version: 1.0.1
 Summary: A PySpark library for machine learning, similar to scikit-learn.
 Home-page: https://github.com/pratiush1234/pratlib
 Author: Pratiush
 Author-email: pratiushanand1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pratlib-0.1.0/pratlib.egg-info/SOURCES.txt` & `pratlib-1.0.1/pratlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pratlib-0.1.0/preprocessing/scaler.py` & `pratlib-1.0.1/preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `pratlib-0.1.0/setup.py` & `pratlib-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='pratlib',
-    version='0.1.0',
+    version='1.0.1',
     author='Pratiush',
     author_email='pratiushanand1@gmail.com',
     description='A PySpark library for machine learning, similar to scikit-learn.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/pratiush1234/pratlib',
     packages=find_packages(),
```

