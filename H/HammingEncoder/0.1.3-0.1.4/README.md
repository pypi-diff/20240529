# Comparing `tmp/hammingencoder-0.1.3.tar.gz` & `tmp/hammingencoder-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hammingencoder-0.1.3.tar", last modified: Wed May 29 16:40:34 2024, max compression
+gzip compressed data, was "hammingencoder-0.1.4.tar", last modified: Wed May 29 16:54:07 2024, max compression
```

## Comparing `hammingencoder-0.1.3.tar` & `hammingencoder-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 16:40:34.040068 hammingencoder-0.1.3/
-drwxrwxrwx   0        0        0        0 2024-05-29 16:40:34.023136 hammingencoder-0.1.3/HammingEncoder/
--rw-rw-rw-   0        0        0    10003 2024-05-29 14:53:08.000000 hammingencoder-0.1.3/HammingEncoder/HammingEncoder.py
--rw-rw-rw-   0        0        0       74 2024-05-29 14:54:44.000000 hammingencoder-0.1.3/HammingEncoder/__init__.py
--rw-rw-rw-   0        0        0     1670 2024-05-29 14:53:05.000000 hammingencoder-0.1.3/HammingEncoder/data_generator.py
--rw-rw-rw-   0        0        0     1500 2024-05-29 14:42:22.000000 hammingencoder-0.1.3/HammingEncoder/test.py
--rw-rw-rw-   0        0        0     4430 2024-05-29 14:53:04.000000 hammingencoder-0.1.3/HammingEncoder/train_function.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:40:34.038073 hammingencoder-0.1.3/HammingEncoder.egg-info/
--rw-rw-rw-   0        0        0      464 2024-05-29 16:40:33.000000 hammingencoder-0.1.3/HammingEncoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-05-29 16:40:33.000000 hammingencoder-0.1.3/HammingEncoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 16:40:33.000000 hammingencoder-0.1.3/HammingEncoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-29 16:40:33.000000 hammingencoder-0.1.3/HammingEncoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-29 16:40:33.000000 hammingencoder-0.1.3/HammingEncoder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      464 2024-05-29 16:40:34.039071 hammingencoder-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-29 16:40:34.040068 hammingencoder-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      599 2024-05-29 16:40:26.000000 hammingencoder-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:54:07.506065 hammingencoder-0.1.4/
+drwxrwxrwx   0        0        0        0 2024-05-29 16:54:07.491062 hammingencoder-0.1.4/HammingEncoder/
+-rw-rw-rw-   0        0        0    10003 2024-05-29 14:53:08.000000 hammingencoder-0.1.4/HammingEncoder/HammingEncoder.py
+-rw-rw-rw-   0        0        0       74 2024-05-29 14:54:44.000000 hammingencoder-0.1.4/HammingEncoder/__init__.py
+-rw-rw-rw-   0        0        0     1670 2024-05-29 14:53:05.000000 hammingencoder-0.1.4/HammingEncoder/data_generator.py
+-rw-rw-rw-   0        0        0     1500 2024-05-29 14:42:22.000000 hammingencoder-0.1.4/HammingEncoder/test.py
+-rw-rw-rw-   0        0        0     4430 2024-05-29 14:53:04.000000 hammingencoder-0.1.4/HammingEncoder/train_function.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:54:07.503073 hammingencoder-0.1.4/HammingEncoder.egg-info/
+-rw-rw-rw-   0        0        0     1756 2024-05-29 16:54:07.000000 hammingencoder-0.1.4/HammingEncoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2024-05-29 16:54:07.000000 hammingencoder-0.1.4/HammingEncoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 16:54:07.000000 hammingencoder-0.1.4/HammingEncoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-29 16:54:07.000000 hammingencoder-0.1.4/HammingEncoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-29 16:54:07.000000 hammingencoder-0.1.4/HammingEncoder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1756 2024-05-29 16:54:07.505067 hammingencoder-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1676 2024-05-29 16:49:27.000000 hammingencoder-0.1.4/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-29 16:54:07.506065 hammingencoder-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      750 2024-05-29 16:52:48.000000 hammingencoder-0.1.4/setup.py
```

### Comparing `hammingencoder-0.1.3/HammingEncoder/HammingEncoder.py` & `hammingencoder-0.1.4/HammingEncoder/HammingEncoder.py`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.3/HammingEncoder/data_generator.py` & `hammingencoder-0.1.4/HammingEncoder/data_generator.py`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.3/HammingEncoder/test.py` & `hammingencoder-0.1.4/HammingEncoder/test.py`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.3/HammingEncoder/train_function.py` & `hammingencoder-0.1.4/HammingEncoder/train_function.py`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.3/setup.py` & `hammingencoder-0.1.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='HammingEncoder',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'torch',
         'scikit-learn',
         'pandas',
         'tqdm'
     ],
+    description='A Hamming Encoder package',
+    long_description=open('README.md').read(),
+    # long_description_content_type='text/x-rst',
+    long_description_content_type='text/markdown',
     author='Junjie Dong',
     author_email='jd445@qq.com',
-    description='A Hamming Encoder package',
     url='https://github.com/jd445/HammingEncoder',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

