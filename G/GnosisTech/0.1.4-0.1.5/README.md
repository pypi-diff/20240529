# Comparing `tmp/gnosistech-0.1.4.tar.gz` & `tmp/gnosistech-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gnosistech-0.1.4.tar", last modified: Wed May 29 02:20:56 2024, max compression
+gzip compressed data, was "dist\gnosistech-0.1.5.tar", last modified: Wed May 29 02:24:04 2024, max compression
```

## Comparing `gnosistech-0.1.4.tar` & `gnosistech-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.751957 gnosistech-0.1.4/
-drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.747916 gnosistech-0.1.4/GnosisTech.egg-info/
--rw-rw-rw-   0        0        0      416 2024-05-29 02:20:56.000000 gnosistech-0.1.4/GnosisTech.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      736 2024-05-29 02:20:56.000000 gnosistech-0.1.4/GnosisTech.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 02:20:56.000000 gnosistech-0.1.4/GnosisTech.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 02:20:56.000000 gnosistech-0.1.4/GnosisTech.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       31 2024-05-28 10:06:02.000000 gnosistech-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      416 2024-05-29 02:20:56.750230 gnosistech-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.698981 gnosistech-0.1.4/pyquanttrade/
--rw-rw-rw-   0        0        0      532 2024-05-28 09:51:19.000000 gnosistech-0.1.4/pyquanttrade/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.725424 gnosistech-0.1.4/pyquanttrade/_backtest_source/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:41:32.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/__init__.py
--rw-rw-rw-   0        0        0    30092 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/_plotting.py
--rw-rw-rw-   0        0        0     6924 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/_stats.py
--rw-rw-rw-   0        0        0     5915 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/_util.py
--rw-rw-rw-   0        0        0     1236 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/autoscale_cb.js
--rw-rw-rw-   0        0        0    16793 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/lib.py
--rw-rw-rw-   0        0        0    72566 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/source.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.731600 gnosistech-0.1.4/pyquanttrade/backtest/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:41:51.000000 gnosistech-0.1.4/pyquanttrade/backtest/__init__.py
--rw-rw-rw-   0        0        0      969 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/backtest/event_base.py
--rw-rw-rw-   0        0        0     4188 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/backtest/vectorized.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.736598 gnosistech-0.1.4/pyquanttrade/data/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:42:11.000000 gnosistech-0.1.4/pyquanttrade/data/__init__.py
--rw-rw-rw-   0        0        0     4228 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/data/get_data.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.745918 gnosistech-0.1.4/pyquanttrade/plot/
--rw-rw-rw-   0        0        0        0 2024-05-28 09:42:34.000000 gnosistech-0.1.4/pyquanttrade/plot/__init__.py
--rw-rw-rw-   0        0        0     7421 2024-05-26 09:16:51.000000 gnosistech-0.1.4/pyquanttrade/plot/plot.py
--rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 gnosistech-0.1.4/pyquanttrade/plot/ultils.py
--rw-rw-rw-   0        0        0       42 2024-05-29 02:20:56.751957 gnosistech-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-29 02:20:44.000000 gnosistech-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:24:04.260750 gnosistech-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-05-29 02:24:04.255751 gnosistech-0.1.5/GnosisTech.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-05-29 02:24:03.000000 gnosistech-0.1.5/GnosisTech.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      736 2024-05-29 02:24:04.000000 gnosistech-0.1.5/GnosisTech.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 02:24:03.000000 gnosistech-0.1.5/GnosisTech.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 02:24:03.000000 gnosistech-0.1.5/GnosisTech.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       31 2024-05-28 10:06:02.000000 gnosistech-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      416 2024-05-29 02:24:04.258750 gnosistech-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 02:24:04.211777 gnosistech-0.1.5/pyquanttrade/
+-rw-rw-rw-   0        0        0      532 2024-05-28 09:51:19.000000 gnosistech-0.1.5/pyquanttrade/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:24:04.232765 gnosistech-0.1.5/pyquanttrade/_backtest_source/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:41:32.000000 gnosistech-0.1.5/pyquanttrade/_backtest_source/__init__.py
+-rw-rw-rw-   0        0        0    30097 2024-05-29 02:23:26.000000 gnosistech-0.1.5/pyquanttrade/_backtest_source/_plotting.py
+-rw-rw-rw-   0        0        0     6924 2024-05-23 03:58:58.000000 gnosistech-0.1.5/pyquanttrade/_backtest_source/_stats.py
+-rw-rw-rw-   0        0        0     5915 2024-05-23 03:58:58.000000 gnosistech-0.1.5/pyquanttrade/_backtest_source/_util.py
+-rw-rw-rw-   0        0        0     1236 2024-05-23 03:58:58.000000 gnosistech-0.1.5/pyquanttrade/_backtest_source/autoscale_cb.js
+-rw-rw-rw-   0        0        0    16793 2024-05-23 03:58:58.000000 gnosistech-0.1.5/pyquanttrade/_backtest_source/lib.py
+-rw-rw-rw-   0        0        0    72566 2024-05-23 03:58:58.000000 gnosistech-0.1.5/pyquanttrade/_backtest_source/source.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:24:04.238762 gnosistech-0.1.5/pyquanttrade/backtest/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:41:51.000000 gnosistech-0.1.5/pyquanttrade/backtest/__init__.py
+-rw-rw-rw-   0        0        0      969 2024-05-23 03:58:58.000000 gnosistech-0.1.5/pyquanttrade/backtest/event_base.py
+-rw-rw-rw-   0        0        0     4188 2024-05-23 03:58:58.000000 gnosistech-0.1.5/pyquanttrade/backtest/vectorized.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:24:04.243759 gnosistech-0.1.5/pyquanttrade/data/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:42:11.000000 gnosistech-0.1.5/pyquanttrade/data/__init__.py
+-rw-rw-rw-   0        0        0     4228 2024-05-23 03:58:58.000000 gnosistech-0.1.5/pyquanttrade/data/get_data.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:24:04.252753 gnosistech-0.1.5/pyquanttrade/plot/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:42:34.000000 gnosistech-0.1.5/pyquanttrade/plot/__init__.py
+-rw-rw-rw-   0        0        0     7421 2024-05-26 09:16:51.000000 gnosistech-0.1.5/pyquanttrade/plot/plot.py
+-rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 gnosistech-0.1.5/pyquanttrade/plot/ultils.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 02:24:04.260750 gnosistech-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-29 02:23:55.000000 gnosistech-0.1.5/setup.py
```

### Comparing `gnosistech-0.1.4/GnosisTech.egg-info/SOURCES.txt` & `gnosistech-0.1.5/GnosisTech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/LICENSE` & `gnosistech-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/README.md` & `gnosistech-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/pyquanttrade/__init__.py` & `gnosistech-0.1.5/pyquanttrade/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/pyquanttrade/_backtest_source/_plotting.py` & `gnosistech-0.1.5/pyquanttrade/_backtest_source/_plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     from bokeh.models import FuncTickFormatter as CustomJSTickFormatter  # type: ignore
 from bokeh.io import output_notebook, output_file, show
 from bokeh.io.state import curstate
 from bokeh.layouts import gridplot
 from bokeh.palettes import Category10
 from bokeh.transform import factor_cmap
 
