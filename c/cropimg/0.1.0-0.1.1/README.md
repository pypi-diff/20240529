# Comparing `tmp/cropimg-0.1.0.tar.gz` & `tmp/cropimg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cropimg-0.1.0.tar", last modified: Tue May 28 14:12:33 2024, max compression
+gzip compressed data, was "cropimg-0.1.1.tar", last modified: Tue May 28 23:23:29 2024, max compression
```

## Comparing `cropimg-0.1.0.tar` & `cropimg-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-28 14:12:33.343009 cropimg-0.1.0/
--rw-r--r--   0 iuchi      (501) staff       (20)     1068 2024-05-28 13:09:12.000000 cropimg-0.1.0/LICENSE
--rw-r--r--   0 iuchi      (501) staff       (20)      361 2024-05-28 14:12:33.342885 cropimg-0.1.0/PKG-INFO
--rw-r--r--   0 iuchi      (501) staff       (20)     2478 2024-05-28 13:45:48.000000 cropimg-0.1.0/README.md
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-28 14:12:33.342038 cropimg-0.1.0/crop_image/
--rw-r--r--   0 iuchi      (501) staff       (20)        0 2024-05-28 12:52:37.000000 cropimg-0.1.0/crop_image/__init__.py
--rwxr-xr-x   0 iuchi      (501) staff       (20)     3380 2024-05-28 13:08:14.000000 cropimg-0.1.0/crop_image/crop_image.py
--rw-r--r--   0 iuchi      (501) staff       (20)      647 2024-05-28 07:17:22.000000 cropimg-0.1.0/crop_image/update_image.py
--rw-r--r--   0 iuchi      (501) staff       (20)      660 2024-05-28 13:00:29.000000 cropimg-0.1.0/crop_image/update_image_adb.py
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-28 14:12:33.342711 cropimg-0.1.0/cropimg.egg-info/
--rw-r--r--   0 iuchi      (501) staff       (20)      361 2024-05-28 14:12:33.000000 cropimg-0.1.0/cropimg.egg-info/PKG-INFO
--rw-r--r--   0 iuchi      (501) staff       (20)      320 2024-05-28 14:12:33.000000 cropimg-0.1.0/cropimg.egg-info/SOURCES.txt
--rw-r--r--   0 iuchi      (501) staff       (20)        1 2024-05-28 14:12:33.000000 cropimg-0.1.0/cropimg.egg-info/dependency_links.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       55 2024-05-28 14:12:33.000000 cropimg-0.1.0/cropimg.egg-info/entry_points.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       32 2024-05-28 14:12:33.000000 cropimg-0.1.0/cropimg.egg-info/requires.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       11 2024-05-28 14:12:33.000000 cropimg-0.1.0/cropimg.egg-info/top_level.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       38 2024-05-28 14:12:33.343046 cropimg-0.1.0/setup.cfg
--rw-r--r--   0 iuchi      (501) staff       (20)      683 2024-05-28 14:11:07.000000 cropimg-0.1.0/setup.py
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-28 23:23:29.793304 cropimg-0.1.1/
+-rw-r--r--   0 iuchi      (501) staff       (20)     1068 2024-05-28 13:09:12.000000 cropimg-0.1.1/LICENSE
+-rw-r--r--   0 iuchi      (501) staff       (20)      361 2024-05-28 23:23:29.793172 cropimg-0.1.1/PKG-INFO
+-rw-r--r--   0 iuchi      (501) staff       (20)     1802 2024-05-28 23:22:36.000000 cropimg-0.1.1/README.md
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-28 23:23:29.792163 cropimg-0.1.1/cropimg/
+-rw-r--r--   0 iuchi      (501) staff       (20)        0 2024-05-28 12:52:37.000000 cropimg-0.1.1/cropimg/__init__.py
+-rwxr-xr-x   0 iuchi      (501) staff       (20)     3374 2024-05-28 23:19:17.000000 cropimg-0.1.1/cropimg/cropimg.py
+-rw-r--r--   0 iuchi      (501) staff       (20)      647 2024-05-28 07:17:22.000000 cropimg-0.1.1/cropimg/update_image.py
+-rw-r--r--   0 iuchi      (501) staff       (20)      657 2024-05-28 23:19:25.000000 cropimg-0.1.1/cropimg/update_image_adb.py
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-28 23:23:29.792964 cropimg-0.1.1/cropimg.egg-info/
+-rw-r--r--   0 iuchi      (501) staff       (20)      361 2024-05-28 23:23:29.000000 cropimg-0.1.1/cropimg.egg-info/PKG-INFO
+-rw-r--r--   0 iuchi      (501) staff       (20)      305 2024-05-28 23:23:29.000000 cropimg-0.1.1/cropimg.egg-info/SOURCES.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)        1 2024-05-28 23:23:29.000000 cropimg-0.1.1/cropimg.egg-info/dependency_links.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       49 2024-05-28 23:23:29.000000 cropimg-0.1.1/cropimg.egg-info/entry_points.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       32 2024-05-28 23:23:29.000000 cropimg-0.1.1/cropimg.egg-info/requires.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)        8 2024-05-28 23:23:29.000000 cropimg-0.1.1/cropimg.egg-info/top_level.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       38 2024-05-28 23:23:29.793346 cropimg-0.1.1/setup.cfg
+-rw-r--r--   0 iuchi      (501) staff       (20)      677 2024-05-28 23:20:18.000000 cropimg-0.1.1/setup.py
```

### Comparing `cropimg-0.1.0/LICENSE` & `cropimg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cropimg-0.1.0/crop_image/crop_image.py` & `cropimg-0.1.1/cropimg/cropimg.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from datetime import datetime
 import io
 import os
 import base64
 from flask import Flask, request, send_file, render_template, abort, jsonify
 from PIL import Image
-from crop_image.update_image import UpdateImage
-from crop_image.update_image_adb import *
+from cropimg.update_image import UpdateImage
+from cropimg.update_image_adb import *
 
 # Input image file path
 IMAGE_PATH = os.path.join(os.path.dirname(__file__), 'static', 'input.png')
 
 # Output image directory
 OUTPUT_DIR = os.path.join(os.getcwd(), 'output')
```

### Comparing `cropimg-0.1.0/crop_image/update_image.py` & `cropimg-0.1.1/cropimg/update_image.py`

 * *Files identical despite different names*

### Comparing `cropimg-0.1.0/crop_image/update_image_adb.py` & `cropimg-0.1.1/cropimg/update_image_adb.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from crop_image.update_image import UpdateImage
+from cropimg.update_image import UpdateImage
 import adb_tool_py as adb_tool
 import adb_tool_py.command as command
 
 
 class UpdateImageAdb(UpdateImage):
     def __init__(self, name: str) -> None:
         super().__init__(self, name)
```

### Comparing `cropimg-0.1.0/setup.py` & `cropimg-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cropimg',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'Flask',
         'pillow',
         'adb-tool-py>=0.1.2',
     ],
     entry_points={
         'console_scripts': [
-            'cropimg=crop_image.crop_image:main',
+            'cropimg=cropimg.cropimg:main',
         ],
     },
     author='Shota Iuchi',
     author_email='shotaiuchi.develop@gmail.com',
     description='Cropping images',
     license='MIT',
     classifiers=[
```

