# Comparing `tmp/cfresolve-0.0.1.tar.gz` & `tmp/cfresolve-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfresolve-0.0.1.tar", last modified: Wed May 29 15:23:43 2024, max compression
+gzip compressed data, was "cfresolve-0.0.2a0.tar", last modified: Wed May 29 15:31:15 2024, max compression
```

## Comparing `cfresolve-0.0.1.tar` & `cfresolve-0.0.2a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:23:43.755235 cfresolve-0.0.1/
--rw-rw-r--   0 smz       (1000) smz       (1000)       68 2024-05-29 15:22:36.000000 cfresolve-0.0.1/.gitignore
--rw-r--r--   0 smz       (1000) smz       (1000)      659 2024-05-29 15:23:43.755235 cfresolve-0.0.1/PKG-INFO
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:23:43.754234 cfresolve-0.0.1/assets/
--rw-rw-r--   0 smz       (1000) smz       (1000)   296778 2024-05-29 08:08:36.000000 cfresolve-0.0.1/assets/domains.csv
--rw-rw-r--   0 smz       (1000) smz       (1000)     3216 2024-05-29 15:15:08.000000 cfresolve-0.0.1/pyproject.toml
--rw-rw-r--   0 smz       (1000) smz       (1000)       38 2024-05-29 15:23:43.755235 cfresolve-0.0.1/setup.cfg
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:23:43.754234 cfresolve-0.0.1/src/
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:23:43.755235 cfresolve-0.0.1/src/cfresolve/
--rw-rw-r--   0 smz       (1000) smz       (1000)       49 2024-05-29 14:58:39.000000 cfresolve-0.0.1/src/cfresolve/__init__.py
--rw-rw-r--   0 smz       (1000) smz       (1000)       68 2024-05-29 14:58:56.000000 cfresolve-0.0.1/src/cfresolve/__main__.py
--rw-rw-r--   0 smz       (1000) smz       (1000)      411 2024-05-29 15:23:43.000000 cfresolve-0.0.1/src/cfresolve/_version.py
--rw-rw-r--   0 smz       (1000) smz       (1000)     6034 2024-05-29 15:17:11.000000 cfresolve-0.0.1/src/cfresolve/cli.py
--rw-rw-r--   0 smz       (1000) smz       (1000)      296 2024-05-29 10:08:39.000000 cfresolve-0.0.1/src/cfresolve/exceptions.py
-drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:23:43.755235 cfresolve-0.0.1/src/cfresolve.egg-info/
--rw-r--r--   0 smz       (1000) smz       (1000)      659 2024-05-29 15:23:43.000000 cfresolve-0.0.1/src/cfresolve.egg-info/PKG-INFO
--rw-rw-r--   0 smz       (1000) smz       (1000)      395 2024-05-29 15:23:43.000000 cfresolve-0.0.1/src/cfresolve.egg-info/SOURCES.txt
--rw-rw-r--   0 smz       (1000) smz       (1000)        1 2024-05-29 15:23:43.000000 cfresolve-0.0.1/src/cfresolve.egg-info/dependency_links.txt
--rw-rw-r--   0 smz       (1000) smz       (1000)       44 2024-05-29 15:23:43.000000 cfresolve-0.0.1/src/cfresolve.egg-info/entry_points.txt
--rw-rw-r--   0 smz       (1000) smz       (1000)       47 2024-05-29 15:23:43.000000 cfresolve-0.0.1/src/cfresolve.egg-info/requires.txt
--rw-rw-r--   0 smz       (1000) smz       (1000)       10 2024-05-29 15:23:43.000000 cfresolve-0.0.1/src/cfresolve.egg-info/top_level.txt
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:31:15.954160 cfresolve-0.0.2a0/
+-rw-rw-r--   0 smz       (1000) smz       (1000)       68 2024-05-29 15:22:36.000000 cfresolve-0.0.2a0/.gitignore
+-rw-r--r--   0 smz       (1000) smz       (1000)      700 2024-05-29 15:31:15.953160 cfresolve-0.0.2a0/PKG-INFO
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:31:15.951160 cfresolve-0.0.2a0/assets/
+-rw-rw-r--   0 smz       (1000) smz       (1000)   296778 2024-05-29 08:08:36.000000 cfresolve-0.0.2a0/assets/domains.csv
+-rw-rw-r--   0 smz       (1000) smz       (1000)     3268 2024-05-29 15:30:02.000000 cfresolve-0.0.2a0/pyproject.toml
+-rw-rw-r--   0 smz       (1000) smz       (1000)       38 2024-05-29 15:31:15.954160 cfresolve-0.0.2a0/setup.cfg
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:31:15.951160 cfresolve-0.0.2a0/src/
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:31:15.952160 cfresolve-0.0.2a0/src/cfresolve/
+-rw-rw-r--   0 smz       (1000) smz       (1000)       49 2024-05-29 14:58:39.000000 cfresolve-0.0.2a0/src/cfresolve/__init__.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)       68 2024-05-29 14:58:56.000000 cfresolve-0.0.2a0/src/cfresolve/__main__.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)      413 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve/_version.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)     6034 2024-05-29 15:17:11.000000 cfresolve-0.0.2a0/src/cfresolve/cli.py
+-rw-rw-r--   0 smz       (1000) smz       (1000)      296 2024-05-29 10:08:39.000000 cfresolve-0.0.2a0/src/cfresolve/exceptions.py
+drwxrwxr-x   0 smz       (1000) smz       (1000)        0 2024-05-29 15:31:15.953160 cfresolve-0.0.2a0/src/cfresolve.egg-info/
+-rw-r--r--   0 smz       (1000) smz       (1000)      700 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve.egg-info/PKG-INFO
+-rw-rw-r--   0 smz       (1000) smz       (1000)      395 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve.egg-info/SOURCES.txt
+-rw-rw-r--   0 smz       (1000) smz       (1000)        1 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve.egg-info/dependency_links.txt
+-rw-rw-r--   0 smz       (1000) smz       (1000)       44 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve.egg-info/entry_points.txt
+-rw-rw-r--   0 smz       (1000) smz       (1000)       86 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve.egg-info/requires.txt
+-rw-rw-r--   0 smz       (1000) smz       (1000)       10 2024-05-29 15:31:15.000000 cfresolve-0.0.2a0/src/cfresolve.egg-info/top_level.txt
```

### Comparing `cfresolve-0.0.1/PKG-INFO` & `cfresolve-0.0.2a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: cfresolve
-Version: 0.0.1
+Version: 0.0.2a0
 Summary: Pings domains that use cloudflare to retrieve edge ips
 Author-email: tempookian <tempookian@gmail.com>
 Project-URL: Homepage, https://github.com/tempookian/cfresolve/
 Project-URL: Bug Tracker, https://github.com/tempookian/cfresolve/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: polars
