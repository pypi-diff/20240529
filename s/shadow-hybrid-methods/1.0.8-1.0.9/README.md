# Comparing `tmp/shadow-hybrid-methods-1.0.8.tar.gz` & `tmp/shadow-hybrid-methods-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadow-hybrid-methods-1.0.8.tar", last modified: Thu Feb 29 20:26:58 2024, max compression
+gzip compressed data, was "shadow-hybrid-methods-1.0.9.tar", last modified: Wed May 29 18:58:19 2024, max compression
```

## Comparing `shadow-hybrid-methods-1.0.8.tar` & `shadow-hybrid-methods-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,29 @@
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-29 20:26:58.448933 shadow-hybrid-methods-1.0.8/
--rw-r--r--   0 rook       (505) staff       (20)     1526 2023-11-27 21:11:30.000000 shadow-hybrid-methods-1.0.8/LICENSE
--rw-r--r--   0 rook       (505) staff       (20)       18 2022-06-23 16:10:07.000000 shadow-hybrid-methods-1.0.8/MANIFEST.in
--rw-r--r--   0 rook       (505) staff       (20)     1227 2024-02-29 20:26:58.448752 shadow-hybrid-methods-1.0.8/PKG-INFO
--rw-r--r--   0 rook       (505) staff       (20)      104 2023-11-27 21:11:30.000000 shadow-hybrid-methods-1.0.8/README.md
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-29 20:26:58.445547 shadow-hybrid-methods-1.0.8/hybrid_methods/
--rw-r--r--   0 rook       (505) staff       (20)     3390 2023-11-27 21:13:04.000000 shadow-hybrid-methods-1.0.8/hybrid_methods/__init__.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-29 20:26:58.446212 shadow-hybrid-methods-1.0.8/hybrid_methods/coherence/
--rw-r--r--   0 rook       (505) staff       (20)     3390 2023-11-27 21:41:13.000000 shadow-hybrid-methods-1.0.8/hybrid_methods/coherence/__init__.py
--rw-r--r--   0 rook       (505) staff       (20)   131337 2024-02-29 16:45:33.000000 shadow-hybrid-methods-1.0.8/hybrid_methods/coherence/hybrid_screen.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-29 20:26:58.447232 shadow-hybrid-methods-1.0.8/hybrid_methods/undulator/
--rw-r--r--   0 rook       (505) staff       (20)     3390 2023-11-27 21:41:20.000000 shadow-hybrid-methods-1.0.8/hybrid_methods/undulator/__init__.py
--rw-r--r--   0 rook       (505) staff       (20)       38 2024-02-29 20:26:58.448991 shadow-hybrid-methods-1.0.8/setup.cfg
--rwxr-xr-x   0 rook       (505) staff       (20)     2472 2024-02-29 20:26:47.000000 shadow-hybrid-methods-1.0.8/setup.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-29 20:26:58.448394 shadow-hybrid-methods-1.0.8/shadow_hybrid_methods.egg-info/
--rw-r--r--   0 rook       (505) staff       (20)     1227 2024-02-29 20:26:58.000000 shadow-hybrid-methods-1.0.8/shadow_hybrid_methods.egg-info/PKG-INFO
--rw-r--r--   0 rook       (505) staff       (20)      445 2024-02-29 20:26:58.000000 shadow-hybrid-methods-1.0.8/shadow_hybrid_methods.egg-info/SOURCES.txt
--rw-r--r--   0 rook       (505) staff       (20)        1 2024-02-29 20:26:58.000000 shadow-hybrid-methods-1.0.8/shadow_hybrid_methods.egg-info/dependency_links.txt
--rw-r--r--   0 rook       (505) staff       (20)       71 2024-02-29 20:26:58.000000 shadow-hybrid-methods-1.0.8/shadow_hybrid_methods.egg-info/requires.txt
--rw-r--r--   0 rook       (505) staff       (20)       15 2024-02-29 20:26:58.000000 shadow-hybrid-methods-1.0.8/shadow_hybrid_methods.egg-info/top_level.txt
--rw-r--r--   0 rook       (505) staff       (20)        1 2024-02-13 17:41:30.000000 shadow-hybrid-methods-1.0.8/shadow_hybrid_methods.egg-info/zip-safe
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-05-29 18:58:19.811782 shadow-hybrid-methods-1.0.9/
+-rw-r--r--   0 rook       (505) staff       (20)     1526 2023-11-27 21:11:30.000000 shadow-hybrid-methods-1.0.9/LICENSE
+-rw-r--r--   0 rook       (505) staff       (20)       18 2022-06-23 16:10:07.000000 shadow-hybrid-methods-1.0.9/MANIFEST.in
+-rw-r--r--   0 rook       (505) staff       (20)     1403 2024-05-29 18:58:19.811407 shadow-hybrid-methods-1.0.9/PKG-INFO
+-rw-r--r--   0 rook       (505) staff       (20)      104 2023-11-27 21:11:30.000000 shadow-hybrid-methods-1.0.9/README.md
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-05-29 18:58:19.803388 shadow-hybrid-methods-1.0.9/hybrid_methods/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2023-11-27 21:13:04.000000 shadow-hybrid-methods-1.0.9/hybrid_methods/__init__.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-05-29 18:58:19.804405 shadow-hybrid-methods-1.0.9/hybrid_methods/coherence/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2023-11-27 21:41:13.000000 shadow-hybrid-methods-1.0.9/hybrid_methods/coherence/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)   131337 2024-02-29 16:45:33.000000 shadow-hybrid-methods-1.0.9/hybrid_methods/coherence/hybrid_screen.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-05-29 18:58:19.805717 shadow-hybrid-methods-1.0.9/hybrid_methods/fresnel_zone_plate/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2024-02-21 16:33:31.000000 shadow-hybrid-methods-1.0.9/hybrid_methods/fresnel_zone_plate/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)     5582 2024-02-21 20:32:31.000000 shadow-hybrid-methods-1.0.9/hybrid_methods/fresnel_zone_plate/hybrid_fresnel_zone_plate.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-05-29 18:58:19.807430 shadow-hybrid-methods-1.0.9/hybrid_methods/fresnel_zone_plate/simulator/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2024-02-21 20:31:49.000000 shadow-hybrid-methods-1.0.9/hybrid_methods/fresnel_zone_plate/simulator/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)    33168 2024-02-21 20:32:31.000000 shadow-hybrid-methods-1.0.9/hybrid_methods/fresnel_zone_plate/simulator/fresnel_zone_plate_simulator.py
+-rw-r--r--   0 rook       (505) staff       (20)     6536 2024-02-22 15:40:08.000000 shadow-hybrid-methods-1.0.9/hybrid_methods/fresnel_zone_plate/simulator/hankel_transform.py
+-rw-r--r--   0 rook       (505) staff       (20)   225474 2022-06-23 16:17:32.000000 shadow-hybrid-methods-1.0.9/hybrid_methods/fresnel_zone_plate/simulator/refractive_index.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-05-29 18:58:19.808332 shadow-hybrid-methods-1.0.9/hybrid_methods/undulator/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2023-11-27 21:41:20.000000 shadow-hybrid-methods-1.0.9/hybrid_methods/undulator/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)       38 2024-05-29 18:58:19.811859 shadow-hybrid-methods-1.0.9/setup.cfg
+-rwxr-xr-x   0 rook       (505) staff       (20)     2564 2024-05-29 18:57:57.000000 shadow-hybrid-methods-1.0.9/setup.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-05-29 18:58:19.810900 shadow-hybrid-methods-1.0.9/shadow_hybrid_methods.egg-info/
+-rw-r--r--   0 rook       (505) staff       (20)     1403 2024-05-29 18:58:19.000000 shadow-hybrid-methods-1.0.9/shadow_hybrid_methods.egg-info/PKG-INFO
+-rw-r--r--   0 rook       (505) staff       (20)      814 2024-05-29 18:58:19.000000 shadow-hybrid-methods-1.0.9/shadow_hybrid_methods.egg-info/SOURCES.txt
+-rw-r--r--   0 rook       (505) staff       (20)        1 2024-05-29 18:58:19.000000 shadow-hybrid-methods-1.0.9/shadow_hybrid_methods.egg-info/dependency_links.txt
+-rw-r--r--   0 rook       (505) staff       (20)       71 2024-05-29 18:58:19.000000 shadow-hybrid-methods-1.0.9/shadow_hybrid_methods.egg-info/requires.txt
+-rw-r--r--   0 rook       (505) staff       (20)       15 2024-05-29 18:58:19.000000 shadow-hybrid-methods-1.0.9/shadow_hybrid_methods.egg-info/top_level.txt
+-rw-r--r--   0 rook       (505) staff       (20)        1 2024-02-13 17:41:30.000000 shadow-hybrid-methods-1.0.9/shadow_hybrid_methods.egg-info/zip-safe
```

### Comparing `shadow-hybrid-methods-1.0.8/LICENSE` & `shadow-hybrid-methods-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shadow-hybrid-methods-1.0.8/PKG-INFO` & `shadow-hybrid-methods-1.0.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadow-hybrid-methods
-Version: 1.0.8
+Version: 1.0.9
 Summary: Hybrid Methods, combining raytracing with wave optics
 Home-page: https://github.com/oasys-kit/hybrid-methods
 Download-URL: https://github.com/oasys-kit/hybrid-methods
 Author: Luca Rebuffi, Xianbo Shi
 Author-email: lrebuffi@anl.gov
 Maintainer: Luca Rebuffi
 Maintainer-email: lrebuffi@anl.gov
