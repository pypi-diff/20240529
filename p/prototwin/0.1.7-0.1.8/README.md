# Comparing `tmp/prototwin-0.1.7.tar.gz` & `tmp/prototwin-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prototwin-0.1.7.tar", last modified: Tue May 28 20:33:31 2024, max compression
+gzip compressed data, was "prototwin-0.1.8.tar", last modified: Wed May 29 07:02:52 2024, max compression
```

## Comparing `prototwin-0.1.7.tar` & `prototwin-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:33:31.794459 prototwin-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-28 20:33:17.000000 prototwin-0.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 20:33:17.000000 prototwin-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-28 20:33:31.794459 prototwin-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-28 20:33:17.000000 prototwin-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:33:31.790459 prototwin-0.1.7/prototwin/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:33:17.000000 prototwin-0.1.7/prototwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-28 20:33:17.000000 prototwin-0.1.7/prototwin/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:33:31.794459 prototwin-0.1.7/prototwin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-28 20:33:31.000000 prototwin-0.1.7/prototwin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 20:33:31.000000 prototwin-0.1.7/prototwin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:33:31.000000 prototwin-0.1.7/prototwin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 20:33:31.000000 prototwin-0.1.7/prototwin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 20:33:31.000000 prototwin-0.1.7/prototwin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-28 20:33:17.000000 prototwin-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 20:33:31.794459 prototwin-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-28 20:33:17.000000 prototwin-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:02:52.300811 prototwin-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-29 07:02:39.000000 prototwin-0.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 07:02:39.000000 prototwin-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-29 07:02:52.300811 prototwin-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-29 07:02:39.000000 prototwin-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:02:52.300811 prototwin-0.1.8/prototwin/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 07:02:39.000000 prototwin-0.1.8/prototwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-29 07:02:39.000000 prototwin-0.1.8/prototwin/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:02:52.300811 prototwin-0.1.8/prototwin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-29 07:02:52.000000 prototwin-0.1.8/prototwin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-29 07:02:52.000000 prototwin-0.1.8/prototwin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 07:02:52.000000 prototwin-0.1.8/prototwin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 07:02:52.000000 prototwin-0.1.8/prototwin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 07:02:52.000000 prototwin-0.1.8/prototwin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 07:02:39.000000 prototwin-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 07:02:52.300811 prototwin-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-29 07:02:39.000000 prototwin-0.1.8/setup.py
```

### Comparing `prototwin-0.1.7/LICENSE.txt` & `prototwin-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prototwin-0.1.7/PKG-INFO` & `prototwin-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prototwin
-Version: 0.1.7
+Version: 0.1.8
 Summary: The official python client interface for ProtoTwin Connect.
 Home-page: https://prototwin.com
 Author: ProtoTwin
 License: MIT
 Keywords: Industrial Simulation,Physics,Machine Learning,Robotics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `prototwin-0.1.7/README.md` & `prototwin-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `prototwin-0.1.7/prototwin.egg-info/PKG-INFO` & `prototwin-0.1.8/prototwin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prototwin
-Version: 0.1.7
+Version: 0.1.8
 Summary: The official python client interface for ProtoTwin Connect.
 Home-page: https://prototwin.com
 Author: ProtoTwin
 License: MIT
 Keywords: Industrial Simulation,Physics,Machine Learning,Robotics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `prototwin-0.1.7/setup.py` & `prototwin-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name = "prototwin",
     packages = find_packages(include=["prototwin"]),
-    version = "0.1.7",
+    version = "0.1.8",
     license = "MIT",
     description = "The official python client interface for ProtoTwin Connect.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     author = "ProtoTwin",
     url = "https://prototwin.com",
     keywords = ["Industrial Simulation", "Physics", "Machine Learning", "Robotics"],
```

