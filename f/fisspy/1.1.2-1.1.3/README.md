# Comparing `tmp/fisspy-1.1.2.tar.gz` & `tmp/fisspy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fisspy-1.1.2.tar", last modified: Tue May 21 11:01:10 2024, max compression
+gzip compressed data, was "fisspy-1.1.3.tar", last modified: Wed May 29 00:24:06 2024, max compression
```

## Comparing `fisspy-1.1.2.tar` & `fisspy-1.1.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.727981 fisspy-1.1.2/
--rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.1.2/LICENSE.txt
--rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-21 11:01:10.727778 fisspy-1.1.2/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.1.2/README.md
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.719081 fisspy-1.1.2/fisspy/
--rw-r--r--   0 jhkang     (501) staff       (20)      430 2024-05-21 10:57:52.000000 fisspy-1.1.2/fisspy/__init__.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.720480 fisspy-1.1.2/fisspy/align/
--rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/align/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15179 2024-04-24 08:05:01.000000 fisspy-1.1.2/fisspy/align/alignment.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-25 11:40:56.000000 fisspy-1.1.2/fisspy/align/base.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.721888 fisspy-1.1.2/fisspy/analysis/
--rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/analysis/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-25 11:37:49.000000 fisspy-1.1.2/fisspy/analysis/doppler.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/analysis/filter.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-25 11:30:36.000000 fisspy-1.1.2/fisspy/analysis/forecast.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/analysis/ofe.py
--rw-r--r--   0 jhkang     (501) staff       (20)    35716 2024-05-21 10:49:50.000000 fisspy-1.1.2/fisspy/analysis/tdmap.py
--rw-r--r--   0 jhkang     (501) staff       (20)    33907 2024-04-25 11:35:30.000000 fisspy-1.1.2/fisspy/analysis/wavelet.py
--rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.1.2/fisspy/cm.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.722394 fisspy-1.1.2/fisspy/correction/
--rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/correction/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-05-01 13:33:13.000000 fisspy-1.1.2/fisspy/correction/correction.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-30 00:59:33.000000 fisspy-1.1.2/fisspy/correction/get_inform.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.723177 fisspy-1.1.2/fisspy/data/
--rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.1.2/fisspy/data/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.1.2/fisspy/data/_sample.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.1.2/fisspy/data/download.py
--rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.1.2/fisspy/data/sample.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.723830 fisspy-1.1.2/fisspy/image/
--rw-r--r--   0 jhkang     (501) staff       (20)       73 2024-04-25 10:45:58.000000 fisspy-1.1.2/fisspy/image/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    30919 2024-05-21 08:38:40.000000 fisspy-1.1.2/fisspy/image/interactive_image.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12849 2024-05-01 06:38:35.000000 fisspy-1.1.2/fisspy/image/raster_set.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.724056 fisspy-1.1.2/fisspy/inversion/
--rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/inversion/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/inversion/_mlsi.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.724524 fisspy-1.1.2/fisspy/io/
--rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.1.2/fisspy/io/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.1.2/fisspy/io/read.py
--rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/makevideo.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.726820 fisspy-1.1.2/fisspy/preprocess/
--rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/preprocess/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    55166 2024-05-21 00:20:39.000000 fisspy-1.1.2/fisspy/preprocess/proc_base.py
--rw-r--r--   0 jhkang     (501) staff       (20)   151958 2024-05-21 03:46:35.000000 fisspy-1.1.2/fisspy/preprocess/proc_gui.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/preprocess/t_y_sh.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.727522 fisspy-1.1.2/fisspy/read/
--rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/read/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    50279 2024-05-10 13:45:00.000000 fisspy-1.1.2/fisspy/read/read_factory.py
--rw-r--r--   0 jhkang     (501) staff       (20)     6847 2024-04-25 06:03:54.000000 fisspy-1.1.2/fisspy/read/readbase.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.719853 fisspy-1.1.2/fisspy.egg-info/
--rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-21 11:01:10.000000 fisspy-1.1.2/fisspy.egg-info/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1079 2024-05-21 11:01:10.000000 fisspy-1.1.2/fisspy.egg-info/SOURCES.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-21 11:01:10.000000 fisspy-1.1.2/fisspy.egg-info/dependency_links.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-21 11:01:10.000000 fisspy-1.1.2/fisspy.egg-info/not-zip-safe
--rw-r--r--   0 jhkang     (501) staff       (20)      137 2024-05-21 11:01:10.000000 fisspy-1.1.2/fisspy.egg-info/requires.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-05-21 11:01:10.000000 fisspy-1.1.2/fisspy.egg-info/top_level.txt
--rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-05-21 11:01:10.728020 fisspy-1.1.2/setup.cfg
--rw-r--r--   0 jhkang     (501) staff       (20)      582 2024-05-21 10:59:23.000000 fisspy-1.1.2/setup.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-29 00:24:06.697578 fisspy-1.1.3/
+-rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.1.3/LICENSE.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-29 00:24:06.697372 fisspy-1.1.3/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.1.3/README.md
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-29 00:24:06.691865 fisspy-1.1.3/fisspy/
+-rw-r--r--   0 jhkang     (501) staff       (20)      430 2024-05-29 00:23:19.000000 fisspy-1.1.3/fisspy/__init__.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-29 00:24:06.692978 fisspy-1.1.3/fisspy/align/
+-rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.1.3/fisspy/align/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15179 2024-04-24 08:05:01.000000 fisspy-1.1.3/fisspy/align/alignment.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-25 11:40:56.000000 fisspy-1.1.3/fisspy/align/base.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-29 00:24:06.693914 fisspy-1.1.3/fisspy/analysis/
+-rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.1.3/fisspy/analysis/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-25 11:37:49.000000 fisspy-1.1.3/fisspy/analysis/doppler.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.1.3/fisspy/analysis/filter.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-25 11:30:36.000000 fisspy-1.1.3/fisspy/analysis/forecast.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.1.3/fisspy/analysis/ofe.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    35716 2024-05-21 10:49:50.000000 fisspy-1.1.3/fisspy/analysis/tdmap.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    33907 2024-04-25 11:35:30.000000 fisspy-1.1.3/fisspy/analysis/wavelet.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.1.3/fisspy/cm.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-29 00:24:06.694333 fisspy-1.1.3/fisspy/correction/
+-rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.1.3/fisspy/correction/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-05-01 13:33:13.000000 fisspy-1.1.3/fisspy/correction/correction.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-30 00:59:33.000000 fisspy-1.1.3/fisspy/correction/get_inform.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-29 00:24:06.694722 fisspy-1.1.3/fisspy/data/
+-rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.1.3/fisspy/data/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.1.3/fisspy/data/_sample.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.1.3/fisspy/data/download.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.1.3/fisspy/data/sample.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-29 00:24:06.695052 fisspy-1.1.3/fisspy/image/
+-rw-r--r--   0 jhkang     (501) staff       (20)       73 2024-04-25 10:45:58.000000 fisspy-1.1.3/fisspy/image/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    30919 2024-05-21 08:38:40.000000 fisspy-1.1.3/fisspy/image/interactive_image.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12849 2024-05-01 06:38:35.000000 fisspy-1.1.3/fisspy/image/raster_set.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-29 00:24:06.695287 fisspy-1.1.3/fisspy/inversion/
+-rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.1.3/fisspy/inversion/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.1.3/fisspy/inversion/_mlsi.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-29 00:24:06.695493 fisspy-1.1.3/fisspy/io/
+-rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.1.3/fisspy/io/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.1.3/fisspy/io/read.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.1.3/fisspy/makevideo.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-29 00:24:06.696716 fisspy-1.1.3/fisspy/preprocess/
+-rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.1.3/fisspy/preprocess/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    55171 2024-05-27 06:01:27.000000 fisspy-1.1.3/fisspy/preprocess/proc_base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)   151962 2024-05-27 06:01:27.000000 fisspy-1.1.3/fisspy/preprocess/proc_gui.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.1.3/fisspy/preprocess/t_y_sh.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-29 00:24:06.697098 fisspy-1.1.3/fisspy/read/
+-rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.1.3/fisspy/read/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    50279 2024-05-10 13:45:00.000000 fisspy-1.1.3/fisspy/read/read_factory.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     6847 2024-04-25 06:03:54.000000 fisspy-1.1.3/fisspy/read/readbase.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-29 00:24:06.692598 fisspy-1.1.3/fisspy.egg-info/
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-29 00:24:06.000000 fisspy-1.1.3/fisspy.egg-info/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1079 2024-05-29 00:24:06.000000 fisspy-1.1.3/fisspy.egg-info/SOURCES.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-29 00:24:06.000000 fisspy-1.1.3/fisspy.egg-info/dependency_links.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-29 00:24:06.000000 fisspy-1.1.3/fisspy.egg-info/not-zip-safe
+-rw-r--r--   0 jhkang     (501) staff       (20)      137 2024-05-29 00:24:06.000000 fisspy-1.1.3/fisspy.egg-info/requires.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-05-29 00:24:06.000000 fisspy-1.1.3/fisspy.egg-info/top_level.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-05-29 00:24:06.697618 fisspy-1.1.3/setup.cfg
+-rw-r--r--   0 jhkang     (501) staff       (20)      582 2024-05-29 00:23:18.000000 fisspy-1.1.3/setup.py
```

### Comparing `fisspy-1.1.2/LICENSE.txt` & `fisspy-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/PKG-INFO` & `fisspy-1.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisspy
-Version: 1.1.2
+Version: 1.1.3
 Summary: fisspy: Python analysis tools for GST/FISS
 Home-page: http://fiss.snu.ac.kr
 Author: Juhyung Kang
 Author-email: jhkang@astro.snu.ac.kr
 License: BSD-2
 Requires-Python: >=3.6
 License-File: LICENSE.txt
