# Comparing `tmp/raster_tools-0.8.3.tar.gz` & `tmp/raster_tools-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster_tools-0.8.3.tar", last modified: Thu May 16 23:01:54 2024, max compression
+gzip compressed data, was "raster_tools-0.8.4.tar", last modified: Wed May 29 18:56:46 2024, max compression
```

## Comparing `raster_tools-0.8.3.tar` & `raster_tools-0.8.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-16 23:01:54.799033 raster_tools-0.8.3/
--rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster_tools-0.8.3/LICENSE
--rw-r--r--   0 fred      (1000) fred      (1000)      316 2024-01-18 23:44:47.000000 raster_tools-0.8.3/MANIFEST.in
--rw-r--r--   0 fred      (1000) fred      (1000)     2257 2024-05-16 23:01:54.799033 raster_tools-0.8.3/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1198 2024-01-18 23:44:47.000000 raster_tools-0.8.3/README.md
--rw-r--r--   0 fred      (1000) fred      (1000)     1406 2024-05-16 22:02:46.000000 raster_tools-0.8.3/pyproject.toml
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-16 23:01:54.795033 raster_tools-0.8.3/raster_tools/
--rw-r--r--   0 fred      (1000) fred      (1000)     1052 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)      383 2024-01-18 23:44:47.000000 raster_tools-0.8.3/raster_tools/_compat.py
--rw-r--r--   0 fred      (1000) fred      (1000)       22 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/_version.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7648 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/batch.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6693 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/clipping.py
--rw-r--r--   0 fred      (1000) fred      (1000)    11181 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/creation.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1600 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/dask_utils.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-16 23:01:54.795033 raster_tools-0.8.3/raster_tools/distance/
--rw-r--r--   0 fred      (1000) fred      (1000)      427 2024-01-18 23:44:47.000000 raster_tools-0.8.3/raster_tools/distance/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6737 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/distance/_heap.py
--rw-r--r--   0 fred      (1000) fred      (1000)    26525 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/distance/cost_distance.py
--rw-r--r--   0 fred      (1000) fred      (1000)    34945 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/distance/proximity.py
--rw-r--r--   0 fred      (1000) fred      (1000)     3221 2024-01-18 23:44:47.000000 raster_tools-0.8.3/raster_tools/dtypes.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    21032 2024-01-18 23:44:47.000000 raster_tools-0.8.3/raster_tools/focal.py
--rw-r--r--   0 fred      (1000) fred      (1000)    44623 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/general.py
--rw-r--r--   0 fred      (1000) fred      (1000)    11595 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/io.py
--rw-r--r--   0 fred      (1000) fred      (1000)    13317 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/line_stats.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2123 2024-05-16 22:02:37.000000 raster_tools-0.8.3/raster_tools/masking.py
--rw-r--r--   0 fred      (1000) fred      (1000)    76485 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/raster.py
--rw-r--r--   0 fred      (1000) fred      (1000)    24204 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/rasterize.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4281 2024-01-18 23:44:47.000000 raster_tools-0.8.3/raster_tools/stat_common.py
--rw-r--r--   0 fred      (1000) fred      (1000)    18429 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/surface.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4878 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/utils.py
--rw-r--r--   0 fred      (1000) fred      (1000)    30090 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/vector.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4138 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/warp.py
--rw-r--r--   0 fred      (1000) fred      (1000)    21212 2024-05-16 22:02:46.000000 raster_tools-0.8.3/raster_tools/zonal.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-16 23:01:54.795033 raster_tools-0.8.3/raster_tools.egg-info/
--rw-r--r--   0 fred      (1000) fred      (1000)     2257 2024-05-16 23:01:54.000000 raster_tools-0.8.3/raster_tools.egg-info/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1973 2024-05-16 23:01:54.000000 raster_tools-0.8.3/raster_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)        1 2024-05-16 23:01:54.000000 raster_tools-0.8.3/raster_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)      172 2024-05-16 23:01:54.000000 raster_tools-0.8.3/raster_tools.egg-info/requires.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       13 2024-05-16 23:01:54.000000 raster_tools-0.8.3/raster_tools.egg-info/top_level.txt
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-16 23:01:54.795033 raster_tools-0.8.3/requirements/
--rw-r--r--   0 fred      (1000) fred      (1000)      172 2024-05-16 22:02:46.000000 raster_tools-0.8.3/requirements/default.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       38 2024-05-16 23:01:54.799033 raster_tools-0.8.3/setup.cfg
--rw-r--r--   0 fred      (1000) fred      (1000)     1526 2024-05-16 22:02:46.000000 raster_tools-0.8.3/setup.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-16 23:01:54.795033 raster_tools-0.8.3/tests/
--rw-r--r--   0 fred      (1000) fred      (1000)     4332 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_clipping.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4832 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_creation.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7425 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_distance.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1297 2024-01-18 23:44:48.000000 raster_tools-0.8.3/tests/test_distance__heap.py
--rw-r--r--   0 fred      (1000) fred      (1000)    10034 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_distance_proximity.py
--rw-r--r--   0 fred      (1000) fred      (1000)    20208 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_focal.py
--rw-r--r--   0 fred      (1000) fred      (1000)    31451 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_general.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2540 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_io.py
--rw-r--r--   0 fred      (1000) fred      (1000)     8004 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_line_stats.py
--rw-r--r--   0 fred      (1000) fred      (1000)    85277 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_raster.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7679 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_rasterize.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4141 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_stat_common.py
--rw-r--r--   0 fred      (1000) fred      (1000)     5005 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_surface.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9117 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_vector.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6116 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_warp.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9453 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/test_zonal.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2113 2024-05-16 22:02:46.000000 raster_tools-0.8.3/tests/testdata.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-29 18:56:46.424682 raster_tools-0.8.4/
+-rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster_tools-0.8.4/LICENSE
+-rw-r--r--   0 fred      (1000) fred      (1000)      316 2024-01-18 23:44:47.000000 raster_tools-0.8.4/MANIFEST.in
+-rw-r--r--   0 fred      (1000) fred      (1000)     2280 2024-05-29 18:56:46.424682 raster_tools-0.8.4/PKG-INFO
+-rw-r--r--   0 fred      (1000) fred      (1000)     1221 2024-05-20 22:12:33.000000 raster_tools-0.8.4/README.md
+-rw-r--r--   0 fred      (1000) fred      (1000)     1406 2024-05-16 22:02:46.000000 raster_tools-0.8.4/pyproject.toml
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-29 18:56:46.424682 raster_tools-0.8.4/raster_tools/
+-rw-r--r--   0 fred      (1000) fred      (1000)     1052 2024-05-20 22:12:30.000000 raster_tools-0.8.4/raster_tools/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)      383 2024-01-18 23:44:47.000000 raster_tools-0.8.4/raster_tools/_compat.py
+-rw-r--r--   0 fred      (1000) fred      (1000)       22 2024-05-29 18:11:30.000000 raster_tools-0.8.4/raster_tools/_version.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7648 2024-05-16 22:02:46.000000 raster_tools-0.8.4/raster_tools/batch.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6693 2024-05-16 22:02:46.000000 raster_tools-0.8.4/raster_tools/clipping.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    11181 2024-05-16 22:02:46.000000 raster_tools-0.8.4/raster_tools/creation.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1600 2024-05-20 22:12:30.000000 raster_tools-0.8.4/raster_tools/dask_utils.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-29 18:56:46.424682 raster_tools-0.8.4/raster_tools/distance/
+-rw-r--r--   0 fred      (1000) fred      (1000)      427 2024-01-18 23:44:47.000000 raster_tools-0.8.4/raster_tools/distance/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6737 2024-05-16 22:02:46.000000 raster_tools-0.8.4/raster_tools/distance/_heap.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    26525 2024-05-16 22:02:46.000000 raster_tools-0.8.4/raster_tools/distance/cost_distance.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    34945 2024-05-16 22:02:46.000000 raster_tools-0.8.4/raster_tools/distance/proximity.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     3221 2024-01-18 23:44:47.000000 raster_tools-0.8.4/raster_tools/dtypes.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    21032 2024-01-18 23:44:47.000000 raster_tools-0.8.4/raster_tools/focal.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    46240 2024-05-29 17:47:19.000000 raster_tools-0.8.4/raster_tools/general.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    11595 2024-05-16 22:02:46.000000 raster_tools-0.8.4/raster_tools/io.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    13317 2024-05-16 22:02:46.000000 raster_tools-0.8.4/raster_tools/line_stats.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2123 2024-05-23 00:31:52.000000 raster_tools-0.8.4/raster_tools/masking.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    77041 2024-05-29 17:47:19.000000 raster_tools-0.8.4/raster_tools/raster.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    24204 2024-05-16 22:02:46.000000 raster_tools-0.8.4/raster_tools/rasterize.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4281 2024-01-18 23:44:47.000000 raster_tools-0.8.4/raster_tools/stat_common.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    18429 2024-05-16 22:02:46.000000 raster_tools-0.8.4/raster_tools/surface.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4878 2024-05-23 01:39:31.000000 raster_tools-0.8.4/raster_tools/utils.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    30090 2024-05-16 22:02:46.000000 raster_tools-0.8.4/raster_tools/vector.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4138 2024-05-16 22:02:46.000000 raster_tools-0.8.4/raster_tools/warp.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    21212 2024-05-29 18:22:04.000000 raster_tools-0.8.4/raster_tools/zonal.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-29 18:56:46.424682 raster_tools-0.8.4/raster_tools.egg-info/
+-rw-r--r--   0 fred      (1000) fred      (1000)     2280 2024-05-29 18:56:46.000000 raster_tools-0.8.4/raster_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1973 2024-05-29 18:56:46.000000 raster_tools-0.8.4/raster_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)        1 2024-05-29 18:56:46.000000 raster_tools-0.8.4/raster_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)      172 2024-05-29 18:56:46.000000 raster_tools-0.8.4/raster_tools.egg-info/requires.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       13 2024-05-29 18:56:46.000000 raster_tools-0.8.4/raster_tools.egg-info/top_level.txt
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-29 18:56:46.424682 raster_tools-0.8.4/requirements/
+-rw-r--r--   0 fred      (1000) fred      (1000)      172 2024-05-16 22:02:46.000000 raster_tools-0.8.4/requirements/default.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       38 2024-05-29 18:56:46.424682 raster_tools-0.8.4/setup.cfg
+-rw-r--r--   0 fred      (1000) fred      (1000)     1526 2024-05-16 22:02:46.000000 raster_tools-0.8.4/setup.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-29 18:56:46.424682 raster_tools-0.8.4/tests/
+-rw-r--r--   0 fred      (1000) fred      (1000)     4332 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/test_clipping.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4832 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/test_creation.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7425 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/test_distance.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1297 2024-01-18 23:44:48.000000 raster_tools-0.8.4/tests/test_distance__heap.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    10034 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/test_distance_proximity.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    20208 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/test_focal.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    32844 2024-05-29 17:47:19.000000 raster_tools-0.8.4/tests/test_general.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2540 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/test_io.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     8004 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/test_line_stats.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    84451 2024-05-29 17:47:19.000000 raster_tools-0.8.4/tests/test_raster.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7679 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/test_rasterize.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4141 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/test_stat_common.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     5005 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/test_surface.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9117 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/test_vector.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6116 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/test_warp.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9453 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/test_zonal.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2113 2024-05-16 22:02:46.000000 raster_tools-0.8.4/tests/testdata.py
```

### Comparing `raster_tools-0.8.3/LICENSE` & `raster_tools-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/PKG-INFO` & `raster_tools-0.8.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.8.3
+Version: 0.8.4
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,15 @@
 introducing new spatial, statistical, machine learning concepts into an
 easy-to-use python based API.
 
 ![image.gif](./notebooks/images/animatedRMRS2.gif)
 
 ## Helpful Links
 - [How to Contribute](./CONTRIBUTING.md)
