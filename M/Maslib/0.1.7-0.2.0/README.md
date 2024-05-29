# Comparing `tmp/maslib-0.1.7.tar.gz` & `tmp/maslib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maslib-0.1.7.tar", last modified: Sun May 26 16:48:26 2024, max compression
+gzip compressed data, was "maslib-0.2.0.tar", last modified: Wed May 29 07:34:22 2024, max compression
```

## Comparing `maslib-0.1.7.tar` & `maslib-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 16:48:26.158263 maslib-0.1.7/
--rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 maslib-0.1.7/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-26 16:48:26.132239 maslib-0.1.7/MasLib/
--rw-rw-rw-   0        0        0     1289 2024-05-26 16:09:16.000000 maslib-0.1.7/MasLib/__init__.py
--rw-rw-rw-   0        0        0    19758 2024-05-26 09:46:27.000000 maslib-0.1.7/MasLib/classification.py
--rw-rw-rw-   0        0        0    10049 2024-05-26 09:34:23.000000 maslib-0.1.7/MasLib/clustering.py
--rw-rw-rw-   0        0        0     1820 2024-05-26 09:28:23.000000 maslib-0.1.7/MasLib/correlation.py
--rw-rw-rw-   0        0        0     3677 2024-05-26 09:52:52.000000 maslib-0.1.7/MasLib/encoding.py
--rw-rw-rw-   0        0        0      563 2024-05-26 09:24:37.000000 maslib-0.1.7/MasLib/loading.py
--rw-rw-rw-   0        0        0    10025 2024-05-26 09:23:11.000000 maslib-0.1.7/MasLib/regressions.py
--rw-rw-rw-   0        0        0    10975 2024-05-26 16:48:13.000000 maslib-0.1.7/MasLib/text_coding.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:48:26.154259 maslib-0.1.7/Maslib.egg-info/
--rw-rw-rw-   0        0        0      884 2024-05-26 16:48:25.000000 maslib-0.1.7/Maslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-05-26 16:48:25.000000 maslib-0.1.7/Maslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 16:48:25.000000 maslib-0.1.7/Maslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-05-26 16:48:25.000000 maslib-0.1.7/Maslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 16:48:25.000000 maslib-0.1.7/Maslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      884 2024-05-26 16:48:26.156261 maslib-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-26 09:52:47.000000 maslib-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 16:48:26.158263 maslib-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      806 2024-05-26 16:47:56.000000 maslib-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:48:26.152257 maslib-0.1.7/tests/
--rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 maslib-0.1.7/tests/test_clustering.py
--rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 maslib-0.1.7/tests/test_correlation.py
--rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 maslib-0.1.7/tests/test_encoding.py
--rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 maslib-0.1.7/tests/test_grid_search.py
--rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 maslib-0.1.7/tests/test_loading.py
--rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 maslib-0.1.7/tests/test_regression.py
--rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 maslib-0.1.7/tests/test_text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-29 07:34:22.874000 maslib-0.2.0/
+-rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 maslib-0.2.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-29 07:34:22.851265 maslib-0.2.0/MasLib/
+-rw-rw-rw-   0        0        0     1971 2024-05-29 07:32:45.000000 maslib-0.2.0/MasLib/__init__.py
+-rw-rw-rw-   0        0        0    19758 2024-05-26 09:46:27.000000 maslib-0.2.0/MasLib/classification.py
+-rw-rw-rw-   0        0        0    10049 2024-05-26 09:34:23.000000 maslib-0.2.0/MasLib/clustering.py
+-rw-rw-rw-   0        0        0     1820 2024-05-26 09:28:23.000000 maslib-0.2.0/MasLib/correlation.py
+-rw-rw-rw-   0        0        0     3677 2024-05-26 09:52:52.000000 maslib-0.2.0/MasLib/encoding.py
+-rw-rw-rw-   0        0        0      563 2024-05-26 09:24:37.000000 maslib-0.2.0/MasLib/loading.py
+-rw-rw-rw-   0        0        0    10025 2024-05-26 09:23:11.000000 maslib-0.2.0/MasLib/regressions.py
+-rw-rw-rw-   0        0        0    17434 2024-05-29 07:29:01.000000 maslib-0.2.0/MasLib/sql.py
+-rw-rw-rw-   0        0        0    10975 2024-05-26 16:48:13.000000 maslib-0.2.0/MasLib/text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-29 07:34:22.871999 maslib-0.2.0/Maslib.egg-info/
+-rw-rw-rw-   0        0        0     1057 2024-05-29 07:34:22.000000 maslib-0.2.0/Maslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2024-05-29 07:34:22.000000 maslib-0.2.0/Maslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 07:34:22.000000 maslib-0.2.0/Maslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-05-29 07:34:22.000000 maslib-0.2.0/Maslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-29 07:34:22.000000 maslib-0.2.0/Maslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1057 2024-05-29 07:34:22.872999 maslib-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-05-29 07:33:41.000000 maslib-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 07:34:22.874000 maslib-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      908 2024-05-29 07:30:00.000000 maslib-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 07:34:22.869996 maslib-0.2.0/tests/
+-rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 maslib-0.2.0/tests/test_clustering.py
+-rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 maslib-0.2.0/tests/test_correlation.py
+-rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 maslib-0.2.0/tests/test_encoding.py
+-rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 maslib-0.2.0/tests/test_grid_search.py
+-rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 maslib-0.2.0/tests/test_loading.py
+-rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 maslib-0.2.0/tests/test_regression.py
+-rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 maslib-0.2.0/tests/test_text_coding.py
```

### Comparing `maslib-0.1.7/MasLib/classification.py` & `maslib-0.2.0/MasLib/classification.py`

 * *Files identical despite different names*

### Comparing `maslib-0.1.7/MasLib/clustering.py` & `maslib-0.2.0/MasLib/clustering.py`

 * *Files identical despite different names*

### Comparing `maslib-0.1.7/MasLib/correlation.py` & `maslib-0.2.0/MasLib/correlation.py`

 * *Files identical despite different names*

### Comparing `maslib-0.1.7/MasLib/encoding.py` & `maslib-0.2.0/MasLib/encoding.py`

 * *Files identical despite different names*

### Comparing `maslib-0.1.7/MasLib/loading.py` & `maslib-0.2.0/MasLib/loading.py`

 * *Files identical despite different names*

### Comparing `maslib-0.1.7/MasLib/regressions.py` & `maslib-0.2.0/MasLib/regressions.py`

 * *Files identical despite different names*

### Comparing `maslib-0.1.7/MasLib/text_coding.py` & `maslib-0.2.0/MasLib/text_coding.py`

 * *Files identical despite different names*

### Comparing `maslib-0.1.7/Maslib.egg-info/PKG-INFO` & `maslib-0.2.0/Maslib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.1.7
+Version: 0.2.0
 Summary: This is a library for optimizing code for python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -15,19 +15,24 @@
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 Requires-Dist: catboost
 Requires-Dist: joblib
 Requires-Dist: wordcloud
 Requires-Dist: xgboost
 Requires-Dist: nltk
