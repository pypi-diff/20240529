# Comparing `tmp/datastew-0.1.1.tar.gz` & `tmp/datastew-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastew-0.1.1.tar", last modified: Tue May 28 12:46:43 2024, max compression
+gzip compressed data, was "datastew-0.1.2.tar", last modified: Tue May 28 12:59:01 2024, max compression
```

## Comparing `datastew-0.1.1.tar` & `datastew-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:46:43.026416 datastew-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 12:46:34.000000 datastew-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-28 12:46:43.026416 datastew-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-28 12:46:34.000000 datastew-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:46:43.022416 datastew-0.1.1/datastew/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-28 12:46:34.000000 datastew-0.1.1/datastew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-28 12:46:34.000000 datastew-0.1.1/datastew/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-28 12:46:34.000000 datastew-0.1.1/datastew/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-05-28 12:46:34.000000 datastew-0.1.1/datastew/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-28 12:46:34.000000 datastew-0.1.1/datastew/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-05-28 12:46:34.000000 datastew-0.1.1/datastew/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:46:43.026416 datastew-0.1.1/datastew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-28 12:46:43.000000 datastew-0.1.1/datastew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-28 12:46:43.000000 datastew-0.1.1/datastew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:46:43.000000 datastew-0.1.1/datastew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 12:46:43.000000 datastew-0.1.1/datastew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:46:43.026416 datastew-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-28 12:46:40.000000 datastew-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:46:43.026416 datastew-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 12:46:34.000000 datastew-0.1.1/tests/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-28 12:46:34.000000 datastew-0.1.1/tests/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-28 12:46:34.000000 datastew-0.1.1/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-28 12:46:34.000000 datastew-0.1.1/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 12:46:34.000000 datastew-0.1.1/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-28 12:46:34.000000 datastew-0.1.1/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-05-28 12:46:34.000000 datastew-0.1.1/tests/test_visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:59:01.018792 datastew-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 12:58:52.000000 datastew-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-28 12:59:01.018792 datastew-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-28 12:58:52.000000 datastew-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:59:01.018792 datastew-0.1.2/datastew/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-28 12:58:52.000000 datastew-0.1.2/datastew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-28 12:58:52.000000 datastew-0.1.2/datastew/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-28 12:58:52.000000 datastew-0.1.2/datastew/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-05-28 12:58:52.000000 datastew-0.1.2/datastew/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-28 12:58:52.000000 datastew-0.1.2/datastew/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-05-28 12:58:52.000000 datastew-0.1.2/datastew/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:59:01.018792 datastew-0.1.2/datastew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-28 12:59:01.000000 datastew-0.1.2/datastew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-28 12:59:01.000000 datastew-0.1.2/datastew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:59:01.000000 datastew-0.1.2/datastew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 12:59:01.000000 datastew-0.1.2/datastew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:59:01.018792 datastew-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-28 12:58:58.000000 datastew-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:59:01.018792 datastew-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 12:58:52.000000 datastew-0.1.2/tests/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-28 12:58:52.000000 datastew-0.1.2/tests/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-28 12:58:52.000000 datastew-0.1.2/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-28 12:58:52.000000 datastew-0.1.2/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 12:58:52.000000 datastew-0.1.2/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-28 12:58:52.000000 datastew-0.1.2/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-05-28 12:58:52.000000 datastew-0.1.2/tests/test_visualisation.py
```

### Comparing `datastew-0.1.1/LICENSE` & `datastew-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datastew-0.1.1/README.md` & `datastew-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `datastew-0.1.1/datastew/conf.py` & `datastew-0.1.2/datastew/conf.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.1/datastew/embedding.py` & `datastew-0.1.2/datastew/embedding.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.1/datastew/evaluation.py` & `datastew-0.1.2/datastew/evaluation.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.1/datastew/mapping.py` & `datastew-0.1.2/datastew/mapping.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.1/datastew/visualisation.py` & `datastew-0.1.2/datastew/visualisation.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.1/setup.py` & `datastew-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
     name='datastew',
-    version='v0.1.1',
+    version='v0.1.2',
     packages=['datastew'],
     url='https://github.com/SCAI-BIO/index',
     license='Apache-2.0 license"',
     author='Tim Adams',
     author_email='tim.adams@scai.fraunhofer.de',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
```

### Comparing `datastew-0.1.1/tests/test_embedding.py` & `datastew-0.1.2/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.1/tests/test_evaluation.py` & `datastew-0.1.2/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.1/tests/test_mapping.py` & `datastew-0.1.2/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.1/tests/test_parser.py` & `datastew-0.1.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.1/tests/test_repository.py` & `datastew-0.1.2/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.1/tests/test_system.py` & `datastew-0.1.2/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.1/tests/test_visualisation.py` & `datastew-0.1.2/tests/test_visualisation.py`

 * *Files identical despite different names*

