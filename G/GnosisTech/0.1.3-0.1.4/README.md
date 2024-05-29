# Comparing `tmp/gnosistech-0.1.3.tar.gz` & `tmp/gnosistech-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gnosistech-0.1.3.tar", last modified: Tue May 28 07:35:43 2024, max compression
+gzip compressed data, was "dist\gnosistech-0.1.4.tar", last modified: Wed May 29 02:20:56 2024, max compression
```

## Comparing `gnosistech-0.1.3.tar` & `gnosistech-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 07:35:43.874204 gnosistech-0.1.3/
-drwxrwxrwx   0        0        0        0 2024-05-28 07:35:43.870207 gnosistech-0.1.3/GnosisTech.egg-info/
--rw-rw-rw-   0        0        0      416 2024-05-28 07:35:43.000000 gnosistech-0.1.3/GnosisTech.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      678 2024-05-28 07:35:43.000000 gnosistech-0.1.3/GnosisTech.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 07:35:43.000000 gnosistech-0.1.3/GnosisTech.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-28 07:35:43.000000 gnosistech-0.1.3/GnosisTech.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      416 2024-05-28 07:35:43.872206 gnosistech-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 07:35:43.806111 gnosistech-0.1.3/pyquanttrade/
--rw-rw-rw-   0        0        0        0 2024-05-27 06:31:36.000000 gnosistech-0.1.3/pyquanttrade/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:35:43.826100 gnosistech-0.1.3/pyquanttrade/_backtest_source/
--rw-rw-rw-   0        0        0       30 2024-05-28 06:24:55.000000 gnosistech-0.1.3/pyquanttrade/_backtest_source/__init__.py
--rw-rw-rw-   0        0        0    30092 2024-05-23 03:58:58.000000 gnosistech-0.1.3/pyquanttrade/_backtest_source/_plotting.py
--rw-rw-rw-   0        0        0     6924 2024-05-23 03:58:58.000000 gnosistech-0.1.3/pyquanttrade/_backtest_source/_stats.py
--rw-rw-rw-   0        0        0     5915 2024-05-23 03:58:58.000000 gnosistech-0.1.3/pyquanttrade/_backtest_source/_util.py
--rw-rw-rw-   0        0        0    16793 2024-05-23 03:58:58.000000 gnosistech-0.1.3/pyquanttrade/_backtest_source/lib.py
--rw-rw-rw-   0        0        0    72566 2024-05-23 03:58:58.000000 gnosistech-0.1.3/pyquanttrade/_backtest_source/source.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:35:43.837094 gnosistech-0.1.3/pyquanttrade/backtest/
--rw-rw-rw-   0        0        0       22 2024-05-28 06:24:54.000000 gnosistech-0.1.3/pyquanttrade/backtest/__init__.py
--rw-rw-rw-   0        0        0      969 2024-05-23 03:58:58.000000 gnosistech-0.1.3/pyquanttrade/backtest/event_base.py
--rw-rw-rw-   0        0        0     4188 2024-05-23 03:58:58.000000 gnosistech-0.1.3/pyquanttrade/backtest/vectorized.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:35:43.844090 gnosistech-0.1.3/pyquanttrade/data/
--rw-rw-rw-   0        0        0       18 2024-05-28 06:24:54.000000 gnosistech-0.1.3/pyquanttrade/data/__init__.py
--rw-rw-rw-   0        0        0     4228 2024-05-23 03:58:58.000000 gnosistech-0.1.3/pyquanttrade/data/get_data.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:35:43.858082 gnosistech-0.1.3/pyquanttrade/plot/
--rw-rw-rw-   0        0        0       18 2024-05-28 06:25:19.000000 gnosistech-0.1.3/pyquanttrade/plot/__init__.py
--rw-rw-rw-   0        0        0     7421 2024-05-26 09:16:51.000000 gnosistech-0.1.3/pyquanttrade/plot/plot.py
--rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 gnosistech-0.1.3/pyquanttrade/plot/ultils.py
--rw-rw-rw-   0        0        0       42 2024-05-28 07:35:43.874204 gnosistech-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      523 2024-05-28 07:32:19.000000 gnosistech-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.751957 gnosistech-0.1.4/
+drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.747916 gnosistech-0.1.4/GnosisTech.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-05-29 02:20:56.000000 gnosistech-0.1.4/GnosisTech.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      736 2024-05-29 02:20:56.000000 gnosistech-0.1.4/GnosisTech.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 02:20:56.000000 gnosistech-0.1.4/GnosisTech.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 02:20:56.000000 gnosistech-0.1.4/GnosisTech.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2024-05-23 03:58:58.000000 gnosistech-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       31 2024-05-28 10:06:02.000000 gnosistech-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      416 2024-05-29 02:20:56.750230 gnosistech-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4709 2024-05-23 03:58:58.000000 gnosistech-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.698981 gnosistech-0.1.4/pyquanttrade/
+-rw-rw-rw-   0        0        0      532 2024-05-28 09:51:19.000000 gnosistech-0.1.4/pyquanttrade/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.725424 gnosistech-0.1.4/pyquanttrade/_backtest_source/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:41:32.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/__init__.py
+-rw-rw-rw-   0        0        0    30092 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/_plotting.py
+-rw-rw-rw-   0        0        0     6924 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/_stats.py
+-rw-rw-rw-   0        0        0     5915 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/_util.py
+-rw-rw-rw-   0        0        0     1236 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/autoscale_cb.js
+-rw-rw-rw-   0        0        0    16793 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/lib.py
+-rw-rw-rw-   0        0        0    72566 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/_backtest_source/source.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.731600 gnosistech-0.1.4/pyquanttrade/backtest/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:41:51.000000 gnosistech-0.1.4/pyquanttrade/backtest/__init__.py
+-rw-rw-rw-   0        0        0      969 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/backtest/event_base.py
+-rw-rw-rw-   0        0        0     4188 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/backtest/vectorized.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.736598 gnosistech-0.1.4/pyquanttrade/data/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:42:11.000000 gnosistech-0.1.4/pyquanttrade/data/__init__.py
+-rw-rw-rw-   0        0        0     4228 2024-05-23 03:58:58.000000 gnosistech-0.1.4/pyquanttrade/data/get_data.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:20:56.745918 gnosistech-0.1.4/pyquanttrade/plot/
+-rw-rw-rw-   0        0        0        0 2024-05-28 09:42:34.000000 gnosistech-0.1.4/pyquanttrade/plot/__init__.py
+-rw-rw-rw-   0        0        0     7421 2024-05-26 09:16:51.000000 gnosistech-0.1.4/pyquanttrade/plot/plot.py
+-rw-rw-rw-   0        0        0    22450 2024-05-23 08:08:08.000000 gnosistech-0.1.4/pyquanttrade/plot/ultils.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 02:20:56.751957 gnosistech-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-29 02:20:44.000000 gnosistech-0.1.4/setup.py
```

### Comparing `gnosistech-0.1.3/GnosisTech.egg-info/SOURCES.txt` & `gnosistech-0.1.4/GnosisTech.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 GnosisTech.egg-info/PKG-INFO
 GnosisTech.egg-info/SOURCES.txt
 GnosisTech.egg-info/dependency_links.txt
 GnosisTech.egg-info/top_level.txt
 pyquanttrade/__init__.py
 pyquanttrade/_backtest_source/__init__.py
 pyquanttrade/_backtest_source/_plotting.py
 pyquanttrade/_backtest_source/_stats.py
 pyquanttrade/_backtest_source/_util.py
