# Comparing `tmp/monorepo-0.1.0.tar.gz` & `tmp/monorepo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monorepo-0.1.0.tar", last modified: Mon May  2 20:53:03 2022, max compression
+gzip compressed data, was "monorepo-0.1.1.tar", last modified: Thu Nov 30 05:31:21 2023, max compression
```

## Comparing `monorepo-0.1.0.tar` & `monorepo-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxr-x   0 myle     (20005) myle     (20005)        0 2022-05-02 20:53:03.931571 monorepo-0.1.0/
--rw-rw-r--   0 myle     (20005) myle     (20005)     1065 2022-05-02 20:29:19.000000 monorepo-0.1.0/LICENSE
--rw-rw-r--   0 myle     (20005) myle     (20005)      915 2022-05-02 20:53:03.927579 monorepo-0.1.0/PKG-INFO
--rw-rw-r--   0 myle     (20005) myle     (20005)      640 2022-05-02 20:37:30.000000 monorepo-0.1.0/README.md
-drwxrwxr-x   0 myle     (20005) myle     (20005)        0 2022-05-02 20:53:03.877573 monorepo-0.1.0/monorepo/
--rw-rw-r--   0 myle     (20005) myle     (20005)      867 2022-05-02 20:31:49.000000 monorepo-0.1.0/monorepo/__init__.py
-drwxrwxr-x   0 myle     (20005) myle     (20005)        0 2022-05-02 20:53:03.918570 monorepo-0.1.0/monorepo.egg-info/
--rw-rw-r--   0 myle     (20005) myle     (20005)      915 2022-05-02 20:53:03.000000 monorepo-0.1.0/monorepo.egg-info/PKG-INFO
--rw-rw-r--   0 myle     (20005) myle     (20005)      175 2022-05-02 20:53:03.000000 monorepo-0.1.0/monorepo.egg-info/SOURCES.txt
--rw-rw-r--   0 myle     (20005) myle     (20005)        1 2022-05-02 20:53:03.000000 monorepo-0.1.0/monorepo.egg-info/dependency_links.txt
--rw-rw-r--   0 myle     (20005) myle     (20005)        9 2022-05-02 20:53:03.000000 monorepo-0.1.0/monorepo.egg-info/top_level.txt
--rw-rw-r--   0 myle     (20005) myle     (20005)       38 2022-05-02 20:53:03.932580 monorepo-0.1.0/setup.cfg
--rw-rw-r--   0 myle     (20005) myle     (20005)      401 2022-05-02 20:52:30.000000 monorepo-0.1.0/setup.py
+drwxr-xr-x   0 myleott    (501) staff       (20)        0 2023-11-30 05:31:21.870978 monorepo-0.1.1/
+-rw-r--r--   0 myleott    (501) staff       (20)     1080 2023-11-30 05:31:21.870880 monorepo-0.1.1/PKG-INFO
+-rw-r--r--   0 myleott    (501) staff       (20)      640 2023-11-30 05:30:37.000000 monorepo-0.1.1/README.md
+drwxr-xr-x   0 myleott    (501) staff       (20)        0 2023-11-30 05:31:21.870341 monorepo-0.1.1/monorepo/
+-rw-r--r--   0 myleott    (501) staff       (20)      955 2023-11-30 05:30:37.000000 monorepo-0.1.1/monorepo/__init__.py
+drwxr-xr-x   0 myleott    (501) staff       (20)        0 2023-11-30 05:31:21.870737 monorepo-0.1.1/monorepo.egg-info/
+-rw-r--r--   0 myleott    (501) staff       (20)     1080 2023-11-30 05:31:21.000000 monorepo-0.1.1/monorepo.egg-info/PKG-INFO
+-rw-r--r--   0 myleott    (501) staff       (20)      167 2023-11-30 05:31:21.000000 monorepo-0.1.1/monorepo.egg-info/SOURCES.txt
+-rw-r--r--   0 myleott    (501) staff       (20)        1 2023-11-30 05:31:21.000000 monorepo-0.1.1/monorepo.egg-info/dependency_links.txt
+-rw-r--r--   0 myleott    (501) staff       (20)        9 2023-11-30 05:31:21.000000 monorepo-0.1.1/monorepo.egg-info/top_level.txt
+-rw-r--r--   0 myleott    (501) staff       (20)       38 2023-11-30 05:31:21.871013 monorepo-0.1.1/setup.cfg
+-rw-r--r--   0 myleott    (501) staff       (20)      401 2023-11-30 05:31:04.000000 monorepo-0.1.1/setup.py
```

### Comparing `monorepo-0.1.0/PKG-INFO` & `monorepo-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: monorepo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Import packages from the root of a monorepo
 Home-page: https://github.com/myleott/monorepo
 License: UNKNOWN
