# Comparing `tmp/khipu_metabolomics-2.0.0.tar.gz` & `tmp/khipu_metabolomics-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khipu_metabolomics-2.0.0.tar", last modified: Tue Apr 30 00:39:17 2024, max compression
+gzip compressed data, was "khipu_metabolomics-2.0.1.tar", last modified: Wed May 29 21:24:05 2024, max compression
```

## Comparing `khipu_metabolomics-2.0.0.tar` & `khipu_metabolomics-2.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-30 00:39:17.481614 khipu_metabolomics-2.0.0/
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)      360 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/LICENSE
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       38 2023-09-18 15:05:27.000000 khipu_metabolomics-2.0.0/MANIFEST.in
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     9717 2024-04-30 00:39:17.480933 khipu_metabolomics-2.0.0/PKG-INFO
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     8803 2024-04-30 00:36:50.000000 khipu_metabolomics-2.0.0/README.md
-drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-30 00:39:17.463256 khipu_metabolomics-2.0.0/khipu/
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       68 2024-04-30 00:31:29.000000 khipu_metabolomics-2.0.0/khipu/__init__.py
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    18736 2024-04-30 00:21:47.000000 khipu_metabolomics-2.0.0/khipu/analysis.py
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       24 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/khipu/command_line.py
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     3913 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/khipu/epdsConstructor.py
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    13754 2024-04-25 13:06:56.000000 khipu_metabolomics-2.0.0/khipu/extended.py
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     5531 2023-10-02 02:43:08.000000 khipu_metabolomics-2.0.0/khipu/formula_filter.py
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    11636 2024-04-30 00:21:47.000000 khipu_metabolomics-2.0.0/khipu/isotopes.py
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     1607 2024-04-25 13:06:56.000000 khipu_metabolomics-2.0.0/khipu/main.py
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    30719 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/khipu/model.py
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     3383 2023-09-29 15:48:17.000000 khipu_metabolomics-2.0.0/khipu/plot.py
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     4360 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/khipu/test.py
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)  7428142 2023-10-02 02:04:57.000000 khipu_metabolomics-2.0.0/khipu/tree_formulas.py
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    24528 2024-04-25 13:06:56.000000 khipu_metabolomics-2.0.0/khipu/utils.py
-drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-30 00:39:17.480309 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     9717 2024-04-30 00:39:17.000000 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/PKG-INFO
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)      547 2024-04-30 00:39:17.000000 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/SOURCES.txt
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        1 2024-04-30 00:39:17.000000 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/dependency_links.txt
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       50 2024-04-30 00:39:17.000000 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/entry_points.txt
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       27 2024-04-30 00:39:17.000000 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/requires.txt
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        6 2024-04-30 00:39:17.000000 khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/top_level.txt
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       67 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/requirements.txt
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       38 2024-04-30 00:39:17.481685 khipu_metabolomics-2.0.0/setup.cfg
--rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     1412 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.0/setup.py
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-05-29 21:24:05.650259 khipu_metabolomics-2.0.1/
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)      360 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.1/LICENSE
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       38 2023-09-18 15:05:27.000000 khipu_metabolomics-2.0.1/MANIFEST.in
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     9717 2024-05-29 21:24:05.649660 khipu_metabolomics-2.0.1/PKG-INFO
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     8803 2024-04-30 00:36:50.000000 khipu_metabolomics-2.0.1/README.md
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-05-29 21:24:05.646152 khipu_metabolomics-2.0.1/khipu/
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       69 2024-05-29 21:22:08.000000 khipu_metabolomics-2.0.1/khipu/__init__.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    18736 2024-04-30 00:21:47.000000 khipu_metabolomics-2.0.1/khipu/analysis.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       24 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.1/khipu/command_line.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     3913 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.1/khipu/epdsConstructor.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    13754 2024-04-25 13:06:56.000000 khipu_metabolomics-2.0.1/khipu/extended.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     5531 2023-10-02 02:43:08.000000 khipu_metabolomics-2.0.1/khipu/formula_filter.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    11636 2024-05-29 21:22:08.000000 khipu_metabolomics-2.0.1/khipu/isotopes.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     1607 2024-04-25 13:06:56.000000 khipu_metabolomics-2.0.1/khipu/main.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    30719 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.1/khipu/model.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     3383 2023-09-29 15:48:17.000000 khipu_metabolomics-2.0.1/khipu/plot.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     4360 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.1/khipu/test.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)  7428142 2023-10-02 02:04:57.000000 khipu_metabolomics-2.0.1/khipu/tree_formulas.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)    24528 2024-04-25 13:06:56.000000 khipu_metabolomics-2.0.1/khipu/utils.py
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-05-29 21:24:05.649212 khipu_metabolomics-2.0.1/khipu_metabolomics.egg-info/
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     9717 2024-05-29 21:24:05.000000 khipu_metabolomics-2.0.1/khipu_metabolomics.egg-info/PKG-INFO
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)      547 2024-05-29 21:24:05.000000 khipu_metabolomics-2.0.1/khipu_metabolomics.egg-info/SOURCES.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        1 2024-05-29 21:24:05.000000 khipu_metabolomics-2.0.1/khipu_metabolomics.egg-info/dependency_links.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       50 2024-05-29 21:24:05.000000 khipu_metabolomics-2.0.1/khipu_metabolomics.egg-info/entry_points.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       27 2024-05-29 21:24:05.000000 khipu_metabolomics-2.0.1/khipu_metabolomics.egg-info/requires.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        6 2024-05-29 21:24:05.000000 khipu_metabolomics-2.0.1/khipu_metabolomics.egg-info/top_level.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       67 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.1/requirements.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       38 2024-05-29 21:24:05.650299 khipu_metabolomics-2.0.1/setup.cfg
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     1412 2023-09-29 14:47:06.000000 khipu_metabolomics-2.0.1/setup.py
```

### Comparing `khipu_metabolomics-2.0.0/PKG-INFO` & `khipu_metabolomics-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khipu-metabolomics
-Version: 2.0.0
+Version: 2.0.1
 Summary: Common utilities for interpreting mass spectrometry data
 Home-page: https://github.com/shuzhao-li/khipu
 Author: Shuzhao Li
 Author-email: shuzhao.li@gmail.com
 License: BSD
 Keywords: chemistry,bioinformatics,mass spectrometry
 Classifier: Development Status :: 4 - Beta
