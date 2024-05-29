# Comparing `tmp/jeffutils-0.6.6.tar.gz` & `tmp/jeffutils-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.6.6.tar", last modified: Tue May 28 22:17:28 2024, max compression
+gzip compressed data, was "jeffutils-0.6.7.tar", last modified: Wed May 29 16:00:09 2024, max compression
```

## Comparing `jeffutils-0.6.6.tar` & `jeffutils-0.6.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 22:17:28.477836 jeffutils-0.6.6/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.6/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-28 22:17:28.477836 jeffutils-0.6.6/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2614 2024-05-28 19:37:43.000000 jeffutils-0.6.6/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.6/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-28 22:17:28.477836 jeffutils-0.6.6/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      611 2024-05-28 22:17:22.000000 jeffutils-0.6.6/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 22:17:28.477836 jeffutils-0.6.6/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 22:17:28.477836 jeffutils-0.6.6/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.6/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    33093 2024-05-28 22:17:07.000000 jeffutils-0.6.6/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 22:17:28.477836 jeffutils-0.6.6/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-28 22:17:28.000000 jeffutils-0.6.6/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-28 22:17:28.000000 jeffutils-0.6.6/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-28 22:17:28.000000 jeffutils-0.6.6/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-28 22:17:28.000000 jeffutils-0.6.6/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:00:09.561427 jeffutils-0.6.7/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.7/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-29 16:00:09.561427 jeffutils-0.6.7/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2614 2024-05-28 19:37:43.000000 jeffutils-0.6.7/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.7/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-29 16:00:09.561427 jeffutils-0.6.7/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      611 2024-05-29 16:00:05.000000 jeffutils-0.6.7/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:00:09.561427 jeffutils-0.6.7/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:00:09.561427 jeffutils-0.6.7/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.7/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    36112 2024-05-29 15:59:51.000000 jeffutils-0.6.7/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:00:09.561427 jeffutils-0.6.7/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-29 16:00:09.000000 jeffutils-0.6.7/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-29 16:00:09.000000 jeffutils-0.6.7/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-29 16:00:09.000000 jeffutils-0.6.7/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-29 16:00:09.000000 jeffutils-0.6.7/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.6.6/LICENSE.txt` & `jeffutils-0.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.6.6/README.md` & `jeffutils-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `jeffutils-0.6.6/setup.py` & `jeffutils-0.6.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.6.6',
+    version='0.6.7',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.6.6/src/jeffutils/utils.py` & `jeffutils-0.6.7/src/jeffutils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import time
 from datetime import datetime, timezone
 from collections import defaultdict
 import sqlite3 as sql
 import json
 import numpy as np
 import pandas as pd
+import pkgutil
 import io
 import os
 import sys
 import importlib
 import re
 import pstats
 import cProfile
@@ -636,47 +637,123 @@
     
     def _import_one(module:str):
         """ takes in a string like 'random' or 'numpy as np' and imports that
         module with its alias if given
         """
         if 'as' in module:
             module_name, alias = module.split(' as ')
-            if module_name in sys.modules:
-                importlib.reload(sys.modules[module_name])
-                module_obj = sys.modules[module_name]
+            module_name = module_name.strip()
+            alias = alias.strip()
+        else:
+            module_name, alias = module, None
+            
+        if module_name in sys.modules:
+            importlib.reload(sys.modules[module_name])
+            module_obj = sys.modules[module_name]
+        else:
+            if "." in module_name:
+                module_obj = _import_module_hierarchy(module_name)[module_name]
             else:
                 module_obj = importlib.import_module(module_name)
+        globals()[module_name] = module_obj
+        
+        if alias:
             globals()[alias] = module_obj
             
-        else:
-            if module in sys.modules:
-                importlib.reload(sys.modules[module])
-                module_obj = sys.modules[module]
-            else:
-                module_obj = importlib.import_module(module)
+        return module_obj
             
-    def _import_sub_fun(module, func):
+    def _import_sub_func(module, func):
         """ handles something like "from random import randint" where 'random'
         is the module and 'randint' is the function
         """
         if module not in sys.modules:
             raise AttributeError(f"Module {module} not found in sys.modules")
         module_obj = sys.modules[module]
         
-        if 'as' in func:
+        if ' as ' in func:
             func_name, alias = func.split(' as ')
-            if func_name in dir(module_obj):
+            func_name = func_name.strip()
+            alias = alias.strip()
+        else:
+            func_name, alias = func.strip(), None
+        
+        if func_name in dir(module_obj):
+            if alias:
                 globals()[alias] = getattr(module_obj, func_name)
             else:
-                raise AttributeError(f"Function {func_name} not found in module {module}")
+                globals()[func_name] = getattr(module_obj, func_name)
+        else:
+            raise AttributeError(f"Function {func_name} not found in module {module}")
+        
+    def _get_sub_modules(module_path:str):
+        """ takes in a module_path like directory.sub_directory and returns a 
+        string of all of the modules in that directory like ['directory.sub_directory.module1',
+        'directory.sub_directory.module2', ...]
+        """
+        module_obj = _import_one(module_path)
+        return [
+            module_info.name
+            for module_info in pkgutil.walk_packages(module_obj.__path__, module_obj.__name__ + ".")
+        ]
+    
+    def _get_type_as_str(parent_module, name):
+        
+        if isinstance(parent_module, str):
+            parent_module_obj = sys.modules[parent_module]
+        else:
+            parent_module_obj = parent_module
+        
+        # if there is an alias in the name, remove it
+        main_portion = name.split(" as ")[0].strip()
+        
+        # packages with modules inside of them don't have attributes for each of the
+        # modules inside of them. Modules with functions, do have string attributes
+        # for each of their functions
+        if hasattr(parent_module_obj, main_portion):
+            return "function"
+        else:
+            return "module"
+
+    def _import_sub_module_component(parent_module, sub_component):
+        sub_component_type = _get_type_as_str(parent_module, sub_component)
+        if sub_component_type == 'module':
+            full_module_name = f"{parent_module}.{sub_component}"
+            _import_one(full_module_name)
+        elif sub_component_type == 'function':
+            _import_sub_func(parent_module, sub_component)
         else:
-            if func in dir(module_obj):
-                globals()[func] = getattr(module_obj, func)
+            print(f"Unknown type: {sub_component_type}")
+            
+    def _import_module_hierarchy(module_path:str):
+        """ This takes in a module_path like 'directory.sub_directory.module_name'
+        and imports all the modules in the hierarchy like directory, 
+        director.sub_directory, director.sub_directory.module_name
+        
+        returns a dictionary where the keys are the module paths and the values 
+        are the module objects
+        """
+        parts = module_path.split(".")
+        
+        # keep a record of the module objects for later use
+        module_objs = {}
+        
+        curr_module = ""
+        for i in range(len(parts)):
+            # import everything up to the current module
+            curr_module = ".".join(parts[:i+1])
+            if curr_module in sys.modules:
+                importlib.reload(sys.modules[curr_module])
+                module_obj = sys.modules[curr_module]
             else:
-                raise AttributeError(f"Function {func} not found in module {module}")
+                module_obj = importlib.import_module(curr_module)
+            # add the current_module path to the module_objs dictionary
+            module_objs[curr_module] = module_obj
+            globals()[curr_module] = module_obj
+            
+        return module_objs
             
     def _process_single_import_statement(import_statement:str):
         """ takes in a single import statement like 'import numpy as np' or 'from random import choice'
         and imports the module or function
         """
         # remove whitespace at the start and end of the import statement
         import_statement = import_statement.strip()
@@ -694,16 +771,16 @@
         elif import_statement.startswith("from"):
             
             # import the base module
             module = module_names[0]
             _import_one(module)
             
             # import each sub-function from the module
-            for func_name in module_names[1:]:
-                _import_sub_fun(module, func_name)
+            for sub_component in module_names[1:]:
+                _import_sub_module_component(module, sub_component)
                 
     def _get_statements_from_str(statements):
         """ takes in a statement representing python import code and returns a list of
         all of the import statements in that code. This handles situations where the import
         statements are split by newlines or have (...) blocks in them
         """
         # first strip the input string of any leading/trailing whitespace
```

