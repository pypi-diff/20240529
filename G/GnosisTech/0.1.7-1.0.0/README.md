# Comparing `tmp/gnosistech-0.1.7.tar.gz` & `tmp/gnosistech-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gnosistech-0.1.7.tar", last modified: Wed May 29 02:38:32 2024, max compression
+gzip compressed data, was "dist\gnosistech-1.0.0.tar", last modified: Wed May 29 04:05:22 2024, max compression
```

## Comparing `gnosistech-0.1.7.tar` & `gnosistech-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.260600 gnosistech-0.1.7/
-drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.255728 gnosistech-0.1.7/GnosisTech.egg-info/
--rw-rw-rw-   0        0        0      416 2024-05-29 02:38:31.000000 gnosistech-0.1.7/GnosisTech.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      736 2024-05-29 02:38:31.000000 gnosistech-0.1.7/GnosisTech.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 02:38:31.000000 gnosistech-0.1.7/GnosisTech.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 02:38:31.000000 gnosistech-0.1.7/GnosisTech.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       55 2024-05-29 02:36:41.000000 gnosistech-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      416 2024-05-29 02:38:32.257728 gnosistech-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.116690 gnosistech-0.1.7/pyquanttrade/
--rw-rw-rw-   0        0        0      532 2024-05-28 09:51:19.000000 gnosistech-0.1.7/pyquanttrade/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.146227 gnosistech-0.1.7/pyquanttrade/_backtest_source/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:41:32.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/__init__.py
--rw-rw-rw-   0        0        0    30081 2024-05-29 02:27:24.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/_plotting.py
--rw-rw-rw-   0        0        0     6924 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/_stats.py
--rw-rw-rw-   0        0        0     5915 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/_util.py
--rw-rw-rw-   0        0        0     1236 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/autoscale_cb.js
--rw-rw-rw-   0        0        0    16793 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/lib.py
--rw-rw-rw-   0        0        0    72566 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/_backtest_source/source.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.160108 gnosistech-0.1.7/pyquanttrade/backtest/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:41:51.000000 gnosistech-0.1.7/pyquanttrade/backtest/__init__.py
--rw-rw-rw-   0        0        0      969 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/backtest/event_base.py
--rw-rw-rw-   0        0        0     4188 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/backtest/vectorized.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.170230 gnosistech-0.1.7/pyquanttrade/data/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:42:11.000000 gnosistech-0.1.7/pyquanttrade/data/__init__.py
--rw-rw-rw-   0        0        0     4228 2024-05-23 03:58:58.000000 gnosistech-0.1.7/pyquanttrade/data/get_data.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:38:32.252732 gnosistech-0.1.7/pyquanttrade/plot/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:42:34.000000 gnosistech-0.1.7/pyquanttrade/plot/__init__.py
--rw-rw-rw-   0        0        0     7421 2024-05-26 09:16:51.000000 gnosistech-0.1.7/pyquanttrade/plot/plot.py
--rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 gnosistech-0.1.7/pyquanttrade/plot/ultils.py
--rw-rw-rw-   0        0        0       42 2024-05-29 02:38:32.262273 gnosistech-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      594 2024-05-29 02:38:26.000000 gnosistech-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.683092 gnosistech-1.0.0/
+drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.678886 gnosistech-1.0.0/GnosisTech.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-05-29 04:05:22.000000 gnosistech-1.0.0/GnosisTech.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      745 2024-05-29 04:05:22.000000 gnosistech-1.0.0/GnosisTech.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 04:05:22.000000 gnosistech-1.0.0/GnosisTech.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 04:05:22.000000 gnosistech-1.0.0/GnosisTech.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       55 2024-05-29 02:36:41.000000 gnosistech-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      416 2024-05-29 04:05:22.680093 gnosistech-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.627737 gnosistech-1.0.0/pyquanttrade/
+-rw-rw-rw-   0        0        0      368 2024-05-29 03:31:03.000000 gnosistech-1.0.0/pyquanttrade/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.649786 gnosistech-1.0.0/pyquanttrade/_backtest_source/
+-rw-rw-rw-   0        0        0        0 2024-05-29 02:53:26.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/__init__.py
+-rw-rw-rw-   0        0        0    30081 2024-05-29 02:53:24.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/_plotting.py
+-rw-rw-rw-   0        0        0     6924 2024-05-29 02:53:27.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/_stats.py
+-rw-rw-rw-   0        0        0     5915 2024-05-29 02:53:28.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/_util.py
+-rw-rw-rw-   0        0        0     1236 2024-05-29 02:53:29.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/autoscale_cb.js
+-rw-rw-rw-   0        0        0    16793 2024-05-29 03:05:18.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/lib.py
+-rw-rw-rw-   0        0        0    72566 2024-05-29 03:05:20.000000 gnosistech-1.0.0/pyquanttrade/_backtest_source/source.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.657366 gnosistech-1.0.0/pyquanttrade/backtest/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:41:51.000000 gnosistech-1.0.0/pyquanttrade/backtest/__init__.py
+-rw-rw-rw-   0        0        0      982 2024-05-29 03:05:23.000000 gnosistech-1.0.0/pyquanttrade/backtest/event_base.py
+-rw-rw-rw-   0        0        0     4214 2024-05-29 03:05:21.000000 gnosistech-1.0.0/pyquanttrade/backtest/vectorized.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.664850 gnosistech-1.0.0/pyquanttrade/data/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:42:11.000000 gnosistech-1.0.0/pyquanttrade/data/__init__.py
+-rw-rw-rw-   0        0        0     4228 2024-05-23 03:58:58.000000 gnosistech-1.0.0/pyquanttrade/data/get_data.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:05:22.672890 gnosistech-1.0.0/pyquanttrade/plotlib/
+-rw-rw-rw-   0        0        0        0 2024-05-29 03:54:49.000000 gnosistech-1.0.0/pyquanttrade/plotlib/__init__.py
+-rw-rw-rw-   0        0        0     7421 2024-05-29 03:30:57.000000 gnosistech-1.0.0/pyquanttrade/plotlib/plot.py
+-rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 gnosistech-1.0.0/pyquanttrade/plotlib/ultils.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 04:05:22.683092 gnosistech-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      594 2024-05-29 03:59:42.000000 gnosistech-1.0.0/setup.py
```

### Comparing `gnosistech-0.1.7/GnosisTech.egg-info/SOURCES.txt` & `gnosistech-1.0.0/GnosisTech.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 pyquanttrade/_backtest_source/lib.py
 pyquanttrade/_backtest_source/source.py
 pyquanttrade/backtest/__init__.py
 pyquanttrade/backtest/event_base.py
 pyquanttrade/backtest/vectorized.py
 pyquanttrade/data/__init__.py
 pyquanttrade/data/get_data.py
