# Comparing `tmp/freeze_dried_data-2.2.0.tar.gz` & `tmp/freeze_dried_data-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeze_dried_data-2.2.0.tar", last modified: Tue May 28 23:04:22 2024, max compression
+gzip compressed data, was "freeze_dried_data-2.2.1.tar", last modified: Tue May 28 23:37:27 2024, max compression
```

## Comparing `freeze_dried_data-2.2.0.tar` & `freeze_dried_data-2.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 23:04:22.287333 freeze_dried_data-2.2.0/
--rwxr-xr-x   0 root         (0) root         (0)     1072 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11553 2024-05-28 23:04:22.287333 freeze_dried_data-2.2.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    10686 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 23:04:22.287333 freeze_dried_data-2.2.0/freeze_dried_data/
--rwxr-xr-x   0 root         (0) root         (0)       33 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5125 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/efficient_index.py
--rwxr-xr-x   0 root         (0) root         (0)    34904 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/freeze_dried_data.py
--rwxr-xr-x   0 root         (0) root         (0)    11613 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/freeze_dried_data_old.py
--rw-r--r--   0 root         (0) root         (0)     2233 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/test_efficient_index.py
--rwxr-xr-x   0 root         (0) root         (0)    40000 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/test_freeze_dried_data.py
--rwxr-xr-x   0 root         (0) root         (0)     7982 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/freeze_dried_data/test_freeze_dried_data_old.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 23:04:22.287333 freeze_dried_data-2.2.0/freeze_dried_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11553 2024-05-28 23:04:22.000000 freeze_dried_data-2.2.0/freeze_dried_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      473 2024-05-28 23:04:22.000000 freeze_dried_data-2.2.0/freeze_dried_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 23:04:22.000000 freeze_dried_data-2.2.0/freeze_dried_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-28 23:04:22.000000 freeze_dried_data-2.2.0/freeze_dried_data.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 23:04:22.287333 freeze_dried_data-2.2.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1125 2024-05-28 23:03:55.000000 freeze_dried_data-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 23:37:27.104439 freeze_dried_data-2.2.1/
+-rwxr-xr-x   0 root         (0) root         (0)     1072 2024-05-28 23:36:26.000000 freeze_dried_data-2.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11553 2024-05-28 23:37:27.104439 freeze_dried_data-2.2.1/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    10686 2024-05-28 23:36:26.000000 freeze_dried_data-2.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 23:37:27.104439 freeze_dried_data-2.2.1/freeze_dried_data/
+-rwxr-xr-x   0 root         (0) root         (0)       33 2024-05-28 23:36:26.000000 freeze_dried_data-2.2.1/freeze_dried_data/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5125 2024-05-28 23:36:26.000000 freeze_dried_data-2.2.1/freeze_dried_data/efficient_index.py
+-rwxr-xr-x   0 root         (0) root         (0)    35063 2024-05-28 23:36:26.000000 freeze_dried_data-2.2.1/freeze_dried_data/freeze_dried_data.py
+-rwxr-xr-x   0 root         (0) root         (0)    11613 2024-05-28 23:36:26.000000 freeze_dried_data-2.2.1/freeze_dried_data/freeze_dried_data_old.py
+-rwxr-xr-x   0 root         (0) root         (0)     2233 2024-05-28 23:36:26.000000 freeze_dried_data-2.2.1/freeze_dried_data/test_efficient_index.py
+-rwxr-xr-x   0 root         (0) root         (0)    39973 2024-05-28 23:36:26.000000 freeze_dried_data-2.2.1/freeze_dried_data/test_freeze_dried_data.py
+-rwxr-xr-x   0 root         (0) root         (0)     7982 2024-05-28 23:36:26.000000 freeze_dried_data-2.2.1/freeze_dried_data/test_freeze_dried_data_old.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 23:37:27.104439 freeze_dried_data-2.2.1/freeze_dried_data.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11553 2024-05-28 23:37:27.000000 freeze_dried_data-2.2.1/freeze_dried_data.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      473 2024-05-28 23:37:27.000000 freeze_dried_data-2.2.1/freeze_dried_data.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 23:37:27.000000 freeze_dried_data-2.2.1/freeze_dried_data.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-28 23:37:27.000000 freeze_dried_data-2.2.1/freeze_dried_data.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 23:37:27.104439 freeze_dried_data-2.2.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1125 2024-05-28 23:36:26.000000 freeze_dried_data-2.2.1/setup.py
```

### Comparing `freeze_dried_data-2.2.0/LICENSE` & `freeze_dried_data-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.2.0/PKG-INFO` & `freeze_dried_data-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze_dried_data
-Version: 2.2.0
+Version: 2.2.1
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-2.2.0/README.md` & `freeze_dried_data-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.2.0/freeze_dried_data/efficient_index.py` & `freeze_dried_data-2.2.1/freeze_dried_data/efficient_index.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.2.0/freeze_dried_data/freeze_dried_data.py` & `freeze_dried_data-2.2.1/freeze_dried_data/freeze_dried_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import pickle as pkl
 import os
 from typing import Any, Dict, Iterator, Tuple, Optional, Union, List
 import sys
 import warnings
 import zlib
 import torch
-from efficient_index import FDDIndexKeyless, FDDIndexComparableKey, FDDIntList, FDDIndexGeneral
+try:
+    from .efficient_index import FDDIndexKeyless, FDDIndexComparableKey, FDDIntList, FDDIndexGeneral, FDDIndexBase
+except ImportError:
+    from efficient_index import FDDIndexKeyless, FDDIndexComparableKey, FDDIntList, FDDIndexGeneral, FDDIndexBase
+
 
 # data is stored in the following format:
 # [record, record, ..., record], [custom_property, custom_property, ..., custom_property], [split, split, ..., split], [columns], index_index, 8 bytes for index_index length
```

### Comparing `freeze_dried_data-2.2.0/freeze_dried_data/freeze_dried_data_old.py` & `freeze_dried_data-2.2.1/freeze_dried_data/freeze_dried_data_old.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.2.0/freeze_dried_data/test_efficient_index.py` & `freeze_dried_data-2.2.1/freeze_dried_data/test_efficient_index.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.2.0/freeze_dried_data/test_freeze_dried_data.py` & `freeze_dried_data-2.2.1/freeze_dried_data/test_freeze_dried_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import unittest
 import random
-from freeze_dried_data import RFDD, WFDD, add_column
-from efficient_index import FDDIndexBase
+from freeze_dried_data import RFDD, WFDD, add_column, FDDIndexBase
 
 class TestFDD(unittest.TestCase):
     test_file = '/tmp/test_fdd.fdd'
     test_file2 = '/tmp/test_fdd2.fdd'
     test_file3 = '/tmp/test_fdd3.fdd'
     test_file4 = '/tmp/test_fdd4.fdd'
```

### Comparing `freeze_dried_data-2.2.0/freeze_dried_data/test_freeze_dried_data_old.py` & `freeze_dried_data-2.2.1/freeze_dried_data/test_freeze_dried_data_old.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.2.0/freeze_dried_data.egg-info/PKG-INFO` & `freeze_dried_data-2.2.1/freeze_dried_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze-dried-data
-Version: 2.2.0
+Version: 2.2.1
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-2.2.0/setup.py` & `freeze_dried_data-2.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='freeze_dried_data',
-    version='2.2.0',
+    version='2.2.1',
     description='A simple format for machine learning datasets',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/tstandley/freeze_dried_data',
     author='Trevor Standley',
     author_email='trevor.standley@gmail.com',
     license='MIT',
```

