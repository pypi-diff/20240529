# Comparing `tmp/elody-0.0.84.tar.gz` & `tmp/elody-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elody-0.0.84.tar", last modified: Wed May 29 16:57:29 2024, max compression
+gzip compressed data, was "elody-0.0.9.tar", last modified: Wed Jul 12 10:58:58 2023, max compression
```

## Comparing `elody-0.0.84.tar` & `elody-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:57:29.624688 elody-0.0.84/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-29 16:57:25.000000 elody-0.0.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23087 2024-05-29 16:57:29.624688 elody-0.0.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-29 16:57:25.000000 elody-0.0.84/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-29 16:57:25.000000 elody-0.0.84/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 16:57:29.624688 elody-0.0.84/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:57:29.616688 elody-0.0.84/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:57:25.000000 elody-0.0.84/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:57:29.620688 elody-0.0.84/src/elody/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:57:29.620688 elody-0.0.84/src/elody/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:57:29.620688 elody-0.0.84/src/elody/policies/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/authentication/base_user_tenant_validation_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/authentication/multi_tenant_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:57:29.620688 elody-0.0.84/src/elody/policies/authorization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/authorization/filter_generic_objects_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/authorization/generic_object_detail_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/authorization/generic_object_metadata_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/authorization/generic_object_relations_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/authorization/generic_object_request_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/authorization/multi_tenant_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/authorization/tenant_request_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/policies/permission_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-29 16:57:25.000000 elody-0.0.84/src/elody/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:57:29.624688 elody-0.0.84/src/elody.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23087 2024-05-29 16:57:29.000000 elody-0.0.84/src/elody.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-29 16:57:29.000000 elody-0.0.84/src/elody.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:57:29.000000 elody-0.0.84/src/elody.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 16:57:29.000000 elody-0.0.84/src/elody.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 16:57:29.000000 elody-0.0.84/src/elody.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:58:58.971030 elody-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-12 10:58:44.000000 elody-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 10:58:58.971030 elody-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-12 10:58:44.000000 elody-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-12 10:58:44.000000 elody-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:58:58.971030 elody-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:58:58.967030 elody-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:58:58.971030 elody-0.0.9/src/elody/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 10:58:44.000000 elody-0.0.9/src/elody/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-12 10:58:44.000000 elody-0.0.9/src/elody/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-12 10:58:44.000000 elody-0.0.9/src/elody/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-12 10:58:44.000000 elody-0.0.9/src/elody/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-12 10:58:44.000000 elody-0.0.9/src/elody/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:58:58.971030 elody-0.0.9/src/elody.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 10:58:58.000000 elody-0.0.9/src/elody.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-12 10:58:58.000000 elody-0.0.9/src/elody.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:58:58.000000 elody-0.0.9/src/elody.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-12 10:58:58.000000 elody-0.0.9/src/elody.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 10:58:58.000000 elody-0.0.9/src/elody.egg-info/top_level.txt
```

### Comparing `elody-0.0.84/LICENSE` & `elody-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `elody-0.0.84/PKG-INFO` & `elody-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elody
-Version: 0.0.84
+Version: 0.0.9
 Summary: elody SDK for Python
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -349,33 +349,25 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: certifi>=2023.5.7
-Requires-Dist: charset-normalizer>=3.2.0
-Requires-Dist: idna>=3.4
-Requires-Dist: requests>=2.31.0
-Requires-Dist: urllib3>=1.26.16
 Provides-Extra: loader
-Requires-Dist: cloudevents>=1.9.0; extra == "loader"
-Requires-Dist: inuits-policy-based-auth>=9.6.0; extra == "loader"
 Provides-Extra: util
-Requires-Dist: cloudevents>=1.9.0; extra == "util"
+License-File: LICENSE
 
 # elody SDK for Python
 
 ## Installation
 
 To install the Python SDK library using pip:
 ```
-pip install elody
+pip install elody-python-sdk
 ```
 
 ## Usage
 
 Begin by importing the `elody` module:
 ```
 import elody
```

### Comparing `elody-0.0.84/README.md` & `elody-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # elody SDK for Python
 
 ## Installation
 
 To install the Python SDK library using pip:
 ```
-pip install elody
+pip install elody-python-sdk
 ```
 
 ## Usage
 
 Begin by importing the `elody` module:
 ```
 import elody
```

### Comparing `elody-0.0.84/pyproject.toml` & `elody-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elody"
-version = "0.0.84"
+version = "0.0.9"
 description = "elody SDK for Python"
 readme = "README.md"
 authors = [{ name = "Inuits", email = "developers@inuits.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
   "Intended Audience :: Developers",
@@ -18,25 +18,25 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 keywords = ["elody", "SDK"]
 dependencies = [
-  "certifi>=2023.5.7",
-  "charset-normalizer>=3.2.0",
-  "idna>=3.4",
-  "requests>=2.31.0",
+  "certifi==2023.5.7",
+  "charset-normalizer==3.2.0",
+  "idna==3.4",
+  "requests==2.31.0",
   "urllib3>=1.26.16",
 ]
 
 [project.optional-dependencies]
 loader = [
-  "cloudevents>=1.9.0",
-  "inuits-policy-based-auth>=9.6.0",
+  "cloudevents==1.9.0",
+  "inuits-policy-based-auth==4.1.0",
 ]
 util = [
-  "cloudevents>=1.9.0",
+  "cloudevents==1.9.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/inuits/elody-python-sdk"
```

### Comparing `elody-0.0.84/src/elody.egg-info/PKG-INFO` & `elody-0.0.9/src/elody.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elody
-Version: 0.0.84
+Version: 0.0.9
 Summary: elody SDK for Python
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -349,33 +349,25 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: certifi>=2023.5.7
-Requires-Dist: charset-normalizer>=3.2.0
-Requires-Dist: idna>=3.4
-Requires-Dist: requests>=2.31.0
-Requires-Dist: urllib3>=1.26.16
 Provides-Extra: loader
-Requires-Dist: cloudevents>=1.9.0; extra == "loader"
-Requires-Dist: inuits-policy-based-auth>=9.6.0; extra == "loader"
 Provides-Extra: util
-Requires-Dist: cloudevents>=1.9.0; extra == "util"
+License-File: LICENSE
 
 # elody SDK for Python
 
 ## Installation
 
 To install the Python SDK library using pip:
 ```
-pip install elody
+pip install elody-python-sdk
 ```
 
 ## Usage
 
 Begin by importing the `elody` module:
 ```
 import elody
```