```

### Comparing `fisspy-1.1.2/README.md` & `fisspy-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/align/alignment.py` & `fisspy-1.1.3/fisspy/align/alignment.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/align/base.py` & `fisspy-1.1.3/fisspy/align/base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/analysis/doppler.py` & `fisspy-1.1.3/fisspy/analysis/doppler.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/analysis/filter.py` & `fisspy-1.1.3/fisspy/analysis/filter.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/analysis/forecast.py` & `fisspy-1.1.3/fisspy/analysis/forecast.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/analysis/ofe.py` & `fisspy-1.1.3/fisspy/analysis/ofe.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/analysis/tdmap.py` & `fisspy-1.1.3/fisspy/analysis/tdmap.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/analysis/wavelet.py` & `fisspy-1.1.3/fisspy/analysis/wavelet.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/cm.py` & `fisspy-1.1.3/fisspy/cm.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/correction/correction.py` & `fisspy-1.1.3/fisspy/correction/correction.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/correction/get_inform.py` & `fisspy-1.1.3/fisspy/correction/get_inform.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/data/_sample.py` & `fisspy-1.1.3/fisspy/data/_sample.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/data/download.py` & `fisspy-1.1.3/fisspy/data/download.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/image/interactive_image.py` & `fisspy-1.1.3/fisspy/image/interactive_image.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/image/raster_set.py` & `fisspy-1.1.3/fisspy/image/raster_set.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/io/read.py` & `fisspy-1.1.3/fisspy/io/read.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/makevideo.py` & `fisspy-1.1.3/fisspy/makevideo.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/preprocess/proc_base.py` & `fisspy-1.1.3/fisspy/preprocess/proc_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     x = np.arange(nwl)
     # sig = hw/np.sqrt(2/np.log(2))
     sig = hw
     p = [1, xc, sig]
     GF = Gaussian(x, *p)
     
     wv = wvlet.wavelet*GF[None,:,None]
