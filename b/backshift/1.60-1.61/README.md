# Comparing `tmp/backshift-1.60.tar.gz` & `tmp/backshift-1.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backshift-1.60.tar", last modified: Wed May 29 17:26:16 2024, max compression
+gzip compressed data, was "backshift-1.61.tar", last modified: Wed May 29 17:59:52 2024, max compression
```

## Comparing `backshift-1.60.tar` & `backshift-1.61.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)        0 2024-05-29 17:26:16.140455 backshift-1.60/
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     2003 2024-05-29 17:26:16.140455 backshift-1.60/PKG-INFO
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)      655 2021-10-25 04:59:28.000000 backshift-1.60/backshift
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     4219 2021-10-25 04:59:28.000000 backshift-1.60/backshift-extracts
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     2509 2021-10-25 04:59:28.000000 backshift-1.60/backshift-one
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1461 2021-10-25 04:59:28.000000 backshift-1.60/backshift-recent-backup-id
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     3381 2022-11-23 04:36:34.000000 backshift-1.60/backshift-verify-file
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     7406 2022-11-23 04:36:34.000000 backshift-1.60/backshift-verify-filesystem
-drwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)        0 2024-05-29 17:26:16.140455 backshift-1.60/backshift.egg-info/
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     2003 2024-05-29 17:26:16.000000 backshift-1.60/backshift.egg-info/PKG-INFO
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      785 2024-05-29 17:26:16.000000 backshift-1.60/backshift.egg-info/SOURCES.txt
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)        1 2024-05-29 17:26:16.000000 backshift-1.60/backshift.egg-info/dependency_links.txt
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)       40 2024-05-29 17:26:16.000000 backshift-1.60/backshift.egg-info/requires.txt
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      364 2024-05-29 17:26:16.000000 backshift-1.60/backshift.egg-info/top_level.txt
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    16262 2021-10-25 04:59:28.000000 backshift-1.60/backshift_file_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     1921 2021-10-25 04:59:28.000000 backshift-1.60/backshift_os_mod.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1803 2021-10-25 05:04:57.000000 backshift-1.60/base255.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    20670 2022-11-23 04:36:37.000000 backshift-1.60/bloom_filter_mod.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    10906 2021-10-25 05:04:58.000000 backshift-1.60/bufsock.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     8353 2021-10-25 04:59:28.000000 backshift-1.60/cacher_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     5784 2021-10-25 04:59:28.000000 backshift-1.60/chunk_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      507 2021-10-25 04:59:28.000000 backshift-1.60/comma_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3390 2021-10-25 04:59:28.000000 backshift-1.60/compressed_file_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3233 2023-11-11 04:50:47.000000 backshift-1.60/compressed_string_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     2300 2021-10-25 04:59:28.000000 backshift-1.60/constants_mod.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    15570 2021-10-25 05:04:59.000000 backshift-1.60/count
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     1147 2021-10-25 04:59:28.000000 backshift-1.60/db_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     4338 2021-10-25 04:59:28.000000 backshift-1.60/dirops_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     8871 2022-11-23 04:36:35.000000 backshift-1.60/dohdbm.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3021 2021-10-25 04:59:28.000000 backshift-1.60/escape_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    10731 2021-10-25 04:59:28.000000 backshift-1.60/expire_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      407 2021-10-25 04:59:28.000000 backshift-1.60/file_count_mod.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1344 2021-10-25 04:59:28.000000 backshift-1.60/get_chunk.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     7274 2021-10-25 04:59:28.000000 backshift-1.60/hardlinks_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      543 2021-10-25 04:59:28.000000 backshift-1.60/helpers.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    32195 2021-10-25 04:59:28.000000 backshift-1.60/main.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    10731 2021-10-25 04:59:28.000000 backshift-1.60/metadata_mod.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    19157 2022-11-23 04:36:37.000000 backshift-1.60/modunits.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     6967 2021-10-25 05:04:57.000000 backshift-1.60/readline0.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    31969 2024-05-28 20:58:55.000000 backshift-1.60/repo_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     4388 2021-10-25 04:59:28.000000 backshift-1.60/saveset_files_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    14689 2021-10-25 04:59:28.000000 backshift-1.60/saveset_summary_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)       38 2024-05-29 17:26:16.140455 backshift-1.60/setup.cfg
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3702 2024-05-29 17:24:13.000000 backshift-1.60/setup.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1803 2021-11-15 02:12:43.000000 backshift-1.60/sshfs-backup
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)      352 2021-10-25 04:59:28.000000 backshift-1.60/stringio.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1482 2021-10-25 04:59:28.000000 backshift-1.60/strip-components
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     2680 2023-07-09 17:16:50.000000 backshift-1.60/touch.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    17647 2021-10-25 05:04:58.000000 backshift-1.60/xz_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      989 2023-11-11 17:14:48.000000 backshift-1.60/zst_mod.py
+drwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)        0 2024-05-29 17:59:52.424043 backshift-1.61/
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     2003 2024-05-29 17:59:52.424043 backshift-1.61/PKG-INFO
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)      655 2021-10-25 04:59:28.000000 backshift-1.61/backshift
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     4219 2021-10-25 04:59:28.000000 backshift-1.61/backshift-extracts
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     2509 2021-10-25 04:59:28.000000 backshift-1.61/backshift-one
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1461 2021-10-25 04:59:28.000000 backshift-1.61/backshift-recent-backup-id
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     3381 2022-11-23 04:36:34.000000 backshift-1.61/backshift-verify-file
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     7406 2022-11-23 04:36:34.000000 backshift-1.61/backshift-verify-filesystem
+drwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)        0 2024-05-29 17:59:52.424043 backshift-1.61/backshift.egg-info/
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     2003 2024-05-29 17:59:52.000000 backshift-1.61/backshift.egg-info/PKG-INFO
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      802 2024-05-29 17:59:52.000000 backshift-1.61/backshift.egg-info/SOURCES.txt
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)        1 2024-05-29 17:59:52.000000 backshift-1.61/backshift.egg-info/dependency_links.txt
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)       40 2024-05-29 17:59:52.000000 backshift-1.61/backshift.egg-info/requires.txt
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      378 2024-05-29 17:59:52.000000 backshift-1.61/backshift.egg-info/top_level.txt
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    16262 2021-10-25 04:59:28.000000 backshift-1.61/backshift_file_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     1921 2021-10-25 04:59:28.000000 backshift-1.61/backshift_os_mod.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1803 2021-10-25 05:04:57.000000 backshift-1.61/base255.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    20670 2022-11-23 04:36:37.000000 backshift-1.61/bloom_filter_mod.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    10906 2021-10-25 05:04:58.000000 backshift-1.61/bufsock.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     8353 2021-10-25 04:59:28.000000 backshift-1.61/cacher_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     5784 2021-10-25 04:59:28.000000 backshift-1.61/chunk_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      507 2021-10-25 04:59:28.000000 backshift-1.61/comma_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3390 2021-10-25 04:59:28.000000 backshift-1.61/compressed_file_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3233 2023-11-11 04:50:47.000000 backshift-1.61/compressed_string_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     2300 2021-10-25 04:59:28.000000 backshift-1.61/constants_mod.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    15570 2021-10-25 05:04:59.000000 backshift-1.61/count
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     1147 2021-10-25 04:59:28.000000 backshift-1.61/db_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     4338 2021-10-25 04:59:28.000000 backshift-1.61/dirops_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     8871 2022-11-23 04:36:35.000000 backshift-1.61/dohdbm.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3021 2021-10-25 04:59:28.000000 backshift-1.61/escape_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    10731 2021-10-25 04:59:28.000000 backshift-1.61/expire_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      407 2021-10-25 04:59:28.000000 backshift-1.61/file_count_mod.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1344 2021-10-25 04:59:28.000000 backshift-1.61/get_chunk.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     7274 2021-10-25 04:59:28.000000 backshift-1.61/hardlinks_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      543 2021-10-25 04:59:28.000000 backshift-1.61/helpers.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    32195 2021-10-25 04:59:28.000000 backshift-1.61/main.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    10731 2021-10-25 04:59:28.000000 backshift-1.61/metadata_mod.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    19157 2022-11-23 04:36:37.000000 backshift-1.61/modunits.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     6967 2021-10-25 05:04:57.000000 backshift-1.61/readline0.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    31969 2024-05-28 20:58:55.000000 backshift-1.61/repo_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     4388 2021-10-25 04:59:28.000000 backshift-1.61/saveset_files_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    14689 2021-10-25 04:59:28.000000 backshift-1.61/saveset_summary_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)       38 2024-05-29 17:59:52.424043 backshift-1.61/setup.cfg
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3727 2024-05-29 17:56:50.000000 backshift-1.61/setup.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1803 2021-11-15 02:12:43.000000 backshift-1.61/sshfs-backup
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)      352 2021-10-25 04:59:28.000000 backshift-1.61/stringio.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1482 2021-10-25 04:59:28.000000 backshift-1.61/strip-components
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     2680 2023-07-09 17:16:50.000000 backshift-1.61/touch.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    17647 2021-10-25 05:04:58.000000 backshift-1.61/xz_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      989 2023-11-11 17:14:48.000000 backshift-1.61/zst_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      436 2023-11-11 04:50:50.000000 backshift-1.61/zst_zstandard.py
```

### Comparing `backshift-1.60/PKG-INFO` & `backshift-1.61/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backshift
-Version: 1.60
+Version: 1.61
 Summary: Filesystem to filesystem backup (deduplicated, compressed)
 Home-page: http://stromberg.dnsalias.org/~strombrg/backshift/
 Author: Daniel Richard Stromberg
 Author-email: strombrg@gmail.com
 License: GPL, MIT, UCI, Apache (all opensource)
 Platform: Cross platform
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `backshift-1.60/backshift` & `backshift-1.61/backshift`

 * *Files identical despite different names*

