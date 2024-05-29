# Comparing `tmp/ox_script-2.0.5.tar.gz` & `tmp/ox_script-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ox_script-2.0.5.tar", last modified: Tue May 28 20:09:58 2024, max compression
+gzip compressed data, was "ox_script-2.1.0.tar", last modified: Tue May 28 20:12:42 2024, max compression
```

## Comparing `ox_script-2.0.5.tar` & `ox_script-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2024-05-28 20:09:58.050798 ox_script-2.0.5/
--rw-r--r--   0 jarvislu   (501) staff       (20)       13 2023-04-22 17:32:02.000000 ox_script-2.0.5/MANIFEST.in
--rw-r--r--   0 jarvislu   (501) staff       (20)      389 2024-05-28 20:09:58.050508 ox_script-2.0.5/PKG-INFO
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2024-05-28 20:09:58.048301 ox_script-2.0.5/ox_script/
--rw-r--r--   0 jarvislu   (501) staff       (20)       72 2023-04-22 22:41:41.000000 ox_script-2.0.5/ox_script/__init__.py
--rw-------   0 jarvislu   (501) staff       (20)    12256 2023-04-26 16:53:14.000000 ox_script-2.0.5/ox_script/general_purpose_apis.py
--rw-------   0 jarvislu   (501) staff       (20)    36820 2023-04-26 18:04:03.000000 ox_script-2.0.5/ox_script/printer_specific_apis.py
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2024-05-28 20:09:58.050076 ox_script-2.0.5/ox_script.egg-info/
--rw-r--r--   0 jarvislu   (501) staff       (20)      389 2024-05-28 20:09:58.000000 ox_script-2.0.5/ox_script.egg-info/PKG-INFO
--rw-r--r--   0 jarvislu   (501) staff       (20)      275 2024-05-28 20:09:58.000000 ox_script-2.0.5/ox_script.egg-info/SOURCES.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)        1 2024-05-28 20:09:58.000000 ox_script-2.0.5/ox_script.egg-info/dependency_links.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)       16 2024-05-28 20:09:58.000000 ox_script-2.0.5/ox_script.egg-info/requires.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)       10 2024-05-28 20:09:58.000000 ox_script-2.0.5/ox_script.egg-info/top_level.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)       38 2024-05-28 20:09:58.050854 ox_script-2.0.5/setup.cfg
--rw-r--r--   0 jarvislu   (501) staff       (20)      875 2024-05-28 20:07:58.000000 ox_script-2.0.5/setup.py
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2024-05-28 20:12:42.068400 ox_script-2.1.0/
+-rw-r--r--   0 jarvislu   (501) staff       (20)       13 2023-04-22 17:32:02.000000 ox_script-2.1.0/MANIFEST.in
+-rw-r--r--   0 jarvislu   (501) staff       (20)      939 2024-05-28 20:12:42.068094 ox_script-2.1.0/PKG-INFO
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2024-05-28 20:12:42.066436 ox_script-2.1.0/ox_script/
+-rw-r--r--   0 jarvislu   (501) staff       (20)       72 2023-04-22 22:41:41.000000 ox_script-2.1.0/ox_script/__init__.py
+-rw-------   0 jarvislu   (501) staff       (20)    12256 2023-04-26 16:53:14.000000 ox_script-2.1.0/ox_script/general_purpose_apis.py
+-rw-------   0 jarvislu   (501) staff       (20)    36820 2023-04-26 18:04:03.000000 ox_script-2.1.0/ox_script/printer_specific_apis.py
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2024-05-28 20:12:42.067748 ox_script-2.1.0/ox_script.egg-info/
+-rw-r--r--   0 jarvislu   (501) staff       (20)      939 2024-05-28 20:12:42.000000 ox_script-2.1.0/ox_script.egg-info/PKG-INFO
+-rw-r--r--   0 jarvislu   (501) staff       (20)      275 2024-05-28 20:12:42.000000 ox_script-2.1.0/ox_script.egg-info/SOURCES.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)        1 2024-05-28 20:12:42.000000 ox_script-2.1.0/ox_script.egg-info/dependency_links.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)       16 2024-05-28 20:12:42.000000 ox_script-2.1.0/ox_script.egg-info/requires.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)       10 2024-05-28 20:12:42.000000 ox_script-2.1.0/ox_script.egg-info/top_level.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)       38 2024-05-28 20:12:42.068456 ox_script-2.1.0/setup.cfg
+-rw-r--r--   0 jarvislu   (501) staff       (20)     1497 2024-05-28 20:12:37.000000 ox_script-2.1.0/setup.py
```

### Comparing `ox_script-2.0.5/ox_script/general_purpose_apis.py` & `ox_script-2.1.0/ox_script/general_purpose_apis.py`

 * *Files identical despite different names*

### Comparing `ox_script-2.0.5/ox_script/printer_specific_apis.py` & `ox_script-2.1.0/ox_script/printer_specific_apis.py`

 * *Files identical despite different names*

### Comparing `ox_script-2.0.5/setup.py` & `ox_script-2.1.0/ox_script.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from setuptools import setup, find_packages
+Metadata-Version: 2.1
+Name: ox-script
+Version: 2.1.0
+Summary: The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
+Home-page: https://github.com/POSTEK-OX-Script
+Author: Postek Electronics Co., Ltd.
+Author-email: support@postek.com.cn
+License: MIT
+Description-Content-Type: text/markdown
+Requires-Dist: pandas
+Requires-Dist: openpyxl
 
-setup(
-    name='ox_script',
-    version='2.0.5',
-    author='Postek Electronics Co., Ltd.',
-    author_email='support@postek.com.cn',
-    packages=find_packages(),
-    license="MIT",
-    description="The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.\nMost printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. ",
-    url="https://github.com/POSTEK-OX-Script",
-    install_requires=[
-        "pandas",
-        "openpyxl",
-    ],
-)
+The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
+Most printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip.
```

