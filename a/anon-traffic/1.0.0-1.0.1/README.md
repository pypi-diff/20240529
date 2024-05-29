# Comparing `tmp/anon_traffic-1.0.0.tar.gz` & `tmp/anon_traffic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anon_traffic-1.0.0.tar", last modified: Wed May 29 13:08:05 2024, max compression
+gzip compressed data, was "anon_traffic-1.0.1.tar", last modified: Wed May 29 13:09:44 2024, max compression
```

## Comparing `anon_traffic-1.0.0.tar` & `anon_traffic-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:08:05.546951 anon_traffic-1.0.0/
--rw-r--r--   0 aimafan   (1001) aimafan   (1001)      638 2024-05-29 13:08:05.546951 anon_traffic-1.0.0/PKG-INFO
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      210 2024-05-29 12:59:11.000000 anon_traffic-1.0.0/README.md
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       38 2024-05-29 13:08:05.546951 anon_traffic-1.0.0/setup.cfg
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      850 2024-05-29 13:07:52.000000 anon_traffic-1.0.0/setup.py
-drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:08:05.544951 anon_traffic-1.0.0/src/
-drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:08:05.545951 anon_traffic-1.0.0/src/anon_traffic.egg-info/
--rw-r--r--   0 aimafan   (1001) aimafan   (1001)      638 2024-05-29 13:08:05.000000 anon_traffic-1.0.0/src/anon_traffic.egg-info/PKG-INFO
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      328 2024-05-29 13:08:05.000000 anon_traffic-1.0.0/src/anon_traffic.egg-info/SOURCES.txt
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)        1 2024-05-29 13:08:05.000000 anon_traffic-1.0.0/src/anon_traffic.egg-info/dependency_links.txt
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       62 2024-05-29 13:08:05.000000 anon_traffic-1.0.0/src/anon_traffic.egg-info/entry_points.txt
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       13 2024-05-29 13:08:05.000000 anon_traffic-1.0.0/src/anon_traffic.egg-info/requires.txt
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)        8 2024-05-29 13:08:05.000000 anon_traffic-1.0.0/src/anon_traffic.egg-info/top_level.txt
-drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:08:05.545951 anon_traffic-1.0.0/src/myutils/
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      120 2024-05-29 12:13:13.000000 anon_traffic-1.0.0/src/myutils/__init__.py
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      585 2024-05-29 12:13:13.000000 anon_traffic-1.0.0/src/myutils/config.py
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)     1439 2024-05-29 12:13:13.000000 anon_traffic-1.0.0/src/myutils/logger.py
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:09:44.548349 anon_traffic-1.0.1/
+-rw-r--r--   0 aimafan   (1001) aimafan   (1001)      638 2024-05-29 13:09:44.547349 anon_traffic-1.0.1/PKG-INFO
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      210 2024-05-29 12:59:11.000000 anon_traffic-1.0.1/README.md
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       38 2024-05-29 13:09:44.548349 anon_traffic-1.0.1/setup.cfg
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      858 2024-05-29 13:09:42.000000 anon_traffic-1.0.1/setup.py
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:09:44.546349 anon_traffic-1.0.1/src/
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:09:44.546349 anon_traffic-1.0.1/src/anon_traffic/
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 12:45:57.000000 anon_traffic-1.0.1/src/anon_traffic/__init__.py
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      519 2024-05-29 13:09:16.000000 anon_traffic-1.0.1/src/anon_traffic/disanon.py
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:09:44.547349 anon_traffic-1.0.1/src/anon_traffic/myutils/
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      120 2024-05-29 12:13:13.000000 anon_traffic-1.0.1/src/anon_traffic/myutils/__init__.py
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      585 2024-05-29 12:13:13.000000 anon_traffic-1.0.1/src/anon_traffic/myutils/config.py
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)     1439 2024-05-29 12:13:13.000000 anon_traffic-1.0.1/src/anon_traffic/myutils/logger.py
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      939 2024-05-29 12:31:29.000000 anon_traffic-1.0.1/src/anon_traffic/utils.py
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 13:09:44.547349 anon_traffic-1.0.1/src/anon_traffic.egg-info/
+-rw-r--r--   0 aimafan   (1001) aimafan   (1001)      638 2024-05-29 13:09:44.000000 anon_traffic-1.0.1/src/anon_traffic.egg-info/PKG-INFO
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      450 2024-05-29 13:09:44.000000 anon_traffic-1.0.1/src/anon_traffic.egg-info/SOURCES.txt
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)        1 2024-05-29 13:09:44.000000 anon_traffic-1.0.1/src/anon_traffic.egg-info/dependency_links.txt
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       70 2024-05-29 13:09:44.000000 anon_traffic-1.0.1/src/anon_traffic.egg-info/entry_points.txt
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       13 2024-05-29 13:09:44.000000 anon_traffic-1.0.1/src/anon_traffic.egg-info/requires.txt
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       13 2024-05-29 13:09:44.000000 anon_traffic-1.0.1/src/anon_traffic.egg-info/top_level.txt
```

### Comparing `anon_traffic-1.0.0/PKG-INFO` & `anon_traffic-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anon_traffic
-Version: 1.0.0
+Version: 1.0.1
 Summary: disanon ip and port
 Home-page: https://github.com/aimafan/anon_traffic
 Author: aimafan
 Author-email: chongrufan@nuaa.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anon_traffic-1.0.0/setup.py` & `anon_traffic-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="anon_traffic",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         # 在这里列出你的依赖包，例如：
         "cryptography",
     ],
     entry_points={
         "console_scripts": [
-            "anon_traffic.disanon=anon_traffic:disanon",
+            "anon_traffic.disanon=anon_traffic.disanon:disanon",
         ],
     },
     author="aimafan",
     author_email="chongrufan@nuaa.edu.cn",
     description="disanon ip and port",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `anon_traffic-1.0.0/src/anon_traffic.egg-info/PKG-INFO` & `anon_traffic-1.0.1/src/anon_traffic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anon_traffic
-Version: 1.0.0
+Version: 1.0.1
 Summary: disanon ip and port
 Home-page: https://github.com/aimafan/anon_traffic
 Author: aimafan
 Author-email: chongrufan@nuaa.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anon_traffic-1.0.0/src/myutils/config.py` & `anon_traffic-1.0.1/src/anon_traffic/myutils/config.py`

 * *Files identical despite different names*

### Comparing `anon_traffic-1.0.0/src/myutils/logger.py` & `anon_traffic-1.0.1/src/anon_traffic/myutils/logger.py`

 * *Files identical despite different names*

