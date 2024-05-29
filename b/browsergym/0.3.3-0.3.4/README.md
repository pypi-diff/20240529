# Comparing `tmp/browsergym-0.3.3.tar.gz` & `tmp/browsergym-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browsergym-0.3.3.tar", last modified: Fri May 24 20:05:55 2024, max compression
+gzip compressed data, was "browsergym-0.3.4.tar", last modified: Wed May 29 15:01:40 2024, max compression
```

## Comparing `browsergym-0.3.3.tar` & `browsergym-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:05:55.158759 browsergym-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-24 20:05:39.000000 browsergym-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-24 20:05:55.158759 browsergym-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-24 20:05:39.000000 browsergym-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:05:55.158759 browsergym-0.3.3/browsergym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-24 20:05:55.000000 browsergym-0.3.3/browsergym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-24 20:05:55.000000 browsergym-0.3.3/browsergym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:05:55.000000 browsergym-0.3.3/browsergym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-24 20:05:55.000000 browsergym-0.3.3/browsergym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:05:55.000000 browsergym-0.3.3/browsergym.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-24 20:05:39.000000 browsergym-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 20:05:55.158759 browsergym-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:01:40.060007 browsergym-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-29 15:01:22.000000 browsergym-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-29 15:01:40.060007 browsergym-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-29 15:01:22.000000 browsergym-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:01:40.060007 browsergym-0.3.4/browsergym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-29 15:01:40.000000 browsergym-0.3.4/browsergym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-29 15:01:40.000000 browsergym-0.3.4/browsergym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:01:40.000000 browsergym-0.3.4/browsergym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-29 15:01:40.000000 browsergym-0.3.4/browsergym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:01:40.000000 browsergym-0.3.4/browsergym.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-29 15:01:22.000000 browsergym-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:01:40.060007 browsergym-0.3.4/setup.cfg
```

### Comparing `browsergym-0.3.3/LICENSE` & `browsergym-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `browsergym-0.3.3/PKG-INFO` & `browsergym-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: browsergym
-Version: 0.3.3
+Version: 0.3.4
 Summary: BrowserGym: a gym environment for web task automation in the Chromium browser
 Author: Rim Assouel, Léo Boisvert, Massimo Caccia, Alex Drouin, Maxime Gasse, Alex Lacoste, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: browsergym-core==0.3.3
-Requires-Dist: browsergym-miniwob==0.3.3
-Requires-Dist: browsergym-webarena==0.3.3
-Requires-Dist: browsergym-experiments==0.3.3
+Requires-Dist: browsergym-core==0.3.4
+Requires-Dist: browsergym-miniwob==0.3.4
+Requires-Dist: browsergym-webarena==0.3.4
+Requires-Dist: browsergym-experiments==0.3.4
 Requires-Dist: browsergym-workarena
 
 # BrowserGym: a Gym Environment for Web Task Automation
 
 [[Setup]](#setup) ♦ [[Usage]](#usage) ♦ [[Demo]](#demo)
 
 This package provides `browsergym`, a gym environment for web task automation in the Chromium browser.
```

### Comparing `browsergym-0.3.3/README.md` & `browsergym-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `browsergym-0.3.3/browsergym.egg-info/PKG-INFO` & `browsergym-0.3.4/browsergym.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: browsergym
-Version: 0.3.3
+Version: 0.3.4
 Summary: BrowserGym: a gym environment for web task automation in the Chromium browser
 Author: Rim Assouel, Léo Boisvert, Massimo Caccia, Alex Drouin, Maxime Gasse, Alex Lacoste, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: browsergym-core==0.3.3
-Requires-Dist: browsergym-miniwob==0.3.3
-Requires-Dist: browsergym-webarena==0.3.3
-Requires-Dist: browsergym-experiments==0.3.3
+Requires-Dist: browsergym-core==0.3.4
+Requires-Dist: browsergym-miniwob==0.3.4
+Requires-Dist: browsergym-webarena==0.3.4
+Requires-Dist: browsergym-experiments==0.3.4
 Requires-Dist: browsergym-workarena
 
 # BrowserGym: a Gym Environment for Web Task Automation
 
 [[Setup]](#setup) ♦ [[Usage]](#usage) ♦ [[Demo]](#demo)
 
 This package provides `browsergym`, a gym environment for web task automation in the Chromium browser.
```

### Comparing `browsergym-0.3.3/pyproject.toml` & `browsergym-0.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: Apache Software License",
 ]
-version="0.3.3"
+version="0.3.4"
 dependencies = [
-    "browsergym-core==0.3.3",
-    "browsergym-miniwob==0.3.3",
-    "browsergym-webarena==0.3.3",
-    "browsergym-experiments==0.3.3",
+    "browsergym-core==0.3.4",
+    "browsergym-miniwob==0.3.4",
+    "browsergym-webarena==0.3.4",
+    "browsergym-experiments==0.3.4",
     "browsergym-workarena",
 ]
 
 [tool.setuptools]
 packages = []  # meta distribution, packages are included as dependencies
 
 [tool.black]
```

