# Comparing `tmp/cdktf-cdktf-provider-time-9.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-time-9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-time-9.0.1.tar", last modified: Mon Dec  4 13:58:55 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-time-9.0.2.tar", last modified: Thu Dec  7 11:59:00 2023, max compression
```

## Comparing `cdktf-cdktf-provider-time-9.0.1.tar` & `cdktf-cdktf-provider-time-9.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 13:58:55.269001 cdktf-cdktf-provider-time-9.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    16012 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2023-12-04 13:58:55.265001 cdktf-cdktf-provider-time-9.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-04 13:58:55.269001 cdktf-cdktf-provider-time-9.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 13:58:55.265001 cdktf-cdktf-provider-time-9.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 13:58:55.265001 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 13:58:55.265001 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37811 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/_jsii/provider-time@9.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 13:58:55.265001 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/offset/
--rw-r--r--   0 runner    (1001) docker     (127)    38654 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/offset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 13:58:55.265001 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/provider/
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 13:58:55.265001 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/rotating/
--rw-r--r--   0 runner    (1001) docker     (127)    41756 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/rotating/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 13:58:55.265001 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/sleep/
--rw-r--r--   0 runner    (1001) docker     (127)    24572 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/sleep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 13:58:55.265001 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/static_resource/
--rw-r--r--   0 runner    (1001) docker     (127)    22129 2023-12-04 13:58:43.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/static_resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 13:58:55.265001 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2023-12-04 13:58:55.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-04 13:58:55.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 13:58:55.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-04 13:58:55.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-04 13:58:55.000000 cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:59:00.758580 cdktf-cdktf-provider-time-9.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16012 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2023-12-07 11:59:00.758580 cdktf-cdktf-provider-time-9.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 11:59:00.758580 cdktf-cdktf-provider-time-9.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:59:00.754580 cdktf-cdktf-provider-time-9.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:59:00.758580 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:59:00.758580 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37022 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/_jsii/provider-time@9.0.2.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:59:00.758580 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/offset/
+-rw-r--r--   0 runner    (1001) docker     (127)    38682 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/offset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:59:00.758580 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:59:00.758580 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/rotating/
+-rw-r--r--   0 runner    (1001) docker     (127)    41784 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/rotating/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:59:00.758580 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/sleep/
+-rw-r--r--   0 runner    (1001) docker     (127)    24585 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/sleep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:59:00.758580 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/static_resource/
+-rw-r--r--   0 runner    (1001) docker     (127)    22139 2023-12-07 11:58:50.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/static_resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:59:00.758580 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2023-12-07 11:59:00.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-07 11:59:00.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 11:59:00.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-07 11:59:00.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-07 11:59:00.000000 cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-time-9.0.1/LICENSE` & `cdktf-cdktf-provider-time-9.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-time-9.0.1/PKG-INFO` & `cdktf-cdktf-provider-time-9.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-time
-Version: 9.0.1
+Version: 9.0.2
 Summary: Prebuilt time Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-time.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-time.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Terraform CDK time Provider tracks ~> 0.7
 
 This repo builds and publishes the Terraform time Provider bindings for [CDK for Terraform](https://cdk.tf).
 
-Is based directly on time 0.9.2
+Is based directly on time 0.10.0
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-time](https://www.npmjs.com/package/@cdktf/provider-time).
 
@@ -80,15 +80,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform time Provider version 1:1. In fact, it always tracks `latest` of `~> 0.7` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform time Provider](https://registry.terraform.io/providers/hashicorp/time/0.9.2)
+* [Terraform time Provider](https://registry.terraform.io/providers/hashicorp/time/0.10.0)
 
   * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-time/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
```

### Comparing `cdktf-cdktf-provider-time-9.0.1/README.md` & `cdktf-cdktf-provider-time-9.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Terraform CDK time Provider tracks ~> 0.7
 
 This repo builds and publishes the Terraform time Provider bindings for [CDK for Terraform](https://cdk.tf).
 
-Is based directly on time 0.9.2
+Is based directly on time 0.10.0
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-time](https://www.npmjs.com/package/@cdktf/provider-time).
 
@@ -57,15 +57,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform time Provider version 1:1. In fact, it always tracks `latest` of `~> 0.7` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform time Provider](https://registry.terraform.io/providers/hashicorp/time/0.9.2)
+* [Terraform time Provider](https://registry.terraform.io/providers/hashicorp/time/0.10.0)
 
   * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-time/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
```

### Comparing `cdktf-cdktf-provider-time-9.0.1/setup.py` & `cdktf-cdktf-provider-time-9.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-time",
-    "version": "9.0.1",
+    "version": "9.0.2",
     "description": "Prebuilt time Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-time.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -27,15 +27,15 @@
         "cdktf_cdktf_provider_time.provider",
         "cdktf_cdktf_provider_time.rotating",
         "cdktf_cdktf_provider_time.sleep",
         "cdktf_cdktf_provider_time.static_resource"
     ],
     "package_data": {
         "cdktf_cdktf_provider_time._jsii": [
-            "provider-time@9.0.1.jsii.tgz"
+            "provider-time@9.0.2.jsii.tgz"
         ],
         "cdktf_cdktf_provider_time": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/__init__.py` & `cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 # Terraform CDK time Provider tracks ~> 0.7
 
 This repo builds and publishes the Terraform time Provider bindings for [CDK for Terraform](https://cdk.tf).
 
-Is based directly on time 0.9.2
+Is based directly on time 0.10.0
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-time](https://www.npmjs.com/package/@cdktf/provider-time).
 
@@ -58,15 +58,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform time Provider version 1:1. In fact, it always tracks `latest` of `~> 0.7` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform time Provider](https://registry.terraform.io/providers/hashicorp/time/0.9.2)
+* [Terraform time Provider](https://registry.terraform.io/providers/hashicorp/time/0.10.0)
 
   * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-time/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
```

### Comparing `cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/offset/__init__.py` & `cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/offset/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `time_offset`
 
-Refer to the Terraform Registory for docs: [`time_offset`](https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset).
+Refer to the Terraform Registory for docs: [`time_offset`](https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Offset(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-time.offset.Offset",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset time_offset}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset time_offset}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         base_rfc3339: typing.Optional[builtins.str] = None,
@@ -45,26 +45,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset time_offset} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset time_offset} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param base_rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#base_rfc3339 Offset#base_rfc3339}
-        :param offset_days: Number of days to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_days Offset#offset_days}
-        :param offset_hours: Number of hours to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_hours Offset#offset_hours}
-        :param offset_minutes: Number of minutes to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_minutes Offset#offset_minutes}
-        :param offset_months: Number of months to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_months Offset#offset_months}
-        :param offset_seconds: Number of seconds to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_seconds Offset#offset_seconds}
-        :param offset_years: Number of years to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_years Offset#offset_years}
-        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#triggers Offset#triggers}
+        :param base_rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#base_rfc3339 Offset#base_rfc3339}
+        :param offset_days: Number of days to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_days Offset#offset_days}
+        :param offset_hours: Number of hours to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_hours Offset#offset_hours}
+        :param offset_minutes: Number of minutes to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_minutes Offset#offset_minutes}
+        :param offset_months: Number of months to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_months Offset#offset_months}
+        :param offset_seconds: Number of seconds to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_seconds Offset#offset_seconds}
+        :param offset_years: Number of years to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_years Offset#offset_years}
+        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#triggers Offset#triggers}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -102,15 +102,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Offset resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Offset to import.
-        :param import_from_id: The id of the existing Offset that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Offset that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Offset to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ed990d9310f975fba57041307e2315d24379b797f25f62ca7dfcdc8f750c81ea)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -387,22 +387,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param base_rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#base_rfc3339 Offset#base_rfc3339}
-        :param offset_days: Number of days to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_days Offset#offset_days}
-        :param offset_hours: Number of hours to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_hours Offset#offset_hours}
-        :param offset_minutes: Number of minutes to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_minutes Offset#offset_minutes}
-        :param offset_months: Number of months to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_months Offset#offset_months}
-        :param offset_seconds: Number of seconds to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_seconds Offset#offset_seconds}
-        :param offset_years: Number of years to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_years Offset#offset_years}
-        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#triggers Offset#triggers}
+        :param base_rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#base_rfc3339 Offset#base_rfc3339}
+        :param offset_days: Number of days to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_days Offset#offset_days}
+        :param offset_hours: Number of hours to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_hours Offset#offset_hours}
+        :param offset_minutes: Number of minutes to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_minutes Offset#offset_minutes}
+        :param offset_months: Number of months to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_months Offset#offset_months}
+        :param offset_seconds: Number of seconds to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_seconds Offset#offset_seconds}
+        :param offset_years: Number of years to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_years Offset#offset_years}
+        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#triggers Offset#triggers}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__129647c305336dbf1cae2ce70d04cb6a6fee40863714fac62a4bfe71187fa828)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -515,80 +515,80 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def base_rfc3339(self) -> typing.Optional[builtins.str]:
         '''Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#base_rfc3339 Offset#base_rfc3339}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#base_rfc3339 Offset#base_rfc3339}
         '''
         result = self._values.get("base_rfc3339")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def offset_days(self) -> typing.Optional[jsii.Number]:
         '''Number of days to offset the base timestamp. At least one of the 'offset_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_days Offset#offset_days}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_days Offset#offset_days}
         '''
         result = self._values.get("offset_days")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def offset_hours(self) -> typing.Optional[jsii.Number]:
         '''Number of hours to offset the base timestamp. At least one of the 'offset_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_hours Offset#offset_hours}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_hours Offset#offset_hours}
         '''
         result = self._values.get("offset_hours")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def offset_minutes(self) -> typing.Optional[jsii.Number]:
         '''Number of minutes to offset the base timestamp. At least one of the 'offset_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_minutes Offset#offset_minutes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_minutes Offset#offset_minutes}
         '''
         result = self._values.get("offset_minutes")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def offset_months(self) -> typing.Optional[jsii.Number]:
         '''Number of months to offset the base timestamp. At least one of the 'offset_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_months Offset#offset_months}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_months Offset#offset_months}
         '''
         result = self._values.get("offset_months")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def offset_seconds(self) -> typing.Optional[jsii.Number]:
         '''Number of seconds to offset the base timestamp. At least one of the 'offset_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_seconds Offset#offset_seconds}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_seconds Offset#offset_seconds}
         '''
         result = self._values.get("offset_seconds")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def offset_years(self) -> typing.Optional[jsii.Number]:
         '''Number of years to offset the base timestamp. At least one of the 'offset_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#offset_years Offset#offset_years}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#offset_years Offset#offset_years}
         '''
         result = self._values.get("offset_years")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def triggers(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved.
 
         See `the main provider documentation <../index.md>`_ for more information.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/offset#triggers Offset#triggers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/offset#triggers Offset#triggers}
         '''
         result = self._values.get("triggers")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/provider/__init__.py` & `cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`time`](https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs).
+Refer to the Terraform Registory for docs: [`time`](https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,28 +22,28 @@
 
 
 class TimeProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-time.provider.TimeProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs time}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs time}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs time} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs time} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs#alias TimeProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs#alias TimeProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c869539a3d05780607af068e02b355518195eadc27a829071227e5c37a3a6b69)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = TimeProviderConfig(alias=alias)
 
@@ -58,15 +58,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a TimeProvider resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the TimeProvider to import.
-        :param import_from_id: The id of the existing TimeProvider that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing TimeProvider that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the TimeProvider to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__70cbc7965ebe6aa806c83665b51c440a7732523f04cc40d141db6727787caaee)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -108,28 +108,28 @@
     jsii_type="@cdktf/provider-time.provider.TimeProviderConfig",
     jsii_struct_bases=[],
     name_mapping={"alias": "alias"},
 )
 class TimeProviderConfig:
     def __init__(self, *, alias: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs#alias TimeProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs#alias TimeProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__77704b117f84b4019cf445d89efdcfb386e41b68dfdf53448bbb9298a0e4435f)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if alias is not None:
             self._values["alias"] = alias
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs#alias TimeProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs#alias TimeProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/rotating/__init__.py` & `cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/rotating/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `time_rotating`
 
-Refer to the Terraform Registory for docs: [`time_rotating`](https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating).
+Refer to the Terraform Registory for docs: [`time_rotating`](https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Rotating(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-time.rotating.Rotating",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating time_rotating}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating time_rotating}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         rfc3339: typing.Optional[builtins.str] = None,
@@ -45,26 +45,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating time_rotating} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating time_rotating} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rfc3339 Rotating#rfc3339}
-        :param rotation_days: Number of days to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_days Rotating#rotation_days}
-        :param rotation_hours: Number of hours to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_hours Rotating#rotation_hours}
-        :param rotation_minutes: Number of minutes to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_minutes Rotating#rotation_minutes}
-        :param rotation_months: Number of months to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_months Rotating#rotation_months}
-        :param rotation_rfc3339: Configure the rotation timestamp with an `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format of the offset timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_rfc3339 Rotating#rotation_rfc3339}
-        :param rotation_years: Number of years to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_years Rotating#rotation_years}
-        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. These conditions recreate the resource in addition to other rotation arguments. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#triggers Rotating#triggers}
+        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rfc3339 Rotating#rfc3339}
+        :param rotation_days: Number of days to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_days Rotating#rotation_days}
+        :param rotation_hours: Number of hours to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_hours Rotating#rotation_hours}
+        :param rotation_minutes: Number of minutes to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_minutes Rotating#rotation_minutes}
+        :param rotation_months: Number of months to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_months Rotating#rotation_months}
+        :param rotation_rfc3339: Configure the rotation timestamp with an `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format of the offset timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_rfc3339 Rotating#rotation_rfc3339}
+        :param rotation_years: Number of years to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_years Rotating#rotation_years}
+        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. These conditions recreate the resource in addition to other rotation arguments. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#triggers Rotating#triggers}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -102,15 +102,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Rotating resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Rotating to import.
-        :param import_from_id: The id of the existing Rotating that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Rotating that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Rotating to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__04cf0e3e1ad621f1ad0c9b4ff22367eb972d94fc45af03cbdb50440a60db6caf)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -382,22 +382,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rfc3339 Rotating#rfc3339}
-        :param rotation_days: Number of days to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_days Rotating#rotation_days}
-        :param rotation_hours: Number of hours to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_hours Rotating#rotation_hours}
-        :param rotation_minutes: Number of minutes to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_minutes Rotating#rotation_minutes}
-        :param rotation_months: Number of months to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_months Rotating#rotation_months}
-        :param rotation_rfc3339: Configure the rotation timestamp with an `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format of the offset timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_rfc3339 Rotating#rotation_rfc3339}
-        :param rotation_years: Number of years to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_years Rotating#rotation_years}
-        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. These conditions recreate the resource in addition to other rotation arguments. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#triggers Rotating#triggers}
+        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rfc3339 Rotating#rfc3339}
+        :param rotation_days: Number of days to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_days Rotating#rotation_days}
+        :param rotation_hours: Number of hours to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_hours Rotating#rotation_hours}
+        :param rotation_minutes: Number of minutes to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_minutes Rotating#rotation_minutes}
+        :param rotation_months: Number of months to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_months Rotating#rotation_months}
+        :param rotation_rfc3339: Configure the rotation timestamp with an `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format of the offset timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_rfc3339 Rotating#rotation_rfc3339}
+        :param rotation_years: Number of years to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_years Rotating#rotation_years}
+        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. These conditions recreate the resource in addition to other rotation arguments. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#triggers Rotating#triggers}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9ff127dfa3aa123c42955f732770508fb130fcb2094145ead1fd7fbe2809aa7e)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -510,90 +510,90 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def rfc3339(self) -> typing.Optional[builtins.str]:
         '''Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rfc3339 Rotating#rfc3339}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rfc3339 Rotating#rfc3339}
         '''
         result = self._values.get("rfc3339")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def rotation_days(self) -> typing.Optional[jsii.Number]:
         '''Number of days to add to the base timestamp to configure the rotation timestamp.
 
         When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_days Rotating#rotation_days}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_days Rotating#rotation_days}
         '''
         result = self._values.get("rotation_days")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def rotation_hours(self) -> typing.Optional[jsii.Number]:
         '''Number of hours to add to the base timestamp to configure the rotation timestamp.
 
         When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_hours Rotating#rotation_hours}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_hours Rotating#rotation_hours}
         '''
         result = self._values.get("rotation_hours")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def rotation_minutes(self) -> typing.Optional[jsii.Number]:
         '''Number of minutes to add to the base timestamp to configure the rotation timestamp.
 
         When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_minutes Rotating#rotation_minutes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_minutes Rotating#rotation_minutes}
         '''
         result = self._values.get("rotation_minutes")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def rotation_months(self) -> typing.Optional[jsii.Number]:
         '''Number of months to add to the base timestamp to configure the rotation timestamp.
 
         When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_months Rotating#rotation_months}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_months Rotating#rotation_months}
         '''
         result = self._values.get("rotation_months")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def rotation_rfc3339(self) -> typing.Optional[builtins.str]:
         '''Configure the rotation timestamp with an `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format of the offset timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_rfc3339 Rotating#rotation_rfc3339}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_rfc3339 Rotating#rotation_rfc3339}
         '''
         result = self._values.get("rotation_rfc3339")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def rotation_years(self) -> typing.Optional[jsii.Number]:
         '''Number of years to add to the base timestamp to configure the rotation timestamp.
 
         When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#rotation_years Rotating#rotation_years}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#rotation_years Rotating#rotation_years}
         '''
         result = self._values.get("rotation_years")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def triggers(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved.
 
         These conditions recreate the resource in addition to other rotation arguments. See `the main provider documentation <../index.md>`_ for more information.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/rotating#triggers Rotating#triggers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/rotating#triggers Rotating#triggers}
         '''
         result = self._values.get("triggers")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/sleep/__init__.py` & `cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/sleep/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `time_sleep`
 
-Refer to the Terraform Registory for docs: [`time_sleep`](https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/sleep).
+Refer to the Terraform Registory for docs: [`time_sleep`](https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/sleep).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Sleep(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-time.sleep.Sleep",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/sleep time_sleep}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/sleep time_sleep}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         create_duration: typing.Optional[builtins.str] = None,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/sleep time_sleep} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/sleep time_sleep} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param create_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource creation. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/sleep#create_duration Sleep#create_duration}
-        :param destroy_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource destroy. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. This value or any updates to it must be successfully applied into the Terraform state before destroying this resource to take effect. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/sleep#destroy_duration Sleep#destroy_duration}
-        :param triggers: (Optional) Arbitrary map of values that, when changed, will run any creation or destroy delays again. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/sleep#triggers Sleep#triggers}
+        :param create_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource creation. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/sleep#create_duration Sleep#create_duration}
+        :param destroy_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource destroy. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. This value or any updates to it must be successfully applied into the Terraform state before destroying this resource to take effect. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/sleep#destroy_duration Sleep#destroy_duration}
+        :param triggers: (Optional) Arbitrary map of values that, when changed, will run any creation or destroy delays again. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/sleep#triggers Sleep#triggers}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -87,15 +87,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Sleep resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Sleep to import.
-        :param import_from_id: The id of the existing Sleep that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/sleep#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Sleep that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/sleep#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Sleep to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__954fd4060c3a8b2f73884935070c97c401c34712d9ecd134b24a45b09f16d634)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -217,17 +217,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param create_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource creation. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/sleep#create_duration Sleep#create_duration}
-        :param destroy_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource destroy. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. This value or any updates to it must be successfully applied into the Terraform state before destroying this resource to take effect. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/sleep#destroy_duration Sleep#destroy_duration}
-        :param triggers: (Optional) Arbitrary map of values that, when changed, will run any creation or destroy delays again. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/sleep#triggers Sleep#triggers}
+        :param create_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource creation. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/sleep#create_duration Sleep#create_duration}
+        :param destroy_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource destroy. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. This value or any updates to it must be successfully applied into the Terraform state before destroying this resource to take effect. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/sleep#destroy_duration Sleep#destroy_duration}
+        :param triggers: (Optional) Arbitrary map of values that, when changed, will run any creation or destroy delays again. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/sleep#triggers Sleep#triggers}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2a5326ad9173cd184a5987482265cc897932e1ea5d86f4294def627dc1a98c34)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -325,35 +325,35 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def create_duration(self) -> typing.Optional[builtins.str]:
         '''`Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource creation. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/sleep#create_duration Sleep#create_duration}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/sleep#create_duration Sleep#create_duration}
         '''
         result = self._values.get("create_duration")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def destroy_duration(self) -> typing.Optional[builtins.str]:
         '''`Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource destroy. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. This value or any updates to it must be successfully applied into the Terraform state before destroying this resource to take effect.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/sleep#destroy_duration Sleep#destroy_duration}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/sleep#destroy_duration Sleep#destroy_duration}
         '''
         result = self._values.get("destroy_duration")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def triggers(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''(Optional) Arbitrary map of values that, when changed, will run any creation or destroy delays again.
 
         See `the main provider documentation <../index.md>`_ for more information.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/sleep#triggers Sleep#triggers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/sleep#triggers Sleep#triggers}
         '''
         result = self._values.get("triggers")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time/static_resource/__init__.py` & `cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time/static_resource/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `time_static`
 
-Refer to the Terraform Registory for docs: [`time_static`](https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/static).
+Refer to the Terraform Registory for docs: [`time_static`](https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/static).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class StaticResource(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-time.staticResource.StaticResource",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/static time_static}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/static time_static}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         rfc3339: typing.Optional[builtins.str] = None,
@@ -39,20 +39,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/static time_static} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/static time_static} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/static#rfc3339 StaticResource#rfc3339}
-        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/static#triggers StaticResource#triggers}
+        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/static#rfc3339 StaticResource#rfc3339}
+        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/static#triggers StaticResource#triggers}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -84,15 +84,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a StaticResource resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the StaticResource to import.
-        :param import_from_id: The id of the existing StaticResource that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/static#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing StaticResource that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/static#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the StaticResource to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1a49174803abefe09d52915b356749cbb8bbea1df2040babd8c23918d52dbb78)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -226,16 +226,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/static#rfc3339 StaticResource#rfc3339}
-        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/static#triggers StaticResource#triggers}
+        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/static#rfc3339 StaticResource#rfc3339}
+        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/static#triggers StaticResource#triggers}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4c379934e27cbed249355b819eba1f15c20fc2c2b6039e308a1ebfcb6edc88e6)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -330,26 +330,26 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def rfc3339(self) -> typing.Optional[builtins.str]:
         '''Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/static#rfc3339 StaticResource#rfc3339}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/static#rfc3339 StaticResource#rfc3339}
         '''
         result = self._values.get("rfc3339")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def triggers(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved.
 
         See `the main provider documentation <../index.md>`_ for more information.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.2/docs/resources/static#triggers StaticResource#triggers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.10.0/docs/resources/static#triggers StaticResource#triggers}
         '''
         result = self._values.get("triggers")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time.egg-info/PKG-INFO` & `cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-time
-Version: 9.0.1
+Version: 9.0.2
 Summary: Prebuilt time Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-time.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-time.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Terraform CDK time Provider tracks ~> 0.7
 
 This repo builds and publishes the Terraform time Provider bindings for [CDK for Terraform](https://cdk.tf).
 
-Is based directly on time 0.9.2
+Is based directly on time 0.10.0
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-time](https://www.npmjs.com/package/@cdktf/provider-time).
 
@@ -80,15 +80,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform time Provider version 1:1. In fact, it always tracks `latest` of `~> 0.7` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform time Provider](https://registry.terraform.io/providers/hashicorp/time/0.9.2)
+* [Terraform time Provider](https://registry.terraform.io/providers/hashicorp/time/0.10.0)
 
   * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-time/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
```

### Comparing `cdktf-cdktf-provider-time-9.0.1/src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-time-9.0.2/src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/cdktf_cdktf_provider_time/py.typed
 src/cdktf_cdktf_provider_time.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_time.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_time.egg-info/requires.txt
 src/cdktf_cdktf_provider_time.egg-info/top_level.txt
 src/cdktf_cdktf_provider_time/_jsii/__init__.py
-src/cdktf_cdktf_provider_time/_jsii/provider-time@9.0.1.jsii.tgz
+src/cdktf_cdktf_provider_time/_jsii/provider-time@9.0.2.jsii.tgz
 src/cdktf_cdktf_provider_time/offset/__init__.py
 src/cdktf_cdktf_provider_time/provider/__init__.py
 src/cdktf_cdktf_provider_time/rotating/__init__.py
 src/cdktf_cdktf_provider_time/sleep/__init__.py
 src/cdktf_cdktf_provider_time/static_resource/__init__.py
```

