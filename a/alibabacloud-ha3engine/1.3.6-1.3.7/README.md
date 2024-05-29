# Comparing `tmp/alibabacloud_ha3engine-1.3.6.tar.gz` & `tmp/alibabacloud_ha3engine-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ha3engine-1.3.6.tar", last modified: Tue Nov 14 05:59:25 2023, max compression
+gzip compressed data, was "dist/alibabacloud_ha3engine-1.3.7.tar", last modified: Wed May 29 08:49:56 2024, max compression
```

## Comparing `alibabacloud_ha3engine-1.3.6.tar` & `alibabacloud_ha3engine-1.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/
--rw-r--r--   0 root         (0) root         (0)      888 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/alibabacloud_ha3engine/
--rw-r--r--   0 root         (0) root         (0)       22 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/alibabacloud_ha3engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41232 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/alibabacloud_ha3engine/client.py
--rw-r--r--   0 root         (0) root         (0)    24211 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/alibabacloud_ha3engine/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/alibabacloud_ha3engine.egg-info/
--rw-r--r--   0 root         (0) root         (0)      888 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/alibabacloud_ha3engine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      338 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/alibabacloud_ha3engine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/alibabacloud_ha3engine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      171 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/alibabacloud_ha3engine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/alibabacloud_ha3engine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2609 2023-11-14 05:59:25.000000 alibabacloud_ha3engine-1.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/
+-rw-r--r--   0 root         (0) root         (0)      888 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/alibabacloud_ha3engine/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/alibabacloud_ha3engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51052 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/alibabacloud_ha3engine/client.py
+-rw-r--r--   0 root         (0) root         (0)    24211 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/alibabacloud_ha3engine/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/alibabacloud_ha3engine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      888 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/alibabacloud_ha3engine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      338 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/alibabacloud_ha3engine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/alibabacloud_ha3engine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/alibabacloud_ha3engine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/alibabacloud_ha3engine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2609 2024-05-29 08:49:56.000000 alibabacloud_ha3engine-1.3.7/setup.py
```

### Comparing `alibabacloud_ha3engine-1.3.6/PKG-INFO` & `alibabacloud_ha3engine-1.3.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ha3engine
-Version: 1.3.6
+Version: 1.3.7
 Summary: Alibaba Cloud Ha3engine SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-ha3-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,ha3engine
```

### Comparing `alibabacloud_ha3engine-1.3.6/alibabacloud_ha3engine/models.py` & `alibabacloud_ha3engine-1.3.7/alibabacloud_ha3engine/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_ha3engine-1.3.6/alibabacloud_ha3engine.egg-info/PKG-INFO` & `alibabacloud_ha3engine-1.3.7/alibabacloud_ha3engine.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ha3engine
-Version: 1.3.6
+Version: 1.3.7
 Summary: Alibaba Cloud Ha3engine SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-ha3-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,ha3engine
```

### Comparing `alibabacloud_ha3engine-1.3.6/setup.py` & `alibabacloud_ha3engine-1.3.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ha3engine.
 
-Created on 14/11/2023
+Created on 29/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ha3engine"
 NAME = "alibabacloud_ha3engine" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Ha3engine SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-ha3-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
     "alibabacloud_darabonba_string>=0.0.4, <1.0.0",
     "alibabacloud_darabonba_encode_util>=0.0.2, <1.0.0",
     "alibabacloud_darabonba_map>=0.0.1, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

