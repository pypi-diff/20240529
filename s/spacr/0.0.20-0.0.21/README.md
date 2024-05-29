# Comparing `tmp/spacr-0.0.20.tar.gz` & `tmp/spacr-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacr-0.0.20.tar", last modified: Fri Mar 29 19:29:07 2024, max compression
+gzip compressed data, was "spacr-0.0.21.tar", last modified: Wed May 29 17:33:56 2024, max compression
```

## Comparing `spacr-0.0.20.tar` & `spacr-0.0.21.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-03-29 19:29:07.025213 spacr-0.0.20/
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1083 2024-03-18 14:14:52.000000 spacr-0.0.20/LICENSE
--rw-r--r--   0 carruthers  (1000) carruthers  (1000)     4354 2024-03-29 19:29:07.025213 spacr-0.0.20/PKG-INFO
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     3004 2024-03-29 18:21:59.000000 spacr-0.0.20/README.md
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)       38 2024-03-29 19:29:07.025213 spacr-0.0.20/setup.cfg
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1898 2024-03-29 19:27:54.000000 spacr-0.0.20/setup.py
-drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-03-29 19:29:07.025213 spacr-0.0.20/spacr/
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      879 2024-03-18 14:14:52.000000 spacr-0.0.20/spacr/__init__.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      285 2024-03-18 14:14:52.000000 spacr-0.0.20/spacr/__main__.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      462 2024-03-18 14:25:17.000000 spacr-0.0.20/spacr/alpha.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    19932 2024-03-18 14:14:52.000000 spacr-0.0.20/spacr/annotate_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1800 2024-03-27 18:50:03.000000 spacr-0.0.20/spacr/cli.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)   120307 2024-03-29 18:55:28.000000 spacr-0.0.20/spacr/core.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    12568 2024-03-21 13:14:11.000000 spacr-0.0.20/spacr/graph_learning.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     3385 2024-03-21 13:14:20.000000 spacr-0.0.20/spacr/graph_learning_lap.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     7965 2024-03-18 17:12:55.000000 spacr-0.0.20/spacr/gui_classify_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     8079 2024-03-21 13:14:26.000000 spacr-0.0.20/spacr/gui_mask_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     8061 2024-03-21 13:14:27.000000 spacr-0.0.20/spacr/gui_measure_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)        0 2024-03-18 17:12:53.000000 spacr-0.0.20/spacr/gui_sim_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    29631 2024-03-29 16:51:38.000000 spacr-0.0.20/spacr/gui_utils.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)   102042 2024-03-29 18:55:23.000000 spacr-0.0.20/spacr/io.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      670 2024-03-18 14:14:52.000000 spacr-0.0.20/spacr/logger.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    39278 2024-03-22 19:23:09.000000 spacr-0.0.20/spacr/mask_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    50795 2024-03-29 18:55:25.000000 spacr-0.0.20/spacr/measure.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    11226 2024-03-21 13:14:15.000000 spacr-0.0.20/spacr/old_code.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    55040 2024-03-27 19:04:20.000000 spacr-0.0.20/spacr/plot.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    51534 2024-03-18 14:14:52.000000 spacr-0.0.20/spacr/sim.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    34003 2024-03-29 15:44:24.000000 spacr-0.0.20/spacr/timelapse.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    25631 2024-03-18 14:14:52.000000 spacr-0.0.20/spacr/train.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    29370 2024-03-18 14:14:52.000000 spacr-0.0.20/spacr/umap.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)   120992 2024-03-29 18:55:27.000000 spacr-0.0.20/spacr/utils.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      409 2024-03-18 14:14:52.000000 spacr-0.0.20/spacr/version.py
-drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-03-29 19:29:07.025213 spacr-0.0.20/spacr.egg-info/
--rw-r--r--   0 carruthers  (1000) carruthers  (1000)     4354 2024-03-29 19:29:07.000000 spacr-0.0.20/spacr.egg-info/PKG-INFO
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1021 2024-03-29 19:29:07.000000 spacr-0.0.20/spacr.egg-info/SOURCES.txt
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)        1 2024-03-29 19:29:07.000000 spacr-0.0.20/spacr.egg-info/dependency_links.txt
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      290 2024-03-29 19:29:07.000000 spacr-0.0.20/spacr.egg-info/entry_points.txt
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      469 2024-03-29 19:29:07.000000 spacr-0.0.20/spacr.egg-info/requires.txt
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)        6 2024-03-29 19:29:07.000000 spacr-0.0.20/spacr.egg-info/top_level.txt
-drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-03-29 19:29:07.025213 spacr-0.0.20/tests/
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2289 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_annotate_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2761 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_core.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      775 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_gui_classify_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      771 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_gui_mask_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      786 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_gui_measure_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      766 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_gui_sim_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     5555 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_gui_utils.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1786 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_io.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2127 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_mask_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1957 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_measure.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2075 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_plot.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1097 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_sim.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1644 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_timelapse.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1217 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_train.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1503 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_umap.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1307 2024-03-18 14:14:52.000000 spacr-0.0.20/tests/test_utils.py
+drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-05-29 17:33:56.223083 spacr-0.0.21/
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1083 2024-03-18 14:14:52.000000 spacr-0.0.21/LICENSE
+-rw-r--r--   0 carruthers  (1000) carruthers  (1000)     4943 2024-05-29 17:33:56.223083 spacr-0.0.21/PKG-INFO
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     3503 2024-04-19 22:18:02.000000 spacr-0.0.21/README.md
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)       38 2024-05-29 17:33:56.223083 spacr-0.0.21/setup.cfg
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1965 2024-05-29 17:30:50.000000 spacr-0.0.21/setup.py
+drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-05-29 17:33:56.219083 spacr-0.0.21/spacr/
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      879 2024-03-18 14:14:52.000000 spacr-0.0.21/spacr/__init__.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      285 2024-03-18 14:14:52.000000 spacr-0.0.21/spacr/__main__.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    13776 2024-05-28 15:21:47.000000 spacr-0.0.21/spacr/alpha.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    19951 2024-04-29 20:22:59.000000 spacr-0.0.21/spacr/annotate_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1800 2024-03-27 18:50:03.000000 spacr-0.0.21/spacr/cli.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)   156457 2024-05-28 22:42:28.000000 spacr-0.0.21/spacr/core.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    33970 2024-04-29 20:23:08.000000 spacr-0.0.21/spacr/foldseek.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     3541 2024-04-29 20:23:07.000000 spacr-0.0.21/spacr/get_alfafold_structures.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    12568 2024-03-21 13:14:11.000000 spacr-0.0.21/spacr/graph_learning.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     3385 2024-03-21 13:14:20.000000 spacr-0.0.21/spacr/graph_learning_lap.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     7965 2024-03-18 17:12:55.000000 spacr-0.0.21/spacr/gui_classify_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     8752 2024-05-29 17:30:54.000000 spacr-0.0.21/spacr/gui_mask_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     8061 2024-03-21 13:14:27.000000 spacr-0.0.21/spacr/gui_measure_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)        0 2024-03-18 17:12:53.000000 spacr-0.0.21/spacr/gui_sim_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    30493 2024-05-29 14:11:59.000000 spacr-0.0.21/spacr/gui_utils.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)   108683 2024-05-28 22:42:29.000000 spacr-0.0.21/spacr/io.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      670 2024-03-18 14:14:52.000000 spacr-0.0.21/spacr/logger.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    39278 2024-03-22 19:23:09.000000 spacr-0.0.21/spacr/mask_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    54686 2024-05-28 15:21:46.000000 spacr-0.0.21/spacr/measure.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    11226 2024-03-21 13:14:15.000000 spacr-0.0.21/spacr/old_code.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    61655 2024-05-29 17:30:53.000000 spacr-0.0.21/spacr/plot.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    72997 2024-05-23 17:29:19.000000 spacr-0.0.21/spacr/sim.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    39661 2024-04-29 20:23:14.000000 spacr-0.0.21/spacr/timelapse.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    25904 2024-05-28 22:42:27.000000 spacr-0.0.21/spacr/train.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    29370 2024-05-07 16:13:08.000000 spacr-0.0.21/spacr/umap.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)   121205 2024-05-28 22:42:24.000000 spacr-0.0.21/spacr/utils.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      409 2024-03-18 14:14:52.000000 spacr-0.0.21/spacr/version.py
+drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-05-29 17:33:56.223083 spacr-0.0.21/spacr.egg-info/
+-rw-r--r--   0 carruthers  (1000) carruthers  (1000)     4943 2024-05-29 17:33:56.000000 spacr-0.0.21/spacr.egg-info/PKG-INFO
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1072 2024-05-29 17:33:56.000000 spacr-0.0.21/spacr.egg-info/SOURCES.txt
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)        1 2024-05-29 17:33:56.000000 spacr-0.0.21/spacr.egg-info/dependency_links.txt
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      290 2024-05-29 17:33:56.000000 spacr-0.0.21/spacr.egg-info/entry_points.txt
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      515 2024-05-29 17:33:56.000000 spacr-0.0.21/spacr.egg-info/requires.txt
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)        6 2024-05-29 17:33:56.000000 spacr-0.0.21/spacr.egg-info/top_level.txt
+drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-05-29 17:33:56.223083 spacr-0.0.21/tests/
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2289 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_annotate_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2761 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_core.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      775 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_gui_classify_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      771 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_gui_mask_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      786 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_gui_measure_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      766 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_gui_sim_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     5555 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_gui_utils.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1786 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_io.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2127 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_mask_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1957 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_measure.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2075 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_plot.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1097 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_sim.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1644 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_timelapse.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1217 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_train.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1503 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_umap.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1307 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_utils.py
```

### Comparing `spacr-0.0.20/LICENSE` & `spacr-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/PKG-INFO` & `spacr-0.0.21/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacr
-Version: 0.0.20
+Version: 0.0.21
 Summary: Spatial phenotype analysis of crisp screens (SpaCr)
 Home-page: https://github.com/EinarOlafsson/spacr
 Author: Einar Birnir Olafsson
 Author-email: olafsson@med.umich.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,26 +15,29 @@
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.1
 Requires-Dist: statsmodels>=0.14.1
 Requires-Dist: scikit-image>=0.22.0
 Requires-Dist: scikit-learn>=1.4.1
 Requires-Dist: seaborn>=0.13.2
 Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: shap>=0.45.0
 Requires-Dist: pillow>=10.2.0
 Requires-Dist: imageio>=2.34.0
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: ipywidgets>=8.1.2
 Requires-Dist: mahotas>=1.4.13
 Requires-Dist: btrack>=0.6.5
 Requires-Dist: trackpy>=0.6.2
 Requires-Dist: cellpose>=3.0.6
 Requires-Dist: IPython>=8.18.1
 Requires-Dist: opencv-python-headless>=4.9.0.80
 Requires-Dist: umap>=0.1.1
 Requires-Dist: ttkthemes>=3.2.2
+Requires-Dist: xgboost>=2.0.3
+Requires-Dist: PyWavelets>=1.6.0
 Requires-Dist: lxml>=5.1.0
 Provides-Extra: dev
 Requires-Dist: pytest>=3.9; extra == "dev"
 Provides-Extra: headless
 Requires-Dist: opencv-python-headless; extra == "headless"
 Provides-Extra: full
 Requires-Dist: opencv-python; extra == "full"
