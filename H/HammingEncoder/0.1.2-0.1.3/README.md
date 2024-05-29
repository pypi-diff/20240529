# Comparing `tmp/hammingencoder-0.1.2.tar.gz` & `tmp/hammingencoder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hammingencoder-0.1.2.tar", last modified: Wed May 29 16:27:17 2024, max compression
+gzip compressed data, was "hammingencoder-0.1.3.tar", last modified: Wed May 29 16:40:34 2024, max compression
```

## Comparing `hammingencoder-0.1.2.tar` & `hammingencoder-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 16:27:17.262152 hammingencoder-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-05-29 16:27:17.245198 hammingencoder-0.1.2/HammingEncoder/
--rw-rw-rw-   0        0        0    10003 2024-05-29 14:53:08.000000 hammingencoder-0.1.2/HammingEncoder/HammingEncoder.py
--rw-rw-rw-   0        0        0       74 2024-05-29 14:54:44.000000 hammingencoder-0.1.2/HammingEncoder/__init__.py
--rw-rw-rw-   0        0        0     1670 2024-05-29 14:53:05.000000 hammingencoder-0.1.2/HammingEncoder/data_generator.py
--rw-rw-rw-   0        0        0     1500 2024-05-29 14:42:22.000000 hammingencoder-0.1.2/HammingEncoder/test.py
--rw-rw-rw-   0        0        0     4430 2024-05-29 14:53:04.000000 hammingencoder-0.1.2/HammingEncoder/train_function.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:27:17.260157 hammingencoder-0.1.2/HammingEncoder.egg-info/
--rw-rw-rw-   0        0        0      464 2024-05-29 16:27:17.000000 hammingencoder-0.1.2/HammingEncoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-05-29 16:27:17.000000 hammingencoder-0.1.2/HammingEncoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 16:27:17.000000 hammingencoder-0.1.2/HammingEncoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-29 16:27:17.000000 hammingencoder-0.1.2/HammingEncoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-29 16:27:17.000000 hammingencoder-0.1.2/HammingEncoder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      464 2024-05-29 16:27:17.261155 hammingencoder-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-29 16:27:17.262152 hammingencoder-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      599 2024-05-29 16:27:15.000000 hammingencoder-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:40:34.040068 hammingencoder-0.1.3/
+drwxrwxrwx   0        0        0        0 2024-05-29 16:40:34.023136 hammingencoder-0.1.3/HammingEncoder/
+-rw-rw-rw-   0        0        0    10003 2024-05-29 14:53:08.000000 hammingencoder-0.1.3/HammingEncoder/HammingEncoder.py
+-rw-rw-rw-   0        0        0       74 2024-05-29 14:54:44.000000 hammingencoder-0.1.3/HammingEncoder/__init__.py
+-rw-rw-rw-   0        0        0     1670 2024-05-29 14:53:05.000000 hammingencoder-0.1.3/HammingEncoder/data_generator.py
+-rw-rw-rw-   0        0        0     1500 2024-05-29 14:42:22.000000 hammingencoder-0.1.3/HammingEncoder/test.py
+-rw-rw-rw-   0        0        0     4430 2024-05-29 14:53:04.000000 hammingencoder-0.1.3/HammingEncoder/train_function.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:40:34.038073 hammingencoder-0.1.3/HammingEncoder.egg-info/
+-rw-rw-rw-   0        0        0      464 2024-05-29 16:40:33.000000 hammingencoder-0.1.3/HammingEncoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-05-29 16:40:33.000000 hammingencoder-0.1.3/HammingEncoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 16:40:33.000000 hammingencoder-0.1.3/HammingEncoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-29 16:40:33.000000 hammingencoder-0.1.3/HammingEncoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-29 16:40:33.000000 hammingencoder-0.1.3/HammingEncoder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      464 2024-05-29 16:40:34.039071 hammingencoder-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-29 16:40:34.040068 hammingencoder-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      599 2024-05-29 16:40:26.000000 hammingencoder-0.1.3/setup.py
```

### Comparing `hammingencoder-0.1.2/HammingEncoder/HammingEncoder.py` & `hammingencoder-0.1.3/HammingEncoder/HammingEncoder.py`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.2/HammingEncoder/data_generator.py` & `hammingencoder-0.1.3/HammingEncoder/data_generator.py`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.2/HammingEncoder/test.py` & `hammingencoder-0.1.3/HammingEncoder/test.py`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.2/HammingEncoder/train_function.py` & `hammingencoder-0.1.3/HammingEncoder/train_function.py`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.2/setup.py` & `hammingencoder-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='HammingEncoder',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'torch',
         'scikit-learn',
         'pandas',
         'tqdm'
```