@@ -19,10 +19,17 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: srxraylib>=1.0.45
+Requires-Dist: syned
+Requires-Dist: wofry
+Requires-Dist: wofryimpl>=1.0.26
 
 # hybrid-methods
 Collection of algorithms that combine raytracing with wave optics, to improve accuracy
```

### Comparing `shadow-hybrid-methods-1.0.8/hybrid_methods/__init__.py` & `shadow-hybrid-methods-1.0.9/hybrid_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `shadow-hybrid-methods-1.0.8/hybrid_methods/coherence/__init__.py` & `shadow-hybrid-methods-1.0.9/hybrid_methods/coherence/__init__.py`

 * *Files identical despite different names*

### Comparing `shadow-hybrid-methods-1.0.8/hybrid_methods/coherence/hybrid_screen.py` & `shadow-hybrid-methods-1.0.9/hybrid_methods/coherence/hybrid_screen.py`

 * *Files identical despite different names*

### Comparing `shadow-hybrid-methods-1.0.8/hybrid_methods/undulator/__init__.py` & `shadow-hybrid-methods-1.0.9/hybrid_methods/undulator/__init__.py`

 * *Files identical despite different names*

### Comparing `shadow-hybrid-methods-1.0.8/setup.py` & `shadow-hybrid-methods-1.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 try:
     from setuptools import find_packages, setup
 except AttributeError:
     from setuptools import find_packages, setup
 
 NAME = 'shadow-hybrid-methods'
 
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 ISRELEASED = True
 
 DESCRIPTION = 'Hybrid Methods, combining raytracing with wave optics'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.md')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Luca Rebuffi, Xianbo Shi'
 AUTHOR_EMAIL = 'lrebuffi@anl.gov'
