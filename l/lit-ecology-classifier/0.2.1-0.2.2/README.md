# Comparing `tmp/lit_ecology_classifier-0.2.1.tar.gz` & `tmp/lit_ecology_classifier-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lit_ecology_classifier-0.2.1.tar", last modified: Wed May 29 13:14:53 2024, max compression
+gzip compressed data, was "lit_ecology_classifier-0.2.2.tar", last modified: Wed May 29 13:16:04 2024, max compression
```

## Comparing `lit_ecology_classifier-0.2.1.tar` & `lit_ecology_classifier-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 13:14:53.000000 lit_ecology_classifier-0.2.1/
--rw-r--r--   0 bkch     (29810) em09     (32012)     1068 2024-05-29 12:20:15.000000 lit_ecology_classifier-0.2.1/LICENSE
--rw-r--r--   0 bkch     (29810) em09     (32012)     3701 2024-05-29 13:14:53.000000 lit_ecology_classifier-0.2.1/PKG-INFO
--rw-r--r--   0 bkch     (29810) em09     (32012)     2969 2024-05-29 12:20:15.000000 lit_ecology_classifier-0.2.1/README.md
-drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 13:14:53.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/
--rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/__init__.py
-drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 13:14:53.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/data/
--rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/data/__init__.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     8631 2024-05-29 08:00:08.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/data/datamodule.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     8457 2024-05-28 12:07:34.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/data/tardataset.py
-drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 13:14:53.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/helpers/
--rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/helpers/__init__.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     2652 2024-05-29 12:47:00.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/helpers/argparser.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     1145 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/helpers/calc_class_weights.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     8045 2024-05-29 07:04:21.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/helpers/helpers.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     3469 2024-05-29 08:00:08.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/main.py
-drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 13:14:53.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/models/
--rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/models/__init__.py
--rw-r--r--   0 bkch     (29810) em09     (32012)    11407 2024-05-29 12:46:01.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/models/model.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     2665 2024-05-29 12:45:34.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/models/setup_model.py
--rw-r--r--   0 bkch     (29810) em09     (32012)     1817 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier/predict.py
-drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 13:14:53.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier.egg-info/
--rw-r--r--   0 bkch     (29810) em09     (32012)     3701 2024-05-29 13:14:52.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier.egg-info/PKG-INFO
--rw-r--r--   0 bkch     (29810) em09     (32012)      836 2024-05-29 13:14:52.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 bkch     (29810) em09     (32012)        1 2024-05-29 13:14:52.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 bkch     (29810) em09     (32012)       76 2024-05-29 13:14:52.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier.egg-info/entry_points.txt
--rw-r--r--   0 bkch     (29810) em09     (32012)       94 2024-05-29 13:14:52.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier.egg-info/requires.txt
--rw-r--r--   0 bkch     (29810) em09     (32012)       23 2024-05-29 13:14:52.000000 lit_ecology_classifier-0.2.1/lit_ecology_classifier.egg-info/top_level.txt
--rw-r--r--   0 bkch     (29810) em09     (32012)       38 2024-05-29 13:14:53.000000 lit_ecology_classifier-0.2.1/setup.cfg
--rw-r--r--   0 bkch     (29810) em09     (32012)     1133 2024-05-29 13:14:44.000000 lit_ecology_classifier-0.2.1/setup.py
+drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/
+-rw-r--r--   0 bkch     (29810) em09     (32012)     1068 2024-05-29 12:20:15.000000 lit_ecology_classifier-0.2.2/LICENSE
+-rw-r--r--   0 bkch     (29810) em09     (32012)     3706 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/PKG-INFO
+-rw-r--r--   0 bkch     (29810) em09     (32012)     2969 2024-05-29 12:20:15.000000 lit_ecology_classifier-0.2.2/README.md
+drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/
+-rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/__init__.py
+drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/data/
+-rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/data/__init__.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     8631 2024-05-29 08:00:08.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/data/datamodule.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     8457 2024-05-28 12:07:34.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/data/tardataset.py
+drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/helpers/
+-rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/helpers/__init__.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     2652 2024-05-29 12:47:00.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/helpers/argparser.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     1145 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/helpers/calc_class_weights.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     8045 2024-05-29 07:04:21.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/helpers/helpers.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     3469 2024-05-29 08:00:08.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/main.py
+drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/models/
+-rw-r--r--   0 bkch     (29810) em09     (32012)        0 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/models/__init__.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)    11407 2024-05-29 12:46:01.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/models/model.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     2665 2024-05-29 12:45:34.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/models/setup_model.py
+-rw-r--r--   0 bkch     (29810) em09     (32012)     1817 2024-05-28 11:43:01.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier/predict.py
+drwxr-xr-x   0 bkch     (29810) em09     (32012)        0 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier.egg-info/
+-rw-r--r--   0 bkch     (29810) em09     (32012)     3706 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 bkch     (29810) em09     (32012)      836 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 bkch     (29810) em09     (32012)        1 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 bkch     (29810) em09     (32012)       76 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier.egg-info/entry_points.txt
+-rw-r--r--   0 bkch     (29810) em09     (32012)       99 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier.egg-info/requires.txt
+-rw-r--r--   0 bkch     (29810) em09     (32012)       23 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/lit_ecology_classifier.egg-info/top_level.txt
+-rw-r--r--   0 bkch     (29810) em09     (32012)       38 2024-05-29 13:16:04.000000 lit_ecology_classifier-0.2.2/setup.cfg
+-rw-r--r--   0 bkch     (29810) em09     (32012)     1138 2024-05-29 13:16:01.000000 lit_ecology_classifier-0.2.2/setup.py
```

### Comparing `lit_ecology_classifier-0.2.1/LICENSE` & `lit_ecology_classifier-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.2.1/PKG-INFO` & `lit_ecology_classifier-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit_ecology_classifier
-Version: 0.2.1
+Version: 0.2.2
 Summary: Image Classifier optimised for ecology use-cases
 Home-page: https://github.com/kaechb/lit_ecology_classifier
 Author: Benno Kaech
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Requires-Dist: lightning
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: timm
 Requires-Dist: safetensors
