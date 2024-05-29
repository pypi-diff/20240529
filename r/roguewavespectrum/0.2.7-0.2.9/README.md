# Comparing `tmp/roguewavespectrum-0.2.7.tar.gz` & `tmp/roguewavespectrum-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roguewavespectrum-0.2.7.tar", last modified: Mon Apr 15 22:38:01 2024, max compression
+gzip compressed data, was "roguewavespectrum-0.2.9.tar", last modified: Mon May 27 23:25:16 2024, max compression
```

## Comparing `roguewavespectrum-0.2.7.tar` & `roguewavespectrum-0.2.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.088642 roguewavespectrum-0.2.7/
--rw-r--r--   0 pietersmit   (502) staff       (20)    11357 2023-08-20 18:47:38.000000 roguewavespectrum-0.2.7/LICENSE
--rw-r--r--   0 pietersmit   (502) staff       (20)      947 2024-04-15 22:38:01.088504 roguewavespectrum-0.2.7/PKG-INFO
--rw-r--r--   0 pietersmit   (502) staff       (20)      288 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.7/README.md
--rw-r--r--   0 pietersmit   (502) staff       (20)       38 2024-04-15 22:38:01.088682 roguewavespectrum-0.2.7/setup.cfg
--rw-r--r--   0 pietersmit   (502) staff       (20)     1350 2024-04-15 22:37:35.000000 roguewavespectrum-0.2.7/setup.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.077732 roguewavespectrum-0.2.7/src/
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.082438 roguewavespectrum-0.2.7/src/roguewavespectrum/
--rw-r--r--   0 pietersmit   (502) staff       (20)    17787 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/__init__.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     4306 2023-10-21 02:34:11.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_directions.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.084590 roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/
--rw-r--r--   0 pietersmit   (502) staff       (20)      658 2023-10-21 02:24:56.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/__init__.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     4697 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/estimate.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3862 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/mem.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    28728 2023-11-27 00:48:14.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/mem2.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    16922 2024-04-15 22:37:17.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_factory_methods.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     1432 2024-01-23 21:48:48.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_geospatial.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3275 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_operations.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    16190 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_partitioning.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3902 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_physical_constants.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    79503 2024-03-26 23:59:44.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_spectrum.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    21216 2023-11-27 00:51:17.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_spline_interpolation.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3514 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_time.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     2922 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_timeseries.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    16274 2023-11-27 00:51:17.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_variable_names.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    27327 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/parametric.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.086314 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/
--rw-r--r--   0 pietersmit   (502) staff       (20)     5066 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/__init__.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     9651 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_extrapolate_tail.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3802 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_post_processing.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     2762 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_sdcard_data.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    12122 2024-01-20 00:31:36.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_time_integration.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    16780 2024-01-23 21:48:48.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_wavefleet_api.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.083519 roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/
--rw-r--r--   0 pietersmit   (502) staff       (20)      947 2024-04-15 22:38:01.000000 roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/PKG-INFO
--rw-r--r--   0 pietersmit   (502) staff       (20)     1398 2024-04-15 22:38:01.000000 roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/SOURCES.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)        1 2024-04-15 22:38:01.000000 roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/dependency_links.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)      129 2024-04-15 22:38:01.000000 roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/requires.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)       18 2024-04-15 22:38:01.000000 roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/top_level.txt
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.088194 roguewavespectrum-0.2.7/test/
--rw-r--r--   0 pietersmit   (502) staff       (20)     1776 2023-10-27 21:23:45.000000 roguewavespectrum-0.2.7/test/test_directions.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     8227 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.7/test/test_factory_methods.py
--rw-r--r--   0 pietersmit   (502) staff       (20)      876 2024-02-28 21:55:38.000000 roguewavespectrum-0.2.7/test/test_geospatial.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     2188 2023-10-21 21:15:35.000000 roguewavespectrum-0.2.7/test/test_parametric.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    19854 2024-03-27 00:02:22.000000 roguewavespectrum-0.2.7/test/test_spectrum.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3820 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.7/test/test_timeseries.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-05-27 23:25:16.666024 roguewavespectrum-0.2.9/
+-rw-r--r--   0 pietersmit   (502) staff       (20)    11357 2023-08-20 18:47:38.000000 roguewavespectrum-0.2.9/LICENSE
+-rw-r--r--   0 pietersmit   (502) staff       (20)      947 2024-05-27 23:25:16.665879 roguewavespectrum-0.2.9/PKG-INFO
+-rw-r--r--   0 pietersmit   (502) staff       (20)      288 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.9/README.md
+-rw-r--r--   0 pietersmit   (502) staff       (20)       38 2024-05-27 23:25:16.666065 roguewavespectrum-0.2.9/setup.cfg
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1350 2024-05-27 22:24:46.000000 roguewavespectrum-0.2.9/setup.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-05-27 23:25:16.659436 roguewavespectrum-0.2.9/src/
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-05-27 23:25:16.662265 roguewavespectrum-0.2.9/src/roguewavespectrum/
+-rw-r--r--   0 pietersmit   (502) staff       (20)    17788 2024-04-16 20:30:13.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/__init__.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     4306 2023-10-21 02:34:11.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_directions.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-05-27 23:25:16.663857 roguewavespectrum-0.2.9/src/roguewavespectrum/_estimators/
+-rw-r--r--   0 pietersmit   (502) staff       (20)      658 2023-10-21 02:24:56.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_estimators/__init__.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     4697 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_estimators/estimate.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3862 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_estimators/mem.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    28728 2023-11-27 00:48:14.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_estimators/mem2.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    16922 2024-04-15 22:37:17.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_factory_methods.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1432 2024-01-23 21:48:48.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_geospatial.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3275 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_operations.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    16190 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_partitioning.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3903 2024-05-27 22:04:11.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_physical_constants.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    83871 2024-05-27 23:21:53.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_spectrum.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    21205 2024-04-16 18:55:29.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_spline_interpolation.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3514 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_time.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     2922 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_timeseries.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    17108 2024-05-27 23:07:33.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/_variable_names.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    27327 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/parametric.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-05-27 23:25:16.664797 roguewavespectrum-0.2.9/src/roguewavespectrum/spotter/
+-rw-r--r--   0 pietersmit   (502) staff       (20)     5066 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/spotter/__init__.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     9651 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/spotter/_spotter_extrapolate_tail.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3802 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/spotter/_spotter_post_processing.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     2762 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/spotter/_spotter_sdcard_data.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    12122 2024-01-20 00:31:36.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/spotter/_spotter_time_integration.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    16780 2024-01-23 21:48:48.000000 roguewavespectrum-0.2.9/src/roguewavespectrum/spotter/_spotter_wavefleet_api.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-05-27 23:25:16.663289 roguewavespectrum-0.2.9/src/roguewavespectrum.egg-info/
+-rw-r--r--   0 pietersmit   (502) staff       (20)      947 2024-05-27 23:25:16.000000 roguewavespectrum-0.2.9/src/roguewavespectrum.egg-info/PKG-INFO
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1398 2024-05-27 23:25:16.000000 roguewavespectrum-0.2.9/src/roguewavespectrum.egg-info/SOURCES.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)        1 2024-05-27 23:25:16.000000 roguewavespectrum-0.2.9/src/roguewavespectrum.egg-info/dependency_links.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)      129 2024-05-27 23:25:16.000000 roguewavespectrum-0.2.9/src/roguewavespectrum.egg-info/requires.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)       18 2024-05-27 23:25:16.000000 roguewavespectrum-0.2.9/src/roguewavespectrum.egg-info/top_level.txt
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-05-27 23:25:16.665667 roguewavespectrum-0.2.9/test/
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1776 2023-10-27 21:23:45.000000 roguewavespectrum-0.2.9/test/test_directions.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     8227 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.9/test/test_factory_methods.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)      876 2024-02-28 21:55:38.000000 roguewavespectrum-0.2.9/test/test_geospatial.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     2188 2023-10-21 21:15:35.000000 roguewavespectrum-0.2.9/test/test_parametric.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    21092 2024-05-27 23:23:35.000000 roguewavespectrum-0.2.9/test/test_spectrum.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3820 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.9/test/test_timeseries.py
```

### Comparing `roguewavespectrum-0.2.7/LICENSE` & `roguewavespectrum-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/PKG-INFO` & `roguewavespectrum-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roguewavespectrum
-Version: 0.2.7
+Version: 0.2.9
 Summary: Python package that implements a spectral object for ocean surface gravity waves
 Home-page: https://github.com/sofarocean/oceanwavespectrum.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `roguewavespectrum-0.2.7/setup.py` & `roguewavespectrum-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme_contents = file.read()
 
 setuptools.setup(
     name="roguewavespectrum",
-    version="0.2.7",
+    version="0.2.9",
     license="Apache 2 License",
     install_requires=[
         "numpy",
         "numba",
         "linearwavetheory",
         "xarray",
         "scipy",
```

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/__init__.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 possible to install and use.
 
 Ideally I would love to make this a community effort, and I would love to see others contribute to this package and
 become maintainers.
 
 How well is this package tested?
 --------------------------------
-The package contains a number of unit tests, but those mostly test if the code runs, and if the code is consitent
+The package contains a number of unit tests, but those mostly test if the code runs, and if the code is consistent
 with previous behaviour, not if the code is correct. Most of these routines have been in use in
 my own work and calculations are based on well established theory.
 
 Spectra
 =======
 We consider ocean surface-wave variance density spectra, either as:
```

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_directions.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_directions.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/__init__.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/estimate.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_estimators/estimate.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/mem.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_estimators/mem.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/mem2.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_estimators/mem2.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_factory_methods.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_factory_methods.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_geospatial.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_geospatial.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_operations.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_operations.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_partitioning.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_partitioning.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_physical_constants.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_physical_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,13 +85,13 @@
     """
     Convert a PhysicsOptions object to a PhysicsOptionsLWT object. This is used to pass the PhysicsOptions object
     to the linearwavetheory package.
 
     :param physicsoptions: PhysicsOptions object
     :return: PhysicsOptionsLWT object
     """
-    return lwt.PhysicsOptions(
+    return lwt.physics_options(
         kinematic_surface_tension=physicsoptions.kinematic_surface_tension,
         grav=physicsoptions.gravity,
         wave_type=physicsoptions.wave_type,
         wave_regime=physicsoptions.wave_regime,
     )
```

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_spectrum.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_spectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import numpy as np
 import pandas as pd
 from linearwavetheory import (
     inverse_intrinsic_dispersion_relation,
     intrinsic_group_speed,
     intrinsic_phase_speed,
 )
+from linearwavetheory.stokes_theory import surface_elevation_skewness
+
 from roguewavespectrum._geospatial import contains
 from roguewavespectrum._time import to_datetime64
 from roguewavespectrum._physical_constants import (
     PHYSICSOPTIONS,
     PhysicsOptions,
     _as_physicsoptions_lwt,
 )
@@ -1357,14 +1359,17 @@
 
         :param fmin: minimum frequency, inclusive
         :param fmax: maximum frequency, inclusive
         :return: Significant wave height
         """
         return set_conventions(4 * np.sqrt(self.m0(fmin, fmax)), "Hm0", overwrite=True)
 
+    def significant_waveheight(self, fmin=0, fmax=np.inf) -> DataArray:
+        return self.hm0(fmin, fmax)
+
     def hrms(self, fmin: float = 0.0, fmax: float = np.inf) -> DataArray:
         """
         Root mean square wave height estimated from the spectrum.
 
         :param fmin: minimum frequency, inclusive
         :param fmax: maximum frequency, inclusive
         :return: RMS wave height
@@ -1745,26 +1750,125 @@
         :param fmax: maximum frequency, inclusive
         :return: Mean period
         """
         return set_conventions(
             self.m0(fmin, fmax) / self.m1(fmin, fmax), "mean_period", overwrite=True
         )
 
+    def third_order_moment_surface_elevation(self) -> DataArray:
+        """
+        Third order moment ("skewness") of the surface elevation associated with the spectrum defined as $E[\\eta^3]$,
+        where $\\eta$ is the zero mean surface elevation, and $E[\\ldots]$ is the expectation operator.
+
+        The third-order moment is estimated from finite depth theory (e.g. Herbers & Janssen, 2016) as implemented in
+        the `linearwavetheory` package. It is assumed the Ursell number is small.
+
+        The skewness can only be calculated for 2D spectra. Convert to a 2D spectrum using the
+        `as_frequency_direction_spectrum` method if need be.
+
+        Herbers, T. H. C., & Janssen, T. T. (2016). Lagrangian surface wave motion and Stokes drift fluctuations.
+        Journal of Physical Oceanography, 46(4), 1009-1021.
+
+        :param fmin: minimum frequency, inclusive
+        :param fmax: maximum frequency, inclusive
+        :return: skewness
+        """
+        if self.is_1d:
+            raise ValueError("Skewness can only be estimated for 2D spectra")
+
+        # Construct the output coordinates and dimension of the data array
+        coords = {}
+        for dim in self.dims_space_time:
+            coords[dim] = self.dataset[dim].values
+
+        moment = DataArray(
+            data=surface_elevation_skewness(
+                self.frequency.values,
+                self.direction().values,
+                self.directional_variance_density.values,
+                self.depth.values,
+                _as_physicsoptions_lwt(self._physics_options),
+            ),
+            dims=self.dims_space_time,
+            coords=coords,
+        )
+        return set_conventions(
+            moment, "third_order_moment_surface_elevation", overwrite=True
+        )
+
+    def skewness_surface_elevation(self) -> DataArray:
+        """
+        Skewness of the surface elevation associated with the spectrum. Defined as
+
+        $$\\text{Sk} = \\frac{E[\\eta^3]}{m_0^{3/2}}$$
+
+        where $\\eta$ is the zero mean surface elevation, $E[\\ldots]$ is the expectation operator, and $m_0$ is the
+        zeroth frequency moment of the spectrum.
+
+        The third-order moment $E[\\eta^3]$ is estimated from finite depth theory (e.g. Herbers & Janssen, 2016) as
+        implemented in the `linearwavetheory`  package. It is assumed the Ursell number is small.
+
+        The skewness can only be calculated for 2D spectra. Convert to a 2D spectrum using the
+        `as_frequency_direction_spectrum` method if need be.
+
+        Herbers, T. H. C., & Janssen, T. T. (2016). Lagrangian surface wave motion and Stokes drift fluctuations.
+        Journal of Physical Oceanography, 46(4), 1009-1021.
+
+        :param fmin: minimum frequency, inclusive
+        :param fmax: maximum frequency, inclusive
+        :return: skewness
+        """
+        return set_conventions(
+            self.third_order_moment_surface_elevation() / np.sqrt(self.m0() ** 3),
+            "wave_skewness",
+            overwrite=True,
+        )
+
     def energy_period(self, fmin: float = 0.0, fmax: float = np.inf) -> DataArray:
         """
         Wave energy period defined as the ratio of the zeroth and second frequency moment.
 
         :param fmin: minimum frequency, inclusive
         :param fmax: maximum frequency, inclusive
         :return: Mean period
         """
         return set_conventions(
             self.m1(fmin, fmax) / self.m0(fmin, fmax), "energy_period", overwrite=True
         )
 
+    def ursell_number(self, fmin: float = 0.0, fmax: float = np.inf) -> DataArray:
+        """
+        Ursell number of the wave spectrum. The Ursell number is a measure of the shallow water-nonlinearity of the wave
+        field which we define here as
+
+        $$Ur = \\frac{\\delta}{\\mu^2}$$
+
+        where $\\delta$ is the shallow water nonlinearity parameter and $\\mu$ is the relative depth. Here we estimate
+        the shallow water nonlinearity parameter from the spectrum as
+
+        $$\\delta = \\frac{a}{d} = \\frac{H_{rms}}{2d}$$
+
+        where $H_{rms}$ is the root-mean-square wave-height, $d$ is the water depth. Furthermore, the relative depth is
+        defined as
+
+        $$\\mu = d k_{p}$$
+
+        :param fmin: minimum frequency, inclusive
+        :param fmax: maximum frequency, inclusive
+        :return: Ursell number
+        """
+        shallow_water_nonlinearity = self.hrms(fmin, fmax) / self.depth / 2.0
+        relative_depth = self.depth * self.peak_wavenumber(fmin, fmax)
+
+        return set_conventions(
+            shallow_water_nonlinearity / relative_depth**2,
+            "ursell_number",
+            overwrite=True,
+        )
+
     def zero_crossing_period(
         self, fmin: float = 0.0, fmax: float = np.inf
     ) -> DataArray:
         """
         Zero crossing period based on Rice's spectral estimate.
 
         :param fmin: minimum frequency, inclusive
```

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_spline_interpolation.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_spline_interpolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -461,15 +461,15 @@
     for index, root in enumerate(list_of_roots_for_all_spectra):
         # ..evaluate density spectrum at those roots.
         values_at_roots = interpolator(root)
 
         # Because the interpolator returns values at the current roots evaluated at _all_ spectra, we still have to
         # select the values at the spectrum of interest. This implementation is silly, adds computational costs, and can
         # probably be improved. It seems "fast enough" so that I'll punt that to another time.
-        if len(list_of_roots_for_all_spectra) > 1:
+        if frequency_spectrum.ndim > 1:
             values_at_roots = values_at_roots[index, :]
 
         _root = root[np.isfinite(values_at_roots)]
         values_at_roots = values_at_roots[np.isfinite(values_at_roots)]
 
         # ... get the root that corresponds to the largest peak.
         index_peak = np.argmax(values_at_roots)
```

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_time.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_time.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_timeseries.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_timeseries.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/_variable_names.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/_variable_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -420,14 +420,38 @@
     },
     "peak_wavenumber": {
         "units": "rad/m",
         "long_name": "Peak wave wavenumber",
         "missing_value": np.NAN,
         "valid_min": 0,
     },
+    "third_order_moment_surface_elevation": {
+        # Not an official cf-standard name
+        "units": "m^3",
+        "long_name": "sea_surface_third_order_moment",
+        "missing_value": np.NAN,
+        "valid_min": -100,
+        "valid_max": 100,
+        "comment": "Moment estimated based on second-order perturbation theory",
+    },
+    "wave_skewness": {
+        # Not an official cf-standard name
+        "long_name": "sea_surface_wave_skewness",
+        "missing_value": np.NAN,
+        "valid_min": -5,
+        "valid_max": 5,
+        "comment": "Skewness estimated based on second-order perturbation theory",
+    },
+    "ursell_number": {
+        # Not an official cf-standard name
+        "long_name": "ursell_number",
+        "missing_value": np.NAN,
+        "valid_min": 0,
+        "comment": "Ursell number",
+    },
 }
 
 
 def get_conventions(variable):
     """
     Get CF conventions for a variable.
     :param variable: may be a list or a string. If a list we assume the attributes are found in a nested dictionary.
```

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/parametric.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/parametric.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/__init__.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/spotter/__init__.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_extrapolate_tail.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/spotter/_spotter_extrapolate_tail.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_post_processing.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/spotter/_spotter_post_processing.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_sdcard_data.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/spotter/_spotter_sdcard_data.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_time_integration.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/spotter/_spotter_time_integration.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_wavefleet_api.py` & `roguewavespectrum-0.2.9/src/roguewavespectrum/spotter/_spotter_wavefleet_api.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/PKG-INFO` & `roguewavespectrum-0.2.9/src/roguewavespectrum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roguewavespectrum
-Version: 0.2.7
+Version: 0.2.9
 Summary: Python package that implements a spectral object for ocean surface gravity waves
 Home-page: https://github.com/sofarocean/oceanwavespectrum.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/SOURCES.txt` & `roguewavespectrum-0.2.9/src/roguewavespectrum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/test/test_directions.py` & `roguewavespectrum-0.2.9/test/test_directions.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/test/test_factory_methods.py` & `roguewavespectrum-0.2.9/test/test_factory_methods.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/test/test_geospatial.py` & `roguewavespectrum-0.2.9/test/test_geospatial.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/test/test_parametric.py` & `roguewavespectrum-0.2.9/test/test_parametric.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.7/test/test_spectrum.py` & `roguewavespectrum-0.2.9/test/test_spectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -673,7 +673,46 @@
         _ = spec.wavenumber_spectral_density
 
 
 def test_wavenumber_directional_spectral_density():
     specs = helper_create_spectra(4)
     spec = specs[0]
     _ = spec.wavenumber_directional_spectral_density
+
+
+def test_third_order_moment_surface_elevation():
+    specs = helper_create_spectra(4)
+    _canary_values = [0.00436271, 0.01378833, 0.03366291, 0.06980341]
+    for spec in specs:
+        if spec.is_1d:
+            try:
+                skewness = spec.third_order_moment_surface_elevation()
+            except ValueError:
+                continue
+        else:
+            skewness = spec.third_order_moment_surface_elevation()
+
+        assert_allclose(skewness, _canary_values, atol=1e-4, rtol=1e-4)
+
+
+def test_skewness():
+    specs = helper_create_spectra(4)
+    _canary_values = [0.03490171, 0.04653561, 0.05816951, 0.06980341]
+    for spec in specs:
+        if spec.is_1d:
+            try:
+                skewness = spec.skewness_surface_elevation()
+            except ValueError:
+                continue
+        else:
+            skewness = spec.skewness_surface_elevation()
+        assert_allclose(skewness, _canary_values, atol=1e-4, rtol=1e-4)
+
+
+def test_ursell():
+    specs = helper_create_spectra(4)
+
+    _canary_values = [0.65625939, 0.87501251, 1.09376564, 1.31251877]
+    for spec in specs:
+        spec.depth = 5
+        ursell = spec.ursell_number()
+        assert_allclose(ursell, _canary_values, atol=1e-4, rtol=1e-4)
```

### Comparing `roguewavespectrum-0.2.7/test/test_timeseries.py` & `roguewavespectrum-0.2.9/test/test_timeseries.py`

 * *Files identical despite different names*

