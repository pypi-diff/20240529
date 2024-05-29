# Comparing `tmp/hammingencoder-0.1.4.tar.gz` & `tmp/hammingencoder-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hammingencoder-0.1.4.tar", last modified: Wed May 29 16:54:07 2024, max compression
+gzip compressed data, was "hammingencoder-0.1.5.tar", last modified: Wed May 29 17:02:18 2024, max compression
```

## Comparing `hammingencoder-0.1.4.tar` & `hammingencoder-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 16:54:07.506065 hammingencoder-0.1.4/
-drwxrwxrwx   0        0        0        0 2024-05-29 16:54:07.491062 hammingencoder-0.1.4/HammingEncoder/
--rw-rw-rw-   0        0        0    10003 2024-05-29 14:53:08.000000 hammingencoder-0.1.4/HammingEncoder/HammingEncoder.py
--rw-rw-rw-   0        0        0       74 2024-05-29 14:54:44.000000 hammingencoder-0.1.4/HammingEncoder/__init__.py
--rw-rw-rw-   0        0        0     1670 2024-05-29 14:53:05.000000 hammingencoder-0.1.4/HammingEncoder/data_generator.py
--rw-rw-rw-   0        0        0     1500 2024-05-29 14:42:22.000000 hammingencoder-0.1.4/HammingEncoder/test.py
--rw-rw-rw-   0        0        0     4430 2024-05-29 14:53:04.000000 hammingencoder-0.1.4/HammingEncoder/train_function.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:54:07.503073 hammingencoder-0.1.4/HammingEncoder.egg-info/
--rw-rw-rw-   0        0        0     1756 2024-05-29 16:54:07.000000 hammingencoder-0.1.4/HammingEncoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-05-29 16:54:07.000000 hammingencoder-0.1.4/HammingEncoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 16:54:07.000000 hammingencoder-0.1.4/HammingEncoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-29 16:54:07.000000 hammingencoder-0.1.4/HammingEncoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-29 16:54:07.000000 hammingencoder-0.1.4/HammingEncoder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1756 2024-05-29 16:54:07.505067 hammingencoder-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1676 2024-05-29 16:49:27.000000 hammingencoder-0.1.4/README.rst
--rw-rw-rw-   0        0        0       42 2024-05-29 16:54:07.506065 hammingencoder-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      750 2024-05-29 16:52:48.000000 hammingencoder-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:02:18.959344 hammingencoder-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-05-29 17:02:18.940800 hammingencoder-0.1.5/HammingEncoder/
+-rw-rw-rw-   0        0        0    10003 2024-05-29 14:53:08.000000 hammingencoder-0.1.5/HammingEncoder/HammingEncoder.py
+-rw-rw-rw-   0        0        0       74 2024-05-29 14:54:44.000000 hammingencoder-0.1.5/HammingEncoder/__init__.py
+-rw-rw-rw-   0        0        0     1670 2024-05-29 14:53:05.000000 hammingencoder-0.1.5/HammingEncoder/data_generator.py
+-rw-rw-rw-   0        0        0     1500 2024-05-29 14:42:22.000000 hammingencoder-0.1.5/HammingEncoder/test.py
+-rw-rw-rw-   0        0        0     4430 2024-05-29 14:53:04.000000 hammingencoder-0.1.5/HammingEncoder/train_function.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:02:18.957349 hammingencoder-0.1.5/HammingEncoder.egg-info/
+-rw-rw-rw-   0        0        0     1655 2024-05-29 17:02:18.000000 hammingencoder-0.1.5/HammingEncoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2024-05-29 17:02:18.000000 hammingencoder-0.1.5/HammingEncoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 17:02:18.000000 hammingencoder-0.1.5/HammingEncoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-29 17:02:18.000000 hammingencoder-0.1.5/HammingEncoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-29 17:02:18.000000 hammingencoder-0.1.5/HammingEncoder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1655 2024-05-29 17:02:18.958346 hammingencoder-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1676 2024-05-29 16:49:27.000000 hammingencoder-0.1.5/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-29 17:02:18.960343 hammingencoder-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      750 2024-05-29 17:02:13.000000 hammingencoder-0.1.5/setup.py
```

### Comparing `hammingencoder-0.1.4/HammingEncoder/HammingEncoder.py` & `hammingencoder-0.1.5/HammingEncoder/HammingEncoder.py`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.4/HammingEncoder/data_generator.py` & `hammingencoder-0.1.5/HammingEncoder/data_generator.py`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.4/HammingEncoder/test.py` & `hammingencoder-0.1.5/HammingEncoder/test.py`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.4/HammingEncoder/train_function.py` & `hammingencoder-0.1.5/HammingEncoder/train_function.py`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.4/HammingEncoder.egg-info/PKG-INFO` & `hammingencoder-0.1.5/HammingEncoder.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HammingEncoder
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Hamming Encoder package
 Home-page: https://github.com/jd445/HammingEncoder
 Author: Junjie Dong
 Author-email: jd445@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,14 @@
 
 # Example data
 sequences = [
     ['0', '1', '2', '3', '4', '5', '1', '6', '5', '1', '7', '4', '5', '8', '5'], 
     ['0', '1', '4', '2', '3', '4', '5', '8', '5', '1', '7', '4', '5', '1', '5', '1', '5', '6', '5'],
     ['0', '1', '2', '3', '4', '5', '8', '5', '1', '5', '7', '5', '1', '8', '5', '1', '5', '1', '5', '1', '6', '4', '5'], 
     ['0', '4', '2', '3', '5', '7', '5', '1', '5', '4', '6', '5', '1', '5', '4', '5'],
-    ['4', '5', '4', '0', '1', '4', '2', '3', '5', '7', '5', '4', '5', '1', '5', '8', '5', '1', '5']
     ]
 labels = [0, 1, 0, 1]
 
 # Initialize the encoder
 encoder = HammingEncoder(sequences, labels, gap_constrain=5, label_number=2, Preset_set_pattern_num=1024)
 
 # Fit the model
```

### Comparing `hammingencoder-0.1.4/PKG-INFO` & `hammingencoder-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HammingEncoder
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Hamming Encoder package
 Home-page: https://github.com/jd445/HammingEncoder
 Author: Junjie Dong
 Author-email: jd445@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,14 @@
 
 # Example data
 sequences = [
     ['0', '1', '2', '3', '4', '5', '1', '6', '5', '1', '7', '4', '5', '8', '5'], 
     ['0', '1', '4', '2', '3', '4', '5', '8', '5', '1', '7', '4', '5', '1', '5', '1', '5', '6', '5'],
     ['0', '1', '2', '3', '4', '5', '8', '5', '1', '5', '7', '5', '1', '8', '5', '1', '5', '1', '5', '1', '6', '4', '5'], 
     ['0', '4', '2', '3', '5', '7', '5', '1', '5', '4', '6', '5', '1', '5', '4', '5'],
-    ['4', '5', '4', '0', '1', '4', '2', '3', '5', '7', '5', '4', '5', '1', '5', '8', '5', '1', '5']
     ]
 labels = [0, 1, 0, 1]
 
 # Initialize the encoder
 encoder = HammingEncoder(sequences, labels, gap_constrain=5, label_number=2, Preset_set_pattern_num=1024)
 
 # Fit the model
```

### Comparing `hammingencoder-0.1.4/README.rst` & `hammingencoder-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.4/setup.py` & `hammingencoder-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='HammingEncoder',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'torch',
         'scikit-learn',
         'pandas',
         'tqdm'
```

