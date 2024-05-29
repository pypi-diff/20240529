# Comparing `tmp/hwdesk-1.0.0.tar.gz` & `tmp/hwdesk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hwdesk-1.0.0.tar", last modified: Wed May 29 18:36:49 2024, max compression
+gzip compressed data, was "hwdesk-1.0.1.tar", last modified: Wed May 29 18:40:22 2024, max compression
```

## Comparing `hwdesk-1.0.0.tar` & `hwdesk-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:49.228695 hwdesk-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 18:36:43.000000 hwdesk-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-29 18:36:43.000000 hwdesk-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-29 18:36:49.224695 hwdesk-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-29 18:36:43.000000 hwdesk-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:49.224695 hwdesk-1.0.0/hwdesk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:49.224695 hwdesk-1.0.0/hwdesk/camera/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/camera/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/camera/ms2109.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/camera/ms2130.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/camera/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:49.224695 hwdesk-1.0.0/hwdesk/controls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/controls/ch9329.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/controls/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:43.000000 hwdesk-1.0.0/hwdesk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:36:49.224695 hwdesk-1.0.0/hwdesk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-29 18:36:49.000000 hwdesk-1.0.0/hwdesk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-29 18:36:49.000000 hwdesk-1.0.0/hwdesk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:36:49.000000 hwdesk-1.0.0/hwdesk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-29 18:36:49.000000 hwdesk-1.0.0/hwdesk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 18:36:49.000000 hwdesk-1.0.0/hwdesk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-29 18:36:43.000000 hwdesk-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 18:36:49.228695 hwdesk-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:22.812915 hwdesk-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 18:40:16.000000 hwdesk-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-29 18:40:16.000000 hwdesk-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-29 18:40:22.812915 hwdesk-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-29 18:40:16.000000 hwdesk-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:22.812915 hwdesk-1.0.1/hwdesk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:22.812915 hwdesk-1.0.1/hwdesk/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/camera/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/camera/ms2109.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/camera/ms2130.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/camera/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:22.812915 hwdesk-1.0.1/hwdesk/controls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/controls/ch9329.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/controls/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:22.812915 hwdesk-1.0.1/hwdesk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-29 18:40:22.000000 hwdesk-1.0.1/hwdesk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 18:40:22.000000 hwdesk-1.0.1/hwdesk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:40:22.000000 hwdesk-1.0.1/hwdesk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 18:40:22.000000 hwdesk-1.0.1/hwdesk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-29 18:40:22.000000 hwdesk-1.0.1/hwdesk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 18:40:22.000000 hwdesk-1.0.1/hwdesk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-29 18:40:16.000000 hwdesk-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 18:40:22.812915 hwdesk-1.0.1/setup.cfg
```

### Comparing `hwdesk-1.0.0/LICENSE` & `hwdesk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.0/PKG-INFO` & `hwdesk-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hwdesk
-Version: 1.0.0
+Version: 1.0.1
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `hwdesk-1.0.0/hwdesk/__main__.py` & `hwdesk-1.0.1/hwdesk/__main__.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.0/hwdesk/camera/base.py` & `hwdesk-1.0.1/hwdesk/camera/base.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.0/hwdesk/camera/prompt.py` & `hwdesk-1.0.1/hwdesk/camera/prompt.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.0/hwdesk/controls/ch9329.py` & `hwdesk-1.0.1/hwdesk/controls/ch9329.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.0/hwdesk/controls/prompt.py` & `hwdesk-1.0.1/hwdesk/controls/prompt.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.0/hwdesk/gui.py` & `hwdesk-1.0.1/hwdesk/gui.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.0/hwdesk/logger.py` & `hwdesk-1.0.1/hwdesk/logger.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.0/hwdesk.egg-info/PKG-INFO` & `hwdesk-1.0.1/hwdesk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hwdesk
-Version: 1.0.0
+Version: 1.0.1
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `hwdesk-1.0.0/pyproject.toml` & `hwdesk-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hwdesk"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = [
     "ch9329==1.1.2",
     "opencv-cam-idx==1.0.1",
     "opencv-python==4.9.0.80",
     "pydantic==2.6.4",
     "pillow==10.3.0",
 ]
@@ -20,14 +20,17 @@
 keywords = []
 classifiers = ["Programming Language :: Python :: 3"]
 
 [project.urls]
 Homepage = "https://github.com/sandbox-pokhara/hwdesk"
 Issues = "https://github.com/sandbox-pokhara/hwdesk/issues"
 
+[project.gui-scripts]
+hwdesk = "hwdesk.__main__:main"
+
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-dir]
 "hwdesk" = "hwdesk"
 
 [tool.isort]
```

