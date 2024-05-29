# Comparing `tmp/gnosistech-1.0.1.tar.gz` & `tmp/gnosistech-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gnosistech-1.0.1.tar", last modified: Wed May 29 04:10:18 2024, max compression
+gzip compressed data, was "dist\gnosistech-1.0.2.tar", last modified: Wed May 29 04:28:45 2024, max compression
```

## Comparing `gnosistech-1.0.1.tar` & `gnosistech-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.209015 gnosistech-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.205017 gnosistech-1.0.1/GnosisTech.egg-info/
--rw-rw-rw-   0        0        0      416 2024-05-29 04:10:17.000000 gnosistech-1.0.1/GnosisTech.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2024-05-29 04:10:18.000000 gnosistech-1.0.1/GnosisTech.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 04:10:17.000000 gnosistech-1.0.1/GnosisTech.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 04:10:17.000000 gnosistech-1.0.1/GnosisTech.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       55 2024-05-29 02:36:41.000000 gnosistech-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      416 2024-05-29 04:10:18.207016 gnosistech-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.157644 gnosistech-1.0.1/pyquanttrade/
--rw-rw-rw-   0        0        0      352 2024-05-29 04:09:17.000000 gnosistech-1.0.1/pyquanttrade/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.175635 gnosistech-1.0.1/pyquanttrade/_backtest_source/
--rw-rw-rw-   0        0        0        0 2024-05-29 02:53:26.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/__init__.py
--rw-rw-rw-   0        0        0    30081 2024-05-29 02:53:24.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/_plotting.py
--rw-rw-rw-   0        0        0     6924 2024-05-29 02:53:27.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/_stats.py
--rw-rw-rw-   0        0        0     5915 2024-05-29 02:53:28.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/_util.py
--rw-rw-rw-   0        0        0     1236 2024-05-29 02:53:29.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/autoscale_cb.js
--rw-rw-rw-   0        0        0    16793 2024-05-29 03:05:18.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/lib.py
--rw-rw-rw-   0        0        0    72566 2024-05-29 03:05:20.000000 gnosistech-1.0.1/pyquanttrade/_backtest_source/source.py
-drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.188847 gnosistech-1.0.1/pyquanttrade/backtest/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:41:51.000000 gnosistech-1.0.1/pyquanttrade/backtest/__init__.py
--rw-rw-rw-   0        0        0      982 2024-05-29 03:05:23.000000 gnosistech-1.0.1/pyquanttrade/backtest/event_base.py
--rw-rw-rw-   0        0        0     4214 2024-05-29 03:05:21.000000 gnosistech-1.0.1/pyquanttrade/backtest/vectorized.py
-drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.194790 gnosistech-1.0.1/pyquanttrade/data/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:42:11.000000 gnosistech-1.0.1/pyquanttrade/data/__init__.py
--rw-rw-rw-   0        0        0     2632 2024-05-29 04:09:22.000000 gnosistech-1.0.1/pyquanttrade/data/get_data.py
-drwxrwxrwx   0        0        0        0 2024-05-29 04:10:18.200019 gnosistech-1.0.1/pyquanttrade/plotlib/
--rw-rw-rw-   0        0        0        0 2024-05-29 03:54:49.000000 gnosistech-1.0.1/pyquanttrade/plotlib/__init__.py
--rw-rw-rw-   0        0        0     7421 2024-05-29 03:30:57.000000 gnosistech-1.0.1/pyquanttrade/plotlib/plot.py
--rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 gnosistech-1.0.1/pyquanttrade/plotlib/ultils.py
--rw-rw-rw-   0        0        0       42 2024-05-29 04:10:18.209015 gnosistech-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      594 2024-05-29 04:10:13.000000 gnosistech-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:28:45.285049 gnosistech-1.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-29 04:28:45.279055 gnosistech-1.0.2/GnosisTech.egg-info/
+-rw-rw-rw-   0        0        0      844 2024-05-29 04:28:44.000000 gnosistech-1.0.2/GnosisTech.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2024-05-29 04:28:45.000000 gnosistech-1.0.2/GnosisTech.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 04:28:44.000000 gnosistech-1.0.2/GnosisTech.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2024-05-29 04:28:44.000000 gnosistech-1.0.2/GnosisTech.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 04:28:44.000000 gnosistech-1.0.2/GnosisTech.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       55 2024-05-29 02:36:41.000000 gnosistech-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      844 2024-05-29 04:28:45.282051 gnosistech-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 04:28:45.235368 gnosistech-1.0.2/pyquanttrade/
+-rw-rw-rw-   0        0        0      352 2024-05-29 04:09:17.000000 gnosistech-1.0.2/pyquanttrade/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:28:45.256543 gnosistech-1.0.2/pyquanttrade/_backtest_source/
+-rw-rw-rw-   0        0        0        0 2024-05-29 02:53:26.000000 gnosistech-1.0.2/pyquanttrade/_backtest_source/__init__.py
+-rw-rw-rw-   0        0        0    30081 2024-05-29 02:53:24.000000 gnosistech-1.0.2/pyquanttrade/_backtest_source/_plotting.py
+-rw-rw-rw-   0        0        0     6924 2024-05-29 02:53:27.000000 gnosistech-1.0.2/pyquanttrade/_backtest_source/_stats.py
+-rw-rw-rw-   0        0        0     5915 2024-05-29 02:53:28.000000 gnosistech-1.0.2/pyquanttrade/_backtest_source/_util.py
+-rw-rw-rw-   0        0        0     1236 2024-05-29 02:53:29.000000 gnosistech-1.0.2/pyquanttrade/_backtest_source/autoscale_cb.js
+-rw-rw-rw-   0        0        0    16793 2024-05-29 03:05:18.000000 gnosistech-1.0.2/pyquanttrade/_backtest_source/lib.py
+-rw-rw-rw-   0        0        0    72566 2024-05-29 03:05:20.000000 gnosistech-1.0.2/pyquanttrade/_backtest_source/source.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:28:45.263843 gnosistech-1.0.2/pyquanttrade/backtest/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:41:51.000000 gnosistech-1.0.2/pyquanttrade/backtest/__init__.py
+-rw-rw-rw-   0        0        0      982 2024-05-29 03:05:23.000000 gnosistech-1.0.2/pyquanttrade/backtest/event_base.py
+-rw-rw-rw-   0        0        0     4214 2024-05-29 03:05:21.000000 gnosistech-1.0.2/pyquanttrade/backtest/vectorized.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:28:45.269922 gnosistech-1.0.2/pyquanttrade/data/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:42:11.000000 gnosistech-1.0.2/pyquanttrade/data/__init__.py
+-rw-rw-rw-   0        0        0     2632 2024-05-29 04:09:22.000000 gnosistech-1.0.2/pyquanttrade/data/get_data.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:28:45.277053 gnosistech-1.0.2/pyquanttrade/plotlib/
+-rw-rw-rw-   0        0        0        0 2024-05-29 03:54:49.000000 gnosistech-1.0.2/pyquanttrade/plotlib/__init__.py
+-rw-rw-rw-   0        0        0     7421 2024-05-29 03:30:57.000000 gnosistech-1.0.2/pyquanttrade/plotlib/plot.py
+-rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 gnosistech-1.0.2/pyquanttrade/plotlib/ultils.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 04:28:45.286049 gnosistech-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      756 2024-05-29 04:28:42.000000 gnosistech-1.0.2/setup.py
```

### Comparing `gnosistech-1.0.1/GnosisTech.egg-info/SOURCES.txt` & `gnosistech-1.0.2/GnosisTech.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 GnosisTech.egg-info/PKG-INFO
 GnosisTech.egg-info/SOURCES.txt
 GnosisTech.egg-info/dependency_links.txt
