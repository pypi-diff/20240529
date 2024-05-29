# Comparing `tmp/mirabolic-0.2.3.tar.gz` & `tmp/mirabolic-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirabolic-0.2.3.tar", last modified: Mon May 20 15:12:52 2024, max compression
+gzip compressed data, was "mirabolic-0.2.4.tar", last modified: Wed May 29 00:42:41 2024, max compression
```

## Comparing `mirabolic-0.2.3.tar` & `mirabolic-0.2.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 15:12:52.366087 mirabolic-0.2.3/
--rw-r--r--   0 wfbradley   (501) staff       (20)     1066 2022-12-13 21:29:13.000000 mirabolic-0.2.3/LICENSE
--rw-r--r--   0 wfbradley   (501) staff       (20)     8356 2024-05-20 15:12:52.365863 mirabolic-0.2.3/PKG-INFO
--rw-r--r--   0 wfbradley   (501) staff       (20)     7202 2024-05-20 04:06:56.000000 mirabolic-0.2.3/README.md
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 15:12:52.358247 mirabolic-0.2.3/mirabolic/
--rw-r--r--   0 wfbradley   (501) staff       (20)      342 2024-05-17 13:21:46.000000 mirabolic-0.2.3/mirabolic/__init__.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 15:12:52.360660 mirabolic-0.2.3/mirabolic/cdf/
--rw-r--r--   0 wfbradley   (501) staff       (20)     9850 2022-12-31 14:49:14.000000 mirabolic-0.2.3/mirabolic/cdf/cdf_tools.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     1923 2023-01-01 19:46:02.000000 mirabolic-0.2.3/mirabolic/cdf/sample_usage.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 15:12:52.361006 mirabolic-0.2.3/mirabolic/cdf/unit_tests/
--rw-r--r--   0 wfbradley   (501) staff       (20)     5054 2022-12-30 20:05:39.000000 mirabolic-0.2.3/mirabolic/cdf/unit_tests/test_cdf_tools.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 15:12:52.364251 mirabolic-0.2.3/mirabolic/neural_glm/
--rw-r--r--   0 wfbradley   (501) staff       (20)      313 2023-01-01 19:46:02.000000 mirabolic-0.2.3/mirabolic/neural_glm/__init__.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     8469 2022-12-13 21:29:13.000000 mirabolic-0.2.3/mirabolic/neural_glm/actuarial_loss_functions.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     4785 2023-01-01 19:46:02.000000 mirabolic-0.2.3/mirabolic/neural_glm/basic_glm_nn.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     4299 2022-12-13 21:29:13.000000 mirabolic-0.2.3/mirabolic/neural_glm/generate_synthetic_data.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     2183 2022-12-13 21:29:13.000000 mirabolic-0.2.3/mirabolic/neural_glm/run_examples.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 15:12:52.364844 mirabolic-0.2.3/mirabolic/rates/
--rw-r--r--   0 wfbradley   (501) staff       (20)     7979 2024-05-20 15:11:11.000000 mirabolic-0.2.3/mirabolic/rates/rate_tools.py
--rw-r--r--   0 wfbradley   (501) staff       (20)        6 2024-05-20 15:11:57.000000 mirabolic-0.2.3/mirabolic/version
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 15:12:52.365316 mirabolic-0.2.3/mirabolic.egg-info/
--rw-r--r--   0 wfbradley   (501) staff       (20)     8356 2024-05-20 15:12:52.000000 mirabolic-0.2.3/mirabolic.egg-info/PKG-INFO
--rw-r--r--   0 wfbradley   (501) staff       (20)      574 2024-05-20 15:12:52.000000 mirabolic-0.2.3/mirabolic.egg-info/SOURCES.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)        1 2024-05-20 15:12:52.000000 mirabolic-0.2.3/mirabolic.egg-info/dependency_links.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)       93 2024-05-20 15:12:52.000000 mirabolic-0.2.3/mirabolic.egg-info/requires.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)       10 2024-05-20 15:12:52.000000 mirabolic-0.2.3/mirabolic.egg-info/top_level.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)      103 2024-05-20 15:12:52.366559 mirabolic-0.2.3/setup.cfg
--rw-r--r--   0 wfbradley   (501) staff       (20)     2190 2022-12-31 16:39:50.000000 mirabolic-0.2.3/setup.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-29 00:42:41.514146 mirabolic-0.2.4/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     1066 2022-12-13 21:29:13.000000 mirabolic-0.2.4/LICENSE
+-rw-r--r--   0 wfbradley   (501) staff       (20)     8356 2024-05-29 00:42:41.513826 mirabolic-0.2.4/PKG-INFO
+-rw-r--r--   0 wfbradley   (501) staff       (20)     7202 2024-05-20 04:06:56.000000 mirabolic-0.2.4/README.md
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-29 00:42:41.503402 mirabolic-0.2.4/mirabolic/
+-rw-r--r--   0 wfbradley   (501) staff       (20)      342 2024-05-17 13:21:46.000000 mirabolic-0.2.4/mirabolic/__init__.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-29 00:42:41.506689 mirabolic-0.2.4/mirabolic/cdf/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     9850 2022-12-31 14:49:14.000000 mirabolic-0.2.4/mirabolic/cdf/cdf_tools.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     1923 2023-01-01 19:46:02.000000 mirabolic-0.2.4/mirabolic/cdf/sample_usage.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-29 00:42:41.507496 mirabolic-0.2.4/mirabolic/cdf/unit_tests/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     5054 2022-12-30 20:05:39.000000 mirabolic-0.2.4/mirabolic/cdf/unit_tests/test_cdf_tools.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-29 00:42:41.511601 mirabolic-0.2.4/mirabolic/neural_glm/
+-rw-r--r--   0 wfbradley   (501) staff       (20)      313 2023-01-01 19:46:02.000000 mirabolic-0.2.4/mirabolic/neural_glm/__init__.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     8469 2022-12-13 21:29:13.000000 mirabolic-0.2.4/mirabolic/neural_glm/actuarial_loss_functions.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     4785 2023-01-01 19:46:02.000000 mirabolic-0.2.4/mirabolic/neural_glm/basic_glm_nn.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     4299 2022-12-13 21:29:13.000000 mirabolic-0.2.4/mirabolic/neural_glm/generate_synthetic_data.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     2183 2022-12-13 21:29:13.000000 mirabolic-0.2.4/mirabolic/neural_glm/run_examples.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-29 00:42:41.512373 mirabolic-0.2.4/mirabolic/rates/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     7991 2024-05-29 00:40:53.000000 mirabolic-0.2.4/mirabolic/rates/rate_tools.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)        6 2024-05-29 00:41:32.000000 mirabolic-0.2.4/mirabolic/version
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-29 00:42:41.512982 mirabolic-0.2.4/mirabolic.egg-info/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     8356 2024-05-29 00:42:41.000000 mirabolic-0.2.4/mirabolic.egg-info/PKG-INFO
+-rw-r--r--   0 wfbradley   (501) staff       (20)      574 2024-05-29 00:42:41.000000 mirabolic-0.2.4/mirabolic.egg-info/SOURCES.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)        1 2024-05-29 00:42:41.000000 mirabolic-0.2.4/mirabolic.egg-info/dependency_links.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)       93 2024-05-29 00:42:41.000000 mirabolic-0.2.4/mirabolic.egg-info/requires.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)       10 2024-05-29 00:42:41.000000 mirabolic-0.2.4/mirabolic.egg-info/top_level.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)      103 2024-05-29 00:42:41.514725 mirabolic-0.2.4/setup.cfg
+-rw-r--r--   0 wfbradley   (501) staff       (20)     2190 2022-12-31 16:39:50.000000 mirabolic-0.2.4/setup.py
```

### Comparing `mirabolic-0.2.3/LICENSE` & `mirabolic-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.3/PKG-INFO` & `mirabolic-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mirabolic
-Version: 0.2.3
+Version: 0.2.4
 Summary: Statistical and Machine Learning tools from Mirabolic
 Home-page: https://github.com/Mirabolic/mirabolic
