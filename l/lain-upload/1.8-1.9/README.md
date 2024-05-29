# Comparing `tmp/lain_upload-1.8.tar.gz` & `tmp/lain_upload-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lain_upload-1.8.tar", last modified: Tue Feb 20 14:13:50 2024, max compression
+gzip compressed data, was "lain_upload-1.9.tar", last modified: Wed Feb 21 00:53:02 2024, max compression
```

## Comparing `lain_upload-1.8.tar` & `lain_upload-1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:13:50.919335 lain_upload-1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-02-20 14:13:40.000000 lain_upload-1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-20 14:13:50.919335 lain_upload-1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-20 14:13:40.000000 lain_upload-1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:13:50.915335 lain_upload-1.8/lain_upload/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-20 14:13:40.000000 lain_upload-1.8/lain_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-20 14:13:40.000000 lain_upload-1.8/lain_upload/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-02-20 14:13:40.000000 lain_upload-1.8/lain_upload/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:13:50.919335 lain_upload-1.8/lain_upload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-20 14:13:50.000000 lain_upload-1.8/lain_upload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-20 14:13:50.000000 lain_upload-1.8/lain_upload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 14:13:50.000000 lain_upload-1.8/lain_upload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-20 14:13:50.000000 lain_upload-1.8/lain_upload.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-20 14:13:50.000000 lain_upload-1.8/lain_upload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-20 14:13:50.000000 lain_upload-1.8/lain_upload.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 14:13:50.919335 lain_upload-1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-20 14:13:40.000000 lain_upload-1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:53:02.393466 lain_upload-1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-02-21 00:52:44.000000 lain_upload-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-21 00:53:02.389465 lain_upload-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-21 00:52:44.000000 lain_upload-1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:53:02.389465 lain_upload-1.9/lain_upload/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-21 00:52:44.000000 lain_upload-1.9/lain_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-21 00:52:44.000000 lain_upload-1.9/lain_upload/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-02-21 00:52:44.000000 lain_upload-1.9/lain_upload/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:53:02.389465 lain_upload-1.9/lain_upload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-21 00:53:02.000000 lain_upload-1.9/lain_upload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-21 00:53:02.000000 lain_upload-1.9/lain_upload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 00:53:02.000000 lain_upload-1.9/lain_upload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-21 00:53:02.000000 lain_upload-1.9/lain_upload.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-21 00:53:02.000000 lain_upload-1.9/lain_upload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-21 00:53:02.000000 lain_upload-1.9/lain_upload.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 00:53:02.393466 lain_upload-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-21 00:52:44.000000 lain_upload-1.9/setup.py
```

### Comparing `lain_upload-1.8/LICENSE` & `lain_upload-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lain_upload-1.8/PKG-INFO` & `lain_upload-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lain_upload
-Version: 1.8
+Version: 1.9
 Summary: pomf.lain.la uploader.
 Home-page: https://github.com/NecRaul/lain.la-pomf-uploader
 Author: NecRaul
 Project-URL: Documentation, https://github.com/NecRaul/lain.la-pomf-uploader#readme
 Project-URL: Source, https://github.com/NecRaul/lain.la-pomf-uploader
 Keywords: python,uploader,pomf,lain,lain.la,pomf.lain.la
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lain_upload-1.8/README.md` & `lain_upload-1.9/README.md`

 * *Files identical despite different names*

### Comparing `lain_upload-1.8/lain_upload/upload.py` & `lain_upload-1.9/lain_upload/upload.py`

 * *Files identical despite different names*

### Comparing `lain_upload-1.8/lain_upload.egg-info/PKG-INFO` & `lain_upload-1.9/lain_upload.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lain_upload
-Version: 1.8
+Version: 1.9
 Summary: pomf.lain.la uploader.
 Home-page: https://github.com/NecRaul/lain.la-pomf-uploader
 Author: NecRaul
 Project-URL: Documentation, https://github.com/NecRaul/lain.la-pomf-uploader#readme
 Project-URL: Source, https://github.com/NecRaul/lain.la-pomf-uploader
 Keywords: python,uploader,pomf,lain,lain.la,pomf.lain.la
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lain_upload-1.8/setup.py` & `lain_upload-1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.8"
+VERSION = "1.9"
 DESCRIPTION = "pomf.lain.la uploader."
 with open("README.md", "r") as file:
     LONG_DESCRIPTION = file.read()
 AUTHOR = "NecRaul"
 
 setup(
     name="lain_upload",
```

