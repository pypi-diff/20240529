# Comparing `tmp/utilsds-0.3.2.tar.gz` & `tmp/utilsds-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilsds-0.3.2.tar", last modified: Tue May 28 11:50:27 2024, max compression
+gzip compressed data, was "utilsds-0.3.3.tar", last modified: Wed May 29 09:59:12 2024, max compression
```

## Comparing `utilsds-0.3.2.tar` & `utilsds-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 patryk.kotulak   (502) staff       (20)        0 2024-05-28 11:50:27.324451 utilsds-0.3.2/
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     6226 2024-05-28 11:50:27.323367 utilsds-0.3.2/PKG-INFO
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)       67 2024-05-28 11:30:15.000000 utilsds-0.3.2/README.md
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)       38 2024-05-28 11:50:27.324512 utilsds-0.3.2/setup.cfg
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     5405 2024-05-28 11:50:23.000000 utilsds-0.3.2/setup.py
-drwxr-xr-x   0 patryk.kotulak   (502) staff       (20)        0 2024-05-28 11:50:27.313960 utilsds-0.3.2/utilsds/
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)        0 2024-05-28 09:41:40.000000 utilsds-0.3.2/utilsds/__init__.py
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     2789 2024-05-28 09:39:31.000000 utilsds-0.3.2/utilsds/data_split.py
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     1174 2024-05-28 09:39:30.000000 utilsds-0.3.2/utilsds/ds_statistics.py
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)    14396 2024-05-28 09:39:30.000000 utilsds-0.3.2/utilsds/model_experiments.py
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     4659 2024-05-28 09:39:31.000000 utilsds-0.3.2/utilsds/transform_data.py
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)    12367 2024-05-28 09:39:31.000000 utilsds-0.3.2/utilsds/visualization.py
-drwxr-xr-x   0 patryk.kotulak   (502) staff       (20)        0 2024-05-28 11:50:27.319360 utilsds-0.3.2/utilsds.egg-info/
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     6226 2024-05-28 11:50:27.000000 utilsds-0.3.2/utilsds.egg-info/PKG-INFO
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)      319 2024-05-28 11:50:27.000000 utilsds-0.3.2/utilsds.egg-info/SOURCES.txt
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)        1 2024-05-28 11:50:27.000000 utilsds-0.3.2/utilsds.egg-info/dependency_links.txt
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)     2940 2024-05-28 11:50:27.000000 utilsds-0.3.2/utilsds.egg-info/requires.txt
--rw-r--r--   0 patryk.kotulak   (502) staff       (20)        8 2024-05-28 11:50:27.000000 utilsds-0.3.2/utilsds.egg-info/top_level.txt
+drwxr-xr-x   0 piotr.suchon   (502) staff       (20)        0 2024-05-29 09:59:12.886067 utilsds-0.3.3/
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)     6230 2024-05-29 09:59:12.882530 utilsds-0.3.3/PKG-INFO
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)      627 2024-05-29 09:49:30.000000 utilsds-0.3.3/README.md
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)       38 2024-05-29 09:59:12.886132 utilsds-0.3.3/setup.cfg
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)     5405 2024-05-29 09:54:01.000000 utilsds-0.3.3/setup.py
+drwxr-xr-x   0 piotr.suchon   (502) staff       (20)        0 2024-05-29 09:59:12.875162 utilsds-0.3.3/utilsds/
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)        0 2024-05-29 09:49:30.000000 utilsds-0.3.3/utilsds/__init__.py
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)     2789 2024-05-29 09:49:30.000000 utilsds-0.3.3/utilsds/data_split.py
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)     1174 2024-05-29 09:49:30.000000 utilsds-0.3.3/utilsds/ds_statistics.py
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)    14396 2024-05-29 09:49:30.000000 utilsds-0.3.3/utilsds/model_experiments.py
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)     4659 2024-05-29 09:49:30.000000 utilsds-0.3.3/utilsds/transform_data.py
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)    12367 2024-05-29 09:49:30.000000 utilsds-0.3.3/utilsds/visualization.py
+drwxr-xr-x   0 piotr.suchon   (502) staff       (20)        0 2024-05-29 09:59:12.879036 utilsds-0.3.3/utilsds.egg-info/
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)     6230 2024-05-29 09:59:12.000000 utilsds-0.3.3/utilsds.egg-info/PKG-INFO
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)      319 2024-05-29 09:59:12.000000 utilsds-0.3.3/utilsds.egg-info/SOURCES.txt
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)        1 2024-05-29 09:59:12.000000 utilsds-0.3.3/utilsds.egg-info/dependency_links.txt
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)     2940 2024-05-29 09:59:12.000000 utilsds-0.3.3/utilsds.egg-info/requires.txt
+-rw-r--r--   0 piotr.suchon   (502) staff       (20)        8 2024-05-29 09:59:12.000000 utilsds-0.3.3/utilsds.egg-info/top_level.txt
```

### Comparing `utilsds-0.3.2/PKG-INFO` & `utilsds-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsds
-Version: 0.3.2
+Version: 0.3.3
 Summary: Solution for DS Team
 Author: DS Team
 Author-email: ds@sts.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -174,15 +174,15 @@
 Requires-Dist: wcwidth==0.2.13
 Requires-Dist: yarl==1.9.4
 Requires-Dist: yellowbrick==1.5
 Requires-Dist: zc.lockfile==3.0.post1
 
 # utilsds
 
