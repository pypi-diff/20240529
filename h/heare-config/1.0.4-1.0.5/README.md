# Comparing `tmp/heare_config-1.0.4.tar.gz` & `tmp/heare_config-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heare_config-1.0.4.tar", last modified: Mon May 13 06:29:02 2024, max compression
+gzip compressed data, was "heare_config-1.0.5.tar", last modified: Tue May 28 01:27:27 2024, max compression
```

## Comparing `heare_config-1.0.4.tar` & `heare_config-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:29:02.582966 heare_config-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-13 06:28:53.000000 heare_config-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-13 06:29:02.582966 heare_config-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-05-13 06:28:53.000000 heare_config-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:29:02.578966 heare_config-1.0.4/heare/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:29:02.578966 heare_config-1.0.4/heare/config/
--rw-r--r--   0 runner    (1001) docker     (127)    18070 2024-05-13 06:28:53.000000 heare_config-1.0.4/heare/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:29:02.582966 heare_config-1.0.4/heare_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-13 06:29:02.000000 heare_config-1.0.4/heare_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 06:29:02.000000 heare_config-1.0.4/heare_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 06:29:02.000000 heare_config-1.0.4/heare_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 06:29:02.000000 heare_config-1.0.4/heare_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 06:29:02.582966 heare_config-1.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      542 2024-05-13 06:28:53.000000 heare_config-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:29:02.582966 heare_config-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-13 06:28:53.000000 heare_config-1.0.4/tests/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-13 06:28:53.000000 heare_config-1.0.4/tests/test_setting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:27:27.644220 heare_config-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-28 01:27:14.000000 heare_config-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-28 01:27:27.644220 heare_config-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-05-28 01:27:14.000000 heare_config-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:27:27.640220 heare_config-1.0.5/heare/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:27:27.640220 heare_config-1.0.5/heare/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-05-28 01:27:14.000000 heare_config-1.0.5/heare/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:27:27.644220 heare_config-1.0.5/heare_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-28 01:27:27.000000 heare_config-1.0.5/heare_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-28 01:27:27.000000 heare_config-1.0.5/heare_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:27:27.000000 heare_config-1.0.5/heare_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 01:27:27.000000 heare_config-1.0.5/heare_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:27:27.644220 heare_config-1.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      542 2024-05-28 01:27:14.000000 heare_config-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:27:27.644220 heare_config-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-28 01:27:14.000000 heare_config-1.0.5/tests/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-28 01:27:14.000000 heare_config-1.0.5/tests/test_setting.py
```

### Comparing `heare_config-1.0.4/LICENSE` & `heare_config-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `heare_config-1.0.4/PKG-INFO` & `heare_config-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heare-config
-Version: 1.0.4
+Version: 1.0.5
 Summary: Heare.io Configuration Utilities
 Home-page: https://github.com/heare-io/heare-config
 Author: Sean Fitzgerald
 Author-email: seanfitz@heare.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `heare_config-1.0.4/README.md` & `heare_config-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `heare_config-1.0.4/heare/config/__init__.py` & `heare_config-1.0.5/heare/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import glob
 import os
 import re
 import sys
 import typing
 from abc import ABCMeta, abstractmethod
 from collections import defaultdict
 from json import JSONEncoder
@@ -445,22 +446,40 @@
                 if child not in subclasses:
                     subclasses.add(child)
                     work.append(child)
         return subclasses
 
     @classmethod
     def load(cls,
-             args: List[str] = sys.argv,
+             args: Union[List[str], None] = None,
              env: FlexibleEnvironType = os.environ,
-             config_files: List[str] = []):
+             config_files: Union[List[str], None] = None):
         sources: List[SettingsSource] = []
 
+        if not args:
+            args = sys.argv
+
+        if not config_files:
+            config_files = []
+            # check environ config
+            # this is a PATH-like string, containing either files or directories
+            # directories are not traversed recursively
+            env_var = os.environ.get('HEARE_CONFIG_PATH', '')
+            parts = env_var.split(os.pathsep)
+            for part in parts:
+                if os.path.isdir(part):
+                    for f in glob.glob(part + os.path.sep + '*.ini'):
+                        config_files.append(f)
+                if os.path.isfile(part):
+                    config_files.append(part)
+
         for file in config_files:
             if os.path.exists(file):
                 sources.append(ConfigFileSource.from_filename(file))
+
         if env:
             sources.append(EnvironSettingsSource(env))
         if args:
             sources.append(CLISettingsSource(args))
 
         return SettingsDefinition.load_for_class(cls, sources)
```

### Comparing `heare_config-1.0.4/heare_config.egg-info/PKG-INFO` & `heare_config-1.0.5/heare_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heare-config
-Version: 1.0.4
+Version: 1.0.5
 Summary: Heare.io Configuration Utilities
 Home-page: https://github.com/heare-io/heare-config
 Author: Sean Fitzgerald
 Author-email: seanfitz@heare.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `heare_config-1.0.4/setup.py` & `heare_config-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 long_description = None
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(name='heare-config',
-      version='1.0.4',
+      version='1.0.5',
       description='Heare.io Configuration Utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       author='Sean Fitzgerald',
       author_email='seanfitz@heare.io',
       url='https://github.com/heare-io/heare-config',
       packages=['heare.config'],
```

### Comparing `heare_config-1.0.4/tests/test_cli_parsing.py` & `heare_config-1.0.5/tests/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `heare_config-1.0.4/tests/test_setting.py` & `heare_config-1.0.5/tests/test_setting.py`

 * *Files identical despite different names*