-Requires-Dist: sklearn
+Requires-Dist: scikit-learn
 
 # Lit Ecology Classifier
 Documentation: https://lit-ecology-classifier.readthedocs.io/en/latest/
 Lit Ecology Classifier is a machine learning project designed for image classification tasks. It leverages PyTorch Lightning for streamlined training and evaluation processes.
 
 ## Features
```

### Comparing `lit_ecology_classifier-0.2.1/README.md` & `lit_ecology_classifier-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.2.1/lit_ecology_classifier/data/datamodule.py` & `lit_ecology_classifier-0.2.2/lit_ecology_classifier/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.2.1/lit_ecology_classifier/data/tardataset.py` & `lit_ecology_classifier-0.2.2/lit_ecology_classifier/data/tardataset.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.2.1/lit_ecology_classifier/helpers/argparser.py` & `lit_ecology_classifier-0.2.2/lit_ecology_classifier/helpers/argparser.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.2.1/lit_ecology_classifier/helpers/calc_class_weights.py` & `lit_ecology_classifier-0.2.2/lit_ecology_classifier/helpers/calc_class_weights.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.2.1/lit_ecology_classifier/helpers/helpers.py` & `lit_ecology_classifier-0.2.2/lit_ecology_classifier/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.2.1/lit_ecology_classifier/main.py` & `lit_ecology_classifier-0.2.2/lit_ecology_classifier/main.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.2.1/lit_ecology_classifier/models/model.py` & `lit_ecology_classifier-0.2.2/lit_ecology_classifier/models/model.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.2.1/lit_ecology_classifier/models/setup_model.py` & `lit_ecology_classifier-0.2.2/lit_ecology_classifier/models/setup_model.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.2.1/lit_ecology_classifier/predict.py` & `lit_ecology_classifier-0.2.2/lit_ecology_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.2.1/lit_ecology_classifier.egg-info/PKG-INFO` & `lit_ecology_classifier-0.2.2/lit_ecology_classifier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit_ecology_classifier
-Version: 0.2.1
+Version: 0.2.2
 Summary: Image Classifier optimised for ecology use-cases
 Home-page: https://github.com/kaechb/lit_ecology_classifier
 Author: Benno Kaech
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Requires-Dist: lightning
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: timm
 Requires-Dist: safetensors
-Requires-Dist: sklearn
+Requires-Dist: scikit-learn
 
 # Lit Ecology Classifier
 Documentation: https://lit-ecology-classifier.readthedocs.io/en/latest/
 Lit Ecology Classifier is a machine learning project designed for image classification tasks. It leverages PyTorch Lightning for streamlined training and evaluation processes.
 
 ## Features
```

### Comparing `lit_ecology_classifier-0.2.1/lit_ecology_classifier.egg-info/SOURCES.txt` & `lit_ecology_classifier-0.2.2/lit_ecology_classifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lit_ecology_classifier-0.2.1/setup.py` & `lit_ecology_classifier-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lit_ecology_classifier',
-    version='0.2.1',
+    version='0.2.2',
     description='Image Classifier optimised for ecology use-cases',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'torch',
         'torchvision',
@@ -19,15 +19,15 @@
         'lightning',
         'numpy',
         'scipy',
         'pandas',
         'matplotlib',
         'timm',
         'safetensors',
-        'sklearn'
+        'scikit-learn'
         # Add other dependencies here
     ],
     entry_points={
         'console_scripts': [
             'lit_ecology_classifier=lit_ecology_classifier.main:main',
         ],
     },
```

