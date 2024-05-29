# Comparing `tmp/backshift-1.55.tar.gz` & `tmp/backshift-1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backshift-1.55.tar", last modified: Wed Nov 23 04:39:21 2022, max compression
+gzip compressed data, was "backshift-1.60.tar", last modified: Wed May 29 17:26:16 2024, max compression
```

## Comparing `backshift-1.55.tar` & `backshift-1.60.tar`

### file list

```diff
@@ -1,42 +1,50 @@
-drwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)        0 2022-11-23 04:39:21.126777 backshift-1.55/
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     2248 2022-11-23 04:39:21.126777 backshift-1.55/PKG-INFO
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)      655 2021-10-25 04:59:28.552517 backshift-1.55/backshift
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     4219 2021-10-25 04:59:28.552517 backshift-1.55/backshift-extracts
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     2509 2021-10-25 04:59:28.552517 backshift-1.55/backshift-one
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1461 2021-10-25 04:59:28.556517 backshift-1.55/backshift-recent-backup-id
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     3381 2022-11-23 04:36:34.128761 backshift-1.55/backshift-verify-file
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     7406 2022-11-23 04:36:34.128761 backshift-1.55/backshift-verify-filesystem
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    16262 2021-10-25 04:59:28.556517 backshift-1.55/backshift_file_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     1921 2021-10-25 04:59:28.556517 backshift-1.55/backshift_os_mod.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1803 2021-10-25 05:04:57.171524 backshift-1.55/base255.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    20670 2022-11-23 04:36:37.184798 backshift-1.55/bloom_filter_mod.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    10906 2021-10-25 05:04:58.139541 backshift-1.55/bufsock.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     8353 2021-10-25 04:59:28.552517 backshift-1.55/cacher_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     5784 2021-10-25 04:59:28.620518 backshift-1.55/chunk_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      507 2021-10-25 04:59:28.556517 backshift-1.55/comma_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3390 2021-10-25 04:59:28.556517 backshift-1.55/compressed_file_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3366 2021-10-25 04:59:28.588517 backshift-1.55/compressed_string_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     2300 2021-10-25 04:59:28.556517 backshift-1.55/constants_mod.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    15570 2021-10-25 05:04:59.315562 backshift-1.55/count
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     1147 2021-10-25 04:59:28.556517 backshift-1.55/db_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     4338 2021-10-25 04:59:28.588517 backshift-1.55/dirops_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     8871 2022-11-23 04:36:35.004772 backshift-1.55/dohdbm.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3021 2021-10-25 04:59:28.588517 backshift-1.55/escape_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    10731 2021-10-25 04:59:28.588517 backshift-1.55/expire_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      407 2021-10-25 04:59:28.588517 backshift-1.55/file_count_mod.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1344 2021-10-25 04:59:28.592517 backshift-1.55/get_chunk.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     7274 2021-10-25 04:59:28.644518 backshift-1.55/hardlinks_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      543 2021-10-25 04:59:28.592517 backshift-1.55/helpers.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    32195 2021-10-25 04:59:28.592517 backshift-1.55/main.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    10731 2021-10-25 04:59:28.592517 backshift-1.55/metadata_mod.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    19157 2022-11-23 04:36:37.400801 backshift-1.55/modunits.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     6967 2021-10-25 05:04:57.931537 backshift-1.55/readline0.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    31969 2021-10-25 04:59:28.748519 backshift-1.55/repo_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     4388 2021-10-25 04:59:28.748519 backshift-1.55/saveset_files_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    14689 2021-10-25 04:59:28.676518 backshift-1.55/saveset_summary_mod.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3670 2022-11-23 04:38:25.758111 backshift-1.55/setup.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1803 2021-11-15 02:12:43.546482 backshift-1.55/sshfs-backup
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)      352 2021-10-25 04:59:28.676518 backshift-1.55/stringio.py
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1482 2021-10-25 04:59:28.664518 backshift-1.55/strip-components
--rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     2555 2022-11-23 04:36:38.236811 backshift-1.55/touch.py
--rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    17647 2021-10-25 05:04:58.347545 backshift-1.55/xz_mod.py
+drwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)        0 2024-05-29 17:26:16.140455 backshift-1.60/
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     2003 2024-05-29 17:26:16.140455 backshift-1.60/PKG-INFO
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)      655 2021-10-25 04:59:28.000000 backshift-1.60/backshift
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     4219 2021-10-25 04:59:28.000000 backshift-1.60/backshift-extracts
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     2509 2021-10-25 04:59:28.000000 backshift-1.60/backshift-one
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1461 2021-10-25 04:59:28.000000 backshift-1.60/backshift-recent-backup-id
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     3381 2022-11-23 04:36:34.000000 backshift-1.60/backshift-verify-file
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     7406 2022-11-23 04:36:34.000000 backshift-1.60/backshift-verify-filesystem
+drwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)        0 2024-05-29 17:26:16.140455 backshift-1.60/backshift.egg-info/
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     2003 2024-05-29 17:26:16.000000 backshift-1.60/backshift.egg-info/PKG-INFO
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      785 2024-05-29 17:26:16.000000 backshift-1.60/backshift.egg-info/SOURCES.txt
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)        1 2024-05-29 17:26:16.000000 backshift-1.60/backshift.egg-info/dependency_links.txt
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)       40 2024-05-29 17:26:16.000000 backshift-1.60/backshift.egg-info/requires.txt
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      364 2024-05-29 17:26:16.000000 backshift-1.60/backshift.egg-info/top_level.txt
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    16262 2021-10-25 04:59:28.000000 backshift-1.60/backshift_file_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     1921 2021-10-25 04:59:28.000000 backshift-1.60/backshift_os_mod.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1803 2021-10-25 05:04:57.000000 backshift-1.60/base255.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    20670 2022-11-23 04:36:37.000000 backshift-1.60/bloom_filter_mod.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    10906 2021-10-25 05:04:58.000000 backshift-1.60/bufsock.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     8353 2021-10-25 04:59:28.000000 backshift-1.60/cacher_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     5784 2021-10-25 04:59:28.000000 backshift-1.60/chunk_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      507 2021-10-25 04:59:28.000000 backshift-1.60/comma_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3390 2021-10-25 04:59:28.000000 backshift-1.60/compressed_file_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3233 2023-11-11 04:50:47.000000 backshift-1.60/compressed_string_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     2300 2021-10-25 04:59:28.000000 backshift-1.60/constants_mod.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    15570 2021-10-25 05:04:59.000000 backshift-1.60/count
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     1147 2021-10-25 04:59:28.000000 backshift-1.60/db_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     4338 2021-10-25 04:59:28.000000 backshift-1.60/dirops_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     8871 2022-11-23 04:36:35.000000 backshift-1.60/dohdbm.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3021 2021-10-25 04:59:28.000000 backshift-1.60/escape_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    10731 2021-10-25 04:59:28.000000 backshift-1.60/expire_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      407 2021-10-25 04:59:28.000000 backshift-1.60/file_count_mod.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1344 2021-10-25 04:59:28.000000 backshift-1.60/get_chunk.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     7274 2021-10-25 04:59:28.000000 backshift-1.60/hardlinks_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      543 2021-10-25 04:59:28.000000 backshift-1.60/helpers.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    32195 2021-10-25 04:59:28.000000 backshift-1.60/main.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    10731 2021-10-25 04:59:28.000000 backshift-1.60/metadata_mod.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)    19157 2022-11-23 04:36:37.000000 backshift-1.60/modunits.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     6967 2021-10-25 05:04:57.000000 backshift-1.60/readline0.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    31969 2024-05-28 20:58:55.000000 backshift-1.60/repo_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     4388 2021-10-25 04:59:28.000000 backshift-1.60/saveset_files_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    14689 2021-10-25 04:59:28.000000 backshift-1.60/saveset_summary_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)       38 2024-05-29 17:26:16.140455 backshift-1.60/setup.cfg
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)     3702 2024-05-29 17:24:13.000000 backshift-1.60/setup.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1803 2021-11-15 02:12:43.000000 backshift-1.60/sshfs-backup
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)      352 2021-10-25 04:59:28.000000 backshift-1.60/stringio.py
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     1482 2021-10-25 04:59:28.000000 backshift-1.60/strip-components
+-rwxr-xr-x   0 dstromberg  (1000) dstromberg  (1000)     2680 2023-07-09 17:16:50.000000 backshift-1.60/touch.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)    17647 2021-10-25 05:04:58.000000 backshift-1.60/xz_mod.py
+-rw-r--r--   0 dstromberg  (1000) dstromberg  (1000)      989 2023-11-11 17:14:48.000000 backshift-1.60/zst_mod.py
```

### Comparing `backshift-1.55/PKG-INFO` & `backshift-1.60/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: backshift
-Version: 1.55
-Summary: Filesystem to filesystem backup (deduplicated, compressed with xz)
+Version: 1.60
+Summary: Filesystem to filesystem backup (deduplicated, compressed)
 Home-page: http://stromberg.dnsalias.org/~strombrg/backshift/
 Author: Daniel Richard Stromberg
 Author-email: strombrg@gmail.com
 License: GPL, MIT, UCI, Apache (all opensource)
