# Comparing `tmp/ttemtoolbox-1.1.tar.gz` & `tmp/ttemtoolbox-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttemtoolbox-1.1.tar", last modified: Wed May 29 18:50:22 2024, max compression
+gzip compressed data, was "ttemtoolbox-1.1.1.tar", last modified: Wed May 29 20:34:40 2024, max compression
```

## Comparing `ttemtoolbox-1.1.tar` & `ttemtoolbox-1.1.1.tar`

### file list

```diff
@@ -1,38 +1,35 @@
-drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 18:50:22.263701 ttemtoolbox-1.1/
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)    35149 2024-05-17 22:22:49.000000 ttemtoolbox-1.1/LICENSE
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)      785 2024-05-29 18:50:22.263701 ttemtoolbox-1.1/PKG-INFO
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)       85 2024-05-17 22:23:52.000000 ttemtoolbox-1.1/Readme.md
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)     1003 2024-05-29 18:40:06.000000 ttemtoolbox-1.1/pyproject.toml
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)       38 2024-05-29 18:50:22.263701 ttemtoolbox-1.1/setup.cfg
-drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 18:50:22.253701 ttemtoolbox-1.1/src/
-drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 18:50:22.263701 ttemtoolbox-1.1/src/ttemtoolbox/
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)      248 2024-05-29 00:47:06.000000 ttemtoolbox-1.1/src/ttemtoolbox/__init__.py
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)       19 2024-05-29 18:47:19.000000 ttemtoolbox-1.1/src/ttemtoolbox/_version.py
-drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 18:50:22.263701 ttemtoolbox-1.1/src/ttemtoolbox/core/
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)       21 2024-05-23 21:35:36.000000 ttemtoolbox-1.1/src/ttemtoolbox/core/__init__.py
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)     7382 2024-05-17 22:52:56.000000 ttemtoolbox-1.1/src/ttemtoolbox/core/gridsearch.py
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)     7371 2024-05-29 01:10:53.000000 ttemtoolbox-1.1/src/ttemtoolbox/core/lithology_connect.py
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)    14626 2024-05-17 22:23:52.000000 ttemtoolbox-1.1/src/ttemtoolbox/core/plot.py
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)     6148 2024-05-17 22:23:52.000000 ttemtoolbox-1.1/src/ttemtoolbox/core/process_gamma.py
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)    16312 2024-05-29 17:57:55.000000 ttemtoolbox-1.1/src/ttemtoolbox/core/process_ttem.py
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)     6473 2024-05-28 23:02:41.000000 ttemtoolbox-1.1/src/ttemtoolbox/core/process_water.py
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)    14993 2024-05-29 18:14:03.000000 ttemtoolbox-1.1/src/ttemtoolbox/core/process_well.py
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)     2240 2024-05-17 22:23:52.000000 ttemtoolbox-1.1/src/ttemtoolbox/core/rock_trans.py
-drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 18:50:22.263701 ttemtoolbox-1.1/src/ttemtoolbox/defaults/
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)     2230 2024-05-29 16:09:50.000000 ttemtoolbox-1.1/src/ttemtoolbox/defaults/CONFIG
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)       22 2024-05-23 21:35:45.000000 ttemtoolbox-1.1/src/ttemtoolbox/defaults/__init__.py
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)      958 2024-05-27 22:13:21.000000 ttemtoolbox-1.1/src/ttemtoolbox/defaults/constants.py
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)    11528 2024-05-29 18:36:57.000000 ttemtoolbox-1.1/src/ttemtoolbox/main.py
-drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 18:50:22.263701 ttemtoolbox-1.1/src/ttemtoolbox/utils/
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        1 2024-05-23 21:35:48.000000 ttemtoolbox-1.1/src/ttemtoolbox/utils/__init__.py
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)     7563 2024-05-17 22:23:52.000000 ttemtoolbox-1.1/src/ttemtoolbox/utils/canny_edge_detection.py
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-17 22:23:52.000000 ttemtoolbox-1.1/src/ttemtoolbox/utils/datafilter.py
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)     4869 2024-05-28 22:48:36.000000 ttemtoolbox-1.1/src/ttemtoolbox/utils/tools.py
--rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)     9768 2024-05-17 22:23:52.000000 ttemtoolbox-1.1/src/ttemtoolbox/utils/visualize_surface_kansas.py
-drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 18:50:22.263701 ttemtoolbox-1.1/src/ttemtoolbox.egg-info/
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)      785 2024-05-29 18:50:22.000000 ttemtoolbox-1.1/src/ttemtoolbox.egg-info/PKG-INFO
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)      976 2024-05-29 18:50:22.000000 ttemtoolbox-1.1/src/ttemtoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)        1 2024-05-29 18:50:22.000000 ttemtoolbox-1.1/src/ttemtoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)       54 2024-05-29 18:50:22.000000 ttemtoolbox-1.1/src/ttemtoolbox.egg-info/entry_points.txt
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)       45 2024-05-29 18:50:22.000000 ttemtoolbox-1.1/src/ttemtoolbox.egg-info/requires.txt
--rw-r--r--   0 jldz9     (1000) jldz9     (1000)       12 2024-05-29 18:50:22.000000 ttemtoolbox-1.1/src/ttemtoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 20:34:40.731977 ttemtoolbox-1.1.1/
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)    35149 2024-05-17 22:22:49.000000 ttemtoolbox-1.1.1/LICENSE
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)     3721 2024-05-29 20:34:40.731977 ttemtoolbox-1.1.1/PKG-INFO
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)     3019 2024-05-29 20:32:40.000000 ttemtoolbox-1.1.1/Readme.md
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)     1003 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/pyproject.toml
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)       38 2024-05-29 20:34:40.731977 ttemtoolbox-1.1.1/setup.cfg
+drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 20:34:40.721977 ttemtoolbox-1.1.1/src/
+drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 20:34:40.721977 ttemtoolbox-1.1.1/src/ttemtoolbox/
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)      303 2024-05-29 19:55:56.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/__init__.py
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)       21 2024-05-29 20:34:37.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/_version.py
+drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 20:34:40.721977 ttemtoolbox-1.1.1/src/ttemtoolbox/core/
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)       21 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/core/__init__.py
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)     7382 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/core/gridsearch.py
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)     7371 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/core/lithology_connect.py
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)    14626 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/core/plot.py
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)     6148 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/core/process_gamma.py
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)    16312 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/core/process_ttem.py
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)     6473 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/core/process_water.py
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)    14993 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/core/process_well.py
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)     2240 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/core/rock_trans.py
+drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 20:34:40.721977 ttemtoolbox-1.1.1/src/ttemtoolbox/defaults/
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)     2230 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/defaults/CONFIG
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)       22 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/defaults/__init__.py
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)      958 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/defaults/constants.py
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)    11802 2024-05-29 20:25:21.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/main.py
+drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 20:34:40.731977 ttemtoolbox-1.1.1/src/ttemtoolbox/utils/
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        1 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/utils/__init__.py
+-rwxr-xr-x   0 jldz9     (1000) jldz9     (1000)     4869 2024-05-29 18:51:39.000000 ttemtoolbox-1.1.1/src/ttemtoolbox/utils/tools.py
+drwxr-xr-x   0 jldz9     (1000) jldz9     (1000)        0 2024-05-29 20:34:40.731977 ttemtoolbox-1.1.1/src/ttemtoolbox.egg-info/
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)     3721 2024-05-29 20:34:40.000000 ttemtoolbox-1.1.1/src/ttemtoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)      844 2024-05-29 20:34:40.000000 ttemtoolbox-1.1.1/src/ttemtoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)        1 2024-05-29 20:34:40.000000 ttemtoolbox-1.1.1/src/ttemtoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)       54 2024-05-29 20:34:40.000000 ttemtoolbox-1.1.1/src/ttemtoolbox.egg-info/entry_points.txt
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)       45 2024-05-29 20:34:40.000000 ttemtoolbox-1.1.1/src/ttemtoolbox.egg-info/requires.txt
+-rw-r--r--   0 jldz9     (1000) jldz9     (1000)       12 2024-05-29 20:34:40.000000 ttemtoolbox-1.1.1/src/ttemtoolbox.egg-info/top_level.txt
```

### Comparing `ttemtoolbox-1.1/LICENSE` & `ttemtoolbox-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.1/pyproject.toml` & `ttemtoolbox-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.1/src/ttemtoolbox/core/gridsearch.py` & `ttemtoolbox-1.1.1/src/ttemtoolbox/core/gridsearch.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.1/src/ttemtoolbox/core/lithology_connect.py` & `ttemtoolbox-1.1.1/src/ttemtoolbox/core/lithology_connect.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.1/src/ttemtoolbox/core/plot.py` & `ttemtoolbox-1.1.1/src/ttemtoolbox/core/plot.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.1/src/ttemtoolbox/core/process_gamma.py` & `ttemtoolbox-1.1.1/src/ttemtoolbox/core/process_gamma.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.1/src/ttemtoolbox/core/process_ttem.py` & `ttemtoolbox-1.1.1/src/ttemtoolbox/core/process_ttem.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.1/src/ttemtoolbox/core/process_water.py` & `ttemtoolbox-1.1.1/src/ttemtoolbox/core/process_water.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.1/src/ttemtoolbox/core/process_well.py` & `ttemtoolbox-1.1.1/src/ttemtoolbox/core/process_well.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.1/src/ttemtoolbox/core/rock_trans.py` & `ttemtoolbox-1.1.1/src/ttemtoolbox/core/rock_trans.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.1/src/ttemtoolbox/defaults/CONFIG` & `ttemtoolbox-1.1.1/src/ttemtoolbox/defaults/CONFIG`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.1/src/ttemtoolbox/defaults/constants.py` & `ttemtoolbox-1.1.1/src/ttemtoolbox/defaults/constants.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.1/src/ttemtoolbox/main.py` & `ttemtoolbox-1.1.1/src/ttemtoolbox/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,26 +182,30 @@
         lithologylist = Path(config['well_temp']).glob('*.csv')
         temp_lithology = pd.concat([pd.read_csv(file) for file in lithologylist])
         lithology = gpd.GeoDataFrame(temp_lithology, geometry=gpd.points_from_xy(temp_lithology['X'], temp_lithology['Y']), 
                                 crs=config['lithology_reproject_crs'])
     matched_ttem, matched_lithology = lithology_connect.select_closest(ttem, lithology,
                                                                        search_radius = config['search_radius'])
     stitched = lithology_connect.ttem_well_connect(matched_ttem, matched_lithology)
-    stitched.to_csv(config['deliver'].joinpath('ttem_well_connect.csv'))
+    stitched.to_csv(Path(config['deliver']).joinpath('ttem_well_connect.csv'))
+    print('connected file saved to {}'.format(Path(config['deliver']).joinpath('ttem_well_connect.csv')))
     return stitched
     
 def main(iargs=None):
     inps = vars(cmd_line_parse(iargs)) # parse CLI input to dict
     #########run entire ttem rock physics tranform process
     if inps.get('config_path'):
         print('Run entire ttem rock physics tranform process')
         user_config = tools.parse_config(inps['config_path'])
         tools.clean_output(Path(user_config['output']))
         config = tools.create_dir_structure(user_config)
         ttemdata = step_ttem(config, inps)
+        lithology = step_lithology(config, inps)
+        water, meta = step_water(config, inps)
+        stitched = step_connect(config,inps, ttemdata, lithology)
         
     if inps.get('force_clean'):
         print('All result will be purged')
         tools.clean_output()
         
     #########Step1: Process ttem
     if inps.get('ttem'):
```

### Comparing `ttemtoolbox-1.1/src/ttemtoolbox/utils/tools.py` & `ttemtoolbox-1.1.1/src/ttemtoolbox/utils/tools.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.1/src/ttemtoolbox.egg-info/SOURCES.txt` & `ttemtoolbox-1.1.1/src/ttemtoolbox.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,11 +19,8 @@
 src/ttemtoolbox/core/process_water.py
 src/ttemtoolbox/core/process_well.py
 src/ttemtoolbox/core/rock_trans.py
 src/ttemtoolbox/defaults/CONFIG
 src/ttemtoolbox/defaults/__init__.py
 src/ttemtoolbox/defaults/constants.py
 src/ttemtoolbox/utils/__init__.py
-src/ttemtoolbox/utils/canny_edge_detection.py
-src/ttemtoolbox/utils/datafilter.py
-src/ttemtoolbox/utils/tools.py
-src/ttemtoolbox/utils/visualize_surface_kansas.py
+src/ttemtoolbox/utils/tools.py
```

