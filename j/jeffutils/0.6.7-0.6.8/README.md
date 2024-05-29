# Comparing `tmp/jeffutils-0.6.7.tar.gz` & `tmp/jeffutils-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.6.7.tar", last modified: Wed May 29 16:00:09 2024, max compression
+gzip compressed data, was "jeffutils-0.6.8.tar", last modified: Wed May 29 16:08:44 2024, max compression
```

## Comparing `jeffutils-0.6.7.tar` & `jeffutils-0.6.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:00:09.561427 jeffutils-0.6.7/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.7/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-29 16:00:09.561427 jeffutils-0.6.7/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2614 2024-05-28 19:37:43.000000 jeffutils-0.6.7/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.7/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-29 16:00:09.561427 jeffutils-0.6.7/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      611 2024-05-29 16:00:05.000000 jeffutils-0.6.7/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:00:09.561427 jeffutils-0.6.7/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:00:09.561427 jeffutils-0.6.7/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.7/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    36112 2024-05-29 15:59:51.000000 jeffutils-0.6.7/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:00:09.561427 jeffutils-0.6.7/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-29 16:00:09.000000 jeffutils-0.6.7/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-29 16:00:09.000000 jeffutils-0.6.7/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-29 16:00:09.000000 jeffutils-0.6.7/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-29 16:00:09.000000 jeffutils-0.6.7/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:08:44.550606 jeffutils-0.6.8/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.8/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-29 16:08:44.550606 jeffutils-0.6.8/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2614 2024-05-28 19:37:43.000000 jeffutils-0.6.8/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.8/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-29 16:08:44.550606 jeffutils-0.6.8/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      611 2024-05-29 16:08:41.000000 jeffutils-0.6.8/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:08:44.550606 jeffutils-0.6.8/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:08:44.550606 jeffutils-0.6.8/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.8/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    36114 2024-05-29 16:08:22.000000 jeffutils-0.6.8/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:08:44.550606 jeffutils-0.6.8/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-29 16:08:44.000000 jeffutils-0.6.8/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-29 16:08:44.000000 jeffutils-0.6.8/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-29 16:08:44.000000 jeffutils-0.6.8/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-29 16:08:44.000000 jeffutils-0.6.8/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.6.7/LICENSE.txt` & `jeffutils-0.6.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.6.7/README.md` & `jeffutils-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `jeffutils-0.6.7/setup.py` & `jeffutils-0.6.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.6.7',
+    version='0.6.8',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.6.7/src/jeffutils/utils.py` & `jeffutils-0.6.8/src/jeffutils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -635,15 +635,15 @@
     # inner helper functions #
     ##########################
     
     def _import_one(module:str):
         """ takes in a string like 'random' or 'numpy as np' and imports that
         module with its alias if given
         """
-        if 'as' in module:
+        if ' as ' in module:
             module_name, alias = module.split(' as ')
             module_name = module_name.strip()
             alias = alias.strip()
         else:
             module_name, alias = module, None
             
         if module_name in sys.modules:
```