### Comparing `backshift-1.60/backshift-extracts` & `backshift-1.61/backshift-extracts`

 * *Files identical despite different names*

### Comparing `backshift-1.60/backshift-one` & `backshift-1.61/backshift-one`

 * *Files identical despite different names*

### Comparing `backshift-1.60/backshift-recent-backup-id` & `backshift-1.61/backshift-recent-backup-id`

 * *Files identical despite different names*

### Comparing `backshift-1.60/backshift-verify-file` & `backshift-1.61/backshift-verify-file`

 * *Files identical despite different names*

### Comparing `backshift-1.60/backshift-verify-filesystem` & `backshift-1.61/backshift-verify-filesystem`

 * *Files identical despite different names*

### Comparing `backshift-1.60/backshift.egg-info/PKG-INFO` & `backshift-1.61/backshift.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backshift
-Version: 1.60
+Version: 1.61
 Summary: Filesystem to filesystem backup (deduplicated, compressed)
 Home-page: http://stromberg.dnsalias.org/~strombrg/backshift/
 Author: Daniel Richard Stromberg
 Author-email: strombrg@gmail.com
 License: GPL, MIT, UCI, Apache (all opensource)
 Platform: Cross platform
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `backshift-1.60/backshift.egg-info/SOURCES.txt` & `backshift-1.61/backshift.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,12 +35,13 @@
 setup.py
 sshfs-backup
 stringio.py
 strip-components
 touch.py
 xz_mod.py
 zst_mod.py
+zst_zstandard.py
 backshift.egg-info/PKG-INFO
 backshift.egg-info/SOURCES.txt
 backshift.egg-info/dependency_links.txt
 backshift.egg-info/requires.txt
 backshift.egg-info/top_level.txt
```

