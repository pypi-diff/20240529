# Comparing `tmp/gnosistech-0.1.6.tar.gz` & `tmp/gnosistech-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gnosistech-0.1.6.tar", last modified: Wed May 29 02:28:15 2024, max compression
+gzip compressed data, was "dist\gnosistech-0.1.7.tar", last modified: Wed May 29 02:38:32 2024, max compression
```

## Comparing `gnosistech-0.1.6.tar` & `gnosistech-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 02:28:15.394378 gnosistech-0.1.6/
-drwxrwxrwx   0        0        0        0 2024-05-29 02:28:15.390379 gnosistech-0.1.6/GnosisTech.egg-info/
--rw-rw-rw-   0        0        0      416 2024-05-29 02:28:14.000000 gnosistech-0.1.6/GnosisTech.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      736 2024-05-29 02:28:15.000000 gnosistech-0.1.6/GnosisTech.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 02:28:14.000000 gnosistech-0.1.6/GnosisTech.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 02:28:14.000000 gnosistech-0.1.6/GnosisTech.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       31 2024-05-28 10:06:02.000000 gnosistech-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      416 2024-05-29 02:28:15.392377 gnosistech-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 02:28:15.340408 gnosistech-0.1.6/pyquanttrade/
--rw-rw-rw-   0        0        0      532 2024-05-28 09:51:19.000000 gnosistech-0.1.6/pyquanttrade/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:28:15.363394 gnosistech-0.1.6/pyquanttrade/_backtest_source/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:41:32.000000 gnosistech-0.1.6/pyquanttrade/_backtest_source/__init__.py
--rw-rw-rw-   0        0        0    30081 2024-05-29 02:27:24.000000 gnosistech-0.1.6/pyquanttrade/_backtest_source/_plotting.py
--rw-rw-rw-   0        0        0     6924 2024-05-23 03:58:58.000000 gnosistech-0.1.6/pyquanttrade/_backtest_source/_stats.py
--rw-rw-rw-   0        0        0     5915 2024-05-23 03:58:58.000000 gnosistech-0.1.6/pyquanttrade/_backtest_source/_util.py
--rw-rw-rw-   0        0        0     1236 2024-05-23 03:58:58.000000 gnosistech-0.1.6/pyquanttrade/_backtest_source/autoscale_cb.js
--rw-rw-rw-   0        0        0    16793 2024-05-23 03:58:58.000000 gnosistech-0.1.6/pyquanttrade/_backtest_source/lib.py
--rw-rw-rw-   0        0        0    72566 2024-05-23 03:58:58.000000 gnosistech-0.1.6/pyquanttrade/_backtest_source/source.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:28:15.373388 gnosistech-0.1.6/pyquanttrade/backtest/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:41:51.000000 gnosistech-0.1.6/pyquanttrade/backtest/__init__.py
--rw-rw-rw-   0        0        0      969 2024-05-23 03:58:58.000000 gnosistech-0.1.6/pyquanttrade/backtest/event_base.py
--rw-rw-rw-   0        0        0     4188 2024-05-23 03:58:58.000000 gnosistech-0.1.6/pyquanttrade/backtest/vectorized.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:28:15.377386 gnosistech-0.1.6/pyquanttrade/data/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:42:11.000000 gnosistech-0.1.6/pyquanttrade/data/__init__.py
--rw-rw-rw-   0        0        0     4228 2024-05-23 03:58:58.000000 gnosistech-0.1.6/pyquanttrade/data/get_data.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:28:15.386382 gnosistech-0.1.6/pyquanttrade/plot/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:42:34.000000 gnosistech-0.1.6/pyquanttrade/plot/__init__.py
--rw-rw-rw-   0        0        0     7421 2024-05-26 09:16:51.000000 gnosistech-0.1.6/pyquanttrade/plot/plot.py
--rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 gnosistech-0.1.6/pyquanttrade/plot/ultils.py
--rw-rw-rw-   0        0        0       42 2024-05-29 02:28:15.394378 gnosistech-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-29 02:28:10.000000 gnosistech-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.260600 gnosistech-0.1.7/
+drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.255728 gnosistech-0.1.7/GnosisTech.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-05-29 02:38:31.000000 gnosistech-0.1.7/GnosisTech.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      736 2024-05-29 02:38:31.000000 gnosistech-0.1.7/GnosisTech.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 02:38:31.000000 gnosistech-0.1.7/GnosisTech.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 02:38:31.000000 gnosistech-0.1.7/GnosisTech.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       55 2024-05-29 02:36:41.000000 gnosistech-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      416 2024-05-29 02:38:32.257728 gnosistech-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.116690 gnosistech-0.1.7/pyquanttrade/
+-rw-rw-rw-   0        0        0      532 2024-05-28 09:51:19.000000 gnosistech-0.1.7/pyquanttrade/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.146227 gnosistech-0.1.7/pyquanttrade/_backtest_source/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:41:32.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/__init__.py
+-rw-rw-rw-   0        0        0    30081 2024-05-29 02:27:24.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/_plotting.py
+-rw-rw-rw-   0        0        0     6924 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/_stats.py
+-rw-rw-rw-   0        0        0     5915 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/_util.py
+-rw-rw-rw-   0        0        0     1236 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/autoscale_cb.js
+-rw-rw-rw-   0        0        0    16793 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/lib.py
+-rw-rw-rw-   0        0        0    72566 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/source.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.160108 gnosistech-0.1.7/pyquanttrade/backtest/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:41:51.000000 gnosistech-0.1.7/pyquanttrade/backtest/__init__.py
+-rw-rw-rw-   0        0        0      969 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/backtest/event_base.py
+-rw-rw-rw-   0        0        0     4188 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/backtest/vectorized.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.170230 gnosistech-0.1.7/pyquanttrade/data/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:42:11.000000 gnosistech-0.1.7/pyquanttrade/data/__init__.py
+-rw-rw-rw-   0        0        0     4228 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/data/get_data.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.252732 gnosistech-0.1.7/pyquanttrade/plot/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:42:34.000000 gnosistech-0.1.7/pyquanttrade/plot/__init__.py
+-rw-rw-rw-   0        0        0     7421 2024-05-26 09:16:51.000000 gnosistech-0.1.7/pyquanttrade/plot/plot.py
+-rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 gnosistech-0.1.7/pyquanttrade/plot/ultils.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 02:38:32.262273 gnosistech-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      594 2024-05-29 02:38:26.000000 gnosistech-0.1.7/setup.py
```

### Comparing `gnosistech-0.1.6/GnosisTech.egg-info/SOURCES.txt` & `gnosistech-0.1.7/GnosisTech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/LICENSE` & `gnosistech-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/README.md` & `gnosistech-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/pyquanttrade/__init__.py` & `gnosistech-0.1.7/pyquanttrade/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/pyquanttrade/_backtest_source/_plotting.py` & `gnosistech-0.1.7/pyquanttrade/_backtest_source/_plotting.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/pyquanttrade/_backtest_source/_stats.py` & `gnosistech-0.1.7/pyquanttrade/_backtest_source/_stats.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/pyquanttrade/_backtest_source/_util.py` & `gnosistech-0.1.7/pyquanttrade/_backtest_source/_util.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/pyquanttrade/_backtest_source/autoscale_cb.js` & `gnosistech-0.1.7/pyquanttrade/_backtest_source/autoscale_cb.js`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/pyquanttrade/_backtest_source/lib.py` & `gnosistech-0.1.7/pyquanttrade/_backtest_source/lib.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/pyquanttrade/_backtest_source/source.py` & `gnosistech-0.1.7/pyquanttrade/_backtest_source/source.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/pyquanttrade/backtest/event_base.py` & `gnosistech-0.1.7/pyquanttrade/backtest/event_base.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/pyquanttrade/backtest/vectorized.py` & `gnosistech-0.1.7/pyquanttrade/backtest/vectorized.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/pyquanttrade/data/get_data.py` & `gnosistech-0.1.7/pyquanttrade/data/get_data.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/pyquanttrade/plot/plot.py` & `gnosistech-0.1.7/pyquanttrade/plot/plot.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/pyquanttrade/plot/ultils.py` & `gnosistech-0.1.7/pyquanttrade/plot/ultils.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.6/setup.py` & `gnosistech-0.1.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 setup(
     name='GnosisTech',
-    version='0.1.6',
+    version='0.1.7',
     author='Phung Ngoc An',
     author_email='phungankh2@gmail.com',
     description='PyQuantTrader là một thư viện Python hỗ trợ những vấn đề về quant trading.',
     packages=find_packages(),
-    package_data= {'': ['*.json']},       
+    package_data= {'pyquanttrade': ['_backtest_source/*.js']},       
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
     python_requires='>=3.6',
 )
```