-Description: 
-        Backshift is a filesystem to filesystem backup program, analogous to rsync --link-dest.
-        
-        Compared to rsync, backshift deduplicates much better, and compresses files - rsync does not.
-        
-        Backshift also allows easy removal of old backups, despite its strong deduplication and compression.
-        
-        Files to back up are selected using something like 'find / -xdev -print0' and piping that to backshift.
-        
-        Files are restored by piping to 'tar xfp'.
-        
-        Metadata is partially compressed.  Each directory's metadata is compressed separately for easy
-        partial restores.
-        
-        Content-based, variable length chunks are deduplicated - so simply inserting a byte at a random place in a large file
-        is not going to require backing up the entire file anew.
-        
-        Backshift runs on CPython 3.x and Pypy3.  It may run on nuitka - backshift+nuitka has not been tested much.
-        
-        On many modern systems, Backshift runs fastest on Pypy, but on some (older?) machines you may be better off with
-        CPython 3.x plus the Cython versions of treap and rolling_checksum_mod.
-        
-        For pypy, simply install backshift with pip.  This should give you a pure-python version of backshift that pypy likes.
-        For CPython+Cython, first install backshift with pip just as you would for pypy.  Then additionally install pyx-treap
-        and rolling-checksum-pyx-mod with pip - for a speed boost.
-        
-        Backshift is not as fast as rsync --link-dest; rsync does not have to do as much work to accomplish what it sets out
-        to do.  But if you are paying for your storage, backshift will probably be significantly cheaper.
-        
 Platform: Cross platform
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
+
+
+Backshift is a filesystem to filesystem backup program, analogous to rsync --link-dest.
+
+Compared to rsync, backshift deduplicates much better, and compresses files - rsync does not.
+
+Backshift also allows easy removal of old backups, despite its strong deduplication and compression.
+
+Files to back up are selected using something like 'find / -xdev -print0' and piping that to backshift.
+
+Files are restored by piping to 'tar xfp'.
+
+Metadata is partially compressed.  Each directory's metadata is compressed separately for easy
+partial restores.
+
+Content-based, variable length chunks are deduplicated - so simply inserting a byte at a random place in a large file
+is not going to require backing up the entire file anew.
+
+Backshift runs on CPython 3.x and Pypy3.  It may run on nuitka - backshift+nuitka has not been tested much.
+
+On many modern systems, Backshift runs fastest on Pypy, but on some (older?) machines you may be better off with
+CPython 3.x plus the Cython versions of treap and rolling_checksum_mod.
+
+For pypy, simply install backshift with pip.  This should give you a pure-python version of backshift that pypy likes.
+For CPython+Cython, first install backshift with pip just as you would for pypy.  Then additionally install pyx-treap
+and rolling-checksum-pyx-mod with pip - for a speed boost.
+
+Backshift is not as fast as rsync --link-dest; rsync does not have to do as much work to accomplish what it sets out
+to do.  But if you are paying for your storage, backshift will probably be significantly cheaper.
```

### Comparing `backshift-1.55/backshift` & `backshift-1.60/backshift`

 * *Files identical despite different names*

### Comparing `backshift-1.55/backshift-extracts` & `backshift-1.60/backshift-extracts`

 * *Files identical despite different names*

### Comparing `backshift-1.55/backshift-one` & `backshift-1.60/backshift-one`

 * *Files identical despite different names*

### Comparing `backshift-1.55/backshift-recent-backup-id` & `backshift-1.60/backshift-recent-backup-id`

 * *Files identical despite different names*

### Comparing `backshift-1.55/backshift-verify-file` & `backshift-1.60/backshift-verify-file`

 * *Files identical despite different names*

### Comparing `backshift-1.55/backshift-verify-filesystem` & `backshift-1.60/backshift-verify-filesystem`

 * *Files identical despite different names*

### Comparing `backshift-1.55/backshift_file_mod.py` & `backshift-1.60/backshift_file_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/backshift_os_mod.py` & `backshift-1.60/backshift_os_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/base255.py` & `backshift-1.60/base255.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/bloom_filter_mod.py` & `backshift-1.60/bloom_filter_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/bufsock.py` & `backshift-1.60/bufsock.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/cacher_mod.py` & `backshift-1.60/cacher_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/chunk_mod.py` & `backshift-1.60/chunk_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/compressed_file_mod.py` & `backshift-1.60/compressed_file_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/compressed_string_mod.py` & `backshift-1.60/compressed_string_mod.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 # 1: Not compressed
 # 2: Compressed with pack: .z
 # 3: Compressed with compress: .Z
 # 4: Compressed with gzip: .gz
 # 5: Compressed with bzip2: .bz2 (quite a bit slower than gzip, but packs harder)
 # 6: Compressed with xz -2: .xz (quite a bit faster than bz2, only a tiny bit larger)
 # 7: Compressed with xz -6: .xz (packs harder than bzip2, but slower)