### Comparing `backshift-1.60/backshift_file_mod.py` & `backshift-1.61/backshift_file_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/backshift_os_mod.py` & `backshift-1.61/backshift_os_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/base255.py` & `backshift-1.61/base255.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/bloom_filter_mod.py` & `backshift-1.61/bloom_filter_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/bufsock.py` & `backshift-1.61/bufsock.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/cacher_mod.py` & `backshift-1.61/cacher_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/chunk_mod.py` & `backshift-1.61/chunk_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/compressed_file_mod.py` & `backshift-1.61/compressed_file_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/compressed_string_mod.py` & `backshift-1.61/compressed_string_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/constants_mod.py` & `backshift-1.61/constants_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/count` & `backshift-1.61/count`

 * *Files identical despite different names*

### Comparing `backshift-1.60/db_mod.py` & `backshift-1.61/db_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/dirops_mod.py` & `backshift-1.61/dirops_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/dohdbm.py` & `backshift-1.61/dohdbm.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/escape_mod.py` & `backshift-1.61/escape_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/expire_mod.py` & `backshift-1.61/expire_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/get_chunk.py` & `backshift-1.61/get_chunk.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/hardlinks_mod.py` & `backshift-1.61/hardlinks_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/helpers.py` & `backshift-1.61/helpers.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/main.py` & `backshift-1.61/main.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/metadata_mod.py` & `backshift-1.61/metadata_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/modunits.py` & `backshift-1.61/modunits.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/readline0.py` & `backshift-1.61/readline0.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/repo_mod.py` & `backshift-1.61/repo_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/saveset_files_mod.py` & `backshift-1.61/saveset_files_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/saveset_summary_mod.py` & `backshift-1.61/saveset_summary_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/setup.py` & `backshift-1.61/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 """Package up backshift for Pypi."""
 
 import os
 import distutils.core
 
-version = '1.60'
+version = '1.61'
 
 
 def unlinker(filename):
     """Delete a file. Do not error if there is a problem doing so."""
     try:
         os.unlink(filename)
     except (OSError, IOError):
@@ -50,14 +50,15 @@
         'repo_mod',
         'saveset_files_mod',
         'saveset_summary_mod',
         'stringio',
         'touch',
         'xz_mod',
         'zst_mod',
+        'zst_zstandard',
         ],
     version=version,
     description='Filesystem to filesystem backup (deduplicated, compressed)',
     long_description="""
 Backshift is a filesystem to filesystem backup program, analogous to rsync --link-dest.
 
 Compared to rsync, backshift deduplicates much better, and compresses files - rsync does not.
```

### Comparing `backshift-1.60/sshfs-backup` & `backshift-1.61/sshfs-backup`

 * *Files identical despite different names*

### Comparing `backshift-1.60/strip-components` & `backshift-1.61/strip-components`

 * *Files identical despite different names*

### Comparing `backshift-1.60/touch.py` & `backshift-1.61/touch.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/xz_mod.py` & `backshift-1.61/xz_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.60/zst_mod.py` & `backshift-1.61/zst_mod.py`

 * *Files identical despite different names*

