# Comparing `tmp/xfapi-0.0.5.tar.gz` & `tmp/xfapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfapi-0.0.5.tar", last modified: Wed May 29 07:38:45 2024, max compression
+gzip compressed data, was "xfapi-0.0.6.tar", last modified: Wed May 29 07:45:10 2024, max compression
```

## Comparing `xfapi-0.0.5.tar` & `xfapi-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 07:38:45.992227 xfapi-0.0.5/
--rw-r--r--   0 asia       (501) staff       (20)     1307 2024-05-29 07:38:45.991987 xfapi-0.0.5/PKG-INFO
--rw-r--r--   0 asia       (501) staff       (20)      883 2024-05-29 05:46:51.000000 xfapi-0.0.5/README.md
--rw-r--r--   0 asia       (501) staff       (20)       14 2024-05-29 05:50:03.000000 xfapi-0.0.5/requirements.txt
--rw-r--r--   0 asia       (501) staff       (20)       38 2024-05-29 07:38:45.992278 xfapi-0.0.5/setup.cfg
--rw-r--r--   0 asia       (501) staff       (20)     1393 2024-05-29 07:38:44.000000 xfapi-0.0.5/setup.py
-drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 07:38:45.990762 xfapi-0.0.5/xfapi/
--rw-r--r--   0 asia       (501) staff       (20)       69 2024-05-29 07:38:27.000000 xfapi-0.0.5/xfapi/__init__.py
--rw-r--r--   0 asia       (501) staff       (20)     2980 2024-05-29 04:48:29.000000 xfapi-0.0.5/xfapi/server.py
-drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 07:38:45.991736 xfapi-0.0.5/xfapi.egg-info/
--rw-r--r--   0 asia       (501) staff       (20)     1307 2024-05-29 07:38:45.000000 xfapi-0.0.5/xfapi.egg-info/PKG-INFO
--rw-r--r--   0 asia       (501) staff       (20)      213 2024-05-29 07:38:45.000000 xfapi-0.0.5/xfapi.egg-info/SOURCES.txt
--rw-r--r--   0 asia       (501) staff       (20)        1 2024-05-29 07:38:45.000000 xfapi-0.0.5/xfapi.egg-info/dependency_links.txt
--rw-r--r--   0 asia       (501) staff       (20)       15 2024-05-29 07:38:45.000000 xfapi-0.0.5/xfapi.egg-info/requires.txt
--rw-r--r--   0 asia       (501) staff       (20)        6 2024-05-29 07:38:45.000000 xfapi-0.0.5/xfapi.egg-info/top_level.txt
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 07:45:10.360012 xfapi-0.0.6/
+-rw-r--r--   0 asia       (501) staff       (20)     1307 2024-05-29 07:45:10.359732 xfapi-0.0.6/PKG-INFO
+-rw-r--r--   0 asia       (501) staff       (20)      883 2024-05-29 05:46:51.000000 xfapi-0.0.6/README.md
+-rw-r--r--   0 asia       (501) staff       (20)       14 2024-05-29 05:50:03.000000 xfapi-0.0.6/requirements.txt
+-rw-r--r--   0 asia       (501) staff       (20)       38 2024-05-29 07:45:10.360074 xfapi-0.0.6/setup.cfg
+-rw-r--r--   0 asia       (501) staff       (20)     1393 2024-05-29 07:45:09.000000 xfapi-0.0.6/setup.py
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 07:45:10.357715 xfapi-0.0.6/xfapi/
+-rw-r--r--   0 asia       (501) staff       (20)       45 2024-05-29 07:44:34.000000 xfapi-0.0.6/xfapi/__init__.py
+-rw-r--r--   0 asia       (501) staff       (20)     2980 2024-05-29 07:45:01.000000 xfapi-0.0.6/xfapi/server.py
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 07:45:10.358860 xfapi-0.0.6/xfapi/utils/
+-rw-r--r--   0 asia       (501) staff       (20)       18 2024-05-29 07:44:50.000000 xfapi-0.0.6/xfapi/utils/__init__.py
+-rw-r--r--   0 asia       (501) staff       (20)     1467 2024-05-29 03:49:23.000000 xfapi-0.0.6/xfapi/utils/auth.py
+-rw-r--r--   0 asia       (501) staff       (20)     1096 2024-05-29 03:52:36.000000 xfapi-0.0.6/xfapi/utils/load_yaml.py
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 07:45:10.359422 xfapi-0.0.6/xfapi.egg-info/
+-rw-r--r--   0 asia       (501) staff       (20)     1307 2024-05-29 07:45:10.000000 xfapi-0.0.6/xfapi.egg-info/PKG-INFO
+-rw-r--r--   0 asia       (501) staff       (20)      282 2024-05-29 07:45:10.000000 xfapi-0.0.6/xfapi.egg-info/SOURCES.txt
+-rw-r--r--   0 asia       (501) staff       (20)        1 2024-05-29 07:45:10.000000 xfapi-0.0.6/xfapi.egg-info/dependency_links.txt
+-rw-r--r--   0 asia       (501) staff       (20)       15 2024-05-29 07:45:10.000000 xfapi-0.0.6/xfapi.egg-info/requires.txt
+-rw-r--r--   0 asia       (501) staff       (20)        6 2024-05-29 07:45:10.000000 xfapi-0.0.6/xfapi.egg-info/top_level.txt
```

### Comparing `xfapi-0.0.5/PKG-INFO` & `xfapi-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Apis tool base fastapi
 Home-page: https://pypi.org/project/xfapi/
 Author: Alex_M
 Author-email: asiaier@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xfapi-0.0.5/README.md` & `xfapi-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `xfapi-0.0.5/setup.py` & `xfapi-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
  
 package_name = "xfapi"
  
 
 def get_version():
-   return "0.0.5"
+   return "0.0.6"
  
  
 def upload():
     with open("README.md", "r") as fh:
         long_description = fh.read()
     with open('requirements.txt') as f:
         required = f.read().splitlines()
```

### Comparing `xfapi-0.0.5/xfapi/server.py` & `xfapi-0.0.6/xfapi/server.py`

 * *Files identical despite different names*

### Comparing `xfapi-0.0.5/xfapi.egg-info/PKG-INFO` & `xfapi-0.0.6/xfapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Apis tool base fastapi
 Home-page: https://pypi.org/project/xfapi/
 Author: Alex_M
 Author-email: asiaier@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