```

### Comparing `khipu_metabolomics-2.0.0/README.md` & `khipu_metabolomics-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `khipu_metabolomics-2.0.0/khipu/analysis.py` & `khipu_metabolomics-2.0.1/khipu/analysis.py`

 * *Files identical despite different names*

### Comparing `khipu_metabolomics-2.0.0/khipu/epdsConstructor.py` & `khipu_metabolomics-2.0.1/khipu/epdsConstructor.py`

 * *Files identical despite different names*

### Comparing `khipu_metabolomics-2.0.0/khipu/extended.py` & `khipu_metabolomics-2.0.1/khipu/extended.py`

 * *Files identical despite different names*

### Comparing `khipu_metabolomics-2.0.0/khipu/formula_filter.py` & `khipu_metabolomics-2.0.1/khipu/formula_filter.py`

 * *Files identical despite different names*

### Comparing `khipu_metabolomics-2.0.0/khipu/isotopes.py` & `khipu_metabolomics-2.0.1/khipu/isotopes.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import pandas as pd
 import numpy as np
 
 # this is a master list of isotopes sourced from NIST
 # update this if the NAPs in yours system are non-canonical
 # see the function below on how to override this list.
 
-ISOTOPE_RAW_DATA = """
-    element,mass,abundance
+ISOTOPE_RAW_DATA = """element,mass,abundance
     H,1.00782503223,0.999885
     H,2.01410177812,0.000115
     He,3.0160293201,1.34e-06
     He,4.00260325413,0.99999866
     Li,6.0151228874,0.0759
     Li,7.0160034366,0.9241
     Be,9.012183065,1.0
