# Comparing `tmp/datagen_kuma-0.0.1.tar.gz` & `tmp/datagen_kuma-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagen_kuma-0.0.1.tar", last modified: Tue May 28 05:48:57 2024, max compression
+gzip compressed data, was "datagen_kuma-0.0.2.tar", last modified: Wed May 29 01:31:11 2024, max compression
```

## Comparing `datagen_kuma-0.0.1.tar` & `datagen_kuma-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 05:48:57.342537 datagen_kuma-0.0.1/
--rw-rw-rw-   0        0        0     2538 2024-05-28 05:48:57.342537 datagen_kuma-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2024-05-28 05:47:03.000000 datagen_kuma-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 05:48:57.311287 datagen_kuma-0.0.1/datagen_kuma/
--rw-rw-rw-   0        0        0        0 2024-05-28 05:05:39.000000 datagen_kuma-0.0.1/datagen_kuma/__init__.py
--rw-rw-rw-   0        0        0     8785 2024-05-28 04:49:18.000000 datagen_kuma-0.0.1/datagen_kuma/datagen.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:48:57.342537 datagen_kuma-0.0.1/datagen_kuma.egg-info/
--rw-rw-rw-   0        0        0     2538 2024-05-28 05:48:57.000000 datagen_kuma-0.0.1/datagen_kuma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-28 05:48:57.000000 datagen_kuma-0.0.1/datagen_kuma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 05:48:57.000000 datagen_kuma-0.0.1/datagen_kuma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      204 2024-05-28 05:48:57.000000 datagen_kuma-0.0.1/datagen_kuma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-28 05:48:57.000000 datagen_kuma-0.0.1/datagen_kuma.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 05:48:57.342537 datagen_kuma-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1231 2024-05-28 05:48:40.000000 datagen_kuma-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:48:57.326912 datagen_kuma-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2024-05-28 01:36:16.000000 datagen_kuma-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1081 2024-05-28 05:47:03.000000 datagen_kuma-0.0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:11.117751 datagen_kuma-0.0.2/
+-rw-rw-rw-   0        0        0     2538 2024-05-29 01:31:11.117751 datagen_kuma-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1564 2024-05-28 05:47:03.000000 datagen_kuma-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:11.086555 datagen_kuma-0.0.2/datagen_kuma/
+-rw-rw-rw-   0        0        0        0 2024-05-28 05:05:39.000000 datagen_kuma-0.0.2/datagen_kuma/__init__.py
+-rw-rw-rw-   0        0        0     8732 2024-05-28 07:22:19.000000 datagen_kuma-0.0.2/datagen_kuma/datagen.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:11.117751 datagen_kuma-0.0.2/datagen_kuma.egg-info/
+-rw-rw-rw-   0        0        0     2538 2024-05-29 01:31:10.000000 datagen_kuma-0.0.2/datagen_kuma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-29 01:31:11.000000 datagen_kuma-0.0.2/datagen_kuma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 01:31:10.000000 datagen_kuma-0.0.2/datagen_kuma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      204 2024-05-29 01:31:10.000000 datagen_kuma-0.0.2/datagen_kuma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-29 01:31:10.000000 datagen_kuma-0.0.2/datagen_kuma.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 01:31:11.117751 datagen_kuma-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1231 2024-05-29 01:29:46.000000 datagen_kuma-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:11.117751 datagen_kuma-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-28 01:36:16.000000 datagen_kuma-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1081 2024-05-28 05:47:03.000000 datagen_kuma-0.0.2/tests/test.py
```

### Comparing `datagen_kuma-0.0.1/PKG-INFO` & `datagen_kuma-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagen_kuma
-Version: 0.0.1
+Version: 0.0.2
 Summary: DataGen is a library for generating test data.
 Home-page: https://github.com/develinu/datagen.git
 Author: devinu
 Author-email: iwlee.dev@gmail.com
 Project-URL: Homepage, https://github.com/develinu/datagen.git
 Keywords: data generator datagen_kuma pandas dataframe fake
 Classifier: Programming Language :: Python :: 3
```

### Comparing `datagen_kuma-0.0.1/README.md` & `datagen_kuma-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `datagen_kuma-0.0.1/datagen_kuma/datagen.py` & `datagen_kuma-0.0.2/datagen_kuma/datagen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import copy
 from typing import List
 from collections import defaultdict
 
-from icecream import ic
 import numpy as np
 import pandas as pd
 from scipy.stats import gaussian_kde
 
 
 class DataGen:
     """
@@ -213,9 +212,8 @@
         generated_data = [
             *self._generate_categorical_data(),
             *self._generate_numeric_data(),
             *self._generate_datetime_data(),
             *self._generate_boolean_data(),
             *self._generate_etc_data(),
         ]
-        ic(generated_data)
         self._generated_df = pd.concat(generated_data, axis=1)
```

### Comparing `datagen_kuma-0.0.1/datagen_kuma.egg-info/PKG-INFO` & `datagen_kuma-0.0.2/datagen_kuma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagen_kuma
-Version: 0.0.1
+Version: 0.0.2
 Summary: DataGen is a library for generating test data.
 Home-page: https://github.com/develinu/datagen.git
 Author: devinu
 Author-email: iwlee.dev@gmail.com
 Project-URL: Homepage, https://github.com/develinu/datagen.git
 Keywords: data generator datagen_kuma pandas dataframe fake
 Classifier: Programming Language :: Python :: 3
```

### Comparing `datagen_kuma-0.0.1/setup.py` & `datagen_kuma-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="datagen_kuma",
-    version="0.0.1",
+    version="0.0.2",
     author="devinu",
     author_email="iwlee.dev@gmail.com",
     description="DataGen is a library for generating test data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/develinu/datagen.git",
     packages=setuptools.find_packages(),
```

### Comparing `datagen_kuma-0.0.1/tests/test.py` & `datagen_kuma-0.0.2/tests/test.py`

 * *Files identical despite different names*

