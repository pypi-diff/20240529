# Comparing `tmp/pyerualjetwork-1.3.2.tar.gz` & `tmp/pyerualjetwork-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.3.2.tar", last modified: Wed May 29 18:16:42 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.3.3.tar", last modified: Wed May 29 18:19:20 2024, max compression
```

## Comparing `pyerualjetwork-1.3.2.tar` & `pyerualjetwork-1.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 18:16:42.650583 pyerualjetwork-1.3.2/
--rw-rw-rw-   0        0        0      259 2024-05-29 18:16:42.649586 pyerualjetwork-1.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-29 18:16:42.627473 pyerualjetwork-1.3.2/plan/
--rw-rw-rw-   0        0        0      375 2024-05-29 18:09:13.000000 pyerualjetwork-1.3.2/plan/__init__.py
--rw-rw-rw-   0        0        0    44206 2024-05-29 18:16:26.000000 pyerualjetwork-1.3.2/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-29 18:16:42.646589 pyerualjetwork-1.3.2/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      259 2024-05-29 18:16:41.000000 pyerualjetwork-1.3.2/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-29 18:16:42.000000 pyerualjetwork-1.3.2/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 18:16:41.000000 pyerualjetwork-1.3.2/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-29 18:16:41.000000 pyerualjetwork-1.3.2/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 18:16:42.651579 pyerualjetwork-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      684 2024-05-29 18:12:38.000000 pyerualjetwork-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:19:20.757344 pyerualjetwork-1.3.3/
+-rw-rw-rw-   0        0        0      502 2024-05-29 18:19:20.756349 pyerualjetwork-1.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-29 18:19:20.721831 pyerualjetwork-1.3.3/plan/
+-rw-rw-rw-   0        0        0      375 2024-05-29 18:09:13.000000 pyerualjetwork-1.3.3/plan/__init__.py
+-rw-rw-rw-   0        0        0    44206 2024-05-29 18:16:26.000000 pyerualjetwork-1.3.3/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:19:20.753351 pyerualjetwork-1.3.3/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      502 2024-05-29 18:19:19.000000 pyerualjetwork-1.3.3/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-29 18:19:20.000000 pyerualjetwork-1.3.3/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:19:19.000000 pyerualjetwork-1.3.3/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-29 18:19:19.000000 pyerualjetwork-1.3.3/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:19:20.757344 pyerualjetwork-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      681 2024-05-29 18:19:10.000000 pyerualjetwork-1.3.3/setup.py
```

### Comparing `pyerualjetwork-1.3.2/plan/plan.py` & `pyerualjetwork-1.3.3/plan/plan.py`

 * *Files identical despite different names*

### Comparing `pyerualjetwork-1.3.2/setup.py` & `pyerualjetwork-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "1.3.2",
+      version = "1.3.3",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
-      description= "Advanced python deep learning library. \n New Features: 'SyntheticAugmentation' function added for unbalanced datasets. Changes for variable names to snake_case (Function names are still PascalCase). (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
+      description= "Advanced python deep learning library. New Features: 'SyntheticAugmentation' function added for unbalanced datasets. Changes for variable names to snake_case (Function names are still PascalCase). (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks'],
 
       
       )
```

