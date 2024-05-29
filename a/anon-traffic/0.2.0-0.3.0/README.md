# Comparing `tmp/anon_traffic-0.2.0.tar.gz` & `tmp/anon_traffic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anon_traffic-0.2.0.tar", last modified: Wed May 29 12:57:50 2024, max compression
+gzip compressed data, was "anon_traffic-0.3.0.tar", last modified: Wed May 29 12:59:42 2024, max compression
```

## Comparing `anon_traffic-0.2.0.tar` & `anon_traffic-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 12:57:50.772155 anon_traffic-0.2.0/
--rw-r--r--   0 aimafan   (1001) aimafan   (1001)      638 2024-05-29 12:57:50.771155 anon_traffic-0.2.0/PKG-INFO
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      210 2024-05-29 12:52:41.000000 anon_traffic-0.2.0/README.md
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       38 2024-05-29 12:57:50.772155 anon_traffic-0.2.0/setup.cfg
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      727 2024-05-29 12:57:46.000000 anon_traffic-0.2.0/setup.py
-drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 12:57:50.770155 anon_traffic-0.2.0/src/
-drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 12:57:50.771155 anon_traffic-0.2.0/src/anon_traffic.egg-info/
--rw-r--r--   0 aimafan   (1001) aimafan   (1001)      638 2024-05-29 12:57:50.000000 anon_traffic-0.2.0/src/anon_traffic.egg-info/PKG-INFO
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      285 2024-05-29 12:57:50.000000 anon_traffic-0.2.0/src/anon_traffic.egg-info/SOURCES.txt
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)        1 2024-05-29 12:57:50.000000 anon_traffic-0.2.0/src/anon_traffic.egg-info/dependency_links.txt
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       13 2024-05-29 12:57:50.000000 anon_traffic-0.2.0/src/anon_traffic.egg-info/requires.txt
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)        8 2024-05-29 12:57:50.000000 anon_traffic-0.2.0/src/anon_traffic.egg-info/top_level.txt
-drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 12:57:50.771155 anon_traffic-0.2.0/src/myutils/
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      120 2024-05-29 12:13:13.000000 anon_traffic-0.2.0/src/myutils/__init__.py
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      585 2024-05-29 12:13:13.000000 anon_traffic-0.2.0/src/myutils/config.py
--rw-rw-r--   0 aimafan   (1001) aimafan   (1001)     1439 2024-05-29 12:13:13.000000 anon_traffic-0.2.0/src/myutils/logger.py
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 12:59:42.579882 anon_traffic-0.3.0/
+-rw-r--r--   0 aimafan   (1001) aimafan   (1001)      638 2024-05-29 12:59:42.579882 anon_traffic-0.3.0/PKG-INFO
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      210 2024-05-29 12:59:11.000000 anon_traffic-0.3.0/README.md
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       38 2024-05-29 12:59:42.579882 anon_traffic-0.3.0/setup.cfg
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      727 2024-05-29 12:59:23.000000 anon_traffic-0.3.0/setup.py
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 12:59:42.578882 anon_traffic-0.3.0/src/
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 12:59:42.579882 anon_traffic-0.3.0/src/anon_traffic.egg-info/
+-rw-r--r--   0 aimafan   (1001) aimafan   (1001)      638 2024-05-29 12:59:42.000000 anon_traffic-0.3.0/src/anon_traffic.egg-info/PKG-INFO
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      285 2024-05-29 12:59:42.000000 anon_traffic-0.3.0/src/anon_traffic.egg-info/SOURCES.txt
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)        1 2024-05-29 12:59:42.000000 anon_traffic-0.3.0/src/anon_traffic.egg-info/dependency_links.txt
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)       13 2024-05-29 12:59:42.000000 anon_traffic-0.3.0/src/anon_traffic.egg-info/requires.txt
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)        8 2024-05-29 12:59:42.000000 anon_traffic-0.3.0/src/anon_traffic.egg-info/top_level.txt
+drwxrwxr-x   0 aimafan   (1001) aimafan   (1001)        0 2024-05-29 12:59:42.579882 anon_traffic-0.3.0/src/myutils/
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      120 2024-05-29 12:13:13.000000 anon_traffic-0.3.0/src/myutils/__init__.py
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)      585 2024-05-29 12:13:13.000000 anon_traffic-0.3.0/src/myutils/config.py
+-rw-rw-r--   0 aimafan   (1001) aimafan   (1001)     1439 2024-05-29 12:13:13.000000 anon_traffic-0.3.0/src/myutils/logger.py
```

### Comparing `anon_traffic-0.2.0/PKG-INFO` & `anon_traffic-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anon_traffic
-Version: 0.2.0
+Version: 0.3.0
 Summary: disanon ip and port
 Home-page: https://github.com/aimafan/anon_traffic
 Author: aimafan
 Author-email: chongrufan@nuaa.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anon_traffic-0.2.0/setup.py` & `anon_traffic-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="anon_traffic",
-    version="0.2.0",
+    version="0.3.0",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         # 在这里列出你的依赖包，例如：
         "cryptography",
     ],
     author="aimafan",
```

### Comparing `anon_traffic-0.2.0/src/anon_traffic.egg-info/PKG-INFO` & `anon_traffic-0.3.0/src/anon_traffic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anon_traffic
-Version: 0.2.0
+Version: 0.3.0
 Summary: disanon ip and port
 Home-page: https://github.com/aimafan/anon_traffic
 Author: aimafan
 Author-email: chongrufan@nuaa.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anon_traffic-0.2.0/src/myutils/config.py` & `anon_traffic-0.3.0/src/myutils/config.py`

 * *Files identical despite different names*

### Comparing `anon_traffic-0.2.0/src/myutils/logger.py` & `anon_traffic-0.3.0/src/myutils/logger.py`

 * *Files identical despite different names*