+Requires-Dist: pyodbc
+Requires-Dist: mysql-connector-python
+Requires-Dist: pymongo
+Requires-Dist: psycopg2-binary
 
 # MasLib
 
 MasLib - this is a Python library for code reduction
 
 My library can safely optimize everyday tasks for python
 
 There is no documentation yet, for understanding the library, see it in the code
+I'm not sure about the performance of the 2.0 version
 ## Installation
 
 ```bash
 pip install MasLib
```

### Comparing `maslib-0.1.7/Maslib.egg-info/SOURCES.txt` & `maslib-0.2.0/Maslib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 MasLib/__init__.py
 MasLib/classification.py
 MasLib/clustering.py
 MasLib/correlation.py
 MasLib/encoding.py
 MasLib/loading.py
 MasLib/regressions.py
+MasLib/sql.py
 MasLib/text_coding.py
 Maslib.egg-info/PKG-INFO
 Maslib.egg-info/SOURCES.txt
 Maslib.egg-info/dependency_links.txt
 Maslib.egg-info/requires.txt
 Maslib.egg-info/top_level.txt
 tests/test_clustering.py
```

### Comparing `maslib-0.1.7/PKG-INFO` & `maslib-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.1.7
+Version: 0.2.0
 Summary: This is a library for optimizing code for python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -15,19 +15,24 @@
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 Requires-Dist: catboost
 Requires-Dist: joblib
 Requires-Dist: wordcloud
 Requires-Dist: xgboost
 Requires-Dist: nltk
+Requires-Dist: pyodbc
+Requires-Dist: mysql-connector-python
+Requires-Dist: pymongo
+Requires-Dist: psycopg2-binary
 
 # MasLib
 
 MasLib - this is a Python library for code reduction
 
 My library can safely optimize everyday tasks for python
 
 There is no documentation yet, for understanding the library, see it in the code
+I'm not sure about the performance of the 2.0 version
 ## Installation
 
 ```bash
 pip install MasLib
```

### Comparing `maslib-0.1.7/tests/test_clustering.py` & `maslib-0.2.0/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `maslib-0.1.7/tests/test_correlation.py` & `maslib-0.2.0/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `maslib-0.1.7/tests/test_encoding.py` & `maslib-0.2.0/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `maslib-0.1.7/tests/test_grid_search.py` & `maslib-0.2.0/tests/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `maslib-0.1.7/tests/test_regression.py` & `maslib-0.2.0/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `maslib-0.1.7/tests/test_text_coding.py` & `maslib-0.2.0/tests/test_text_coding.py`

 * *Files identical despite different names*