+GnosisTech.egg-info/requires.txt
 GnosisTech.egg-info/top_level.txt
 pyquanttrade/__init__.py
 pyquanttrade/_backtest_source/__init__.py
 pyquanttrade/_backtest_source/_plotting.py
 pyquanttrade/_backtest_source/_stats.py
 pyquanttrade/_backtest_source/_util.py
 pyquanttrade/_backtest_source/autoscale_cb.js
```

### Comparing `gnosistech-1.0.1/LICENSE` & `gnosistech-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.1/README.md` & `gnosistech-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.1/pyquanttrade/_backtest_source/_plotting.py` & `gnosistech-1.0.2/pyquanttrade/_backtest_source/_plotting.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.1/pyquanttrade/_backtest_source/_stats.py` & `gnosistech-1.0.2/pyquanttrade/_backtest_source/_stats.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.1/pyquanttrade/_backtest_source/_util.py` & `gnosistech-1.0.2/pyquanttrade/_backtest_source/_util.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.1/pyquanttrade/_backtest_source/autoscale_cb.js` & `gnosistech-1.0.2/pyquanttrade/_backtest_source/autoscale_cb.js`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.1/pyquanttrade/_backtest_source/lib.py` & `gnosistech-1.0.2/pyquanttrade/_backtest_source/lib.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.1/pyquanttrade/_backtest_source/source.py` & `gnosistech-1.0.2/pyquanttrade/_backtest_source/source.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.1/pyquanttrade/backtest/event_base.py` & `gnosistech-1.0.2/pyquanttrade/backtest/event_base.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.1/pyquanttrade/backtest/vectorized.py` & `gnosistech-1.0.2/pyquanttrade/backtest/vectorized.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.1/pyquanttrade/data/get_data.py` & `gnosistech-1.0.2/pyquanttrade/data/get_data.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.1/pyquanttrade/plotlib/plot.py` & `gnosistech-1.0.2/pyquanttrade/plotlib/plot.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.1/pyquanttrade/plotlib/ultils.py` & `gnosistech-1.0.2/pyquanttrade/plotlib/ultils.py`

 * *Files identical despite different names*

### Comparing `gnosistech-1.0.1/setup.py` & `gnosistech-1.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from setuptools import setup, find_packages
+
+def read_requirements():
+    with open('requirements.txt') as req_file:
+        return req_file.readlines()
+    
 setup(
+    install_requires=read_requirements(),
     name='GnosisTech',
-    version='1.0.1',
+    version='1.0.2',
     author='Phung Ngoc An',
     author_email='phungankh2@gmail.com',
     description='PyQuantTrader là một thư viện Python hỗ trợ những vấn đề về quant trading.',
     packages=find_packages(),
     package_data= {'pyquanttrade': ['_backtest_source/*.js']},       
     classifiers=[
         'Programming Language :: Python :: 3',
```