-Download-URL: https://github.com/Mirabolic/mirabolic/archive/refs/tags/v0.2.3.tar.gz
+Download-URL: https://github.com/Mirabolic/mirabolic/archive/refs/tags/v0.2.4.tar.gz
 Author: Bill Bradley
 License: MIT
 Keywords: Statistics,Machine Learning,CDF,Quantiles
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `mirabolic-0.2.3/README.md` & `mirabolic-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.3/mirabolic/cdf/cdf_tools.py` & `mirabolic-0.2.4/mirabolic/cdf/cdf_tools.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.3/mirabolic/cdf/sample_usage.py` & `mirabolic-0.2.4/mirabolic/cdf/sample_usage.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.3/mirabolic/cdf/unit_tests/test_cdf_tools.py` & `mirabolic-0.2.4/mirabolic/cdf/unit_tests/test_cdf_tools.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.3/mirabolic/neural_glm/actuarial_loss_functions.py` & `mirabolic-0.2.4/mirabolic/neural_glm/actuarial_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.3/mirabolic/neural_glm/basic_glm_nn.py` & `mirabolic-0.2.4/mirabolic/neural_glm/basic_glm_nn.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.3/mirabolic/neural_glm/generate_synthetic_data.py` & `mirabolic-0.2.4/mirabolic/neural_glm/generate_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.3/mirabolic/neural_glm/run_examples.py` & `mirabolic-0.2.4/mirabolic/neural_glm/run_examples.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.3/mirabolic/rates/rate_tools.py` & `mirabolic-0.2.4/mirabolic/rates/rate_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     if num_experiments == 0:
         raise ValueError("Must have at least 1 experiment!")
     for arm in arms:
         assert num_experiments == len(num_successes[arm])
         assert num_experiments == len(num_trials[arm])
         for i in range(num_experiments):
             assert num_trials[arm][i] >= 1
-    if labels:
+    if labels is not None:
         assert num_experiments == len(labels)
 
     assert confidence > 0
     assert confidence < 1
 
     #########################
     # Compute statistics
```

### Comparing `mirabolic-0.2.3/mirabolic.egg-info/PKG-INFO` & `mirabolic-0.2.4/mirabolic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mirabolic
-Version: 0.2.3
+Version: 0.2.4
 Summary: Statistical and Machine Learning tools from Mirabolic
 Home-page: https://github.com/Mirabolic/mirabolic
-Download-URL: https://github.com/Mirabolic/mirabolic/archive/refs/tags/v0.2.3.tar.gz
+Download-URL: https://github.com/Mirabolic/mirabolic/archive/refs/tags/v0.2.4.tar.gz
 Author: Bill Bradley
 License: MIT
 Keywords: Statistics,Machine Learning,CDF,Quantiles
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `mirabolic-0.2.3/mirabolic.egg-info/SOURCES.txt` & `mirabolic-0.2.4/mirabolic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.3/setup.py` & `mirabolic-0.2.4/setup.py`

 * *Files identical despite different names*

