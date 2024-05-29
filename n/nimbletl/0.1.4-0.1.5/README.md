# Comparing `tmp/nimbletl-0.1.4.tar.gz` & `tmp/nimbletl-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimbletl-0.1.4.tar", last modified: Tue May 28 08:44:31 2024, max compression
+gzip compressed data, was "nimbletl-0.1.5.tar", last modified: Tue May 28 08:49:04 2024, max compression
```

## Comparing `nimbletl-0.1.4.tar` & `nimbletl-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 08:44:31.554530 nimbletl-0.1.4/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 08:44:31.554217 nimbletl-0.1.4/PKG-INFO
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      217 2024-05-28 06:32:53.000000 nimbletl-0.1.4/README.md
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 08:44:31.551296 nimbletl-0.1.4/log_driver/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 03:12:18.000000 nimbletl-0.1.4/log_driver/__init__.py
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 08:44:31.552094 nimbletl-0.1.4/log_driver/init/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 03:12:25.000000 nimbletl-0.1.4/log_driver/init/__init__.py
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      782 2024-05-28 06:42:38.000000 nimbletl-0.1.4/log_driver/init/cli.py
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)     1365 2024-05-28 06:44:00.000000 nimbletl-0.1.4/log_driver/init/db.py
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 08:44:31.553863 nimbletl-0.1.4/nimbletl.egg-info/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 08:44:31.000000 nimbletl-0.1.4/nimbletl.egg-info/PKG-INFO
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      308 2024-05-28 08:44:31.000000 nimbletl-0.1.4/nimbletl.egg-info/SOURCES.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-28 08:44:31.000000 nimbletl-0.1.4/nimbletl.egg-info/dependency_links.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       54 2024-05-28 08:44:31.000000 nimbletl-0.1.4/nimbletl.egg-info/entry_points.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       57 2024-05-28 08:44:31.000000 nimbletl-0.1.4/nimbletl.egg-info/requires.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       11 2024-05-28 08:44:31.000000 nimbletl-0.1.4/nimbletl.egg-info/top_level.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       38 2024-05-28 08:44:31.554606 nimbletl-0.1.4/setup.cfg
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      742 2024-05-28 08:41:19.000000 nimbletl-0.1.4/setup.py
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 08:49:04.431060 nimbletl-0.1.5/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 08:49:04.430747 nimbletl-0.1.5/PKG-INFO
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      217 2024-05-28 06:32:53.000000 nimbletl-0.1.5/README.md
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 08:49:04.427521 nimbletl-0.1.5/log_driver/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 03:12:18.000000 nimbletl-0.1.5/log_driver/__init__.py
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 08:49:04.428511 nimbletl-0.1.5/log_driver/init/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 03:12:25.000000 nimbletl-0.1.5/log_driver/init/__init__.py
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      778 2024-05-28 08:46:37.000000 nimbletl-0.1.5/log_driver/init/cli.py
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)     1365 2024-05-28 06:44:00.000000 nimbletl-0.1.5/log_driver/init/db.py
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 08:49:04.430400 nimbletl-0.1.5/nimbletl.egg-info/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 08:49:04.000000 nimbletl-0.1.5/nimbletl.egg-info/PKG-INFO
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      308 2024-05-28 08:49:04.000000 nimbletl-0.1.5/nimbletl.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-28 08:49:04.000000 nimbletl-0.1.5/nimbletl.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       54 2024-05-28 08:49:04.000000 nimbletl-0.1.5/nimbletl.egg-info/entry_points.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       57 2024-05-28 08:49:04.000000 nimbletl-0.1.5/nimbletl.egg-info/requires.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       11 2024-05-28 08:49:04.000000 nimbletl-0.1.5/nimbletl.egg-info/top_level.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       38 2024-05-28 08:49:04.431128 nimbletl-0.1.5/setup.cfg
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      742 2024-05-28 08:48:34.000000 nimbletl-0.1.5/setup.py
```

### Comparing `nimbletl-0.1.4/log_driver/init/cli.py` & `nimbletl-0.1.5/log_driver/init/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import click
 import yaml
 
-from src.log_driver.init.db import initialize_database
+from log_driver.init.db import initialize_database
 
 
 @click.group()
 def main():
     pass
```

### Comparing `nimbletl-0.1.4/log_driver/init/db.py` & `nimbletl-0.1.5/log_driver/init/db.py`

 * *Files identical despite different names*

### Comparing `nimbletl-0.1.4/setup.py` & `nimbletl-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         lock_data = json.load(f)
     dependencies = lock_data['default']
     return [f"{pkg}{info.get('version', '')}" for pkg, info in dependencies.items()]
 
 
 setuptools.setup(
     name='nimbletl',
-    version='0.1.4',
+    version='0.1.5',
     packages=setuptools.find_packages(),
     install_requires=parse_pipfile_lock(),
     entry_points={
         'console_scripts': [
             'nimbletl=log_driver.init.cli:main',
         ],
     },
```