-    mwv = np.abs(wv).mean((0,2))
+    mwv = (np.abs(wv)**2).mean((0,2))
     return mwv, wvlet.iwavelet(wv, wvlet.scale)
     # freq = np.arctan2(wvlet.wavelet.imag, wvlet.wavelet.real)
     # coeff = np.zeros((3, shape[0], shape[2]))
     # Awvlet = np.abs(wvlet.wavelet)
     # fringe_wvlet = np.zeros(shape, dtype=complex)
 
     # for ii in range(shape[0]):
```

### Comparing `fisspy-1.1.2/fisspy/preprocess/proc_gui.py` & `fisspy-1.1.3/fisspy/preprocess/proc_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1946,21 +1946,21 @@
         self.B_s3_2_simple.setEnabled(True)
 
     def s3_2_wvShow(self):
         self.ax_sub[1][0].set_visible(True)
         self.ax_sub[1][1].set_visible(False)
         nfreq = self.wvlet_y[self.frameNum].wavelet.shape[1]
         self.ax_sub[1][0].cla()
-        data = np.abs(self.wvlet_y[self.frameNum].wavelet).mean((0,2))
+        data = np.abs(self.wvlet_y[self.frameNum].power).mean((0,2))
         ymax = data[:nfreq-10].max()*1.1
         self.ax_sub[1][0].plot(data)
         self.ax_sub[1][0].set_ylim(0,ymax)
         self.ax_sub[1][0].set_xlim(-0.5, nfreq-1)
         self.ax_sub[1][0].set_xlabel('freq_y (pix)')
-        self.ax_sub[1][0].set_ylabel('Amplitude')
+        self.ax_sub[1][0].set_ylabel('Power (DN$^2$)')
         self.ax_sub[1][0].set_title('Averaged Wavelet Spectrum (y-dir)')
         self.pFRmin_y = self.ax_sub[1][0].plot([self.yf_min, self.yf_min], [0, ymax], color='r', ls='dashed')[0]
         self.pFRmax_y = self.ax_sub[1][0].plot([self.yf_max, self.yf_max], [0, ymax], color='r', ls='dashed')[0]
         self.fig.canvas.draw_idle()
 
     def s3_2_FRapply(self):
         self.yf_min = int(self.LE_s3_2_FRmin.text())
