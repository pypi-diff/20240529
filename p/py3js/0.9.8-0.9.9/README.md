# Comparing `tmp/py3js-0.9.8.tar.gz` & `tmp/py3js-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3js-0.9.8.tar", last modified: Fri Dec  8 13:21:09 2023, max compression
+gzip compressed data, was "py3js-0.9.9.tar", last modified: Fri Dec  8 13:42:15 2023, max compression
```

## Comparing `py3js-0.9.8.tar` & `py3js-0.9.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 13:21:09.886344 py3js-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-08 13:20:54.000000 py3js-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-08 13:20:54.000000 py3js-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-12-08 13:21:09.882344 py3js-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-12-08 13:20:54.000000 py3js-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 13:21:09.882344 py3js-0.9.8/py3js/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 13:20:54.000000 py3js-0.9.8/py3js/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-12-08 13:20:54.000000 py3js-0.9.8/py3js/d3v6.html
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2023-12-08 13:20:54.000000 py3js-0.9.8/py3js/force.html
--rw-r--r--   0 runner    (1001) docker     (127)      671 2023-12-08 13:20:54.000000 py3js-0.9.8/py3js/infra.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2023-12-08 13:20:54.000000 py3js-0.9.8/py3js/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2023-12-08 13:20:54.000000 py3js-0.9.8/py3js/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-12-08 13:20:54.000000 py3js-0.9.8/py3js/visualisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2023-12-08 13:20:54.000000 py3js-0.9.8/py3js/wordcloud.html
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-12-08 13:20:54.000000 py3js-0.9.8/py3js/wordcloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 13:21:09.882344 py3js-0.9.8/py3js.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-12-08 13:21:09.000000 py3js-0.9.8/py3js.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-08 13:21:09.000000 py3js-0.9.8/py3js.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 13:21:09.000000 py3js-0.9.8/py3js.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-08 13:21:09.000000 py3js-0.9.8/py3js.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 13:21:09.886344 py3js-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2023-12-08 13:20:54.000000 py3js-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 13:21:09.882344 py3js-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-12-08 13:20:54.000000 py3js-0.9.8/tests/test_force.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-12-08 13:20:54.000000 py3js-0.9.8/tests/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-08 13:20:54.000000 py3js-0.9.8/tests/test_wordcloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 13:42:15.044849 py3js-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-08 13:42:02.000000 py3js-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-08 13:42:02.000000 py3js-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2023-12-08 13:42:15.044849 py3js-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2023-12-08 13:42:02.000000 py3js-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 13:42:15.044849 py3js-0.9.9/py3js/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 13:42:02.000000 py3js-0.9.9/py3js/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2023-12-08 13:42:02.000000 py3js-0.9.9/py3js/d3v6.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2023-12-08 13:42:02.000000 py3js-0.9.9/py3js/force.html
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2023-12-08 13:42:02.000000 py3js-0.9.9/py3js/infra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2023-12-08 13:42:02.000000 py3js-0.9.9/py3js/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2023-12-08 13:42:02.000000 py3js-0.9.9/py3js/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-12-08 13:42:02.000000 py3js-0.9.9/py3js/visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2023-12-08 13:42:02.000000 py3js-0.9.9/py3js/wordcloud.html
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2023-12-08 13:42:02.000000 py3js-0.9.9/py3js/wordcloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 13:42:15.044849 py3js-0.9.9/py3js.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2023-12-08 13:42:15.000000 py3js-0.9.9/py3js.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-08 13:42:15.000000 py3js-0.9.9/py3js.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 13:42:15.000000 py3js-0.9.9/py3js.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-08 13:42:15.000000 py3js-0.9.9/py3js.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 13:42:15.044849 py3js-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2023-12-08 13:42:02.000000 py3js-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 13:42:15.044849 py3js-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-12-08 13:42:02.000000 py3js-0.9.9/tests/test_force.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2023-12-08 13:42:02.000000 py3js-0.9.9/tests/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-08 13:42:02.000000 py3js-0.9.9/tests/test_wordcloud.py
```

### Comparing `py3js-0.9.8/LICENSE` & `py3js-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py3js-0.9.8/PKG-INFO` & `py3js-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3js
-Version: 0.9.8
+Version: 0.9.9
 Summary: d3js wrapper. At the moment only for directed force graphs
 Home-page: https://github.com/aloneguid/py3js
 Author: Ivan Gavryliuk
 Author-email: aloneguid@outlook.com
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `py3js-0.9.8/py3js/force.html` & `py3js-0.9.9/py3js/force.html`

 * *Files identical despite different names*

### Comparing `py3js-0.9.8/py3js/infra.py` & `py3js-0.9.9/py3js/infra.py`

 * *Files identical despite different names*

### Comparing `py3js-0.9.8/py3js/network.py` & `py3js-0.9.9/py3js/network.py`

 * *Files identical despite different names*

### Comparing `py3js-0.9.8/py3js/tree.py` & `py3js-0.9.9/py3js/tree.py`

 * *Files identical despite different names*

### Comparing `py3js-0.9.8/py3js/visualisation.py` & `py3js-0.9.9/py3js/visualisation.py`

 * *Files identical despite different names*

### Comparing `py3js-0.9.8/py3js/wordcloud.html` & `py3js-0.9.9/py3js/wordcloud.html`

 * *Files identical despite different names*

### Comparing `py3js-0.9.8/py3js/wordcloud.py` & `py3js-0.9.9/py3js/wordcloud.py`

 * *Files identical despite different names*

### Comparing `py3js-0.9.8/py3js.egg-info/PKG-INFO` & `py3js-0.9.9/py3js.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3js
-Version: 0.9.8
+Version: 0.9.9
 Summary: d3js wrapper. At the moment only for directed force graphs
 Home-page: https://github.com/aloneguid/py3js
 Author: Ivan Gavryliuk
 Author-email: aloneguid@outlook.com
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `py3js-0.9.8/setup.py` & `py3js-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `py3js-0.9.8/tests/test_force.py` & `py3js-0.9.9/tests/test_force.py`

 * *Files identical despite different names*

### Comparing `py3js-0.9.8/tests/test_tree.py` & `py3js-0.9.9/tests/test_tree.py`

 * *Files identical despite different names*

