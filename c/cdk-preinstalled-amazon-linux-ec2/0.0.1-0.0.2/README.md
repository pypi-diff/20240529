# Comparing `tmp/cdk-preinstalled-amazon-linux-ec2-0.0.1.tar.gz` & `tmp/cdk-preinstalled-amazon-linux-ec2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-preinstalled-amazon-linux-ec2-0.0.1.tar", last modified: Wed May 29 12:43:09 2024, max compression
+gzip compressed data, was "cdk-preinstalled-amazon-linux-ec2-0.0.2.tar", last modified: Wed May 29 13:07:26 2024, max compression
```

## Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.1.tar` & `cdk-preinstalled-amazon-linux-ec2-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:43:09.212707 cdk-preinstalled-amazon-linux-ec2-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-29 12:43:09.212707 cdk-preinstalled-amazon-linux-ec2-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:43:09.212707 cdk-preinstalled-amazon-linux-ec2-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:43:09.208707 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:43:09.208707 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/
--rw-r--r--   0 runner    (1001) docker     (127)    54253 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:43:09.212707 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26914 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/_jsii/cdk-preinstalled-amazon-linux-ec2@0.0.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:43:09.212707 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-29 12:43:09.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-29 12:43:09.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:43:09.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-29 12:43:09.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-29 12:43:09.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:07:26.816539 cdk-preinstalled-amazon-linux-ec2-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-29 13:07:26.816539 cdk-preinstalled-amazon-linux-ec2-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:07:26.816539 cdk-preinstalled-amazon-linux-ec2-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:07:26.812539 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:07:26.812539 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)    54253 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:07:26.816539 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26913 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/_jsii/cdk-preinstalled-amazon-linux-ec2@0.0.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:07:26.816539 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-29 13:07:26.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-29 13:07:26.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:07:26.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-29 13:07:26.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-29 13:07:26.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/top_level.txt
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.1/LICENSE` & `cdk-preinstalled-amazon-linux-ec2-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.1/PKG-INFO` & `cdk-preinstalled-amazon-linux-ec2-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-preinstalled-amazon-linux-ec2
-Version: 0.0.1
+Version: 0.0.2
 Summary: CDK Construct for creating an Amazon Linux EC2 instance with pre-installed software
 Home-page: https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.1/README.md` & `cdk-preinstalled-amazon-linux-ec2-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.1/setup.py` & `cdk-preinstalled-amazon-linux-ec2-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-preinstalled-amazon-linux-ec2",
-    "version": "0.0.1",
+    "version": "0.0.2",
     "description": "CDK Construct for creating an Amazon Linux EC2 instance with pre-installed software",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_preinstalled_amazon_linux_ec2",
         "cdk_preinstalled_amazon_linux_ec2._jsii"
     ],
     "package_data": {
         "cdk_preinstalled_amazon_linux_ec2._jsii": [
-            "cdk-preinstalled-amazon-linux-ec2@0.0.1.jsii.tgz"
+            "cdk-preinstalled-amazon-linux-ec2@0.0.2.jsii.tgz"
         ],
         "cdk_preinstalled_amazon_linux_ec2": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/__init__.py` & `cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py` & `cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "cdk-preinstalled-amazon-linux-ec2",
-    "0.0.1",
+    "0.0.2",
     __name__[0:-6],
-    "cdk-preinstalled-amazon-linux-ec2@0.0.1.jsii.tgz",
+    "cdk-preinstalled-amazon-linux-ec2@0.0.2.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/PKG-INFO` & `cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-preinstalled-amazon-linux-ec2
-Version: 0.0.1
+Version: 0.0.2
 Summary: CDK Construct for creating an Amazon Linux EC2 instance with pre-installed software
 Home-page: https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt` & `cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_preinstalled_amazon_linux_ec2/py.typed
 src/cdk_preinstalled_amazon_linux_ec2.egg-info/PKG-INFO
 src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt
 src/cdk_preinstalled_amazon_linux_ec2.egg-info/dependency_links.txt
 src/cdk_preinstalled_amazon_linux_ec2.egg-info/requires.txt
 src/cdk_preinstalled_amazon_linux_ec2.egg-info/top_level.txt
 src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py
-src/cdk_preinstalled_amazon_linux_ec2/_jsii/cdk-preinstalled-amazon-linux-ec2@0.0.1.jsii.tgz
+src/cdk_preinstalled_amazon_linux_ec2/_jsii/cdk-preinstalled-amazon-linux-ec2@0.0.2.jsii.tgz
```

