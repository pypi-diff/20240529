# Comparing `tmp/linearwavetheory-0.0.8.tar.gz` & `tmp/linearwavetheory-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linearwavetheory-0.0.8.tar", last modified: Sat Aug 19 01:11:33 2023, max compression
+gzip compressed data, was "linearwavetheory-0.0.9.tar", last modified: Fri Aug 25 20:08:08 2023, max compression
```

## Comparing `linearwavetheory-0.0.8.tar` & `linearwavetheory-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-19 01:11:33.108888 linearwavetheory-0.0.8/
--rw-r--r--   0 pietersmit   (502) staff       (20)    11357 2023-08-06 02:37:22.000000 linearwavetheory-0.0.8/LICENSE
--rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-19 01:11:33.108761 linearwavetheory-0.0.8/PKG-INFO
--rw-r--r--   0 pietersmit   (502) staff       (20)      532 2023-08-06 03:43:57.000000 linearwavetheory-0.0.8/README.md
--rw-r--r--   0 pietersmit   (502) staff       (20)       38 2023-08-19 01:11:33.108935 linearwavetheory-0.0.8/setup.cfg
--rw-r--r--   0 pietersmit   (502) staff       (20)     1055 2023-08-19 01:11:12.000000 linearwavetheory-0.0.8/setup.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-19 01:11:33.106433 linearwavetheory-0.0.8/src/
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-19 01:11:33.107808 linearwavetheory-0.0.8/src/linearwavetheory/
--rw-r--r--   0 pietersmit   (502) staff       (20)      249 2023-08-06 03:43:57.000000 linearwavetheory-0.0.8/src/linearwavetheory/__init__.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3005 2023-08-16 03:36:48.000000 linearwavetheory-0.0.8/src/linearwavetheory/_array_shape_preprocessing.py
--rw-r--r--   0 pietersmit   (502) staff       (20)      260 2023-08-10 17:23:06.000000 linearwavetheory-0.0.8/src/linearwavetheory/_constants.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    12736 2023-08-18 23:51:32.000000 linearwavetheory-0.0.8/src/linearwavetheory/_dispersion_ufuncs.py
--rw-r--r--   0 pietersmit   (502) staff       (20)      499 2023-08-10 01:43:38.000000 linearwavetheory-0.0.8/src/linearwavetheory/_numba_settings.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    27277 2023-08-18 23:52:21.000000 linearwavetheory-0.0.8/src/linearwavetheory/dispersion.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3757 2023-08-10 21:04:24.000000 linearwavetheory-0.0.8/src/linearwavetheory/settings.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-19 01:11:33.108565 linearwavetheory-0.0.8/src/linearwavetheory.egg-info/
--rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-19 01:11:33.000000 linearwavetheory-0.0.8/src/linearwavetheory.egg-info/PKG-INFO
--rw-r--r--   0 pietersmit   (502) staff       (20)      515 2023-08-19 01:11:33.000000 linearwavetheory-0.0.8/src/linearwavetheory.egg-info/SOURCES.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)        1 2023-08-19 01:11:33.000000 linearwavetheory-0.0.8/src/linearwavetheory.egg-info/dependency_links.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)       12 2023-08-19 01:11:33.000000 linearwavetheory-0.0.8/src/linearwavetheory.egg-info/requires.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)       17 2023-08-19 01:11:33.000000 linearwavetheory-0.0.8/src/linearwavetheory.egg-info/top_level.txt
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-25 20:08:08.102799 linearwavetheory-0.0.9/
+-rw-r--r--   0 pietersmit   (502) staff       (20)    11357 2023-08-06 02:37:22.000000 linearwavetheory-0.0.9/LICENSE
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-25 20:08:08.102561 linearwavetheory-0.0.9/PKG-INFO
+-rw-r--r--   0 pietersmit   (502) staff       (20)      532 2023-08-06 03:43:57.000000 linearwavetheory-0.0.9/README.md
+-rw-r--r--   0 pietersmit   (502) staff       (20)       38 2023-08-25 20:08:08.102896 linearwavetheory-0.0.9/setup.cfg
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1055 2023-08-25 20:04:08.000000 linearwavetheory-0.0.9/setup.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-25 20:08:08.096915 linearwavetheory-0.0.9/src/
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-25 20:08:08.100719 linearwavetheory-0.0.9/src/linearwavetheory/
+-rw-r--r--   0 pietersmit   (502) staff       (20)      296 2023-08-25 20:07:47.000000 linearwavetheory-0.0.9/src/linearwavetheory/__init__.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3005 2023-08-16 03:36:48.000000 linearwavetheory-0.0.9/src/linearwavetheory/_array_shape_preprocessing.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    12736 2023-08-18 23:51:32.000000 linearwavetheory-0.0.9/src/linearwavetheory/_dispersion_ufuncs.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)      499 2023-08-10 01:43:38.000000 linearwavetheory-0.0.9/src/linearwavetheory/_numba_settings.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    27277 2023-08-18 23:52:21.000000 linearwavetheory-0.0.9/src/linearwavetheory/dispersion.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3865 2023-08-25 20:07:48.000000 linearwavetheory-0.0.9/src/linearwavetheory/settings.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-25 20:08:08.102144 linearwavetheory-0.0.9/src/linearwavetheory.egg-info/
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-25 20:08:08.000000 linearwavetheory-0.0.9/src/linearwavetheory.egg-info/PKG-INFO
+-rw-r--r--   0 pietersmit   (502) staff       (20)      480 2023-08-25 20:08:08.000000 linearwavetheory-0.0.9/src/linearwavetheory.egg-info/SOURCES.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)        1 2023-08-25 20:08:08.000000 linearwavetheory-0.0.9/src/linearwavetheory.egg-info/dependency_links.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)       12 2023-08-25 20:08:08.000000 linearwavetheory-0.0.9/src/linearwavetheory.egg-info/requires.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)       17 2023-08-25 20:08:08.000000 linearwavetheory-0.0.9/src/linearwavetheory.egg-info/top_level.txt
```

### Comparing `linearwavetheory-0.0.8/LICENSE` & `linearwavetheory-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `linearwavetheory-0.0.8/PKG-INFO` & `linearwavetheory-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linearwavetheory
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package that implements linear wave theory for ocean surface gravity waves
 Home-page: https://github.com/sofarocean/linearwavetheory.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linearwavetheory-0.0.8/README.md` & `linearwavetheory-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `linearwavetheory-0.0.8/setup.py` & `linearwavetheory-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme_contents = file.read()
 
 setuptools.setup(
     name="linearwavetheory",
-    version="0.0.8",
+    version="0.0.9",
     license="Apache 2 License",
     install_requires=[
         "numpy",
         "numba",
     ],
     description="Python package that implements linear wave theory for ocean surface gravity waves",
     long_description=readme_contents,
```

### Comparing `linearwavetheory-0.0.8/src/linearwavetheory/_array_shape_preprocessing.py` & `linearwavetheory-0.0.9/src/linearwavetheory/_array_shape_preprocessing.py`

 * *Files identical despite different names*

### Comparing `linearwavetheory-0.0.8/src/linearwavetheory/_dispersion_ufuncs.py` & `linearwavetheory-0.0.9/src/linearwavetheory/_dispersion_ufuncs.py`

 * *Files identical despite different names*

### Comparing `linearwavetheory-0.0.8/src/linearwavetheory/dispersion.py` & `linearwavetheory-0.0.9/src/linearwavetheory/dispersion.py`

 * *Files identical despite different names*

### Comparing `linearwavetheory-0.0.8/src/linearwavetheory/settings.py` & `linearwavetheory-0.0.9/src/linearwavetheory/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from numba import float64, int64, jit
 from ._numba_settings import numba_default
 from numba.core.types import unicode_type
 from numba.experimental import jitclass
+import numpy as np
 
-from ._constants import (
-    GRAV,
-    KINEMATIC_SURFACE_TENSION,
-    RELATIVE_TOLERANCE,
-    MAXIMUM_NUMBER_OF_ITERATIONS,
-    ABSOLUTE_TOLERANCE,
-)
+GRAV = 9.80665
+SURFACE_TENSION = 0.074
+WATER_DENSITY = 1025
+KINEMATIC_SURFACE_TENSION = SURFACE_TENSION / WATER_DENSITY
+
+# Default Numerical Parameters
+RELATIVE_TOLERANCE = 1e-3
+MAXIMUM_NUMBER_OF_ITERATIONS = 10
+ABSOLUTE_TOLERANCE = np.inf
 
 
 @jitclass(
     [
         ("_kinematic_surface_tension", float64),
         ("_grav", float64),
         ("wave_type", unicode_type),
```

### Comparing `linearwavetheory-0.0.8/src/linearwavetheory.egg-info/PKG-INFO` & `linearwavetheory-0.0.9/src/linearwavetheory.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linearwavetheory
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package that implements linear wave theory for ocean surface gravity waves
 Home-page: https://github.com/sofarocean/linearwavetheory.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Classifier: Programming Language :: Python :: 3
```

