# Comparing `tmp/mcd_stitcher-0.1.3.tar.gz` & `tmp/mcd_stitcher-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcd_stitcher-0.1.3.tar", last modified: Fri May 24 17:35:31 2024, max compression
+gzip compressed data, was "mcd_stitcher-0.1.4.tar", last modified: Wed May 29 18:38:31 2024, max compression
```

## Comparing `mcd_stitcher-0.1.3.tar` & `mcd_stitcher-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:35:31.337997 mcd_stitcher-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-24 17:35:31.337997 mcd_stitcher-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:35:31.337997 mcd_stitcher-0.1.3/mcd_stitcher/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/mcd_stitcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/mcd_stitcher/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:35:31.337997 mcd_stitcher-0.1.3/mcd_stitcher/imclib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/mcd_stitcher/imclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/mcd_stitcher/imclib/imcdataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/mcd_stitcher/imclib/imcraw.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/mcd_stitcher/imclib/mcdmeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/mcd_stitcher/imclib/mcdutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/mcd_stitcher/imclib/mcdxmlparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/mcd_stitcher/imclib/metadefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/mcd_stitcher/stitcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:35:31.337997 mcd_stitcher-0.1.3/mcd_stitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-24 17:35:31.000000 mcd_stitcher-0.1.3/mcd_stitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-24 17:35:31.000000 mcd_stitcher-0.1.3/mcd_stitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:35:31.000000 mcd_stitcher-0.1.3/mcd_stitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-24 17:35:31.000000 mcd_stitcher-0.1.3/mcd_stitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-24 17:35:31.000000 mcd_stitcher-0.1.3/mcd_stitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 17:35:31.000000 mcd_stitcher-0.1.3/mcd_stitcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 17:35:31.337997 mcd_stitcher-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-24 17:35:21.000000 mcd_stitcher-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:38:31.183911 mcd_stitcher-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 18:38:31.183911 mcd_stitcher-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:38:31.179911 mcd_stitcher-0.1.4/mcd_stitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/mcd_stitcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/mcd_stitcher/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:38:31.183911 mcd_stitcher-0.1.4/mcd_stitcher/imclib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/mcd_stitcher/imclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/mcd_stitcher/imclib/imcdataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/mcd_stitcher/imclib/imcraw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/mcd_stitcher/imclib/mcdmeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/mcd_stitcher/imclib/mcdutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/mcd_stitcher/imclib/mcdxmlparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/mcd_stitcher/imclib/metadefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/mcd_stitcher/stitcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:38:31.183911 mcd_stitcher-0.1.4/mcd_stitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 18:38:31.000000 mcd_stitcher-0.1.4/mcd_stitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-29 18:38:31.000000 mcd_stitcher-0.1.4/mcd_stitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:38:31.000000 mcd_stitcher-0.1.4/mcd_stitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 18:38:31.000000 mcd_stitcher-0.1.4/mcd_stitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 18:38:31.000000 mcd_stitcher-0.1.4/mcd_stitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 18:38:31.000000 mcd_stitcher-0.1.4/mcd_stitcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 18:38:31.183911 mcd_stitcher-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-29 18:38:22.000000 mcd_stitcher-0.1.4/setup.py
```

### Comparing `mcd_stitcher-0.1.3/LICENSE` & `mcd_stitcher-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.3/PKG-INFO` & `mcd_stitcher-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcd_stitcher
-Version: 0.1.3
+Version: 0.1.4
 Summary: MCD to Zarr conversion and stitching
 Home-page: https://github.com/PawanChaurasia/mcd_stitcher
 Author: Pawan Chaurasia
 Author-email: pchaurasia98@gmail.com
 Project-URL: Bug Tracker, https://github.com/PawanChaurasia/mcd_stitcher/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,16 @@
 Requires-Dist: click
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: python_dateutil
 Requires-Dist: xarray
 Requires-Dist: zarr
 Requires-Dist: scikit-image
+Requires-Dist: xmltodict
+Requires-Dist: tifffile
 
 # MCD STITCHER
 
 Stitch rois from MCD files into OME-TIFFS.
 
 ## Install
```

### Comparing `mcd_stitcher-0.1.3/README.md` & `mcd_stitcher-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.3/mcd_stitcher/__init__.py` & `mcd_stitcher-0.1.4/mcd_stitcher/__init__.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.3/mcd_stitcher/converter.py` & `mcd_stitcher-0.1.4/mcd_stitcher/converter.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.3/mcd_stitcher/imclib/imcdataparser.py` & `mcd_stitcher-0.1.4/mcd_stitcher/imclib/imcdataparser.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.3/mcd_stitcher/imclib/imcraw.py` & `mcd_stitcher-0.1.4/mcd_stitcher/imclib/imcraw.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.3/mcd_stitcher/imclib/mcdmeta.py` & `mcd_stitcher-0.1.4/mcd_stitcher/imclib/mcdmeta.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.3/mcd_stitcher/imclib/mcdutils.py` & `mcd_stitcher-0.1.4/mcd_stitcher/imclib/mcdutils.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.3/mcd_stitcher/imclib/mcdxmlparser.py` & `mcd_stitcher-0.1.4/mcd_stitcher/imclib/mcdxmlparser.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.3/mcd_stitcher/imclib/metadefs.py` & `mcd_stitcher-0.1.4/mcd_stitcher/imclib/metadefs.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.3/mcd_stitcher.egg-info/PKG-INFO` & `mcd_stitcher-0.1.4/mcd_stitcher.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcd_stitcher
-Version: 0.1.3
+Version: 0.1.4
 Summary: MCD to Zarr conversion and stitching
 Home-page: https://github.com/PawanChaurasia/mcd_stitcher
 Author: Pawan Chaurasia
 Author-email: pchaurasia98@gmail.com
 Project-URL: Bug Tracker, https://github.com/PawanChaurasia/mcd_stitcher/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,16 @@
 Requires-Dist: click
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: python_dateutil
 Requires-Dist: xarray
 Requires-Dist: zarr
 Requires-Dist: scikit-image
+Requires-Dist: xmltodict
+Requires-Dist: tifffile
 
 # MCD STITCHER
 
 Stitch rois from MCD files into OME-TIFFS.
 
 ## Install
```

### Comparing `mcd_stitcher-0.1.3/mcd_stitcher.egg-info/SOURCES.txt` & `mcd_stitcher-0.1.4/mcd_stitcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.3/setup.py` & `mcd_stitcher-0.1.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mcd_stitcher',
-    version='0.1.3',
+    version='0.1.4',
     author='Pawan Chaurasia',
     author_email='pchaurasia98@gmail.com',
     description='MCD to Zarr conversion and stitching',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/PawanChaurasia/mcd_stitcher',
     project_urls={
@@ -22,15 +22,17 @@
     install_requires=[
         'click',
         'numpy',
         'pandas',
         'python_dateutil',
         'xarray',
         'zarr',
-        'scikit-image'
+        'scikit-image',
+        'xmltodict',
+        'tifffile'
     ],
     entry_points={
         'console_scripts': [
             'imc2zarr=mcd_stitcher.converter:main',
             'zarr_stitch=mcd_stitcher.stitcher:main',
             'mcd_stitch=mcd_stitcher:main',
         ],
```

