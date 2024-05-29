# Comparing `tmp/jeffutils-0.6.5.tar.gz` & `tmp/jeffutils-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.6.5.tar", last modified: Tue May 28 19:36:52 2024, max compression
+gzip compressed data, was "jeffutils-0.6.6.tar", last modified: Tue May 28 22:17:28 2024, max compression
```

## Comparing `jeffutils-0.6.5.tar` & `jeffutils-0.6.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 19:36:52.470285 jeffutils-0.6.5/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.5/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-28 19:36:52.470285 jeffutils-0.6.5/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2613 2024-05-28 19:36:25.000000 jeffutils-0.6.5/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.5/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-28 19:36:52.470285 jeffutils-0.6.5/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      611 2024-05-28 19:36:48.000000 jeffutils-0.6.5/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 19:36:52.470285 jeffutils-0.6.5/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 19:36:52.470285 jeffutils-0.6.5/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.5/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    33111 2024-05-28 19:01:16.000000 jeffutils-0.6.5/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 19:36:52.470285 jeffutils-0.6.5/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-28 19:36:52.000000 jeffutils-0.6.5/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-28 19:36:52.000000 jeffutils-0.6.5/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-28 19:36:52.000000 jeffutils-0.6.5/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-28 19:36:52.000000 jeffutils-0.6.5/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 22:17:28.477836 jeffutils-0.6.6/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.6/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-28 22:17:28.477836 jeffutils-0.6.6/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2614 2024-05-28 19:37:43.000000 jeffutils-0.6.6/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.6/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-28 22:17:28.477836 jeffutils-0.6.6/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      611 2024-05-28 22:17:22.000000 jeffutils-0.6.6/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 22:17:28.477836 jeffutils-0.6.6/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 22:17:28.477836 jeffutils-0.6.6/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.6/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    33093 2024-05-28 22:17:07.000000 jeffutils-0.6.6/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-28 22:17:28.477836 jeffutils-0.6.6/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-28 22:17:28.000000 jeffutils-0.6.6/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-28 22:17:28.000000 jeffutils-0.6.6/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-28 22:17:28.000000 jeffutils-0.6.6/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-28 22:17:28.000000 jeffutils-0.6.6/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.6.5/LICENSE.txt` & `jeffutils-0.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.6.5/README.md` & `jeffutils-0.6.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # jeffutils
 
-Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my projects, and I hope you feel free to using them as well!
+Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my projects, and I hope you find some of them useful as well!
 
 # Installation
 
 You can install this package from `PyPi` with
 ```
 pip install jeffutils
 ```
```

### Comparing `jeffutils-0.6.5/setup.py` & `jeffutils-0.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.6.5',
+    version='0.6.6',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.6.5/src/jeffutils/utils.py` & `jeffutils-0.6.6/src/jeffutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,35 +595,35 @@
 def reimport(statements:str|list):
     """ takes in python import code represented as a string or a list of strings, and
     it reimports all of the modules and functions in the import statements. This allows
     you to reimport modules that have been changed in the background without having to
     restart the kernel.
     
     The input can either be:
-    - a string with a single import statement\n
+    - a string with a single import statement
       ex: 'import numpy as np' or 'from random import choice, randint'
-    - a multiline string with multiple import statements\n
-      ex: '''import numpy as np\n
-      import pandas as pd\n
+    - a multiline string with multiple import statements
+      ex: '''import numpy as np
+      import pandas as pd
       from random import choice, randint'''
-    - a list of strings where each string is an import statement\n
+    - a list of strings where each string is an import statement
       ex: ['import numpy as np', 'import pandas as pd', 'from random import choice, randint']
       
-    This also handles situations where imports look like:\n
-    'from config import (
+    This also handles situations where imports look like:
+    from config import (
         thing1,
         thing2,
         thing3
-    )'
+    )
     
-    or that have the line continuation character \\ at the end of a line:\n
-    'from config import thing 1, \\
+    or that have the line continuation character \\ at the end of a line:
+    from config import thing 1, \\
         thing2, \\
         thing3
-    '
+    
     
     raises:
     AttributeError: if the module or function is not found in sys.modules
     
     DEPENDENCY NOTE: 
     If you make changes to two files file_1.py and file_2.py, and file_2 imports file_1, if you
     reimport file_2, then the changes in file_1 will not be reflected in file_2. You must reimport
```

