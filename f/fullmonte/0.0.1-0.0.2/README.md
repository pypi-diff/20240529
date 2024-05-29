# Comparing `tmp/fullmonte-0.0.1.tar.gz` & `tmp/fullmonte-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullmonte-0.0.1.tar", last modified: Tue Mar 12 16:19:40 2024, max compression
+gzip compressed data, was "fullmonte-0.0.2.tar", last modified: Wed May 29 21:26:46 2024, max compression
```

## Comparing `fullmonte-0.0.1.tar` & `fullmonte-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2024-03-12 16:19:40.412474 fullmonte-0.0.1/
--rw-r--r--   0 sackfield   (501) staff       (20)     1071 2024-03-12 15:02:32.000000 fullmonte-0.0.1/LICENSE
--rw-r--r--   0 sackfield   (501) staff       (20)       91 2024-03-12 15:04:53.000000 fullmonte-0.0.1/MANIFEST.in
--rw-r--r--   0 sackfield   (501) staff       (20)     1867 2024-03-12 16:19:40.412257 fullmonte-0.0.1/PKG-INFO
--rw-r--r--   0 sackfield   (501) staff       (20)     1358 2024-03-12 16:17:33.000000 fullmonte-0.0.1/README.md
-drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2024-03-12 16:19:40.411197 fullmonte-0.0.1/fullmonte/
--rw-r--r--   0 sackfield   (501) staff       (20)      110 2024-03-12 16:04:11.000000 fullmonte-0.0.1/fullmonte/__init__.py
--rw-r--r--   0 sackfield   (501) staff       (20)      195 2024-03-12 16:03:54.000000 fullmonte-0.0.1/fullmonte/plot.py
--rw-r--r--   0 sackfield   (501) staff       (20)      992 2024-03-12 16:03:54.000000 fullmonte-0.0.1/fullmonte/simulation.py
-drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2024-03-12 16:19:40.412013 fullmonte-0.0.1/fullmonte.egg-info/
--rw-r--r--   0 sackfield   (501) staff       (20)     1867 2024-03-12 16:19:40.000000 fullmonte-0.0.1/fullmonte.egg-info/PKG-INFO
--rw-r--r--   0 sackfield   (501) staff       (20)      315 2024-03-12 16:19:40.000000 fullmonte-0.0.1/fullmonte.egg-info/SOURCES.txt
--rw-r--r--   0 sackfield   (501) staff       (20)        1 2024-03-12 16:19:40.000000 fullmonte-0.0.1/fullmonte.egg-info/dependency_links.txt
--rw-r--r--   0 sackfield   (501) staff       (20)        1 2024-03-12 15:42:48.000000 fullmonte-0.0.1/fullmonte.egg-info/not-zip-safe
--rw-r--r--   0 sackfield   (501) staff       (20)       46 2024-03-12 16:19:40.000000 fullmonte-0.0.1/fullmonte.egg-info/requires.txt
--rw-r--r--   0 sackfield   (501) staff       (20)       10 2024-03-12 16:19:40.000000 fullmonte-0.0.1/fullmonte.egg-info/top_level.txt
--rw-r--r--   0 sackfield   (501) staff       (20)       45 2024-03-12 15:36:40.000000 fullmonte-0.0.1/requirements.txt
--rw-r--r--   0 sackfield   (501) staff       (20)       38 2024-03-12 16:19:40.412507 fullmonte-0.0.1/setup.cfg
--rw-r--r--   0 sackfield   (501) staff       (20)     1254 2024-03-12 15:04:26.000000 fullmonte-0.0.1/setup.py
+drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2024-05-29 21:26:46.119180 fullmonte-0.0.2/
+-rw-r--r--   0 sackfield   (501) staff       (20)     1071 2024-03-12 15:02:32.000000 fullmonte-0.0.2/LICENSE
+-rw-r--r--   0 sackfield   (501) staff       (20)       91 2024-03-12 15:04:53.000000 fullmonte-0.0.2/MANIFEST.in
+-rw-r--r--   0 sackfield   (501) staff       (20)     1867 2024-05-29 21:26:46.118966 fullmonte-0.0.2/PKG-INFO
+-rw-r--r--   0 sackfield   (501) staff       (20)     1358 2024-05-29 21:24:59.000000 fullmonte-0.0.2/README.md
+drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2024-05-29 21:26:46.118072 fullmonte-0.0.2/fullmonte/
+-rw-r--r--   0 sackfield   (501) staff       (20)      110 2024-03-12 16:04:11.000000 fullmonte-0.0.2/fullmonte/__init__.py
+-rw-r--r--   0 sackfield   (501) staff       (20)      195 2024-03-12 16:03:54.000000 fullmonte-0.0.2/fullmonte/plot.py
+-rw-r--r--   0 sackfield   (501) staff       (20)      992 2024-03-12 16:03:54.000000 fullmonte-0.0.2/fullmonte/simulation.py
+drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2024-05-29 21:26:46.118735 fullmonte-0.0.2/fullmonte.egg-info/
+-rw-r--r--   0 sackfield   (501) staff       (20)     1867 2024-05-29 21:26:46.000000 fullmonte-0.0.2/fullmonte.egg-info/PKG-INFO
+-rw-r--r--   0 sackfield   (501) staff       (20)      315 2024-05-29 21:26:46.000000 fullmonte-0.0.2/fullmonte.egg-info/SOURCES.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)        1 2024-05-29 21:26:46.000000 fullmonte-0.0.2/fullmonte.egg-info/dependency_links.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)        1 2024-03-12 15:42:48.000000 fullmonte-0.0.2/fullmonte.egg-info/not-zip-safe
+-rw-r--r--   0 sackfield   (501) staff       (20)       46 2024-05-29 21:26:46.000000 fullmonte-0.0.2/fullmonte.egg-info/requires.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)       10 2024-05-29 21:26:46.000000 fullmonte-0.0.2/fullmonte.egg-info/top_level.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)       45 2024-05-29 21:24:40.000000 fullmonte-0.0.2/requirements.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)       38 2024-05-29 21:26:46.119214 fullmonte-0.0.2/setup.cfg
+-rw-r--r--   0 sackfield   (501) staff       (20)     1254 2024-05-29 21:26:19.000000 fullmonte-0.0.2/setup.py
```

### Comparing `fullmonte-0.0.1/LICENSE` & `fullmonte-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fullmonte-0.0.1/PKG-INFO` & `fullmonte-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: fullmonte
-Version: 0.0.1
+Version: 0.0.2
 Summary: A monte carlo simulation for extrapolated returns.
 Home-page: https://github.com/8W9aG/fullmonte
 Author: Will Sackfield
 Author-email: will.sackfield@gmail.com
 License: MIT
 Keywords: monte carlo
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=2.2.1
-Requires-Dist: numpy>=1.26.4
+Requires-Dist: numpy>=1.26.0
 Requires-Dist: matplotlib>=3.8.3
 
 # fullmonte
 
 <a href="https://pypi.org/project/fullmonte/">
     <img alt="PyPi" src="https://img.shields.io/pypi/v/fullmonte">
 </a>
 
 Monte Carlo simulations for extrapolated returns.
 
 ## Dependencies :globe_with_meridians:
 
 Python 3.11.6:
 
