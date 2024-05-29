# Comparing `tmp/omigo_matel-0.6.3.tar.gz` & `tmp/omigo_matel-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omigo_matel-0.6.3.tar", last modified: Mon Jan 29 22:24:42 2024, max compression
+gzip compressed data, was "omigo_matel-0.6.4.tar", last modified: Wed May 29 18:42:09 2024, max compression
```

## Comparing `omigo_matel-0.6.3.tar` & `omigo_matel-0.6.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:24:42.668594 omigo_matel-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-29 22:24:42.668594 omigo_matel-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:13.000000 omigo_matel-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-29 22:23:13.000000 omigo_matel-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-29 22:24:42.668594 omigo_matel-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:24:42.668594 omigo_matel-0.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:24:42.668594 omigo_matel-0.6.3/src/omigo_matel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:13.000000 omigo_matel-0.6.3/src/omigo_matel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:24:42.668594 omigo_matel-0.6.3/src/omigo_matel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-29 22:24:42.000000 omigo_matel-0.6.3/src/omigo_matel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-29 22:24:42.000000 omigo_matel-0.6.3/src/omigo_matel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 22:24:42.000000 omigo_matel-0.6.3/src/omigo_matel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-29 22:24:42.000000 omigo_matel-0.6.3/src/omigo_matel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-29 22:24:42.000000 omigo_matel-0.6.3/src/omigo_matel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:09.291456 omigo_matel-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-29 18:42:09.291456 omigo_matel-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:25.000000 omigo_matel-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 18:41:25.000000 omigo_matel-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-29 18:42:09.291456 omigo_matel-0.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:09.287456 omigo_matel-0.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:09.287456 omigo_matel-0.6.4/src/omigo_matel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:25.000000 omigo_matel-0.6.4/src/omigo_matel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:42:09.291456 omigo_matel-0.6.4/src/omigo_matel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-29 18:42:09.000000 omigo_matel-0.6.4/src/omigo_matel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-29 18:42:09.000000 omigo_matel-0.6.4/src/omigo_matel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:42:09.000000 omigo_matel-0.6.4/src/omigo_matel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-29 18:42:09.000000 omigo_matel-0.6.4/src/omigo_matel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 18:42:09.000000 omigo_matel-0.6.4/src/omigo_matel.egg-info/top_level.txt
```

### Comparing `omigo_matel-0.6.3/PKG-INFO` & `omigo_matel-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo_matel
-Version: 0.6.3
+Version: 0.6.4
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_matel-0.6.3/setup.cfg` & `omigo_matel-0.6.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = omigo_matel
-version = 0.6.3
+version = 0.6.4
 author = amit jaiswal
 author_email = amit.jaiswal@gmail.com
 description = Data Analytics Library for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrowdStrike/omigo-data-analytics
 project_urls =
```

### Comparing `omigo_matel-0.6.3/src/omigo_matel.egg-info/PKG-INFO` & `omigo_matel-0.6.4/src/omigo_matel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo_matel
-Version: 0.6.3
+Version: 0.6.4
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