+# 8: Compressed with zstandard: .zst (gives a balance of compression ratio and performance. Laughably faster than xz)
 #
 # Brotli may prove worth adding:
-# http://tech.slashdot.org/story/15/09/22/1723219/google-launches-brotli-a-new-open-source-compression-algorithm-for-the-web?utm_source=rss1.0mainlinkanon&utm_medium=feed
+# http://tech.slashdot.org/story/15/09/22/1723219/google-launches-brotli-a-new-open-source-compression-algorithm-for-the-web
 #
 # At this time, only 1, 5 and 7 are used
 
 import sys
 
 try:
     import bz2 as bz2_mod
@@ -25,28 +26,29 @@
 else:
     HAVE_BZ2 = True
 
 import constants_mod
 import helpers
 import stringio
 import xz_mod
+import zst_mod
 
 
 def compress_string(data, bz2_announced=False):
     """
     Compress a string.
 
-    1) If we have xz, try to use it.
+    1) If we have zstandard, try to use it.
     2) Fallback: if we have bz2, try to use that.
     3) Else save without compressing.
     4) Or if the compressed version is larger, save without compressing then too.
     """
     try:
-        compressed_data = xz_mod.compress(data)
-        compression_type = 7
+        compressed_data = zst_mod.compress(data)
+        compression_type = 8
         compressed_ok = True
     except OSError:
         if HAVE_BZ2:
             if not bz2_announced:
                 sys.stderr.write('%s: warning: falling back to bzip2 compression due to lack of xz\n' % sys.argv[0])
                 bz2_announced = True
             compressed_data = bz2_mod.compress(data)