-- [numpy 1.26.4](https://numpy.org/)
+- [numpy 1.26.0](https://numpy.org/)
 - [pandas 2.2.1](https://pandas.pydata.org/)
 - [matplotlib 3.8.3](https://matplotlib.org/)
 
 ## Raison D'être :thought_balloon:
 
 fullmonte is a python library that implements the simulation and plotting of a monte carlo run on a financial return assuming normal distributions.
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: fullmonte Version: 0.0.1 Summary: A monte carlo
+Metadata-Version: 2.1 Name: fullmonte Version: 0.0.2 Summary: A monte carlo
 simulation for extrapolated returns. Home-page: https://github.com/8W9aG/
 fullmonte Author: Will Sackfield Author-email: will.sackfield@gmail.com
 License: MIT Keywords: monte carlo Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: pandas>=2.2.1
-Requires-Dist: numpy>=1.26.4 Requires-Dist: matplotlib>=3.8.3 # fullmonte
+Requires-Dist: numpy>=1.26.0 Requires-Dist: matplotlib>=3.8.3 # fullmonte
 _[_P_y_P_i_]Monte Carlo simulations for extrapolated returns. ## Dependencies :
-globe_with_meridians: Python 3.11.6: - [numpy 1.26.4](https://numpy.org/) -
+globe_with_meridians: Python 3.11.6: - [numpy 1.26.0](https://numpy.org/) -
 [pandas 2.2.1](https://pandas.pydata.org/) - [matplotlib 3.8.3](https://
 matplotlib.org/) ## Raison D'Ãªtre :thought_balloon: fullmonte is a python
 library that implements the simulation and plotting of a monte carlo run on a
 financial return assuming normal distributions. ## Installation :inbox_tray:
 This is a python package hosted on pypi, so to install simply run the following
 command: `pip install fullmonte` ## Usage example :eyes: A quick example of how
 to use this library is the following: ```python from fullmonte import simulate,
```

### Comparing `fullmonte-0.0.1/README.md` & `fullmonte-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Monte Carlo simulations for extrapolated returns.
 
 ## Dependencies :globe_with_meridians:
 
 Python 3.11.6:
 
-- [numpy 1.26.4](https://numpy.org/)
+- [numpy 1.26.0](https://numpy.org/)
 - [pandas 2.2.1](https://pandas.pydata.org/)
 - [matplotlib 3.8.3](https://matplotlib.org/)
 
 ## Raison D'être :thought_balloon:
 
 fullmonte is a python library that implements the simulation and plotting of a monte carlo run on a financial return assuming normal distributions.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # fullmonte _[_P_y_P_i_]Monte Carlo simulations for extrapolated returns. ##
-Dependencies :globe_with_meridians: Python 3.11.6: - [numpy 1.26.4](https://
+Dependencies :globe_with_meridians: Python 3.11.6: - [numpy 1.26.0](https://
 numpy.org/) - [pandas 2.2.1](https://pandas.pydata.org/) - [matplotlib 3.8.3]
 (https://matplotlib.org/) ## Raison D'Ãªtre :thought_balloon: fullmonte is a
 python library that implements the simulation and plotting of a monte carlo run
 on a financial return assuming normal distributions. ## Installation :
 inbox_tray: This is a python package hosted on pypi, so to install simply run
 the following command: `pip install fullmonte` ## Usage example :eyes: A quick
 example of how to use this library is the following: ```python from fullmonte
```

### Comparing `fullmonte-0.0.1/fullmonte/simulation.py` & `fullmonte-0.0.2/fullmonte/simulation.py`

 * *Files identical despite different names*

### Comparing `fullmonte-0.0.1/fullmonte.egg-info/PKG-INFO` & `fullmonte-0.0.2/fullmonte.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: fullmonte
-Version: 0.0.1
+Version: 0.0.2
 Summary: A monte carlo simulation for extrapolated returns.
 Home-page: https://github.com/8W9aG/fullmonte
 Author: Will Sackfield
 Author-email: will.sackfield@gmail.com
 License: MIT
 Keywords: monte carlo
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=2.2.1
-Requires-Dist: numpy>=1.26.4
+Requires-Dist: numpy>=1.26.0
 Requires-Dist: matplotlib>=3.8.3
 
 # fullmonte
 
 <a href="https://pypi.org/project/fullmonte/">
     <img alt="PyPi" src="https://img.shields.io/pypi/v/fullmonte">
 </a>
 
 Monte Carlo simulations for extrapolated returns.
 
 ## Dependencies :globe_with_meridians:
 
 Python 3.11.6:
 
-- [numpy 1.26.4](https://numpy.org/)
+- [numpy 1.26.0](https://numpy.org/)
 - [pandas 2.2.1](https://pandas.pydata.org/)
 - [matplotlib 3.8.3](https://matplotlib.org/)
 
 ## Raison D'être :thought_balloon:
 
 fullmonte is a python library that implements the simulation and plotting of a monte carlo run on a financial return assuming normal distributions.
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: fullmonte Version: 0.0.1 Summary: A monte carlo
+Metadata-Version: 2.1 Name: fullmonte Version: 0.0.2 Summary: A monte carlo
 simulation for extrapolated returns. Home-page: https://github.com/8W9aG/
 fullmonte Author: Will Sackfield Author-email: will.sackfield@gmail.com
 License: MIT Keywords: monte carlo Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: pandas>=2.2.1
-Requires-Dist: numpy>=1.26.4 Requires-Dist: matplotlib>=3.8.3 # fullmonte
+Requires-Dist: numpy>=1.26.0 Requires-Dist: matplotlib>=3.8.3 # fullmonte
 _[_P_y_P_i_]Monte Carlo simulations for extrapolated returns. ## Dependencies :
-globe_with_meridians: Python 3.11.6: - [numpy 1.26.4](https://numpy.org/) -
+globe_with_meridians: Python 3.11.6: - [numpy 1.26.0](https://numpy.org/) -
 [pandas 2.2.1](https://pandas.pydata.org/) - [matplotlib 3.8.3](https://
 matplotlib.org/) ## Raison D'Ãªtre :thought_balloon: fullmonte is a python
 library that implements the simulation and plotting of a monte carlo run on a
 financial return assuming normal distributions. ## Installation :inbox_tray:
 This is a python package hosted on pypi, so to install simply run the following
 command: `pip install fullmonte` ## Usage example :eyes: A quick example of how
 to use this library is the following: ```python from fullmonte import simulate,
```

### Comparing `fullmonte-0.0.1/setup.py` & `fullmonte-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             if not x.startswith(".") and not x.startswith("-e")
         ]
     return requires
 
 
 setup(
     name='fullmonte',
-    version='0.0.1',
+    version='0.0.2',
     description='A monte carlo simulation for extrapolated returns.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
```

