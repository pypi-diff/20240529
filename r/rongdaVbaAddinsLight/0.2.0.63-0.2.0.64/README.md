# Comparing `tmp/rongdaVbaAddinsLight-0.2.0.63.tar.gz` & `tmp/rongdaVbaAddinsLight-0.2.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rongdaVbaAddinsLight-0.2.0.63.tar", last modified: Mon May  6 08:27:41 2024, max compression
+gzip compressed data, was "rongdaVbaAddinsLight-0.2.0.64.tar", last modified: Wed May 29 08:52:49 2024, max compression
```

## Comparing `rongdaVbaAddinsLight-0.2.0.63.tar` & `rongdaVbaAddinsLight-0.2.0.64.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.645329 rongdaVbaAddinsLight-0.2.0.63/
--rw-rw-rw-   0        0        0        0 2023-10-11 02:09:37.000000 rongdaVbaAddinsLight-0.2.0.63/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdaVbaAddinsLight-0.2.0.63/MANIFEST.in
--rw-rw-rw-   0        0        0      405 2024-05-06 08:27:41.643332 rongdaVbaAddinsLight-0.2.0.63/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-10-11 02:09:37.000000 rongdaVbaAddinsLight-0.2.0.63/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.597326 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/
-drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.618366 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Function/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Function/__init__.py
--rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Function/minusFunction.pyd
--rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Function/minusFunctionpy.py
--rw-rw-rw-   0        0        0  1998544 2024-04-02 03:41:08.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/RDaddins.xlam
--rw-rw-rw-   0        0        0     8192 2023-08-21 07:30:54.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/RecentTime.db
-drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.624334 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Ui/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Ui/__init__.py
--rw-rw-rw-   0        0        0    66560 2023-08-17 01:40:15.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Ui/rongdaVbaAddinsUi.pyd
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.628330 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.641331 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/
--rw-rw-rw-   0        0        0      152 2023-12-29 05:53:14.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/__init__.py
--rw-rw-rw-   0        0        0       63 2023-12-29 05:53:05.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/__version__.py
--rw-rw-rw-   0        0        0    95557 2023-12-29 05:53:06.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/zipfile.py
--rw-rw-rw-   0        0        0    11589 2023-12-29 05:52:58.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/zipfile_aes.py
--rw-rw-rw-   0        0        0   379904 2024-05-06 08:16:13.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/registerCode.pyd
--rw-rw-rw-   0        0        0   210944 2024-05-06 08:27:08.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/rongdavbaaddinsLight.pyd
--rw-rw-rw-   0        0        0      152 2023-08-22 06:02:10.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/runregiterCode.py
--rw-rw-rw-   0        0        0    57354 2024-04-02 03:41:08.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/文件处理类模板.xlsx
-drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.610330 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight.egg-info/
--rw-rw-rw-   0        0        0      405 2024-05-06 08:27:41.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      969 2024-05-06 08:27:41.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 08:27:41.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-05-06 08:27:41.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2024-05-06 08:27:41.646329 rongdaVbaAddinsLight-0.2.0.63/setup.cfg
--rw-rw-rw-   0        0        0     1032 2024-05-06 08:24:19.000000 rongdaVbaAddinsLight-0.2.0.63/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:52:49.413729 rongdaVbaAddinsLight-0.2.0.64/
+-rw-rw-rw-   0        0        0        0 2023-10-11 02:09:37.000000 rongdaVbaAddinsLight-0.2.0.64/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdaVbaAddinsLight-0.2.0.64/MANIFEST.in
+-rw-rw-rw-   0        0        0      405 2024-05-29 08:52:49.410724 rongdaVbaAddinsLight-0.2.0.64/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-10-11 02:09:37.000000 rongdaVbaAddinsLight-0.2.0.64/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 08:52:49.322744 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/
+drwxrwxrwx   0        0        0        0 2024-05-29 08:52:49.363722 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/Function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/Function/__init__.py
+-rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/Function/minusFunction.pyd
+-rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/Function/minusFunctionpy.py
+-rw-rw-rw-   0        0        0  1998544 2024-04-02 03:41:08.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/RDaddins.xlam
+-rw-rw-rw-   0        0        0     8192 2023-08-21 07:30:54.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/RecentTime.db
+drwxrwxrwx   0        0        0        0 2024-05-29 08:52:49.373734 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/Ui/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/Ui/__init__.py
+-rw-rw-rw-   0        0        0    66560 2023-08-17 01:40:15.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/Ui/rongdaVbaAddinsUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:52:49.381723 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/package/
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:52:49.404724 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/package/pyzipper/
+-rw-rw-rw-   0        0        0      152 2023-12-29 05:53:14.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/package/pyzipper/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-12-29 05:53:05.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/package/pyzipper/__version__.py
+-rw-rw-rw-   0        0        0    95557 2023-12-29 05:53:06.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/package/pyzipper/zipfile.py
+-rw-rw-rw-   0        0        0    11589 2023-12-29 05:52:58.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/package/pyzipper/zipfile_aes.py
+-rw-rw-rw-   0        0        0   379904 2024-05-06 08:16:13.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/registerCode.pyd
+-rw-rw-rw-   0        0        0   210944 2024-05-29 08:50:46.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/rongdavbaaddinsLight.pyd
+-rw-rw-rw-   0        0        0      152 2023-08-22 06:02:10.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/runregiterCode.py
+-rw-rw-rw-   0        0        0    57354 2024-04-02 03:41:08.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/文件处理类模板.xlsx
+drwxrwxrwx   0        0        0        0 2024-05-29 08:52:49.345733 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight.egg-info/
+-rw-rw-rw-   0        0        0      405 2024-05-29 08:52:49.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2024-05-29 08:52:49.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:52:49.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-05-29 08:52:49.000000 rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2024-05-29 08:52:49.416740 rongdaVbaAddinsLight-0.2.0.64/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2024-05-29 08:52:28.000000 rongdaVbaAddinsLight-0.2.0.64/setup.py
```

### Comparing `rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/RDaddins.xlam` & `rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/RDaddins.xlam`

 * *Files identical despite different names*

### Comparing `rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/RecentTime.db` & `rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/RecentTime.db`

 * *Files identical despite different names*

### Comparing `rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/zipfile.py` & `rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/package/pyzipper/zipfile.py`

 * *Files identical despite different names*

### Comparing `rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/zipfile_aes.py` & `rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/package/pyzipper/zipfile_aes.py`

 * *Files identical despite different names*

### Comparing `rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/文件处理类模板.xlsx` & `rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight/文件处理类模板.xlsx`

 * *Files identical despite different names*

### Comparing `rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight.egg-info/SOURCES.txt` & `rongdaVbaAddinsLight-0.2.0.64/rongdaVbaAddinsLight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rongdaVbaAddinsLight-0.2.0.63/setup.py` & `rongdaVbaAddinsLight-0.2.0.64/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 2
 PATCH = 0
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.63"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.64"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "rongdaVbaAddinsLight",
     version=VERSION,
```

