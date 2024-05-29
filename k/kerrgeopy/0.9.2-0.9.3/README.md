# Comparing `tmp/kerrgeopy-0.9.2.tar.gz` & `tmp/kerrgeopy-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerrgeopy-0.9.2.tar", last modified: Mon May 27 15:23:23 2024, max compression
+gzip compressed data, was "kerrgeopy-0.9.3.tar", last modified: Wed May 29 12:45:51 2024, max compression
```

## Comparing `kerrgeopy-0.9.2.tar` & `kerrgeopy-0.9.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:23:23.259323 kerrgeopy-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-05-27 15:23:23.259323 kerrgeopy-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:23:23.259323 kerrgeopy-0.9.2/kerrgeopy/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    27367 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12869 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)    32635 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/orbit.py
--rw-r--r--   0 runner    (1001) docker     (127)    24000 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/plunge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/spacetime.py
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/stable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:23:23.259323 kerrgeopy-0.9.2/kerrgeopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-05-27 15:23:23.000000 kerrgeopy-0.9.2/kerrgeopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-27 15:23:23.000000 kerrgeopy-0.9.2/kerrgeopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:23:23.000000 kerrgeopy-0.9.2/kerrgeopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:23:23.000000 kerrgeopy-0.9.2/kerrgeopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 15:23:23.000000 kerrgeopy-0.9.2/kerrgeopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:23:23.259323 kerrgeopy-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:23:23.259323 kerrgeopy-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/tests/test_four_velocity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/tests/test_frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/tests/test_initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/tests/test_plunging_solutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/tests/test_stable_solutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:45:51.518497 kerrgeopy-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-29 12:45:42.000000 kerrgeopy-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-29 12:45:51.518497 kerrgeopy-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-29 12:45:42.000000 kerrgeopy-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:45:51.518497 kerrgeopy-0.9.3/kerrgeopy/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-29 12:45:42.000000 kerrgeopy-0.9.3/kerrgeopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-05-29 12:45:42.000000 kerrgeopy-0.9.3/kerrgeopy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27367 2024-05-29 12:45:42.000000 kerrgeopy-0.9.3/kerrgeopy/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12869 2024-05-29 12:45:42.000000 kerrgeopy-0.9.3/kerrgeopy/initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32635 2024-05-29 12:45:42.000000 kerrgeopy-0.9.3/kerrgeopy/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24000 2024-05-29 12:45:42.000000 kerrgeopy-0.9.3/kerrgeopy/plunge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-05-29 12:45:42.000000 kerrgeopy-0.9.3/kerrgeopy/spacetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-29 12:45:42.000000 kerrgeopy-0.9.3/kerrgeopy/stable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-29 12:45:42.000000 kerrgeopy-0.9.3/kerrgeopy/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:45:51.518497 kerrgeopy-0.9.3/kerrgeopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-29 12:45:51.000000 kerrgeopy-0.9.3/kerrgeopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-29 12:45:51.000000 kerrgeopy-0.9.3/kerrgeopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:45:51.000000 kerrgeopy-0.9.3/kerrgeopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:45:51.000000 kerrgeopy-0.9.3/kerrgeopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 12:45:51.000000 kerrgeopy-0.9.3/kerrgeopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:45:51.518497 kerrgeopy-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-29 12:45:42.000000 kerrgeopy-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:45:51.518497 kerrgeopy-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-29 12:45:43.000000 kerrgeopy-0.9.3/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-29 12:45:43.000000 kerrgeopy-0.9.3/tests/test_four_velocity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-29 12:45:43.000000 kerrgeopy-0.9.3/tests/test_frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-29 12:45:43.000000 kerrgeopy-0.9.3/tests/test_initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-29 12:45:43.000000 kerrgeopy-0.9.3/tests/test_plunging_solutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-29 12:45:43.000000 kerrgeopy-0.9.3/tests/test_stable_solutions.py
```

### Comparing `kerrgeopy-0.9.2/PKG-INFO` & `kerrgeopy-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: kerrgeopy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Library for computing stable and plunging geodesics in Kerr spacetime
 Home-page: https://github.com/BlackHolePerturbationToolkit/KerrGeoPy
 Author: Seyong Park
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy>=1.8
 Requires-Dist: numpy
 Requires-Dist: matplotlib>=3.7
 Requires-Dist: tqdm
```

### Comparing `kerrgeopy-0.9.2/README.md` & `kerrgeopy-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/kerrgeopy/constants.py` & `kerrgeopy-0.9.3/kerrgeopy/constants.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/kerrgeopy/frequencies.py` & `kerrgeopy-0.9.3/kerrgeopy/frequencies.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/kerrgeopy/initial_conditions.py` & `kerrgeopy-0.9.3/kerrgeopy/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/kerrgeopy/orbit.py` & `kerrgeopy-0.9.3/kerrgeopy/orbit.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/kerrgeopy/plunge.py` & `kerrgeopy-0.9.3/kerrgeopy/plunge.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/kerrgeopy/spacetime.py` & `kerrgeopy-0.9.3/kerrgeopy/spacetime.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/kerrgeopy/stable.py` & `kerrgeopy-0.9.3/kerrgeopy/stable.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/kerrgeopy/units.py` & `kerrgeopy-0.9.3/kerrgeopy/units.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/kerrgeopy.egg-info/PKG-INFO` & `kerrgeopy-0.9.3/kerrgeopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: kerrgeopy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Library for computing stable and plunging geodesics in Kerr spacetime
 Home-page: https://github.com/BlackHolePerturbationToolkit/KerrGeoPy
 Author: Seyong Park
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy>=1.8
 Requires-Dist: numpy
 Requires-Dist: matplotlib>=3.7
 Requires-Dist: tqdm
```

### Comparing `kerrgeopy-0.9.2/kerrgeopy.egg-info/SOURCES.txt` & `kerrgeopy-0.9.3/kerrgeopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/setup.py` & `kerrgeopy-0.9.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="kerrgeopy",
-    version="0.9.2",
+    version="0.9.3",
     author="Seyong Park",
     description="Library for computing stable and plunging geodesics in Kerr spacetime",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/BlackHolePerturbationToolkit/KerrGeoPy",
     packages=setuptools.find_packages(exclude=["tests"]),
     classifiers=(
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: GNU General Public License (GPL)",
+        "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
     ),
     install_requires=["scipy>=1.8","numpy","matplotlib>=3.7","tqdm"]
 )
```

### Comparing `kerrgeopy-0.9.2/tests/test_constants.py` & `kerrgeopy-0.9.3/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/tests/test_four_velocity.py` & `kerrgeopy-0.9.3/tests/test_four_velocity.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/tests/test_frequencies.py` & `kerrgeopy-0.9.3/tests/test_frequencies.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/tests/test_initial_conditions.py` & `kerrgeopy-0.9.3/tests/test_initial_conditions.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/tests/test_plunging_solutions.py` & `kerrgeopy-0.9.3/tests/test_plunging_solutions.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.2/tests/test_stable_solutions.py` & `kerrgeopy-0.9.3/tests/test_stable_solutions.py`

 * *Files identical despite different names*

