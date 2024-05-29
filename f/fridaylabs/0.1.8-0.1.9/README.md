# Comparing `tmp/fridaylabs-0.1.8.tar.gz` & `tmp/fridaylabs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fridaylabs-0.1.8.tar", last modified: Wed May 29 19:59:28 2024, max compression
+gzip compressed data, was "fridaylabs-0.1.9.tar", last modified: Wed May 29 20:07:28 2024, max compression
```

## Comparing `fridaylabs-0.1.8.tar` & `fridaylabs-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 19:59:28.193975 fridaylabs-0.1.8/
--rw-r--r--   0 ricky      (501) staff       (20)     1070 2024-05-21 04:23:26.000000 fridaylabs-0.1.8/LICENSE
--rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-29 19:59:28.193724 fridaylabs-0.1.8/PKG-INFO
--rw-r--r--   0 ricky      (501) staff       (20)      792 2024-05-21 05:35:31.000000 fridaylabs-0.1.8/README.md
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 19:59:28.192216 fridaylabs-0.1.8/fridaylabs/
--rw-r--r--   0 ricky      (501) staff       (20)       61 2024-05-21 05:49:44.000000 fridaylabs-0.1.8/fridaylabs/__init__.py
--rw-r--r--   0 ricky      (501) staff       (20)     5613 2024-05-29 19:59:14.000000 fridaylabs-0.1.8/fridaylabs/fridaylabs.py
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 19:59:28.193470 fridaylabs-0.1.8/fridaylabs.egg-info/
--rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-29 19:59:28.000000 fridaylabs-0.1.8/fridaylabs.egg-info/PKG-INFO
--rw-r--r--   0 ricky      (501) staff       (20)      243 2024-05-29 19:59:28.000000 fridaylabs-0.1.8/fridaylabs.egg-info/SOURCES.txt
--rw-r--r--   0 ricky      (501) staff       (20)        1 2024-05-29 19:59:28.000000 fridaylabs-0.1.8/fridaylabs.egg-info/dependency_links.txt
--rw-r--r--   0 ricky      (501) staff       (20)        9 2024-05-29 19:59:28.000000 fridaylabs-0.1.8/fridaylabs.egg-info/requires.txt
--rw-r--r--   0 ricky      (501) staff       (20)       11 2024-05-29 19:59:28.000000 fridaylabs-0.1.8/fridaylabs.egg-info/top_level.txt
--rw-r--r--   0 ricky      (501) staff       (20)       38 2024-05-29 19:59:28.194024 fridaylabs-0.1.8/setup.cfg
--rw-r--r--   0 ricky      (501) staff       (20)      693 2024-05-29 19:59:25.000000 fridaylabs-0.1.8/setup.py
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 20:07:28.702937 fridaylabs-0.1.9/
+-rw-r--r--   0 ricky      (501) staff       (20)     1070 2024-05-21 04:23:26.000000 fridaylabs-0.1.9/LICENSE
+-rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-29 20:07:28.702608 fridaylabs-0.1.9/PKG-INFO
+-rw-r--r--   0 ricky      (501) staff       (20)      792 2024-05-21 05:35:31.000000 fridaylabs-0.1.9/README.md
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 20:07:28.701060 fridaylabs-0.1.9/fridaylabs/
+-rw-r--r--   0 ricky      (501) staff       (20)       61 2024-05-21 05:49:44.000000 fridaylabs-0.1.9/fridaylabs/__init__.py
+-rw-r--r--   0 ricky      (501) staff       (20)     5613 2024-05-29 20:07:19.000000 fridaylabs-0.1.9/fridaylabs/fridaylabs.py
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-29 20:07:28.702283 fridaylabs-0.1.9/fridaylabs.egg-info/
+-rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-29 20:07:28.000000 fridaylabs-0.1.9/fridaylabs.egg-info/PKG-INFO
+-rw-r--r--   0 ricky      (501) staff       (20)      243 2024-05-29 20:07:28.000000 fridaylabs-0.1.9/fridaylabs.egg-info/SOURCES.txt
+-rw-r--r--   0 ricky      (501) staff       (20)        1 2024-05-29 20:07:28.000000 fridaylabs-0.1.9/fridaylabs.egg-info/dependency_links.txt
+-rw-r--r--   0 ricky      (501) staff       (20)        9 2024-05-29 20:07:28.000000 fridaylabs-0.1.9/fridaylabs.egg-info/requires.txt
+-rw-r--r--   0 ricky      (501) staff       (20)       11 2024-05-29 20:07:28.000000 fridaylabs-0.1.9/fridaylabs.egg-info/top_level.txt
+-rw-r--r--   0 ricky      (501) staff       (20)       38 2024-05-29 20:07:28.703332 fridaylabs-0.1.9/setup.cfg
+-rw-r--r--   0 ricky      (501) staff       (20)      693 2024-05-29 20:04:40.000000 fridaylabs-0.1.9/setup.py
```

### Comparing `fridaylabs-0.1.8/LICENSE` & `fridaylabs-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.8/PKG-INFO` & `fridaylabs-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fridaylabs
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to interact with FridayLabs AI API
 Home-page: https://github.com/ImJustRicky/fridaylabs-package
 Author: FridayLabs
 Author-email: fridaylabs@fridaylabs.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fridaylabs-0.1.8/README.md` & `fridaylabs-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.8/fridaylabs/fridaylabs.py` & `fridaylabs-0.1.9/fridaylabs/fridaylabs.py`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.8/fridaylabs.egg-info/PKG-INFO` & `fridaylabs-0.1.9/fridaylabs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fridaylabs
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to interact with FridayLabs AI API
 Home-page: https://github.com/ImJustRicky/fridaylabs-package
 Author: FridayLabs
 Author-email: fridaylabs@fridaylabs.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fridaylabs-0.1.8/setup.py` & `fridaylabs-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name="fridaylabs",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     install_requires=["requests"],  # Add any dependencies here
     author="FridayLabs",
     author_email="fridaylabs@fridaylabs.ai",
     description="A package to interact with FridayLabs AI API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