@@ -383,16 +382,15 @@
     Bi,208.9803991,1.0
     Th,232.0380558,1.0
     Pa,231.0358842,1.0
     U,234.0409523,5.4e-05
     U,235.0439301,0.007204
     U,236.0000,0.0000
     U,237.0000,0.0000
-    U,238.0507884,0.992742
-"""
+    U,238.0507884,0.992742"""
 
 def get_isotope_data(data_path=None):
     """
     This function parses either the ISOTOPE_RAW_DATA above or the provided
     csv file provided by data_path and returns the data properly formatted
     for use by isocor.
 
@@ -419,23 +417,23 @@
             dg = gb.get_group(g).sort_values(by='mass').to_dict('list')
             e = dg.pop('element')[0]
             d[e] = dg
         return d
     
     if data_path is None:
         parsed_data = []
-        iso_data = ISOTOPE_RAW_DATA[0].strip()
+        iso_data = ISOTOPE_RAW_DATA[0].split("\n")
         for line in iso_data[1:]:
             element, mass, abundance = line.strip().split(",")
-            dfIsotopes.append({
+            parsed_data.append({
                 "element": element,
                 "mass": Decimal(mass),
                 "abundance": np.float64(abundance)
             })
         dfIsotopes = pd.DataFrame(parsed_data)
     else:
         with open(str(data_path), 'r', encoding='utf-8') as fp:
             dfIsotopes = pd.read_csv(fp, converters={'mass': Decimal, 'abundance': np.float64})
     _stripColNames(dfIsotopes)
     _stripCol(dfIsotopes, ['element', ])
     dictIsotopes = _makeIsotopesDict(dfIsotopes)
-    return dictIsotopes
+    return dictIsotopes
```

### Comparing `khipu_metabolomics-2.0.0/khipu/main.py` & `khipu_metabolomics-2.0.1/khipu/main.py`

 * *Files identical despite different names*

### Comparing `khipu_metabolomics-2.0.0/khipu/model.py` & `khipu_metabolomics-2.0.1/khipu/model.py`

 * *Files identical despite different names*

### Comparing `khipu_metabolomics-2.0.0/khipu/plot.py` & `khipu_metabolomics-2.0.1/khipu/plot.py`

 * *Files identical despite different names*

### Comparing `khipu_metabolomics-2.0.0/khipu/test.py` & `khipu_metabolomics-2.0.1/khipu/test.py`

 * *Files identical despite different names*

### Comparing `khipu_metabolomics-2.0.0/khipu/tree_formulas.py` & `khipu_metabolomics-2.0.1/khipu/tree_formulas.py`

 * *Files identical despite different names*

### Comparing `khipu_metabolomics-2.0.0/khipu/utils.py` & `khipu_metabolomics-2.0.1/khipu/utils.py`

 * *Files identical despite different names*

### Comparing `khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/PKG-INFO` & `khipu_metabolomics-2.0.1/khipu_metabolomics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khipu-metabolomics
-Version: 2.0.0
+Version: 2.0.1
 Summary: Common utilities for interpreting mass spectrometry data
 Home-page: https://github.com/shuzhao-li/khipu
 Author: Shuzhao Li
 Author-email: shuzhao.li@gmail.com
 License: BSD
 Keywords: chemistry,bioinformatics,mass spectrometry
 Classifier: Development Status :: 4 - Beta
```

### Comparing `khipu_metabolomics-2.0.0/khipu_metabolomics.egg-info/SOURCES.txt` & `khipu_metabolomics-2.0.1/khipu_metabolomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khipu_metabolomics-2.0.0/setup.py` & `khipu_metabolomics-2.0.1/setup.py`

 * *Files identical despite different names*