@@ -45,15 +48,15 @@
 [![repo size](https://img.shields.io/github/repo-size/EinarOlafsson/spacr)](https://github.com/EinarOlafsson/spacr/)
 
 # SpaCr
 <table>
 <tr>
 <td>
   
-Spatial phenotype analysis of crisp screens (SpaCr). A collection of functions for generating cellpose masks -> single object images and measurements -> annotation and classification of single object images. Spacr uses batch normalization to facilitate accurate segmentation of objects with low foreground representation.
+Spatial phenotype analysis of CRISPR-Cas9 screens (SpaCr). The spatial organization of organelles and proteins within cells constitutes a key level of functional regulation. In the context of infectious disease, the spatial relationships between host cell structures and intracellular pathogens are critical to understand host clearance mechanisms and how pathogens evade them. Spacr is a Python-based software package for generating single cell image data for deep-learning sub-cellular/cellular phenotypic classification from pooled genetic CRISPR-Cas9 screens. Spacr provides a flexible toolset to extract single cell images and measurements from high content cell painting experiments, train deep-learning models to classify cellular/ subcellular phenotypes, simulate and analyze pooled CRISPR-Cas9 imaging screens.
 
 </td>
 <td>
 
 <img src="spacr/logo_spacr.png" alt="SPACR Logo" title="SPACR Logo" width="600"/>
 
 </td>
```

#### html2text {}

```diff
@@ -1,36 +1,45 @@
-Metadata-Version: 2.1 Name: spacr Version: 0.0.20 Summary: Spatial phenotype
+Metadata-Version: 2.1 Name: spacr Version: 0.0.21 Summary: Spatial phenotype
 analysis of crisp screens (SpaCr) Home-page: https://github.com/EinarOlafsson/
 spacr Author: Einar Birnir Olafsson Author-email: olafsson@med.umich.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent License-
 File: LICENSE Requires-Dist: torch>=2.2.1 Requires-Dist: torchvision>=0.17.1
 Requires-Dist: torch-geometric>=2.5.1 Requires-Dist: numpy>=1.26.4 Requires-
 Dist: pandas>=2.2.1 Requires-Dist: statsmodels>=0.14.1 Requires-Dist: scikit-
 image>=0.22.0 Requires-Dist: scikit-learn>=1.4.1 Requires-Dist: seaborn>=0.13.2
-Requires-Dist: matplotlib>=3.8.3 Requires-Dist: pillow>=10.2.0 Requires-Dist:
-imageio>=2.34.0 Requires-Dist: scipy>=1.12.0 Requires-Dist: ipywidgets>=8.1.2
-Requires-Dist: mahotas>=1.4.13 Requires-Dist: btrack>=0.6.5 Requires-Dist:
-trackpy>=0.6.2 Requires-Dist: cellpose>=3.0.6 Requires-Dist: IPython>=8.18.1
-Requires-Dist: opencv-python-headless>=4.9.0.80 Requires-Dist: umap>=0.1.1
-Requires-Dist: ttkthemes>=3.2.2 Requires-Dist: lxml>=5.1.0 Provides-Extra: dev
-Requires-Dist: pytest>=3.9; extra == "dev" Provides-Extra: headless Requires-
-Dist: opencv-python-headless; extra == "headless" Provides-Extra: full
-Requires-Dist: opencv-python; extra == "full" [![PyPI version](https://
-badge.fury.io/py/spacr.svg)](https://badge.fury.io/py/spacr) [![Python version]
-(https://img.shields.io/pypi/pyversions/spacr)](https://pypistats.org/packages/
-spacr) [![Licence: GPL v3](https://img.shields.io/github/license/EinarOlafsson/
-spacr)](https://github.com/EinarOlafsson/spacr/blob/master/LICENSE) [![repo
-size](https://img.shields.io/github/repo-size/EinarOlafsson/spacr)](https://
-github.com/EinarOlafsson/spacr/) # SpaCr
-Spatial phenotype analysis of crisp screens (SpaCr). A collection
-of functions for generating cellpose masks -> single object images
-and measurements -> annotation and classification of single object [SPACR Logo]
-images. Spacr uses batch normalization to facilitate accurate
-segmentation of objects with low foreground representation.
+Requires-Dist: matplotlib>=3.8.3 Requires-Dist: shap>=0.45.0 Requires-Dist:
+pillow>=10.2.0 Requires-Dist: imageio>=2.34.0 Requires-Dist: scipy>=1.12.0
+Requires-Dist: ipywidgets>=8.1.2 Requires-Dist: mahotas>=1.4.13 Requires-Dist:
+btrack>=0.6.5 Requires-Dist: trackpy>=0.6.2 Requires-Dist: cellpose>=3.0.6
+Requires-Dist: IPython>=8.18.1 Requires-Dist: opencv-python-headless>=4.9.0.80
+Requires-Dist: umap>=0.1.1 Requires-Dist: ttkthemes>=3.2.2 Requires-Dist:
+xgboost>=2.0.3 Requires-Dist: PyWavelets>=1.6.0 Requires-Dist: lxml>=5.1.0
+Provides-Extra: dev Requires-Dist: pytest>=3.9; extra == "dev" Provides-Extra:
+headless Requires-Dist: opencv-python-headless; extra == "headless" Provides-
+Extra: full Requires-Dist: opencv-python; extra == "full" [![PyPI version]
+(https://badge.fury.io/py/spacr.svg)](https://badge.fury.io/py/spacr) [![Python
+version](https://img.shields.io/pypi/pyversions/spacr)](https://pypistats.org/
+packages/spacr) [![Licence: GPL v3](https://img.shields.io/github/license/
+EinarOlafsson/spacr)](https://github.com/EinarOlafsson/spacr/blob/master/
+LICENSE) [![repo size](https://img.shields.io/github/repo-size/EinarOlafsson/
+spacr)](https://github.com/EinarOlafsson/spacr/) # SpaCr
+Spatial phenotype analysis of CRISPR-Cas9 screens (SpaCr). The
+spatial organization of organelles and proteins within cells
+constitutes a key level of functional regulation. In the context
+of infectious disease, the spatial relationships between host cell
+structures and intracellular pathogens are critical to understand
+host clearance mechanisms and how pathogens evade them. Spacr is a
+Python-based software package for generating single cell image     [SPACR Logo]
+data for deep-learning sub-cellular/cellular phenotypic
+classification from pooled genetic CRISPR-Cas9 screens. Spacr
+provides a flexible toolset to extract single cell images and
+measurements from high content cell painting experiments, train
+deep-learning models to classify cellular/ subcellular phenotypes,
+simulate and analyze pooled CRISPR-Cas9 imaging screens.
 ## Features - **Generate Masks:** Generate cellpose masks for cells, nuclei and
 pathogen images. - **Object Measurements:** Measurements for each object
 including scikit-image-regionprops, intensity quantiles, shannon-entropy,
 pearsons and manders correlation, homogenicity and radial distribution.
 Measurements are saved to a sql database in object level tables. - **Crop
 Images:** Objects (e.g. cells) can be saved as PNGs from the object area or
 bounding box area of each object. Object paths are saved in an sql database
```

### Comparing `spacr-0.0.20/README.md` & `spacr-0.0.21/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![repo size](https://img.shields.io/github/repo-size/EinarOlafsson/spacr)](https://github.com/EinarOlafsson/spacr/)
 
 # SpaCr
 <table>
 <tr>
 <td>
   
-Spatial phenotype analysis of crisp screens (SpaCr). A collection of functions for generating cellpose masks -> single object images and measurements -> annotation and classification of single object images. Spacr uses batch normalization to facilitate accurate segmentation of objects with low foreground representation.
+Spatial phenotype analysis of CRISPR-Cas9 screens (SpaCr). The spatial organization of organelles and proteins within cells constitutes a key level of functional regulation. In the context of infectious disease, the spatial relationships between host cell structures and intracellular pathogens are critical to understand host clearance mechanisms and how pathogens evade them. Spacr is a Python-based software package for generating single cell image data for deep-learning sub-cellular/cellular phenotypic classification from pooled genetic CRISPR-Cas9 screens. Spacr provides a flexible toolset to extract single cell images and measurements from high content cell painting experiments, train deep-learning models to classify cellular/ subcellular phenotypes, simulate and analyze pooled CRISPR-Cas9 imaging screens.
 
 </td>
 <td>
 
 <img src="spacr/logo_spacr.png" alt="SPACR Logo" title="SPACR Logo" width="600"/>
 
 </td>
@@ -82,8 +82,8 @@
 Train torch CNNs/Transformers to classify single object images.
 ```
 gui_classify
 ```
 Simulate spatial phenotype screens.
 ```
 gui_sim
-```
+```
```

#### html2text {}

```diff
@@ -1,18 +1,26 @@
 [![PyPI version](https://badge.fury.io/py/spacr.svg)](https://badge.fury.io/py/
 spacr) [![Python version](https://img.shields.io/pypi/pyversions/spacr)](https:
 //pypistats.org/packages/spacr) [![Licence: GPL v3](https://img.shields.io/
 github/license/EinarOlafsson/spacr)](https://github.com/EinarOlafsson/spacr/
 blob/master/LICENSE) [![repo size](https://img.shields.io/github/repo-size/
 EinarOlafsson/spacr)](https://github.com/EinarOlafsson/spacr/) # SpaCr
-Spatial phenotype analysis of crisp screens (SpaCr). A collection
-of functions for generating cellpose masks -> single object images
-and measurements -> annotation and classification of single object [SPACR Logo]
-images. Spacr uses batch normalization to facilitate accurate
-segmentation of objects with low foreground representation.
+Spatial phenotype analysis of CRISPR-Cas9 screens (SpaCr). The
+spatial organization of organelles and proteins within cells
+constitutes a key level of functional regulation. In the context
+of infectious disease, the spatial relationships between host cell
+structures and intracellular pathogens are critical to understand
+host clearance mechanisms and how pathogens evade them. Spacr is a
+Python-based software package for generating single cell image     [SPACR Logo]
+data for deep-learning sub-cellular/cellular phenotypic
+classification from pooled genetic CRISPR-Cas9 screens. Spacr
+provides a flexible toolset to extract single cell images and
+measurements from high content cell painting experiments, train
+deep-learning models to classify cellular/ subcellular phenotypes,
+simulate and analyze pooled CRISPR-Cas9 imaging screens.
 ## Features - **Generate Masks:** Generate cellpose masks for cells, nuclei and
 pathogen images. - **Object Measurements:** Measurements for each object
 including scikit-image-regionprops, intensity quantiles, shannon-entropy,
 pearsons and manders correlation, homogenicity and radial distribution.
 Measurements are saved to a sql database in object level tables. - **Crop
 Images:** Objects (e.g. cells) can be saved as PNGs from the object area or
 bounding box area of each object. Object paths are saved in an sql database
```

### Comparing `spacr-0.0.20/setup.py` & `spacr-0.0.21/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,32 +11,35 @@
     'numpy>=1.26.4',
     'pandas>=2.2.1',
     'statsmodels>=0.14.1',
     'scikit-image>=0.22.0',
     'scikit-learn>=1.4.1',
     'seaborn>=0.13.2',
     'matplotlib>=3.8.3',
+    'shap>=0.45.0',
     'pillow>=10.2.0',
     'imageio>=2.34.0',
     'scipy>=1.12.0',
     'ipywidgets>=8.1.2',
     'mahotas>=1.4.13',
     'btrack>=0.6.5',
     'trackpy>=0.6.2',
     'cellpose>=3.0.6',
     'IPython>=8.18.1',
     'opencv-python-headless>=4.9.0.80',
     'umap>=0.1.1',
     'ttkthemes>=3.2.2',
+    'xgboost>=2.0.3',
+    'PyWavelets>=1.6.0',
     'lxml>=5.1.0'
 ]
 
 setup(
     name="spacr",
-    version="0.0.20",
+    version="0.0.21",
     author="Einar Birnir Olafsson",
     author_email="olafsson@med.umich.com",
     description="Spatial phenotype analysis of crisp screens (SpaCr)",
     long_description=long_description,
     url="https://github.com/EinarOlafsson/spacr",
     packages=find_packages(exclude=["tests.*", "tests"]),
     install_requires=dependencies,
```

### Comparing `spacr-0.0.20/spacr/__init__.py` & `spacr-0.0.21/spacr/__init__.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/spacr/annotate_app.py` & `spacr-0.0.21/spacr/annotate_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     - labels (list): A list of label widgets for displaying images.
     - terminate (bool): A flag indicating whether the application should terminate.
     - update_queue (Queue): A queue for storing image annotation updates.
     - status_label (tkinter.Label): A label widget for displaying status messages.
     - db_update_thread (threading.Thread): A thread for updating the database.
     """
 
-    def _init_(self, root, db_path, image_type=None, channels=None, grid_rows=None, grid_cols=None, image_size=(200, 200), annotation_column='annotate'):
+    def __init__(self, root, db_path, image_type=None, channels=None, grid_rows=None, grid_cols=None, image_size=(200, 200), annotation_column='annotate'):
         """
         Initializes an instance of the ImageApp class.
 
         Parameters:
         - root (tkinter.Tk): The root window of the application.
         - db_path (str): The path to the SQLite database.
         - image_type (str): The type of images to display.
@@ -379,15 +379,15 @@
         c.execute(f'ALTER TABLE png_list ADD COLUMN {annotation_column} integer')
     conn.commit()
     conn.close()
 
     root = tk.Tk()
     root.geometry(geom)
     app = ImageApp(root, db, image_type=image_type, channels=channels, image_size=img_size, grid_rows=rows, grid_cols=columns, annotation_column=annotation_column)
-    
+    #app = ImageApp()
     next_button = tk.Button(root, text="Next", command=app.next_page)
     next_button.grid(row=app.grid_rows, column=app.grid_cols - 1)
     back_button = tk.Button(root, text="Back", command=app.previous_page)
     back_button.grid(row=app.grid_rows, column=app.grid_cols - 2)
     exit_button = tk.Button(root, text="Exit", command=app.shutdown)
     exit_button.grid(row=app.grid_rows, column=app.grid_cols - 3)
```

### Comparing `spacr-0.0.20/spacr/cli.py` & `spacr-0.0.21/spacr/cli.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/spacr/core.py` & `spacr-0.0.21/spacr/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-import os, sqlite3, gc, torch, time, random, shutil, cv2, tarfile, datetime
+import os, sqlite3, gc, torch, time, random, shutil, cv2, tarfile, datetime, shap, string
 
 # image and array processing
 import numpy as np
 import pandas as pd
 
+from cellpose import train
 import cellpose
 from cellpose import models as cp_models
+from cellpose.models import CellposeModel
 
 import statsmodels.formula.api as smf
 import statsmodels.api as sm
 from functools import reduce
 from IPython.display import display
 from multiprocessing import Pool, cpu_count, Value, Lock
 
@@ -23,17 +25,25 @@
 import multiprocessing
 from torch.utils.data import DataLoader, random_split
 import matplotlib
 matplotlib.use('Agg')
 
 import torchvision.transforms as transforms
 from sklearn.model_selection import train_test_split
-from sklearn.ensemble import  IsolationForest
+from sklearn.ensemble import  IsolationForest, RandomForestClassifier, HistGradientBoostingClassifier
 from .logger import log_function_call
 
+from sklearn.linear_model import LogisticRegression
+from sklearn.inspection import permutation_importance
+from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score, classification_report
+from xgboost import XGBClassifier
+
+from scipy.spatial.distance import cosine, euclidean, mahalanobis, cityblock, minkowski, chebyshev, hamming, jaccard, braycurtis
+from sklearn.preprocessing import StandardScaler
+import shap
 
 def analyze_plaques(folder):
     summary_data = []
     details_data = []
     
     for filename in os.listdir(folder):
         filepath = os.path.join(folder, filename)
@@ -63,82 +73,14 @@
     summary_df.to_sql('summary', conn, if_exists='replace', index=False)
     details_df.to_sql('details', conn, if_exists='replace', index=False)
     
     conn.close()
     
     print(f"Analysis completed and saved to database '{db_name}'.")
 
-def compare_masks(dir1, dir2, dir3, verbose=False):
-    
-    from .io import _read_mask
-    from .plot import visualize_masks, plot_comparison_results
-    from .utils import extract_boundaries, boundary_f1_score, compute_segmentation_ap, jaccard_index, dice_coefficient
-    
-    filenames = os.listdir(dir1)
-    results = []
-    cond_1 = os.path.basename(dir1)
-    cond_2 = os.path.basename(dir2)
-    cond_3 = os.path.basename(dir3)
-    for index, filename in enumerate(filenames):
-        print(f'Processing image:{index+1}', end='\r', flush=True)
-        path1, path2, path3 = os.path.join(dir1, filename), os.path.join(dir2, filename), os.path.join(dir3, filename)
-        if os.path.exists(path2) and os.path.exists(path3):
-            
-            mask1, mask2, mask3 = _read_mask(path1), _read_mask(path2), _read_mask(path3)
-            boundary_true1, boundary_true2, boundary_true3 = extract_boundaries(mask1), extract_boundaries(mask2), extract_boundaries(mask3)
-            
-            
-            true_masks, pred_masks = [mask1], [mask2, mask3]  # Assuming mask1 is the ground truth for simplicity
-            true_labels, pred_labels_1, pred_labels_2 = label(mask1), label(mask2), label(mask3)
-            average_precision_0, average_precision_1 = compute_segmentation_ap(mask1, mask2), compute_segmentation_ap(mask1, mask3)
-            ap_scores = [average_precision_0, average_precision_1]
-
-            if verbose:
-                unique_values1, unique_values2, unique_values3 = np.unique(mask1),  np.unique(mask2), np.unique(mask3)
-                print(f"Unique values in mask 1: {unique_values1}, mask 2: {unique_values2}, mask 3: {unique_values3}")
-                visualize_masks(boundary_true1, boundary_true2, boundary_true3, title=f"Boundaries - {filename}")
-            
-            boundary_f1_12, boundary_f1_13, boundary_f1_23 = boundary_f1_score(mask1, mask2), boundary_f1_score(mask1, mask3), boundary_f1_score(mask2, mask3)
-
-            if (np.unique(mask1).size == 1 and np.unique(mask1)[0] == 0) and \
-               (np.unique(mask2).size == 1 and np.unique(mask2)[0] == 0) and \
-               (np.unique(mask3).size == 1 and np.unique(mask3)[0] == 0):
-                continue
-            
-            if verbose:
-                unique_values4, unique_values5, unique_values6 = np.unique(boundary_f1_12), np.unique(boundary_f1_13), np.unique(boundary_f1_23)
-                print(f"Unique values in boundary mask 1: {unique_values4}, mask 2: {unique_values5}, mask 3: {unique_values6}")
-                visualize_masks(mask1, mask2, mask3, title=filename)
-            
-            jaccard12 = jaccard_index(mask1, mask2)
-            dice12 = dice_coefficient(mask1, mask2)
-            jaccard13 = jaccard_index(mask1, mask3)
-            dice13 = dice_coefficient(mask1, mask3)
-            jaccard23 = jaccard_index(mask2, mask3)
-            dice23 = dice_coefficient(mask2, mask3)    
-
-            results.append({
-                f'filename': filename,
-                f'jaccard_{cond_1}_{cond_2}': jaccard12,
-                f'dice_{cond_1}_{cond_2}': dice12,
-                f'jaccard_{cond_1}_{cond_3}': jaccard13,
-                f'dice_{cond_1}_{cond_3}': dice13,
-                f'jaccard_{cond_2}_{cond_3}': jaccard23,
-                f'dice_{cond_2}_{cond_3}': dice23,
-                f'boundary_f1_{cond_1}_{cond_2}': boundary_f1_12,
-                f'boundary_f1_{cond_1}_{cond_3}': boundary_f1_13,
-                f'boundary_f1_{cond_2}_{cond_3}': boundary_f1_23,
-                f'average_precision_{cond_1}_{cond_2}': ap_scores[0],
-                f'average_precision_{cond_1}_{cond_3}': ap_scores[1]
-            })
-        else:
-            print(f'Cannot find {path1} or {path2} or {path3}')
-    fig = plot_comparison_results(results)
-    return results, fig
-
 def generate_cp_masks(settings):
     
     src = settings['src']
     model_name = settings['model_name']
     channels = settings['channels']
     diameter = settings['diameter']
     regex = '.tif'
@@ -173,63 +115,213 @@
 
 def train_cellpose(settings):
     
     from .io import _load_normalized_images_and_labels, _load_images_and_labels
     from .utils import resize_images_and_labels
 
     img_src = settings['img_src'] 
-    mask_src= settings['mask_src']
-    secondary_image_dir = None
+    mask_src = os.path.join(img_src, 'mask')
+    
+    model_name = settings['model_name']
+    model_type = settings['model_type']
+    learning_rate = settings['learning_rate']
+    weight_decay = settings['weight_decay']
+    batch_size = settings['batch_size']
+    n_epochs = settings['n_epochs']
+    from_scratch = settings['from_scratch']
+    diameter = settings['diameter']
+    verbose = settings['verbose']
+
+    channels = [0,0]
+    signal_thresholds = 1000
+    normalize = True
+    percentiles = [2,98]
+    circular = False
+    invert = False
+    resize = False
+    settings['width_height'] = [1000,1000]
+    target_height = settings['width_height'][1]
+    target_width = settings['width_height'][0]
+    rescale = False
+    grayscale = True
+    test = False
+
+    if test:
+        test_img_src = os.path.join(os.path.dirname(img_src), 'test')
+        test_mask_src = os.path.join(test_img_src, 'mask')
+
+    test_images, test_masks, test_image_names, test_mask_names = None,None,None,None,
+    print(settings)
+
+    if from_scratch:
+        model_name=f'scratch_{model_name}_{model_type}_e{n_epochs}_X{target_width}_Y{target_height}.CP_model'
+    else:
+        if resize:
+            model_name=f'{model_name}_{model_type}_e{n_epochs}_X{target_width}_Y{target_height}.CP_model'
+        else:
+            model_name=f'{model_name}_{model_type}_e{n_epochs}.CP_model'
+
+    model_save_path = os.path.join(mask_src, 'models', 'cellpose_model')
+    print(model_save_path)
+    os.makedirs(model_save_path, exist_ok=True)
+    
+    settings_df = pd.DataFrame(list(settings.items()), columns=['Key', 'Value'])
+    settings_csv = os.path.join(model_save_path,f'{model_name}_settings.csv')
+    settings_df.to_csv(settings_csv, index=False)
+    
+    if from_scratch:
+        model = cp_models.CellposeModel(gpu=True, model_type=model_type, diam_mean=diameter, pretrained_model=None)
+    else:
+        model = cp_models.CellposeModel(gpu=True, model_type=model_type)
+        
+    if normalize:
+
+        image_files = [os.path.join(img_src, f) for f in os.listdir(img_src) if f.endswith('.tif')]
+        label_files = [os.path.join(mask_src, f) for f in os.listdir(mask_src) if f.endswith('.tif')]
+        images, masks, image_names, mask_names = _load_normalized_images_and_labels(image_files, label_files, signal_thresholds, channels=channels, percentiles=percentiles,  circular=circular, invert=invert, visualize=verbose)
+        images = [np.squeeze(img) if img.shape[-1] == 1 else img for img in images]
+        
+        if test:
+            test_image_files = [os.path.join(test_img_src, f) for f in os.listdir(test_img_src) if f.endswith('.tif')]
+            test_label_files = [os.path.join(test_mask_src, f) for f in os.listdir(test_mask_src) if f.endswith('.tif')]
+            test_images, test_masks, test_image_names, test_mask_names = _load_normalized_images_and_labels(image_files=test_image_files, label_files=test_label_files, signal_thresholds=signal_thresholds, channels=channels, percentiles=percentiles,  circular=circular, invert=invert, visualize=verbose)
+            test_images = [np.squeeze(img) if img.shape[-1] == 1 else img for img in test_images]
+            
+        
+    else:
+        images, masks, image_names, mask_names = _load_images_and_labels(img_src, mask_src, circular, invert)
+        images = [np.squeeze(img) if img.shape[-1] == 1 else img for img in images]
+        
+        if test:
+            test_images, test_masks, test_image_names, test_mask_names = _load_images_and_labels(img_src=test_img_src, mask_src=test_mask_src, circular=circular, invert=circular)
+            test_images = [np.squeeze(img) if img.shape[-1] == 1 else img for img in test_images]
+    
+    if resize:
+        images, masks = resize_images_and_labels(images, masks, target_height, target_width, show_example=True)
+
+    if model_type == 'cyto':
+        cp_channels = [0,1]
+    if model_type == 'cyto2':
+        cp_channels = [0,2]
+    if model_type == 'nucleus':
+        cp_channels = [0,0]
+    if grayscale:
+        cp_channels = [0,0]
+        images = [np.squeeze(img) if img.ndim == 3 and 1 in img.shape else img for img in images]
+    
+    masks = [np.squeeze(mask) if mask.ndim == 3 and 1 in mask.shape else mask for mask in masks]
+
+    print(f'image shape: {images[0].shape}, image type: images[0].shape mask shape: {masks[0].shape}, image type: masks[0].shape')
+    save_every = int(n_epochs/10)
+    if save_every < 10:
+        save_every = n_epochs
+
+    train.train_seg(model.net,
+                    train_data=images,
+                    train_labels=masks,
+                    train_files=image_names,
+                    train_labels_files=mask_names,
+                    train_probs=None,
+                    test_data=test_images,
+                    test_labels=test_masks,
+                    test_files=test_image_names,
+                    test_labels_files=test_mask_names, 
+                    test_probs=None,
+                    load_files=True,
+                    batch_size=batch_size,
+                    learning_rate=learning_rate,
+                    n_epochs=n_epochs,
+                    weight_decay=weight_decay,
+                    momentum=0.9,
+                    SGD=False,
+                    channels=cp_channels,
+                    channel_axis=None,
+                    #rgb=False,
+                    normalize=False, 
+                    compute_flows=False,
+                    save_path=model_save_path,
+                    save_every=save_every,
+                    nimg_per_epoch=None,
+                    nimg_test_per_epoch=None,
+                    rescale=rescale,
+                    #scale_range=None,
+                    #bsize=224,
+                    min_train_masks=1,
+                    model_name=model_name)
+
+    return print(f"Model saved at: {model_save_path}/{model_name}")
+
+def train_cellpose_v1(settings):
+    
+    from .io import _load_normalized_images_and_labels, _load_images_and_labels
+    from .utils import resize_images_and_labels
+
+    img_src = settings['img_src'] 
+    
+    mask_src = os.path.join(img_src, 'mask')
+    
     model_name = settings['model_name']
     model_type = settings['model_type']
     learning_rate = settings['learning_rate']
     weight_decay = settings['weight_decay']
     batch_size = settings['batch_size']
     n_epochs = settings['n_epochs']
     verbose = settings['verbose']
-    signal_thresholds = settings['signal_thresholds']
+
+    signal_thresholds = 100 #settings['signal_thresholds']
+
     channels = settings['channels']
     from_scratch = settings['from_scratch']
     diameter = settings['diameter']
     resize = settings['resize']
     rescale = settings['rescale']
     normalize = settings['normalize']
     target_height = settings['width_height'][1]
     target_width = settings['width_height'][0]
     circular = settings['circular']
     invert = settings['invert']
     percentiles = settings['percentiles']
     grayscale = settings['grayscale']
-    
+
+    if model_type == 'cyto':
+        settings['diameter'] = 30
+        diameter = settings['diameter']
+        print(f'Cyto model must have diamiter 30. Diameter set the 30')
+
+    if model_type == 'nuclei':
+        settings['diameter'] = 17
+        diameter = settings['diameter']
+        print(f'Nuclei model must have diamiter 17. Diameter set the 17')
+
     print(settings)
 
     if from_scratch:
         model_name=f'scratch_{model_name}_{model_type}_e{n_epochs}_X{target_width}_Y{target_height}.CP_model'
     else:
         model_name=f'{model_name}_{model_type}_e{n_epochs}_X{target_width}_Y{target_height}.CP_model'
 
     model_save_path = os.path.join(mask_src, 'models', 'cellpose_model')
-    os.makedirs(os.path.dirname(model_save_path), exist_ok=True)
+    print(model_save_path)
+    os.makedirs(model_save_path, exist_ok=True)
     
     settings_df = pd.DataFrame(list(settings.items()), columns=['Key', 'Value'])
     settings_csv = os.path.join(model_save_path,f'{model_name}_settings.csv')
     settings_df.to_csv(settings_csv, index=False)
     
-    if model_type =='cyto':
-        if not from_scratch:
-            model = cp_models.CellposeModel(gpu=True, model_type=model_type)
-        else:
-            model = cp_models.CellposeModel(gpu=True, model_type=model_type, net_avg=False, diam_mean=diameter, pretrained_model=None)
-    if model_type !='cyto':
+    if not from_scratch:
         model = cp_models.CellposeModel(gpu=True, model_type=model_type)
-        
-    
-    
-    if normalize:    	
-        images, masks, image_names, mask_names = _load_normalized_images_and_labels(image_dir=img_src, label_dir=mask_src, secondary_image_dir=secondary_image_dir, signal_thresholds=signal_thresholds, channels=channels, percentiles=percentiles,  circular=circular, invert=invert, visualize=verbose)
+
+    else:
+        model = cp_models.CellposeModel(gpu=True, model_type=model_type, pretrained_model=None)
+            
+    if normalize:
+        image_files = [os.path.join(img_src, f) for f in os.listdir(img_src) if f.endswith('.tif')]
+        label_files = [os.path.join(mask_src, f) for f in os.listdir(mask_src) if f.endswith('.tif')]
+
+        images, masks, image_names, mask_names = _load_normalized_images_and_labels(image_files, label_files, signal_thresholds, channels=channels, percentiles=percentiles,  circular=circular, invert=invert, visualize=verbose)
         images = [np.squeeze(img) if img.shape[-1] == 1 else img for img in images]
     else:
         images, masks, image_names, mask_names = _load_images_and_labels(img_src, mask_src, circular, invert)
         images = [np.squeeze(img) if img.shape[-1] == 1 else img for img in images]
     
     if resize:
         images, masks = resize_images_and_labels(images, masks, target_height, target_width, show_example=True)
@@ -244,33 +336,94 @@
         cp_channels = [0,0]
         images = [np.squeeze(img) if img.ndim == 3 and 1 in img.shape else img for img in images]
     
     masks = [np.squeeze(mask) if mask.ndim == 3 and 1 in mask.shape else mask for mask in masks]
 
     print(f'image shape: {images[0].shape}, image type: images[0].shape mask shape: {masks[0].shape}, image type: masks[0].shape')
     save_every = int(n_epochs/10)
-    print('cellpose image input dtype', images[0].dtype)
-    print('cellpose mask input dtype', masks[0].dtype)
+    if save_every < 10:
+        save_every = n_epochs
+
+
+    #print('cellpose image input dtype', images[0].dtype)
+    #print('cellpose mask input dtype', masks[0].dtype)
+    
     # Train the model
-    model.train(train_data=images, #(list of arrays (2D or 3D)) – images for training
-                train_labels=masks, #(list of arrays (2D or 3D)) – labels for train_data, where 0=no masks; 1,2,…=mask labels can include flows as additional images
-                train_files=image_names, #(list of strings) – file names for images in train_data (to save flows for future runs)
-                channels=cp_channels, #(list of ints (default, None)) – channels to use for training
-                normalize=False, #(bool (default, True)) – normalize data so 0.0=1st percentile and 1.0=99th percentile of image intensities in each channel
-                save_path=model_save_path, #(string (default, None)) – where to save trained model, if None it is not saved
-                save_every=save_every, #(int (default, 100)) – save network every [save_every] epochs
-                learning_rate=learning_rate, #(float or list/np.ndarray (default, 0.2)) – learning rate for training, if list, must be same length as n_epochs
-                n_epochs=n_epochs, #(int (default, 500)) – how many times to go through whole training set during training
-                weight_decay=weight_decay, #(float (default, 0.00001)) –
-                SGD=True, #(bool (default, True)) – use SGD as optimization instead of RAdam
-                batch_size=batch_size, #(int (optional, default 8)) – number of 224x224 patches to run simultaneously on the GPU (can make smaller or bigger depending on GPU memory usage)
-                nimg_per_epoch=None, #(int (optional, default None)) – minimum number of images to train on per epoch, with a small training set (< 8 images) it may help to set to 8
-                rescale=rescale, #(bool (default, True)) – whether or not to rescale images to diam_mean during training, if True it assumes you will fit a size model after training or resize your images accordingly, if False it will try to train the model to be scale-invariant (works worse)
-                min_train_masks=1, #(int (default, 5)) – minimum number of masks an image must have to use in training set
-                model_name=model_name) #(str (default, None)) – name of network, otherwise saved with name as params + training start time 
+    #model.train(train_data=images, #(list of arrays (2D or 3D)) – images for training
+
+    #model.train(train_data=images, #(list of arrays (2D or 3D)) – images for training
+    #            train_labels=masks, #(list of arrays (2D or 3D)) – labels for train_data, where 0=no masks; 1,2,…=mask labels can include flows as additional images
+    #            train_files=image_names, #(list of strings) – file names for images in train_data (to save flows for future runs)
+    #            channels=cp_channels, #(list of ints (default, None)) – channels to use for training
+    #            normalize=False, #(bool (default, True)) – normalize data so 0.0=1st percentile and 1.0=99th percentile of image intensities in each channel
+    #            save_path=model_save_path, #(string (default, None)) – where to save trained model, if None it is not saved
+    #            save_every=save_every, #(int (default, 100)) – save network every [save_every] epochs
+    #            learning_rate=learning_rate, #(float or list/np.ndarray (default, 0.2)) – learning rate for training, if list, must be same length as n_epochs
+    #            n_epochs=n_epochs, #(int (default, 500)) – how many times to go through whole training set during training
+    #            weight_decay=weight_decay, #(float (default, 0.00001)) –
+    #            SGD=True, #(bool (default, True)) – use SGD as optimization instead of RAdam
+    #            batch_size=batch_size, #(int (optional, default 8)) – number of 224x224 patches to run simultaneously on the GPU (can make smaller or bigger depending on GPU memory usage)
+    #            nimg_per_epoch=None, #(int (optional, default None)) – minimum number of images to train on per epoch, with a small training set (< 8 images) it may help to set to 8
+    #            rescale=rescale, #(bool (default, True)) – whether or not to rescale images to diam_mean during training, if True it assumes you will fit a size model after training or resize your images accordingly, if False it will try to train the model to be scale-invariant (works worse)
+    #            min_train_masks=1, #(int (default, 5)) – minimum number of masks an image must have to use in training set
+    #            model_name=model_name) #(str (default, None)) – name of network, otherwise saved with name as params + training start time 
+
+
+    train.train_seg(model.net,
+                    train_data=images,
+                    train_labels=masks,
+                    train_files=image_names,
+                    train_labels_files=None,
+                    train_probs=None,
+                    test_data=None,
+                    test_labels=None,
+                    test_files=None,
+                    test_labels_files=None, 
+                    test_probs=None,
+                    load_files=True,
+                    batch_size=batch_size,
+                    learning_rate=learning_rate,
+                    n_epochs=n_epochs,
+                    weight_decay=weight_decay,
+                    momentum=0.9,
+                    SGD=False,
+                    channels=cp_channels,
+                    channel_axis=None,
+                    #rgb=False,
+                    normalize=False, 
+                    compute_flows=False,
+                    save_path=model_save_path,
+                    save_every=save_every,
+                    nimg_per_epoch=None,
+                    nimg_test_per_epoch=None,
+                    rescale=rescale,
+                    #scale_range=None,
+                    #bsize=224,
+                    min_train_masks=1,
+                    model_name=model_name)
+
+    #model_save_path = train.train_seg(model.net,
+    #                                  train_data=images,
+    #                                  train_files=image_names,
+    #                                  train_labels=masks,
+    #                                  channels=cp_channels,
+    #                                  normalize=False,
+    #                                  save_every=save_every,
+    #                                  learning_rate=learning_rate,
+    #                                  n_epochs=n_epochs,
+    #                                  #test_data=test_images,
+    #                                  #test_labels=test_labels,
+    #                                  weight_decay=weight_decay,
+    #                                  SGD=True,
+    #                                  batch_size=batch_size, 
+    #                                  nimg_per_epoch=None,
+    #                                  rescale=rescale,
+    #                                  min_train_masks=1,
+    #                                  model_name=model_name)
+ 
 
     return print(f"Model saved at: {model_save_path}/{model_name}")
 
 def analyze_data_reg(sequencing_loc, dv_loc, agg_type = 'mean', dv_col='pred', transform=None, min_cell_count=50, min_reads=100, min_wells=2, max_wells=1000, min_frequency=0.0,remove_outlier_genes=False, refine_model=False,by_plate=False, regression_type='mlr', alpha_value=0.01, fishers=False, fisher_threshold=0.9):
     
     from .plot import _reg_v_plot
     from .utils import generate_fraction_map, MLR, fishers_odds, lasso_reg
@@ -922,110 +1075,111 @@
     df.loc[(df['col'].isin(nc_col_list)) & (df['plate'].isin(nc_plate_list)), 'condition'] = 'nc'
     df.loc[(df['col'].isin(screen_col_list)) & (df['plate'].isin(screen_plate_list)), 'condition'] = 'screen'
 
     df = df.dropna(subset=['condition'])
     display(df)
     return df
 
-def generate_dataset(src, file_type=None, experiment='TSG101_screen', sample=None):
+def generate_dataset(src, file_metadata=None, experiment='TSG101_screen', sample=None):
     
-    from .utils import init_globals, add_images_to_tar
-	
-    db_path = os.path.join(src, 'measurements','measurements.db')
+    from .utils import initiate_counter, add_images_to_tar
+    
+    db_path = os.path.join(src, 'measurements', 'measurements.db')
     dst = os.path.join(src, 'datasets')
-	
-    global total_images
     all_paths = []
-    
+
     # Connect to the database and retrieve the image paths
     print(f'Reading DataBase: {db_path}')
-    with sqlite3.connect(db_path) as conn:
-        cursor = conn.cursor()
-        if file_type:
-            cursor.execute("SELECT png_path FROM png_list WHERE png_path LIKE ?", (f"%{file_type}%",))
-        else:
-            cursor.execute("SELECT png_path FROM png_list")
-        while True:
-            rows = cursor.fetchmany(1000)
-            if not rows:
-                break
-            all_paths.extend([row[0] for row in rows])
-    
+    try:
+        with sqlite3.connect(db_path) as conn:
+            cursor = conn.cursor()
+            if file_metadata:
+                if isinstance(file_metadata, str):
+                    cursor.execute("SELECT png_path FROM png_list WHERE png_path LIKE ?", (f"%{file_metadata}%",))
+            else:
+                cursor.execute("SELECT png_path FROM png_list")
+
+            while True:
+                rows = cursor.fetchmany(1000)
+                if not rows:
+                    break
+                all_paths.extend([row[0] for row in rows])
+
+    except sqlite3.Error as e:
+        print(f"Database error: {e}")
+        return
+    except Exception as e:
+        print(f"Error: {e}")
+        return
+
     if isinstance(sample, int):
         selected_paths = random.sample(all_paths, sample)
         print(f'Random selection of {len(selected_paths)} paths')
     else:
         selected_paths = all_paths
         random.shuffle(selected_paths)
         print(f'All paths: {len(selected_paths)} paths')
-        
+
     total_images = len(selected_paths)
-    print(f'found {total_images} images')
-    
+    print(f'Found {total_images} images')
+
     # Create a temp folder in dst
     temp_dir = os.path.join(dst, "temp_tars")
     os.makedirs(temp_dir, exist_ok=True)
 
     # Chunking the data
-    if len(selected_paths) > 10000:
-        num_procs = cpu_count()-2
-        chunk_size = len(selected_paths) // num_procs
-        remainder = len(selected_paths) % num_procs
-    else:
-        num_procs = 2
-        chunk_size = len(selected_paths) // 2
-        remainder = 0
+    num_procs = max(2, cpu_count() - 2)
+    chunk_size = len(selected_paths) // num_procs
+    remainder = len(selected_paths) % num_procs
 
     paths_chunks = []
     start = 0
     for i in range(num_procs):
         end = start + chunk_size + (1 if i < remainder else 0)
         paths_chunks.append(selected_paths[start:end])
         start = end
 
     temp_tar_files = [os.path.join(temp_dir, f'temp_{i}.tar') for i in range(num_procs)]
-    
-    # Initialize the shared objects
-    counter_ = Value('i', 0)
-    lock_ = Lock()
 
-    ctx = multiprocessing.get_context('spawn')
-    
     print(f'Generating temporary tar files in {dst}')
-    
+
+    # Initialize shared counter and lock
+    counter = Value('i', 0)
+    lock = Lock()
+
+    with Pool(processes=num_procs, initializer=initiate_counter, initargs=(counter, lock)) as pool:
+        pool.starmap(add_images_to_tar, [(paths_chunks[i], temp_tar_files[i], total_images) for i in range(num_procs)])
+
     # Combine the temporary tar files into a final tar
     date_name = datetime.date.today().strftime('%y%m%d')
-    tar_name = f'{date_name}_{experiment}_{file_type}.tar'
+    if not file_metadata is None:
+        tar_name = f'{date_name}_{experiment}_{file_metadata}.tar'
+    else:
+        tar_name = f'{date_name}_{experiment}.tar'
+    tar_name = os.path.join(dst, tar_name)
     if os.path.exists(tar_name):
         number = random.randint(1, 100)
-        tar_name_2 = f'{date_name}_{experiment}_{file_type}_{number}.tar'
-        print(f'Warning: {os.path.basename(tar_name)} exists saving as {os.path.basename(tar_name_2)} ')
-        tar_name = tar_name_2
-    
-    # Add the counter and lock to the arguments for pool.map
+        tar_name_2 = f'{date_name}_{experiment}_{file_metadata}_{number}.tar'
+        print(f'Warning: {os.path.basename(tar_name)} exists, saving as {os.path.basename(tar_name_2)} ')
+        tar_name = os.path.join(dst, tar_name_2)
+
     print(f'Merging temporary files')
-    #with Pool(processes=num_procs, initializer=init_globals, initargs=(counter_, lock_)) as pool:
-    #    results = pool.map(add_images_to_tar, zip(paths_chunks, temp_tar_files))
 
-    with ctx.Pool(processes=num_procs, initializer=init_globals, initargs=(counter_, lock_)) as pool:
-        results = pool.map(add_images_to_tar, zip(paths_chunks, temp_tar_files))
-    
-    with tarfile.open(os.path.join(dst, tar_name), 'w') as final_tar:
-        for tar_path in results:
-            with tarfile.open(tar_path, 'r') as t:
-                for member in t.getmembers():
-                    t.extract(member, path=dst)
-                    final_tar.add(os.path.join(dst, member.name), arcname=member.name)
-                    os.remove(os.path.join(dst, member.name))
-            os.remove(tar_path)
+    with tarfile.open(tar_name, 'w') as final_tar:
+        for temp_tar_path in temp_tar_files:
+            with tarfile.open(temp_tar_path, 'r') as temp_tar:
+                for member in temp_tar.getmembers():
+                    file_obj = temp_tar.extractfile(member)
+                    final_tar.addfile(member, file_obj)
+            os.remove(temp_tar_path)
 
     # Delete the temp folder
     shutil.rmtree(temp_dir)
-    print(f"\nSaved {total_images} images to {os.path.join(dst, tar_name)}")
-    
+    print(f"\nSaved {total_images} images to {tar_name}")
+
 def apply_model_to_tar(tar_path, model_path, file_type='cell_png', image_size=224, batch_size=64, normalize=True, preload='images', num_workers=10, verbose=False):
     
     from .io import TarImageDataset, DataLoader
     
     device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
     if normalize:
         transform = transforms.Compose([
@@ -1253,33 +1407,52 @@
 def generate_training_dataset(src, mode='annotation', annotation_column='test', annotated_classes=[1,2], classes=['nc','pc'], size=200, test_split=0.1, class_metadata=[['c1'],['c2']], metadata_type_by='col', channel_of_interest=3, custom_measurement=None, tables=None, png_type='cell_png'):
     
     from .io import _read_and_merge_data, _read_db
     from .utils import get_paths_from_db, annotate_conditions
     
     db_path = os.path.join(src, 'measurements','measurements.db')
     dst = os.path.join(src, 'datasets', 'training')
-    
+
+    if os.path.exists(dst):
+        for i in range(1, 1000):
+            dst = os.path.join(src, 'datasets', f'training_{i}')
+            if not os.path.exists(dst):
+                print(f'Creating new directory for training: {dst}')
+                break
+                
     if mode == 'annotation':
         class_paths_ls_2 = []
         class_paths_ls = training_dataset_from_annotation(db_path, dst, annotation_column, annotated_classes=annotated_classes)
         for class_paths in class_paths_ls:
             class_paths_temp = random.sample(class_paths, size)
             class_paths_ls_2.append(class_paths_temp)
         class_paths_ls = class_paths_ls_2
 
     elif mode == 'metadata':
         class_paths_ls = []
+        class_len_ls = []
         [df] = _read_db(db_loc=db_path, tables=['png_list'])
         df['metadata_based_class'] = pd.NA
         for i, class_ in enumerate(classes):
             ls = class_metadata[i]
             df.loc[df[metadata_type_by].isin(ls), 'metadata_based_class'] = class_
             
         for class_ in classes:
+            if size == None:
+                c_s = []
+                for c in classes:
+                    c_s_t_df = df[df['metadata_based_class'] == c]
+                    c_s.append(len(c_s_t_df))
+                    print(f'Found {len(c_s_t_df)} images for class {c}')
+                size = min(c_s)
+                print(f'Using the smallest class size: {size}')
+
             class_temp_df = df[df['metadata_based_class'] == class_]
+            class_len_ls.append(len(class_temp_df))
+            print(f'Found {len(class_temp_df)} images for class {class_}')
             class_paths_temp = random.sample(class_temp_df['png_path'].tolist(), size)
             class_paths_ls.append(class_paths_temp)
     
     elif mode == 'recruitment':
         class_paths_ls = []
         if not isinstance(tables, list):
             tables = ['cell', 'nucleus', 'pathogen','cytoplasm']
@@ -1328,15 +1501,15 @@
         class_paths_upper = random.sample(class_paths_upper['png_path'].tolist(), size)
         class_paths_ls.append(class_paths_upper)
     
     generate_dataset_from_lists(dst, class_data=class_paths_ls, classes=classes, test_split=0.1)
     
     return
 
-def generate_loaders(src, train_mode='erm', mode='train', image_size=224, batch_size=32, classes=['nc','pc'], num_workers=None, validation_split=0.0, max_show=2, pin_memory=False, normalize=False, verbose=False):
+def generate_loaders_v1(src, train_mode='erm', mode='train', image_size=224, batch_size=32, classes=['nc','pc'], num_workers=None, validation_split=0.0, max_show=2, pin_memory=False, normalize=False, verbose=False):
     """
     Generate data loaders for training and validation/test datasets.
 
     Parameters:
     - src (str): The source directory containing the data.
     - train_mode (str): The training mode. Options are 'erm' (Empirical Risk Minimization) or 'irm' (Invariant Risk Minimization).
     - mode (str): The mode of operation. Options are 'train' or 'test'.
@@ -1459,14 +1632,181 @@
                         break
                     images = images.cpu()
                     label_strings = [str(label.item()) for label in labels]
                     _imshow(images, label_strings, nrow=20, fontsize=12)
     
     return train_loaders, val_loaders, plate_names
 
+def generate_loaders(src, train_mode='erm', mode='train', image_size=224, batch_size=32, classes=['nc','pc'], num_workers=None, validation_split=0.0, max_show=2, pin_memory=False, normalize=False, channels=[1, 2, 3], verbose=False):
+    
+    """
+    Generate data loaders for training and validation/test datasets.
+
+    Parameters:
+    - src (str): The source directory containing the data.
+    - train_mode (str): The training mode. Options are 'erm' (Empirical Risk Minimization) or 'irm' (Invariant Risk Minimization).
+    - mode (str): The mode of operation. Options are 'train' or 'test'.
+    - image_size (int): The size of the input images.
+    - batch_size (int): The batch size for the data loaders.
+    - classes (list): The list of classes to consider.
+    - num_workers (int): The number of worker threads for data loading.
+    - validation_split (float): The fraction of data to use for validation when train_mode is 'erm'.
+    - max_show (int): The maximum number of images to show when verbose is True.
+    - pin_memory (bool): Whether to pin memory for faster data transfer.
+    - normalize (bool): Whether to normalize the input images.
+    - verbose (bool): Whether to print additional information and show images.
+    - channels (list): The list of channels to retain. Options are [1, 2, 3] for all channels, [1, 2] for blue and green, etc.
+
+    Returns:
+    - train_loaders (list): List of data loaders for training datasets.
+    - val_loaders (list): List of data loaders for validation datasets.
+    - plate_names (list): List of plate names (only applicable when train_mode is 'irm').
+    """
+
+    from .io import MyDataset
+    from .plot import _imshow
+    from torchvision import transforms
+    from torch.utils.data import DataLoader, random_split
+    from collections import defaultdict
+    import os
+    import random
+    from PIL import Image
+    from torchvision.transforms import ToTensor
+
+    chans = []
+
+    if 'r' in channels:
+        chans.append(1)
+    if 'g' in channels:
+        chans.append(2)
+    if 'b' in channels:
+        chans.append(3)
+
+    channels = chans
+
+    if verbose:
+        print(f'Training a network on channels: {channels}')
+        print(f'Channel 1: Red, Channel 2: Green, Channel 3: Blue')
+
+    class SelectChannels:
+        def __init__(self, channels):
+            self.channels = channels
+        
+        def __call__(self, img):
+            img = img.clone()
+            if 1 not in self.channels:
+                img[0, :, :] = 0  # Zero out the red channel
+            if 2 not in self.channels:
+                img[1, :, :] = 0  # Zero out the green channel
+            if 3 not in self.channels:
+                img[2, :, :] = 0  # Zero out the blue channel
+            return img
+
+    plate_to_filenames = defaultdict(list)
+    plate_to_labels = defaultdict(list)
+    train_loaders = []
+    val_loaders = []
+    plate_names = []
+
+    if normalize:
+        transform = transforms.Compose([
+            transforms.ToTensor(),
+            transforms.CenterCrop(size=(image_size, image_size)),
+            SelectChannels(channels),
+            transforms.Normalize(mean=(0.5, 0.5, 0.5), std=(0.5, 0.5, 0.5))])
+    else:
+        transform = transforms.Compose([
+            transforms.ToTensor(),
+            transforms.CenterCrop(size=(image_size, image_size)),
+            SelectChannels(channels)])
+
+    if mode == 'train':
+        data_dir = os.path.join(src, 'train')
+        shuffle = True
+        print('Generating Train and validation datasets')
+    elif mode == 'test':
+        data_dir = os.path.join(src, 'test')
+        val_loaders = []
+        validation_split = 0.0
+        shuffle = True
+        print('Generating test dataset')
+    else:
+        print(f'mode:{mode} is not valid, use mode = train or test')
+        return
+
+    if train_mode == 'erm':
+        data = MyDataset(data_dir, classes, transform=transform, shuffle=shuffle, pin_memory=pin_memory)
+        if validation_split > 0:
+            train_size = int((1 - validation_split) * len(data))
+            val_size = len(data) - train_size
+
+            print(f'Train data:{train_size}, Validation data:{val_size}')
+
+            train_dataset, val_dataset = random_split(data, [train_size, val_size])
+
+            train_loaders = DataLoader(train_dataset, batch_size=batch_size, shuffle=shuffle, num_workers=num_workers if num_workers is not None else 0, pin_memory=pin_memory)
+            val_loaders = DataLoader(val_dataset, batch_size=batch_size, shuffle=shuffle, num_workers=num_workers if num_workers is not None else 0, pin_memory=pin_memory)
+        else:
+            train_loaders = DataLoader(data, batch_size=batch_size, shuffle=shuffle, num_workers=num_workers if num_workers is not None else 0, pin_memory=pin_memory)
+        
+    elif train_mode == 'irm':
+        data = MyDataset(data_dir, classes, transform=transform, shuffle=shuffle, pin_memory=pin_memory)
+        
+        for filename, label in zip(data.filenames, data.labels):
+            plate = data.get_plate(filename)
+            plate_to_filenames[plate].append(filename)
+            plate_to_labels[plate].append(label)
+
+        for plate, filenames in plate_to_filenames.items():
+            labels = plate_to_labels[plate]
+            plate_data = MyDataset(data_dir, classes, specific_files=filenames, specific_labels=labels, transform=transform, shuffle=False, pin_memory=pin_memory)
+            plate_names.append(plate)
+
+            if validation_split > 0:
+                train_size = int((1 - validation_split) * len(plate_data))
+                val_size = len(plate_data) - train_size
+
+                print(f'Train data:{train_size}, Validation data:{val_size}')
+
+                train_dataset, val_dataset = random_split(plate_data, [train_size, val_size])
+
+                train_loader = DataLoader(train_dataset, batch_size=batch_size, shuffle=shuffle, num_workers=num_workers if num_workers is not None else 0, pin_memory=pin_memory)
+                val_loader = DataLoader(val_dataset, batch_size=batch_size, shuffle=shuffle, num_workers=num_workers if num_workers is not None else 0, pin_memory=pin_memory)
+
+                train_loaders.append(train_loader)
+                val_loaders.append(val_loader)
+            else:
+                train_loader = DataLoader(plate_data, batch_size=batch_size, shuffle=shuffle, num_workers=num_workers if num_workers is not None else 0, pin_memory=pin_memory)
+                train_loaders.append(train_loader)
+                val_loaders.append(None)
+    
+    else:
+        print(f'train_mode:{train_mode} is not valid, use: train_mode = irm or erm')
+        return
+
+    if verbose:
+        if train_mode == 'erm':
+            for idx, (images, labels, filenames) in enumerate(train_loaders):
+                if idx >= max_show:
+                    break
+                images = images.cpu()
+                label_strings = [str(label.item()) for label in labels]
+                _imshow(images, label_strings, nrow=20, fontsize=12)
+        elif train_mode == 'irm':
+            for plate_name, train_loader in zip(plate_names, train_loaders):
+                print(f'Plate: {plate_name} with {len(train_loader.dataset)} images')
+                for idx, (images, labels, filenames) in enumerate(train_loader):
+                    if idx >= max_show:
+                        break
+                    images = images.cpu()
+                    label_strings = [str(label.item()) for label in labels]
+                    _imshow(images, label_strings, nrow=20, fontsize=12)
+    
+    return train_loaders, val_loaders, plate_names
+
 def analyze_recruitment(src, metadata_settings, advanced_settings):
     """
     Analyze recruitment data by grouping the DataFrame by well coordinates and plotting controls and recruitment data.
 
     Parameters:
     src (str): The source of the recruitment data.
     metadata_settings (dict): The settings for metadata.
@@ -1565,23 +1905,38 @@
                              treatments=treatments, 
                              treatment_loc=treatment_plate_metadata,
                              types=metadata_types)
     
     df = df.dropna(subset=['condition'])
     print(f'After dropping non-annotated wells: {len(df)} rows')
     files = df['file_name'].tolist()
+    print(f'found: {len(files)} files')
     files = [item + '.npy' for item in files]
     random.shuffle(files)
-    
+
+    _max = 10**100
+
+    if cell_size_range is None and nucleus_size_range is None and pathogen_size_range is None:
+        filter_min_max = None
+    else:
+        if cell_size_range is None:
+            cell_size_range = [0,_max]
+        if nucleus_size_range is None:
+            nucleus_size_range = [0,_max]
+        if pathogen_size_range is None:
+            pathogen_size_range = [0,_max]
+
+        filter_min_max = [[cell_size_range[0],cell_size_range[1]],[nucleus_size_range[0],nucleus_size_range[1]],[pathogen_size_range[0],pathogen_size_range[1]]]
+
     if plot:
         plot_settings = {'include_noninfected':include_noninfected, 
                          'include_multiinfected':include_multiinfected,
                          'include_multinucleated':include_multinucleated,
                          'remove_background':remove_background,
-                         'filter_min_max':[[cell_size_range[0],cell_size_range[1]],[nucleus_size_range[0],nucleus_size_range[1]],[pathogen_size_range[0],pathogen_size_range[1]]],
+                         'filter_min_max':filter_min_max,
                          'channel_dims':channel_dims,
                          'backgrounds':backgrounds,
                          'cell_mask_dim':mask_dims[0],
                          'nucleus_mask_dim':mask_dims[1],
                          'pathogen_mask_dim':mask_dims[2],
                          'overlay_chans':overlay_channels,
                          'outline_thickness':3,
@@ -1636,14 +1991,15 @@
 
 def preprocess_generate_masks(src, settings={}):
 
     from .io import preprocess_img_data, _load_and_concatenate_arrays
     from .plot import plot_merged, plot_arrays
     from .utils import _pivot_counts_table
 
+    settings['plot'] = False
     settings['fps'] = 2
     settings['remove_background'] = True
     settings['lower_quantile'] = 0.02
     settings['merge'] = False
     settings['normalize_plots'] = True
     settings['all_to_mip'] = False
     settings['pick_slice'] = False
@@ -1651,14 +2007,23 @@
     settings['workers'] = os.cpu_count()-4
     settings['verbose'] = True
     settings['examples_to_plot'] = 1
     settings['src'] = src
     settings['upscale'] = False
     settings['upscale_factor'] = 2.0
 
+    settings['randomize'] = True
+    settings['timelapse'] = False
+    settings['timelapse_displacement'] = None
+    settings['timelapse_memory'] = 3
+    settings['timelapse_frame_limits'] = None
+    settings['timelapse_remove_transient'] = False
+    settings['timelapse_mode'] = 'trackpy'
+    settings['timelapse_objects'] = ['cells']
+
     settings_df = pd.DataFrame(list(settings.items()), columns=['Key', 'Value'])
     settings_csv = os.path.join(src,'settings','preprocess_generate_masks_settings.csv')
     os.makedirs(os.path.join(src,'settings'), exist_ok=True)
     settings_df.to_csv(settings_csv, index=False)
     
     if settings['timelapse']:
         settings['randomize'] = False
@@ -1719,77 +2084,117 @@
                                  'remove_background':False,
                                  'filter_min_max':None,
                                  'channel_dims':settings['channels'],
                                  'backgrounds':[100,100,100,100],
                                  'cell_mask_dim':cell_mask_dim,
                                  'nucleus_mask_dim':nucleus_mask_dim,
                                  'pathogen_mask_dim':pathogen_mask_dim,
-                                 'overlay_chans':[0,2,3],
                                  'outline_thickness':3,
                                  'outline_color':'gbr',
                                  'overlay_chans':overlay_channels,
                                  'overlay':True,
                                  'normalization_percentiles':[1,99],
                                  'normalize':True,
                                  'print_object_number':True,
                                  'nr':settings['examples_to_plot'],
                                  'figuresize':20,
                                  'cmap':'inferno',
                                  'verbose':False}
+                
+                if settings['test_mode'] == True:
+                    plot_settings['nr'] = len(os.path.join(src,'merged'))
+
                 try:
                     fig = plot_merged(src=os.path.join(src,'merged'), settings=plot_settings)
                 except Exception as e:
                     print(f'Failed to plot image mask overly. Error: {e}')
             else:
                 plot_arrays(src=os.path.join(src,'merged'), figuresize=50, cmap='inferno', nr=1, normalize=True, q1=1, q2=99)
             
     torch.cuda.empty_cache()
     gc.collect()
     print("Successfully completed run")
     return
 
-def identify_masks_finetune(src, dst, model_name, channels, diameter, batch_size, flow_threshold=30, cellprob_threshold=1, figuresize=25, cmap='inferno', verbose=False, plot=False, save=False, custom_model=None, signal_thresholds=1000, normalize=True, resize=False, target_height=None, target_width=None, rescale=True, resample=True, net_avg=False, invert=False, circular=False, percentiles=None, overlay=True, grayscale=False):
+def identify_masks_finetune(settings):
     
     from .plot import print_mask_and_flows
     from .utils import get_files_from_dir, resize_images_and_labels
     from .io import _load_normalized_images_and_labels, _load_images_and_labels
     
+    src=settings['src']
+    dst=settings['dst']
+    model_name=settings['model_name']
+    diameter=settings['diameter']
+    batch_size=settings['batch_size']
+    flow_threshold=settings['flow_threshold']
+    cellprob_threshold=settings['cellprob_threshold']
+
+    verbose=settings['verbose']
+    plot=settings['plot']
+    save=settings['save']
+    custom_model=settings['custom_model']
+    overlay=settings['overlay']
+
+    figuresize=25
+    cmap='inferno'
+    channels = [0,0]
+    signal_thresholds = 1000
+    normalize = True
+    percentiles = [2,98]
+    circular = False
+    invert = False
+    resize = False
+    settings['width_height'] = [1000,1000]
+    target_height = settings['width_height'][1]
+    target_width = settings['width_height'][0]
+    rescale = False
+    resample = False
+    grayscale = True
+    test = False
+
+    os.makedirs(dst, exist_ok=True)
+
+    if not custom_model is None:
+        if not os.path.exists(custom_model):
+            print(f'Custom model not found: {custom_model}')
+            return 
+
     if not torch.cuda.is_available():
         print(f'Torch CUDA is not available, using CPU')
     
     device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
     
     if custom_model == None:
-        if model_name =='cyto':
-            model = cp_models.CellposeModel(gpu=True, model_type=model_name, net_avg=False, diam_mean=diameter, pretrained_model=None)
-        else:
-            model = cp_models.CellposeModel(gpu=True, model_type=model_name)
-
-    if custom_model != None:
-        model = cp_models.CellposeModel(gpu=torch.cuda.is_available(), model_type=None, pretrained_model=custom_model, diam_mean=diameter, device=device, net_avg=False)  #Assuming diameter is defined elsewhere 
-        print(f'loaded custom model:{custom_model}')
+        model = cp_models.CellposeModel(gpu=True, model_type=model_name, device=device)
+        print(f'Loaded model: {model_name}')
+    else:
+        model = cp_models.CellposeModel(gpu=torch.cuda.is_available(), model_type=None, pretrained_model=custom_model, diam_mean=diameter, device=device)
+        print("Pretrained Model Loaded:", model.pretrained_model)
 
     chans = [2, 1] if model_name == 'cyto2' else [0,0] if model_name == 'nucleus' else [1,0] if model_name == 'cyto' else [2, 0]
     
     if grayscale:
         chans=[0, 0]
     
     print(f'Using channels: {chans} for model of type {model_name}')
     
     if verbose == True:
         print(f'Cellpose settings: Model: {model_name}, channels: {channels}, cellpose_chans: {chans}, diameter:{diameter}, flow_threshold:{flow_threshold}, cellprob_threshold:{cellprob_threshold}')
         
-    all_image_files = get_files_from_dir(src, file_extension="*.tif")
+    all_image_files = [os.path.join(src, f) for f in os.listdir(src) if f.endswith('.tif')]
+
     random.shuffle(all_image_files)
     
     time_ls = []
     for i in range(0, len(all_image_files), batch_size):
         image_files = all_image_files[i:i+batch_size]
+
         if normalize:
-            images, _, image_names, _ = _load_normalized_images_and_labels(image_files=image_files, label_files=None, signal_thresholds=signal_thresholds, channels=channels, percentiles=percentiles,  circular=circular, invert=invert, visualize=verbose)
+            images, _, image_names, _ = _load_normalized_images_and_labels(image_files=image_files, label_files=None, signal_thresholds=signal_thresholds, channels=channels, percentiles=percentiles,  circular=circular, invert=invert, visualize=plot)
             images = [np.squeeze(img) if img.shape[-1] == 1 else img for img in images]
             orig_dims = [(image.shape[0], image.shape[1]) for image in images]
         else:
             images, _, image_names, _ = _load_images_and_labels(image_files=image_files, label_files=None, circular=circular, invert=invert) 
             images = [np.squeeze(img) if img.shape[-1] == 1 else img for img in images]
             orig_dims = [(image.shape[0], image.shape[1]) for image in images]
         if resize:
@@ -1802,16 +2207,15 @@
                          channels=chans,
                          channel_axis=3,
                          diameter=diameter,
                          flow_threshold=flow_threshold,
                          cellprob_threshold=cellprob_threshold,
                          rescale=rescale,
                          resample=resample,
-                         net_avg=net_avg,
-                         progress=False)
+                         progress=True)
 
             if len(output) == 4:
                 mask, flows, _, _ = output
             elif len(output) == 3:
                 mask, flows, _ = output
             else:
                 raise ValueError("Unexpected number of return values from model.eval()")
@@ -1878,15 +2282,14 @@
     from .utils import _masks_to_masks_stack, _filter_cp_masks, _get_cellpose_batch_size
     from .io import _create_database, _save_object_counts_to_database, _check_masks, _get_avg_object_size
     from .timelapse import _npz_to_movie, _btrack_track_cells, _trackpy_track_cells
     from .plot import plot_masks
     
     #Note add logic that handles batches of size 1 as these will break the code batches must all be > 2 images
     gc.collect()
-    #print('========== generating masks ==========')
     
     if not torch.cuda.is_available():
         print(f'Torch CUDA is not available, using CPU')
     
     device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
     model = cp_models.Cellpose(gpu=True, model_type=model_name, device=device)
 
@@ -2043,17 +2446,17 @@
         gc.collect()
     return
 
 def all_elements_match(list1, list2):
     # Check if all elements in list1 are in list2
     return all(element in list2 for element in list1)
 
-def generate_cellpose_masks_v1(src, settings, object_type):
+def generate_cellpose_masks(src, settings, object_type):
     
-    from .utils import _masks_to_masks_stack, _filter_cp_masks, _get_cellpose_batch_size, _get_object_settings, _get_cellpose_channels, mask_object_count
+    from .utils import _masks_to_masks_stack, _filter_cp_masks, _get_cellpose_batch_size, _get_object_settings, _get_cellpose_channels, _choose_model, mask_object_count
     from .io import _create_database, _save_object_counts_to_database, _check_masks, _get_avg_object_size
     from .timelapse import _npz_to_movie, _btrack_track_cells, _trackpy_track_cells
     from .plot import plot_masks
     
     gc.collect()
     if not torch.cuda.is_available():
         print(f'Torch CUDA is not available, using CPU')
@@ -2075,32 +2478,28 @@
     
     object_settings = _get_object_settings(object_type, settings)
     model_name = object_settings['model_name']
     
     cellpose_channels = _get_cellpose_channels(src, settings['nucleus_channel'], settings['pathogen_channel'], settings['cell_channel'])
     if settings['verbose']:
         print(cellpose_channels)
+
     channels = cellpose_channels[object_type]
     cellpose_batch_size = _get_cellpose_batch_size()
-    
     device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-    model = cp_models.Cellpose(gpu=True, model_type=model_name, device=device) #net_avg=net_avg
-    #dn = denoise.CellposeDenoiseModel(model_type=f"denoise_{model_name}", gpu=True, device=device)
-    
+    model = _choose_model(model_name, device, object_type='cell', restore_type=None)
     chans = [2, 1] if model_name == 'cyto2' else [0,0] if model_name == 'nucleus' else [2,0] if model_name == 'cyto' else [2, 0] if model_name == 'cyto3' else [2, 0]
-    
     paths = [os.path.join(src, file) for file in os.listdir(src) if file.endswith('.npz')]    
     
     count_loc = os.path.dirname(src)+'/measurements/measurements.db'
     os.makedirs(os.path.dirname(src)+'/measurements', exist_ok=True)
     _create_database(count_loc)
     
     average_sizes = []
     time_ls = []
-
     for file_index, path in enumerate(paths):
         name = os.path.basename(path)
         name, ext = os.path.splitext(name)
         output_folder = os.path.join(os.path.dirname(path), object_type+'_mask_stack')
         os.makedirs(output_folder, exist_ok=True)
         overall_average_size = 0
         with np.load(path) as data:
@@ -2206,31 +2605,53 @@
                                                           timelapse_memory=timelapse_memory,
                                                           timelapse_remove_transient=timelapse_remove_transient,
                                                           plot=settings['plot'],
                                                           save=settings['save'],
                                                           mode=timelapse_mode)
                 else:
                     mask_stack = _masks_to_masks_stack(masks)
-
             else:
                 _save_object_counts_to_database(masks, object_type, batch_filenames, count_loc, added_string='_before_filtration')
-                mask_stack = _filter_cp_masks(masks=masks,
-                                              flows=flows,
-                                              filter_size=object_settings['filter_size'],
-                                              filter_intensity=object_settings['filter_intensity'],
-                                              minimum_size=object_settings['minimum_size'],
-                                              maximum_size=object_settings['maximum_size'],
-                                              remove_border_objects=object_settings['remove_border_objects'],
-                                              merge=False,
-                                              batch=batch,
-                                              plot=settings['plot'],
-                                              figuresize=figuresize)
-                
-                _save_object_counts_to_database(mask_stack, object_type, batch_filenames, count_loc, added_string='_after_filtration')
+                if object_settings['merge'] and not settings['filter']:
+                    mask_stack = _filter_cp_masks(masks=masks,
+                                                flows=flows,
+                                                filter_size=False,
+                                                filter_intensity=False,
+                                                minimum_size=object_settings['minimum_size'],
+                                                maximum_size=object_settings['maximum_size'],
+                                                remove_border_objects=False,
+                                                merge=object_settings['merge'],
+                                                batch=batch,
+                                                plot=settings['plot'],
+                                                figuresize=figuresize)
+
+                if settings['filter']:
+                    mask_stack = _filter_cp_masks(masks=masks,
+                                                flows=flows,
+                                                filter_size=object_settings['filter_size'],
+                                                filter_intensity=object_settings['filter_intensity'],
+                                                minimum_size=object_settings['minimum_size'],
+                                                maximum_size=object_settings['maximum_size'],
+                                                remove_border_objects=object_settings['remove_border_objects'],
+                                                merge=object_settings['merge'],
+                                                batch=batch,
+                                                plot=settings['plot'],
+                                                figuresize=figuresize)
+                    
+                    _save_object_counts_to_database(mask_stack, object_type, batch_filenames, count_loc, added_string='_after_filtration')
+                else:
+                    mask_stack = _masks_to_masks_stack(masks)
 
+                    if settings['plot']:
+                        for idx, (mask, flow, image) in enumerate(zip(masks, flows[0], batch)):
+                            if idx == 0:
+                                num_objects = mask_object_count(mask)
+                                print(f'Number of objects, : {num_objects}')
+                                plot_masks(batch=image, masks=mask, flows=flow, cmap='inferno', figuresize=figuresize, nr=1, file_type='.npz', print_object_number=True)
+        
             if not np.any(mask_stack):
                 average_obj_size = 0
             else:
                 average_obj_size = _get_avg_object_size(mask_stack)
 
             average_sizes.append(average_obj_size) 
             overall_average_size = np.mean(average_sizes) if len(average_sizes) > 0 else 0
@@ -2251,211 +2672,665 @@
                 np.save(output_filename, mask)
             mask_stack = []
             batch_filenames = []
         gc.collect()
     torch.cuda.empty_cache()
     return
 
-def generate_cellpose_masks(src, settings, object_type):
+def generate_masks_from_imgs(src, model, model_name, batch_size, diameter, cellprob_threshold, grayscale, save, normalize, channels, percentiles, circular, invert, plot, resize, target_height, target_width, verbose):
+    from .io import _load_images_and_labels, _load_normalized_images_and_labels
+    from .utils import resize_images_and_labels, resizescikit
+    from .plot import print_mask_and_flows
+
+    dst = os.path.join(src, model_name)
+    os.makedirs(dst, exist_ok=True)
     
-    from .utils import _masks_to_masks_stack, _filter_cp_masks, _get_cellpose_batch_size, _get_object_settings, _get_cellpose_channels, _choose_model, mask_object_count
-    from .io import _create_database, _save_object_counts_to_database, _check_masks, _get_avg_object_size
-    from .timelapse import _npz_to_movie, _btrack_track_cells, _trackpy_track_cells
-    from .plot import plot_masks
+    flow_threshold = 30
+    chans = [2, 1] if model_name == 'cyto2' else [0,0] if model_name == 'nucleus' else [1,0] if model_name == 'cyto' else [2, 0]
+
+    if grayscale:
+        chans=[0, 0]
+    
+    all_image_files = [os.path.join(src, f) for f in os.listdir(src) if f.endswith('.tif')]
+    random.shuffle(all_image_files)
     
-    gc.collect()
-    if not torch.cuda.is_available():
-        print(f'Torch CUDA is not available, using CPU')
         
-    figuresize=25
-    timelapse = settings['timelapse']
+    if verbose == True:
+        print(f'Cellpose settings: Model: {model_name}, channels: {channels}, cellpose_chans: {chans}, diameter:{diameter}, flow_threshold:{flow_threshold}, cellprob_threshold:{cellprob_threshold}')
     
-    if timelapse:
-        timelapse_displacement = settings['timelapse_displacement']
-        timelapse_frame_limits = settings['timelapse_frame_limits']
-        timelapse_memory = settings['timelapse_memory']
-        timelapse_remove_transient = settings['timelapse_remove_transient']
-        timelapse_mode = settings['timelapse_mode']
-        timelapse_objects = settings['timelapse_objects']
+    time_ls = []
+    for i in range(0, len(all_image_files), batch_size):
+        image_files = all_image_files[i:i+batch_size]
+
+        if normalize:
+            images, _, image_names, _ = _load_normalized_images_and_labels(image_files=image_files, label_files=None, signal_thresholds=100, channels=channels, percentiles=percentiles,  circular=circular, invert=invert, visualize=plot)
+            images = [np.squeeze(img) if img.shape[-1] == 1 else img for img in images]
+            orig_dims = [(image.shape[0], image.shape[1]) for image in images]
+        else:
+            images, _, image_names, _ = _load_images_and_labels(image_files=image_files, label_files=None, circular=circular, invert=invert) 
+            images = [np.squeeze(img) if img.shape[-1] == 1 else img for img in images]
+            orig_dims = [(image.shape[0], image.shape[1]) for image in images]
+        if resize:
+            images, _ = resize_images_and_labels(images, None, target_height, target_width, True)
+
+        for file_index, stack in enumerate(images):
+            start = time.time()
+            output = model.eval(x=stack,
+                         normalize=False,
+                         channels=chans,
+                         channel_axis=3,
+                         diameter=diameter,
+                         flow_threshold=flow_threshold,
+                         cellprob_threshold=cellprob_threshold,
+                         rescale=False,
+                         resample=False,
+                         progress=True)
+
+            if len(output) == 4:
+                mask, flows, _, _ = output
+            elif len(output) == 3:
+                mask, flows, _ = output
+            else:
+                raise ValueError("Unexpected number of return values from model.eval()")
+
+            if resize:
+                dims = orig_dims[file_index]
+                mask = resizescikit(mask, dims, order=0, preserve_range=True, anti_aliasing=False).astype(mask.dtype)
+
+            stop = time.time()
+            duration = (stop - start)
+            time_ls.append(duration)
+            average_time = np.mean(time_ls) if len(time_ls) > 0 else 0
+            print(f'Processing {file_index+1}/{len(images)} images : Time/image {average_time:.3f} sec', end='\r', flush=True)
+            if plot:
+                if resize:
+                    stack = resizescikit(stack, dims, preserve_range=True, anti_aliasing=False).astype(stack.dtype)
+                print_mask_and_flows(stack, mask, flows, overlay=True)
+            if save:
+                output_filename = os.path.join(dst, image_names[file_index])
+                cv2.imwrite(output_filename, mask)
+
+
+def check_cellpose_models(settings):
     
+    src = settings['src']
     batch_size = settings['batch_size']
-    cellprob_threshold = settings[f'{object_type}_CP_prob']
-    flow_threshold = 30
+    cellprob_threshold = settings['cellprob_threshold']
+    save = settings['save']
+    normalize = settings['normalize']
+    channels = settings['channels']
+    percentiles = settings['percentiles']
+    circular = settings['circular']
+    invert = settings['invert']
+    plot = settings['plot']
+    diameter = settings['diameter']
+    resize = settings['resize']
+    grayscale = settings['grayscale']
+    verbose = settings['verbose']
+    target_height = settings['width_height'][0]
+    target_width = settings['width_height'][1]
     
-    object_settings = _get_object_settings(object_type, settings)
-    model_name = object_settings['model_name']
+    cellpose_models = ['cyto', 'nuclei', 'cyto2', 'cyto3']
+    device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
     
-    cellpose_channels = _get_cellpose_channels(src, settings['nucleus_channel'], settings['pathogen_channel'], settings['cell_channel'])
-    if settings['verbose']:
-        print(cellpose_channels)
+    for model_name in cellpose_models:
 
-    channels = cellpose_channels[object_type]
-    cellpose_batch_size = _get_cellpose_batch_size()
-    device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-    model = _choose_model(model_name, device, object_type='cell', restore_type=None)
-    chans = [2, 1] if model_name == 'cyto2' else [0,0] if model_name == 'nucleus' else [2,0] if model_name == 'cyto' else [2, 0] if model_name == 'cyto3' else [2, 0]
-    paths = [os.path.join(src, file) for file in os.listdir(src) if file.endswith('.npz')]    
+        model = cp_models.CellposeModel(gpu=True, model_type=model_name, device=device)
+        print(f'Using {model_name}')
+        generate_masks_from_imgs(src, model, model_name, batch_size, diameter, cellprob_threshold, grayscale, save, normalize, channels, percentiles, circular, invert, plot, resize, target_height, target_width, verbose)
     
-    count_loc = os.path.dirname(src)+'/measurements/measurements.db'
-    os.makedirs(os.path.dirname(src)+'/measurements', exist_ok=True)
-    _create_database(count_loc)
+    return
+
+def compare_masks_v1(dir1, dir2, dir3, verbose=False):
     
-    average_sizes = []
-    time_ls = []
-    for file_index, path in enumerate(paths):
-        name = os.path.basename(path)
-        name, ext = os.path.splitext(name)
-        output_folder = os.path.join(os.path.dirname(path), object_type+'_mask_stack')
-        os.makedirs(output_folder, exist_ok=True)
-        overall_average_size = 0
-        with np.load(path) as data:
-            stack = data['data']
-            filenames = data['filenames']
-        if settings['timelapse']:
+    from .io import _read_mask
+    from .plot import visualize_masks, plot_comparison_results
+    from .utils import extract_boundaries, boundary_f1_score, compute_segmentation_ap, jaccard_index, dice_coefficient
+    
+    filenames = os.listdir(dir1)
+    results = []
+    cond_1 = os.path.basename(dir1)
+    cond_2 = os.path.basename(dir2)
+    cond_3 = os.path.basename(dir3)
 
-            trackable_objects = ['cell','nucleus','pathogen']
-            if not all_elements_match(settings['timelapse_objects'], trackable_objects):
-                print(f'timelapse_objects {settings["timelapse_objects"]} must be a subset of {trackable_objects}')
-                return
+    for index, filename in enumerate(filenames):
+        print(f'Processing image:{index+1}', end='\r', flush=True)
+        path1, path2, path3 = os.path.join(dir1, filename), os.path.join(dir2, filename), os.path.join(dir3, filename)
 
-            if len(stack) != batch_size:
-                print(f'Changed batch_size:{batch_size} to {len(stack)}, data length:{len(stack)}')
-                settings['timelapse_batch_size'] = len(stack)
-                batch_size = len(stack)
-                if isinstance(timelapse_frame_limits, list):
-                    if len(timelapse_frame_limits) >= 2:
-                        stack = stack[timelapse_frame_limits[0]: timelapse_frame_limits[1], :, :, :].astype(stack.dtype)
-                        filenames = filenames[timelapse_frame_limits[0]: timelapse_frame_limits[1]]
-                        batch_size = len(stack)
-                        print(f'Cut batch at indecies: {timelapse_frame_limits}, New batch_size: {batch_size} ')
+        print(path1)
+        print(path2)
+        print(path3)
+        
+        if os.path.exists(path2) and os.path.exists(path3):
+            
+            mask1, mask2, mask3 = _read_mask(path1), _read_mask(path2), _read_mask(path3)
+            boundary_true1, boundary_true2, boundary_true3 = extract_boundaries(mask1), extract_boundaries(mask2), extract_boundaries(mask3)
+            
+            
+            true_masks, pred_masks = [mask1], [mask2, mask3]  # Assuming mask1 is the ground truth for simplicity
+            true_labels, pred_labels_1, pred_labels_2 = label(mask1), label(mask2), label(mask3)
+            average_precision_0, average_precision_1 = compute_segmentation_ap(mask1, mask2), compute_segmentation_ap(mask1, mask3)
+            ap_scores = [average_precision_0, average_precision_1]
 
-        for i in range(0, stack.shape[0], batch_size):
-            mask_stack = []
-            start = time.time()
+            if verbose:
+                #unique_values1, unique_values2, unique_values3 = np.unique(mask1),  np.unique(mask2), np.unique(mask3)
+                #print(f"Unique values in mask 1: {unique_values1}, mask 2: {unique_values2}, mask 3: {unique_values3}")
+                visualize_masks(boundary_true1, boundary_true2, boundary_true3, title=f"Boundaries - {filename}")
+            
+            boundary_f1_12, boundary_f1_13, boundary_f1_23 = boundary_f1_score(mask1, mask2), boundary_f1_score(mask1, mask3), boundary_f1_score(mask2, mask3)
 
-            if stack.shape[3] == 1:
-                batch = stack[i: i+batch_size, :, :, [0,0]].astype(stack.dtype)
-            else:
-                batch = stack[i: i+batch_size, :, :, channels].astype(stack.dtype)
+            if (np.unique(mask1).size == 1 and np.unique(mask1)[0] == 0) and \
+               (np.unique(mask2).size == 1 and np.unique(mask2)[0] == 0) and \
+               (np.unique(mask3).size == 1 and np.unique(mask3)[0] == 0):
+                continue
+            
+            if verbose:
+                #unique_values4, unique_values5, unique_values6 = np.unique(boundary_f1_12), np.unique(boundary_f1_13), np.unique(boundary_f1_23)
+                #print(f"Unique values in boundary mask 1: {unique_values4}, mask 2: {unique_values5}, mask 3: {unique_values6}")
+                visualize_masks(mask1, mask2, mask3, title=filename)
+            
+            jaccard12 = jaccard_index(mask1, mask2)
+            dice12 = dice_coefficient(mask1, mask2)
+            
+            jaccard13 = jaccard_index(mask1, mask3)
+            dice13 = dice_coefficient(mask1, mask3)
+            
+            jaccard23 = jaccard_index(mask2, mask3)
+            dice23 = dice_coefficient(mask2, mask3)    
 
-            batch_filenames = filenames[i: i+batch_size].tolist()
+            results.append({
+                f'filename': filename,
+                f'jaccard_{cond_1}_{cond_2}': jaccard12,
+                f'dice_{cond_1}_{cond_2}': dice12,
+                f'jaccard_{cond_1}_{cond_3}': jaccard13,
+                f'dice_{cond_1}_{cond_3}': dice13,
+                f'jaccard_{cond_2}_{cond_3}': jaccard23,
+                f'dice_{cond_2}_{cond_3}': dice23,
+                f'boundary_f1_{cond_1}_{cond_2}': boundary_f1_12,
+                f'boundary_f1_{cond_1}_{cond_3}': boundary_f1_13,
+                f'boundary_f1_{cond_2}_{cond_3}': boundary_f1_23,
+                f'average_precision_{cond_1}_{cond_2}': ap_scores[0],
+                f'average_precision_{cond_1}_{cond_3}': ap_scores[1]
+            })
+        else:
+            print(f'Cannot find {path1} or {path2} or {path3}')
+    fig = plot_comparison_results(results)
+    return results, fig
 
-            if not settings['plot']:
-                batch, batch_filenames = _check_masks(batch, batch_filenames, output_folder)
-            if batch.size == 0:
-                print(f'Processing {file_index}/{len(paths)}: Images/npz {batch.shape[0]}')
-                continue
-            if batch.max() > 1:
-                batch = batch / batch.max()
+def compare_cellpose_masks_v1(src, verbose=False):
+    from .io import _read_mask
+    from .plot import visualize_masks, plot_comparison_results, visualize_cellpose_masks
+    from .utils import extract_boundaries, boundary_f1_score, compute_segmentation_ap, jaccard_index
 
-            if timelapse:
-                stitch_threshold=100.0
-                movie_path = os.path.join(os.path.dirname(src), 'movies')
-                os.makedirs(movie_path, exist_ok=True)
-                save_path = os.path.join(movie_path, f'timelapse_{object_type}_{name}.mp4')
-                _npz_to_movie(batch, batch_filenames, save_path, fps=2)
-            else:
-                stitch_threshold=0.0
+    import os
+    import numpy as np
+    from skimage.measure import label
+
+    # Collect all subdirectories in src
+    dirs = [os.path.join(src, d) for d in os.listdir(src) if os.path.isdir(os.path.join(src, d))]
+
+    dirs.sort()  # Optional: sort directories if needed
+
+    # Get common files in all directories
+    common_files = set(os.listdir(dirs[0]))
+    for d in dirs[1:]:
+        common_files.intersection_update(os.listdir(d))
+    common_files = list(common_files)
 
-            print('batch.shape',batch.shape)
-            masks, flows, _, _ = model.eval(x=batch,
-                                            batch_size=cellpose_batch_size,
-                                            normalize=False,
-                                            channels=chans,
-                                            channel_axis=3,
-                                            diameter=object_settings['diameter'],
-                                            flow_threshold=flow_threshold,
-                                            cellprob_threshold=cellprob_threshold,
-                                            rescale=None,
-                                            resample=object_settings['resample'],
-                                            stitch_threshold=stitch_threshold)
-            
-            if timelapse:
+    results = []
+    conditions = [os.path.basename(d) for d in dirs]
 
-                if settings['plot']:
-                    for idx, (mask, flow, image) in enumerate(zip(masks, flows[0], batch)):
-                        if idx == 0:
-                            num_objects = mask_object_count(mask)
-                            print(f'Number of objects: {num_objects}')
-                            plot_masks(batch=image, masks=mask, flows=flow, cmap='inferno', figuresize=figuresize, nr=1, file_type='.npz', print_object_number=True)
+    for index, filename in enumerate(common_files):
+        print(f'Processing image {index+1}/{len(common_files)}', end='\r', flush=True)
+        paths = [os.path.join(d, filename) for d in dirs]
+
+        # Check if file exists in all directories
+        if not all(os.path.exists(path) for path in paths):
+            print(f'Skipping {filename} as it is not present in all directories.')
+            continue
+
+        masks = [_read_mask(path) for path in paths]
+        boundaries = [extract_boundaries(mask) for mask in masks]
+
+        if verbose:
+            visualize_cellpose_masks(masks, titles=conditions, comparison_title=f"Masks Comparison for {filename}")
+
+        # Initialize data structure for results
+        file_results = {'filename': filename}
+
+        # Compare each mask with each other
+        for i in range(len(masks)):
+            for j in range(i + 1, len(masks)):
+                condition_i = conditions[i]
+                condition_j = conditions[j]
+                mask_i = masks[i]
+                mask_j = masks[j]
+
+                # Compute metrics
+                boundary_f1 = boundary_f1_score(mask_i, mask_j)
+                jaccard = jaccard_index(mask_i, mask_j)
+                average_precision = compute_segmentation_ap(mask_i, mask_j)
+
+                # Store results
+                file_results[f'jaccard_{condition_i}_{condition_j}'] = jaccard
+                file_results[f'boundary_f1_{condition_i}_{condition_j}'] = boundary_f1
+                file_results[f'average_precision_{condition_i}_{condition_j}'] = average_precision
 
-                _save_object_counts_to_database(masks, object_type, batch_filenames, count_loc, added_string='_timelapse')
-                if object_type in timelapse_objects:
-                    if timelapse_mode == 'btrack':
-                        if not timelapse_displacement is None:
-                            radius = timelapse_displacement
-                        else:
-                            radius = 100
+        results.append(file_results)
 
-                        workers = os.cpu_count()-2
-                        if workers < 1:
-                            workers = 1
+    fig = plot_comparison_results(results)
+    return results, fig
 
-                        mask_stack = _btrack_track_cells(src=src,
-                                                         name=name,
-                                                         batch_filenames=batch_filenames,
-                                                         object_type=object_type,
-                                                         plot=settings['plot'],
-                                                         save=settings['save'],
-                                                         masks_3D=masks,
-                                                         mode=timelapse_mode,
-                                                         timelapse_remove_transient=timelapse_remove_transient,
-                                                         radius=radius,
-                                                         workers=workers)
-                    if timelapse_mode == 'trackpy':
-                        mask_stack = _trackpy_track_cells(src=src,
-                                                          name=name,
-                                                          batch_filenames=batch_filenames,
-                                                          object_type=object_type,
-                                                          masks=masks,
-                                                          timelapse_displacement=timelapse_displacement,
-                                                          timelapse_memory=timelapse_memory,
-                                                          timelapse_remove_transient=timelapse_remove_transient,
-                                                          plot=settings['plot'],
-                                                          save=settings['save'],
-                                                          mode=timelapse_mode)
-                else:
-                    mask_stack = _masks_to_masks_stack(masks)
+def compare_mask(args):
+    src, filename, dirs, conditions = args
+    paths = [os.path.join(d, filename) for d in dirs]
+
+    if not all(os.path.exists(path) for path in paths):
+        return None
+
+    from .io import _read_mask  # Import here to avoid issues in multiprocessing
+    from .utils import extract_boundaries, boundary_f1_score, compute_segmentation_ap, jaccard_index
+    from .plot import plot_comparison_results
+
+    masks = [_read_mask(path) for path in paths]
+    file_results = {'filename': filename}
+
+    for i in range(len(masks)):
+        for j in range(i + 1, len(masks)):
+            mask_i, mask_j = masks[i], masks[j]
+            f1_score = boundary_f1_score(mask_i, mask_j)
+            jac_index = jaccard_index(mask_i, mask_j)
+            ap_score = compute_segmentation_ap(mask_i, mask_j)
+
+            file_results.update({
+                f'jaccard_{conditions[i]}_{conditions[j]}': jac_index,
+                f'boundary_f1_{conditions[i]}_{conditions[j]}': f1_score,
+                f'ap_{conditions[i]}_{conditions[j]}': ap_score
+            })
+    
+    return file_results
 
-            else:
-                _save_object_counts_to_database(masks, object_type, batch_filenames, count_loc, added_string='_before_filtration')
-                mask_stack = _filter_cp_masks(masks=masks,
-                                              flows=flows,
-                                              filter_size=object_settings['filter_size'],
-                                              filter_intensity=object_settings['filter_intensity'],
-                                              minimum_size=object_settings['minimum_size'],
-                                              maximum_size=object_settings['maximum_size'],
-                                              remove_border_objects=object_settings['remove_border_objects'],
-                                              merge=False,
-                                              batch=batch,
-                                              plot=settings['plot'],
-                                              figuresize=figuresize)
-                
-                _save_object_counts_to_database(mask_stack, object_type, batch_filenames, count_loc, added_string='_after_filtration')
+def compare_cellpose_masks(src, verbose=False, processes=None):
+    from .plot import visualize_cellpose_masks, plot_comparison_results
+    from .io import _read_mask
+    dirs = [os.path.join(src, d) for d in os.listdir(src) if os.path.isdir(os.path.join(src, d))]
+    dirs.sort()  # Optional: sort directories if needed
+    conditions = [os.path.basename(d) for d in dirs]
+
+    # Get common files in all directories
+    common_files = set(os.listdir(dirs[0]))
+    for d in dirs[1:]:
+        common_files.intersection_update(os.listdir(d))
+    common_files = list(common_files)
+
+    # Create a pool of workers
+    with Pool(processes=processes) as pool:
+        args = [(src, filename, dirs, conditions) for filename in common_files]
+        results = pool.map(compare_mask, args)
 
-            if not np.any(mask_stack):
-                average_obj_size = 0
-            else:
-                average_obj_size = _get_avg_object_size(mask_stack)
+    # Filter out None results (from skipped files)
+    results = [res for res in results if res is not None]
 
-            average_sizes.append(average_obj_size) 
-            overall_average_size = np.mean(average_sizes) if len(average_sizes) > 0 else 0
+    if verbose:
+        for result in results:
+            filename = result['filename']
+            masks = [_read_mask(os.path.join(d, filename)) for d in dirs]
+            visualize_cellpose_masks(masks, titles=conditions, comparison_title=f"Masks Comparison for {filename}")
 
-        stop = time.time()
-        duration = (stop - start)
-        time_ls.append(duration)
-        average_time = np.mean(time_ls) if len(time_ls) > 0 else 0
-        time_in_min = average_time/60
-        time_per_mask = average_time/batch_size
-        print(f'Processing {len(paths)}  files with {batch_size} imgs: {(file_index+1)*(batch_size+1)}/{(len(paths))*(batch_size+1)}: Time/batch {time_in_min:.3f} min: Time/mask {time_per_mask:.3f}sec: {object_type} size: {overall_average_size:.3f} px2')
-        if not timelapse:
-            if settings['plot']:
-                plot_masks(batch, mask_stack, flows, figuresize=figuresize, cmap='inferno', nr=batch_size)
-        if settings['save']:
-            for mask_index, mask in enumerate(mask_stack):
-                output_filename = os.path.join(output_folder, batch_filenames[mask_index])
-                np.save(output_filename, mask)
-            mask_stack = []
-            batch_filenames = []
-        gc.collect()
-    torch.cuda.empty_cache()
-    return
+    fig = plot_comparison_results(results)
+    return results, fig
+
+
+def _calculate_similarity(df, features, col_to_compare, val1, val2):
+    """
+    Calculate similarity scores of each well to the positive and negative controls using various metrics.
+    
+    Args:
+    df (pandas.DataFrame): DataFrame containing the data.
+    features (list): List of feature columns to use for similarity calculation.
+    col_to_compare (str): Column name to use for comparing groups.
+    val1, val2 (str): Values in col_to_compare to create subsets for comparison.
+
+    Returns:
+    pandas.DataFrame: DataFrame with similarity scores.
+    """
+    # Separate positive and negative control wells
+    pos_control = df[df[col_to_compare] == val1][features].mean()
+    neg_control = df[df[col_to_compare] == val2][features].mean()
+    
+    # Standardize features for Mahalanobis distance
+    scaler = StandardScaler()
+    scaled_features = scaler.fit_transform(df[features])
+    
+    # Regularize the covariance matrix to avoid singularity
+    cov_matrix = np.cov(scaled_features, rowvar=False)
+    inv_cov_matrix = None
+    try:
+        inv_cov_matrix = np.linalg.inv(cov_matrix)
+    except np.linalg.LinAlgError:
+        # Add a small value to the diagonal elements for regularization
+        epsilon = 1e-5
+        inv_cov_matrix = np.linalg.inv(cov_matrix + np.eye(cov_matrix.shape[0]) * epsilon)
+    
+    # Calculate similarity scores
+    df['similarity_to_pos_euclidean'] = df[features].apply(lambda row: euclidean(row, pos_control), axis=1)
+    df['similarity_to_neg_euclidean'] = df[features].apply(lambda row: euclidean(row, neg_control), axis=1)
+    df['similarity_to_pos_cosine'] = df[features].apply(lambda row: cosine(row, pos_control), axis=1)
+    df['similarity_to_neg_cosine'] = df[features].apply(lambda row: cosine(row, neg_control), axis=1)
+    df['similarity_to_pos_mahalanobis'] = df[features].apply(lambda row: mahalanobis(row, pos_control, inv_cov_matrix), axis=1)
+    df['similarity_to_neg_mahalanobis'] = df[features].apply(lambda row: mahalanobis(row, neg_control, inv_cov_matrix), axis=1)
+    df['similarity_to_pos_manhattan'] = df[features].apply(lambda row: cityblock(row, pos_control), axis=1)
+    df['similarity_to_neg_manhattan'] = df[features].apply(lambda row: cityblock(row, neg_control), axis=1)
+    df['similarity_to_pos_minkowski'] = df[features].apply(lambda row: minkowski(row, pos_control, p=3), axis=1)
+    df['similarity_to_neg_minkowski'] = df[features].apply(lambda row: minkowski(row, neg_control, p=3), axis=1)
+    df['similarity_to_pos_chebyshev'] = df[features].apply(lambda row: chebyshev(row, pos_control), axis=1)
+    df['similarity_to_neg_chebyshev'] = df[features].apply(lambda row: chebyshev(row, neg_control), axis=1)
+    df['similarity_to_pos_hamming'] = df[features].apply(lambda row: hamming(row, pos_control), axis=1)
+    df['similarity_to_neg_hamming'] = df[features].apply(lambda row: hamming(row, neg_control), axis=1)
+    df['similarity_to_pos_jaccard'] = df[features].apply(lambda row: jaccard(row, pos_control), axis=1)
+    df['similarity_to_neg_jaccard'] = df[features].apply(lambda row: jaccard(row, neg_control), axis=1)
+    df['similarity_to_pos_braycurtis'] = df[features].apply(lambda row: braycurtis(row, pos_control), axis=1)
+    df['similarity_to_neg_braycurtis'] = df[features].apply(lambda row: braycurtis(row, neg_control), axis=1)
+    
+    return df
+
+def _permutation_importance(df, feature_string='channel_3', col_to_compare='col', pos='c1', neg='c2', exclude=None, n_repeats=10, clean=True, nr_to_plot=30, n_estimators=100, test_size=0.2, random_state=42, model_type='xgboost', n_jobs=-1):
+    
+    """
+    Calculates permutation importance for numerical features in the dataframe,
+    comparing groups based on specified column values and uses the model to predict 
+    the class for all other rows in the dataframe.
+
+    Args:
+    df (pandas.DataFrame): The DataFrame containing the data.
+    feature_string (str): String to filter features that contain this substring.
+    col_to_compare (str): Column name to use for comparing groups.
+    pos, neg (str): Values in col_to_compare to create subsets for comparison.
+    exclude (list or str, optional): Columns to exclude from features.
+    n_repeats (int): Number of repeats for permutation importance.
+    clean (bool): Whether to remove columns with a single value.
+    nr_to_plot (int): Number of top features to plot based on permutation importance.
+    n_estimators (int): Number of trees in the random forest, gradient boosting, or XGBoost model.
+    test_size (float): Proportion of the dataset to include in the test split.
+    random_state (int): Random seed for reproducibility.
+    model_type (str): Type of model to use ('random_forest', 'logistic_regression', 'gradient_boosting', 'xgboost').
+    n_jobs (int): Number of jobs to run in parallel for applicable models.
+
+    Returns:
+    pandas.DataFrame: The original dataframe with added prediction and data usage columns.
+    pandas.DataFrame: DataFrame containing the importances and standard deviations.
+    """
+
+    if 'cells_per_well' in df.columns:
+        df = df.drop(columns=['cells_per_well'])
+
+    # Subset the dataframe based on specified column values
+    df1 = df[df[col_to_compare] == pos].copy()
+    df2 = df[df[col_to_compare] == neg].copy()
+
+    # Create target variable
+    df1['target'] = 0
+    df2['target'] = 1
+
+    # Combine the subsets for analysis
+    combined_df = pd.concat([df1, df2])
+
+    # Automatically select numerical features
+    features = combined_df.select_dtypes(include=[np.number]).columns.tolist()
+    features.remove('target')
+
+    if clean:
+        combined_df = combined_df.loc[:, combined_df.nunique() > 1]
+        features = [feature for feature in features if feature in combined_df.columns]
+        
+    if feature_string is not None:
+        feature_list = ['channel_0', 'channel_1', 'channel_2', 'channel_3']
+
+        # Remove feature_string from the list if it exists
+        if feature_string in feature_list:
+            feature_list.remove(feature_string)
+
+        features = [feature for feature in features if feature_string in feature]
+
+        # Iterate through the list and remove columns from df
+        for feature_ in feature_list:
+            features = [feature for feature in features if feature_ not in feature]
+            print(f'After removing {feature_} features: {len(features)}')
+
+    if exclude:
+        if isinstance(exclude, list):
+            features = [feature for feature in features if feature not in exclude]
+        else:
+            features.remove(exclude)
+
+    X = combined_df[features]
+    y = combined_df['target']
+
+    # Split the data into training and testing sets
+    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=random_state)
+    
+    # Label the data in the original dataframe
+    combined_df['data_usage'] = 'train'
+    combined_df.loc[X_test.index, 'data_usage'] = 'test'
+
+    # Initialize the model based on model_type
+    if model_type == 'random_forest':
+        model = RandomForestClassifier(n_estimators=n_estimators, random_state=random_state, n_jobs=n_jobs)
+    elif model_type == 'logistic_regression':
+        model = LogisticRegression(max_iter=1000, random_state=random_state, n_jobs=n_jobs)
+    elif model_type == 'gradient_boosting':
+        model = HistGradientBoostingClassifier(max_iter=n_estimators, random_state=random_state)  # Supports n_jobs internally
+    elif model_type == 'xgboost':
+        model = XGBClassifier(n_estimators=n_estimators, random_state=random_state, nthread=n_jobs, use_label_encoder=False, eval_metric='logloss')
+    else:
+        raise ValueError(f"Unsupported model_type: {model_type}")
+
+    model.fit(X_train, y_train)
+
+    perm_importance = permutation_importance(model, X_train, y_train, n_repeats=n_repeats, random_state=random_state, n_jobs=n_jobs)
+
+    # Create a DataFrame for permutation importances
+    permutation_df = pd.DataFrame({
+        'feature': [features[i] for i in perm_importance.importances_mean.argsort()],
+        'importance_mean': perm_importance.importances_mean[perm_importance.importances_mean.argsort()],
+        'importance_std': perm_importance.importances_std[perm_importance.importances_mean.argsort()]
+    }).tail(nr_to_plot)
+
+    # Plotting
+    fig, ax = plt.subplots()
+    ax.barh(permutation_df['feature'], permutation_df['importance_mean'], xerr=permutation_df['importance_std'], color="teal", align="center", alpha=0.6)
+    ax.set_xlabel('Permutation Importance')
+    plt.tight_layout()
+    plt.show()
+    
+    # Feature importance for models that support it
+    if model_type in ['random_forest', 'xgboost', 'gradient_boosting']:
+        feature_importances = model.feature_importances_
+        feature_importance_df = pd.DataFrame({
+            'feature': features,
+            'importance': feature_importances
+        }).sort_values(by='importance', ascending=False).head(nr_to_plot)
+        
+        # Plotting feature importance
+        fig, ax = plt.subplots()
+        ax.barh(feature_importance_df['feature'], feature_importance_df['importance'], color="blue", align="center", alpha=0.6)
+        ax.set_xlabel('Feature Importance')
+        plt.tight_layout()
+        plt.show()
+    else:
+        feature_importance_df = pd.DataFrame()
+
+    # Predicting the target variable for the test set
+    predictions_test = model.predict(X_test)
+    combined_df.loc[X_test.index, 'predictions'] = predictions_test
+
+    # Predicting the target variable for the training set
+    predictions_train = model.predict(X_train)
+    combined_df.loc[X_train.index, 'predictions'] = predictions_train
+
+    # Predicting the target variable for all other rows in the dataframe
+    X_all = df[features]
+    all_predictions = model.predict(X_all)
+    df['predictions'] = all_predictions
+
+    # Combine data usage labels back to the original dataframe
+    combined_data_usage = pd.concat([combined_df[['data_usage']], df[['predictions']]], axis=0)
+    df = df.join(combined_data_usage, how='left', rsuffix='_model')
+
+    # Calculating and printing the accuracy metrics
+    accuracy = accuracy_score(y_test, predictions_test)
+    precision = precision_score(y_test, predictions_test)
+    recall = recall_score(y_test, predictions_test)
+    f1 = f1_score(y_test, predictions_test)
+    print(f"Accuracy: {accuracy}")
+    print(f"Precision: {precision}")
+    print(f"Recall: {recall}")
+    print(f"F1 Score: {f1}")
+    
+    # Printing class-specific accuracy metrics
+    print("\nClassification Report:")
+    print(classification_report(y_test, predictions_test))
+
+    df = _calculate_similarity(df, features, col_to_compare, pos, neg)
+
+    return [df, permutation_df, feature_importance_df, model, X_train, X_test, y_train, y_test]
+
+def _shap_analysis(model, X_train, X_test):
+    
+    """
+    Performs SHAP analysis on the given model and data.
+
+    Args:
+    model: The trained model.
+    X_train (pandas.DataFrame): Training feature set.
+    X_test (pandas.DataFrame): Testing feature set.
+    """
+
+    explainer = shap.Explainer(model, X_train)
+    shap_values = explainer(X_test)
+
+    # Summary plot
+    shap.summary_plot(shap_values, X_test)
+
+def plate_heatmap(src, model_type='xgboost', variable='predictions', grouping='mean', min_max='allq', cmap='viridis', channel_of_interest=3, min_count=25, n_estimators=100, col_to_compare='col', pos='c1', neg='c2', exclude=None, n_repeats=10, clean=True, nr_to_plot=20, verbose=False, n_jobs=-1):
+    from .io import _read_and_merge_data
+    from .plot import _plot_plates
+
+    db_loc = [src+'/measurements/measurements.db']
+    tables = ['cell', 'nucleus', 'pathogen','cytoplasm']
+    include_multinucleated, include_multiinfected, include_noninfected = True, 2.0, True
+    
+    df, _ = _read_and_merge_data(db_loc, 
+                                 tables,
+                                 verbose=verbose,
+                                 include_multinucleated=include_multinucleated,
+                                 include_multiinfected=include_multiinfected,
+                                 include_noninfected=include_noninfected)
+        
+    if not channel_of_interest is None:
+        df['recruitment'] = df[f'pathogen_channel_{channel_of_interest}_mean_intensity']/df[f'cytoplasm_channel_{channel_of_interest}_mean_intensity']
+        feature_string = f'channel_{channel_of_interest}'
+    else:
+        feature_string = None
+    
+    output = _permutation_importance(df, feature_string, col_to_compare, pos, neg, exclude, n_repeats, clean, nr_to_plot, n_estimators=n_estimators, random_state=42, model_type=model_type, n_jobs=n_jobs)
+    
+    _shap_analysis(output[3], output[4], output[5])
+
+    features = output[0].select_dtypes(include=[np.number]).columns.tolist()
+
+    if not variable in features:
+        raise ValueError(f"Variable {variable} not found in the dataframe. Please choose one of the following: {features}")
+    
+    plate_heatmap = _plot_plates(output[0], variable, grouping, min_max, cmap, min_count)
+    return [output, plate_heatmap]
+
+def join_measurments_and_annotation(src, tables = ['cell', 'nucleus', 'pathogen','cytoplasm']):
+    
+    from .io import _read_and_merge_data, _read_db
+    
+    db_loc = [src+'/measurements/measurements.db']
+    loc = src+'/measurements/measurements.db'
+    df, _ = _read_and_merge_data(db_loc, 
+                                 tables, 
+                                 verbose=True, 
+                                 include_multinucleated=True, 
+                                 include_multiinfected=True, 
+                                 include_noninfected=True)
+    
+    paths_df = _read_db(loc, tables=['png_list'])
+
+    merged_df = pd.merge(df, paths_df[0], on='prcfo', how='left')
+
+    return merged_df
+
+def jitterplot_by_annotation(src, x_column, y_column, plot_title='Jitter Plot', output_path=None, filter_column=None, filter_values=None):
+    """
+    Reads a CSV file and creates a jitter plot of one column grouped by another column.
+    
+    Args:
+    src (str): Path to the source data.
+    x_column (str): Name of the column to be used for the x-axis.
+    y_column (str): Name of the column to be used for the y-axis.
+    plot_title (str): Title of the plot. Default is 'Jitter Plot'.
+    output_path (str): Path to save the plot image. If None, the plot will be displayed. Default is None.
+    
+    Returns:
+    pd.DataFrame: The filtered and balanced DataFrame.
+    """
+    # Read the CSV file into a DataFrame
+    df = join_measurments_and_annotation(src, tables=['cell', 'nucleus', 'pathogen', 'cytoplasm'])
+
+    # Print column names for debugging
+    print(f"Generated dataframe with: {df.shape[1]} columns and {df.shape[0]} rows")
+    #print("Columns in DataFrame:", df.columns.tolist())
+
+    # Replace NaN values with a specific label in x_column
+    df[x_column] = df[x_column].fillna('NaN')
+
+    # Filter the DataFrame if filter_column and filter_values are provided
+    if not filter_column is None:
+        if isinstance(filter_column, str):
+            df = df[df[filter_column].isin(filter_values)]
+        if isinstance(filter_column, list):
+            for i,val in enumerate(filter_column):
+                print(f'hello {len(df)}')
+                df = df[df[val].isin(filter_values[i])]
+
+    # Use the correct column names based on your DataFrame
+    required_columns = ['plate_x', 'row_x', 'col_x']
+    if not all(column in df.columns for column in required_columns):
+        raise KeyError(f"DataFrame does not contain the necessary columns: {required_columns}")
+
+    # Filter to retain rows with non-NaN values in x_column and with matching plate, row, col values
+    non_nan_df = df[df[x_column] != 'NaN']
+    retained_rows = df[df[['plate_x', 'row_x', 'col_x']].apply(tuple, axis=1).isin(non_nan_df[['plate_x', 'row_x', 'col_x']].apply(tuple, axis=1))]
+
+    # Determine the minimum count of examples across all groups in x_column
+    min_count = retained_rows[x_column].value_counts().min()
+    print(f'Found {min_count} annotated images')
+
+    # Randomly sample min_count examples from each group in x_column
+    balanced_df = retained_rows.groupby(x_column).apply(lambda x: x.sample(min_count, random_state=42)).reset_index(drop=True)
+
+    # Create the jitter plot
+    plt.figure(figsize=(10, 6))
+    jitter_plot = sns.stripplot(data=balanced_df, x=x_column, y=y_column, hue=x_column, jitter=True, palette='viridis', dodge=False)
+    plt.title(plot_title)
+    plt.xlabel(x_column)
+    plt.ylabel(y_column)
+    
+    # Customize the x-axis labels
+    plt.xticks(rotation=45, ha='right')
+    
+    # Adjust the position of the x-axis labels to be centered below the data
+    ax = plt.gca()
+    ax.set_xticklabels(ax.get_xticklabels(), rotation=45, ha='center')
+    
+    # Save the plot to a file or display it
+    if output_path:
+        plt.savefig(output_path, bbox_inches='tight')
+        print(f"Jitter plot saved to {output_path}")
+    else:
+        plt.show()
+
+    return balanced_df
```

### Comparing `spacr-0.0.20/spacr/graph_learning.py` & `spacr-0.0.21/spacr/graph_learning.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/spacr/graph_learning_lap.py` & `spacr-0.0.21/spacr/graph_learning_lap.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/spacr/gui_classify_app.py` & `spacr-0.0.21/spacr/gui_classify_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/spacr/gui_mask_app.py` & `spacr-0.0.21/spacr/gui_measure_app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,103 +1,104 @@
-import spacr, sys, ctypes, csv, matplotlib
+import sys, traceback, matplotlib, ctypes, csv
 import tkinter as tk
 from tkinter import ttk, scrolledtext
-from ttkthemes import ThemedTk
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
-from matplotlib.figure import Figure
-matplotlib.use('Agg')
-from tkinter import filedialog
+import matplotlib.pyplot as plt
+matplotlib.use('Agg')  # Use the non-GUI Agg backend
 from multiprocessing import Process, Queue, Value
-import traceback
+from ttkthemes import ThemedTk
+from tkinter import filedialog, StringVar, BooleanVar, IntVar, DoubleVar, Tk
 
 try:
     ctypes.windll.shcore.SetProcessDpiAwareness(True)
 except AttributeError:
     pass
 
 from .logger import log_function_call
-from .gui_utils import ScrollableFrame, StdoutRedirector, safe_literal_eval, clear_canvas, main_thread_update_function, create_dark_mode, set_dark_style, set_default_font, generate_fields, process_stdout_stderr
-from .gui_utils import mask_variables, check_mask_gui_settings, preprocess_generate_masks_wrapper, read_settings_from_csv, update_settings_from_csv #, add_mask_gui_defaults
+from .gui_utils import ScrollableFrame, StdoutRedirector, process_stdout_stderr, set_dark_style, set_default_font, generate_fields, create_dark_mode, main_thread_update_function
+from .gui_utils import measure_variables, measure_crop_wrapper, clear_canvas, safe_literal_eval, check_measure_gui_settings, read_settings_from_csv, update_settings_from_csv
 
 thread_control = {"run_thread": None, "stop_requested": False}
 
 @log_function_call
-def initiate_abort():
-    global thread_control
-    if thread_control.get("stop_requested") is not None:
-        thread_control["stop_requested"].value = 1
-
-    if thread_control.get("run_thread") is not None:
-        thread_control["run_thread"].join(timeout=5)
-        if thread_control["run_thread"].is_alive():
-            thread_control["run_thread"].terminate()
-        thread_control["run_thread"] = None
-        
-@log_function_call
-def run_mask_gui(q, fig_queue, stop_requested):
+def run_measure_gui(q, fig_queue, stop_requested):
     global vars_dict
     process_stdout_stderr(q)
     try:
-        settings = check_mask_gui_settings(vars_dict)
-        #settings = add_mask_gui_defaults(settings)
+        print('hello')
+        settings = check_measure_gui_settings(vars_dict)
         #for key in settings:
         #    value = settings[key]
         #    print(key, value, type(value))
-        preprocess_generate_masks_wrapper(settings, q, fig_queue)
+        measure_crop_wrapper(settings=settings, q=q, fig_queue=fig_queue)
     except Exception as e:
         q.put(f"Error during processing: {e}")
         traceback.print_exc()
     finally:
         stop_requested.value = 1
-    
+
 @log_function_call
 def start_process(q, fig_queue):
     global thread_control
     if thread_control.get("run_thread") is not None:
         initiate_abort()
 
     stop_requested = Value('i', 0)  # multiprocessing shared value for inter-process communication
     thread_control["stop_requested"] = stop_requested
-    thread_control["run_thread"] = Process(target=run_mask_gui, args=(q, fig_queue, stop_requested))
+    thread_control["run_thread"] = Process(target=run_measure_gui, args=(q, fig_queue, stop_requested))
     thread_control["run_thread"].start()
-    
+
+@log_function_call
+def initiate_abort():
+    global thread_control
+    if thread_control.get("stop_requested") is not None:
+        thread_control["stop_requested"].value = 1
+
+    if thread_control.get("run_thread") is not None:
+        thread_control["run_thread"].join(timeout=5)
+        if thread_control["run_thread"].is_alive():
+            thread_control["run_thread"].terminate()
+        thread_control["run_thread"] = None
+
+@log_function_call
 def import_settings(scrollable_frame):
     global vars_dict
 
     csv_file_path = filedialog.askopenfilename(filetypes=[("CSV files", "*.csv")])
     csv_settings = read_settings_from_csv(csv_file_path)
-    variables = mask_variables()
-    #variables = add_mask_gui_defaults(variables)
+    variables = measure_variables()
     new_settings = update_settings_from_csv(variables, csv_settings)
     vars_dict = generate_fields(new_settings, scrollable_frame)
-    
+
 @log_function_call
-def initiate_mask_root(width, height):
-    global root, vars_dict, q, canvas, fig_queue, canvas_widget, thread_control
-        
+def initiate_measure_root(width, height):
+    global root, vars_dict, q, canvas, fig_queue, canvas_widget, thread_control, variables
+    
     theme = 'breeze'
     
     if theme in ['clam']:
         root = tk.Tk()
         style = ttk.Style(root)
         style.theme_use(theme) #plastik, clearlooks, elegance, default was clam #alt, breeze, arc
         set_dark_style(style)
+
     elif theme in ['breeze']:
         root = ThemedTk(theme="breeze")
         style = ttk.Style(root)
         set_dark_style(style)
-        
+    
     set_default_font(root, font_name="Arial", size=10)
     #root.state('zoomed')  # For Windows to maximize the window
     root.attributes('-fullscreen', True)
     root.geometry(f"{width}x{height}")
+    root.configure(bg='#333333')
     root.title("SpaCer: generate masks")
     fig_queue = Queue()
-            
+    
     def _process_fig_queue():
         global canvas
         try:
             while not fig_queue.empty():
                 clear_canvas(canvas)
                 fig = fig_queue.get_nowait()
                 #set_fig_text_properties(fig, font_size=8)
@@ -123,25 +124,25 @@
     # Process queue for console output
     def _process_console_queue():
         while not q.empty():
             message = q.get_nowait()
             console_output.insert(tk.END, message)
             console_output.see(tk.END)
         console_output.after(100, _process_console_queue)
-        
+
     # Vertical container for settings and console
     vertical_container = tk.PanedWindow(root, orient=tk.HORIZONTAL) #VERTICAL
     vertical_container.pack(fill=tk.BOTH, expand=True)
 
     # Scrollable Frame for user settings
-    scrollable_frame = ScrollableFrame(vertical_container, bg='#333333')
+    scrollable_frame = ScrollableFrame(vertical_container)
     vertical_container.add(scrollable_frame, stretch="always")
 
     # Setup for user input fields (variables)
-    variables = mask_variables()
+    variables = measure_variables()
     vars_dict = generate_fields(variables, scrollable_frame)
     
     # Horizontal container for Matplotlib figure and the vertical pane (for settings and console)
     horizontal_container = tk.PanedWindow(vertical_container, orient=tk.VERTICAL) #HORIZONTAL
     vertical_container.add(horizontal_container, stretch="always")
 
     # Matplotlib figure setup
@@ -166,34 +167,34 @@
     # Queue and redirection setup for updating console output safely
     q = Queue()
     sys.stdout = StdoutRedirector(console_output)
     sys.stderr = StdoutRedirector(console_output)
     
     # This is your GUI setup where you create the Run button
     run_button = ttk.Button(scrollable_frame.scrollable_frame, text="Run",command=lambda: start_process(q, fig_queue))
-    run_button.grid(row=45, column=0, pady=10)
+    run_button.grid(row=40, column=0, pady=10)
     
     abort_button = ttk.Button(scrollable_frame.scrollable_frame, text="Abort", command=initiate_abort)
-    abort_button.grid(row=45, column=1, pady=10)
+    abort_button.grid(row=40, column=1, pady=10)
     
-    progress_label = ttk.Label(scrollable_frame.scrollable_frame, text="Processing: 0%", background="#333333", foreground="white")
+    progress_label = ttk.Label(scrollable_frame.scrollable_frame, text="Progress: ", background="#333333", foreground="white")
     progress_label.grid(row=41, column=0, columnspan=2, sticky="ew", pady=(5, 0))
     
     # Create the Import Settings button
     import_btn = tk.Button(root, text="Import Settings", command=lambda: import_settings(scrollable_frame))
     import_btn.pack(pady=20)
     
     _process_console_queue()
     _process_fig_queue()
     create_dark_mode(root, style, console_output)
     
-    root.after(100, lambda: main_thread_update_function(root, q, fig_queue, canvas_widget, progress_label))
+    #root.after(100, lambda: main_thread_update_function(root, q, fig_queue, canvas_widget, progress_label))
     
     return root, vars_dict
 
-def gui_mask():
+def gui_measure():
     global vars_dict, root
-    root, vars_dict = initiate_mask_root(1000, 1500)
+    root, vars_dict = initiate_measure_root(1000, 1500)
     root.mainloop()
-    
+
 if __name__ == "__main__":
-    gui_mask()
+    gui_measure()
```

### Comparing `spacr-0.0.20/spacr/gui_measure_app.py` & `spacr-0.0.21/spacr/gui_mask_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,112 @@
-import sys, traceback, matplotlib, ctypes, csv
+import sys, ctypes, matplotlib
 import tkinter as tk
 from tkinter import ttk, scrolledtext
+from ttkthemes import ThemedTk
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
-import matplotlib.pyplot as plt
-matplotlib.use('Agg')  # Use the non-GUI Agg backend
+from matplotlib.figure import Figure
+matplotlib.use('Agg')
+from tkinter import filedialog
 from multiprocessing import Process, Queue, Value
-from ttkthemes import ThemedTk
-from tkinter import filedialog, StringVar, BooleanVar, IntVar, DoubleVar, Tk
+import traceback
 
 try:
     ctypes.windll.shcore.SetProcessDpiAwareness(True)
 except AttributeError:
     pass
 
 from .logger import log_function_call
-from .gui_utils import ScrollableFrame, StdoutRedirector, process_stdout_stderr, set_dark_style, set_default_font, generate_fields, create_dark_mode, main_thread_update_function
-from .gui_utils import measure_variables, measure_crop_wrapper, clear_canvas, safe_literal_eval, check_measure_gui_settings, read_settings_from_csv, update_settings_from_csv
+from .gui_utils import ScrollableFrame, StdoutRedirector, clear_canvas, main_thread_update_function, create_dark_mode, set_dark_style, generate_fields, process_stdout_stderr, set_default_font, style_text_boxes
+from .gui_utils import mask_variables, check_mask_gui_settings, preprocess_generate_masks_wrapper, read_settings_from_csv, update_settings_from_csv#, toggle_advanced_settings
 
 thread_control = {"run_thread": None, "stop_requested": False}
 
+def toggle_advanced_settings():
+    advanced = advanced_var.get()
+    for widget in advanced_widgets:
+        if advanced:
+            widget.grid()
+        else:
+            widget.grid_remove()
+
 @log_function_call
-def run_measure_gui(q, fig_queue, stop_requested):
+def initiate_abort():
+    global thread_control
+    if thread_control.get("stop_requested") is not None:
+        thread_control["stop_requested"].value = 1
+
+    if thread_control.get("run_thread") is not None:
+        thread_control["run_thread"].join(timeout=5)
+        if thread_control["run_thread"].is_alive():
+            thread_control["run_thread"].terminate()
+        thread_control["run_thread"] = None
+        
+@log_function_call
+def run_mask_gui(q, fig_queue, stop_requested):
     global vars_dict
     process_stdout_stderr(q)
     try:
-        print('hello')
-        settings = check_measure_gui_settings(vars_dict)
+        settings = check_mask_gui_settings(vars_dict)
+        #settings = add_mask_gui_defaults(settings)
         #for key in settings:
         #    value = settings[key]
         #    print(key, value, type(value))
-        measure_crop_wrapper(settings=settings, q=q, fig_queue=fig_queue)
+        preprocess_generate_masks_wrapper(settings, q, fig_queue)
     except Exception as e:
         q.put(f"Error during processing: {e}")
         traceback.print_exc()
     finally:
         stop_requested.value = 1
-
+    
 @log_function_call
 def start_process(q, fig_queue):
     global thread_control
     if thread_control.get("run_thread") is not None:
         initiate_abort()
 
     stop_requested = Value('i', 0)  # multiprocessing shared value for inter-process communication
     thread_control["stop_requested"] = stop_requested
-    thread_control["run_thread"] = Process(target=run_measure_gui, args=(q, fig_queue, stop_requested))
+    thread_control["run_thread"] = Process(target=run_mask_gui, args=(q, fig_queue, stop_requested))
     thread_control["run_thread"].start()
-
-@log_function_call
-def initiate_abort():
-    global thread_control
-    if thread_control.get("stop_requested") is not None:
-        thread_control["stop_requested"].value = 1
-
-    if thread_control.get("run_thread") is not None:
-        thread_control["run_thread"].join(timeout=5)
-        if thread_control["run_thread"].is_alive():
-            thread_control["run_thread"].terminate()
-        thread_control["run_thread"] = None
-
-@log_function_call
+    
 def import_settings(scrollable_frame):
     global vars_dict
 
     csv_file_path = filedialog.askopenfilename(filetypes=[("CSV files", "*.csv")])
     csv_settings = read_settings_from_csv(csv_file_path)
-    variables = measure_variables()
+    variables = mask_variables()
+    #variables = add_mask_gui_defaults(variables)
     new_settings = update_settings_from_csv(variables, csv_settings)
     vars_dict = generate_fields(new_settings, scrollable_frame)
-
-@log_function_call
-def initiate_measure_root(width, height):
-    global root, vars_dict, q, canvas, fig_queue, canvas_widget, thread_control, variables
     
+@log_function_call
+def initiate_mask_root(width, height):
+    global root, vars_dict, q, canvas, fig_queue, canvas_widget, thread_control, advanced_widgets, advanced_var
+        
     theme = 'breeze'
     
     if theme in ['clam']:
         root = tk.Tk()
         style = ttk.Style(root)
         style.theme_use(theme) #plastik, clearlooks, elegance, default was clam #alt, breeze, arc
         set_dark_style(style)
-
     elif theme in ['breeze']:
         root = ThemedTk(theme="breeze")
         style = ttk.Style(root)
         set_dark_style(style)
-    
-    set_default_font(root, font_name="Arial", size=10)
+        
+    style_text_boxes(style)
+    set_default_font(root, font_name="Arial", size=8)
     #root.state('zoomed')  # For Windows to maximize the window
     root.attributes('-fullscreen', True)
     root.geometry(f"{width}x{height}")
-    root.configure(bg='#333333')
     root.title("SpaCer: generate masks")
     fig_queue = Queue()
-    
+            
     def _process_fig_queue():
         global canvas
         try:
             while not fig_queue.empty():
                 clear_canvas(canvas)
                 fig = fig_queue.get_nowait()
                 #set_fig_text_properties(fig, font_size=8)
@@ -124,26 +132,30 @@
     # Process queue for console output
     def _process_console_queue():
         while not q.empty():
             message = q.get_nowait()
             console_output.insert(tk.END, message)
             console_output.see(tk.END)
         console_output.after(100, _process_console_queue)
-
+        
     # Vertical container for settings and console
     vertical_container = tk.PanedWindow(root, orient=tk.HORIZONTAL) #VERTICAL
     vertical_container.pack(fill=tk.BOTH, expand=True)
 
     # Scrollable Frame for user settings
-    scrollable_frame = ScrollableFrame(vertical_container)
+    scrollable_frame = ScrollableFrame(vertical_container, bg='#333333')
     vertical_container.add(scrollable_frame, stretch="always")
 
     # Setup for user input fields (variables)
-    variables = measure_variables()
+    variables = mask_variables()
     vars_dict = generate_fields(variables, scrollable_frame)
+    #del vars_dict['fps']
+
+    # Debugging: print vars_dict to ensure it is populated correctly
+    #print("vars_dict:", vars_dict)
     
     # Horizontal container for Matplotlib figure and the vertical pane (for settings and console)
     horizontal_container = tk.PanedWindow(vertical_container, orient=tk.VERTICAL) #HORIZONTAL
     vertical_container.add(horizontal_container, stretch="always")
 
     # Matplotlib figure setup
     figure = Figure(figsize=(30, 4), dpi=100, facecolor='#333333')
@@ -164,37 +176,44 @@
     console_output = scrolledtext.ScrolledText(vertical_container, height=10)
     vertical_container.add(console_output, stretch="always")
 
     # Queue and redirection setup for updating console output safely
     q = Queue()
     sys.stdout = StdoutRedirector(console_output)
     sys.stderr = StdoutRedirector(console_output)
+
+    advanced_var = tk.BooleanVar()
+    advanced_checkbox = ttk.Checkbutton(scrollable_frame.scrollable_frame, text="Advanced Settings", variable=advanced_var, command=toggle_advanced_settings)
+    advanced_checkbox.grid(row=46, column=1, pady=10, padx=10)
     
     # This is your GUI setup where you create the Run button
     run_button = ttk.Button(scrollable_frame.scrollable_frame, text="Run",command=lambda: start_process(q, fig_queue))
-    run_button.grid(row=40, column=0, pady=10)
+    run_button.grid(row=45, column=0, pady=10, padx=10)
     
     abort_button = ttk.Button(scrollable_frame.scrollable_frame, text="Abort", command=initiate_abort)
-    abort_button.grid(row=40, column=1, pady=10)
-    
-    progress_label = ttk.Label(scrollable_frame.scrollable_frame, text="Progress: ", background="#333333", foreground="white")
-    progress_label.grid(row=41, column=0, columnspan=2, sticky="ew", pady=(5, 0))
+    abort_button.grid(row=45, column=1, pady=10, padx=10)
     
+    progress_label = ttk.Label(scrollable_frame.scrollable_frame, text="Processing: 0%", background="#333333", foreground="white")
+    progress_label.grid(row=41, column=0, columnspan=2, sticky="ew", pady=(5, 0), padx=10)
+
     # Create the Import Settings button
     import_btn = tk.Button(root, text="Import Settings", command=lambda: import_settings(scrollable_frame))
-    import_btn.pack(pady=20)
+    import_btn.pack(pady=20, padx=10)
+
     
+
     _process_console_queue()
     _process_fig_queue()
     create_dark_mode(root, style, console_output)
     
-    #root.after(100, lambda: main_thread_update_function(root, q, fig_queue, canvas_widget, progress_label))
+    root.after(100, lambda: main_thread_update_function(root, q, fig_queue, canvas_widget, progress_label))
     
     return root, vars_dict
 
-def gui_measure():
+def gui_mask():
     global vars_dict, root
-    root, vars_dict = initiate_measure_root(1000, 1500)
+    root, vars_dict = initiate_mask_root(1000, 1500)
+    
     root.mainloop()
-
+    
 if __name__ == "__main__":
-    gui_measure()
+    gui_mask()
```

### Comparing `spacr-0.0.20/spacr/gui_utils.py` & `spacr-0.0.21/spacr/gui_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,29 @@
 try:
     ctypes.windll.shcore.SetProcessDpiAwareness(True)
 except AttributeError:
     pass
 
 from .logger import log_function_call
 
+def set_default_font(root, font_name="Helvetica", size=12):
+    default_font = (font_name, size)
+    root.option_add("*Font", default_font)
+    root.option_add("*TButton.Font", default_font)
+    root.option_add("*TLabel.Font", default_font)
+    root.option_add("*TEntry.Font", default_font)
+
+def style_text_boxes(style):
+    style.configure('TEntry', padding='5 5 5 5', borderwidth=1, relief='solid', background='#333333', foreground='#ffffff')
+    style.configure('TButton', padding='10 10 10 10', borderwidth=1, relief='solid', background='#444444', foreground='#ffffff', font=('Helvetica', 12, 'bold'))
+    style.map('TButton',
+              background=[('active', '#555555'), ('disabled', '#222222')],
+              foreground=[('active', '#ffffff'), ('disabled', '#888888')])
+    style.configure('TLabel', padding='5 5 5 5', borderwidth=1, relief='flat', background='#2e2e2e', foreground='#ffffff')
+
 def read_settings_from_csv(csv_file_path):
     settings = {}
     with open(csv_file_path, newline='') as csvfile:
         reader = csv.DictReader(csvfile)
         for row in reader:
             key = row['Key']
             value = row['Value']
@@ -47,15 +62,15 @@
         fig.canvas.toolbar.pack_forget()
 
     event_handlers = fig.canvas.callbacks.callbacks
     for event, handlers in list(event_handlers.items()):
         for handler_id in list(handlers.keys()):
             fig.canvas.mpl_disconnect(handler_id)
 
-def set_default_font(app, font_name="Arial Bold", size=10):
+def set_default_font_v1(app, font_name="Arial Bold", size=10):
     default_font = nametofont("TkDefaultFont")
     text_font = nametofont("TkTextFont")
     fixed_font = nametofont("TkFixedFont")
     
     # Set the family to Open Sans and size as desired
     for font in (default_font, text_font, fixed_font):
         font.config(family=font_name, size=size)
@@ -576,15 +591,15 @@
 
     # Temporarily override plt.show
     original_show = plt.show
     plt.show = my_show
 
     try:
         print('start')
-        spacr.measure.measure_crop(settings=settings, annotation_settings={}, advanced_settings={})
+        spacr.measure.measure_crop(settings=settings)
     except Exception as e:
         errorMessage = f"Error during processing: {e}"
         q.put(errorMessage)  # Send the error message to the GUI via the queue
         traceback.print_exc()
     finally:
         plt.show = original_show  # Restore the original plt.show function
```

### Comparing `spacr-0.0.20/spacr/io.py` & `spacr-0.0.21/spacr/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, re, sqlite3, gc, torch, time, random, shutil, cv2, tarfile, cellpose
+import os, re, sqlite3, gc, torch, time, random, shutil, cv2, tarfile, cellpose, glob
 import numpy as np
 import pandas as pd
 import tifffile
 from PIL import Image
 from collections import defaultdict, Counter
 from pathlib import Path
 from functools import partial
@@ -41,37 +41,37 @@
     if not label_files is None:
         label_names = sorted([os.path.basename(f) for f in label_files])
     else:
         label_names = []
 
     if not image_files is None and not label_files is None: 
         for img_file, lbl_file in zip(image_files, label_files):
-            image = cellpose.imread(img_file)
+            image = cellpose.io.imread(img_file)
             if invert:
                 image = invert_image(image)
             if circular:
                 image = apply_mask(image, output_value=0)
-            label = cellpose.imread(lbl_file)
+            label = cellpose.io.imread(lbl_file)
             if image.max() > 1:
                 image = image / image.max()
             images.append(image)
             labels.append(label)
     elif not image_files is None:
         for img_file in image_files:
-            image = cellpose.imread(img_file)
+            image = cellpose.io.imread(img_file)
             if invert:
                 image = invert_image(image)
             if circular:
                 image = apply_mask(image, output_value=0)
             if image.max() > 1:
                 image = image / image.max()
             images.append(image)
     elif not image_files is None:
             for lbl_file in label_files:
-                label = cellpose.imread(lbl_file)
+                label = cellpose.io.imread(lbl_file)
                 if circular:
                     label = apply_mask(label, output_value=0)
             labels.append(label)
             
     if not image_files is None:
         image_dir = os.path.dirname(image_files[0])
     else:
@@ -105,23 +105,25 @@
     percentiles_1 = [[] for _ in range(num_channels)]
     percentiles_99 = [[] for _ in range(num_channels)]
 
     image_names = [os.path.basename(f) for f in image_files]
     
     if label_files is not None:
         label_names = [os.path.basename(f) for f in label_files]
+        label_dir = os.path.dirname(label_files[0])
 
     # Load images and check percentiles
     for i,img_file in enumerate(image_files):
-        image = cellpose.imread(img_file)
+        #print(img_file)
+        image = cellpose.io.imread(img_file)
         if invert:
             image = invert_image(image)
         if circular:
             image = apply_mask(image, output_value=0)
-            
+        #print(image.shape)
         # If specific channels are specified, select them
         if channels is not None and image.ndim == 3:
             image = image[..., channels]
         
         if image.ndim < 3:
             image = np.expand_dims(image, axis=-1)
         
@@ -165,102 +167,23 @@
     if not image_files is None:
         image_dir = os.path.dirname(image_files[0])
     else:
         image_dir = None
             
     if label_files is not None:
         for lbl_file in label_files:
-            labels.append(cellpose.imread(lbl_file))
+            labels.append(cellpose.io.imread(lbl_file))
     else:
         label_names = []
         label_dir = None
 
     print(f'Loaded and normalized {len(normalized_images)} images and {len(labels)} labels from {image_dir} and {label_dir}')
     
     return normalized_images, labels, image_names, label_names
 
-class MyDataset(Dataset):
-    """
-    Custom dataset class for loading and processing image data.
-
-    Args:
-        data_dir (str): The directory path where the data is stored.
-        loader_classes (list): List of class names.
-        transform (callable, optional): A function/transform that takes in an PIL image and returns a transformed version. Default is None.
-        shuffle (bool, optional): Whether to shuffle the dataset. Default is True.
-        load_to_memory (bool, optional): Whether to load images into memory. Default is False.
-
-    Attributes:
-        data_dir (str): The directory path where the data is stored.
-        classes (list): List of class names.
-        transform (callable): A function/transform that takes in an PIL image and returns a transformed version.
-        shuffle (bool): Whether to shuffle the dataset.
-        load_to_memory (bool): Whether to load images into memory.
-        filenames (list): List of file paths.
-        labels (list): List of labels corresponding to each file.
-        images (list): List of loaded images.
-        image_cache (Cache): Cache object for storing loaded images.
-
-    Methods:
-        load_image: Load an image from file.
-        __len__: Get the length of the dataset.
-        shuffle_dataset: Shuffle the dataset.
-        __getitem__: Get an item from the dataset.
-
-    """
-
-    def _init__(self, data_dir, loader_classes, transform=None, shuffle=True, load_to_memory=False):
-        from .utils import Cache
-        self.data_dir = data_dir
-        self.classes = loader_classes
-        self.transform = transform
-        self.shuffle = shuffle
-        self.load_to_memory = load_to_memory
-        self.filenames = []
-        self.labels = []
-        self.images = []
-        self.image_cache = Cache(50)  
-        for class_name in self.classes:
-            class_path = os.path.join(data_dir, class_name)
-            class_files = [os.path.join(class_path, f) for f in os.listdir(class_path) if os.path.isfile(os.path.join(class_path, f))]
-            self.filenames.extend(class_files)
-            self.labels.extend([self.classes.index(class_name)] * len(class_files))
-        if self.shuffle:
-            self.shuffle_dataset()
-        if self.load_to_memory:
-            self.images = [self.load_image(f) for f in self.filenames]
-
-    def load_image(self, img_path):
-        img = self.image_cache.get(img_path)
-        if img is None:
-            img = Image.open(img_path).convert('RGB')
-            self.image_cache.put(img_path, img)
-        return img
-
-    def _len__(self):
-        return len(self.filenames)
-
-    def shuffle_dataset(self):
-        combined = list(zip(self.filenames, self.labels))
-        random.shuffle(combined)
-        self.filenames, self.labels = zip(*combined)
-
-    def _getitem__(self, index):
-        label = self.labels[index]
-        filename = self.filenames[index]
-        if self.load_to_memory:
-            img = self.images[index]
-        else:
-            img = self.load_image(filename)
-        if self.transform is not None:
-            img = self.transform(img)
-        else:
-            img = ToTensor()(img)
-        return img, label, filename
-
 class CombineLoaders:
     """
     A class that combines multiple data loaders into a single iterator.
 
     Args:
         train_loaders (list): A list of data loaders.
 
@@ -379,14 +302,93 @@
             img = self.load_image(self.filenames[index])
         if self.transform is not None:
             img = self.transform(img)
         else:
             img = ToTensor()(img)
         # Return both the image and its filename
         return img, self.filenames[index]
+    
+class MyDataset_v1(Dataset):
+    """
+    Custom dataset class for loading and processing image data.
+
+    Args:
+        data_dir (str): The directory path where the data is stored.
+        loader_classes (list): List of class names.
+        transform (callable, optional): A function/transform that takes in an PIL image and returns a transformed version. Default is None.
+        shuffle (bool, optional): Whether to shuffle the dataset. Default is True.
+        load_to_memory (bool, optional): Whether to load images into memory. Default is False.
+
+    Attributes:
+        data_dir (str): The directory path where the data is stored.
+        classes (list): List of class names.
+        transform (callable): A function/transform that takes in an PIL image and returns a transformed version.
+        shuffle (bool): Whether to shuffle the dataset.
+        load_to_memory (bool): Whether to load images into memory.
+        filenames (list): List of file paths.
+        labels (list): List of labels corresponding to each file.
+        images (list): List of loaded images.
+        image_cache (Cache): Cache object for storing loaded images.
+
+    Methods:
+        load_image: Load an image from file.
+        __len__: Get the length of the dataset.
+        shuffle_dataset: Shuffle the dataset.
+        __getitem__: Get an item from the dataset.
+
+    """
+
+    def __init__(self, data_dir, loader_classes, transform=None, shuffle=True, load_to_memory=False):
+        from .utils import Cache
+        self.data_dir = data_dir
+        self.classes = loader_classes
+        self.transform = transform
+        self.shuffle = shuffle
+        self.load_to_memory = load_to_memory
+        self.filenames = []
+        self.labels = []
+        self.images = []
+        self.image_cache = Cache(50)  
+        for class_name in self.classes:
+            class_path = os.path.join(data_dir, class_name)
+            class_files = [os.path.join(class_path, f) for f in os.listdir(class_path) if os.path.isfile(os.path.join(class_path, f))]
+            self.filenames.extend(class_files)
+            self.labels.extend([self.classes.index(class_name)] * len(class_files))
+        if self.shuffle:
+            self.shuffle_dataset()
+        if self.load_to_memory:
+            self.images = [self.load_image(f) for f in self.filenames]
+
+    def load_image(self, img_path):
+        img = self.image_cache.get(img_path)
+        if img is None:
+            img = Image.open(img_path).convert('RGB')
+            self.image_cache.put(img_path, img)
+        return img
+
+    def _len__(self):
+        return len(self.filenames)
+
+    def shuffle_dataset(self):
+        combined = list(zip(self.filenames, self.labels))
+        random.shuffle(combined)
+        self.filenames, self.labels = zip(*combined)
+
+    def _getitem__(self, index):
+        label = self.labels[index]
+        filename = self.filenames[index]
+        if self.load_to_memory:
+            img = self.images[index]
+        else:
+            img = self.load_image(filename)
+        if self.transform is not None:
+            img = self.transform(img)
+        else:
+            img = ToTensor()(img)
+        return img, label, filename
 
 class MyDataset(Dataset):
     """
     A custom dataset class for loading and processing image data.
 
     Args:
         data_dir (str): The directory path where the image data is stored.
@@ -394,15 +396,15 @@
         transform (callable, optional): A function/transform to apply to the image data. Default is None.
         shuffle (bool, optional): Whether to shuffle the dataset. Default is True.
         pin_memory (bool, optional): Whether to pin the loaded images to memory. Default is False.
         specific_files (list, optional): A list of specific file paths to include in the dataset. Default is None.
         specific_labels (list, optional): A list of specific labels corresponding to the specific files. Default is None.
     """
 
-    def _init__(self, data_dir, loader_classes, transform=None, shuffle=True, pin_memory=False, specific_files=None, specific_labels=None):
+    def __init__(self, data_dir, loader_classes, transform=None, shuffle=True, pin_memory=False, specific_files=None, specific_labels=None):
         self.data_dir = data_dir
         self.classes = loader_classes
         self.transform = transform
         self.shuffle = shuffle
         self.pin_memory = pin_memory
         self.filenames = []
         self.labels = []
@@ -423,27 +425,27 @@
         if self.pin_memory:
             self.images = [self.load_image(f) for f in self.filenames]
     
     def load_image(self, img_path):
         img = Image.open(img_path).convert('RGB')
         return img
     
-    def _len__(self):
+    def __len__(self):
         return len(self.filenames)
     
     def shuffle_dataset(self):
         combined = list(zip(self.filenames, self.labels))
         random.shuffle(combined)
         self.filenames, self.labels = zip(*combined)
         
     def get_plate(self, filepath):
         filename = os.path.basename(filepath)  # Get just the filename from the full path
         return filename.split('_')[0]
     
-    def _getitem__(self, index):
+    def __getitem__(self, index):
         label = self.labels[index]
         filename = self.filenames[index]
         img = self.load_image(filename)
         if self.transform:
             img = self.transform(img)
         return img, label, filename
 
@@ -596,15 +598,15 @@
                 move = os.path.join(newpath, filename)
                 if os.path.exists(move):
                     print(f'WARNING: A file with the same name already exists at location {move}')
                 else:
                     shutil.move(os.path.join(src, filename), move)
     return
 
-def _merge_file(chan_dirs, stack_dir, file):
+def _merge_file_v1(chan_dirs, stack_dir, file):
     """
     Merge multiple channels into a single stack and save it as a numpy array.
 
     Args:
         chan_dirs (list): List of directories containing channel images.
         stack_dir (str): Directory to save the merged stack.
         file (str): File name of the channel image.
@@ -621,23 +623,88 @@
         for chan_dir in chan_dirs[1:]:
             img = cv2.imread(str(chan_dir / file.name), -1)
             chan = np.expand_dims(img, axis=2)
             channels.append(chan)
         stack = np.concatenate(channels, axis=2)
         np.save(new_file, stack)
 
-def _is_dir_empty(dir_path):
+def _merge_file_v1(chan_dirs, stack_dir, file):
     """
-    Check if a directory is empty.
+    Merge multiple channels into a single stack and save it as a numpy array.
+    Args:
+        chan_dirs (list): List of directories containing channel images.
+        stack_dir (str): Directory to save the merged stack.
+        file (str): File name of the channel image.
 
+    Returns:
+        None
+    """
+    new_file = stack_dir / (file.stem + '.npy')
+    if not new_file.exists():
+        stack_dir.mkdir(exist_ok=True)
+        channels = []
+        for i, chan_dir in enumerate(chan_dirs):
+            img_path = str(chan_dir / file.name)
+            img = cv2.imread(img_path, -1)
+            if img is None:
+                print(f"Warning: Failed to read image {img_path}")
+                continue
+            chan = np.expand_dims(img, axis=2)
+            channels.append(chan)
+            del img  # Explicitly delete the reference to the image to free up memory
+            if i % 10 == 0:  # Periodically suggest garbage collection
+                gc.collect()
+
+        if channels:
+            stack = np.concatenate(channels, axis=2)
+            np.save(new_file, stack)
+        else:
+            print(f"No valid channels to merge for file {file.name}")
+
+def _merge_file(chan_dirs, stack_dir, file_name):
+    """
+    Merge multiple channels into a single stack and save it as a numpy array, using os module for path handling.
+    
     Args:
-        dir_path (str): The path to the directory.
+        chan_dirs (list): List of directories containing channel images.
+        stack_dir (str): Directory to save the merged stack.
+        file_name (str): File name of the channel image.
 
     Returns:
-        bool: True if the directory is empty, False otherwise.
+        None
+    """
+    # Construct new file path
+    file_root, file_ext = os.path.splitext(file_name)
+    new_file = os.path.join(stack_dir, file_root + '.npy')
+    
+    # Check if the new file exists and create the stack directory if it doesn't
+    if not os.path.exists(new_file):
+        os.makedirs(stack_dir, exist_ok=True)
+        channels = []
+        for i, chan_dir in enumerate(chan_dirs):
+            img_path = os.path.join(chan_dir, file_name)
+            img = cv2.imread(img_path, -1)
+            if img is None:
+                print(f"Warning: Failed to read image {img_path}")
+                continue
+            chan = np.expand_dims(img, axis=2)
+            channels.append(chan)
+            del img  # Explicitly delete the reference to the image to free up memory
+            if i % 10 == 0:  # Periodically suggest garbage collection
+                gc.collect()
+
+        if channels:
+            stack = np.concatenate(channels, axis=2)
+            np.save(new_file, stack)
+        else:
+            print(f"No valid channels to merge for file {file_name}")
+
+def _is_dir_empty(dir_path):
+    """
+    Check if a directory is empty using os module.
     """
     return len(os.listdir(dir_path)) == 0
 
 def _generate_time_lists(file_list):
     """
     Generate sorted lists of filenames grouped by plate, well, and field.
 
@@ -729,15 +796,15 @@
                 move = os.path.join(newpath, filename)
                 if os.path.exists(move):
                     print(f'WARNING: A file with the same name already exists at location {move}')
                 else:
                     shutil.move(os.path.join(src, filename), move)
     return
 
-def _merge_channels(src, plot=False):
+def _merge_channels_v2(src, plot=False):
     from .plot import plot_arrays
     """
     Merge the channels in the given source directory and save the merged files in a 'stack' directory.
 
     Args:
         src (str): The path to the source directory containing the channel folders.
         plot (bool, optional): Whether to plot the merged arrays. Defaults to False.
@@ -757,26 +824,68 @@
     dir_files = list(chan_dirs[0].iterdir())
 
     # Create the 'stack' directory if it doesn't exist
     stack_dir.mkdir(exist_ok=True)
     print(f'generated folder with merged arrays: {stack_dir}')
 
     if _is_dir_empty(stack_dir):
-        with Pool(cpu_count()) as pool:
+        with Pool(max(cpu_count() // 2, 1)) as pool:
+        #with Pool(cpu_count()) as pool:
             merge_func = partial(_merge_file, chan_dirs, stack_dir)
             pool.map(merge_func, dir_files)
 
     avg_time = (time.time() - start_time) / len(dir_files)
     print(f'Average Time: {avg_time:.3f} sec')
 
     if plot:
         plot_arrays(src+'/stack')
 
     return
 
+def _merge_channels(src, plot=False):
+    """
+    Merge the channels in the given source directory and save the merged files in a 'stack' directory without using multiprocessing.
+    """
+
+    from .plot import plot_arrays
+    
+    stack_dir = os.path.join(src, 'stack')
+    allowed_names = ['01', '02', '03', '04', '00', '1', '2', '3', '4', '0']
+    
+    # List directories that match the allowed names
+    chan_dirs = [d for d in os.listdir(src) if os.path.isdir(os.path.join(src, d)) and d in allowed_names]
+    chan_dirs.sort()
+
+    print(f'List of folders in src: {chan_dirs}. Single channel folders.')
+    start_time = time.time()
+
+    # Assuming chan_dirs[0] is not empty and exists, adjust according to your logic
+    first_dir_path = os.path.join(src, chan_dirs[0])
+    dir_files = os.listdir(first_dir_path)
+
+    # Create the 'stack' directory if it doesn't exist
+    if not os.path.exists(stack_dir):
+        os.makedirs(stack_dir, exist_ok=True)
+    print(f'Generated folder with merged arrays: {stack_dir}')
+
+    if _is_dir_empty(stack_dir):
+        for file_name in dir_files:
+            full_file_path = os.path.join(first_dir_path, file_name)
+            if os.path.isfile(full_file_path):
+                _merge_file([os.path.join(src, d) for d in chan_dirs], stack_dir, file_name)
+
+    elapsed_time = time.time() - start_time
+    avg_time = elapsed_time / len(dir_files) if dir_files else 0
+    print(f'Average Time: {avg_time:.3f} sec, Total Elapsed Time: {elapsed_time:.3f} sec')
+
+    if plot:
+        plot_arrays(os.path.join(src, 'stack'))
+
+    return
+
 def _mip_all(src, include_first_chan=True):
     
     """
     Generate maximum intensity projections (MIPs) for each NumPy array file in the specified directory.
 
     Args:
         src (str): The directory path containing the NumPy array files.
@@ -1202,39 +1311,40 @@
         print(f'Could not find any {valid_ext} files in {src} only found {extension_counts[0]}')
         if os.path.exists(src+'/stack'):
             print('Found existing stack folder.')
         if os.path.exists(src+'/channel_stack'):
             print('Found existing channel_stack folder.')
         if os.path.exists(src+'/norm_channel_stack'):
             print('Found existing norm_channel_stack folder. Skipping preprocessing')
-            return
+            return settings, src
         
     cmap = 'inferno'
     figuresize = 20
     normalize = True
     save_dtype = 'uint16'
     correct_illumination = False
     
-    mask_channels = [settings['nucleus_channel'], settings['pathogen_channel'], settings['cell_channel']]
-    backgrounds = [settings['nucleus_background'], settings['pathogen_background'], settings['cell_background']]
+    #mask_channels = [settings['nucleus_channel'], settings['pathogen_channel'], settings['cell_channel']]
+    #backgrounds = [settings['nucleus_background'], settings['pathogen_background'], settings['cell_background']]
+    mask_channels = [settings['nucleus_channel'], settings['cell_channel'], settings['pathogen_channel']]
+    backgrounds = [settings['nucleus_background'], settings['cell_background'], settings['pathogen_background']]
     
     metadata_type = settings['metadata_type']
     custom_regex = settings['custom_regex']
     nr = settings['examples_to_plot']
     plot = settings['plot']
     batch_size = settings['batch_size']
     timelapse = settings['timelapse']
     remove_background = settings['remove_background']
     lower_quantile = settings['lower_quantile']
     randomize = settings['randomize']
     all_to_mip = settings['all_to_mip']
     pick_slice = settings['pick_slice']
     skip_mode = settings['skip_mode']
 
-
     if not img_format == None:
         if metadata_type == 'cellvoyager':
             regex = f'(?P<plateID>.*)_(?P<wellID>.*)_T(?P<timeID>.*)F(?P<fieldID>.*)L(?P<laserID>..)A(?P<AID>..)Z(?P<sliceID>.*)C(?P<chanID>.*){img_format}'
         elif metadata_type == 'cq1':
             regex = f'W(?P<wellID>.*)F(?P<fieldID>.*)T(?P<timeID>.*)Z(?P<sliceID>.*)C(?P<chanID>.*){img_format}'
         elif metadata_type == 'nikon':
             regex = f'(?P<plateID>.*)_(?P<wellID>.*)_T(?P<timeID>.*)F(?P<fieldID>.*)L(?P<laserID>..)A(?P<AID>..)Z(?P<sliceID>.*)C(?P<chanID>.*){img_format}'
@@ -1244,22 +1354,28 @@
             regex = f'(?P<plateID>.*)_(?P<wellID>.*)_T(?P<timeID>.*)F(?P<fieldID>.*)L(?P<laserID>..)A(?P<AID>..)Z(?P<sliceID>.*)C(?P<chanID>.*){img_format}'
         elif metadata_type == 'custom':
             regex = f'({custom_regex}){img_format}'
         
         print(f'regex mode:{metadata_type} regex:{regex}')
 
     if settings.get('test_mode', False):
+        print(f'Running spacr in test mode')
+        settings['plot'] = True
         try:
             os.rmdir(os.path.join(src, 'test'))
             print(f"Deleted test directory: {os.path.join(src, 'test')}")
         except OSError as e:
             pass
 
         src = _run_test_mode(settings['src'], regex, timelapse=timelapse)
         settings['src'] = src
+
+    if img_format == None:
+        if not os.path.exists(src+'/stack'):
+            _merge_channels(src, plot=False)   
     
     if not os.path.exists(src+'/stack'):
         try:
             if not img_format == None:
                 if timelapse:
                     _move_to_chan_folder(src, regex, timelapse, metadata_type)
                 else:
@@ -2269,14 +2385,16 @@
 
     npy_files = [f for f in files if f.endswith('.npy')]
     
     # Iterate over all files in the folder
     for i, filename in enumerate(files):
         if limit is not None and i >= limit:
             break
+        if not filename.endswith('.npy'):
+            continue
 
         # Construct the full file path
         file_path = os.path.join(folder_path, filename)
         # Load the numpy file
         numpy_array = np.load(file_path)
         
         # Construct the output TIFF file path
@@ -2285,15 +2403,55 @@
         
         # Save the numpy array as a TIFF file
         tifffile.imwrite(tiff_file_path, numpy_array)
         
         print(f"Converted {filename} to {tiff_filename} and saved in 'tiff' subdirectory.")
     return
     
+def generate_cellpose_train_test(src, test_split=0.1):
     
+    mask_src = os.path.join(src, 'masks')
+    img_paths = glob.glob(os.path.join(src, '*.tif'))
+    img_filenames = [os.path.basename(file) for file in img_paths + img_paths]
+    img_filenames = [file for file in img_filenames if os.path.exists(os.path.join(mask_src, file))]
+    print(f'Found {len(img_filenames)} images with masks')
+    
+    random.shuffle(img_filenames)
+    split_index = int(len(img_filenames) * test_split)
+    train_files = img_filenames[split_index:]
+    test_files = img_filenames[:split_index]
+    list_of_lists = [test_files, train_files]
+    print(f'Split dataset into Train {len(train_files)} and Test {len(test_files)} files')
+    
+    train_dir = os.path.join(os.path.dirname(src), 'train')
+    train_dir_masks = os.path.join(train_dir, 'mask')
+    test_dir = os.path.join(os.path.dirname(src), 'test')
+    test_dir_masks = os.path.join(test_dir, 'mask')
+    
+    os.makedirs(train_dir_masks, exist_ok=True)
+    os.makedirs(test_dir_masks, exist_ok=True)
+    for i, ls in enumerate(list_of_lists):
+        
+        if i == 0:
+            dst = test_dir
+            dst_mask = test_dir_masks
+            _type = 'Test'
+        if i == 1:
+            dst = train_dir
+            dst_mask = train_dir_masks
+            _type = 'Train'
+            
+        for idx, filename in enumerate(ls):
+            img_path = os.path.join(src, filename)
+            mask_path = os.path.join(mask_src, filename)
+            new_img_path = os.path.join(dst, filename)
+            new_mask_path = os.path.join(dst_mask, filename)            
+            shutil.copy(img_path, new_img_path)
+            shutil.copy(mask_path, new_mask_path)
+            print(f'Copied {idx+1}/{len(ls)} images to {_type} set', end='\r', flush=True)
```

### Comparing `spacr-0.0.20/spacr/logger.py` & `spacr-0.0.21/spacr/logger.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/spacr/mask_app.py` & `spacr-0.0.21/spacr/mask_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/spacr/measure.py` & `spacr-0.0.21/spacr/measure.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from scipy.ndimage import distance_transform_edt, generate_binary_structure
 from skimage.measure import regionprops, regionprops_table, shannon_entropy
 from skimage.exposure import rescale_intensity
 from scipy.ndimage import binary_dilation
 from skimage.segmentation import find_boundaries
 from skimage.feature import graycomatrix, graycoprops
 from mahotas.features import zernike_moments
+from skimage import morphology, measure, filters
+from skimage.util import img_as_bool
 
 from .logger import log_function_call
 
 #from .io import create_database, _save_settings_to_db
 #from .timelapse import _timelapse_masks_to_gif, _scmovie
 #from .plot import _plot_cropped_arrays, _save_scimg_plot
 #from .utils import _merge_overlapping_objects, _filter_object, _relabel_parent_with_child_labels, _exclude_objects
@@ -88,14 +90,77 @@
                 raise ValueError("All Zernike moments must be of the same length")
 
         zernike_df = pd.DataFrame(zernike_features, columns=[f'zernike_{i}' for i in range(feature_length)])
         return pd.concat([df.reset_index(drop=True), zernike_df], axis=1)
     else:
         return df
 
+def _analyze_cytoskeleton(array, mask, channel):
+    """
+    Analyzes and extracts skeleton properties from labeled objects in a masked image based on microtubule staining intensities.
+
+    Parameters:
+    image : numpy array
+        Intensity image where the microtubules are stained.
+    mask : numpy array
+        Mask where objects are labeled for analysis. Each label corresponds to a unique object.
+
+    Returns:
+    DataFrame
+        A pandas DataFrame containing the measured properties of each object's skeleton.
+    """
+
+    image = array[:, :, channel]
+
+    properties_list = []
+
+    # Process each object in the mask based on its label
+    for label in np.unique(mask):
+        if label == 0:
+            continue  # Skip background
+
+        # Isolate the object using the label
+        object_region = mask == label
+        region_intensity = np.where(object_region, image, 0)  # Use np.where for more efficient masking
+
+        # Ensure there are non-zero values to process
+        if np.any(region_intensity):
+            # Calculate adaptive offset based on intensity percentiles within the object
+            valid_pixels = region_intensity[region_intensity > 0]
+            if len(valid_pixels) > 1:  # Ensure there are enough pixels to compute percentiles
+                offset = np.percentile(valid_pixels, 90) - np.percentile(valid_pixels, 50)
+                block_size = 35  # Adjust this based on your object sizes and detail needs
+                local_thresh = filters.threshold_local(region_intensity, block_size=block_size, offset=offset)
+                cytoskeleton = region_intensity > local_thresh
+
+                # Skeletonize the thresholded cytoskeleton
+                skeleton = morphology.skeletonize(img_as_bool(cytoskeleton))
+
+                # Measure properties of the skeleton
+                skeleton_props = measure.regionprops(measure.label(skeleton), intensity_image=image)
+                skeleton_length = sum(prop.area for prop in skeleton_props)  # Sum of lengths of all skeleton segments
+                branch_data = morphology.skeleton_branch_analysis(skeleton)
+
+                # Store properties
+                properties = {
+                    "object_label": label,
+                    "skeleton_length": skeleton_length,
+                    "skeleton_branch_points": len(branch_data['branch_points'])
+                }
+                properties_list.append(properties)
+            else:
+                # Handle cases with insufficient pixels
+                properties_list.append({
+                    "object_label": label,
+                    "skeleton_length": 0,
+                    "skeleton_branch_points": 0
+                })
+
+    return pd.DataFrame(properties_list)
+
 @log_function_call
 def _morphological_measurements(cell_mask, nucleus_mask, pathogen_mask, cytoplasm_mask, settings, zernike=True, degree=8):
     """
     Calculate morphological measurements for cells, nucleus, pathogens, and cytoplasms based on the given masks.
 
     Args:
         cell_mask (ndarray): Binary mask of cell labels.
@@ -522,14 +587,15 @@
                         coloc_df.columns = [f'{ls[m]}_channel_{i}_channel_{j}_{col}' for col in coloc_df.columns]
                         dfs[m].append(coloc_df)
     
     return pd.concat(cell_dfs, axis=1), pd.concat(nucleus_dfs, axis=1), pd.concat(pathogen_dfs, axis=1), pd.concat(cytoplasm_dfs, axis=1)
 
 @log_function_call
 def _measure_crop_core(index, time_ls, file, settings):
+
     """
     Measure and crop the images based on specified settings.
 
     Parameters:
     - index: int
         The index of the image.
     - time_ls: list
@@ -620,17 +686,16 @@
         if settings['nucleus_min_size'] is not None and settings['nucleus_min_size'] != 0:
             nucleus_mask = _filter_object(nucleus_mask, settings['nucleus_min_size'])
         if settings['pathogen_min_size'] is not None and settings['pathogen_min_size'] != 0:
             pathogen_mask = _filter_object(pathogen_mask, settings['pathogen_min_size'])
         if settings['cytoplasm_min_size'] is not None and settings['cytoplasm_min_size'] != 0:
             cytoplasm_mask = _filter_object(cytoplasm_mask, settings['cytoplasm_min_size'])
 
-        if settings['cell_mask_dim'] is not None and settings['pathogen_mask_dim'] is not None:
-            if settings['include_uninfected'] == False:
-                cell_mask, nucleus_mask, pathogen_mask, cytoplasm_mask = _exclude_objects(cell_mask, nucleus_mask, pathogen_mask, cytoplasm_mask, include_uninfected=False)
+        if settings['cell_mask_dim'] is not None:
+            cell_mask, nucleus_mask, pathogen_mask, cytoplasm_mask = _exclude_objects(cell_mask, nucleus_mask, pathogen_mask, cytoplasm_mask, include_uninfected=settings['include_uninfected'])
 
         # Update data with the new masks
         if settings['cell_mask_dim'] is not None:
             data[:, :, settings['cell_mask_dim']] = cell_mask.astype(data_type)
         if settings['nucleus_mask_dim'] is not None:
             data[:, :, settings['nucleus_mask_dim']] = nucleus_mask.astype(data_type)
         if settings['pathogen_mask_dim'] is not None:
@@ -641,28 +706,31 @@
         if settings['plot_filtration']:
             _plot_cropped_arrays(data)
 
         if settings['save_measurements']:
 
             cell_df, nucleus_df, pathogen_df, cytoplasm_df = _morphological_measurements(cell_mask, nucleus_mask, pathogen_mask, cytoplasm_mask, settings)
 
+            #if settings['skeleton']:
+                #skeleton_df = _analyze_cytoskeleton(image=channel_arrays, mask=cell_mask, channel=1)
+                #merge skeleton_df with cell_df here
+
             cell_intensity_df, nucleus_intensity_df, pathogen_intensity_df, cytoplasm_intensity_df = _intensity_measurements(cell_mask, nucleus_mask, pathogen_mask, cytoplasm_mask, channel_arrays, settings, sizes=[1, 2, 3, 4, 5], periphery=True, outside=True)
             if settings['cell_mask_dim'] is not None:
                 cell_merged_df = _merge_and_save_to_database(cell_df, cell_intensity_df, 'cell', source_folder, file_name, settings['experiment'], settings['timelapse'])
 
             if settings['nucleus_mask_dim'] is not None:
                 nucleus_merged_df = _merge_and_save_to_database(nucleus_df, nucleus_intensity_df, 'nucleus', source_folder, file_name, settings['experiment'], settings['timelapse'])
 
             if settings['pathogen_mask_dim'] is not None:
                 pathogen_merged_df = _merge_and_save_to_database(pathogen_df, pathogen_intensity_df, 'pathogen', source_folder, file_name, settings['experiment'], settings['timelapse'])
 
             if settings['cytoplasm']:
                 cytoplasm_merged_df = _merge_and_save_to_database(cytoplasm_df, cytoplasm_intensity_df, 'cytoplasm', source_folder, file_name, settings['experiment'], settings['timelapse'])
 
-        
         if settings['save_png'] or settings['save_arrays'] or settings['plot']:
 
             if isinstance(settings['dialate_pngs'], bool):
                 dialate_pngs = [settings['dialate_pngs'], settings['dialate_pngs'], settings['dialate_pngs']]
             if isinstance(settings['dialate_pngs'], list):
                 dialate_pngs = settings['dialate_pngs']
 
@@ -727,15 +795,15 @@
                             png_folder = os.path.join(fldr,fldr_type)
 
                             img_path = os.path.join(png_folder, img_name)
                             
                             png_channels = data[:, :, settings['png_dims']].astype(data_type)
 
                             if settings['normalize_by'] == 'fov':
-                                percentiles_list = _get_percentiles(png_channels, settings['normalize_percentiles'][0],q2=settings['normalize_percentiles'][1])
+                                percentiles_list = _get_percentiles(png_channels, settings['normalize'][0],q2=settings['normalize'][1])
 
                             png_channels = _crop_center(png_channels, region, new_width=width, new_height=height)
 
                             if isinstance(settings['normalize'], list):
                                 if settings['normalize_by'] == 'png':
                                     png_channels = normalize_to_dtype(png_channels, q1=settings['normalize'][0],q2=settings['normalize'][1])
 
@@ -784,14 +852,15 @@
 
                                 try:
                                     conn = sqlite3.connect(f'{source_folder}/measurements/measurements.db', timeout=5)
                                     png_df.to_sql('png_list', conn, if_exists='append', index=False)
                                     conn.commit()
                                 except sqlite3.OperationalError as e:
                                     print(f"SQLite error: {e}", flush=True)
+                                    traceback.print_exc()
 
                             if settings['plot']:
                                 _plot_cropped_arrays(png_channels)
 
                         if settings['save_arrays']:
                             row_idx, col_idx = np.where(region)
                             region_array = data[row_idx.min():row_idx.max()+1, col_idx.min():col_idx.max()+1, :]
@@ -815,22 +884,21 @@
     end = time.time()
     duration = end-start
     time_ls.append(duration)
     average_time = np.mean(time_ls) if len(time_ls) > 0 else 0
     return average_time, cells
 
 @log_function_call
-def measure_crop(settings, annotation_settings, advanced_settings):
+def measure_crop(settings):
+    
     """
     Measure the crop of an image based on the provided settings.
 
     Args:
         settings (dict): The settings for measuring the crop.
-        annotation_settings (dict): The annotation settings.
-        advanced_settings (dict): The advanced settings.
 
     Returns:
         None
     """
 
     if settings.get('test_mode', False):
         if not os.basename(settings['src']) == 'test':
@@ -841,48 +909,66 @@
             print(f'Test mode enabled, using source folder {settings["src"]}')
     
     from .io import _save_settings_to_db
     from .timelapse import _timelapse_masks_to_gif, _scmovie
     from .plot import _save_scimg_plot
     from .utils import _list_endpoint_subdirectories, _generate_representative_images
     
-    settings = {**settings, **annotation_settings, **advanced_settings}
-    
-    dirname = os.path.dirname(settings['input_folder'])
-    settings_df = pd.DataFrame(list(settings.items()), columns=['Key', 'Value'])
-    settings_csv = os.path.join(dirname,'settings','measure_crop_settings.csv')
-    os.makedirs(os.path.join(dirname,'settings'), exist_ok=True)
-    settings_df.to_csv(settings_csv, index=False)
-
-    if settings['timelapse_objects'] == 'nucleus':
-        if not settings['cell_mask_dim'] is None:
-            tlo = settings['timelapse_objects']
-            print(f'timelapse object:{tlo}, cells will be relabeled to nucleus labels to track cells.')
-
     #general settings
     settings['merge_edge_pathogen_cells'] = True
     settings['radial_dist'] = True
     settings['calculate_correlation'] = True
     settings['manders_thresholds'] = [15,85,95]
     settings['homogeneity'] = True
     settings['homogeneity_distances'] = [8,16,32]
     settings['save_arrays'] = False
+
+    settings['dialate_pngs'] = False
+    settings['dialate_png_ratios'] = [0.2]
+    settings['timelapse'] = False
+    settings['representative_images'] = False
+    settings['timelapse_objects'] = 'cell'
+    settings['max_workers'] = os.cpu_count()-2
+    settings['experiment'] = 'test'
+    settings['cells'] = 'HeLa'
+    settings['cell_loc'] = None
+    settings['pathogens'] = ['ME49Dku80WT', 'ME49Dku80dgra8:GRA8', 'ME49Dku80dgra8', 'ME49Dku80TKO']
+    settings['pathogen_loc'] = [['c1', 'c2', 'c3', 'c4', 'c5', 'c6'], ['c7', 'c8', 'c9', 'c10', 'c11', 'c12'], ['c13', 'c14', 'c15', 'c16', 'c17', 'c18'], ['c19', 'c20', 'c21', 'c22', 'c23', 'c24']]
+    settings['treatments'] = ['BR1', 'BR2', 'BR3']
+    settings['treatment_loc'] = [['c1', 'c2', 'c7', 'c8', 'c13', 'c14', 'c19', 'c20'], ['c3', 'c4', 'c9', 'c10', 'c15', 'c16', 'c21', 'c22'], ['c5', 'c6', 'c11', 'c12', 'c17', 'c18', 'c23', 'c24']]
+    settings['channel_of_interest'] = 2
+    settings['compartments'] = ['pathogen', 'cytoplasm']
+    settings['measurement'] = 'mean_intensity'
+    settings['nr_imgs'] = 32
+    settings['um_per_pixel'] = 0.1
+    settings['center_crop'] = True
     
     if settings['cell_mask_dim'] is None:
         settings['include_uninfected'] = True
     if settings['pathogen_mask_dim'] is None:
         settings['include_uninfected'] = True
     if settings['cell_mask_dim'] is not None and settings['pathogen_min_size'] is not None:
         settings['cytoplasm'] = True
     elif settings['cell_mask_dim'] is not None and settings['nucleus_min_size'] is not None:
         settings['cytoplasm'] = True
     else:
         settings['cytoplasm'] = False
 
-    settings['center_crop'] = True
+    #settings = {**settings, **annotation_settings, **advanced_settings}
+    
+    dirname = os.path.dirname(settings['input_folder'])
+    settings_df = pd.DataFrame(list(settings.items()), columns=['Key', 'Value'])
+    settings_csv = os.path.join(dirname,'settings','measure_crop_settings.csv')
+    os.makedirs(os.path.join(dirname,'settings'), exist_ok=True)
+    settings_df.to_csv(settings_csv, index=False)
+
+    if settings['timelapse_objects'] == 'nucleus':
+        if not settings['cell_mask_dim'] is None:
+            tlo = settings['timelapse_objects']
+            print(f'timelapse object:{tlo}, cells will be relabeled to nucleus labels to track cells.')
 
     int_setting_keys = ['cell_mask_dim', 'nucleus_mask_dim', 'pathogen_mask_dim', 'cell_min_size', 'nucleus_min_size', 'pathogen_min_size', 'cytoplasm_min_size']
     
     if isinstance(settings['normalize'], bool) and settings['normalize']:
         print(f'WARNING: to notmalize single object pngs set normalize to a list of 2 integers, e.g. [1,99] (lower and upper percentiles)')
         return
 
@@ -918,66 +1004,66 @@
                 time.sleep(1)  # Wait for a short amount of time to avoid excessive printing
                 files_processed = len(time_ls)
                 files_to_process = len(files)
                 average_time = np.mean(time_ls) if len(time_ls) > 0 else 0
                 time_left = (((files_to_process-files_processed)*average_time)/max_workers)/60
                 print(f'Progress: {files_processed}/{files_to_process} Time/img {average_time:.3f}sec, Time Remaining {time_left:.3f} min.', end='\r', flush=True)
             result.get()
-    
-    if settings['save_png']:
-        img_fldr = os.path.join(os.path.dirname(settings['input_folder']), 'data')
-        sc_img_fldrs = _list_endpoint_subdirectories(img_fldr)
-
-        for i, well_src in enumerate(sc_img_fldrs):
-            if len(os.listdir(well_src)) < 16:
-                nr_imgs = len(os.listdir(well_src))
-                standardize = False
-            else:
-                nr_imgs = 16
-                standardize = True
-            try:
-                all_folders = len(sc_img_fldrs)
-                _save_scimg_plot(src=well_src, nr_imgs=nr_imgs, channel_indices=settings['png_dims'], um_per_pixel=0.1, scale_bar_length_um=10, standardize=standardize, fontsize=12, show_filename=True, channel_names=['red','green','blue'], dpi=300, plot=False, i=i, all_folders=all_folders)
-
-            except Exception as e:
-                print(f"Unable to generate figure for folder {well_src}: {e}", end='\r', flush=True)
-                #traceback.print_exc()
+
+    if settings['representative_images']:
+        if settings['save_png']:
+            img_fldr = os.path.join(os.path.dirname(settings['input_folder']), 'data')
+            sc_img_fldrs = _list_endpoint_subdirectories(img_fldr)
+
+            for i, well_src in enumerate(sc_img_fldrs):
+                if len(os.listdir(well_src)) < 16:
+                    nr_imgs = len(os.listdir(well_src))
+                    standardize = False
+                else:
+                    nr_imgs = 16
+                    standardize = True
+                try:
+                    all_folders = len(sc_img_fldrs)
+                    _save_scimg_plot(src=well_src, nr_imgs=nr_imgs, channel_indices=settings['png_dims'], um_per_pixel=0.1, scale_bar_length_um=10, standardize=standardize, fontsize=12, show_filename=True, channel_names=['red','green','blue'], dpi=300, plot=False, i=i, all_folders=all_folders)
+
+                except Exception as e:
+                    print(f"Unable to generate figure for folder {well_src}: {e}", end='\r', flush=True)
+                    #traceback.print_exc()
     
         if settings['save_measurements']:
-            if settings['representative_images']:
-                db_path = os.path.join(os.path.dirname(settings['input_folder']), 'measurements', 'measurements.db')
-                channel_indices = settings['png_dims']
-                channel_indices = [min(value, 2) for value in channel_indices]
-                _generate_representative_images(db_path,
-                                            cells=settings['cells'],
-                                            cell_loc=settings['cell_loc'],
-                                            pathogens=settings['pathogens'],
-                                            pathogen_loc=settings['pathogen_loc'],
-                                            treatments=settings['treatments'],
-                                            treatment_loc=settings['treatment_loc'],
-                                            channel_of_interest=settings['channel_of_interest'],
-                                            compartments = settings['compartments'],
-                                            measurement = settings['measurement'],
-                                            nr_imgs=settings['nr_imgs'],
-                                            channel_indices=channel_indices,
-                                            um_per_pixel=settings['um_per_pixel'],
-                                            scale_bar_length_um=10,
-                                            plot=False,
-                                            fontsize=12,
-                                            show_filename=True,
-                                            channel_names=None)
+            db_path = os.path.join(os.path.dirname(settings['input_folder']), 'measurements', 'measurements.db')
+            channel_indices = settings['png_dims']
+            channel_indices = [min(value, 2) for value in channel_indices]
+            _generate_representative_images(db_path,
+                                        cells=settings['cells'],
+                                        cell_loc=settings['cell_loc'],
+                                        pathogens=settings['pathogens'],
+                                        pathogen_loc=settings['pathogen_loc'],
+                                        treatments=settings['treatments'],
+                                        treatment_loc=settings['treatment_loc'],
+                                        channel_of_interest=settings['channel_of_interest'],
+                                        compartments = settings['compartments'],
+                                        measurement = settings['measurement'],
+                                        nr_imgs=settings['nr_imgs'],
+                                        channel_indices=channel_indices,
+                                        um_per_pixel=settings['um_per_pixel'],
+                                        scale_bar_length_um=10,
+                                        plot=False,
+                                        fontsize=12,
+                                        show_filename=True,
+                                        channel_names=None)
 
     if settings['timelapse']:
         if settings['timelapse_objects'] == 'nucleus':
             folder_path = settings['input_folder']
             mask_channels = [settings['nucleus_mask_dim'], settings['pathogen_mask_dim'],settings['cell_mask_dim']]
             object_types = ['nucleus','pathogen','cell']
             _timelapse_masks_to_gif(folder_path, mask_channels, object_types)
 
-        if settings['save_png']:
+        #if settings['save_png']:
             img_fldr = os.path.join(os.path.dirname(settings['input_folder']), 'data')
             sc_img_fldrs = _list_endpoint_subdirectories(img_fldr)
             _scmovie(sc_img_fldrs)
     print("Successfully completed run")
             
 def generate_cellpose_train_set(folders, dst, min_objects=5):
     os.makedirs(dst, exist_ok=True)
```

### Comparing `spacr-0.0.20/spacr/old_code.py` & `spacr-0.0.21/spacr/old_code.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/spacr/plot.py` & `spacr-0.0.21/spacr/plot.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 import scipy.ndimage as ndi
 import seaborn as sns
 import scipy.stats as stats
 import statsmodels.api as sm
-
+import imageio.v2 as imageio
 from IPython.display import display
 from skimage.segmentation import find_boundaries
 from skimage.measure import find_contours
 from skimage.morphology import square, dilation 
 from skimage import measure
 
 from ipywidgets import IntSlider, interact
@@ -191,14 +191,96 @@
         outline_colors = [[0, 1, 0], [0, 0, 1], [1, 0, 0]]  # gbr
     elif outline_color == 'rbg':
         outline_colors = [[1, 0, 0], [0, 0, 1], [0, 1, 0]]  # rbg
     else:
         outline_colors = [[1, 0, 0], [0, 0, 1], [0, 1, 0]]  # rbg
     return outline_colors
 
+def plot_images_and_arrays(folders, lower_percentile=1, upper_percentile=99, threshold=1000, extensions=['.npy', '.tif', '.tiff', '.png']):
+    """
+    Plot images and arrays from the given folders.
+
+    Args:
+        folders (list): A list of folder paths containing the images and arrays.
+        lower_percentile (int, optional): The lower percentile for image normalization. Defaults to 1.
+        upper_percentile (int, optional): The upper percentile for image normalization. Defaults to 99.
+        threshold (int, optional): The threshold for determining whether to display an image as a mask or normalize it. Defaults to 1000.
+        extensions (list, optional): A list of file extensions to consider. Defaults to ['.npy', '.tif', '.tiff', '.png'].
+    """
+
+    def normalize_image(image, lower=1, upper=99):
+        p2, p98 = np.percentile(image, (lower, upper))
+        return np.clip((image - p2) / (p98 - p2), 0, 1)
+
+    def find_files(folders, extensions=['.npy', '.tif', '.tiff', '.png']):
+        file_dict = {}
+
+        for folder in folders:
+            for root, _, files in os.walk(folder):
+                for file in files:
+                    if any(file.endswith(ext) for ext in extensions):
+                        file_name_wo_ext = os.path.splitext(file)[0]
+                        file_path = os.path.join(root, file)
+                        if file_name_wo_ext not in file_dict:
+                            file_dict[file_name_wo_ext] = {}
+                        file_dict[file_name_wo_ext][folder] = file_path
+
+        # Filter out files that don't have paths in all folders
+        filtered_dict = {k: v for k, v in file_dict.items() if len(v) == len(folders)}
+        return filtered_dict
+
+    def plot_from_file_dict(file_dict, threshold=1000, lower_percentile=1, upper_percentile=99):
+        """
+        Plot images and arrays from the given file dictionary.
+
+        Args:
+            file_dict (dict): A dictionary containing the file paths for each image or array.
+            threshold (int, optional): The threshold for determining whether to display an image as a mask or normalize it. Defaults to 1000.
+            lower_percentile (int, optional): The lower percentile for image normalization. Defaults to 1.
+            upper_percentile (int, optional): The upper percentile for image normalization. Defaults to 99.
+        """
+
+        for filename, folder_paths in file_dict.items():
+            num_files = len(folder_paths)
+            fig, axes = plt.subplots(1, num_files, figsize=(15, 5))
+            #fig.suptitle(filename)
+
+            # Ensure axes is always a list
+            if num_files == 1:
+                axes = [axes]
+
+            for i, (folder, path) in enumerate(folder_paths.items()):
+                if path.endswith('.npy'):
+                    data = np.load(path)
+                elif path.endswith('.tif') or path.endswith('.tiff'):
+                    data = imageio.imread(path)
+                else:
+                    continue
+
+                ax = axes[i]
+                unique_values = np.unique(data)
+                if len(unique_values) > threshold:
+                    # Normalize image to percentiles
+                    data = normalize_image(data, lower_percentile, upper_percentile)
+                    ax.imshow(data, cmap='gray')
+                else:
+                    # Display as mask with random colormap
+                    cmap = random_cmap(num_objects=len(unique_values))
+                    ax.imshow(data, cmap=cmap)
+
+                ax.set_title(f"{os.path.basename(folder)}: {os.path.basename(path)}")
+                ax.axis('off')
+            plt.tight_layout
+            plt.subplots_adjust(wspace=0.01, hspace=0.01)
+            plt.show()
+                        
+    file_dict = find_files(folders, extensions)
+    plot_from_file_dict(file_dict, threshold, lower_percentile, upper_percentile)
+    return
+
 def _filter_objects_in_plot(stack, cell_mask_dim, nucleus_mask_dim, pathogen_mask_dim, mask_dims, filter_min_max, include_multinucleated, include_multiinfected):
     """
     Filters objects in a plot based on various criteria.
 
     Args:
         stack (numpy.ndarray): The input stack of masks.
         cell_mask_dim (int): The dimension index of the cell mask.
@@ -951,15 +1033,15 @@
     canvas = np.zeros((img_height * n_row, img_width * n_col, 3))
     for i in range(n_row):
         for j in range(n_col):
             idx = i * n_col + j
             if idx < n_images:
                 canvas[i * img_height:(i + 1) * img_height, j * img_width:(j + 1) * img_width] = np.transpose(img[idx], (1, 2, 0))        
     plt.figure(figsize=(50, 50))
-    plt._imshow(canvas)
+    plt.imshow(canvas)
     plt.axis("off")
     for i, label in enumerate(labels):
         row = i // n_col
         col = i % n_col
         x = col * img_width + 2
         y = row * img_height + 15
         plt.text(x, y, label, color=color, fontsize=fontsize, fontweight='bold')
@@ -1039,68 +1121,96 @@
     for idx, row in df.iterrows():
         if row['p'] < 0.05:# and abs(row['effect']) > 0.1:
             plt.text(row['effect'], -np.log10(row['p']), idx, fontsize=12, ha='center', va='bottom', color='black')
 
     plt.axhline(y=-np.log10(0.05), color='gray', linestyle='--')  # line for p=0.05
     plt.show()
     
-def generate_plate_heatmap(df, plate_number, variable, grouping, min_max):
+def generate_plate_heatmap(df, plate_number, variable, grouping, min_max, min_count):
     df = df.copy()  # Work on a copy to avoid SettingWithCopyWarning
     df['plate'], df['row'], df['col'] = zip(*df['prc'].str.split('_'))
     
     # Filtering the dataframe based on the plate_number
     df = df[df['plate'] == plate_number].copy()  # Create another copy after filtering
     
     # Ensure proper ordering
     row_order = [f'r{i}' for i in range(1, 17)]
     col_order = [f'c{i}' for i in range(1, 28)]  # Exclude c15 as per your earlier code
     
     df['row'] = pd.Categorical(df['row'], categories=row_order, ordered=True)
     df['col'] = pd.Categorical(df['col'], categories=col_order, ordered=True)
-    
+    df['count'] = df.groupby(['row', 'col'])['row'].transform('count')
+
+    if min_count > 0:
+        df = df[df['count'] >= min_count]
+
     # Explicitly set observed=True to avoid FutureWarning
-    grouped = df.groupby(['row', 'col'], observed=True)  
+    grouped = df.groupby(['row', 'col'], observed=True) 
+
     
     if grouping == 'mean':
         plate = grouped[variable].mean().reset_index()
     elif grouping == 'sum':
         plate = grouped[variable].sum().reset_index()
     elif grouping == 'count':
+        variable = 'count'
         plate = grouped[variable].count().reset_index()
     else:
         raise ValueError(f"Unsupported grouping: {grouping}")
         
     plate_map = pd.pivot_table(plate, values=variable, index='row', columns='col').fillna(0)
     
     if min_max == 'all':
         min_max = [plate_map.min().min(), plate_map.max().max()]
     elif min_max == 'allq':
-        min_max = np.quantile(plate_map.values, [0.2, 0.98])
-    elif min_max == 'plate':
-        min_max = [plate_map.min().min(), plate_map.max().max()]
+        min_max = np.quantile(plate_map.values, [0.02, 0.98])
+    elif isinstance(min_max, (list, tuple)) and len(min_max) == 2:
+        if isinstance(min_max[0], (float)) and isinstance(min_max[1], (float)):
+            min_max = np.quantile(plate_map.values, [min_max[0], min_max[1]])
+        if isinstance(min_max[0], (int)) and isinstance(min_max[1], (int)): 
+            min_max = [min_max[0], min_max[1]]
         
     return plate_map, min_max
 
-def _plot_plates(df, variable, grouping, min_max, cmap):
+def _plot_plates(df, variable, grouping, min_max, cmap, min_count=0):
     plates = df['prc'].str.split('_', expand=True)[0].unique()
     n_rows, n_cols = (len(plates) + 3) // 4, 4
     fig, ax = plt.subplots(n_rows, n_cols, figsize=(40, 5 * n_rows))
     ax = ax.flatten()
 
     for index, plate in enumerate(plates):
-        plate_map, min_max_values = generate_plate_heatmap(df, plate, variable, grouping, min_max)
-        sns.heatmap(plate_map, cmap=cmap, vmin=0, vmax=2, ax=ax[index])
+        plate_map, min_max_values = generate_plate_heatmap(df, plate, variable, grouping, min_max, min_count)
+        sns.heatmap(plate_map, cmap=cmap, vmin=min_max_values[0], vmax=min_max_values[1], ax=ax[index])
         ax[index].set_title(plate)
         
     for i in range(len(plates), n_rows * n_cols):
         fig.delaxes(ax[i])
     
     plt.subplots_adjust(wspace=0.1, hspace=0.4)
     plt.show()
-    return
+    return fig
+
+#def plate_heatmap(src, variable='recruitment', grouping='mean', min_max='allq', cmap='viridis', channel_of_interest=3, min_count=25, verbose=False):
+#    db_loc = [src+'/measurements/measurements.db']
+#    tables = ['cell', 'nucleus', 'pathogen','cytoplasm']
+#    include_multinucleated, include_multiinfected, include_noninfected = True, 2.0, True
+#    df, _ = spacr.io._read_and_merge_data(db_loc, 
+#                                 tables,
+#                                 verbose=verbose,
+#                                 include_multinucleated=include_multinucleated,
+#                                 include_multiinfected=include_multiinfected,
+#                                 include_noninfected=include_noninfected)
+#    
+#    df['recruitment'] = df[f'pathogen_channel_{channel_of_interest}_outside_75_percentile']/df[f'cytoplasm_channel_{channel_of_interest}_mean_intensity']
+#
+#    spacr.plot._plot_plates(df, variable, grouping, min_max, cmap, min_count)
+#    #display(df)
+#    #for col in df.columns:
+#    #    print(col)
+#    return
 
 #from finetune cellpose
 #def plot_arrays(src, figuresize=50, cmap='inferno', nr=1, normalize=True, q1=1, q2=99):
 #    paths = []
 #    for file in os.listdir(src):
 #        if file.endswith('.tif') or file.endswith('.tiff'):
 #            path = os.path.join(src, file)
@@ -1232,14 +1342,43 @@
             # Normalize the image for displaying purposes
             norm = plt.Normalize(vmin=0, vmax=mask.max())
             ax.imshow(mask, cmap=cmap, norm=norm)
         ax.set_title(title)
         ax.axis('off')
     plt.suptitle(title)
     plt.show()
+
+def visualize_cellpose_masks(masks, titles=None, comparison_title="Masks Comparison"):
+    """
+    Visualize multiple masks with optional titles.
+    
+    Parameters:
+        masks (list of np.ndarray): A list of masks to visualize.
+        titles (list of str, optional): A list of titles for the masks. If None, default titles will be used.
+        comparison_title (str): Title for the entire figure.
+    """
+    if titles is None:
+        titles = [f'Mask {i+1}' for i in range(len(masks))]
+    
+    # Ensure the length of titles matches the number of masks
+    assert len(titles) == len(masks), "Number of titles and masks must match"
+    
+    num_masks = len(masks)
+    fig, axs = plt.subplots(1, num_masks, figsize=(10 * num_masks, 10))  # Adjusting figure size dynamically
+    
+    for ax, mask, title in zip(axs, masks, titles):
+        cmap = generate_mask_random_cmap(mask)
+        # Normalize and display the mask
+        norm = plt.Normalize(vmin=0, vmax=mask.max())
+        ax.imshow(mask, cmap=cmap, norm=norm)
+        ax.set_title(title)
+        ax.axis('off')
+    
+    plt.suptitle(comparison_title)
+    plt.show()
     
 def plot_comparison_results(comparison_results):
     df = pd.DataFrame(comparison_results)
     df_melted = pd.melt(df, id_vars=['filename'], var_name='metric', value_name='value')
     df_jaccard = df_melted[df_melted['metric'].str.contains('jaccard')]
     df_dice = df_melted[df_melted['metric'].str.contains('dice')]
     df_boundary_f1 = df_melted[df_melted['metric'].str.contains('boundary_f1')]
```

### Comparing `spacr-0.0.20/spacr/sim.py` & `spacr-0.0.21/spacr/sim.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 
-import os, gc, random, warnings, traceback, itertools, matplotlib, sqlite3
-import time as tm
+import os, random, warnings, traceback, sqlite3, shap, math, gc
 from time import time, sleep
 from datetime import datetime
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
+from matplotlib.patches import Patch
 import seaborn as sns
 import sklearn.metrics as metrics
-from sklearn.metrics import roc_curve, auc, roc_auc_score, confusion_matrix, precision_recall_curve
+from sklearn.ensemble import RandomForestRegressor, GradientBoostingRegressor
+from sklearn.inspection import PartialDependenceDisplay, permutation_importance
+from sklearn.metrics import roc_curve, auc, confusion_matrix, precision_recall_curve
 import statsmodels.api as sm
-from multiprocessing import cpu_count, Value, Array, Lock, Pool, Manager
+from multiprocessing import cpu_count, Pool, Manager
+from copy import deepcopy
 
 from .logger import log_function_call
 
 warnings.filterwarnings("ignore")
 warnings.filterwarnings("ignore", category=RuntimeWarning) # Ignore RuntimeWarning
 
 def generate_gene_list(number_of_genes, number_of_all_genes):
@@ -31,15 +34,15 @@
     genes_ls = list(range(number_of_all_genes))
     random.shuffle(genes_ls)
     gene_list = genes_ls[:number_of_genes]
     return gene_list
 
 # plate_map is a table with a row for each well, containing well metadata: plate_id, row_id, and column_id
 def generate_plate_map(nr_plates):
-    print('nr_plates',nr_plates)
+    #print('nr_plates',nr_plates)
     """
     Generate a plate map based on the number of plates.
 
     Parameters:
     nr_plates (int): The number of plates to generate the map for.
 
     Returns:
@@ -237,32 +240,37 @@
         tuple: A tuple containing the following:
             - cell_df (DataFrame): The DataFrame containing information about the cells.
             - genes_per_well_df (DataFrame): The DataFrame containing gene counts per well.
             - wells_per_gene_df (DataFrame): The DataFrame containing well counts per gene.
             - df_ls (list): A list containing gene counts per well, well counts per gene, Gini coefficients for wells,
               Gini coefficients for genes, gene weights array, and well weights.
     """
+
     #generate primary distributions and genes
     cpw, _ = dist_gen(avg_cells_per_well, sd_cells_per_well, plate_map)
     gpw, _ = dist_gen(avg_genes_per_well, sd_genes_per_well, plate_map)
     genes = [*range(1, number_of_genes+1, 1)]
     
     #gene_weights = generate_power_law_distribution(number_of_genes, gene_ineq_coeff)
     gene_weights = {gene: weight for gene, weight in zip(genes, generate_power_law_distribution(number_of_genes, gene_ineq_coeff))} # Generate gene_weights as a dictionary        
     gene_weights_array = np.array(list(gene_weights.values())) # Convert the values to an array
     
     well_weights = generate_power_law_distribution(len(plate_map), well_ineq_coeff)
-
-    gene_to_well_mapping = {}
-    
-    for gene in genes:
-        gene_to_well_mapping[gene] = np.random.choice(plate_map['plate_row_column'], size=int(gpw[gene-1]), p=well_weights) # Generate a number of wells for each gene according to well_weights
-    
-    gene_to_well_mapping = {gene: wells for gene, wells in gene_to_well_mapping.items() if len(wells) >= 2}
     
+    gene_to_well_mapping = {}
+    for gene in range(1, number_of_genes + 1):  # ensures gene-1 is within bounds
+        if gene-1 < len(gpw):
+            max_index = len(plate_map['plate_row_column'])  # this should be the number of choices available from plate_map
+            num_samples = int(gpw[gene-1])
+            if num_samples >= max_index:
+                num_samples = max_index - 1  # adjust to maximum possible index
+            gene_to_well_mapping[gene] = np.random.choice(plate_map['plate_row_column'], size=num_samples, replace=False, p=well_weights)
+        else:
+            break  # break the loop if gene-1 is out of bounds for gpw
+
     cells = []
     for i in [*range(0,len(plate_map))]:
         ciw = random.choice(cpw)
         present_genes = [gene for gene, wells in gene_to_well_mapping.items() if plate_map.loc[i, 'plate_row_column'] in wells] # Select genes present in the current well
         present_gene_weights = [gene_weights[gene] for gene in present_genes] # For sampling, filter gene_weights according to present_genes
         present_gene_weights /= np.sum(present_gene_weights)
         if present_genes:
@@ -312,17 +320,88 @@
         gini_val = gini_gene_well(x)
         ls_.append(val)
         gini_ls.append(gini_val)
     gini_gene = np.array(gini_ls)
     df_ls = [gene_counts_per_well, well_counts_per_gene, gini_well, gini_gene, gene_weights_array, well_weights]
     return cell_df, genes_per_well_df, wells_per_gene_df, df_ls
 
-# classifier is a function that takes a cell state (active=1/inactive=0) and produces a score in [0, 1]
-# For the input cell, it checks if it is active or inactive, and then samples from an appropriate beta distribution to give a score
-def classifier(positive_mean, positive_variance, negative_mean, negative_variance, df):
+def classifier(positive_mean, positive_variance, negative_mean, negative_variance, classifier_accuracy, df):
+    """
+    Classifies the data in the DataFrame based on the given parameters and a classifier error rate.
+
+    Args:
+        positive_mean (float): The mean of the positive distribution.
+        positive_variance (float): The variance of the positive distribution.
+        negative_mean (float): The mean of the negative distribution.
+        negative_variance (float): The variance of the negative distribution.
+        classifier_accuracy (float): The likelihood (0 to 1) that a gene is correctly classified according to its true label.
+        df (pandas.DataFrame): The DataFrame containing the data to be classified.
+
+    Returns:
+        pandas.DataFrame: The DataFrame with an additional 'score' column containing the classification scores.
+    """
+    def calc_alpha_beta(mean, variance):
+        if mean <= 0 or mean >= 1:
+            raise ValueError("Mean must be between 0 and 1 exclusively.")
+        max_variance = mean * (1 - mean)
+        if variance <= 0 or variance >= max_variance:
+            raise ValueError(f"Variance must be positive and less than {max_variance}.")
+        
+        alpha = mean * (mean * (1 - mean) / variance - 1)
+        beta = alpha * (1 - mean) / mean
+        return alpha, beta
+    
+    # Apply the beta distribution based on 'is_active' status with consideration for classifier error
+    def get_score(is_active):
+        if np.random.rand() < classifier_accuracy:  # With classifier_accuracy probability, choose the correct distribution
+            return np.random.beta(a1, b1) if is_active else np.random.beta(a2, b2)
+        else:  # With 1-classifier_accuracy probability, choose the incorrect distribution
+            return np.random.beta(a2, b2) if is_active else np.random.beta(a1, b1)
+
+    # Calculate alpha and beta for both distributions
+    a1, b1 = calc_alpha_beta(positive_mean, positive_variance)
+    a2, b2 = calc_alpha_beta(negative_mean, negative_variance)
+    df['score'] = df['is_active'].apply(get_score)
+
+    return df
+
+def classifier_v2(positive_mean, positive_variance, negative_mean, negative_variance, df):
+    """
+    Classifies the data in the DataFrame based on the given parameters.
+
+    Args:
+        positive_mean (float): The mean of the positive distribution.
+        positive_variance (float): The variance of the positive distribution.
+        negative_mean (float): The mean of the negative distribution.
+        negative_variance (float): The variance of the negative distribution.
+        df (pandas.DataFrame): The DataFrame containing the data to be classified.
+
+    Returns:
+        pandas.DataFrame: The DataFrame with an additional 'score' column containing the classification scores.
+    """
+    def calc_alpha_beta(mean, variance):
+        if mean <= 0 or mean >= 1:
+            raise ValueError("Mean must be between 0 and 1 exclusively.")
+        max_variance = mean * (1 - mean)
+        if variance <= 0 or variance >= max_variance:
+            raise ValueError(f"Variance must be positive and less than {max_variance}.")
+        
+        alpha = mean * (mean * (1 - mean) / variance - 1)
+        beta = alpha * (1 - mean) / mean
+        return alpha, beta
+
+    # Calculate alpha and beta for both distributions
+    a1, b1 = calc_alpha_beta(positive_mean, positive_variance)
+    a2, b2 = calc_alpha_beta(negative_mean, negative_variance)
+
+    # Apply the beta distribution based on 'is_active' status
+    df['score'] = df['is_active'].apply(lambda is_active: np.random.beta(a1, b1) if is_active else np.random.beta(a2, b2))
+    return df
+
+def classifier_v1(positive_mean, positive_variance, negative_mean, negative_variance, df):
     """
     Classifies the data in the DataFrame based on the given parameters.
 
     Args:
         positive_mean (float): The mean of the positive distribution.
         positive_variance (float): The variance of the positive distribution.
         negative_mean (float): The mean of the negative distribution.
@@ -442,28 +521,30 @@
     well_score = cell_scores.groupby(['plate_row_column']).agg(
         average_active_score=('is_active', 'mean'),
         gene_list=('gene_id', lambda x: np.unique(x).tolist()))
     well_score['score'] = np.log10(well_score['average_active_score'] + 1)
     return well_score
 
 def sequence_plates(well_score, number_of_genes, avg_reads_per_gene, sd_reads_per_gene, sequencing_error=0.01):
+
     """
     Simulates the sequencing of plates and calculates gene fractions and metadata.
 
     Parameters:
     well_score (pd.DataFrame): DataFrame containing well scores and gene lists.
     number_of_genes (int): Number of genes.
     avg_reads_per_gene (float): Average number of reads per gene.
     sd_reads_per_gene (float): Standard deviation of reads per gene.
     sequencing_error (float, optional): Probability of introducing sequencing error. Defaults to 0.01.
 
     Returns:
     gene_fraction_map (pd.DataFrame): DataFrame containing gene fractions for each well.
     metadata (pd.DataFrame): DataFrame containing metadata for each well.
     """
+
     reads, _ = dist_gen(avg_reads_per_gene, sd_reads_per_gene, well_score)
     gene_names = [f'gene_{v}' for v in range(number_of_genes+1)]
     all_wells = well_score.index
 
     gene_counts_map = pd.DataFrame(np.zeros((len(all_wells), number_of_genes+1)), columns=gene_names, index=all_wells)
     sum_reads = []
 
@@ -608,16 +689,20 @@
     - title: The title of the plot.
     - binwidth: The width of each histogram bin.
     - log: Whether to use a logarithmic scale for the y-axis.
 
     Returns:
     None
     """
-    sns.histplot(data=data, x=x_label, ax=ax, color=color, binwidth=binwidth, kde=False, stat='density', 
-                 legend=False, fill=True, element='step', palette='dark')
+    if not binwidth:
+        sns.histplot(data=data, x=x_label, ax=ax, color=color, kde=False, stat='density', 
+                    legend=False, fill=True, element='step', palette='dark')
+    else:
+        sns.histplot(data=data, x=x_label, ax=ax, color=color, binwidth=binwidth, kde=False, stat='density', 
+                    legend=False, fill=True, element='step', palette='dark')
     if log:
         ax.set_yscale('log')
     ax.set_title(title)
     ax.set_xlabel(x_label)
 
 def plot_roc_pr(data, ax, title, x_label, y_label):
     """
@@ -696,15 +781,15 @@
     control_gene_list = generate_gene_list(settings['number_of_control_genes'], settings['number_of_genes'])
     plate_map = generate_plate_map(settings['nr_plates'])
 
     #control_map = plate_map[plate_map['column_id'].isin(['c1', 'c2', 'c3', 'c23', 'c24'])] # Extract rows where 'column_id' is in [1,2,3,23,24]
     plate_map = plate_map[~plate_map['column_id'].isin(['c1', 'c2', 'c3', 'c23', 'c24'])] # Extract rows where 'column_id' is not in [1,2,3,23,24]
 
     cell_level, genes_per_well_df, wells_per_gene_df, dists = run_experiment(plate_map, settings['number_of_genes'], active_gene_list, settings['avg_genes_per_well'], settings['sd_genes_per_well'], settings['avg_cells_per_well'], settings['sd_cells_per_well'], settings['well_ineq_coeff'], settings['gene_ineq_coeff'])
-    cell_scores = classifier(settings['positive_mean'], settings['positive_variance'], settings['negative_mean'], settings['negative_variance'], df=cell_level)
+    cell_scores = classifier(settings['positive_mean'], settings['positive_variance'], settings['negative_mean'], settings['negative_variance'], settings['classifier_accuracy'], df=cell_level)
     cell_roc_dict_df, cell_pr_dict_df, cell_scores, cell_cm = cell_level_roc_auc(cell_scores)
     well_score = generate_well_score(cell_scores)
     gene_fraction_map, metadata = sequence_plates(well_score, settings['number_of_genes'], settings['avg_reads_per_gene'], settings['sd_reads_per_gene'], sequencing_error=settings['sequencing_error'])
     x = gene_fraction_map
     y = np.log10(well_score['score']+1)
     x = sm.add_constant(x)
     #y = y.fillna(0)
@@ -716,15 +801,18 @@
     results_as_html = results_summary.tables[1].as_html()
     results_df = pd.read_html(results_as_html, header=0, index_col=0)[0]
     results_df = results_df.rename_axis("gene").reset_index()
     results_df = results_df.iloc[1: , :]
     results_df, reg_roc_dict_df, reg_pr_dict_df, reg_cm, sim_stats = regression_roc_auc(results_df, active_gene_list, control_gene_list, alpha = 0.05, optimal=False)
     #except Exception as e:
     #    print(f"An error occurred while saving data: {e}")
-    return [cell_scores, cell_roc_dict_df, cell_pr_dict_df, cell_cm, well_score, gene_fraction_map, metadata, results_df, reg_roc_dict_df, reg_pr_dict_df, reg_cm, sim_stats, genes_per_well_df, wells_per_gene_df], dists
+    output = [cell_scores, cell_roc_dict_df, cell_pr_dict_df, cell_cm, well_score, gene_fraction_map, metadata, results_df, reg_roc_dict_df, reg_pr_dict_df, reg_cm, sim_stats, genes_per_well_df, wells_per_gene_df]
+    del cell_scores, cell_roc_dict_df, cell_pr_dict_df, cell_cm, well_score, gene_fraction_map, metadata, results_df, reg_roc_dict_df, reg_pr_dict_df, reg_cm, sim_stats, genes_per_well_df, wells_per_gene_df
+    gc.collect()
+    return output, dists
 
 def vis_dists(dists, src, v, i):
     """
     Visualizes the distributions of given distances.
 
     Args:
         dists (list): List of distance arrays.
@@ -740,17 +828,22 @@
     n=0
     width_graphs = height_graphs*n_graphs
     fig2, ax =plt.subplots(1,n_graphs, figsize = (width_graphs,height_graphs))
     names = ['genes/well', 'wells/gene', 'genes/well gini', 'wells/gene gini', 'gene_weights', 'well_weights']
     for index, dist in enumerate(dists):
         temp = pd.DataFrame(dist, columns = [f'{names[index]}'])
         sns.histplot(data=temp, x=f'{names[index]}', kde=False, binwidth=None, stat='count', element="step", ax=ax[n], color='teal', log_scale=False)
-        #plot_histogram(temp, f'{names[index]}', ax[n], 'slategray', f'{names[index]}', binwidth=None, log=False)
         n+=1
     save_plot(fig2, src, 'dists', i)
+    plt.close(fig2)
+    plt.figure().clear() 
+    plt.cla() 
+    plt.clf()
+    del dists
+
     return
 
 def visualize_all(output):
     """
     Visualizes various plots based on the given output data.
 
     Args:
@@ -769,14 +862,15 @@
             - sim_stats (dict): Dictionary containing simulation statistics.
             - genes_per_well_df (DataFrame): DataFrame containing genes per well data.
             - wells_per_gene_df (DataFrame): DataFrame containing wells per gene data.
 
     Returns:
         fig (matplotlib.figure.Figure): The generated figure object.
     """
+
     cell_scores = output[0]
     cell_roc_dict_df = output[1]
     cell_pr_dict_df = output[2]
     cell_cm = output[3]
     well_score = output[4]
     gene_fraction_map = output[5]
     metadata = output[6]
@@ -806,32 +900,43 @@
     plot_histogram(wells_per_gene_df, "wells_per_gene", ax[n], 'slategray', f'well/gene (Gini = {gini_wells_per_gene:.2f})', binwidth=None, log=False)
     #ax[n].set_xscale('log')
     n+=1
     
     #plot cell classification score by inactive and active
     active_distribution = cell_scores[cell_scores['is_active'] == 1] 
     inactive_distribution = cell_scores[cell_scores['is_active'] == 0]
-    plot_histogram(active_distribution, "score", ax[n], 'slategray', 'Cell scores', binwidth=0.01, log=False)
-    plot_histogram(inactive_distribution, "score", ax[n], 'teal', 'Cell scores', binwidth=0.01, log=False)
+    plot_histogram(active_distribution, "score", ax[n], 'slategray', 'Cell scores', log=False)#, binwidth=0.01, log=False)
+    plot_histogram(inactive_distribution, "score", ax[n], 'teal', 'Cell scores', log=False)#, binwidth=0.01, log=False)
+
+    legend_elements = [Patch(facecolor='slategray', edgecolor='slategray', label='Inactive'),
+                   Patch(facecolor='teal', edgecolor='teal', label='Active')]
+    
+    ax[n].legend(handles=legend_elements, loc='upper right')
+
+
     ax[n].set_xlim([0, 1])
     n+=1
     
     #plot classifier cell predictions by inactive and active well average
-    ##inactive_distribution_well['score'] = pd.to_numeric(inactive_distribution['score'], errors='coerce')
-    ##inactive_distribution_well = inactive_distribution_well.groupby('plate_row_column')['score'].mean()
-    
-    ##active_distribution_well['score'] = pd.to_numeric(active_distribution['score'], errors='coerce')
-    ##active_distribution_well = active_distribution_well.groupby('plate_row_column')['score'].mean()
+    inactive_distribution_well = inactive_distribution.groupby(['plate_id', 'row_id', 'column_id'])['score'].mean().reset_index(name='score')
+    active_distribution_well = active_distribution.groupby(['plate_id', 'row_id', 'column_id'])['score'].mean().reset_index(name='score')
+    mixed_distribution_well = cell_scores.groupby(['plate_id', 'row_id', 'column_id'])['score'].mean().reset_index(name='score')
+
+    plot_histogram(inactive_distribution_well, "score", ax[n], 'slategray', 'Well scores', log=False)#, binwidth=0.01, log=False)
+    plot_histogram(active_distribution_well, "score", ax[n], 'teal', 'Well scores', log=False)#, binwidth=0.01, log=False)
+    plot_histogram(mixed_distribution_well, "score", ax[n], 'red', 'Well scores', log=False)#, binwidth=0.01, log=False)
+    
+    legend_elements = [Patch(facecolor='slategray', edgecolor='slategray', label='Inactive'),
+                   Patch(facecolor='teal', edgecolor='teal', label='Active'),
+                   Patch(facecolor='red', edgecolor='red', label='Mixed')]
     
-    #inactive_distribution_well = inactive_distribution.groupby(['plate_row_column']).mean()
-    #active_distribution_well = active_distribution.groupby(['plate_row_column']).mean()
-    
-    plot_histogram(active_distribution, "score", ax[n], 'slategray', 'Well scores', binwidth=0.01, log=False)
-    plot_histogram(inactive_distribution, "score", ax[n], 'teal', 'Well scores', binwidth=0.01, log=False)
+    ax[n].legend(handles=legend_elements, loc='upper right')
+
     ax[n].set_xlim([0, 1])
+    #ax[n].legend()
     n+=1
     
     #plot ROC (cell classification)
     plot_roc_pr(cell_roc_dict_df, ax[n], 'ROC (Cell)', 'fpr', 'tpr')
     ax[n].plot([0, 1], [0, 1], color='black', lw=0.5, linestyle="--", label='random classifier')
     n+=1
     
@@ -842,16 +947,16 @@
     n+=1
     
     #Confusion matrix at optimal threshold
     plot_confusion_matrix(cell_cm, ax[n], 'Confusion Matrix Cell')
     n+=1
     
     #plot well score
-    plot_histogram(well_score, "score", ax[n], 'teal', 'Well score', binwidth=0.005, log=False)
-    ax[n].set_xlim([0, 1])
+    plot_histogram(well_score, "score", ax[n], 'teal', 'Well score', binwidth=0.005, log=True)
+    #ax[n].set_xlim([0, 1])
     n+=1
 
     control_df = results_df[results_df['color'] == 'control']
     control_mean = control_df['coef'].mean()
     control_var = control_df['coef'].std()
     #control_var = control_df['coef'].var()
     cutoff = abs(control_mean)+(3*control_var)
@@ -907,14 +1012,15 @@
 
     for n in [*range(0,n_graphs,1)]:
         ax[n].spines['top'].set_visible(False)
         ax[n].spines['right'].set_visible(False)
 
     plt.tight_layout()
     plt.show()
+    gc.collect()
     return fig
 
 def create_database(db_path):
     """
     Creates a SQLite database at the specified path.
 
     Args:
@@ -988,25 +1094,30 @@
             df_concat = pd.concat(filtered_output, axis=1)
             df_concat['genes_per_well_gini'] = gini_genes_per_well
             df_concat['wells_per_gene_gini'] = gini_wells_per_gene
             df_concat['date'] = datetime.now()
             df_concat[f'variable_{variable}_sim_nr'] = i
 
             append_database(src, df_concat, 'simulations')
+            del gini_genes_per_well, gini_wells_per_gene, df_concat
 
         if save_all:
             for i, df in enumerate(output):
                 df = output[i]
                 if table_names[i] == 'well_score':
                     df['gene_list'] = df['gene_list'].astype(str)
                 if not isinstance(df, pd.DataFrame):
                     df = pd.DataFrame(df)
                 append_database(src, df, table_names[i])
+            del df
     except Exception as e:
         print(f"An error occurred while saving data: {e}")
+        print(traceback.format_exc())
+    
+    del output, settings_df
     return
 
 def save_plot(fig, src, variable, i):
     """
     Save a matplotlib figure as a PDF file.
 
     Parameters:
@@ -1021,174 +1132,610 @@
     os.makedirs(f'{src}/{variable}', exist_ok=True)
     filename_fig = f'{src}/{variable}/{str(i)}_figure.pdf'
     fig.savefig(filename_fig, dpi=600, format='pdf', bbox_inches='tight')
     return
     
 def run_and_save(i, settings, time_ls, total_sims):
     
-
     """
     Run the simulation and save the results.
 
     Args:
         i (int): The simulation index.
         settings (dict): The simulation settings.
         time_ls (list): The list to store simulation times.
         total_sims (int): The total number of simulations.
 
     Returns:
         tuple: A tuple containing the simulation index, simulation time, and None.
     """
     #print(f'Runnings simulation with the following paramiters')
     #print(settings)
-    
+    settings['random_seed'] = False
     if settings['random_seed']:
         random.seed(42) # sims will be too similar with random seed
     src = settings['src']
     plot = settings['plot']
     v = settings['variable']
     start_time = time()  # Start time of the simulation
-    now = datetime.now() # get current date
-    date_string = now.strftime("%y%m%d") # format as a string in 'ddmmyy' format        
+    #now = datetime.now() # get current date
+    #date_string = now.strftime("%y%m%d") # format as a string in 'ddmmyy' format        
+    date_string = settings['start_time']
     #try:
     output, dists = run_simulation(settings)
     sim_time = time() - start_time  # Elapsed time for the simulation
     settings['sim_time'] = sim_time
     src = os.path.join(f'{src}/{date_string}',settings['name'])
     save_data(src, output, settings, save_all=False, i=i, variable=v)
-    if vis_dists:
-        vis_dists(dists,src, v, i)
     if plot:
+        vis_dists(dists,src, v, i)
         fig = visualize_all(output)
         save_plot(fig, src, v, i)
         plt.close(fig)
         plt.figure().clear() 
         plt.cla() 
         plt.clf()
         del fig
     del output, dists
+    gc.collect()
     #except Exception as e:
     #    print(e, end='\r', flush=True)
     #    sim_time = time() - start_time
         #print(traceback.format_exc(), end='\r', flush=True)
     time_ls.append(sim_time)
     return i, sim_time, None
     
-def generate_paramiters(settings):
+def validate_and_adjust_beta_params(sim_params):
     """
-    Generate a list of parameter sets for simulation based on the given settings.
-
+    Validates and adjusts Beta distribution parameters in simulation settings to ensure they are possible.
+    
     Args:
-        settings (dict): A dictionary containing the simulation settings.
-
+    sim_params (list of dict): List of dictionaries, each containing the simulation parameters.
+    
     Returns:
-        list: A list of parameter sets for simulation.
+    list of dict: The adjusted list of simulation parameter sets.
     """
-    sim_ls = []
-    for avg_genes_per_well in settings['avg_genes_per_well']:
-        replicates = settings['replicates']
-        sett = settings.copy()
-        sett['avg_genes_per_well'] = avg_genes_per_well
-        sett['sd_genes_per_well'] = int(avg_genes_per_well / 2)
-        for avg_cells_per_well in settings['avg_cells_per_well']:
-            sett['avg_cells_per_well'] = avg_cells_per_well
-            sett['sd_cells_per_well'] = int(avg_cells_per_well / 2)
-            for positive_mean in settings['positive_mean']:
-                sett['positive_mean'] = positive_mean
-                sett['negative_mean'] = 1-positive_mean
-                sett['positive_variance'] = (1-positive_mean)/2
-                sett['negative_variance'] = (1-positive_mean)/2
-                for avg_reads_per_gene in settings['avg_reads_per_gene']:
-                    sett['avg_reads_per_gene'] = int(avg_reads_per_gene)
-                    sett['sd_reads_per_gene'] = int(avg_reads_per_gene/2)
-                    for sequencing_error in settings['sequencing_error']:
-                        sett['sequencing_error'] = sequencing_error
-                        for well_ineq_coeff in settings['well_ineq_coeff']:
-                            sett['well_ineq_coeff'] = well_ineq_coeff
-                            for gene_ineq_coeff in settings['gene_ineq_coeff']:
-                                sett['gene_ineq_coeff'] = gene_ineq_coeff
-                                for nr_plates in settings['nr_plates']:
-                                    sett['nr_plates'] = nr_plates
-                                    for number_of_genes in settings['number_of_genes']:
-                                        sett['number_of_genes'] = number_of_genes
-                                        for number_of_active_genes in settings['number_of_active_genes']:
-                                            sett['number_of_active_genes'] = number_of_active_genes
-                                            for i in [*range(1,replicates+1)]:
-                                                sim_ls.append(sett)
-                                                #print(sett)
-    #print('Number of simulations:',len(sim_ls))
-    return sim_ls
+    adjusted_params = []
+    for params in sim_params:
+        max_pos_variance = params['positive_mean'] * (1 - params['positive_mean'])
+        max_neg_variance = params['negative_mean'] * (1 - params['negative_mean'])
+
+        # Adjust positive variance
+        if params['positive_variance'] >= max_pos_variance:
+            print(f'changed positive variance from {params["positive_variance"]} to {max_pos_variance * 0.99}')
+            params['positive_variance'] = max_pos_variance * 0.99  # Adjust to 99% of the maximum allowed variance
+
+        # Adjust negative variance
+        if params['negative_variance'] >= max_neg_variance:
+            print(f'changed negative variance from {params["negative_variance"]} to {max_neg_variance * 0.99}')
+            params['negative_variance'] = max_neg_variance * 0.99  # Adjust to 99% of the maximum allowed variance
+
+        adjusted_params.append(params)
+        
+    return adjusted_params
+
+def generate_paramiters(settings):
 
-#altered for one set of settings see negative_mean and variance
-def generate_paramiters_single(settings):
     """
-    Generate a list of parameter sets for single simulations based on the given settings.
+    Generate a list of parameter sets for simulation based on the given settings.
 
     Args:
         settings (dict): A dictionary containing the simulation settings.
 
     Returns:
-        list: A list of parameter sets for single simulations.
+        list: A list of parameter sets for simulation.
     """
+    
+    settings['positive_mean'] = [0.8]
+
     sim_ls = []
     for avg_genes_per_well in settings['avg_genes_per_well']:
         replicates = settings['replicates']
-        sett = settings.copy()
-        sett['avg_genes_per_well'] = avg_genes_per_well
-        sett['sd_genes_per_well'] = int(avg_genes_per_well / 2)
         for avg_cells_per_well in settings['avg_cells_per_well']:
-            sett['avg_cells_per_well'] = avg_cells_per_well
-            sett['sd_cells_per_well'] = int(avg_cells_per_well / 2)
-            for positive_mean in settings['positive_mean']:
-                sett['positive_mean'] = positive_mean
-                sett['negative_mean'] = 0.2
-                sett['positive_variance'] = 0.13
-                sett['negative_variance'] = 0.13
-                for avg_reads_per_gene in settings['avg_reads_per_gene']:
-                    sett['avg_reads_per_gene'] = int(avg_reads_per_gene)
-                    sett['sd_reads_per_gene'] = int(avg_reads_per_gene/2)
-                    for sequencing_error in settings['sequencing_error']:
-                        sett['sequencing_error'] = sequencing_error
-                        for well_ineq_coeff in settings['well_ineq_coeff']:
-                            sett['well_ineq_coeff'] = well_ineq_coeff
-                            for gene_ineq_coeff in settings['gene_ineq_coeff']:
-                                sett['gene_ineq_coeff'] = gene_ineq_coeff
-                                for nr_plates in settings['nr_plates']:
-                                    sett['nr_plates'] = nr_plates
-                                    for number_of_genes in settings['number_of_genes']:
-                                        sett['number_of_genes'] = number_of_genes
-                                        for number_of_active_genes in settings['number_of_active_genes']:
-                                            sett['number_of_active_genes'] = number_of_active_genes
-                                            for i in [*range(1,replicates+1)]:
-                                                sim_ls.append(sett)
-                                                #print(sett)
-    #print('Number of simulations:',len(sim_ls))
+            for classifier_accuracy in settings['classifier_accuracy']:
+                for positive_mean in settings['positive_mean']:
+                    for avg_reads_per_gene in settings['avg_reads_per_gene']:
+                        for sequencing_error in settings['sequencing_error']:
+                            for well_ineq_coeff in settings['well_ineq_coeff']:
+                                for gene_ineq_coeff in settings['gene_ineq_coeff']:
+                                    for nr_plates in settings['nr_plates']:
+                                        for number_of_genes in settings['number_of_genes']:
+                                            for number_of_active_genes in settings['number_of_active_genes']:
+                                                for i in range(1, replicates+1):
+                                                    sett = deepcopy(settings)
+                                                    sett['avg_genes_per_well'] = avg_genes_per_well
+                                                    sett['sd_genes_per_well'] = avg_genes_per_well / 2
+                                                    sett['avg_cells_per_well'] = avg_cells_per_well
+                                                    sett['sd_cells_per_well'] = avg_cells_per_well / 2
+                                                    sett['classifier_accuracy'] = classifier_accuracy
+                                                    sett['positive_mean'] = positive_mean
+                                                    sett['negative_mean'] = 1-positive_mean
+                                                    sett['positive_variance'] = (1-positive_mean)/2
+                                                    sett['negative_variance'] = (1-positive_mean)/2
+                                                    sett['avg_reads_per_gene'] = avg_reads_per_gene
+                                                    sett['sd_reads_per_gene'] = avg_reads_per_gene / 2
+                                                    sett['sequencing_error'] = sequencing_error
+                                                    sett['well_ineq_coeff'] = well_ineq_coeff
+                                                    sett['gene_ineq_coeff'] = gene_ineq_coeff
+                                                    sett['nr_plates'] = nr_plates
+                                                    sett['number_of_genes'] = number_of_genes
+                                                    sett['number_of_active_genes'] = number_of_active_genes
+                                                    sim_ls.append(sett)
+
+    random.shuffle(sim_ls)
+    sim_ls = validate_and_adjust_beta_params(sim_ls)
+    print(f'Running {len(sim_ls)} simulations.')
+    #for x in sim_ls: 
+    #    print(x['positive_mean'])
     return sim_ls
 
 def run_multiple_simulations(settings):
+
     """
     Run multiple simulations in parallel using the provided settings.
 
     Args:
         settings (dict): A dictionary containing the simulation settings.
 
     Returns:
         None
     """
 
+    now = datetime.now() # get current date
+    start_time = now.strftime("%y%m%d") # format as a string in 'ddmmyy' format 
+    settings['start_time'] = start_time
+
     sim_ls = generate_paramiters(settings)
-    print(f'Running {len(sim_ls)} simulations. Standard deviations for each variable are variable / 2')
+    #print(f'Running {len(sim_ls)} simulations.')
 
     max_workers = settings['max_workers'] or cpu_count() - 4
     with Manager() as manager:
         time_ls = manager.list()
         total_sims = len(sim_ls)
         with Pool(max_workers) as pool:
             result = pool.starmap_async(run_and_save, [(index, settings, time_ls, total_sims) for index, settings in enumerate(sim_ls)])
             while not result.ready():
-                sleep(0.01)
-                sims_processed = len(time_ls)
-                average_time = np.mean(time_ls) if len(time_ls) > 0 else 0
-                time_left = (((total_sims - sims_processed) * average_time) / max_workers) / 60
-                print(f'Progress: {sims_processed}/{total_sims} Time/simulation {average_time:.3f}sec Time Remaining {time_left:.3f} min.', end='\r', flush=True)
-            result.get()
+                try:
+                    sleep(0.01)
+                    sims_processed = len(time_ls)
+                    average_time = np.mean(time_ls) if len(time_ls) > 0 else 0
+                    time_left = (((total_sims - sims_processed) * average_time) / max_workers) / 60
+                    print(f'Progress: {sims_processed}/{total_sims} Time/simulation {average_time:.3f}sec Time Remaining {time_left:.3f} min.', end='\r', flush=True)
+                    gc.collect()
+                except Exception as e:
+                    print(e)
+                    print(traceback.format_exc())
+            try:
+                result.get()
+            except Exception as e:
+                print(e)
+                print(traceback.format_exc())
             
+def generate_integers(start, stop, step):
+    return list(range(start, stop + 1, step))
+
+def generate_floats(start, stop, step):
+    # Determine the number of decimal places in 'step'
+    num_decimals = str(step)[::-1].find('.')
+    
+    current = start
+    floats_list = []
+    while current <= stop:
+        # Round each float to the appropriate number of decimal places
+        floats_list.append(round(current, num_decimals))
+        current += step
+    
+    return floats_list
+
+def remove_columns_with_single_value_v1(df):
+    """
+    Removes columns from the DataFrame that have the same value in all rows.
+
+    Args:
+    df (pandas.DataFrame): The original DataFrame.
+
+    Returns:
+    pandas.DataFrame: A DataFrame with the columns removed that contained only one unique value.
+    """
+    
+    df=df.copy()
+    
+    for column in df.columns:
+        if len(df[column].unique()) == 1:
+            df.drop(column, axis=1, inplace=True)
+    
+    return df
+
+def remove_columns_with_single_value(df):
+    """
+    Removes columns from the DataFrame that have the same value in all rows.
+
+    Args:
+    df (pandas.DataFrame): The original DataFrame.
+
+    Returns:
+    pandas.DataFrame: A DataFrame with the columns removed that contained only one unique value.
+    """
+    to_drop = [column for column in df.columns if df[column].nunique() == 1]
+    return df.drop(to_drop, axis=1)
+
+def read_simulations_table(db_path):
+    """
+    Reads the 'simulations' table from an SQLite database into a pandas DataFrame.
+    
+    Args:
+    db_path (str): The file path to the SQLite database.
+    
+    Returns:
+    pandas.DataFrame: DataFrame containing the 'simulations' table data.
+    """
+    # Create a connection object using the connect function
+    conn = sqlite3.connect(db_path)
+    
+    # Read the 'simulations' table into a pandas DataFrame
+    try:
+        df = pd.read_sql_query("SELECT * FROM simulations", conn)
+    except Exception as e:
+        print(f"An error occurred: {e}")
+        return None
+    finally:
+        # Close the connection to SQLite database
+        conn.close()
+    
+    return df
+
+def plot_simulations(df, variable, x_rotation=None, legend=False, grid=False, clean=True, verbose=False):
+    
+    """
+    Creates separate line plots for 'prauc' against a specified 'variable', 
+    for each unique combination of conditions defined by 'grouping_vars', displayed on a grid.
+
+    Args:
+    df (pandas.DataFrame): DataFrame containing the necessary columns.
+    variable (str): Name of the column to use as the x-axis for grouping and plotting.
+    x_rotation (int, optional): Degrees to rotate the x-axis labels.
+    legend (bool, optional): Whether to display a legend.
+    grid (bool, optional): Whether to display grid lines.
+    verbose (bool, optional): Whether to print the filter conditions.
+
+    Returns:
+    None
+    """
+    
+    grouping_vars = ['number_of_active_genes', 'number_of_control_genes', 'avg_reads_per_gene',
+                     'classifier_accuracy', 'nr_plates', 'number_of_genes', 'avg_genes_per_well',
+                     'avg_cells_per_well', 'sequencing_error', 'well_ineq_coeff', 'gene_ineq_coeff']
+    
+    if clean:
+        relevant_data = remove_columns_with_single_value(relevant_data)
+    
+    grouping_vars = [col for col in grouping_vars if col != variable]
+    
+    # Check if the necessary columns are present in the DataFrame
+    required_columns = {variable, 'prauc'} | set(grouping_vars)
+    if not required_columns.issubset(df.columns):
+        missing_cols = required_columns - set(df.columns)
+        raise ValueError(f"DataFrame must contain {missing_cols} columns")
+        
+    #if not dependent is None:
+    
+    # Get unique combinations of conditions from grouping_vars
+    unique_combinations = df[grouping_vars].drop_duplicates()
+    num_combinations = len(unique_combinations)
+
+    # Determine the layout of the subplots
+    num_rows = math.ceil(np.sqrt(num_combinations))
+    num_cols = math.ceil(num_combinations / num_rows)
+
+    fig, axes = plt.subplots(num_rows, num_cols, figsize=(5 * num_cols, 5 * num_rows))
+    if num_rows * num_cols > 1:
+        axes = axes.flatten()
+    else:
+        axes = [axes]
+
+    for idx, (ax, (_, row)) in enumerate(zip(axes, unique_combinations.iterrows())):
+
+        # Filter the DataFrame for the current combination of variables
+        condition = {var: row[var] for var in grouping_vars}
+        subset_df = df[df[grouping_vars].eq(row).all(axis=1)]
+        
+        # Group by 'variable' and calculate mean and std dev of 'prauc'
+        grouped = subset_df.groupby(variable)['prauc'].agg(['mean', 'std'])
+        grouped = grouped.sort_index()  # Sort by the variable for orderly plots
+
+        # Plotting the mean of 'prauc' with std deviation as shaded area
+        ax.plot(grouped.index, grouped['mean'], marker='o', linestyle='-', color='b', label='Mean PRAUC')
+        ax.fill_between(grouped.index, grouped['mean'] - grouped['std'], grouped['mean'] + grouped['std'], color='gray', alpha=0.5, label='Std Dev')
+
+        # Setting plot labels and title
+        title_details = ', '.join([f"{var}={row[var]}" for var in grouping_vars])
+        ax.set_xlabel(variable)
+        ax.set_ylabel('Precision-Recall AUC (PRAUC)')
+        #ax.set_title(f'PRAUC vs. {variable} | {title_details}')
+        ax.grid(grid)
+
+        if legend:
+            ax.legend()
+
+        # Set x-ticks and rotate them as specified
+        ax.set_xticks(grouped.index)
+        ax.set_xticklabels(grouped.index, rotation=x_rotation if x_rotation is not None else 45)
+        
+        if verbose:
+            verbose_text = '\n'.join([f"{var}: {val}" for var, val in condition.items()])
+            ax.text(0.95, 0.05, verbose_text, transform=ax.transAxes, fontsize=9, verticalalignment='bottom', horizontalalignment='right', bbox=dict(boxstyle='round', facecolor='white', alpha=0.5))
+    
+    # Hide any unused axes if there are any
+    for ax in axes[idx+1:]:
+        ax.set_visible(False)
+
+    plt.tight_layout()
+    plt.show()
+    return fig
+    
+def plot_correlation_matrix(df, annot=False, cmap='inferno', clean=True):
+    """
+    Plots a correlation matrix for the specified variables and the target variable.
+
+    Args:
+    df (pandas.DataFrame): The DataFrame containing the data.
+    variables (list): List of column names to include in the correlation matrix.
+    target_variable (str): The target variable column name.
+
+    Returns:
+    None
+    """
+    cmap = sns.diverging_palette(240, 10, as_cmap=True)
+    grouping_vars = ['number_of_active_genes', 'number_of_control_genes', 'avg_reads_per_gene',
+                     'classifier_accuracy', 'nr_plates', 'number_of_genes', 'avg_genes_per_well',
+                     'avg_cells_per_well', 'sequencing_error', 'well_ineq_coeff', 'gene_ineq_coeff']
+    
+    grouping_vars = grouping_vars + ['optimal_threshold', 'accuracy', 'prauc', 'roc_auc','genes_per_well_gini', 'wells_per_gene_gini']
+    # 'inactive_mean', 'inactive_std', 'inactive_var', 'active_mean', 'active_std', 'inactive_var', 'cutoff', 'TP', 'FP', 'TN', 'FN', 
+
+    if clean:
+        df = remove_constant_columns(df)
+        grouping_vars = [feature for feature in grouping_vars if feature in df.columns]
+
+    # Subsetting the DataFrame to include only the relevant variables
+    relevant_data = df[grouping_vars]
+    
+    if clean:
+        relevant_data = remove_columns_with_single_value(relevant_data)
+        
+    # Calculating the correlation matrix
+    corr_matrix = relevant_data.corr()
+    mask = np.triu(np.ones_like(corr_matrix, dtype=bool))
+    
+    # Plotting the correlation matrix
+    fig = plt.figure(figsize=(12, 8))
+    sns.heatmap(corr_matrix, mask=mask, annot=annot, cmap=cmap, fmt=".2f", linewidths=.5, robust=True)
+    #plt.title('Correlation Matrix with Heatmap')
+
+    plt.tight_layout()
+    plt.show()
+    save_plot(fig, src='figures', variable='correlation_matrix', i=1)
+    return fig
+
+def plot_feature_importance(df, target='prauc', exclude=None, clean=True):
+    """
+    Trains a RandomForestRegressor to determine the importance of each feature in predicting the target.
+
+    Args:
+    df (pandas.DataFrame): The DataFrame containing the data.
+    target (str): The target variable column name.
+    exclude (list or str, optional): Column names to exclude from features.
+
+    Returns:
+    matplotlib.figure.Figure: The figure object containing the feature importance plot.
+    """
+    
+    # Define the features for the model
+    features = ['number_of_active_genes', 'number_of_control_genes', 'avg_reads_per_gene',
+                     'classifier_accuracy', 'nr_plates', 'number_of_genes', 'avg_genes_per_well',
+                     'avg_cells_per_well', 'sequencing_error', 'well_ineq_coeff', 'gene_ineq_coeff']
+    
+    if clean:
+        df = remove_columns_with_single_value(df)
+        features = [feature for feature in features if feature in df.columns]
+    
+    # Remove excluded features if specified
+    if isinstance(exclude, list):
+        features = [feature for feature in features if feature not in exclude]
+    elif exclude is not None:
+        features = [feature for feature in features if feature != exclude]
+    
+    # Train the model
+    model = RandomForestRegressor(n_estimators=1000, random_state=42)
+    model.fit(df[features], df[target])
+    
+    # Get feature importances
+    importances = model.feature_importances_
+    indices = np.argsort(importances)[::-1]
+    
+    # Plot horizontal bar chart
+    fig = plt.figure(figsize=(12, 6))
+    plt.barh(range(len(indices)), importances[indices], color="teal", align="center", alpha=0.6)
+    plt.yticks(range(len(indices)), [features[i] for i in indices[::-1]])  # Invert y-axis to match the order
+    plt.gca().invert_yaxis()  # Invert the axis to have the highest importance at the top
+    plt.xlabel('Feature Importance')
+    plt.title('Feature Importances')
+    plt.tight_layout()
+    plt.show()
+    save_plot(fig, src='figures', variable='feature_importance', i=1)
+    return fig
+
+def calculate_permutation_importance(df, target='prauc', exclude=None, n_repeats=10, clean=True):
+    """
+    Calculates permutation importance for the given features in the dataframe.
+
+    Args:
+    df (pandas.DataFrame): The DataFrame containing the data.
+    features (list): List of column names to include as features.
+    target (str): The name of the target variable column.
+
+    Returns:
+    dict: Dictionary containing the importances and standard deviations.
+    """
+    
+    features = ['number_of_active_genes', 'number_of_control_genes', 'avg_reads_per_gene',
+                'classifier_accuracy', 'nr_plates', 'number_of_genes', 'avg_genes_per_well',
+                'avg_cells_per_well', 'sequencing_error', 'well_ineq_coeff', 'gene_ineq_coeff']
+    
+    if clean:
+        df = remove_columns_with_single_value(df)
+        features = [feature for feature in features if feature in df.columns]
+    
+    if isinstance(exclude, list):
+        for ex in exclude:
+            features.remove(ex)
+    if not exclude is None:
+        features.remove(exclude)
+    
+    X = df[features]
+    y = df[target]
+
+    # Initialize a model (you could pass it as an argument if you'd like to use a different one)
+    model = RandomForestRegressor(n_estimators=100, random_state=42)
+    model.fit(X, y)
+
+    perm_importance = permutation_importance(model, X, y, n_repeats=n_repeats, random_state=42)
+
+    # Plotting
+    sorted_idx = perm_importance.importances_mean.argsort()
+    
+    # Create a figure and a set of subplots
+    fig, ax = plt.subplots()
+    ax.barh(range(len(sorted_idx)), perm_importance.importances_mean[sorted_idx], color="teal", align="center", alpha=0.6)
+    ax.set_yticks(range(len(sorted_idx)))
+    ax.set_yticklabels([df.columns[i] for i in sorted_idx])
+    ax.set_xlabel('Permutation Importance')
+    plt.tight_layout()
+    plt.show()
+    save_plot(fig, src='figures', variable='permutation_importance', i=1)
+    return fig
+    
+def plot_partial_dependences(df, target='prauc', clean=True):
+    
+    """
+    Creates partial dependence plots for the specified features, with improved layout to avoid text overlap.
+
+    Args:
+    df (pandas.DataFrame): The DataFrame containing the data.
+    target (str): The target variable.
+
+    Returns:
+    None
+    """
+    
+    features = ['number_of_active_genes', 'number_of_control_genes', 'avg_reads_per_gene',
+                'classifier_accuracy', 'nr_plates', 'number_of_genes', 'avg_genes_per_well',
+                'avg_cells_per_well', 'sequencing_error', 'well_ineq_coeff', 'gene_ineq_coeff']
+    
+    if clean:
+        df = remove_columns_with_single_value(df)
+        features = [feature for feature in features if feature in df.columns]
+
+    X = df[features]
+    y = df[target]
+    
+    # Train a model
+    model = GradientBoostingRegressor()
+    model.fit(X, y)
+    
+    # Determine the number of rows and columns for subplots
+    n_cols = 4  # Number of columns in subplot grid
+    n_rows = (len(features) + n_cols - 1) // n_cols  # Calculate rows needed
+    
+    # Plot partial dependence
+    fig, axs = plt.subplots(nrows=n_rows, ncols=n_cols, figsize=(5 * n_cols, 5 * n_rows))
+    fig.suptitle('Partial Dependence Plots', fontsize=20, y=1.03)
+    
+    # Flatten the array of axes if it's multidimensional
+    axs = axs.flatten() if n_rows > 1 else [axs]
+    
+    for i, feature in enumerate(features):
+        ax = axs[i]
+        disp = PartialDependenceDisplay.from_estimator(model, X, features=[feature], ax=ax)
+        ax.set_title(feature)  # Set title to the name of the feature
+
+    # Hide unused axes if any
+    for ax in axs[len(features):]:
+        ax.set_visible(False)
+    
+    plt.tight_layout()
+    plt.show()
+    save_plot(fig, src='figures', variable='partial_dependences', i=1)
+    return fig
+
+def save_shap_plot(fig, src, variable, i):
+    import os
+    os.makedirs(f'{src}/{variable}', exist_ok=True)
+    filename_fig = f'{src}/{variable}/{str(i)}_figure.pdf'
+    fig.savefig(filename_fig, dpi=600, format='pdf', bbox_inches='tight')
+    print(f"Saved figure as {filename_fig}")
+
+def generate_shap_summary_plot(df,target='prauc', clean=True):
+    """
+    Generates a SHAP summary plot for the given features in the dataframe.
+
+    Args:
+    df (pandas.DataFrame): The DataFrame containing the data.
+    features (list): List of column names to include as features.
+    target (str): The name of the target variable column.
+
+    Returns:
+    None
+    """
+    
+    features = ['number_of_active_genes', 'number_of_control_genes', 'avg_reads_per_gene',
+                'classifier_accuracy', 'nr_plates', 'number_of_genes', 'avg_genes_per_well',
+                'avg_cells_per_well', 'sequencing_error', 'well_ineq_coeff', 'gene_ineq_coeff']
+    
+    if clean:
+        df = remove_columns_with_single_value(df)
+        features = [feature for feature in features if feature in df.columns]
+
+    X = df[features]
+    y = df[target]
+
+    # Initialize a model (you could pass it as an argument if you'd like to use a different one)
+    model = RandomForestRegressor(n_estimators=100, random_state=42)
+    model.fit(X, y)
+
+    # Calculate SHAP values
+    explainer = shap.TreeExplainer(model)
+    shap_values = explainer.shap_values(X)
+
+    # Summary plot
+    shap.summary_plot(shap_values, X)
+    save_shap_plot(plt.gcf(), src='figures', variable='shap', i=1)
+    #save_shap_plot(fig, src, variable, i)
+    return plt.gcf()
+
+
+def remove_constant_columns(df):
+    """
+    Removes columns in the DataFrame where all entries have the same value.
+
+    Parameters:
+    df (pd.DataFrame): The input DataFrame from which to remove constant columns.
+
+    Returns:
+    pd.DataFrame: A DataFrame with the constant columns removed.
+    """
+    return df.loc[:, df.nunique() > 1]
+
+
+# to justify using beta for sim classifier
+
+# Fit a Beta distribution to these outputs
+#a, b, loc, scale = beta.fit(predicted_probs, floc=0, fscale=1)  # Fix location and scale to match the support of the sigmoid
+
+# Sample from this fitted Beta distribution
+#simulated_probs = beta.rvs(a, b, size=1000)
+
+# Plot the empirical vs simulated distribution
+#plt.hist(predicted_probs, bins=30, alpha=0.5, label='Empirical')
+#plt.hist(simulated_probs, bins=30, alpha=0.5, label='Simulated from Beta')
+#plt.legend()
+#plt.show()
```

### Comparing `spacr-0.0.20/spacr/timelapse.py` & `spacr-0.0.21/spacr/timelapse.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from IPython.display import display
 from IPython.display import Image as ipyimage
 import trackpy as tp
 from btrack import datasets as btrack_datasets
 from skimage.measure import regionprops
 from scipy.signal import find_peaks
 from scipy.optimize import curve_fit
+from scipy.integrate import trapz
 import matplotlib.pyplot as plt
 
 from .logger import log_function_call
 
 #from .plot import _visualize_and_save_timelapse_stack_with_tracks
 #from .utils import _masks_to_masks_stack
 
@@ -586,14 +587,88 @@
         all_timepoints = sorted(result_df['time'].unique())
         ax.set_xticks(all_timepoints)
         ax.set_xticklabels(all_timepoints, rotation=45, ha="right")
 
     plt.tight_layout()
     plt.show()
 
+def save_figure(fig, src, figure_number):
+    source = os.path.dirname(src)
+    results_fldr = os.path.join(source,'results')
+    os.makedirs(results_fldr, exist_ok=True)
+    fig_loc = os.path.join(results_fldr, f'figure_{figure_number}.pdf')
+    fig.savefig(fig_loc)
+    print(f'Saved figure:{fig_loc}')
+
+def save_results_dataframe(df, src, results_name):
+    source = os.path.dirname(src)
+    results_fldr = os.path.join(source,'results')
+    os.makedirs(results_fldr, exist_ok=True)
+    csv_loc = os.path.join(results_fldr, f'{results_name}.csv')
+    df.to_csv(csv_loc, index=True)
+    print(f'Saved results:{csv_loc}')
+
+def summarize_per_well(peak_details_df):
+    # Step 1: Split the 'ID' column
+    split_columns = peak_details_df['ID'].str.split('_', expand=True)
+    peak_details_df[['plate', 'row', 'column', 'field', 'object_number']] = split_columns
+
+    # Step 2: Create 'well_ID' by combining 'row' and 'column'
+    peak_details_df['well_ID'] = peak_details_df['row'] + '_' + peak_details_df['column']
+
+    # Filter entries where 'amplitude' is not null
+    filtered_df = peak_details_df[peak_details_df['amplitude'].notna()]
+
+    # Preparation for Step 3: Identify numeric columns for averaging from the filtered dataframe
+    numeric_cols = filtered_df.select_dtypes(include=['number']).columns
+
+    # Step 3: Calculate summary statistics
+    summary_df = filtered_df.groupby('well_ID').agg(
+        peaks_per_well=('ID', 'size'),
+        unique_IDs_with_amplitude=('ID', 'nunique'),  # Count unique IDs per well with non-null amplitude
+        **{col: (col, 'mean') for col in numeric_cols}  # exclude 'amplitude' from averaging if it's numeric
+    ).reset_index()
+
+    # Step 3: Calculate summary statistics
+    summary_df_2 = peak_details_df.groupby('well_ID').agg(
+        cells_per_well=('object_number', 'nunique'),
+    ).reset_index()
+
+    summary_df['cells_per_well'] = summary_df_2['cells_per_well']
+    summary_df['peaks_per_cell'] = summary_df['peaks_per_well'] / summary_df['cells_per_well']
+    
+    return summary_df
+
+def summarize_per_well_inf_non_inf(peak_details_df):
+    # Step 1: Split the 'ID' column
+    split_columns = peak_details_df['ID'].str.split('_', expand=True)
+    peak_details_df[['plate', 'row', 'column', 'field', 'object_number']] = split_columns
+
+    # Step 2: Create 'well_ID' by combining 'row' and 'column'
+    peak_details_df['well_ID'] = peak_details_df['row'] + '_' + peak_details_df['column']
+
+    # Assume 'pathogen_count' indicates infection if > 0
+    # Add an 'infected_status' column to classify cells
+    peak_details_df['infected_status'] = peak_details_df['infected'].apply(lambda x: 'infected' if x > 0 else 'non_infected')
+
+    # Preparation for Step 3: Identify numeric columns for averaging
+    numeric_cols = peak_details_df.select_dtypes(include=['number']).columns
+
+    # Step 3: Calculate summary statistics
+    summary_df = peak_details_df.groupby(['well_ID', 'infected_status']).agg(
+        cells_per_well=('object_number', 'nunique'),
+        peaks_per_well=('ID', 'size'),
+        **{col: (col, 'mean') for col in numeric_cols}
+    ).reset_index()
+
+    # Calculate peaks per cell
+    summary_df['peaks_per_cell'] = summary_df['peaks_per_well'] / summary_df['cells_per_well']
+
+    return summary_df
+
 def analyze_calcium_oscillations(db_loc, measurement='cell_channel_1_mean_intensity', size_filter='cell_area', fluctuation_threshold=0.25, num_lines=None, peak_height=0.01, pathogen=None, cytoplasm=None, remove_transient=True, verbose=False, transience_threshold=0.9):
     # Load data
     conn = sqlite3.connect(db_loc)
     # Load cell table
     cell_df = pd.read_sql(f"SELECT * FROM {'cell'}", conn)
     
     if pathogen:
@@ -622,15 +697,15 @@
     cell_df['column'] = prcf_components[2]
     cell_df['field'] = prcf_components[3]
     cell_df['time'] = prcf_components[4].str.extract('t(\d+)').astype(int)
     cell_df['object_number'] = cell_df['object_label']
     cell_df['plate_row_column_field_object'] = cell_df['plate'].astype(str) + '_' + cell_df['row'].astype(str) + '_' + cell_df['column'].astype(str) + '_' + cell_df['field'].astype(str) + '_' + cell_df['object_label'].astype(str)
 
     df = cell_df.copy()
-    
+
     # Fit exponential decay model to all scaled fluorescence data
     try:
         params, _ = curve_fit(exponential_decay, df['time'], df[measurement], p0=[max(df[measurement]), 0.01, min(df[measurement])], maxfev=10000)
         df['corrected_' + measurement] = df[measurement] / exponential_decay(df['time'], *params)
     except RuntimeError as e:
         print(f"Curve fitting failed for the entire dataset with error: {e}")
         return
@@ -649,42 +724,86 @@
         if remove_transient:
 
             threshold = int(transience_threshold * total_timepoints)
 
             if verbose:
                 print(f'Group length: {len(group)} Timelapse length: {total_timepoints}, threshold:{threshold}')
 
-            if not len(group) <= threshold:
+            if len(group) <= threshold:
                 transience_removed += 1
+                if verbose:
+                    print(f'removed group {unique_id} due to transience')
                 continue
         
         size_diff = group[size_filter].std() / group[size_filter].mean()
+
         if size_diff <= fluctuation_threshold:
             group['delta_' + measurement] = group['corrected_' + measurement].diff().fillna(0)
             corrected_dfs.append(group)
             
             # Detect peaks
             peaks, properties = find_peaks(group['delta_' + measurement], height=peak_height)
 
+            # Set values < 0 to 0
+            group_filtered = group.copy()
+            group_filtered['delta_' + measurement] = group['delta_' + measurement].clip(lower=0)
+            above_zero_auc = trapz(y=group_filtered['delta_' + measurement], x=group_filtered['time'])
+            auc = trapz(y=group['delta_' + measurement], x=group_filtered['time'])
+            is_infected = (group['parasite_count'] > 0).any()
+            
+            if is_infected:
+                is_infected = 1
+            else:
+                is_infected = 0
+
+            if len(peaks) == 0:
+                peak_details_list.append({
+                    'ID': unique_id,
+                    'plate': group['plate'].iloc[0],
+                    'row': group['row'].iloc[0],
+                    'column': group['column'].iloc[0],
+                    'field': group['field'].iloc[0],
+                    'object_number': group['object_number'].iloc[0],
+                    'time': np.nan,  # The time of the peak
+                    'amplitude': np.nan,
+                    'delta': np.nan,
+                    'AUC': auc,
+                    'AUC_positive': above_zero_auc,
+                    'AUC_peak': np.nan,
+                    'infected': is_infected  
+                })
+
             # Inside the for loop where peaks are detected
             for i, peak in enumerate(peaks):
-                amplitude = properties['peak_heights'][i]  # Correctly access the amplitude
-                peak_time = group['time'].iloc[peak]  # Time corresponding to the peak
-                # Get the number of pathogens in the cell at the time of the peak
+
+                amplitude = properties['peak_heights'][i]
+                peak_time = group['time'].iloc[peak]
                 pathogen_count_at_peak = group['parasite_count'].iloc[peak]
+
+                start_idx = max(peak - 1, 0)
+                end_idx = min(peak + 1, len(group) - 1)
+
+                # Using indices to slice for AUC calculation
+                peak_segment_y = group['delta_' + measurement].iloc[start_idx:end_idx + 1]
+                peak_segment_x = group['time'].iloc[start_idx:end_idx + 1]
+                peak_auc = trapz(y=peak_segment_y, x=peak_segment_x)
+
                 peak_details_list.append({
                     'ID': unique_id,
                     'plate': group['plate'].iloc[0],
                     'row': group['row'].iloc[0],
                     'column': group['column'].iloc[0],
                     'field': group['field'].iloc[0],
                     'object_number': group['object_number'].iloc[0],
                     'time': peak_time,  # The time of the peak
                     'amplitude': amplitude,
                     'delta': group['delta_' + measurement].iloc[peak],
+                    'AUC': auc,
+                    'AUC_positive': above_zero_auc,
+                    'AUC_peak': peak_auc,
                     'infected': pathogen_count_at_peak  
                 })
         else:
             size_filter_removed += 1
 
     if verbose:
         print(f'Removed {size_filter_removed} objects due to size filter fluctuation')
@@ -693,15 +812,22 @@
     if len(corrected_dfs) > 0:
         result_df = pd.concat(corrected_dfs)
     else:
         print("No suitable cells found for analysis")
         return
     
     peak_details_df = pd.DataFrame(peak_details_list)
-    
+    summary_df = summarize_per_well(peak_details_df)
+    summary_df_inf_non_inf = summarize_per_well_inf_non_inf(peak_details_df)
+
+    save_results_dataframe(df=peak_details_df, src=db_loc, results_name='peak_details')
+    save_results_dataframe(df=result_df, src=db_loc, results_name='results')
+    save_results_dataframe(df=summary_df, src=db_loc, results_name='well_results')
+    save_results_dataframe(df=summary_df_inf_non_inf, src=db_loc, results_name='well_results_inf_non_inf')
+
     # Plotting
     fig, ax = plt.subplots(figsize=(10, 8))
     sampled_groups = result_df['plate_row_column_field_object'].unique()
     if num_lines is not None and 0 < num_lines < len(sampled_groups):
         sampled_groups = np.random.choice(sampled_groups, size=num_lines, replace=False)
 
     for group_id in sampled_groups:
@@ -710,28 +836,32 @@
 
     ax.set_xticks(sorted(df['time'].unique()))
     ax.set_xticklabels(sorted(df['time'].unique()), rotation=45, ha="right")
     ax.set_title(f'Normalized Delta of {measurement} Over Time (Corrected for Photobleaching)')
     ax.set_xlabel('Time')
     ax.set_ylabel('Normalized Delta ' + measurement)
     plt.tight_layout()
+    
     plt.show()
+
+    save_figure(fig, src=db_loc, figure_number=1)
     
     if pathogen:
         infected_vs_noninfected(result_df, measurement)
+        save_figure(fig, src=db_loc, figure_number=2)
 
-        # Identifying cells with and without infection
+        # Identify cells with and without pathogens
         infected_cells = result_df[result_df.groupby('plate_row_column_field_object')['parasite_count'].transform('max') > 0]['plate_row_column_field_object'].unique()
         noninfected_cells = result_df[result_df.groupby('plate_row_column_field_object')['parasite_count'].transform('max') == 0]['plate_row_column_field_object'].unique()
 
         # Peaks in infected and noninfected cells
         infected_peaks = peak_details_df[peak_details_df['ID'].isin(infected_cells)]
         noninfected_peaks = peak_details_df[peak_details_df['ID'].isin(noninfected_cells)]
 
         # Calculate the average number of peaks per cell
         avg_inf_peaks_per_cell = len(infected_peaks) / len(infected_cells) if len(infected_cells) > 0 else 0
         avg_non_inf_peaks_per_cell = len(noninfected_peaks) / len(noninfected_cells) if len(noninfected_cells) > 0 else 0
 
         print(f'Average number of peaks per infected cell: {avg_inf_peaks_per_cell:.2f}')
         print(f'Average number of peaks per non-infected cell: {avg_non_inf_peaks_per_cell:.2f}')
-
-    return result_df, peak_details_df
+    print(f'done')
+    return result_df, peak_details_df, fig
```

### Comparing `spacr-0.0.20/spacr/train.py` & `spacr-0.0.21/spacr/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,29 +190,29 @@
         result = pd.concat([pd.DataFrame(result), pd.DataFrame(data_mean, index=[str(epoch)+'_mean'])])
     end_time = time.time()
     test_time = end_time - start_time
     return result, results_df
 
 def train_test_model(src, settings, custom_model=False, custom_model_path=None):
     
-    from .io import save_settings, _copy_missclassified
-    from .utils import pick_best_model, test_model_performance
+    from .io import _save_settings, _copy_missclassified
+    from .utils import pick_best_model
     from .core import generate_loaders
     
     settings['src'] = src
     settings_df = pd.DataFrame(list(settings.items()), columns=['Key', 'Value'])
     settings_csv = os.path.join(src,'settings','train_test_model_settings.csv')
     os.makedirs(os.path.join(src,'settings'), exist_ok=True)
     settings_df.to_csv(settings_csv, index=False)
     
     if custom_model:
         model = torch.load(custom_model_path)
     
     if settings['train']:
-        save_settings(settings, src)
+        _save_settings(settings, src)
     torch.cuda.empty_cache()
     torch.cuda.memory.empty_cache()
     gc.collect()
     dst = os.path.join(src,'model')
     os.makedirs(dst, exist_ok=True)
     settings['src'] = src
     settings['dst'] = dst
@@ -223,27 +223,30 @@
                                                     image_size=settings['image_size'],
                                                     batch_size=settings['batch_size'], 
                                                     classes=settings['classes'], 
                                                     num_workers=settings['num_workers'],
                                                     validation_split=settings['val_split'],
                                                     pin_memory=settings['pin_memory'],
                                                     normalize=settings['normalize'],
-                                                    verbose=settings['verbose']) 
+                                                    channels=settings['channels'],
+                                                    verbose=settings['verbose'])
+                                                    
 
     if settings['test']:
         test, _, plate_names_test = generate_loaders(src, 
                                    train_mode=settings['train_mode'], 
                                    mode='test', 
                                    image_size=settings['image_size'],
                                    batch_size=settings['batch_size'], 
                                    classes=settings['classes'], 
                                    num_workers=settings['num_workers'],
                                    validation_split=0.0,
                                    pin_memory=settings['pin_memory'],
                                    normalize=settings['normalize'],
+                                   channels=settings['channels'],
                                    verbose=settings['verbose'])
         if model == None:
             model_path = pick_best_model(src+'/model')
             print(f'Best model: {model_path}')
 
             model = torch.load(model_path, map_location=lambda storage, loc: storage)
 
@@ -326,16 +329,16 @@
         gradient_accumulation (bool, optional): Whether to use gradient accumulation. Defaults to False.
         gradient_accumulation_steps (int, optional): The number of steps for gradient accumulation. Defaults to 4.
 
     Returns:
         None
     """    
     
-    from .io import save_model, save_progress
-    from .utils import evaluate_model_performance, compute_irm_penalty, calculate_loss, choose_model
+    from .io import _save_model, _save_progress
+    from .utils import compute_irm_penalty, calculate_loss, choose_model #evaluate_model_performance, 
     
     print(f'Train batches:{len(train_loaders)}, Validation batches:{len(val_loaders)}')
     
     if test_loaders != None:
         print(f'Test batches:{len(test_loaders)}')
         
     use_cuda = torch.cuda.is_available()
@@ -343,14 +346,19 @@
     kwargs = {'num_workers': num_workers, 'pin_memory': True} if use_cuda else {}
     
     for idx, (images, labels, filenames) in enumerate(train_loaders):
         batch, channels, height, width = images.shape
         break
 
     model = choose_model(model_type, device, init_weights, dropout_rate, use_checkpoint)
+
+    if model is None:
+        print(f'Model {model_type} not found')
+        return
+
     model.to(device)
     
     if optimizer_type == 'adamw':
         optimizer = AdamW(model.parameters(), lr=learning_rate,  betas=(0.9, 0.999), weight_decay=weight_decay, amsgrad=amsgrad)
     
     if optimizer_type == 'adagrad':
         optimizer = Adagrad(model.parameters(), lr=learning_rate, eps=1e-8, weight_decay=weight_decay)
@@ -417,18 +425,18 @@
             
             if scheduler:
                 if schedule == 'reduce_lr_on_plateau':
                     scheduler.step(val_loss)
                 if schedule == 'step_lr':
                     scheduler.step()
             
-            save_progress(dst, results_df, train_metrics_df)
+            _save_progress(dst, results_df, train_metrics_df)
             clear_output(wait=True)
             display(results_df)
-            save_model(model, model_type, results_df, dst, epoch, epochs, intermedeate_save=[0.99,0.98,0.95,0.94])
+            _save_model(model, model_type, results_df, dst, epoch, epochs, intermedeate_save=[0.99,0.98,0.95,0.94])
             
     if train_mode == 'irm':
         dummy_w = torch.nn.Parameter(torch.Tensor([1.0])).to(device)
         phi = torch.nn.Parameter (torch.ones(4,1))
         for epoch in range(1, epochs):
             model.train()
             penalty_factor = epoch * 1e-5
@@ -490,11 +498,11 @@
                 if schedule == 'reduce_lr_on_plateau':
                     scheduler.step(val_loss)
                 if schedule == 'step_lr':
                     scheduler.step()
             
             clear_output(wait=True)
             display(results_df)
-            save_progress(dst, results_df, train_metrics_df)
-            save_model(model, model_type, results_df, dst, epoch, epochs, intermedeate_save=[0.99,0.98,0.95,0.94])
+            _save_progress(dst, results_df, train_metrics_df)
+            _save_model(model, model_type, results_df, dst, epoch, epochs, intermedeate_save=[0.99,0.98,0.95,0.94])
             print(f'Saved model: {dst}')
     return
```

### Comparing `spacr-0.0.20/spacr/umap.py` & `spacr-0.0.21/spacr/umap.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/spacr/utils.py` & `spacr-0.0.21/spacr/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, re, sqlite3, gc, torch, torchvision, time, random, string, shutil, cv2, tarfile, glob
+import sys, os, re, sqlite3, gc, torch, torchvision, time, random, string, shutil, cv2, tarfile, glob
 
 import numpy as np
 from cellpose import models as cp_models
 from cellpose import denoise
 from skimage import morphology
 from skimage.measure import label, regionprops_table, regionprops
 import skimage.measure as measure
@@ -67,15 +67,16 @@
     overlayed_image = rgb_image.copy()
 
     def process_dim(mask_dim):
         mask = np.take(image, mask_dim, axis=-1)
         outline = np.zeros_like(mask, dtype=np.uint8)  # Use uint8 for contour detection efficiency
 
         # Find and draw contours
-        for j in np.unique(mask)[1:]:
+        for j in np.unique(mask):
+        #for j in np.unique(mask)[1:]:
             contours = find_contours(mask == j, 0.5)
             # Convert contours for OpenCV format and draw directly to optimize
             cv_contours = [np.flip(contour.astype(int), axis=1) for contour in contours]
             cv2.drawContours(outline, cv_contours, -1, color=int(j), thickness=outline_thickness)
 
         return dilation(outline, square(outline_thickness))
 
@@ -777,41 +778,42 @@
     
     return diamiter
 
 def _get_object_settings(object_type, settings):
     object_settings = {}
 
     object_settings['diameter'] = _get_diam(settings['magnification'], obj=object_type)
-    object_settings['minimum_size'] = (object_settings['diameter']**2)/5
-    object_settings['maximum_size'] = (object_settings['diameter']**2)*3
+    object_settings['minimum_size'] = (object_settings['diameter']**2)/4
+    object_settings['maximum_size'] = (object_settings['diameter']**2)*10
     object_settings['merge'] = False
     object_settings['resample'] = True
     object_settings['remove_border_objects'] = False
     object_settings['model_name'] = 'cyto'
     
     if object_type == 'cell':
         if settings['nucleus_channel'] is None:
             object_settings['model_name'] = 'cyto'
         else:
             object_settings['model_name'] = 'cyto2'
-        object_settings['filter_size'] = True
-        object_settings['filter_intensity'] = True
+        object_settings['filter_size'] = False
+        object_settings['filter_intensity'] = False
         object_settings['restore_type'] = settings.get('cell_restore_type', None)
 
     elif object_type == 'nucleus':
         object_settings['model_name'] = 'nuclei'
-        object_settings['filter_size'] = True
-        object_settings['filter_intensity'] = True
+        object_settings['filter_size'] = False
+        object_settings['filter_intensity'] = False
         object_settings['restore_type'] = settings.get('nucleus_restore_type', None)
 
     elif object_type == 'pathogen':
         object_settings['model_name'] = 'cyto'
         object_settings['filter_size'] = True
-        object_settings['filter_intensity'] = True
+        object_settings['filter_intensity'] = False
         object_settings['restore_type'] = settings.get('pathogen_restore_type', None)
+        object_settings['merge'] = settings['merge_pathogens']
         
     else:
         print(f'Object type: {object_type} not supported. Supported object types are : cell, nucleus and pathogen')
 
     if settings['verbose']:
         print(object_settings)
         
@@ -880,25 +882,23 @@
         
     cellpose_channels = {}
     if not nucleus_channel is None:
         cellpose_channels['nucleus'] = [0,0]
         
     if not pathogen_channel is None:
         if not nucleus_channel is None:
-            cellpose_channels['pathogen'] = [0,1]
+            if not pathogen_channel is None:
+                cellpose_channels['pathogen'] = [0,2]
+            else:
+                cellpose_channels['pathogen'] = [0,1]
         else:
             cellpose_channels['pathogen'] = [0,0]
         
     if not cell_channel is None:
         if not nucleus_channel is None:
-            if not pathogen_channel is None:
-                cellpose_channels['cell'] = [0,2]
-            else:
-                cellpose_channels['cell'] = [0,1]
-        elif not pathogen_channel is None:
             cellpose_channels['cell'] = [0,1]
         else:
             cellpose_channels['cell'] = [0,0]
     return cellpose_channels
     
 def annotate_conditions(df, cells=['HeLa'], cell_loc=None, pathogens=['rh'], pathogen_loc=None, treatments=['cm'], treatment_loc=None, types = ['col','col','col']):
     """
@@ -1065,15 +1065,15 @@
     A class representing a cache with a maximum size.
 
     Attributes:
         max_size (int): The maximum size of the cache.
         cache (OrderedDict): The cache data structure.
     """
 
-    def _init__(self, max_size):
+    def __init__(self, max_size):
         self.cache = OrderedDict()
         self.max_size = max_size
 
     def get(self, key):
         if key in self.cache:
             value = self.cache.pop(key)
             self.cache[key] = value
@@ -1096,15 +1096,15 @@
         d_k (int): The dimension of the key and query vectors.
 
     Methods:
         forward(Q, K, V): Performs the forward pass of the attention mechanism.
 
     """
 
-    def _init__(self, d_k):
+    def __init__(self, d_k):
         super(ScaledDotProductAttention, self).__init__()
         self.d_k = d_k
 
     def forward(self, Q, K, V):
         """
         Performs the forward pass of the attention mechanism.
 
@@ -1127,15 +1127,15 @@
     Self-Attention module that applies scaled dot-product attention mechanism.
     
     Args:
         in_channels (int): Number of input channels.
         d_k (int): Dimensionality of the key and query vectors.
     """
 
-    def _init__(self, in_channels, d_k):
+    def __init__(self, in_channels, d_k):
         super(SelfAttention, self).__init__()
         self.W_q = nn.Linear(in_channels, d_k)
         self.W_k = nn.Linear(in_channels, d_k)
         self.W_v = nn.Linear(in_channels, d_k)
         self.attention = ScaledDotProductAttention(d_k)
 
     def forward(self, x):
@@ -1151,15 +1151,15 @@
         Q = self.W_q(x)
         K = self.W_k(x)
         V = self.W_v(x)
         output = self.attention(Q, K, V)
         return output
 
 class ScaledDotProductAttention(nn.Module):
-    def _init__(self, d_k):
+    def __init__(self, d_k):
         """
         Initializes the ScaledDotProductAttention module.
 
         Args:
             d_k (int): The dimension of the key and query vectors.
 
         """
@@ -1188,15 +1188,15 @@
     """
     Self-Attention module that applies scaled dot-product attention mechanism.
     
     Args:
         in_channels (int): Number of input channels.
         d_k (int): Dimensionality of the key and query vectors.
     """
-    def _init__(self, in_channels, d_k):
+    def __init__(self, in_channels, d_k):
         super(SelfAttention, self).__init__()
         self.W_q = nn.Linear(in_channels, d_k)
         self.W_k = nn.Linear(in_channels, d_k)
         self.W_v = nn.Linear(in_channels, d_k)
         self.attention = ScaledDotProductAttention(d_k)
     
     def forward(self, x):
@@ -1219,15 +1219,15 @@
 class EarlyFusion(nn.Module):
     """
     Early Fusion module for image classification.
     
     Args:
         in_channels (int): Number of input channels.
     """
-    def _init__(self, in_channels):
+    def __init__(self, in_channels):
         super(EarlyFusion, self).__init__()
         self.conv1 = nn.Conv2d(in_channels, 64, kernel_size=1, stride=1)
         
     def forward(self, x):
         """
         Forward pass of the Early Fusion module.
         
@@ -1238,15 +1238,15 @@
             torch.Tensor: Output tensor of shape (batch_size, 64, height, width).
         """
         x = self.conv1(x)
         return x
 
 # Spatial Attention Mechanism
 class SpatialAttention(nn.Module):
-    def _init__(self, kernel_size=7):
+    def __init__(self, kernel_size=7):
         """
         Initializes the SpatialAttention module.
 
         Args:
             kernel_size (int): The size of the convolutional kernel. Default is 7.
         """
         super(SpatialAttention, self).__init__()
@@ -1283,15 +1283,15 @@
         spatial_attention (nn.Conv2d): Spatial attention layer.
 
     Methods:
         custom_forward: Custom forward method for the module.
         forward: Forward method for the module.
     """
 
-    def _init__(self, in_channels, out_channels):
+    def __init__(self, in_channels, out_channels):
         super(MultiScaleBlockWithAttention, self).__init__()
         self.dilated_conv1 = nn.Conv2d(in_channels, out_channels, kernel_size=3, dilation=1, padding=1)
         self.spatial_attention = nn.Conv2d(out_channels, out_channels, kernel_size=1)
         
     def custom_forward(self, x):
         """
         Custom forward method for the module.
@@ -1316,15 +1316,15 @@
         Returns:
             torch.Tensor: Output tensor.
         """
         return checkpoint(self.custom_forward, x)
 
 # Final Classifier
 class CustomCellClassifier(nn.Module):
-    def _init__(self, num_classes, pathogen_channel, use_attention, use_checkpoint, dropout_rate):
+    def __init__(self, num_classes, pathogen_channel, use_attention, use_checkpoint, dropout_rate):
         super(CustomCellClassifier, self).__init__()
         self.early_fusion = EarlyFusion(in_channels=3)
         
         self.multi_scale_block_1 = MultiScaleBlockWithAttention(in_channels=64, out_channels=64)
         
         self.fc1 = nn.Linear(64, num_classes)
         self.use_checkpoint = use_checkpoint
@@ -1345,15 +1345,15 @@
             x.requires_grad = True 
             return checkpoint(self.custom_forward, x)
         else:
             return self.custom_forward(x)
 
 #CNN and Transformer class, pick any Torch model.
 class TorchModel(nn.Module):
-    def _init__(self, model_name='resnet50', pretrained=True, dropout_rate=None, use_checkpoint=False):
+    def __init__(self, model_name='resnet50', pretrained=True, dropout_rate=None, use_checkpoint=False):
         super(TorchModel, self).__init__()
         self.model_name = model_name
         self.use_checkpoint = use_checkpoint
         self.base_model = self.init_base_model(pretrained)
         
         # Retain layers up to and including the (5): Linear layer for model 'maxvit_t'
         if model_name == 'maxvit_t':
@@ -1419,27 +1419,27 @@
             x = self.base_model(x)
         if self.use_dropout:
             x = self.dropout(x)
         logits = self.spacr_classifier(x).flatten()
         return logits
 
 class FocalLossWithLogits(nn.Module):
-    def _init__(self, alpha=1, gamma=2):
+    def __init__(self, alpha=1, gamma=2):
         super(FocalLossWithLogits, self).__init__()
         self.alpha = alpha
         self.gamma = gamma
 
     def forward(self, logits, target):
         BCE_loss = F.binary_cross_entropy_with_logits(logits, target, reduction='none')
         pt = torch.exp(-BCE_loss)
         focal_loss = self.alpha * (1-pt)**self.gamma * BCE_loss
         return focal_loss.mean()
     
 class ResNet(nn.Module):
-    def _init__(self, resnet_type='resnet50', dropout_rate=None, use_checkpoint=False, init_weights='imagenet'):
+    def __init__(self, resnet_type='resnet50', dropout_rate=None, use_checkpoint=False, init_weights='imagenet'):
         super(ResNet, self).__init__()
 
         resnet_map = {
             'resnet18': {'func': models.resnet18, 'weights': ResNet18_Weights.IMAGENET1K_V1},
             'resnet34': {'func': models.resnet34, 'weights': ResNet34_Weights.IMAGENET1K_V1},
             'resnet50': {'func': models.resnet50, 'weights': ResNet50_Weights.IMAGENET1K_V1},
             'resnet101': {'func': models.resnet101, 'weights': ResNet101_Weights.IMAGENET1K_V1},
@@ -1784,33 +1784,32 @@
             return 'nc'
         else:
             return ''
 
     df['cond'] = df.apply(assign_condition, axis=1)
     return df
 
-def init_globals(counter_, lock_):
+def initiate_counter(counter_, lock_):
     global counter, lock
     counter = counter_
     lock = lock_
 
-def add_images_to_tar(args):
-    global counter, lock, total_images
-    paths_chunk, tar_path = args
+def add_images_to_tar(paths_chunk, tar_path, total_images):
     with tarfile.open(tar_path, 'w') as tar:
-        for img_path in paths_chunk:
+        for i, img_path in enumerate(paths_chunk):
             arcname = os.path.basename(img_path)
             try:
                 tar.add(img_path, arcname=arcname)
                 with lock:
                     counter.value += 1
-                    print(f"\rProcessed: {counter.value}/{total_images}", end='', flush=True)
+                    if counter.value % 100 == 0:  # Print every 100 updates
+                        progress = (counter.value / total_images) * 100
+                        print(f"Progress: {counter.value}/{total_images} ({progress:.2f}%)", end='\r', file=sys.stdout, flush=True)
             except FileNotFoundError:
                 print(f"File not found: {img_path}")
-    return tar_path
 
 def generate_fraction_map(df, gene_column, min_frequency=0.0):
     df['fraction'] = df['count']/df['well_read_sum']
     genes = df[gene_column].unique().tolist()
     wells = df['prc'].unique().tolist()
     print(len(genes),len(wells))
     independent_variables = pd.DataFrame(columns=genes, index = wells)
@@ -2251,16 +2250,16 @@
     
     # Return the Dice coefficient
     return 2.0 * intersection / total
 
 def extract_boundaries(mask, dilation_radius=1):
     binary_mask = (mask > 0).astype(np.uint8)
     struct_elem = np.ones((dilation_radius*2+1, dilation_radius*2+1))
-    dilated = binary_dilation(binary_mask, footprint=struct_elem)
-    eroded = binary_erosion(binary_mask, footprint=struct_elem)
+    dilated = morphology.binary_dilation(binary_mask, footprint=struct_elem)
+    eroded = morphology.binary_erosion(binary_mask, footprint=struct_elem)
     boundary = dilated ^ eroded
     return boundary
 
 def boundary_f1_score(mask_true, mask_pred, dilation_radius=1):
     # Assume extract_boundaries is defined to extract object boundaries with given dilation_radius
     boundary_true = extract_boundaries(mask_true, dilation_radius)
     boundary_pred = extract_boundaries(mask_pred, dilation_radius)
@@ -2665,14 +2664,21 @@
     for idx, (mask, flow, image) in enumerate(zip(masks, flows[0], batch)):
         
         if plot and idx == 0:
             num_objects = mask_object_count(mask)
             print(f'Number of objects before filtration: {num_objects}')
             plot_masks(batch=image, masks=mask, flows=flow, cmap='inferno', figuresize=figuresize, nr=1, file_type='.npz', print_object_number=True)
 
+        if merge:
+            mask = merge_touching_objects(mask, threshold=0.66)
+            if plot and idx == 0:
+                num_objects = mask_object_count(mask)
+                print(f'Number of objects after merging adjacent objects, : {num_objects}')
+                plot_masks(batch=image, masks=mask, flows=flow, cmap='inferno', figuresize=figuresize, nr=1, file_type='.npz', print_object_number=True)
+
         if filter_size:
             props = measure.regionprops_table(mask, properties=['label', 'area'])
             valid_labels = props['label'][np.logical_and(props['area'] > minimum_size, props['area'] < maximum_size)] 
             mask = np.isin(mask, valid_labels) * mask
             if plot and idx == 0:
                 num_objects = mask_object_count(mask)
                 print(f'Number of objects after size filtration >{minimum_size} and <{maximum_size} : {num_objects}')
@@ -2710,21 +2716,14 @@
         if remove_border_objects:
             mask = clear_border(mask)
             if plot and idx == 0:
                 num_objects = mask_object_count(mask)
                 print(f'Number of objects after removing border objects, : {num_objects}')
                 plot_masks(batch=image, masks=mask, flows=flow, cmap='inferno', figuresize=figuresize, nr=1, file_type='.npz', print_object_number=True)
         
-        if merge:
-            mask = merge_touching_objects(mask, threshold=0.25)
-            if plot and idx == 0:
-                num_objects = mask_object_count(mask)
-                print(f'Number of objects after merging adjacent objects, : {num_objects}')
-                plot_masks(batch=image, masks=mask, flows=flow, cmap='inferno', figuresize=figuresize, nr=1, file_type='.npz', print_object_number=True)
-        
         mask_stack.append(mask)
 
     return mask_stack
     
 def _object_filter(df, object_type, size_range, intensity_range, mask_chans, mask_chan):
     """
     Filter the DataFrame based on object type, size range, and intensity range.
@@ -2785,14 +2784,15 @@
                 # For non-timelapse, you might want to distinguish sets more granularly
                 # Here, assuming you're grouping by plate, well, and field for simplicity
                 set_identifier = (plate, well, field)
             images_by_set[set_identifier].append(filename)
     
     # Prepare for random selection
     set_identifiers = list(images_by_set.keys())
+    random.seed(42)
     random.shuffle(set_identifiers)  # Randomize the order
     
     # Select a subset based on the test_images count
     selected_sets = set_identifiers[:test_images]
 
     # Print information about the number of sets used
     print(f'Using {test_images} random image set(s) for test model')
```

### Comparing `spacr-0.0.20/spacr.egg-info/PKG-INFO` & `spacr-0.0.21/spacr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacr
-Version: 0.0.20
+Version: 0.0.21
 Summary: Spatial phenotype analysis of crisp screens (SpaCr)
 Home-page: https://github.com/EinarOlafsson/spacr
 Author: Einar Birnir Olafsson
 Author-email: olafsson@med.umich.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,26 +15,29 @@
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.1
 Requires-Dist: statsmodels>=0.14.1
 Requires-Dist: scikit-image>=0.22.0
 Requires-Dist: scikit-learn>=1.4.1
 Requires-Dist: seaborn>=0.13.2
 Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: shap>=0.45.0
 Requires-Dist: pillow>=10.2.0
 Requires-Dist: imageio>=2.34.0
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: ipywidgets>=8.1.2
 Requires-Dist: mahotas>=1.4.13
 Requires-Dist: btrack>=0.6.5
 Requires-Dist: trackpy>=0.6.2
 Requires-Dist: cellpose>=3.0.6
 Requires-Dist: IPython>=8.18.1
 Requires-Dist: opencv-python-headless>=4.9.0.80
 Requires-Dist: umap>=0.1.1
 Requires-Dist: ttkthemes>=3.2.2
+Requires-Dist: xgboost>=2.0.3
+Requires-Dist: PyWavelets>=1.6.0
 Requires-Dist: lxml>=5.1.0
 Provides-Extra: dev
 Requires-Dist: pytest>=3.9; extra == "dev"
 Provides-Extra: headless
 Requires-Dist: opencv-python-headless; extra == "headless"
 Provides-Extra: full
 Requires-Dist: opencv-python; extra == "full"
@@ -45,15 +48,15 @@
 [![repo size](https://img.shields.io/github/repo-size/EinarOlafsson/spacr)](https://github.com/EinarOlafsson/spacr/)
 
 # SpaCr
 <table>
 <tr>
 <td>
   
-Spatial phenotype analysis of crisp screens (SpaCr). A collection of functions for generating cellpose masks -> single object images and measurements -> annotation and classification of single object images. Spacr uses batch normalization to facilitate accurate segmentation of objects with low foreground representation.
+Spatial phenotype analysis of CRISPR-Cas9 screens (SpaCr). The spatial organization of organelles and proteins within cells constitutes a key level of functional regulation. In the context of infectious disease, the spatial relationships between host cell structures and intracellular pathogens are critical to understand host clearance mechanisms and how pathogens evade them. Spacr is a Python-based software package for generating single cell image data for deep-learning sub-cellular/cellular phenotypic classification from pooled genetic CRISPR-Cas9 screens. Spacr provides a flexible toolset to extract single cell images and measurements from high content cell painting experiments, train deep-learning models to classify cellular/ subcellular phenotypes, simulate and analyze pooled CRISPR-Cas9 imaging screens.
 
 </td>
 <td>
 
 <img src="spacr/logo_spacr.png" alt="SPACR Logo" title="SPACR Logo" width="600"/>
 
 </td>
```

#### html2text {}

```diff
@@ -1,36 +1,45 @@
-Metadata-Version: 2.1 Name: spacr Version: 0.0.20 Summary: Spatial phenotype
+Metadata-Version: 2.1 Name: spacr Version: 0.0.21 Summary: Spatial phenotype
 analysis of crisp screens (SpaCr) Home-page: https://github.com/EinarOlafsson/
 spacr Author: Einar Birnir Olafsson Author-email: olafsson@med.umich.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent License-
 File: LICENSE Requires-Dist: torch>=2.2.1 Requires-Dist: torchvision>=0.17.1
 Requires-Dist: torch-geometric>=2.5.1 Requires-Dist: numpy>=1.26.4 Requires-
 Dist: pandas>=2.2.1 Requires-Dist: statsmodels>=0.14.1 Requires-Dist: scikit-
 image>=0.22.0 Requires-Dist: scikit-learn>=1.4.1 Requires-Dist: seaborn>=0.13.2
-Requires-Dist: matplotlib>=3.8.3 Requires-Dist: pillow>=10.2.0 Requires-Dist:
-imageio>=2.34.0 Requires-Dist: scipy>=1.12.0 Requires-Dist: ipywidgets>=8.1.2
-Requires-Dist: mahotas>=1.4.13 Requires-Dist: btrack>=0.6.5 Requires-Dist:
-trackpy>=0.6.2 Requires-Dist: cellpose>=3.0.6 Requires-Dist: IPython>=8.18.1
-Requires-Dist: opencv-python-headless>=4.9.0.80 Requires-Dist: umap>=0.1.1
-Requires-Dist: ttkthemes>=3.2.2 Requires-Dist: lxml>=5.1.0 Provides-Extra: dev
-Requires-Dist: pytest>=3.9; extra == "dev" Provides-Extra: headless Requires-
-Dist: opencv-python-headless; extra == "headless" Provides-Extra: full
-Requires-Dist: opencv-python; extra == "full" [![PyPI version](https://
-badge.fury.io/py/spacr.svg)](https://badge.fury.io/py/spacr) [![Python version]
-(https://img.shields.io/pypi/pyversions/spacr)](https://pypistats.org/packages/
-spacr) [![Licence: GPL v3](https://img.shields.io/github/license/EinarOlafsson/
-spacr)](https://github.com/EinarOlafsson/spacr/blob/master/LICENSE) [![repo
-size](https://img.shields.io/github/repo-size/EinarOlafsson/spacr)](https://
-github.com/EinarOlafsson/spacr/) # SpaCr
-Spatial phenotype analysis of crisp screens (SpaCr). A collection
-of functions for generating cellpose masks -> single object images
-and measurements -> annotation and classification of single object [SPACR Logo]
-images. Spacr uses batch normalization to facilitate accurate
-segmentation of objects with low foreground representation.
+Requires-Dist: matplotlib>=3.8.3 Requires-Dist: shap>=0.45.0 Requires-Dist:
+pillow>=10.2.0 Requires-Dist: imageio>=2.34.0 Requires-Dist: scipy>=1.12.0
+Requires-Dist: ipywidgets>=8.1.2 Requires-Dist: mahotas>=1.4.13 Requires-Dist:
+btrack>=0.6.5 Requires-Dist: trackpy>=0.6.2 Requires-Dist: cellpose>=3.0.6
+Requires-Dist: IPython>=8.18.1 Requires-Dist: opencv-python-headless>=4.9.0.80
+Requires-Dist: umap>=0.1.1 Requires-Dist: ttkthemes>=3.2.2 Requires-Dist:
+xgboost>=2.0.3 Requires-Dist: PyWavelets>=1.6.0 Requires-Dist: lxml>=5.1.0
+Provides-Extra: dev Requires-Dist: pytest>=3.9; extra == "dev" Provides-Extra:
+headless Requires-Dist: opencv-python-headless; extra == "headless" Provides-
+Extra: full Requires-Dist: opencv-python; extra == "full" [![PyPI version]
+(https://badge.fury.io/py/spacr.svg)](https://badge.fury.io/py/spacr) [![Python
+version](https://img.shields.io/pypi/pyversions/spacr)](https://pypistats.org/
+packages/spacr) [![Licence: GPL v3](https://img.shields.io/github/license/
+EinarOlafsson/spacr)](https://github.com/EinarOlafsson/spacr/blob/master/
+LICENSE) [![repo size](https://img.shields.io/github/repo-size/EinarOlafsson/
+spacr)](https://github.com/EinarOlafsson/spacr/) # SpaCr
+Spatial phenotype analysis of CRISPR-Cas9 screens (SpaCr). The
+spatial organization of organelles and proteins within cells
+constitutes a key level of functional regulation. In the context
+of infectious disease, the spatial relationships between host cell
+structures and intracellular pathogens are critical to understand
+host clearance mechanisms and how pathogens evade them. Spacr is a
+Python-based software package for generating single cell image     [SPACR Logo]
+data for deep-learning sub-cellular/cellular phenotypic
+classification from pooled genetic CRISPR-Cas9 screens. Spacr
+provides a flexible toolset to extract single cell images and
+measurements from high content cell painting experiments, train
+deep-learning models to classify cellular/ subcellular phenotypes,
+simulate and analyze pooled CRISPR-Cas9 imaging screens.
 ## Features - **Generate Masks:** Generate cellpose masks for cells, nuclei and
 pathogen images. - **Object Measurements:** Measurements for each object
 including scikit-image-regionprops, intensity quantiles, shannon-entropy,
 pearsons and manders correlation, homogenicity and radial distribution.
 Measurements are saved to a sql database in object level tables. - **Crop
 Images:** Objects (e.g. cells) can be saved as PNGs from the object area or
 bounding box area of each object. Object paths are saved in an sql database
```

### Comparing `spacr-0.0.20/spacr.egg-info/SOURCES.txt` & `spacr-0.0.21/spacr.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 setup.py
 spacr/__init__.py
 spacr/__main__.py
 spacr/alpha.py
 spacr/annotate_app.py
 spacr/cli.py
 spacr/core.py
+spacr/foldseek.py
+spacr/get_alfafold_structures.py
 spacr/graph_learning.py
 spacr/graph_learning_lap.py
 spacr/gui_classify_app.py
 spacr/gui_mask_app.py
 spacr/gui_measure_app.py
 spacr/gui_sim_app.py
 spacr/gui_utils.py
```

### Comparing `spacr-0.0.20/tests/test_annotate_app.py` & `spacr-0.0.21/tests/test_annotate_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_core.py` & `spacr-0.0.21/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_gui_classify_app.py` & `spacr-0.0.21/tests/test_gui_classify_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_gui_mask_app.py` & `spacr-0.0.21/tests/test_gui_mask_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_gui_measure_app.py` & `spacr-0.0.21/tests/test_gui_measure_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_gui_sim_app.py` & `spacr-0.0.21/tests/test_gui_sim_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_gui_utils.py` & `spacr-0.0.21/tests/test_gui_utils.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_io.py` & `spacr-0.0.21/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_mask_app.py` & `spacr-0.0.21/tests/test_mask_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_measure.py` & `spacr-0.0.21/tests/test_measure.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_plot.py` & `spacr-0.0.21/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_sim.py` & `spacr-0.0.21/tests/test_sim.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_timelapse.py` & `spacr-0.0.21/tests/test_timelapse.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_train.py` & `spacr-0.0.21/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_umap.py` & `spacr-0.0.21/tests/test_umap.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.20/tests/test_utils.py` & `spacr-0.0.21/tests/test_utils.py`

 * *Files identical despite different names*