@@ -2282,15 +2282,15 @@
             self.wvlet_x[i] = Wavelet(dd, dt=1, axis=1, dj=0.05, param=12)
             data = np.abs(self.wvlet_x[i].wavelet).mean((0,2))
             xwh[i] = data[:-25].argmax()
             hmax = data[:-25].max()/2
             t = x[data[xwh[i]-7:xwh[i]+7] >= hmax]
             w[i] = (t.max() - t.min())/2
 
-        self.xF_hw = int(w.mean()*4)
+        self.xF_hw = int(w.mean()*2)
         self.xF_c = int(xwh.mean())
         self.xf_min = self.xF_c - self.xF_hw
         self.xf_max = self.xF_c + self.xF_hw
 
         self.log += "> Done.<br>"
         self._writeLog()
         self.s3_4_wvShow()
@@ -2304,26 +2304,26 @@
         self.s2Show = False
         self.ax_sub[3][0].set_visible(True)
         self.ax_sub[3][1].set_visible(False)
         nfreq = self.wvlet_x[self.frameNum].wavelet.shape[1]
         self.ax_sub[3][0].cla()
         self.pwvGx = None
         
-        data = np.abs(self.wvlet_x[self.frameNum].wavelet).mean((0,2))
+        data = np.abs(self.wvlet_x[self.frameNum].power).mean((0,2))
         # xwh = data[:nfreq-20].argmax()
         self.xf_min = self.xF_c - self.xF_hw
         self.xf_max = self.xF_c + self.xF_hw
         self.LE_s3_4_FRmin.setText(f"{self.xf_min}")
         self.LE_s3_4_FRmax.setText(f"{self.xf_max}")
         ymax = data[:nfreq-10].max()*1.1
         self.pwvx = self.ax_sub[3][0].plot(data)[0]
         self.ax_sub[3][0].set_ylim(0,ymax)
         self.ax_sub[3][0].set_xlim(-0.5, nfreq-1)
         self.ax_sub[3][0].set_xlabel('Freq_x (pix)')
-        self.ax_sub[3][0].set_ylabel('Amplitude')
+        self.ax_sub[3][0].set_ylabel('Power (DN$^2$)')
         self.ax_sub[3][0].set_title('Averaged Wavelet Spectrum (x-dir)')
         self.pFRmin_x = self.ax_sub[3][0].plot([self.xf_min, self.xf_min], [0, ymax], color='r', ls='dashed')[0]
         self.pFRmax_x = self.ax_sub[3][0].plot([self.xf_max, self.xf_max], [0, ymax], color='r', ls='dashed')[0]
         if self.xGauss:
             if self.pwvGx is None:
                 self.pwvGx = self.ax_sub[3][0].plot(self.xF_mwv[self.frameNum])[0]
             else:
@@ -2497,15 +2497,15 @@
             self.imFx.set_data(data)
         elif self.s2Show:
             data = self.s2[self.frameNum][5:-5,5:-5]
             self.imFx.set_data(data)
         elif self.xwvShow:
             self.ax_sub[3][0].set_visible(True)
             self.ax_sub[3][1].set_visible(False)
-            data = np.abs(self.wvlet_x[self.frameNum].wavelet).mean((0,2))
+            data = np.abs(self.wvlet_x[self.frameNum].power).mean((0,2))
             self.pwvx.set_ydata(data)
             if self.xGauss:
                 if self.pwvGx is None:
                     self.pwvGx = self.ax_sub[3][0].plot(self.xF_mwv[self.frameNum])[0]
                 else:
                     self.pwvGx.set_ydata(self.xF_mwv[self.frameNum])
         else:
```

### Comparing `fisspy-1.1.2/fisspy/preprocess/t_y_sh.py` & `fisspy-1.1.3/fisspy/preprocess/t_y_sh.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/read/read_factory.py` & `fisspy-1.1.3/fisspy/read/read_factory.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy/read/readbase.py` & `fisspy-1.1.3/fisspy/read/readbase.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/fisspy.egg-info/PKG-INFO` & `fisspy-1.1.3/fisspy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisspy
-Version: 1.1.2
+Version: 1.1.3
 Summary: fisspy: Python analysis tools for GST/FISS
 Home-page: http://fiss.snu.ac.kr
 Author: Juhyung Kang
 Author-email: jhkang@astro.snu.ac.kr
 License: BSD-2
 Requires-Python: >=3.6
 License-File: LICENSE.txt
```

### Comparing `fisspy-1.1.2/fisspy.egg-info/SOURCES.txt` & `fisspy-1.1.3/fisspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.2/setup.py` & `fisspy-1.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fisspy',
-    version='1.1.2',
+    version='1.1.3',
     description='fisspy: Python analysis tools for GST/FISS',
     url='http://fiss.snu.ac.kr',
     author='Juhyung Kang',
     author_email='jhkang@astro.snu.ac.kr',
     license='BSD-2',
     python_requires='>=3.6',
     packages=find_packages(exclude=['docs', 'logo']),
```