+pyquanttrade/_backtest_source/autoscale_cb.js
 pyquanttrade/_backtest_source/lib.py
 pyquanttrade/_backtest_source/source.py
 pyquanttrade/backtest/__init__.py
 pyquanttrade/backtest/event_base.py
 pyquanttrade/backtest/vectorized.py
 pyquanttrade/data/__init__.py
 pyquanttrade/data/get_data.py
```

### Comparing `gnosistech-0.1.3/LICENSE` & `gnosistech-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.3/README.md` & `gnosistech-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.3/pyquanttrade/_backtest_source/_plotting.py` & `gnosistech-0.1.4/pyquanttrade/_backtest_source/_plotting.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.3/pyquanttrade/_backtest_source/_stats.py` & `gnosistech-0.1.4/pyquanttrade/_backtest_source/_stats.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.3/pyquanttrade/_backtest_source/_util.py` & `gnosistech-0.1.4/pyquanttrade/_backtest_source/_util.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.3/pyquanttrade/_backtest_source/lib.py` & `gnosistech-0.1.4/pyquanttrade/_backtest_source/lib.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.3/pyquanttrade/_backtest_source/source.py` & `gnosistech-0.1.4/pyquanttrade/_backtest_source/source.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.3/pyquanttrade/backtest/event_base.py` & `gnosistech-0.1.4/pyquanttrade/backtest/event_base.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.3/pyquanttrade/backtest/vectorized.py` & `gnosistech-0.1.4/pyquanttrade/backtest/vectorized.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.3/pyquanttrade/data/get_data.py` & `gnosistech-0.1.4/pyquanttrade/data/get_data.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.3/pyquanttrade/plot/plot.py` & `gnosistech-0.1.4/pyquanttrade/plot/plot.py`

 * *Files identical despite different names*

### Comparing `gnosistech-0.1.3/pyquanttrade/plot/ultils.py` & `gnosistech-0.1.4/pyquanttrade/plot/ultils.py`

 * *Files identical despite different names*