@@ -61,32 +63,27 @@
         result = constants_mod.Constants.b_onenewline + data
     else:
         result = \
             helpers.string_to_binary('%d' % compression_type) + \
             constants_mod.Constants.b_newline + \
             compressed_data
 
-    # print('compress_string: len(result): %s' % len(result))
-    # print('compress_string: result[:10]: %s' % result[:10])
-
     binary_result = helpers.string_to_binary(result)
 
-    # print('compress_string: len(binary_result): %s' % len(binary_result))
-
     return binary_result
 
 
 def decompress_string(compressed_data, zero_length_ok=False):
     """Uncompress a string."""
-    # print('decompress_string: compressed_data: %d' % len(compressed_data))
     memory_file = stringio.StringIO(compressed_data)
     compression_type = memory_file.readline().rstrip()
     remainder = memory_file.read()
-    # print('decompress_string: remainder: %d' % len(remainder))
-    if compression_type == constants_mod.Constants.b_7:
+    if compression_type == constants_mod.Constants.b_8:
+        decompressed_data = zst_mod.decompress(remainder)
+    elif compression_type == constants_mod.Constants.b_7:
         decompressed_data = xz_mod.decompress(remainder)
     elif compression_type == constants_mod.Constants.b_5:
         decompressed_data = bz2_mod.decompress(remainder)
     elif compression_type == constants_mod.Constants.b_1:
         decompressed_data = remainder
     elif zero_length_ok and compression_type == helpers.empty_bytes:
         decompressed_data = helpers.empty_bytes
