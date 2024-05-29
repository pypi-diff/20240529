# Comparing `tmp/datastew-0.1.3.tar.gz` & `tmp/datastew-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastew-0.1.3.tar", last modified: Wed May 29 06:56:00 2024, max compression
+gzip compressed data, was "datastew-0.1.4.tar", last modified: Wed May 29 08:59:16 2024, max compression
```

## Comparing `datastew-0.1.3.tar` & `datastew-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:56:00.417661 datastew-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 06:55:56.000000 datastew-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-29 06:56:00.417661 datastew-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-29 06:55:56.000000 datastew-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:56:00.413661 datastew-0.1.3/datastew/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-29 06:55:56.000000 datastew-0.1.3/datastew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-29 06:55:56.000000 datastew-0.1.3/datastew/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-29 06:55:56.000000 datastew-0.1.3/datastew/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-05-29 06:55:56.000000 datastew-0.1.3/datastew/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-29 06:55:56.000000 datastew-0.1.3/datastew/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-05-29 06:55:56.000000 datastew-0.1.3/datastew/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:56:00.417661 datastew-0.1.3/datastew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-29 06:56:00.000000 datastew-0.1.3/datastew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-29 06:56:00.000000 datastew-0.1.3/datastew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:56:00.000000 datastew-0.1.3/datastew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 06:56:00.000000 datastew-0.1.3/datastew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:56:00.417661 datastew-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 06:55:58.000000 datastew-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:56:00.417661 datastew-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-29 06:55:56.000000 datastew-0.1.3/tests/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-29 06:55:56.000000 datastew-0.1.3/tests/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-29 06:55:56.000000 datastew-0.1.3/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-29 06:55:56.000000 datastew-0.1.3/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-29 06:55:56.000000 datastew-0.1.3/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-29 06:55:56.000000 datastew-0.1.3/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-05-29 06:55:56.000000 datastew-0.1.3/tests/test_visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:59:16.449259 datastew-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 08:59:10.000000 datastew-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-29 08:59:16.449259 datastew-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-29 08:59:10.000000 datastew-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:59:16.449259 datastew-0.1.4/datastew/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-29 08:59:10.000000 datastew-0.1.4/datastew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-29 08:59:10.000000 datastew-0.1.4/datastew/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-29 08:59:10.000000 datastew-0.1.4/datastew/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-05-29 08:59:10.000000 datastew-0.1.4/datastew/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-29 08:59:10.000000 datastew-0.1.4/datastew/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-05-29 08:59:10.000000 datastew-0.1.4/datastew/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:59:16.449259 datastew-0.1.4/datastew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-29 08:59:16.000000 datastew-0.1.4/datastew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-29 08:59:16.000000 datastew-0.1.4/datastew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:59:16.000000 datastew-0.1.4/datastew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 08:59:16.000000 datastew-0.1.4/datastew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:59:16.449259 datastew-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 08:59:14.000000 datastew-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:59:16.449259 datastew-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-29 08:59:10.000000 datastew-0.1.4/tests/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-29 08:59:10.000000 datastew-0.1.4/tests/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-29 08:59:10.000000 datastew-0.1.4/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-29 08:59:10.000000 datastew-0.1.4/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-29 08:59:10.000000 datastew-0.1.4/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-29 08:59:10.000000 datastew-0.1.4/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-05-29 08:59:10.000000 datastew-0.1.4/tests/test_visualisation.py
```

### Comparing `datastew-0.1.3/LICENSE` & `datastew-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datastew-0.1.3/README.md` & `datastew-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `datastew-0.1.3/datastew/conf.py` & `datastew-0.1.4/datastew/conf.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.3/datastew/embedding.py` & `datastew-0.1.4/datastew/embedding.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.3/datastew/evaluation.py` & `datastew-0.1.4/datastew/evaluation.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.3/datastew/mapping.py` & `datastew-0.1.4/datastew/mapping.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.3/datastew/visualisation.py` & `datastew-0.1.4/datastew/visualisation.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.3/setup.py` & `datastew-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
     name='datastew',
-    version='v0.1.3',
+    version='v0.1.4',
     packages=['datastew'],
     url='https://github.com/SCAI-BIO/index',
     license='Apache-2.0 license"',
     author='Tim Adams',
     author_email='tim.adams@scai.fraunhofer.de',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
```

### Comparing `datastew-0.1.3/tests/test_embedding.py` & `datastew-0.1.4/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.3/tests/test_evaluation.py` & `datastew-0.1.4/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.3/tests/test_mapping.py` & `datastew-0.1.4/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.3/tests/test_parser.py` & `datastew-0.1.4/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.3/tests/test_repository.py` & `datastew-0.1.4/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.3/tests/test_system.py` & `datastew-0.1.4/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.3/tests/test_visualisation.py` & `datastew-0.1.4/tests/test_visualisation.py`

 * *Files identical despite different names*