-from backtesting._util import _data_period, _as_list, _Indicator
+from _backtest_source._util import _data_period, _as_list, _Indicator
 
 with open(os.path.join(os.path.dirname(__file__), 'autoscale_cb.js'),
           encoding='utf-8') as _f:
     _AUTOSCALE_JS_CALLBACK = _f.read()
 
 IS_JUPYTER_NOTEBOOK = 'JPY_PARENT_PID' in os.environ
```

### Comparing `gnosistech-0.1.4/pyquanttrade/_backtest_source/_stats.py` & `gnosistech-0.1.5/pyquanttrade/_backtest_source/_stats.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/pyquanttrade/_backtest_source/_util.py` & `gnosistech-0.1.5/pyquanttrade/_backtest_source/_util.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/pyquanttrade/_backtest_source/autoscale_cb.js` & `gnosistech-0.1.5/pyquanttrade/_backtest_source/autoscale_cb.js`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/pyquanttrade/_backtest_source/lib.py` & `gnosistech-0.1.5/pyquanttrade/_backtest_source/lib.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/pyquanttrade/_backtest_source/source.py` & `gnosistech-0.1.5/pyquanttrade/_backtest_source/source.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/pyquanttrade/backtest/event_base.py` & `gnosistech-0.1.5/pyquanttrade/backtest/event_base.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/pyquanttrade/backtest/vectorized.py` & `gnosistech-0.1.5/pyquanttrade/backtest/vectorized.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/pyquanttrade/data/get_data.py` & `gnosistech-0.1.5/pyquanttrade/data/get_data.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/pyquanttrade/plot/plot.py` & `gnosistech-0.1.5/pyquanttrade/plot/plot.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/pyquanttrade/plot/ultils.py` & `gnosistech-0.1.5/pyquanttrade/plot/ultils.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.4/setup.py` & `gnosistech-0.1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='GnosisTech',
-    version='0.1.4',
+    version='0.1.5',
     author='Phung Ngoc An',
     author_email='phungankh2@gmail.com',
     description='PyQuantTrader là một thư viện Python hỗ trợ những vấn đề về quant trading.',
     packages=find_packages(),
     package_data= {'': ['*.json']},       
     classifiers=[
         'Programming Language :: Python :: 3',
```

