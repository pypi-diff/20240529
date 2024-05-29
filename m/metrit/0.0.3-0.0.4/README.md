# Comparing `tmp/metrit-0.0.3.tar.gz` & `tmp/metrit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metrit-0.0.3.tar", last modified: Wed May 29 09:40:13 2024, max compression
+gzip compressed data, was "metrit-0.0.4.tar", last modified: Wed May 29 09:56:11 2024, max compression
```

## Comparing `metrit-0.0.3.tar` & `metrit-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:13.659616 metrit-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 09:40:02.000000 metrit-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-29 09:40:13.659616 metrit-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-05-29 09:40:02.000000 metrit-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:13.655616 metrit-0.0.3/metrit/
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-29 09:40:02.000000 metrit-0.0.3/metrit/Monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    15208 2024-05-29 09:40:02.000000 metrit-0.0.3/metrit/StatCollector.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-29 09:40:02.000000 metrit-0.0.3/metrit/Stats.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-29 09:40:02.000000 metrit-0.0.3/metrit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-05-29 09:40:02.000000 metrit-0.0.3/metrit/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-29 09:40:02.000000 metrit-0.0.3/metrit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:13.659616 metrit-0.0.3/metrit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-29 09:40:13.000000 metrit-0.0.3/metrit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-29 09:40:13.000000 metrit-0.0.3/metrit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:40:13.000000 metrit-0.0.3/metrit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 09:40:13.000000 metrit-0.0.3/metrit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 09:40:13.000000 metrit-0.0.3/metrit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:40:13.659616 metrit-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 09:40:10.000000 metrit-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:13.659616 metrit-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-29 09:40:02.000000 metrit-0.0.3/tests/test_StatsCollector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-29 09:40:02.000000 metrit-0.0.3/tests/test_metrit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-29 09:40:02.000000 metrit-0.0.3/tests/test_metrit_deactivated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-29 09:40:02.000000 metrit-0.0.3/tests/test_metrit_with_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-29 09:40:02.000000 metrit-0.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:56:11.479851 metrit-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 09:56:06.000000 metrit-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-29 09:56:11.479851 metrit-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-05-29 09:56:06.000000 metrit-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:56:11.479851 metrit-0.0.4/metrit/
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-29 09:56:06.000000 metrit-0.0.4/metrit/Monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15208 2024-05-29 09:56:06.000000 metrit-0.0.4/metrit/StatCollector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-29 09:56:06.000000 metrit-0.0.4/metrit/Stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-29 09:56:06.000000 metrit-0.0.4/metrit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-05-29 09:56:06.000000 metrit-0.0.4/metrit/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-29 09:56:06.000000 metrit-0.0.4/metrit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:56:11.479851 metrit-0.0.4/metrit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-29 09:56:11.000000 metrit-0.0.4/metrit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-29 09:56:11.000000 metrit-0.0.4/metrit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:56:11.000000 metrit-0.0.4/metrit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 09:56:11.000000 metrit-0.0.4/metrit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 09:56:11.000000 metrit-0.0.4/metrit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:56:11.479851 metrit-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 09:56:08.000000 metrit-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:56:11.479851 metrit-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-29 09:56:06.000000 metrit-0.0.4/tests/test_StatsCollector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-29 09:56:06.000000 metrit-0.0.4/tests/test_metrit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-29 09:56:06.000000 metrit-0.0.4/tests/test_metrit_deactivated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-29 09:56:06.000000 metrit-0.0.4/tests/test_metrit_with_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-29 09:56:06.000000 metrit-0.0.4/tests/test_utils.py
```

### Comparing `metrit-0.0.3/LICENSE` & `metrit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metrit-0.0.3/PKG-INFO` & `metrit-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrit
-Version: 0.0.3
+Version: 0.0.4
 Summary: A dead simple resources monitoring decorator
 Home-page: https://github.com/mcrespoae/metrit
 Author: mcrespoae
 Author-email: info@mariocrespo.es
 Keywords: metrit
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metrit-0.0.3/README.md` & `metrit-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `metrit-0.0.3/metrit/Monitoring.py` & `metrit-0.0.4/metrit/Monitoring.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.3/metrit/StatCollector.py` & `metrit-0.0.4/metrit/StatCollector.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.3/metrit/Stats.py` & `metrit-0.0.4/metrit/Stats.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.3/metrit/core.py` & `metrit-0.0.4/metrit/core.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.3/metrit/utils.py` & `metrit-0.0.4/metrit/utils.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.3/metrit.egg-info/PKG-INFO` & `metrit-0.0.4/metrit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrit
-Version: 0.0.3
+Version: 0.0.4
 Summary: A dead simple resources monitoring decorator
 Home-page: https://github.com/mcrespoae/metrit
 Author: mcrespoae
 Author-email: info@mariocrespo.es
 Keywords: metrit
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metrit-0.0.3/setup.py` & `metrit-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="metrit",
-    version="0.0.3",
+    version="0.0.4",
     author="mcrespoae",
     author_email="info@mariocrespo.es",
     packages=["metrit"],
     description="A dead simple resources monitoring decorator",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/mcrespoae/metrit",
```

### Comparing `metrit-0.0.3/tests/test_StatsCollector.py` & `metrit-0.0.4/tests/test_StatsCollector.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.3/tests/test_metrit.py` & `metrit-0.0.4/tests/test_metrit.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.3/tests/test_metrit_deactivated.py` & `metrit-0.0.4/tests/test_metrit_deactivated.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.3/tests/test_metrit_with_args.py` & `metrit-0.0.4/tests/test_metrit_with_args.py`

 * *Files identical despite different names*

### Comparing `metrit-0.0.3/tests/test_utils.py` & `metrit-0.0.4/tests/test_utils.py`

 * *Files identical despite different names*

