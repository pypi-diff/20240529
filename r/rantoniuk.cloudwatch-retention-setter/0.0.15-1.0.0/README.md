# Comparing `tmp/rantoniuk.cloudwatch-retention-setter-0.0.15.tar.gz` & `tmp/rantoniuk.cloudwatch-retention-setter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rantoniuk.cloudwatch-retention-setter-0.0.15.tar", last modified: Thu Apr  4 12:49:11 2024, max compression
+gzip compressed data, was "rantoniuk.cloudwatch-retention-setter-1.0.0.tar", last modified: Wed May 29 11:11:32 2024, max compression
```

## Comparing `rantoniuk.cloudwatch-retention-setter-0.0.15.tar` & `rantoniuk.cloudwatch-retention-setter-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:49:11.122576 rantoniuk.cloudwatch-retention-setter-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 12:49:00.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 12:49:00.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-04 12:49:11.122576 rantoniuk.cloudwatch-retention-setter-0.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-04 12:49:00.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 12:49:00.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:49:11.122576 rantoniuk.cloudwatch-retention-setter-0.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-04 12:49:00.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:49:11.122576 rantoniuk.cloudwatch-retention-setter-0.0.15/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:49:11.122576 rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:49:11.122576 rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk/cloudwatch_retention_setter/
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-04 12:49:00.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk/cloudwatch_retention_setter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:49:11.122576 rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk/cloudwatch_retention_setter/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-04 12:49:00.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk/cloudwatch_retention_setter/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51561 2024-04-04 12:49:00.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk/cloudwatch_retention_setter/_jsii/cloudwatch-retention-setter@0.0.15.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:49:00.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk/cloudwatch_retention_setter/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:49:11.122576 rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk.cloudwatch_retention_setter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-04 12:49:11.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk.cloudwatch_retention_setter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-04 12:49:11.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk.cloudwatch_retention_setter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:49:11.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk.cloudwatch_retention_setter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 12:49:11.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk.cloudwatch_retention_setter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 12:49:11.000000 rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk.cloudwatch_retention_setter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:11:32.940813 rantoniuk.cloudwatch-retention-setter-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 11:11:22.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 11:11:22.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-29 11:11:32.940813 rantoniuk.cloudwatch-retention-setter-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-29 11:11:22.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 11:11:22.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 11:11:32.940813 rantoniuk.cloudwatch-retention-setter-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-29 11:11:22.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:11:32.940813 rantoniuk.cloudwatch-retention-setter-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:11:32.940813 rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:11:32.940813 rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk/cloudwatch_retention_setter/
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-29 11:11:22.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk/cloudwatch_retention_setter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:11:32.940813 rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk/cloudwatch_retention_setter/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-29 11:11:22.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk/cloudwatch_retention_setter/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51585 2024-05-29 11:11:22.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk/cloudwatch_retention_setter/_jsii/cloudwatch-retention-setter@1.0.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:11:22.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk/cloudwatch_retention_setter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:11:32.940813 rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk.cloudwatch_retention_setter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-29 11:11:32.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk.cloudwatch_retention_setter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-29 11:11:32.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk.cloudwatch_retention_setter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:11:32.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk.cloudwatch_retention_setter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-29 11:11:32.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk.cloudwatch_retention_setter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 11:11:32.000000 rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk.cloudwatch_retention_setter.egg-info/top_level.txt
```

### Comparing `rantoniuk.cloudwatch-retention-setter-0.0.15/LICENSE` & `rantoniuk.cloudwatch-retention-setter-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rantoniuk.cloudwatch-retention-setter-0.0.15/PKG-INFO` & `rantoniuk.cloudwatch-retention-setter-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rantoniuk.cloudwatch-retention-setter
-Version: 0.0.15
+Version: 1.0.0
 Summary: Based on EventBridge rule, automatically set the logGroup retention policy when new AWS CloudWatch logGroup is created.
 Home-page: https://github.com/rantoniuk/cloudwatch-retention-setter.git
 Author: Radek Antoniuk<radek.antoniuk@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/rantoniuk/cloudwatch-retention-setter.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `rantoniuk.cloudwatch-retention-setter-0.0.15/README.md` & `rantoniuk.cloudwatch-retention-setter-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `rantoniuk.cloudwatch-retention-setter-0.0.15/setup.py` & `rantoniuk.cloudwatch-retention-setter-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "rantoniuk.cloudwatch-retention-setter",
-    "version": "0.0.15",
+    "version": "1.0.0",
     "description": "Based on EventBridge rule, automatically set the logGroup retention policy when new AWS CloudWatch logGroup is created.",
     "license": "Apache-2.0",
     "url": "https://github.com/rantoniuk/cloudwatch-retention-setter.git",
     "long_description_content_type": "text/markdown",
     "author": "Radek Antoniuk<radek.antoniuk@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "rantoniuk.cloudwatch_retention_setter",
         "rantoniuk.cloudwatch_retention_setter._jsii"
     ],
     "package_data": {
         "rantoniuk.cloudwatch_retention_setter._jsii": [
-            "cloudwatch-retention-setter@0.0.15.jsii.tgz"
+            "cloudwatch-retention-setter@1.0.0.jsii.tgz"
         ],
         "rantoniuk.cloudwatch_retention_setter": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.1.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.96.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk/cloudwatch_retention_setter/__init__.py` & `rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk/cloudwatch_retention_setter/__init__.py`

 * *Files identical despite different names*

### Comparing `rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk.cloudwatch_retention_setter.egg-info/PKG-INFO` & `rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk.cloudwatch_retention_setter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rantoniuk.cloudwatch-retention-setter
-Version: 0.0.15
+Version: 1.0.0
 Summary: Based on EventBridge rule, automatically set the logGroup retention policy when new AWS CloudWatch logGroup is created.
 Home-page: https://github.com/rantoniuk/cloudwatch-retention-setter.git
 Author: Radek Antoniuk<radek.antoniuk@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/rantoniuk/cloudwatch-retention-setter.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `rantoniuk.cloudwatch-retention-setter-0.0.15/src/rantoniuk.cloudwatch_retention_setter.egg-info/SOURCES.txt` & `rantoniuk.cloudwatch-retention-setter-1.0.0/src/rantoniuk.cloudwatch_retention_setter.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/rantoniuk.cloudwatch_retention_setter.egg-info/SOURCES.txt
 src/rantoniuk.cloudwatch_retention_setter.egg-info/dependency_links.txt
 src/rantoniuk.cloudwatch_retention_setter.egg-info/requires.txt
 src/rantoniuk.cloudwatch_retention_setter.egg-info/top_level.txt
 src/rantoniuk/cloudwatch_retention_setter/__init__.py
 src/rantoniuk/cloudwatch_retention_setter/py.typed
 src/rantoniuk/cloudwatch_retention_setter/_jsii/__init__.py
-src/rantoniuk/cloudwatch_retention_setter/_jsii/cloudwatch-retention-setter@0.0.15.jsii.tgz
+src/rantoniuk/cloudwatch_retention_setter/_jsii/cloudwatch-retention-setter@1.0.0.jsii.tgz
```

