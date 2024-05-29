# Comparing `tmp/argendolar-1.1.2.tar.gz` & `tmp/argendolar-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argendolar-1.1.2.tar", last modified: Tue May 28 16:03:05 2024, max compression
+gzip compressed data, was "argendolar-2.0.0.tar", last modified: Wed May 29 14:56:14 2024, max compression
```

## Comparing `argendolar-1.1.2.tar` & `argendolar-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 16:03:05.084296 argendolar-1.1.2/
--rw-r--r--   0 mgobea   (1218917679) 1010544492     1062 2024-05-22 19:14:04.000000 argendolar-1.1.2/LICENSE
--rw-r--r--   0 mgobea   (1218917679) 1010544492     4634 2024-05-28 16:03:05.084045 argendolar-1.1.2/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492     3950 2024-05-28 15:34:50.000000 argendolar-1.1.2/README.md
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 16:03:05.082071 argendolar-1.1.2/argendolar/
--rw-r--r--   0 mgobea   (1218917679) 1010544492      114 2024-05-28 14:29:08.000000 argendolar-1.1.2/argendolar/__init__.py
--rw-r--r--   0 mgobea   (1218917679) 1010544492     6351 2024-05-28 14:58:58.000000 argendolar-1.1.2/argendolar/argendolar.py
--rw-r--r--   0 mgobea   (1218917679) 1010544492      225 2024-05-28 12:42:16.000000 argendolar-1.1.2/argendolar/tipo_dolares.py
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-28 16:03:05.083696 argendolar-1.1.2/argendolar.egg-info/
--rw-r--r--   0 mgobea   (1218917679) 1010544492     4634 2024-05-28 16:03:05.000000 argendolar-1.1.2/argendolar.egg-info/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492      270 2024-05-28 16:03:05.000000 argendolar-1.1.2/argendolar.egg-info/SOURCES.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-28 16:03:05.000000 argendolar-1.1.2/argendolar.egg-info/dependency_links.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       16 2024-05-28 16:03:05.000000 argendolar-1.1.2/argendolar.egg-info/requires.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       11 2024-05-28 16:03:05.000000 argendolar-1.1.2/argendolar.egg-info/top_level.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-28 16:03:05.084353 argendolar-1.1.2/setup.cfg
--rw-r--r--   0 mgobea   (1218917679) 1010544492     1030 2024-05-28 16:02:50.000000 argendolar-1.1.2/setup.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 14:56:14.917853 argendolar-2.0.0/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     1062 2024-05-22 19:14:04.000000 argendolar-2.0.0/LICENSE
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     4634 2024-05-29 14:56:14.917602 argendolar-2.0.0/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     3950 2024-05-28 15:34:50.000000 argendolar-2.0.0/README.md
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 14:56:14.915513 argendolar-2.0.0/argendolar/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      114 2024-05-28 14:29:08.000000 argendolar-2.0.0/argendolar/__init__.py
+-rw-r--r--   0 mgobea   (1218917679) 1010544492    11169 2024-05-29 14:52:59.000000 argendolar-2.0.0/argendolar/argendolar.py
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      225 2024-05-28 12:42:16.000000 argendolar-2.0.0/argendolar/tipo_dolares.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-29 14:56:14.917251 argendolar-2.0.0/argendolar.egg-info/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     4634 2024-05-29 14:56:14.000000 argendolar-2.0.0/argendolar.egg-info/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      270 2024-05-29 14:56:14.000000 argendolar-2.0.0/argendolar.egg-info/SOURCES.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-29 14:56:14.000000 argendolar-2.0.0/argendolar.egg-info/dependency_links.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       16 2024-05-29 14:56:14.000000 argendolar-2.0.0/argendolar.egg-info/requires.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       11 2024-05-29 14:56:14.000000 argendolar-2.0.0/argendolar.egg-info/top_level.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-29 14:56:14.917924 argendolar-2.0.0/setup.cfg
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     1030 2024-05-29 14:53:49.000000 argendolar-2.0.0/setup.py
```

### Comparing `argendolar-1.1.2/LICENSE` & `argendolar-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `argendolar-1.1.2/PKG-INFO` & `argendolar-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argendolar
-Version: 1.1.2
+Version: 2.0.0
 Summary: A package to get the exchange rates of the different types of dollars and others currencies in Argentina.
 Home-page: https://github.com/Mgobeaalcoba/argendolar
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `argendolar-1.1.2/README.md` & `argendolar-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `argendolar-1.1.2/argendolar.egg-info/PKG-INFO` & `argendolar-2.0.0/argendolar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argendolar
-Version: 1.1.2
+Version: 2.0.0
 Summary: A package to get the exchange rates of the different types of dollars and others currencies in Argentina.
 Home-page: https://github.com/Mgobeaalcoba/argendolar
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `argendolar-1.1.2/setup.py` & `argendolar-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='argendolar',
-    version='1.1.2',
+    version='2.0.0',
     packages=find_packages(),
     install_requires=['pandas', 'requests'],
     author='Mariano Gobea Alcoba',
     author_email='gobeamariano@gmail.com',
     description='A package to get the exchange rates of the different types of dollars and others currencies in Argentina.',
     long_description=long_description,  # Usa el contenido del README.md como descripción larga
     long_description_content_type="text/markdown",  # Especifica el tipo de contenido como markdown
```