-Requires-Dist: rich_click
-Requires-Dist: pydantic
-Requires-Dist: validators
-Requires-Dist: requests
+Requires-Dist: polars==0.20.30
+Requires-Dist: rich-click==1.8.2
+Requires-Dist: pydantic==2.7.2
+Requires-Dist: validators==0.28.3
+Requires-Dist: requests==2.32.2
```

### Comparing `cfresolve-0.0.1/assets/domains.csv` & `cfresolve-0.0.2a0/assets/domains.csv`

 * *Files identical despite different names*

### Comparing `cfresolve-0.0.1/pyproject.toml` & `cfresolve-0.0.2a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
 ]
-dependencies = ["polars", "rich_click", "pydantic", "validators", "requests"]
+dependencies = [
+  "polars==0.20.30",
+  "rich-click==1.8.2",
+  "pydantic==2.7.2",
+  "validators==0.28.3",
+  "requests==2.32.2",
+]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/tempookian/cfresolve/"
 "Bug Tracker" = "https://github.com/tempookian/cfresolve/issues"
 
 [project.scripts]
```

### Comparing `cfresolve-0.0.1/src/cfresolve/cli.py` & `cfresolve-0.0.2a0/src/cfresolve/cli.py`

 * *Files identical despite different names*

### Comparing `cfresolve-0.0.1/src/cfresolve.egg-info/PKG-INFO` & `cfresolve-0.0.2a0/src/cfresolve.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: cfresolve
-Version: 0.0.1
+Version: 0.0.2a0
 Summary: Pings domains that use cloudflare to retrieve edge ips
 Author-email: tempookian <tempookian@gmail.com>
 Project-URL: Homepage, https://github.com/tempookian/cfresolve/
 Project-URL: Bug Tracker, https://github.com/tempookian/cfresolve/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: polars
-Requires-Dist: rich_click
-Requires-Dist: pydantic
-Requires-Dist: validators
-Requires-Dist: requests
+Requires-Dist: polars==0.20.30
+Requires-Dist: rich-click==1.8.2
+Requires-Dist: pydantic==2.7.2
+Requires-Dist: validators==0.28.3
+Requires-Dist: requests==2.32.2
```