-Utilsds is a library including classes and function used in ds project such as:
+Utilsds is a library that includes classes and function used in ds project such as:
 - data_split: 
     - train_validation_test_split
 - ds_statistics: 
     - test_kruskal_wallis
 - model_experiments: 
     - Modeling
 - transform_data:
```

### Comparing `utilsds-0.3.2/setup.py` & `utilsds-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('docs/ALTERNATIVE_README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='utilsds',
-    version='0.3.2',
+    version='0.3.3',
     packages=find_packages(),
     install_requires=[
         'aiohttp==3.9.5',
         'aiohttp-retry==2.8.3',
         'aiosignal==1.3.1',
         'amqp==5.2.0',
         'annotated-types==0.6.0',
```

### Comparing `utilsds-0.3.2/utilsds/data_split.py` & `utilsds-0.3.3/utilsds/data_split.py`

 * *Files identical despite different names*

### Comparing `utilsds-0.3.2/utilsds/ds_statistics.py` & `utilsds-0.3.3/utilsds/ds_statistics.py`

 * *Files identical despite different names*

### Comparing `utilsds-0.3.2/utilsds/model_experiments.py` & `utilsds-0.3.3/utilsds/model_experiments.py`

 * *Files identical despite different names*

### Comparing `utilsds-0.3.2/utilsds/transform_data.py` & `utilsds-0.3.3/utilsds/transform_data.py`

 * *Files identical despite different names*

### Comparing `utilsds-0.3.2/utilsds/visualization.py` & `utilsds-0.3.3/utilsds/visualization.py`

 * *Files identical despite different names*

### Comparing `utilsds-0.3.2/utilsds.egg-info/PKG-INFO` & `utilsds-0.3.3/utilsds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsds
-Version: 0.3.2
+Version: 0.3.3
 Summary: Solution for DS Team
 Author: DS Team
 Author-email: ds@sts.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -174,15 +174,15 @@
 Requires-Dist: wcwidth==0.2.13
 Requires-Dist: yarl==1.9.4
 Requires-Dist: yellowbrick==1.5
 Requires-Dist: zc.lockfile==3.0.post1
 
 # utilsds
 
-Utilsds is a library including classes and function used in ds project such as:
+Utilsds is a library that includes classes and function used in ds project such as:
 - data_split: 
     - train_validation_test_split
 - ds_statistics: 
     - test_kruskal_wallis
 - model_experiments: 
     - Modeling
 - transform_data:
```

### Comparing `utilsds-0.3.2/utilsds.egg-info/requires.txt` & `utilsds-0.3.3/utilsds.egg-info/requires.txt`

 * *Files identical despite different names*

