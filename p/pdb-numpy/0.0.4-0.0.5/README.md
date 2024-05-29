# Comparing `tmp/pdb_numpy-0.0.4.tar.gz` & `tmp/pdb_numpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdb_numpy-0.0.4.tar", last modified: Wed May 29 08:48:44 2024, max compression
+gzip compressed data, was "pdb_numpy-0.0.5.tar", last modified: Wed May 29 09:32:25 2024, max compression
```

## Comparing `pdb_numpy-0.0.4.tar` & `pdb_numpy-0.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:48:44.776464 pdb_numpy-0.0.4/
--rw-rw-r--   0 murail    (1000) murail    (1000)    18092 2023-11-03 13:13:10.000000 pdb_numpy-0.0.4/LICENSE
--rw-rw-r--   0 murail    (1000) murail    (1000)       32 2023-11-03 13:13:10.000000 pdb_numpy-0.0.4/MANIFEST.in
--rw-r--r--   0 murail    (1000) murail    (1000)     4501 2024-05-29 08:48:44.776464 pdb_numpy-0.0.4/PKG-INFO
--rw-rw-r--   0 murail    (1000) murail    (1000)     3301 2024-04-25 07:49:50.000000 pdb_numpy-0.0.4/README.rst
-drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:48:44.776464 pdb_numpy-0.0.4/pdb_numpy.egg-info/
--rw-r--r--   0 murail    (1000) murail    (1000)     4501 2024-05-29 08:48:44.000000 pdb_numpy-0.0.4/pdb_numpy.egg-info/PKG-INFO
--rw-rw-r--   0 murail    (1000) murail    (1000)      993 2024-05-29 08:48:44.000000 pdb_numpy-0.0.4/pdb_numpy.egg-info/SOURCES.txt
--rw-rw-r--   0 murail    (1000) murail    (1000)        1 2024-05-29 08:48:44.000000 pdb_numpy-0.0.4/pdb_numpy.egg-info/dependency_links.txt
--rw-rw-r--   0 murail    (1000) murail    (1000)       54 2024-05-29 08:48:44.000000 pdb_numpy-0.0.4/pdb_numpy.egg-info/entry_points.txt
--rw-rw-r--   0 murail    (1000) murail    (1000)        1 2024-05-29 08:48:44.000000 pdb_numpy-0.0.4/pdb_numpy.egg-info/not-zip-safe
--rw-rw-r--   0 murail    (1000) murail    (1000)       23 2024-05-29 08:48:44.000000 pdb_numpy-0.0.4/pdb_numpy.egg-info/requires.txt
--rw-rw-r--   0 murail    (1000) murail    (1000)       10 2024-05-29 08:48:44.000000 pdb_numpy-0.0.4/pdb_numpy.egg-info/top_level.txt
--rw-rw-r--   0 murail    (1000) murail    (1000)      477 2024-05-29 08:48:44.776464 pdb_numpy-0.0.4/setup.cfg
--rw-rw-r--   0 murail    (1000) murail    (1000)     2583 2024-05-29 08:46:18.000000 pdb_numpy-0.0.4/setup.py
-drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:48:44.772464 pdb_numpy-0.0.4/src/
-drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:48:44.776464 pdb_numpy-0.0.4/src/pdb_numpy/
--rw-rw-r--   0 murail    (1000) murail    (1000)    14010 2024-03-29 09:26:59.000000 pdb_numpy-0.0.4/src/pdb_numpy/DSSP.py
--rw-rw-r--   0 murail    (1000) murail    (1000)      792 2024-05-29 08:46:18.000000 pdb_numpy-0.0.4/src/pdb_numpy/__init__.py
--rw-rw-r--   0 murail    (1000) murail    (1000)    22870 2024-03-22 14:17:41.000000 pdb_numpy-0.0.4/src/pdb_numpy/abinitio.py
-drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:48:44.776464 pdb_numpy-0.0.4/src/pdb_numpy/alignement/
--rw-rw-r--   0 murail    (1000) murail    (1000)    21728 2024-05-29 08:00:38.000000 pdb_numpy-0.0.4/src/pdb_numpy/alignement/__init__.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     8766 2024-03-29 09:45:03.000000 pdb_numpy-0.0.4/src/pdb_numpy/alignement/align_cython.pyx
--rw-rw-r--   0 murail    (1000) murail    (1000)      741 2024-03-22 14:17:40.000000 pdb_numpy-0.0.4/src/pdb_numpy/alignement/profile_cython.py
--rw-rw-r--   0 murail    (1000) murail    (1000)    30170 2024-05-16 07:45:32.000000 pdb_numpy-0.0.4/src/pdb_numpy/analysis.py
--rw-rw-r--   0 murail    (1000) murail    (1000)    33499 2024-04-20 14:54:34.000000 pdb_numpy-0.0.4/src/pdb_numpy/coor.py
-drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:48:44.776464 pdb_numpy-0.0.4/src/pdb_numpy/data/
--rw-rw-r--   0 murail    (1000) murail    (1000)       40 2023-11-03 13:13:10.000000 pdb_numpy-0.0.4/src/pdb_numpy/data/__init__.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     1068 2024-03-22 14:17:40.000000 pdb_numpy-0.0.4/src/pdb_numpy/data/aa_dict.py
--rw-rw-r--   0 murail    (1000) murail    (1000)      619 2023-11-03 13:13:10.000000 pdb_numpy-0.0.4/src/pdb_numpy/data/blosum.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     2122 2023-11-03 13:13:10.000000 pdb_numpy-0.0.4/src/pdb_numpy/data/blosum62.txt
-drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:48:44.776464 pdb_numpy-0.0.4/src/pdb_numpy/format/
--rw-rw-r--   0 murail    (1000) murail    (1000)       43 2024-03-28 09:37:34.000000 pdb_numpy-0.0.4/src/pdb_numpy/format/__init__.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     5912 2024-03-22 14:17:40.000000 pdb_numpy-0.0.4/src/pdb_numpy/format/encode.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     7343 2024-03-28 22:02:39.000000 pdb_numpy-0.0.4/src/pdb_numpy/format/encode_cython.pyx
--rw-rw-r--   0 murail    (1000) murail    (1000)     5891 2024-03-29 11:06:23.000000 pdb_numpy-0.0.4/src/pdb_numpy/format/gro.py
--rw-rw-r--   0 murail    (1000) murail    (1000)    31473 2024-04-19 17:02:05.000000 pdb_numpy-0.0.4/src/pdb_numpy/format/mmcif.py
--rw-rw-r--   0 murail    (1000) murail    (1000)    14336 2024-03-29 12:36:43.000000 pdb_numpy-0.0.4/src/pdb_numpy/format/pdb.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     3732 2024-01-25 09:35:36.000000 pdb_numpy-0.0.4/src/pdb_numpy/format/pqr.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     1256 2024-03-29 08:57:14.000000 pdb_numpy-0.0.4/src/pdb_numpy/format/split_cython.pyx
--rw-rw-r--   0 murail    (1000) murail    (1000)    12556 2024-03-29 09:52:46.000000 pdb_numpy-0.0.4/src/pdb_numpy/geom.py
--rw-rw-r--   0 murail    (1000) murail    (1000)    16439 2024-04-23 11:49:48.000000 pdb_numpy-0.0.4/src/pdb_numpy/model.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     6288 2024-04-23 10:12:17.000000 pdb_numpy-0.0.4/src/pdb_numpy/select.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     7548 2024-03-22 14:17:40.000000 pdb_numpy-0.0.4/src/pdb_numpy/visu.py
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 09:32:25.892433 pdb_numpy-0.0.5/
+-rw-rw-r--   0 murail    (1000) murail    (1000)    18092 2023-11-03 13:13:10.000000 pdb_numpy-0.0.5/LICENSE
+-rw-rw-r--   0 murail    (1000) murail    (1000)       32 2023-11-03 13:13:10.000000 pdb_numpy-0.0.5/MANIFEST.in
+-rw-r--r--   0 murail    (1000) murail    (1000)     4501 2024-05-29 09:32:25.892433 pdb_numpy-0.0.5/PKG-INFO
+-rw-rw-r--   0 murail    (1000) murail    (1000)     3301 2024-04-25 07:49:50.000000 pdb_numpy-0.0.5/README.rst
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 09:32:25.892433 pdb_numpy-0.0.5/pdb_numpy.egg-info/
+-rw-r--r--   0 murail    (1000) murail    (1000)     4501 2024-05-29 09:32:25.000000 pdb_numpy-0.0.5/pdb_numpy.egg-info/PKG-INFO
+-rw-rw-r--   0 murail    (1000) murail    (1000)      993 2024-05-29 09:32:25.000000 pdb_numpy-0.0.5/pdb_numpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 murail    (1000) murail    (1000)        1 2024-05-29 09:32:25.000000 pdb_numpy-0.0.5/pdb_numpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 murail    (1000) murail    (1000)       54 2024-05-29 09:32:25.000000 pdb_numpy-0.0.5/pdb_numpy.egg-info/entry_points.txt
+-rw-rw-r--   0 murail    (1000) murail    (1000)        1 2024-05-29 09:32:25.000000 pdb_numpy-0.0.5/pdb_numpy.egg-info/not-zip-safe
+-rw-rw-r--   0 murail    (1000) murail    (1000)       23 2024-05-29 09:32:25.000000 pdb_numpy-0.0.5/pdb_numpy.egg-info/requires.txt
+-rw-rw-r--   0 murail    (1000) murail    (1000)       10 2024-05-29 09:32:25.000000 pdb_numpy-0.0.5/pdb_numpy.egg-info/top_level.txt
+-rw-rw-r--   0 murail    (1000) murail    (1000)      477 2024-05-29 09:32:25.892433 pdb_numpy-0.0.5/setup.cfg
+-rw-rw-r--   0 murail    (1000) murail    (1000)     2583 2024-05-29 09:31:02.000000 pdb_numpy-0.0.5/setup.py
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 09:32:25.888433 pdb_numpy-0.0.5/src/
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 09:32:25.892433 pdb_numpy-0.0.5/src/pdb_numpy/
+-rw-rw-r--   0 murail    (1000) murail    (1000)    14010 2024-03-29 09:26:59.000000 pdb_numpy-0.0.5/src/pdb_numpy/DSSP.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)      792 2024-05-29 09:31:02.000000 pdb_numpy-0.0.5/src/pdb_numpy/__init__.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)    22870 2024-03-22 14:17:41.000000 pdb_numpy-0.0.5/src/pdb_numpy/abinitio.py
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 09:32:25.892433 pdb_numpy-0.0.5/src/pdb_numpy/alignement/
+-rw-rw-r--   0 murail    (1000) murail    (1000)    21728 2024-05-29 08:00:38.000000 pdb_numpy-0.0.5/src/pdb_numpy/alignement/__init__.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     8766 2024-03-29 09:45:03.000000 pdb_numpy-0.0.5/src/pdb_numpy/alignement/align_cython.pyx
+-rw-rw-r--   0 murail    (1000) murail    (1000)      741 2024-03-22 14:17:40.000000 pdb_numpy-0.0.5/src/pdb_numpy/alignement/profile_cython.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)    30170 2024-05-16 07:45:32.000000 pdb_numpy-0.0.5/src/pdb_numpy/analysis.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)    33499 2024-04-20 14:54:34.000000 pdb_numpy-0.0.5/src/pdb_numpy/coor.py
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 09:32:25.892433 pdb_numpy-0.0.5/src/pdb_numpy/data/
+-rw-rw-r--   0 murail    (1000) murail    (1000)       40 2023-11-03 13:13:10.000000 pdb_numpy-0.0.5/src/pdb_numpy/data/__init__.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     1068 2024-03-22 14:17:40.000000 pdb_numpy-0.0.5/src/pdb_numpy/data/aa_dict.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)      619 2023-11-03 13:13:10.000000 pdb_numpy-0.0.5/src/pdb_numpy/data/blosum.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     2122 2023-11-03 13:13:10.000000 pdb_numpy-0.0.5/src/pdb_numpy/data/blosum62.txt
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 09:32:25.892433 pdb_numpy-0.0.5/src/pdb_numpy/format/
+-rw-rw-r--   0 murail    (1000) murail    (1000)       43 2024-03-28 09:37:34.000000 pdb_numpy-0.0.5/src/pdb_numpy/format/__init__.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     5912 2024-03-22 14:17:40.000000 pdb_numpy-0.0.5/src/pdb_numpy/format/encode.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     7343 2024-03-28 22:02:39.000000 pdb_numpy-0.0.5/src/pdb_numpy/format/encode_cython.pyx
+-rw-rw-r--   0 murail    (1000) murail    (1000)     5891 2024-03-29 11:06:23.000000 pdb_numpy-0.0.5/src/pdb_numpy/format/gro.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)    31473 2024-04-19 17:02:05.000000 pdb_numpy-0.0.5/src/pdb_numpy/format/mmcif.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)    14336 2024-03-29 12:36:43.000000 pdb_numpy-0.0.5/src/pdb_numpy/format/pdb.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     3732 2024-01-25 09:35:36.000000 pdb_numpy-0.0.5/src/pdb_numpy/format/pqr.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     1256 2024-03-29 08:57:14.000000 pdb_numpy-0.0.5/src/pdb_numpy/format/split_cython.pyx
+-rw-rw-r--   0 murail    (1000) murail    (1000)    12556 2024-03-29 09:52:46.000000 pdb_numpy-0.0.5/src/pdb_numpy/geom.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)    16439 2024-04-23 11:49:48.000000 pdb_numpy-0.0.5/src/pdb_numpy/model.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     6288 2024-04-23 10:12:17.000000 pdb_numpy-0.0.5/src/pdb_numpy/select.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     7548 2024-03-22 14:17:40.000000 pdb_numpy-0.0.5/src/pdb_numpy/visu.py
```

### Comparing `pdb_numpy-0.0.4/LICENSE` & `pdb_numpy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/PKG-INFO` & `pdb_numpy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdb_numpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pdb_Numpy is a python library allowing simple operations on pdb coor files.
 Home-page: https://github.com/samuelmurail/pdb_numpy
 Author: Samuel Murail
 Author-email: samuel.murail@u-paris.fr
 License: GNUv2.0
 Keywords: pdb_numpy,Python,PDB,Numpy,Coor,Model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pdb_numpy-0.0.4/README.rst` & `pdb_numpy-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/pdb_numpy.egg-info/PKG-INFO` & `pdb_numpy-0.0.5/pdb_numpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pdb-numpy
