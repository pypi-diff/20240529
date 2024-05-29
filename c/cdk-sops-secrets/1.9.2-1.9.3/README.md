# Comparing `tmp/cdk-sops-secrets-1.9.2.tar.gz` & `tmp/cdk-sops-secrets-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-sops-secrets-1.9.2.tar", last modified: Wed May 29 07:25:47 2024, max compression
+gzip compressed data, was "cdk-sops-secrets-1.9.3.tar", last modified: Wed May 29 19:47:25 2024, max compression
```

## Comparing `cdk-sops-secrets-1.9.2.tar` & `cdk-sops-secrets-1.9.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:25:47.117302 cdk-sops-secrets-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 07:25:35.000000 cdk-sops-secrets-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 07:25:35.000000 cdk-sops-secrets-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-29 07:25:47.117302 cdk-sops-secrets-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11721 2024-05-29 07:25:35.000000 cdk-sops-secrets-1.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 07:25:35.000000 cdk-sops-secrets-1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 07:25:47.117302 cdk-sops-secrets-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-29 07:25:35.000000 cdk-sops-secrets-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:25:47.101302 cdk-sops-secrets-1.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:25:47.105302 cdk-sops-secrets-1.9.2/src/cdk_sops_secrets/
--rw-r--r--   0 runner    (1001) docker     (127)    80660 2024-05-29 07:25:35.000000 cdk-sops-secrets-1.9.2/src/cdk_sops_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:25:47.105302 cdk-sops-secrets-1.9.2/src/cdk_sops_secrets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 07:25:35.000000 cdk-sops-secrets-1.9.2/src/cdk_sops_secrets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  8974560 2024-05-29 07:25:35.000000 cdk-sops-secrets-1.9.2/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.9.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 07:25:35.000000 cdk-sops-secrets-1.9.2/src/cdk_sops_secrets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:25:47.105302 cdk-sops-secrets-1.9.2/src/cdk_sops_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-29 07:25:47.000000 cdk-sops-secrets-1.9.2/src/cdk_sops_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-29 07:25:47.000000 cdk-sops-secrets-1.9.2/src/cdk_sops_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 07:25:47.000000 cdk-sops-secrets-1.9.2/src/cdk_sops_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-29 07:25:47.000000 cdk-sops-secrets-1.9.2/src/cdk_sops_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 07:25:47.000000 cdk-sops-secrets-1.9.2/src/cdk_sops_secrets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:47:25.331684 cdk-sops-secrets-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 19:47:13.000000 cdk-sops-secrets-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 19:47:13.000000 cdk-sops-secrets-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-29 19:47:25.331684 cdk-sops-secrets-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11721 2024-05-29 19:47:13.000000 cdk-sops-secrets-1.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 19:47:13.000000 cdk-sops-secrets-1.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:47:25.331684 cdk-sops-secrets-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-29 19:47:13.000000 cdk-sops-secrets-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:47:25.319684 cdk-sops-secrets-1.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:47:25.319684 cdk-sops-secrets-1.9.3/src/cdk_sops_secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)    80660 2024-05-29 19:47:13.000000 cdk-sops-secrets-1.9.3/src/cdk_sops_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:47:25.319684 cdk-sops-secrets-1.9.3/src/cdk_sops_secrets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 19:47:13.000000 cdk-sops-secrets-1.9.3/src/cdk_sops_secrets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  8975144 2024-05-29 19:47:13.000000 cdk-sops-secrets-1.9.3/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.9.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:47:13.000000 cdk-sops-secrets-1.9.3/src/cdk_sops_secrets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:47:25.319684 cdk-sops-secrets-1.9.3/src/cdk_sops_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-29 19:47:25.000000 cdk-sops-secrets-1.9.3/src/cdk_sops_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-29 19:47:25.000000 cdk-sops-secrets-1.9.3/src/cdk_sops_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:47:25.000000 cdk-sops-secrets-1.9.3/src/cdk_sops_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-29 19:47:25.000000 cdk-sops-secrets-1.9.3/src/cdk_sops_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 19:47:25.000000 cdk-sops-secrets-1.9.3/src/cdk_sops_secrets.egg-info/top_level.txt
```

### Comparing `cdk-sops-secrets-1.9.2/LICENSE` & `cdk-sops-secrets-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.9.2/PKG-INFO` & `cdk-sops-secrets-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.9.2
+Version: 1.9.3
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<markus.siebert@deutschebahn.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dbsystel/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-sops-secrets-1.9.2/README.md` & `cdk-sops-secrets-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.9.2/setup.py` & `cdk-sops-secrets-1.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-sops-secrets",
-    "version": "1.9.2",
+    "version": "1.9.3",
     "description": "CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.",
     "license": "Apache-2.0",
     "url": "https://constructs.dev/packages/cdk-sops-secrets",
     "long_description_content_type": "text/markdown",
     "author": "Markus Siebert<markus.siebert@deutschebahn.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_sops_secrets",
         "cdk_sops_secrets._jsii"
     ],
     "package_data": {
         "cdk_sops_secrets._jsii": [
-            "cdk-sops-secrets@1.9.2.jsii.tgz"
+            "cdk-sops-secrets@1.9.3.jsii.tgz"
         ],
         "cdk_sops_secrets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-sops-secrets-1.9.2/src/cdk_sops_secrets/__init__.py` & `cdk-sops-secrets-1.9.3/src/cdk_sops_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.9.2/src/cdk_sops_secrets.egg-info/PKG-INFO` & `cdk-sops-secrets-1.9.3/src/cdk_sops_secrets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.9.2
+Version: 1.9.3
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<markus.siebert@deutschebahn.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dbsystel/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

