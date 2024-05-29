# Comparing `tmp/tenorgrabber-1.0.1.tar.gz` & `tmp/tenorgrabber-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenorgrabber-1.0.1.tar", last modified: Wed May 29 08:41:50 2024, max compression
+gzip compressed data, was "tenorgrabber-1.0.2.tar", last modified: Wed May 29 08:46:08 2024, max compression
```

## Comparing `tenorgrabber-1.0.1.tar` & `tenorgrabber-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:41:50.111543 tenorgrabber-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 08:41:46.000000 tenorgrabber-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-29 08:41:50.111543 tenorgrabber-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-29 08:41:46.000000 tenorgrabber-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:41:50.107543 tenorgrabber-1.0.1/TenorGrabber/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:41:46.000000 tenorgrabber-1.0.1/TenorGrabber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-29 08:41:46.000000 tenorgrabber-1.0.1/TenorGrabber/tenorgrabber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:41:50.111543 tenorgrabber-1.0.1/TenorGrabber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-29 08:41:50.000000 tenorgrabber-1.0.1/TenorGrabber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-29 08:41:50.000000 tenorgrabber-1.0.1/TenorGrabber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:41:50.000000 tenorgrabber-1.0.1/TenorGrabber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 08:41:50.000000 tenorgrabber-1.0.1/TenorGrabber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:41:50.111543 tenorgrabber-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 08:41:46.000000 tenorgrabber-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:41:50.111543 tenorgrabber-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:41:46.000000 tenorgrabber-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-29 08:41:46.000000 tenorgrabber-1.0.1/tests/tenorgrabber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:46:08.085304 tenorgrabber-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 08:46:04.000000 tenorgrabber-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-29 08:46:08.085304 tenorgrabber-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-29 08:46:04.000000 tenorgrabber-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:46:08.081303 tenorgrabber-1.0.2/TenorGrabber/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:46:04.000000 tenorgrabber-1.0.2/TenorGrabber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-29 08:46:04.000000 tenorgrabber-1.0.2/TenorGrabber/tenorgrabber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:46:08.085304 tenorgrabber-1.0.2/TenorGrabber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-29 08:46:08.000000 tenorgrabber-1.0.2/TenorGrabber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 08:46:08.000000 tenorgrabber-1.0.2/TenorGrabber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:46:08.000000 tenorgrabber-1.0.2/TenorGrabber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 08:46:08.000000 tenorgrabber-1.0.2/TenorGrabber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 08:46:08.000000 tenorgrabber-1.0.2/TenorGrabber.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:46:08.085304 tenorgrabber-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-29 08:46:04.000000 tenorgrabber-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:46:08.085304 tenorgrabber-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:46:04.000000 tenorgrabber-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-29 08:46:04.000000 tenorgrabber-1.0.2/tests/tenorgrabber.py
```

### Comparing `tenorgrabber-1.0.1/LICENSE` & `tenorgrabber-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tenorgrabber-1.0.1/PKG-INFO` & `tenorgrabber-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: TenorGrabber
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tired of /view links on tenor? This python library allows you to get the direct link of the GIF!
 Author: user0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # TenorGrabber
 Tired of /view links on tenor? This python library allows you to get the direct link of the GIF!
 Useful for discord/guilded bots to grab a tenor gif link and embed it
 <br>
 Usage:
 ```
```

### Comparing `tenorgrabber-1.0.1/README.md` & `tenorgrabber-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tenorgrabber-1.0.1/TenorGrabber.egg-info/PKG-INFO` & `tenorgrabber-1.0.2/TenorGrabber.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: TenorGrabber
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tired of /view links on tenor? This python library allows you to get the direct link of the GIF!
 Author: user0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # TenorGrabber
 Tired of /view links on tenor? This python library allows you to get the direct link of the GIF!
 Useful for discord/guilded bots to grab a tenor gif link and embed it
 <br>
 Usage:
 ```
```

### Comparing `tenorgrabber-1.0.1/setup.py` & `tenorgrabber-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
     name='TenorGrabber',
     packages=find_packages(),
-    version='1.0.1',
+    version='1.0.2',
     description='Tired of /view links on tenor? This python library allows you to get the direct link of the GIF!',
     author='user0',
-    install_reqs=[
+    install_requires=[
     'requests'
     ],
     long_description=long_description,
     long_description_content_type='text/markdown',
 )
```