@@ -61,14 +61,16 @@
 SETUP_REQUIRES = (
     'setuptools',
 )
 
 PACKAGES = [
     "hybrid_methods",
     "hybrid_methods.coherence",
+    "hybrid_methods.fresnel_zone_plate",
+    "hybrid_methods.fresnel_zone_plate.simulator",
     "hybrid_methods.undulator",
 ]
 
 PACKAGE_DATA = {
 }
```

### Comparing `shadow-hybrid-methods-1.0.8/shadow_hybrid_methods.egg-info/PKG-INFO` & `shadow-hybrid-methods-1.0.9/shadow_hybrid_methods.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadow-hybrid-methods
-Version: 1.0.8
+Version: 1.0.9
 Summary: Hybrid Methods, combining raytracing with wave optics
 Home-page: https://github.com/oasys-kit/hybrid-methods
 Download-URL: https://github.com/oasys-kit/hybrid-methods
 Author: Luca Rebuffi, Xianbo Shi
 Author-email: lrebuffi@anl.gov
 Maintainer: Luca Rebuffi
 Maintainer-email: lrebuffi@anl.gov
@@ -19,10 +19,17 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: srxraylib>=1.0.45
+Requires-Dist: syned
+Requires-Dist: wofry
+Requires-Dist: wofryimpl>=1.0.26
 
 # hybrid-methods
 Collection of algorithms that combine raytracing with wave optics, to improve accuracy
```

