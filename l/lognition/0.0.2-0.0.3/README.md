# Comparing `tmp/lognition-0.0.2.tar.gz` & `tmp/lognition-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognition-0.0.2.tar", last modified: Tue May 28 23:53:06 2024, max compression
+gzip compressed data, was "lognition-0.0.3.tar", last modified: Wed May 29 00:05:58 2024, max compression
```

## Comparing `lognition-0.0.2.tar` & `lognition-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:53:06.252110 lognition-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 23:52:54.000000 lognition-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-28 23:53:06.252110 lognition-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-28 23:52:54.000000 lognition-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:53:06.248110 lognition-0.0.2/annonition/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-28 23:52:54.000000 lognition-0.0.2/annonition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-05-28 23:52:54.000000 lognition-0.0.2/annonition/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-28 23:52:54.000000 lognition-0.0.2/annonition/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:53:06.252110 lognition-0.0.2/lognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-28 23:53:06.000000 lognition-0.0.2/lognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-28 23:53:06.000000 lognition-0.0.2/lognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:53:06.000000 lognition-0.0.2/lognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 23:53:06.000000 lognition-0.0.2/lognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 23:53:06.000000 lognition-0.0.2/lognition.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:53:06.252110 lognition-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-28 23:52:54.000000 lognition-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:05:58.187209 lognition-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-29 00:05:47.000000 lognition-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-29 00:05:58.187209 lognition-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-29 00:05:47.000000 lognition-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:05:58.183209 lognition-0.0.3/lognition/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-29 00:05:47.000000 lognition-0.0.3/lognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-05-29 00:05:47.000000 lognition-0.0.3/lognition/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-29 00:05:47.000000 lognition-0.0.3/lognition/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:05:58.187209 lognition-0.0.3/lognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-29 00:05:58.000000 lognition-0.0.3/lognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-29 00:05:58.000000 lognition-0.0.3/lognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 00:05:58.000000 lognition-0.0.3/lognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-29 00:05:58.000000 lognition-0.0.3/lognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 00:05:58.000000 lognition-0.0.3/lognition.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 00:05:58.187209 lognition-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-29 00:05:47.000000 lognition-0.0.3/setup.py
```

### Comparing `lognition-0.0.2/LICENSE` & `lognition-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lognition-0.0.2/PKG-INFO` & `lognition-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognition
-Version: 0.0.2
+Version: 0.0.3
 Summary: Log everything in style.
 Author: Abtin Turing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lognition-0.0.2/README.md` & `lognition-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lognition-0.0.2/annonition/logger.py` & `lognition-0.0.3/lognition/logger.py`

 * *Files identical despite different names*

### Comparing `lognition-0.0.2/lognition.egg-info/PKG-INFO` & `lognition-0.0.3/lognition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognition
-Version: 0.0.2
+Version: 0.0.3
 Summary: Log everything in style.
 Author: Abtin Turing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lognition-0.0.2/setup.py` & `lognition-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open(path.join(working_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="lognition",
-    version="0.0.2",
+    version="0.0.3",
     author="Abtin Turing",
     description="Log everything in style.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