-Version: 0.0.4
+Name: pdb_numpy
+Version: 0.0.5
 Summary: Pdb_Numpy is a python library allowing simple operations on pdb coor files.
 Home-page: https://github.com/samuelmurail/pdb_numpy
 Author: Samuel Murail
 Author-email: samuel.murail@u-paris.fr
 License: GNUv2.0
 Keywords: pdb_numpy,Python,PDB,Numpy,Coor,Model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pdb_numpy-0.0.4/pdb_numpy.egg-info/SOURCES.txt` & `pdb_numpy-0.0.5/pdb_numpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/setup.py` & `pdb_numpy-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
 from setuptools import setup
 from distutils.extension import Extension
 
-version="0.0.4"
+version="0.0.5"
 
 with open('README.rst', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 ext_modules = [
     Extension(
         name="pdb_numpy.alignement.align_cython",
```

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/DSSP.py` & `pdb_numpy-0.0.5/src/pdb_numpy/DSSP.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/__init__.py` & `pdb_numpy-0.0.5/src/pdb_numpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 
 # Autorship information
 __author__ = "Samuel Murail"
 __copyright__ = "Copyright 2022, RPBS"
 __credits__ = ["Samuel Murail"]
 __license__ = "GNU General Public License v2.0"
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 __maintainer__ = "Samuel Murail"
 __email__ = "samuel.murail@u-paris.fr"
 __status__ = "Beta"
 
 # Logging
 logger = logging.getLogger(__name__)
```

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/abinitio.py` & `pdb_numpy-0.0.5/src/pdb_numpy/abinitio.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/alignement/__init__.py` & `pdb_numpy-0.0.5/src/pdb_numpy/alignement/__init__.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/alignement/align_cython.pyx` & `pdb_numpy-0.0.5/src/pdb_numpy/alignement/align_cython.pyx`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/alignement/profile_cython.py` & `pdb_numpy-0.0.5/src/pdb_numpy/alignement/profile_cython.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/analysis.py` & `pdb_numpy-0.0.5/src/pdb_numpy/analysis.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/coor.py` & `pdb_numpy-0.0.5/src/pdb_numpy/coor.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/data/aa_dict.py` & `pdb_numpy-0.0.5/src/pdb_numpy/data/aa_dict.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/data/blosum.py` & `pdb_numpy-0.0.5/src/pdb_numpy/data/blosum.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/data/blosum62.txt` & `pdb_numpy-0.0.5/src/pdb_numpy/data/blosum62.txt`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/format/encode.py` & `pdb_numpy-0.0.5/src/pdb_numpy/format/encode.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/format/encode_cython.pyx` & `pdb_numpy-0.0.5/src/pdb_numpy/format/encode_cython.pyx`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/format/gro.py` & `pdb_numpy-0.0.5/src/pdb_numpy/format/gro.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/format/mmcif.py` & `pdb_numpy-0.0.5/src/pdb_numpy/format/mmcif.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/format/pdb.py` & `pdb_numpy-0.0.5/src/pdb_numpy/format/pdb.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/format/pqr.py` & `pdb_numpy-0.0.5/src/pdb_numpy/format/pqr.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/format/split_cython.pyx` & `pdb_numpy-0.0.5/src/pdb_numpy/format/split_cython.pyx`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/geom.py` & `pdb_numpy-0.0.5/src/pdb_numpy/geom.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/model.py` & `pdb_numpy-0.0.5/src/pdb_numpy/model.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/select.py` & `pdb_numpy-0.0.5/src/pdb_numpy/select.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.4/src/pdb_numpy/visu.py` & `pdb_numpy-0.0.5/src/pdb_numpy/visu.py`

 * *Files identical despite different names*