-pyquanttrade/plot/__init__.py
-pyquanttrade/plot/plot.py
-pyquanttrade/plot/ultils.py
+pyquanttrade/plotlib/__init__.py
+pyquanttrade/plotlib/plot.py
+pyquanttrade/plotlib/ultils.py
```

### Comparing `gnosistech-0.1.7/LICENSE` & `gnosistech-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.7/README.md` & `gnosistech-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.7/pyquanttrade/_backtest_source/_plotting.py` & `gnosistech-1.0.0/pyquanttrade/_backtest_source/_plotting.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.7/pyquanttrade/_backtest_source/_stats.py` & `gnosistech-1.0.0/pyquanttrade/_backtest_source/_stats.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.7/pyquanttrade/_backtest_source/_util.py` & `gnosistech-1.0.0/pyquanttrade/_backtest_source/_util.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.7/pyquanttrade/_backtest_source/autoscale_cb.js` & `gnosistech-1.0.0/pyquanttrade/_backtest_source/autoscale_cb.js`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.7/pyquanttrade/_backtest_source/lib.py` & `gnosistech-1.0.0/pyquanttrade/_backtest_source/lib.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.7/pyquanttrade/_backtest_source/source.py` & `gnosistech-1.0.0/pyquanttrade/_backtest_source/source.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.7/pyquanttrade/backtest/event_base.py` & `gnosistech-1.0.0/pyquanttrade/backtest/event_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from _backtest_source.source import Backtest, Strategy
+from pyquanttrade._backtest_source.source import Backtest, Strategy
 
 def use_changes(data, changes):
     """
     Sử dụng chiến lược dựa trên thay đổi giá và thực hiện backtest.
 
     Parameters:
         data (DataFrame): Dữ liệu chứa giá.
```

### Comparing `gnosistech-0.1.7/pyquanttrade/backtest/vectorized.py` & `gnosistech-1.0.0/pyquanttrade/backtest/vectorized.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
-from _backtest_source.source import Backtest, Strategy
-from _backtest_source.lib import SignalStrategy, TrailingStrategy
+from pyquanttrade._backtest_source.source import Backtest, Strategy
+from pyquanttrade._backtest_source.lib import SignalStrategy, TrailingStrategy
 
 def use_position(data, pos_array):
     """
     Sử dụng tín hiệu mua/bán từ một mảng và thực hiện backtest.
 
     Parameters:
         data (DataFrame): Dữ liệu chứa giá và tín hiệu.
```

### Comparing `gnosistech-0.1.7/pyquanttrade/data/get_data.py` & `gnosistech-1.0.0/pyquanttrade/data/get_data.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.7/pyquanttrade/plot/plot.py` & `gnosistech-1.0.0/pyquanttrade/plotlib/plot.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.7/pyquanttrade/plot/ultils.py` & `gnosistech-1.0.0/pyquanttrade/plotlib/ultils.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.7/setup.py` & `gnosistech-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='GnosisTech',
-    version='0.1.7',
+    version='1.0.0',
     author='Phung Ngoc An',
     author_email='phungankh2@gmail.com',
     description='PyQuantTrader là một thư viện Python hỗ trợ những vấn đề về quant trading.',
     packages=find_packages(),
     package_data= {'pyquanttrade': ['_backtest_source/*.js']},       
     classifiers=[
         'Programming Language :: Python :: 3',
```

