# Comparing `tmp/elements-3.6.4.tar.gz` & `tmp/elements-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elements-3.6.4.tar", last modified: Wed May 22 06:01:31 2024, max compression
+gzip compressed data, was "elements-3.6.5.tar", last modified: Wed May 29 13:31:49 2024, max compression
```

## Comparing `elements-3.6.4.tar` & `elements-3.6.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 06:01:31.881161 elements-3.6.4/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.6.4/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.6.4/MANIFEST.in
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-22 06:01:31.877161 elements-3.6.4/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.6.4/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 06:01:31.877161 elements-3.6.4/elements/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      551 2024-05-22 06:01:24.000000 elements-3.6.4/elements/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.6.4/elements/agg.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3993 2024-05-22 06:01:15.000000 elements-3.6.4/elements/checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.6.4/elements/config.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.6.4/elements/counter.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.6.4/elements/flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.6.4/elements/fps.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.6.4/elements/logger.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    11853 2024-05-22 06:01:10.000000 elements-3.6.4/elements/path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.6.4/elements/plotting.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.6.4/elements/printing.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.6.4/elements/rwlock.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.6.4/elements/timer.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.6.4/elements/tree.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.6.4/elements/usage.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.6.4/elements/utils.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.6.4/elements/uuid.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.6.4/elements/when.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 06:01:31.877161 elements-3.6.4/elements.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-22 06:01:31.000000 elements-3.6.4/elements.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      679 2024-05-22 06:01:31.000000 elements-3.6.4/elements.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-22 06:01:31.000000 elements-3.6.4/elements.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-22 06:01:31.000000 elements-3.6.4/elements.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-22 06:01:31.000000 elements-3.6.4/elements.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       53 2024-05-13 22:39:18.000000 elements-3.6.4/requirements-optional.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-14 17:34:25.000000 elements-3.6.4/requirements.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-22 06:01:31.881161 elements-3.6.4/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.6.4/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 06:01:31.877161 elements-3.6.4/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2024-05-20 18:51:09.000000 elements-3.6.4/tests/test_basics.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1889 2024-05-20 19:03:28.000000 elements-3.6.4/tests/test_checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.6.4/tests/test_flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1307 2024-05-22 06:01:09.000000 elements-3.6.4/tests/test_path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.6.4/tests/test_tree.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-29 13:31:49.545950 elements-3.6.5/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.6.5/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.6.5/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-29 13:31:49.545950 elements-3.6.5/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.6.5/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-29 13:31:49.541950 elements-3.6.5/elements/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      551 2024-05-29 13:31:34.000000 elements-3.6.5/elements/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.6.5/elements/agg.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3993 2024-05-22 06:01:15.000000 elements-3.6.5/elements/checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.6.5/elements/config.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.6.5/elements/counter.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.6.5/elements/flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.6.5/elements/fps.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.6.5/elements/logger.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    11869 2024-05-29 13:31:30.000000 elements-3.6.5/elements/path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.6.5/elements/plotting.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.6.5/elements/printing.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.6.5/elements/rwlock.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.6.5/elements/timer.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.6.5/elements/tree.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.6.5/elements/usage.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.6.5/elements/utils.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.6.5/elements/uuid.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.6.5/elements/when.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-29 13:31:49.541950 elements-3.6.5/elements.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-29 13:31:49.000000 elements-3.6.5/elements.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      679 2024-05-29 13:31:49.000000 elements-3.6.5/elements.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-29 13:31:49.000000 elements-3.6.5/elements.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-29 13:31:49.000000 elements-3.6.5/elements.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-29 13:31:49.000000 elements-3.6.5/elements.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       53 2024-05-13 22:39:18.000000 elements-3.6.5/requirements-optional.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-14 17:34:25.000000 elements-3.6.5/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-29 13:31:49.545950 elements-3.6.5/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.6.5/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-29 13:31:49.541950 elements-3.6.5/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2024-05-20 18:51:09.000000 elements-3.6.5/tests/test_basics.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1889 2024-05-20 19:03:28.000000 elements-3.6.5/tests/test_checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.6.5/tests/test_flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1307 2024-05-22 06:01:09.000000 elements-3.6.5/tests/test_path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.6.5/tests/test_tree.py
```

### Comparing `elements-3.6.4/LICENSE` & `elements-3.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/PKG-INFO` & `elements-3.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.6.4
+Version: 3.6.5
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.6.4/README.md` & `elements-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/__init__.py` & `elements-3.6.5/elements/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.6.4'
+__version__ = '3.6.5'
 
 from .agg import Agg
 from .checkpoint import Checkpoint, Saveable
 from .config import Config
 from .counter import Counter
 from .flags import Flags
 from .fps import FPS
```

### Comparing `elements-3.6.4/elements/agg.py` & `elements-3.6.5/elements/agg.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/checkpoint.py` & `elements-3.6.5/elements/checkpoint.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/config.py` & `elements-3.6.5/elements/config.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/counter.py` & `elements-3.6.5/elements/counter.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/flags.py` & `elements-3.6.5/elements/flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/logger.py` & `elements-3.6.5/elements/logger.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/path.py` & `elements-3.6.5/elements/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     with open(str(self), mode=mode) as f:
       yield f
 
   def absolute(self):
     return type(self)(os.path.absolute(str(self)))
 
   def glob(self, pattern):
-    for path in globlib.glob(f'{str(self)}/{pattern}'):
+    for path in globlib.glob(f'{str(self)}/{pattern}', recursive=True):
       yield type(self)(path)
 
   def exists(self):
     return os.path.exists(str(self))
 
   def isfile(self):
     return os.path.isfile(str(self))
```

### Comparing `elements-3.6.4/elements/plotting.py` & `elements-3.6.5/elements/plotting.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/printing.py` & `elements-3.6.5/elements/printing.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/rwlock.py` & `elements-3.6.5/elements/rwlock.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/timer.py` & `elements-3.6.5/elements/timer.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/tree.py` & `elements-3.6.5/elements/tree.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/usage.py` & `elements-3.6.5/elements/usage.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/uuid.py` & `elements-3.6.5/elements/uuid.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements/when.py` & `elements-3.6.5/elements/when.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/elements.egg-info/PKG-INFO` & `elements-3.6.5/elements.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.6.4
+Version: 3.6.5
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.6.4/elements.egg-info/SOURCES.txt` & `elements-3.6.5/elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/setup.py` & `elements-3.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/tests/test_basics.py` & `elements-3.6.5/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/tests/test_checkpoint.py` & `elements-3.6.5/tests/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/tests/test_flags.py` & `elements-3.6.5/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/tests/test_path.py` & `elements-3.6.5/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.4/tests/test_tree.py` & `elements-3.6.5/tests/test_tree.py`

 * *Files identical despite different names*

