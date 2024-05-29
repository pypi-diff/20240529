# Comparing `tmp/anon_traffic-1.0.1.tar.gz` & `tmp/anon_traffic-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anon_traffic-1.0.1.tar", last modified: Wed May 29 13:09:44 2024, max compression
+gzip compressed data, was "anon_traffic-1.0.2.tar", last modified: Wed May 29 13:10:39 2024, max compression
```

## Comparing `anon_traffic-1.0.1.tar` & `anon_traffic-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:09:44.548349 anon_traffic-1.0.1/
--rw-r--r--   0 aimafan   (1001) aimafan   (1001)      638 2024-05-29 13:09:44.547349 anon_traffic-1.0.1/PKG-INFO
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      210 2024-05-29 12:59:11.000000 anon_traffic-1.0.1/README.md
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       38 2024-05-29 13:09:44.548349 anon_traffic-1.0.1/setup.cfg
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      858 2024-05-29 13:09:42.000000 anon_traffic-1.0.1/setup.py
-drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:09:44.546349 anon_traffic-1.0.1/src/
-drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:09:44.546349 anon_traffic-1.0.1/src/anon_traffic/
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 12:45:57.000000 anon_traffic-1.0.1/src/anon_traffic/__init__.py
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      519 2024-05-29 13:09:16.000000 anon_traffic-1.0.1/src/anon_traffic/disanon.py
-drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:09:44.547349 anon_traffic-1.0.1/src/anon_traffic/myutils/
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      120 2024-05-29 12:13:13.000000 anon_traffic-1.0.1/src/anon_traffic/myutils/__init__.py
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      585 2024-05-29 12:13:13.000000 anon_traffic-1.0.1/src/anon_traffic/myutils/config.py
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)     1439 2024-05-29 12:13:13.000000 anon_traffic-1.0.1/src/anon_traffic/myutils/logger.py
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      939 2024-05-29 12:31:29.000000 anon_traffic-1.0.1/src/anon_traffic/utils.py
-drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:09:44.547349 anon_traffic-1.0.1/src/anon_traffic.egg-info/
--rw-r--r--   0 aimafan   (1001) aimafan   (1001)      638 2024-05-29 13:09:44.000000 anon_traffic-1.0.1/src/anon_traffic.egg-info/PKG-INFO
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      450 2024-05-29 13:09:44.000000 anon_traffic-1.0.1/src/anon_traffic.egg-info/SOURCES.txt
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)        1 2024-05-29 13:09:44.000000 anon_traffic-1.0.1/src/anon_traffic.egg-info/dependency_links.txt
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       70 2024-05-29 13:09:44.000000 anon_traffic-1.0.1/src/anon_traffic.egg-info/entry_points.txt
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       13 2024-05-29 13:09:44.000000 anon_traffic-1.0.1/src/anon_traffic.egg-info/requires.txt
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       13 2024-05-29 13:09:44.000000 anon_traffic-1.0.1/src/anon_traffic.egg-info/top_level.txt
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:10:39.819624 anon_traffic-1.0.2/
+-rw-r--r--   0 aimafan   (1001) aimafan   (1001)      638 2024-05-29 13:10:39.819624 anon_traffic-1.0.2/PKG-INFO
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      210 2024-05-29 12:59:11.000000 anon_traffic-1.0.2/README.md
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       38 2024-05-29 13:10:39.819624 anon_traffic-1.0.2/setup.cfg
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      858 2024-05-29 13:10:28.000000 anon_traffic-1.0.2/setup.py
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:10:39.817624 anon_traffic-1.0.2/src/
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:10:39.818624 anon_traffic-1.0.2/src/anon_traffic/
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 12:45:57.000000 anon_traffic-1.0.2/src/anon_traffic/__init__.py
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      519 2024-05-29 13:09:48.000000 anon_traffic-1.0.2/src/anon_traffic/anon_traffic.py
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      519 2024-05-29 13:09:16.000000 anon_traffic-1.0.2/src/anon_traffic/disanon.py
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:10:39.818624 anon_traffic-1.0.2/src/anon_traffic/myutils/
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      120 2024-05-29 12:13:13.000000 anon_traffic-1.0.2/src/anon_traffic/myutils/__init__.py
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      585 2024-05-29 12:13:13.000000 anon_traffic-1.0.2/src/anon_traffic/myutils/config.py
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)     1439 2024-05-29 12:13:13.000000 anon_traffic-1.0.2/src/anon_traffic/myutils/logger.py
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      939 2024-05-29 12:31:29.000000 anon_traffic-1.0.2/src/anon_traffic/utils.py
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:10:39.819624 anon_traffic-1.0.2/src/anon_traffic.egg-info/
+-rw-r--r--   0 aimafan   (1001) aimafan   (1001)      638 2024-05-29 13:10:39.000000 anon_traffic-1.0.2/src/anon_traffic.egg-info/PKG-INFO
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      483 2024-05-29 13:10:39.000000 anon_traffic-1.0.2/src/anon_traffic.egg-info/SOURCES.txt
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)        1 2024-05-29 13:10:39.000000 anon_traffic-1.0.2/src/anon_traffic.egg-info/dependency_links.txt
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       70 2024-05-29 13:10:39.000000 anon_traffic-1.0.2/src/anon_traffic.egg-info/entry_points.txt
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       13 2024-05-29 13:10:39.000000 anon_traffic-1.0.2/src/anon_traffic.egg-info/requires.txt
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       13 2024-05-29 13:10:39.000000 anon_traffic-1.0.2/src/anon_traffic.egg-info/top_level.txt
```

### Comparing `anon_traffic-1.0.1/PKG-INFO` & `anon_traffic-1.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anon_traffic
-Version: 1.0.1
+Version: 1.0.2
 Summary: disanon ip and port
 Home-page: https://github.com/aimafan/anon_traffic
 Author: aimafan
 Author-email: chongrufan@nuaa.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anon_traffic-1.0.1/setup.py` & `anon_traffic-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="anon_traffic",
-    version="1.0.1",
+    version="1.0.2",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         # 在这里列出你的依赖包，例如：
         "cryptography",
     ],
     entry_points={
```

### Comparing `anon_traffic-1.0.1/src/anon_traffic/disanon.py` & `anon_traffic-1.0.2/src/anon_traffic/anon_traffic.py`

 * *Files identical despite different names*

### Comparing `anon_traffic-1.0.1/src/anon_traffic/myutils/config.py` & `anon_traffic-1.0.2/src/anon_traffic/myutils/config.py`

 * *Files identical despite different names*

### Comparing `anon_traffic-1.0.1/src/anon_traffic/myutils/logger.py` & `anon_traffic-1.0.2/src/anon_traffic/myutils/logger.py`

 * *Files identical despite different names*

### Comparing `anon_traffic-1.0.1/src/anon_traffic/utils.py` & `anon_traffic-1.0.2/src/anon_traffic/utils.py`

 * *Files identical despite different names*

### Comparing `anon_traffic-1.0.1/src/anon_traffic.egg-info/PKG-INFO` & `anon_traffic-1.0.2/src/anon_traffic.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anon_traffic
-Version: 1.0.1
+Version: 1.0.2
 Summary: disanon ip and port
 Home-page: https://github.com/aimafan/anon_traffic
 Author: aimafan
 Author-email: chongrufan@nuaa.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