-- [Documentation](./docs/README.md)
+- [Documentation](https://um-rmrs.github.io/raster_tools/)
 - [Notebooks & Tutorials](./notebooks/README.md)
 - [PyPi link](https://pypi.org/project/raster-tools/)
 - [Installation](./notebooks/install_raster_tools.md)
 
 ## Package Dependencies
 - [dask](https://dask.org/)
 - [dask_image](https://image.dask.org/en/latest/)
```

### Comparing `raster_tools-0.8.3/README.md` & `raster_tools-0.8.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 introducing new spatial, statistical, machine learning concepts into an
 easy-to-use python based API.
 
 ![image.gif](./notebooks/images/animatedRMRS2.gif)
 
 ## Helpful Links
 - [How to Contribute](./CONTRIBUTING.md)
-- [Documentation](./docs/README.md)
+- [Documentation](https://um-rmrs.github.io/raster_tools/)
 - [Notebooks & Tutorials](./notebooks/README.md)
 - [PyPi link](https://pypi.org/project/raster-tools/)
 - [Installation](./notebooks/install_raster_tools.md)
 
 ## Package Dependencies
 - [dask](https://dask.org/)
 - [dask_image](https://image.dask.org/en/latest/)
```

### Comparing `raster_tools-0.8.3/pyproject.toml` & `raster_tools-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/__init__.py` & `raster_tools-0.8.4/raster_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/batch.py` & `raster_tools-0.8.4/raster_tools/batch.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/clipping.py` & `raster_tools-0.8.4/raster_tools/clipping.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/creation.py` & `raster_tools-0.8.4/raster_tools/creation.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/dask_utils.py` & `raster_tools-0.8.4/raster_tools/dask_utils.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/distance/_heap.py` & `raster_tools-0.8.4/raster_tools/distance/_heap.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/distance/cost_distance.py` & `raster_tools-0.8.4/raster_tools/distance/cost_distance.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/distance/proximity.py` & `raster_tools-0.8.4/raster_tools/distance/proximity.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/dtypes.py` & `raster_tools-0.8.4/raster_tools/dtypes.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/focal.py` & `raster_tools-0.8.4/raster_tools/focal.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/general.py` & `raster_tools-0.8.4/raster_tools/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
-   Description: general module used to perform common spatial analyses
-   on Raster objects
+Description: general module used to perform common spatial analyses
+on Raster objects
 
-   * `ESRI Generalization Tools <https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-analyst/an-overview-of-the-generalization-tools.htm>`_
-   * `ESRI Local Tools <https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-analyst/an-overview-of-the-local-tools.htm>`_
+* `ESRI Generalization Tools <https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-analyst/an-overview-of-the-generalization-tools.htm>`_
+* `ESRI Local Tools <https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-analyst/an-overview-of-the-local-tools.htm>`_
 
 """  # noqa: E501
+
 import os
 import re
 from collections.abc import Iterable, Sequence
 from functools import partial
 
 import dask.array as da
 import numba as nb
@@ -42,15 +43,14 @@
     is_bool,
     is_int,
     is_scalar,
     is_str,
 )
 from raster_tools.focal import _get_offsets
 from raster_tools.masking import (
-    create_null_mask,
     get_default_null_value,
     reconcile_nullvalue_with_dtype,
 )
 from raster_tools.raster import Raster, get_raster
 from raster_tools.stat_common import (
     nan_unique_count_jit,
     nanargmax_jit,
@@ -1107,102 +1107,136 @@
     if raster._masked or None in map_news:
         outrs = outrs.set_null_value(nv)
     if f16_workaround:
         outrs = outrs.astype(F16)
     return outrs
 
 
+def _get_where_nv(x, y):
+    assert not ((x is None) and (y is None))
+    if (x is None or is_scalar(x)) and (y is None or is_scalar(y)):
+        # Both are either None or a scalar so get default
+        return get_default_null_value(
+            get_common_dtype([a for a in (x, y) if a is not None])
+        )
+    if isinstance(x, Raster) and isinstance(y, Raster):
+        # No easy way to pick so just get a default
+        return get_default_null_value(np.promote_types(x.dtype, y.dtype))
+    if x is None or is_scalar(x):
+        # y cannot be None or a scalar here. y must be a raster
+        return y.null_value if y._masked else get_default_null_value(y.dtype)
+    else:
+        # x must be a raster but not y
+        return x.null_value if x._masked else get_default_null_value(x.dtype)
+
+
 def where(condition, true_rast, false_rast):
     """
     Return elements chosen from `true_rast` or `false_rast` depending on
     `condition`.
 
+    The mask for the result is a combination of all three raster inputs. Any
+    cells that are masked in the condition raster will be masked in the output.
+    The rest of the cells are masked based on which raster they were taken
+    from, as determined by the condition raster, and if the cell in that raster
+    was null. Effectively, the resulting mask is determined as follows:
+    `where(condition.mask, True, where(condition, true_rast.mask,
+    false_rast.mask)`.
+
+    `true_rast` and `false_rast` can both be ``None`` to indicate a null value
+    but they cannot both be ``None`` at the same time. An error is raised in
+    that case.
+
     Parameters
     ----------
     condition : str or Raster
         A boolean or int raster that indicates where elements in the result
         should be selected from. If the condition is an int raster, it is
         coerced to bool using `condition > 0`.  ``True`` cells pull values from
         `true_rast` and ``False`` cells pull from `y`. *str* is treated as a
         path to a raster.
-    true_rast : scalar, Raster, str
+    true_rast : scalar, Raster, str, None
         Raster or scalar to pull from if the corresponding location in
-        `condition` is ``True``.
-    false_rast : scalar, Raster, str
+        `condition` is ``True``. If None, this is treated as a null value.
+    false_rast : scalar, Raster, str, None
         Raster or scalar to pull from if the corresponding location in
-        `condition` is ``False``.
+        `condition` is ``False``. If None, this is treated as a null value.
 
     Returns
     -------
     Raster
         The resulting Raster.
 
     """
     condition = get_raster(condition)
     if not is_bool(condition.dtype) and not is_int(condition.dtype):
         raise TypeError(
             "Condition argument must be a boolean or integer raster"
         )
     args = []
     for r, name in [(true_rast, "true_rast"), (false_rast, "false_rast")]:
-        if not is_scalar(r):
+        if not is_scalar(r) and r is not None:
             try:
                 r = get_raster(r)
             except TypeError as err:
                 raise TypeError(
                     f"Could not understand {name} argument. Got: {r!r}"
                 ) from err
         args.append(r)
-    true_rast, false_rast = args
+    if all(a is None for a in args):
+        raise ValueError("'true_rast' and 'false_rast' cannot both be None")
     out_crs = None
     for r in [condition, true_rast, false_rast]:
         crs = getattr(r, "crs", None)
         if crs is not None:
             out_crs = crs
             break
+    masked = condition._masked
+    masked |= any(r._masked if isinstance(r, Raster) else False for r in args)
+    masked |= any(a is None for a in args)
 
-    xtrue, xfalse = [r.xdata if isinstance(r, Raster) else r for r in args]
-    masked = any(r._masked if isinstance(r, Raster) else False for r in args)
-    scalar_and_nan = all(is_scalar(r) for r in args) and np.isnan(args).any()
-    masked |= scalar_and_nan
-    xcondition = condition.xdata
+    x, y = args
+    cd = condition.xdata
     if is_int(condition.dtype):
         # if condition.dtype is not bool then must be an int raster so
         # assume that condition is raster of 0 and 1 values.
         # condition > 0 will grab all 1/True values.
-        xcondition = xcondition > 0
-
-    out_xrs = xr.where(xcondition, xtrue, xfalse)
-    if masked and not scalar_and_nan:
-        xtrue_mask, xfalse_mask = [
-            r.xmask
-            if isinstance(r, Raster)
-            else xr.DataArray(
-                create_null_mask(condition.xdata, None),
-                dims=condition.xdata.dims,
-                coords=condition.xdata.coords,
-            )
-            for r in args
-        ]
-        xmask = xr.where(xcondition, xtrue_mask, xfalse_mask)
-    elif scalar_and_nan:
-        xmask = np.isnan(out_xrs)
+        cd = cd > 0
+    if masked:
+        nv = _get_where_nv(x, y)
+        if x is None:
+            x = nv
+        if y is None:
+            y = nv
+        if all(is_scalar(a) for a in (x, y)):
+            dtype = get_common_dtype((x, y))
+            x = dtype.type(x)
+            y = dtype.type(y)
+        cd = xr.where(condition.xmask, False, cd)
+        xd = getattr(x, "xdata", x)
+        yd = getattr(y, "xdata", y)
+        cm = condition.xmask
+        xm = getattr(x, "xmask", False)
+        ym = getattr(y, "xmask", False)
+        data = xr.where(cd, xd, yd)
+        mask = xr.where(cd, xm, ym)
+        mask = xr.where(cm, True, mask)
+        data = xr.where(mask, nv, data)
+        # Pick up any new null values caused by x/y being None or equal to nv
+        mask = data == nv if not np.isnan(nv) else np.isnan(data)
+        data = data.rio.write_nodata(nv)
     else:
-        xmask = xr.DataArray(
-            create_null_mask(condition.xdata, None),
-            dims=condition.xdata.dims,
-            coords=condition.xdata.coords,
-        )
-    if masked or scalar_and_nan:
-        nv = get_default_null_value(out_xrs.dtype)
-        out_xrs = xr.where(xmask, nv, out_xrs).rio.write_nodata(nv)
-    out_ds = make_raster_ds(out_xrs, xmask)
+        xd = getattr(x, "xdata", x)
+        yd = getattr(y, "xdata", y)
+        data = xr.where(cd, xd, yd)
+        mask = xr.zeros_like(data, dtype=bool)
+    ds = make_raster_ds(data, mask)
     if out_crs is not None:
-        out_ds = out_ds.rio.write_crs(out_crs)
-    return Raster(out_ds, _fast_path=True)
+        ds = ds.rio.write_crs(out_crs)
+    return Raster(ds, _fast_path=True)
 
 
 @nb.jit(nopython=True, nogil=True)
 def _reclassify_chunk(
     x, mask, mapping_from, mapping_to, unmapped_to_null, null, out_dtype
 ):
     mapping = dict(zip(mapping_from, mapping_to))
```

### Comparing `raster_tools-0.8.3/raster_tools/io.py` & `raster_tools-0.8.4/raster_tools/io.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/line_stats.py` & `raster_tools-0.8.4/raster_tools/line_stats.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/masking.py` & `raster_tools-0.8.4/raster_tools/masking.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/raster.py` & `raster_tools-0.8.4/raster_tools/raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1269,26 +1269,35 @@
             raise TypeError("value must be a scalar")
 
         return self.set_null_value(value)
 
     def where(self, condition, other):
         """Filter elements from this raster according to `condition`.
 
+        The mask for the result is a combination of all three rasters. Any
+        cells that are masked in the condition raster will be masked in the
+        output. The rest of the cells are masked based on which raster they
+        were taken from, as determined by the condition raster, and if the cell
+        in that raster was null. Effectively, the resulting mask is determined
+        as follows: `where(condition.mask, True, where(condition,
+        true_rast.mask, false_rast.mask)`.
+
         Parameters
         ----------
         condition : str or Raster
             A boolean or int raster that indicates where elements in this
             raster should be preserved and where `other` should be used. If
             the condition is an int raster, it is coerced to bool using
             `condition > 0`.  ``True`` cells pull values from this raster and
             ``False`` cells pull from `other`. *str* is treated as a path to a
             raster.
-        other : scalar, str or Raster
+        other : scalar, str or Raster, None
             A raster or value to use in locations where `condition` is
-            ``False``. *str* is treated as a path to a raster.
+            ``False``. *str* is treated as a path to a raster. If None, this is
+            treated as a null value.
 
         Returns
         -------
         Raster
             The resulting filtered Raster.
 
         """
```

### Comparing `raster_tools-0.8.3/raster_tools/rasterize.py` & `raster_tools-0.8.4/raster_tools/rasterize.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/stat_common.py` & `raster_tools-0.8.4/raster_tools/stat_common.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/surface.py` & `raster_tools-0.8.4/raster_tools/surface.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/utils.py` & `raster_tools-0.8.4/raster_tools/utils.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/vector.py` & `raster_tools-0.8.4/raster_tools/vector.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/warp.py` & `raster_tools-0.8.4/raster_tools/warp.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools/zonal.py` & `raster_tools-0.8.4/raster_tools/zonal.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/raster_tools.egg-info/PKG-INFO` & `raster_tools-0.8.4/raster_tools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.8.3
+Version: 0.8.4
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,15 @@
 introducing new spatial, statistical, machine learning concepts into an
 easy-to-use python based API.
 
 ![image.gif](./notebooks/images/animatedRMRS2.gif)
 
 ## Helpful Links
 - [How to Contribute](./CONTRIBUTING.md)
-- [Documentation](./docs/README.md)
+- [Documentation](https://um-rmrs.github.io/raster_tools/)
 - [Notebooks & Tutorials](./notebooks/README.md)
 - [PyPi link](https://pypi.org/project/raster-tools/)
 - [Installation](./notebooks/install_raster_tools.md)
 
 ## Package Dependencies
 - [dask](https://dask.org/)
 - [dask_image](https://image.dask.org/en/latest/)
```

### Comparing `raster_tools-0.8.3/raster_tools.egg-info/SOURCES.txt` & `raster_tools-0.8.4/raster_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/setup.py` & `raster_tools-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_clipping.py` & `raster_tools-0.8.4/tests/test_clipping.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_creation.py` & `raster_tools-0.8.4/tests/test_creation.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_distance.py` & `raster_tools-0.8.4/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_distance__heap.py` & `raster_tools-0.8.4/tests/test_distance__heap.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_distance_proximity.py` & `raster_tools-0.8.4/tests/test_distance_proximity.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_focal.py` & `raster_tools-0.8.4/tests/test_focal.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_general.py` & `raster_tools-0.8.4/tests/test_general.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     F64,
     I16,
     I32,
     I64,
     U8,
     U16,
     get_common_dtype,
-    is_scalar,
 )
 from raster_tools.masking import get_default_null_value
 from raster_tools.raster import Raster, get_raster
 from raster_tools.stat_common import (
     nan_unique_count_jit,
     nanargmax_jit,
     nanargmin_jit,
@@ -766,113 +765,145 @@
         general.remap_range(rs, (0, 1))
     with pytest.raises(ValueError):
         general.remap_range(rs, [(0, 1, 2), (0, 3)])
     with pytest.raises(ValueError):
         general.remap_range(rs, ())
 
 
-def get_where_truth(cond, x, y):
-    if cond.dtype != np.dtype(bool):
-        cond = cond > 0
-
-    chunks = "auto"
-    if not is_scalar(x):
-        chunks = x.data.chunks
-    elif not is_scalar(y):
-        chunks = y.data.chunks
-    cond = np.array(cond)
-    nx = (
-        np.ma.array(x.data.compute(), mask=x.mask.compute())
-        if not is_scalar(x)
-        else x
-    )
-    ny = (
-        np.ma.array(y.data.compute(), mask=y.mask.compute())
-        if not is_scalar(y)
-        else y
-    )
-    masked = any(r._masked if isinstance(r, Raster) else False for r in (x, y))
-    scalar_and_nan = (
-        all(is_scalar(r) for r in (x, y)) and np.isnan((x, y)).any()
-    )
-    masked |= scalar_and_nan
-
-    xmask = x.mask.compute() if not is_scalar(x) else np.zeros_like(cond)
-    ymask = y.mask.compute() if not is_scalar(y) else np.zeros_like(cond)
-
-    result = np.ma.where(cond, nx, ny)
-    mask = np.isnan(result) if scalar_and_nan else np.where(cond, xmask, ymask)
-    result = Raster(np.array(result))
-    if chunks != "auto":
-        result = result.chunk(chunks)
-    if masked:
-        result.xmask.data = da.from_array(mask, chunks=chunks)
-        result._ds["raster"] = result.xdata.rio.write_nodata(
-            get_default_null_value(result.dtype)
-        )
-        result = result.burn_mask()
-    return result
-
-
-wshape = (10, 10)
-nwhere = np.prod(wshape)
-
-
-def create_rs(x):
-    x = Raster(x)
-    x._ds = x._ds.rio.write_crs("EPSG:3857")
-    return x
+def _make_raster(data, mask, dtype=None):
+    data = np.asarray(data)
+    mask = np.asarray(mask).astype(bool)
+    # Allow nan values as valid data. Raster() automatically converts nans to
+    # null.
+    nan_mask = np.isnan(data)
+    if mask.any():
+        nan_mask[mask] = False
+    sent = -99
+    if nan_mask.any():
+        data[nan_mask] = sent
+    r = Raster(data).set_crs("EPSG:3857")
+    if nan_mask.any():
+        r._ds.raster.data = da.where(nan_mask, np.nan, r._ds.raster.data)
+    mask = Raster(mask)
+    if mask is not None:
+        r = r.set_null(mask)
+    if dtype is not None:
+        r = r.astype(dtype, False)
+    return r
 
 
 @pytest.mark.parametrize(
-    "x,y",
+    "condition,x,y,expected",
     [
-        (0, 1),
-        (0, np.nan),
-        (0, create_rs(np.ones(wshape))),
-        (0, create_rs(np.ones(wshape)).set_null_value(1)),
-        (create_rs(np.ones(wshape)), 0),
-        (create_rs(np.zeros(wshape)), create_rs(np.ones(wshape))),
-        (
-            create_rs(np.zeros(wshape)).set_null_value(0),
-            create_rs(np.ones(wshape)).set_null_value(1),
+        # 0
+        (
+            _make_raster([[0, 0], [1, 1]], np.zeros((2, 2)), bool),
+            _make_raster(np.ones((2, 2)), np.zeros((2, 2))),
+            _make_raster(np.full((2, 2), 2), np.zeros((2, 2))),
+            _make_raster([[2, 2], [1, 1]], np.zeros((2, 2))),
         ),
+        # 1
         (
-            create_rs(np.arange(nwhere).reshape(wshape)).set_null_value(10),
-            create_rs(np.arange(nwhere).reshape(wshape) + 20).set_null_value(
-                45
+            _make_raster([[0, 0], [1, 1]], [[1, 0], [0, 0]], bool),
+            _make_raster(np.ones((2, 2)), np.zeros((2, 2))),
+            _make_raster(np.full((2, 2), 2), np.zeros((2, 2))),
+            _make_raster([[0, 2], [1, 1]], [[1, 0], [0, 0]]),
+        ),
+        # 2
+        (
+            _make_raster([[0, 0], [1, 1]], [[1, 0], [0, 0]], bool),
+            _make_raster(np.ones((2, 2)), [[0, 1], [0, 0]]),
+            _make_raster(np.full((2, 2), 2), [[0, 0], [1, 0]]),
+            _make_raster([[0, 2], [1, 1]], [[1, 0], [0, 0]]),
+        ),
+        # 3
+        (
+            _make_raster([[0, 0], [1, 1]], [[1, 0], [0, 0]], bool),
+            _make_raster(np.ones((2, 2)), [[0, 0], [0, 1]]),
+            _make_raster(np.full((2, 2), 2), [[0, 1], [0, 0]]),
+            _make_raster([[2, 2], [1, 1]], [[1, 1], [0, 1]]),
+        ),
+        # 4
+        (
+            _make_raster([[0, 0], [1, 1]], [[1, 0], [0, 0]], bool),
+            _make_raster(np.ones((2, 2)), [[0, 0], [0, 1]]),
+            2,
+            _make_raster([[2, 2], [1, 1]], [[1, 0], [0, 1]]),
+        ),
+        # 5
+        (
+            _make_raster([[0, 0], [1, 1]], [[1, 0], [0, 0]], bool),
+            1,
+            _make_raster(np.full((2, 2), 2), [[0, 1], [0, 0]]),
+            _make_raster([[2, 2], [1, 1]], [[1, 1], [0, 0]]),
+        ),
+        # 6
+        (
+            _make_raster([[0, 0], [1, 1]], [[0, 0], [0, 0]], bool),
+            1,
+            2,
+            _make_raster([[2, 2], [1, 1]], [[0, 0], [0, 0]]),
+        ),
+        # 7
+        (
+            _make_raster([[0, 0], [1, 1]], [[1, 0], [0, 0]], bool),
+            1,
+            2,
+            _make_raster([[2, 2], [1, 1]], [[1, 0], [0, 0]], np.uint8),
+        ),
+        # 8
+        (
+            _make_raster([[0, 0], [1, 1]], [[1, 0], [0, 0]], bool),
+            1,
+            np.nan,
+            _make_raster(
+                [[np.nan, np.nan], [1, 1]], [[1, 0], [0, 0]], "float16"
             ),
         ),
+        # 9
+        (
+            _make_raster([[0, 0], [1, 1]], [[1, 0], [0, 0]], bool),
+            None,
+            _make_raster(np.full((2, 2), 2), [[0, 1], [0, 0]]),
+            _make_raster([[2, 2], [1, 1]], [[1, 1], [1, 1]]),
+        ),
+        # 10
+        (
+            _make_raster([[0, 0], [1, 1]], [[1, 0], [0, 0]], bool),
+            _make_raster(np.ones((2, 2)), [[0, 0], [0, 1]]),
+            None,
+            _make_raster([[2, 2], [1, 1]], [[1, 1], [0, 1]]),
+        ),
     ],
 )
-@pytest.mark.parametrize(
-    "cond",
-    [
-        create_rs(np.zeros(wshape, dtype=bool)),
-        create_rs(np.ones(wshape, dtype=bool)),
-        create_rs(np.arange(nwhere).reshape(wshape) > 40),
-        create_rs(np.arange(nwhere).reshape(wshape) % 10),
-        create_rs((np.arange(nwhere).reshape(wshape) % 10) > 0),
-        create_rs((np.arange(nwhere).reshape(wshape) % 4) > 0),
-    ],
-)
-def test_where(cond, x, y):
-    truth = get_where_truth(cond, x, y)
-    result = general.where(cond, x, y)
+def test_where(condition, x, y, expected):
+    masked = any(
+        v._masked for v in (condition, x, y) if isinstance(v, Raster)
+    ) or any(v is None for v in (x, y))
 
+    result = general.where(condition, x, y)
     assert_valid_raster(result)
-    assert np.allclose(result, truth, equal_nan=True)
-    assert result.dtype == result.dtype
-    if result._masked:
-        assert not np.isnan(result.null_value)
-    assert result.null_value == truth.null_value
-    assert np.allclose(result.xmask, truth.xmask)
-    assert result.data.chunks == truth.data.chunks
-    assert result.crs is not None
-    assert result.crs == "EPSG:3857"
+    assert_rasters_similar(result, condition)
+    assert result._masked == masked
+    assert np.allclose(result, expected, equal_nan=True)
+    assert np.allclose(result.mask.compute(), expected.mask.compute())
+
+    if isinstance(x, Raster):
+        result = x.where(condition, y)
+        assert_valid_raster(result)
+        assert_rasters_similar(result, condition)
+        assert result._masked == masked
+        assert np.allclose(result, expected, equal_nan=True)
+        assert np.allclose(result.mask.compute(), expected.mask.compute())
+
+
+def test_where_both_none():
+    with pytest.raises(ValueError):
+        cond = _make_raster([[0, 0], [1, 1]], [[1, 0], [0, 0]], bool)
+        general.where(cond, None, None)
 
 
 @pytest.mark.parametrize("unmapped_to_null", [True, False])
 @pytest.mark.parametrize(
     "raster,mapping,expected_out_dtype",
     [
         (
```

### Comparing `raster_tools-0.8.3/tests/test_io.py` & `raster_tools-0.8.4/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_line_stats.py` & `raster_tools-0.8.4/tests/test_line_stats.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_raster.py` & `raster_tools-0.8.4/tests/test_raster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1548,46 +1548,14 @@
     assert np.allclose(result, truth)
     assert np.allclose(result.mask.compute(), truth_mask)
     attrs = raster._ds.raster.attrs
     attrs["_FillValue"] = nv
     assert result._ds.raster.attrs == attrs
 
 
-@pytest.mark.filterwarnings("ignore:The null value")
-def test_where():
-    rs = testdata.raster.dem_small
-    c = rs > 1100
-
-    r = rs.where(c, 0)
-    assert_valid_raster(r)
-    rsnp = np.asarray(rs)
-    truth = np.where(rsnp > 1100, rsnp, 0)
-    assert np.allclose(r, truth)
-    assert np.allclose(rs.where(c, "tests/data/raster/dem_small.tif"), rs)
-    assert r.crs == rs.crs
-
-    c = c.astype(int)
-    r = rs.where(c, 0)
-    assert_valid_raster(r)
-    assert np.allclose(r, truth)
-
-    assert rs._masked
-    assert r._masked
-    assert rs.crs is not None
-    assert r.crs is not None
-    assert r.crs == rs.crs
-    assert r.null_value == get_default_null_value(r.dtype)
-
-    with pytest.raises(TypeError):
-        cf = c.astype(float)
-        rs.where(cf, 0)
-    with pytest.raises(TypeError):
-        rs.where(c, None)
-
-
 def test_to_null_mask():
     rs = testdata.raster.dem_clipped_small
     nv = rs.null_value
     rsnp = rs.to_numpy()
     truth = rsnp == nv
     assert rs.null_value is not None
     nmask = rs.to_null_mask()
```

### Comparing `raster_tools-0.8.3/tests/test_rasterize.py` & `raster_tools-0.8.4/tests/test_rasterize.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_stat_common.py` & `raster_tools-0.8.4/tests/test_stat_common.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_surface.py` & `raster_tools-0.8.4/tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_vector.py` & `raster_tools-0.8.4/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_warp.py` & `raster_tools-0.8.4/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/test_zonal.py` & `raster_tools-0.8.4/tests/test_zonal.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.3/tests/testdata.py` & `raster_tools-0.8.4/tests/testdata.py`

 * *Files identical despite different names*

