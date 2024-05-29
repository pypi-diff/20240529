# Comparing `tmp/gnosistech-1.0.0.tar.gz` & `tmp/gnosistech-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gnosistech-1.0.0.tar", last modified: Wed May 29 04:05:22 2024, max compression
+gzip compressed data, was "dist\gnosistech-1.0.1.tar", last modified: Wed May 29 04:10:18 2024, max compression
```

## Comparing `gnosistech-1.0.0.tar` & `gnosistech-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.683092 gnosistech-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.678886 gnosistech-1.0.0/GnosisTech.egg-info/
--rw-rw-rw-   0        0        0      416 2024-05-29 04:05:22.000000 gnosistech-1.0.0/GnosisTech.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2024-05-29 04:05:22.000000 gnosistech-1.0.0/GnosisTech.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 04:05:22.000000 gnosistech-1.0.0/GnosisTech.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 04:05:22.000000 gnosistech-1.0.0/GnosisTech.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       55 2024-05-29 02:36:41.000000 gnosistech-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      416 2024-05-29 04:05:22.680093 gnosistech-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.627737 gnosistech-1.0.0/pyquanttrade/
--rw-rw-rw-   0        0        0      368 2024-05-29 03:31:03.000000 gnosistech-1.0.0/pyquanttrade/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.649786 gnosistech-1.0.0/pyquanttrade/_backtest_source/
--rw-rw-rw-   0        0        0        0 2024-05-29 02:53:26.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/__init__.py
--rw-rw-rw-   0        0        0    30081 2024-05-29 02:53:24.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/_plotting.py
--rw-rw-rw-   0        0        0     6924 2024-05-29 02:53:27.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/_stats.py
--rw-rw-rw-   0        0        0     5915 2024-05-29 02:53:28.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/_util.py
--rw-rw-rw-   0        0        0     1236 2024-05-29 02:53:29.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/autoscale_cb.js
--rw-rw-rw-   0        0        0    16793 2024-05-29 03:05:18.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/lib.py
--rw-rw-rw-   0        0        0    72566 2024-05-29 03:05:20.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/source.py
-drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.657366 gnosistech-1.0.0/pyquanttrade/backtest/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:41:51.000000 gnosistech-1.0.0/pyquanttrade/backtest/__init__.py
--rw-rw-rw-   0        0        0      982 2024-05-29 03:05:23.000000 gnosistech-1.0.0/pyquanttrade/backtest/event_base.py
--rw-rw-rw-   0        0        0     4214 2024-05-29 03:05:21.000000 gnosistech-1.0.0/pyquanttrade/backtest/vectorized.py
-drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.664850 gnosistech-1.0.0/pyquanttrade/data/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:42:11.000000 gnosistech-1.0.0/pyquanttrade/data/__init__.py
--rw-rw-rw-   0        0        0     4228 2024-05-23 03:58:58.000000 gnosistech-1.0.0/pyquanttrade/data/get_data.py
-drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.672890 gnosistech-1.0.0/pyquanttrade/plotlib/
--rw-rw-rw-   0        0        0        0 2024-05-29 03:54:49.000000 gnosistech-1.0.0/pyquanttrade/plotlib/__init__.py
--rw-rw-rw-   0        0        0     7421 2024-05-29 03:30:57.000000 gnosistech-1.0.0/pyquanttrade/plotlib/plot.py
--rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 gnosistech-1.0.0/pyquanttrade/plotlib/ultils.py
--rw-rw-rw-   0        0        0       42 2024-05-29 04:05:22.683092 gnosistech-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      594 2024-05-29 03:59:42.000000 gnosistech-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.209015 gnosistech-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.205017 gnosistech-1.0.1/GnosisTech.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-05-29 04:10:17.000000 gnosistech-1.0.1/GnosisTech.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      745 2024-05-29 04:10:18.000000 gnosistech-1.0.1/GnosisTech.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 04:10:17.000000 gnosistech-1.0.1/GnosisTech.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 04:10:17.000000 gnosistech-1.0.1/GnosisTech.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       55 2024-05-29 02:36:41.000000 gnosistech-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      416 2024-05-29 04:10:18.207016 gnosistech-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.157644 gnosistech-1.0.1/pyquanttrade/
+-rw-rw-rw-   0        0        0      352 2024-05-29 04:09:17.000000 gnosistech-1.0.1/pyquanttrade/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.175635 gnosistech-1.0.1/pyquanttrade/_backtest_source/
+-rw-rw-rw-   0        0        0        0 2024-05-29 02:53:26.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/__init__.py
+-rw-rw-rw-   0        0        0    30081 2024-05-29 02:53:24.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/_plotting.py
+-rw-rw-rw-   0        0        0     6924 2024-05-29 02:53:27.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/_stats.py
+-rw-rw-rw-   0        0        0     5915 2024-05-29 02:53:28.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/_util.py
+-rw-rw-rw-   0        0        0     1236 2024-05-29 02:53:29.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/autoscale_cb.js
+-rw-rw-rw-   0        0        0    16793 2024-05-29 03:05:18.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/lib.py
+-rw-rw-rw-   0        0        0    72566 2024-05-29 03:05:20.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/source.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.188847 gnosistech-1.0.1/pyquanttrade/backtest/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:41:51.000000 gnosistech-1.0.1/pyquanttrade/backtest/__init__.py
+-rw-rw-rw-   0        0        0      982 2024-05-29 03:05:23.000000 gnosistech-1.0.1/pyquanttrade/backtest/event_base.py
+-rw-rw-rw-   0        0        0     4214 2024-05-29 03:05:21.000000 gnosistech-1.0.1/pyquanttrade/backtest/vectorized.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.194790 gnosistech-1.0.1/pyquanttrade/data/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:42:11.000000 gnosistech-1.0.1/pyquanttrade/data/__init__.py
+-rw-rw-rw-   0        0        0     2632 2024-05-29 04:09:22.000000 gnosistech-1.0.1/pyquanttrade/data/get_data.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.200019 gnosistech-1.0.1/pyquanttrade/plotlib/
+-rw-rw-rw-   0        0        0        0 2024-05-29 03:54:49.000000 gnosistech-1.0.1/pyquanttrade/plotlib/__init__.py
+-rw-rw-rw-   0        0        0     7421 2024-05-29 03:30:57.000000 gnosistech-1.0.1/pyquanttrade/plotlib/plot.py
+-rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 gnosistech-1.0.1/pyquanttrade/plotlib/ultils.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 04:10:18.209015 gnosistech-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      594 2024-05-29 04:10:13.000000 gnosistech-1.0.1/setup.py
```

### Comparing `gnosistech-1.0.0/GnosisTech.egg-info/SOURCES.txt` & `gnosistech-1.0.1/GnosisTech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.0/LICENSE` & `gnosistech-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.0/README.md` & `gnosistech-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.0/pyquanttrade/_backtest_source/_plotting.py` & `gnosistech-1.0.1/pyquanttrade/_backtest_source/_plotting.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.0/pyquanttrade/_backtest_source/_stats.py` & `gnosistech-1.0.1/pyquanttrade/_backtest_source/_stats.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.0/pyquanttrade/_backtest_source/_util.py` & `gnosistech-1.0.1/pyquanttrade/_backtest_source/_util.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.0/pyquanttrade/_backtest_source/autoscale_cb.js` & `gnosistech-1.0.1/pyquanttrade/_backtest_source/autoscale_cb.js`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.0/pyquanttrade/_backtest_source/lib.py` & `gnosistech-1.0.1/pyquanttrade/_backtest_source/lib.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.0/pyquanttrade/_backtest_source/source.py` & `gnosistech-1.0.1/pyquanttrade/_backtest_source/source.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.0/pyquanttrade/backtest/event_base.py` & `gnosistech-1.0.1/pyquanttrade/backtest/event_base.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.0/pyquanttrade/backtest/vectorized.py` & `gnosistech-1.0.1/pyquanttrade/backtest/vectorized.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.0/pyquanttrade/plotlib/plot.py` & `gnosistech-1.0.1/pyquanttrade/plotlib/plot.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.0/pyquanttrade/plotlib/ultils.py` & `gnosistech-1.0.1/pyquanttrade/plotlib/ultils.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.0/setup.py` & `gnosistech-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='GnosisTech',
-    version='1.0.0',
+    version='1.0.1',
     author='Phung Ngoc An',
     author_email='phungankh2@gmail.com',
     description='PyQuantTrader là một thư viện Python hỗ trợ những vấn đề về quant trading.',
     packages=find_packages(),
     package_data= {'pyquanttrade': ['_backtest_source/*.js']},       
     classifiers=[
         'Programming Language :: Python :: 3',
```

