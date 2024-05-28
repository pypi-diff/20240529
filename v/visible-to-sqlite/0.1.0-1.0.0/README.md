# Comparing `tmp/visible_to_sqlite-0.1.0.tar.gz` & `tmp/visible_to_sqlite-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visible_to_sqlite-0.1.0.tar", last modified: Fri May 24 01:54:02 2024, max compression
+gzip compressed data, was "visible_to_sqlite-1.0.0.tar", last modified: Tue May 28 23:18:16 2024, max compression
```

## Comparing `visible_to_sqlite-0.1.0.tar` & `visible_to_sqlite-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:54:02.821314 visible_to_sqlite-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-24 01:53:55.000000 visible_to_sqlite-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-24 01:54:02.821314 visible_to_sqlite-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-24 01:53:55.000000 visible_to_sqlite-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 01:54:02.821314 visible_to_sqlite-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-24 01:53:55.000000 visible_to_sqlite-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:54:02.821314 visible_to_sqlite-0.1.0/visible_to_sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:53:55.000000 visible_to_sqlite-0.1.0/visible_to_sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-24 01:53:55.000000 visible_to_sqlite-0.1.0/visible_to_sqlite/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:54:02.821314 visible_to_sqlite-0.1.0/visible_to_sqlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-24 01:54:02.000000 visible_to_sqlite-0.1.0/visible_to_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-24 01:54:02.000000 visible_to_sqlite-0.1.0/visible_to_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:54:02.000000 visible_to_sqlite-0.1.0/visible_to_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-24 01:54:02.000000 visible_to_sqlite-0.1.0/visible_to_sqlite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 01:54:02.000000 visible_to_sqlite-0.1.0/visible_to_sqlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 01:54:02.000000 visible_to_sqlite-0.1.0/visible_to_sqlite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:18:16.444561 visible_to_sqlite-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-28 23:18:10.000000 visible_to_sqlite-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-28 23:18:16.444561 visible_to_sqlite-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 23:18:10.000000 visible_to_sqlite-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:18:16.444561 visible_to_sqlite-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-28 23:18:10.000000 visible_to_sqlite-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:18:16.440561 visible_to_sqlite-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-28 23:18:10.000000 visible_to_sqlite-1.0.0/test/test_visible_to_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:18:16.440561 visible_to_sqlite-1.0.0/visible_to_sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:18:10.000000 visible_to_sqlite-1.0.0/visible_to_sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-28 23:18:10.000000 visible_to_sqlite-1.0.0/visible_to_sqlite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-28 23:18:10.000000 visible_to_sqlite-1.0.0/visible_to_sqlite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:18:16.444561 visible_to_sqlite-1.0.0/visible_to_sqlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-28 23:18:16.000000 visible_to_sqlite-1.0.0/visible_to_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 23:18:16.000000 visible_to_sqlite-1.0.0/visible_to_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:18:16.000000 visible_to_sqlite-1.0.0/visible_to_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 23:18:16.000000 visible_to_sqlite-1.0.0/visible_to_sqlite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 23:18:16.000000 visible_to_sqlite-1.0.0/visible_to_sqlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 23:18:16.000000 visible_to_sqlite-1.0.0/visible_to_sqlite.egg-info/top_level.txt
```

### Comparing `visible_to_sqlite-0.1.0/LICENSE` & `visible_to_sqlite-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `visible_to_sqlite-0.1.0/PKG-INFO` & `visible_to_sqlite-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1
-Name: visible-to-sqlite
-Version: 0.1.0
-Summary: Convert exported CSV from Visible app to a SQLite DB
-Author: Avner Shanan
-License: Apache License, Version 2.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Click
-Requires-Dist: sqlite-utils
-
 # visible-to-sqlite
 
 *Convert exported CSV from the [Visible app](https://www.makevisible.com/) to a SQLite DB.*
 
 Heavily inspired by [healthkit-to-sqlite](https://github.com/dogsheep/healthkit-to-sqlite) and the rest of the [Dogsheep](https://dogsheep.github.io/) family.  Designed to be explored with [Datasette](https://datasette.io/).
 
+## Installation
+
+`pip install visible-to-sqlite`
+
 ## Usage
 
 Run: `visible-to-sqlite Visible_Data_Export.csv ./visible.db`
 
 And then probably: `datasette ./visible.db`
+
+## Data Model
+
+![Data model diagram with three tables, generated from a PlantUML file](./architecture/data_model.png)
+
+Generated with PlantUML ([source](./architecture/data_model.plantuml)).
```

### Comparing `visible_to_sqlite-0.1.0/setup.py` & `visible_to_sqlite-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         encoding="utf8",
     ) as fp:
         return fp.read()
 
 setup(
     name='visible-to-sqlite',
     author='Avner Shanan',
-    version='0.1.0',
+    version='1.0.0',
     description="Convert exported CSV from Visible app to a SQLite DB",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     license="Apache License, Version 2.0",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

