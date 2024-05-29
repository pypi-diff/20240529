# Comparing `tmp/modelagnosticsafeaipackage-0.5.0.tar.gz` & `tmp/modelagnosticsafeaipackage-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelagnosticsafeaipackage-0.5.0.tar", last modified: Tue May 28 13:29:13 2024, max compression
+gzip compressed data, was "modelagnosticsafeaipackage-0.6.0.tar", last modified: Tue May 28 14:00:46 2024, max compression
```

## Comparing `modelagnosticsafeaipackage-0.5.0.tar` & `modelagnosticsafeaipackage-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 13:29:13.516978 modelagnosticsafeaipackage-0.5.0/
--rw-rw-rw-   0        0        0     1086 2024-05-26 18:09:20.000000 modelagnosticsafeaipackage-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     4988 2024-05-28 13:29:13.516978 modelagnosticsafeaipackage-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     4386 2024-05-28 09:08:56.000000 modelagnosticsafeaipackage-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 13:29:13.509972 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/
--rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/__init__.py
--rw-rw-rw-   0        0        0     3465 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/check_accuracy.py
--rw-rw-rw-   0        0        0     1338 2024-05-28 09:45:56.000000 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/check_explainability.py
--rw-rw-rw-   0        0        0     1298 2024-05-28 09:46:08.000000 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/check_fairness.py
--rw-rw-rw-   0        0        0     1293 2024-05-28 09:46:15.000000 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/check_privacy.py
--rw-rw-rw-   0        0        0     1495 2024-05-28 13:28:18.000000 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/check_robustness.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:29:13.515963 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/utils/
--rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/utils/__init__.py
--rw-rw-rw-   0        0        0     2799 2024-05-28 13:27:37.000000 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/utils/util.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:29:13.513919 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage.egg-info/
--rw-rw-rw-   0        0        0     4988 2024-05-28 13:29:13.000000 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2024-05-28 13:29:13.000000 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 13:29:13.000000 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-28 13:29:13.000000 modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 13:29:13.516978 modelagnosticsafeaipackage-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1117 2024-05-28 13:29:00.000000 modelagnosticsafeaipackage-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:00:46.281054 modelagnosticsafeaipackage-0.6.0/
+-rw-rw-rw-   0        0        0     1086 2024-05-26 18:09:20.000000 modelagnosticsafeaipackage-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     4988 2024-05-28 14:00:46.281054 modelagnosticsafeaipackage-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4386 2024-05-28 09:08:56.000000 modelagnosticsafeaipackage-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 14:00:46.274400 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/
+-rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/__init__.py
+-rw-rw-rw-   0        0        0     3465 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/check_accuracy.py
+-rw-rw-rw-   0        0        0     1338 2024-05-28 09:45:56.000000 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/check_explainability.py
+-rw-rw-rw-   0        0        0     1298 2024-05-28 09:46:08.000000 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/check_fairness.py
+-rw-rw-rw-   0        0        0     1293 2024-05-28 09:46:15.000000 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/check_privacy.py
+-rw-rw-rw-   0        0        0     1524 2024-05-28 13:59:45.000000 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/check_robustness.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:00:46.280051 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/utils/__init__.py
+-rw-rw-rw-   0        0        0     2799 2024-05-28 13:27:37.000000 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/utils/util.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:00:46.278678 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage.egg-info/
+-rw-rw-rw-   0        0        0     4988 2024-05-28 14:00:46.000000 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2024-05-28 14:00:46.000000 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 14:00:46.000000 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-28 14:00:46.000000 modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 14:00:46.281054 modelagnosticsafeaipackage-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2024-05-28 14:00:37.000000 modelagnosticsafeaipackage-0.6.0/setup.py
```

### Comparing `modelagnosticsafeaipackage-0.5.0/LICENSE` & `modelagnosticsafeaipackage-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.5.0/PKG-INFO` & `modelagnosticsafeaipackage-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelagnosticsafeaipackage
-Version: 0.5.0
+Version: 0.6.0
 Summary: MODEL AGNOSTIC SAFE AI package to measure risks of AI models WITHOUT CONSIDERING TYPE OF THE MODEL
 Author: Golnoosh Babaei
 Author-email: <golnoosh.babaei93@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `modelagnosticsafeaipackage-0.5.0/README.md` & `modelagnosticsafeaipackage-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/check_accuracy.py` & `modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/check_accuracy.py`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/check_explainability.py` & `modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/check_explainability.py`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/check_fairness.py` & `modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/check_fairness.py`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/check_privacy.py` & `modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/check_privacy.py`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/check_robustness.py` & `modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/check_robustness.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import numpy as np
 import scipy
 from .check_accuracy import rga
-from .utils.util import _delta_function
+from .utils.util import _delta_function, _rga_random
 
 def rgr(yhat, yhat_pert):
     """
         ### RANK GRADUATION Robustness (RGR) MEASURE ###
         Function for the RGR measure computation regarding perturbation of a single variable
     """ 
     rgr = rga(yhat, yhat_pert)
@@ -30,11 +30,11 @@
     jk_results = []
     for i in range(n):
         jk_sample = jk_mat.iloc[[x for x in index if x != i],:]
         jk_sample.reset_index(drop=True, inplace=True)
         jk_statistic = _delta_function(jk_sample, rgr)
         jk_results.append(jk_statistic)
     se = np.sqrt(((n-1)/n)*(sum([(x-np.mean(jk_results))**2 for x in jk_results])))
-    z = (rgr(yhat, yhat_pert)- rgr(yhat_mod2, yhat_mode2_pert))/se
+    z = (_rga_random(yhat, yhat_pert)- _rga_random(yhat_mod2, yhat_mode2_pert))/se
     p_value = 2*scipy.stats.norm.cdf(-abs(z))
         
     return p_value
```

### Comparing `modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage/utils/util.py` & `modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage/utils/util.py`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage.egg-info/PKG-INFO` & `modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelagnosticsafeaipackage
-Version: 0.5.0
+Version: 0.6.0
 Summary: MODEL AGNOSTIC SAFE AI package to measure risks of AI models WITHOUT CONSIDERING TYPE OF THE MODEL
 Author: Golnoosh Babaei
 Author-email: <golnoosh.babaei93@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `modelagnosticsafeaipackage-0.5.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt` & `modelagnosticsafeaipackage-0.6.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.5.0/setup.py` & `modelagnosticsafeaipackage-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 
 # Open README.md with UTF-8 encoding
 with open(this_directory / "README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '0.5.0'
+VERSION = '0.6.0'
 DESCRIPTION = 'MODEL AGNOSTIC SAFE AI package to measure risks of AI models WITHOUT CONSIDERING TYPE OF THE MODEL'
 
 # Setting up
 setup(
     name="modelagnosticsafeaipackage",
     version=VERSION,
     author="Golnoosh Babaei",
```

