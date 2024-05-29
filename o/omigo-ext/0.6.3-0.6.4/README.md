# Comparing `tmp/omigo_ext-0.6.3.tar.gz` & `tmp/omigo_ext-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omigo_ext-0.6.3.tar", last modified: Mon Jan 29 22:23:43 2024, max compression
+gzip compressed data, was "omigo_ext-0.6.4.tar", last modified: Wed May 29 18:41:42 2024, max compression
```

## Comparing `omigo_ext-0.6.3.tar` & `omigo_ext-0.6.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:43.860721 omigo_ext-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-29 22:23:43.860721 omigo_ext-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-29 22:23:43.864721 omigo_ext-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:43.856721 omigo_ext-0.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:43.860721 omigo_ext-0.6.3/src/omigo_ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/src/omigo_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/src/omigo_ext/etl_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/src/omigo_ext/geomap_viz.py
--rw-r--r--   0 runner    (1001) docker     (127)    16665 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/src/omigo_ext/graph_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/src/omigo_ext/graphviz_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/src/omigo_ext/jira_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/src/omigo_ext/kafka_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/src/omigo_ext/multithread_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/src/omigo_ext/presto_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/src/omigo_ext/spark_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)    31025 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/src/omigo_ext/splunk_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/src/omigo_ext/sql_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-01-29 22:23:13.000000 omigo_ext-0.6.3/src/omigo_ext/ws_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:43.860721 omigo_ext-0.6.3/src/omigo_ext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-29 22:23:43.000000 omigo_ext-0.6.3/src/omigo_ext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-01-29 22:23:43.000000 omigo_ext-0.6.3/src/omigo_ext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 22:23:43.000000 omigo_ext-0.6.3/src/omigo_ext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-29 22:23:43.000000 omigo_ext-0.6.3/src/omigo_ext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-29 22:23:43.000000 omigo_ext-0.6.3/src/omigo_ext.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:42.059793 omigo_ext-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-29 18:41:42.059793 omigo_ext-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-29 18:41:42.059793 omigo_ext-0.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:42.051793 omigo_ext-0.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:42.055793 omigo_ext-0.6.4/src/omigo_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/src/omigo_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/src/omigo_ext/etl_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/src/omigo_ext/geomap_viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16665 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/src/omigo_ext/graph_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/src/omigo_ext/graphviz_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/src/omigo_ext/jira_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/src/omigo_ext/kafka_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/src/omigo_ext/multithread_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/src/omigo_ext/presto_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/src/omigo_ext/spark_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31025 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/src/omigo_ext/splunk_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/src/omigo_ext/sql_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-05-29 18:41:25.000000 omigo_ext-0.6.4/src/omigo_ext/ws_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:42.059793 omigo_ext-0.6.4/src/omigo_ext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-29 18:41:42.000000 omigo_ext-0.6.4/src/omigo_ext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-29 18:41:42.000000 omigo_ext-0.6.4/src/omigo_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:41:42.000000 omigo_ext-0.6.4/src/omigo_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 18:41:42.000000 omigo_ext-0.6.4/src/omigo_ext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 18:41:42.000000 omigo_ext-0.6.4/src/omigo_ext.egg-info/top_level.txt
```

### Comparing `omigo_ext-0.6.3/PKG-INFO` & `omigo_ext-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo_ext
-Version: 0.6.3
+Version: 0.6.4
 Summary: Extensions for omigo_core package
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_ext-0.6.3/setup.cfg` & `omigo_ext-0.6.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = omigo_ext
-version = 0.6.3
+version = 0.6.4
 author = amit jaiswal
 author_email = amit.jaiswal@gmail.com
 description = Extensions for omigo_core package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrowdStrike/omigo-data-analytics
 project_urls =
```

### Comparing `omigo_ext-0.6.3/src/omigo_ext/etl_ext.py` & `omigo_ext-0.6.4/src/omigo_ext/etl_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.6.3/src/omigo_ext/geomap_viz.py` & `omigo_ext-0.6.4/src/omigo_ext/geomap_viz.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.6.3/src/omigo_ext/graph_ext.py` & `omigo_ext-0.6.4/src/omigo_ext/graph_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.6.3/src/omigo_ext/graphviz_ext.py` & `omigo_ext-0.6.4/src/omigo_ext/graphviz_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.6.3/src/omigo_ext/jira_ext.py` & `omigo_ext-0.6.4/src/omigo_ext/jira_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.6.3/src/omigo_ext/kafka_ext.py` & `omigo_ext-0.6.4/src/omigo_ext/kafka_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.6.3/src/omigo_ext/multithread_ext.py` & `omigo_ext-0.6.4/src/omigo_ext/multithread_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.6.3/src/omigo_ext/presto_ext.py` & `omigo_ext-0.6.4/src/omigo_ext/presto_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.6.3/src/omigo_ext/spark_ext.py` & `omigo_ext-0.6.4/src/omigo_ext/spark_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.6.3/src/omigo_ext/splunk_ext.py` & `omigo_ext-0.6.4/src/omigo_ext/splunk_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.6.3/src/omigo_ext/sql_helper.py` & `omigo_ext-0.6.4/src/omigo_ext/sql_helper.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.6.3/src/omigo_ext/ws_ext.py` & `omigo_ext-0.6.4/src/omigo_ext/ws_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.6.3/src/omigo_ext.egg-info/PKG-INFO` & `omigo_ext-0.6.4/src/omigo_ext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo_ext
-Version: 0.6.3
+Version: 0.6.4
 Summary: Extensions for omigo_core package
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_ext-0.6.3/src/omigo_ext.egg-info/SOURCES.txt` & `omigo_ext-0.6.4/src/omigo_ext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