+Description: # Import packages from the root of a monorepo
+        
+        Instructions:
+        
+        1. First create a file named `.monorepo_root` at the root of your monorepo.
+        2. Use `monorepo.load_package` to load packages from anywhere in your monorepo.
+        
+        Example usage:
+        ```python
+        import monorepo
+        
+        # The `load_package` function will search up from the current directory for a
+        # file named `.monorepo_root`, which is used to determine the root directory
+        # from which to load `example.package.foo`:
+        foo = monorepo.load_package("example.package.foo")
+        
+        # The foo package can be used directly:
+        foo.bar_function()
+        
+        # We can also import other subpackages:
+        from foo.bar import baz
+        ```
+        
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Import packages from the root of a monorepo
-
-Instructions:
-
-1. First create a file named `.monorepo_root` at the root of your monorepo.
-2. Use `monorepo.load_package` to load packages from anywhere in your monorepo.
-
-Example usage:
-```python
-import monorepo
-
-# The `load_package` function will search up from the current directory for a
-# file named `.monorepo_root`, which is used to determine the root directory
-# from which to load `example.package.foo`:
-foo = monorepo.load_package("example.package.foo")
-
-# The foo package can be used directly:
-foo.bar_function()
-
-# We can also import other subpackages:
-from foo.bar import baz
-```
-
-
```

### Comparing `monorepo-0.1.0/README.md` & `monorepo-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `monorepo-0.1.0/monorepo/__init__.py` & `monorepo-0.1.1/monorepo/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import inspect
 import os
 import sys
 from importlib import util
 from pathlib import Path
 
 
-def load_package(package):
-    # Find `.monorepo_root` relative to the importing code.
-    root = importer = Path(inspect.stack()[1].filename).resolve()
+def load_package(package, root:str = None):
+    if not root:
+        # Find `.monorepo_root` relative to the importing code.
+        root = importer = Path(inspect.stack()[1].filename).resolve()
+    else:
+        root = Path(root).resolve()
     while not (root / ".monorepo_root").exists():
         if root == root.parent:
             raise FileNotFoundError(
                 f"Couldn't find .monorepo_root in parents of {importer}"
             )
         root = root.parent
```

### Comparing `monorepo-0.1.0/monorepo.egg-info/PKG-INFO` & `monorepo-0.1.1/monorepo.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: monorepo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Import packages from the root of a monorepo
 Home-page: https://github.com/myleott/monorepo
 License: UNKNOWN
+Description: # Import packages from the root of a monorepo
+        
+        Instructions:
+        
+        1. First create a file named `.monorepo_root` at the root of your monorepo.
+        2. Use `monorepo.load_package` to load packages from anywhere in your monorepo.
+        
+        Example usage:
+        ```python
+        import monorepo
+        
+        # The `load_package` function will search up from the current directory for a
+        # file named `.monorepo_root`, which is used to determine the root directory
+        # from which to load `example.package.foo`:
+        foo = monorepo.load_package("example.package.foo")
+        
+        # The foo package can be used directly:
+        foo.bar_function()
+        
+        # We can also import other subpackages:
+        from foo.bar import baz
+        ```
+        
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Import packages from the root of a monorepo
-
-Instructions:
-
-1. First create a file named `.monorepo_root` at the root of your monorepo.
-2. Use `monorepo.load_package` to load packages from anywhere in your monorepo.
-
-Example usage:
-```python
-import monorepo
-
-# The `load_package` function will search up from the current directory for a
-# file named `.monorepo_root`, which is used to determine the root directory
-# from which to load `example.package.foo`:
-foo = monorepo.load_package("example.package.foo")
-
-# The foo package can be used directly:
-foo.bar_function()
-
-# We can also import other subpackages:
-from foo.bar import baz
-```
-
-
```