```

### Comparing `backshift-1.55/constants_mod.py` & `backshift-1.60/constants_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/count` & `backshift-1.60/count`

 * *Files identical despite different names*

### Comparing `backshift-1.55/db_mod.py` & `backshift-1.60/db_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/dirops_mod.py` & `backshift-1.60/dirops_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/dohdbm.py` & `backshift-1.60/dohdbm.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/escape_mod.py` & `backshift-1.60/escape_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/expire_mod.py` & `backshift-1.60/expire_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/get_chunk.py` & `backshift-1.60/get_chunk.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/hardlinks_mod.py` & `backshift-1.60/hardlinks_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/helpers.py` & `backshift-1.60/helpers.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/main.py` & `backshift-1.60/main.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/metadata_mod.py` & `backshift-1.60/metadata_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/modunits.py` & `backshift-1.60/modunits.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/readline0.py` & `backshift-1.60/readline0.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/repo_mod.py` & `backshift-1.60/repo_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/saveset_files_mod.py` & `backshift-1.60/saveset_files_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/saveset_summary_mod.py` & `backshift-1.60/saveset_summary_mod.py`

 * *Files identical despite different names*

### Comparing `backshift-1.55/setup.py` & `backshift-1.60/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 """Package up backshift for Pypi."""
 
 import os
 import distutils.core
 
-version = '1.55'
+version = '1.60'
 
 
 def unlinker(filename):
     """Delete a file. Do not error if there is a problem doing so."""
     try:
         os.unlink(filename)
     except (OSError, IOError):
@@ -49,17 +49,18 @@
         'readline0',
         'repo_mod',
         'saveset_files_mod',
         'saveset_summary_mod',
         'stringio',
         'touch',
         'xz_mod',
+        'zst_mod',
         ],
     version=version,
-    description='Filesystem to filesystem backup (deduplicated, compressed with xz)',
+    description='Filesystem to filesystem backup (deduplicated, compressed)',
     long_description="""
 Backshift is a filesystem to filesystem backup program, analogous to rsync --link-dest.
 
 Compared to rsync, backshift deduplicates much better, and compresses files - rsync does not.
 
 Backshift also allows easy removal of old backups, despite its strong deduplication and compression.
 
@@ -94,14 +95,15 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         ],
     install_requires=[
         'treap',
         'rolling-checksum-py-mod',
+        'zstandard',
         ],
     scripts=[
         'backshift',
         'backshift-extracts',
         'backshift-one',
         'backshift-recent-backup-id',
         'backshift-verify-file',
```

### Comparing `backshift-1.55/sshfs-backup` & `backshift-1.60/sshfs-backup`

 * *Files identical despite different names*

### Comparing `backshift-1.55/strip-components` & `backshift-1.60/strip-components`

 * *Files identical despite different names*

### Comparing `backshift-1.55/touch.py` & `backshift-1.60/touch.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 from pathlib import Path
 import sys
 import timeit
 
 
 def touch1(filename):
-    """Touch a file using pathlib - fastest on pypy3, and fastest overall."""
+    """Touch a file using pathlib - fastest on pypy3, and fastest overall - but has problems with non-UTF-8 filenames."""
     Path(filename).touch()
 
 
 def touch2(filename):
     """Touch a file using open+close."""
     open(filename, 'r+').close()
 
@@ -38,15 +38,16 @@
 def create_test_file(filename, size):
     """Create a test file at filename of size bytes."""
     with open(filename, 'w') as file_:
         file_.write('0' * size)
 
 
 if sys.implementation.name == 'pypy':
-    touch = touch1
+    # Second-fastest on Pypy, but works for all filenames, not just UTF-8 names.
+    touch = touch3
 elif sys.implementation.name == 'cpython':
     touch = touch3
 else:
     print('This does not appear to be pypy or cpython - using an unoptimized touch', file=sys.stderr)
     touch = touch4
```

### Comparing `backshift-1.55/xz_mod.py` & `backshift-1.60/xz_mod.py`

 * *Files identical despite different names*

