# Comparing `tmp/cdk-preinstalled-amazon-linux-ec2-0.0.0.tar.gz` & `tmp/cdk-preinstalled-amazon-linux-ec2-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-preinstalled-amazon-linux-ec2-0.0.0.tar", last modified: Mon May 27 14:20:50 2024, max compression
+gzip compressed data, was "cdk-preinstalled-amazon-linux-ec2-0.0.1.tar", last modified: Wed May 29 12:43:09 2024, max compression
```

## Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.0.tar` & `cdk-preinstalled-amazon-linux-ec2-0.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:50.985770 cdk-preinstalled-amazon-linux-ec2-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-27 14:20:40.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 14:20:40.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-27 14:20:50.985770 cdk-preinstalled-amazon-linux-ec2-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 14:20:40.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-27 14:20:40.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:20:50.985770 cdk-preinstalled-amazon-linux-ec2-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-27 14:20:40.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:50.985770 cdk-preinstalled-amazon-linux-ec2-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:50.985770 cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2/
--rw-r--r--   0 runner    (1001) docker     (127)    50605 2024-05-27 14:20:40.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:50.985770 cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-27 14:20:40.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24510 2024-05-27 14:20:40.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2/_jsii/cdk-preinstalled-amazon-linux-ec2@0.0.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:20:40.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:50.985770 cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-27 14:20:50.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-27 14:20:50.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:20:50.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-27 14:20:50.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 14:20:50.000000 cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:43:09.212707 cdk-preinstalled-amazon-linux-ec2-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-29 12:43:09.212707 cdk-preinstalled-amazon-linux-ec2-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:43:09.212707 cdk-preinstalled-amazon-linux-ec2-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:43:09.208707 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:43:09.208707 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)    54253 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:43:09.212707 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26914 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/_jsii/cdk-preinstalled-amazon-linux-ec2@0.0.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:42:59.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:43:09.212707 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-29 12:43:09.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-29 12:43:09.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:43:09.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-29 12:43:09.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-29 12:43:09.000000 cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/top_level.txt
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.0/LICENSE` & `cdk-preinstalled-amazon-linux-ec2-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.0/setup.py` & `cdk-preinstalled-amazon-linux-ec2-0.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-preinstalled-amazon-linux-ec2",
-    "version": "0.0.0",
+    "version": "0.0.1",
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
-            "cdk-preinstalled-amazon-linux-ec2@0.0.0.jsii.tgz"
+            "cdk-preinstalled-amazon-linux-ec2@0.0.1.jsii.tgz"
         ],
         "cdk_preinstalled_amazon_linux_ec2": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2/__init__.py` & `cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,100 @@
 '''
-# replace this
+# CDK Preinstalled Amazon Linux EC2 Instance Construct
+
+This is a CDK Construct for creating a preinstalled AmazonLinux EC2 instance.
+
+You can use Node.js, Visual Studio Code, git and other software as soon as the EC2 instance starts.
+
+[![View on Construct Hub](https://constructs.dev/badge?package=cdk-preinstalled-amazon-linux-ec2)](https://constructs.dev/packages/cdk-preinstalled-amazon-linux-ec2)
+
+[![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-preinstalled-amazon-linux-ec2)
+[![npm version](https://badge.fury.io/js/cdk-preinstalled-amazon-linux-ec2.svg)](https://badge.fury.io/js/cdk-preinstalled-amazon-linux-ec2)
+[![Build Status](https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2/actions/workflows/build.yml)
+[![Release Status](https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2/actions/workflows/release.yml)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![npm downloads](https://img.shields.io/npm/dm/cdk-preinstalled-amazon-linux-ec2.svg?style=flat)](https://www.npmjs.com/package/cdk-preinstalled-amazon-linux-ec2)
+
+## Usage
+
+Install the package:
+
+```bash
+npm install cdk-preinstalled-amazon-linux-ec2
+```
+
+Use it in your CDK stack:
+
+```python
+import { PreinstalledAmazonLinuxInstance } from 'cdk-preinstalled-amazon-linux-ec2';
+import * as ec2 from 'aws-cdk-lib/aws-ec2';
+
+declare const vpc: ec2.IVpc;
+
+// You can configure all properties of the EC2 instance
+new PreinstalledAmazonLinuxInstance(this, 'Instance', {
+  vpc,
+  instanceType: ec2.InstanceType.of(ec2.InstanceClass.T3, ec2.InstanceSize.NANO),
+  machineImage: new ec2.AmazonLinuxImage({
+    generation: ec2.AmazonLinuxGeneration.AMAZON_LINUX_2023,
+  }),
+  // Specify preinstalled software
+  preinstalledSoftware: {
+    type: [
+      PreinstalledSoftwareType.NODEJS,
+      PreinstalledSoftwareType.VSCODE,
+      PreinstalledSoftwareType.GIT,
+    ],
+    others: ['rsyslog'], // You can specify other software packages. These parameters are used as `sudo dnf install ${parameter}`
+});
+```
+
+After the stack is deployed, you can SSH into the EC2 instance and use Node.js:
+
+```bash
+$ ssh ec2-user@<public-ip>
+$ node --version
+v20.13.1
+$ code --version
+1.89.1
+$ git --version
+git version 2.39.3
+```
+
+## user data
+
+Installation of software is done by user data script. You can see the script in the `src/index.ts` file.
+
+```python
+// Install Node.js
+userData.addCommands(
+  'touch ~/.bashrc',
+  'curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash',
+  'source ~/.bashrc',
+  'export NVM_DIR="$HOME/.nvm"',
+  '[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"',
+  `nvm install ${props.nodeJsVersion ?? '--lts'}`,
+  // Note that the above will install nvm, node and npm for the root user.
+  // It will not add the correct ENV VAR in ec2-user's environment.
+  `cat <<EOF >> /home/ec2-user/.bashrc
+export NVM_DIR="/.nvm"
+[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
+EOF`);
+```
+
+Ofcourse, you can customize the additional user data script by calling `instance.userData.addCommands()` method.
+
+```python
+declare const instance: PreinstalledAmazonLinuxInstance;
+
+// install Postgresql
+instance.userData.addCommands(
+  'sudo dnf install -y postgresql15-server'
+);
+```
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py` & `cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "cdk-preinstalled-amazon-linux-ec2",
-    "0.0.0",
+    "0.0.1",
     __name__[0:-6],
-    "cdk-preinstalled-amazon-linux-ec2@0.0.0.jsii.tgz",
+    "cdk-preinstalled-amazon-linux-ec2@0.0.1.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.0/src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt` & `cdk-preinstalled-amazon-linux-ec2-0.0.1/src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt`

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
-src/cdk_preinstalled_amazon_linux_ec2/_jsii/cdk-preinstalled-amazon-linux-ec2@0.0.0.jsii.tgz
+src/cdk_preinstalled_amazon_linux_ec2/_jsii/cdk-preinstalled-amazon-linux-ec2@0.0.1.jsii.tgz
```

