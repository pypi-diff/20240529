# Comparing `tmp/killercoda_cli-1.0.8.tar.gz` & `tmp/killercoda_cli-1.1.0.tar.gz`

## Comparing `killercoda_cli-1.0.8.tar` & `killercoda_cli-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 killercoda_cli-1.0.8/.coveragerc
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 killercoda_cli-1.0.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 killercoda_cli-1.0.8/killercoda_cli/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.8/killercoda_cli/__init__.py
--rwxr-xr-x   0        0        0    16975 2020-02-02 00:00:00.000000 killercoda_cli-1.0.8/killercoda_cli/cli.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.8/tests/__init__.py
--rwxr-xr-x   0        0        0    12187 2020-02-02 00:00:00.000000 killercoda_cli-1.0.8/tests/test_cli.py
--rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 killercoda_cli-1.0.8/tests/test_integration_cli.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 killercoda_cli-1.0.8/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 killercoda_cli-1.0.8/LICENSE.txt
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 killercoda_cli-1.0.8/README.md
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 killercoda_cli-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 killercoda_cli-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/.coveragerc
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/killercoda_cli/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/killercoda_cli/__init__.py
+-rwxr-xr-x   0        0        0    16418 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/killercoda_cli/cli.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/killercoda_cli/scenario_init.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/tests/__init__.py
+-rwxr-xr-x   0        0        0    12187 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/tests/test_cli.py
+-rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/tests/test_integration_cli.py
+-rwxr-xr-x   0        0        0     4191 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/tests/test_scenario_init.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/README.md
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 killercoda_cli-1.1.0/PKG-INFO
```

### Comparing `killercoda_cli-1.0.8/.github/workflows/ci.yml` & `killercoda_cli-1.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.8/killercoda_cli/cli.py` & `killercoda_cli-1.1.0/killercoda_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import difflib
 import json
 import os
 import subprocess
 import sys
 from typing import List, Optional
 from killercoda_cli.__about__ import __version__
+from killercoda_cli.scenario_init import init_project
 
 class FileOperation:
     """
     Define a type hint for the different types of file operations that can be performed.
     This Union type allows for specifying the operation (as a string literal indicating the type of action),
     and the required arguments for each operation type:
     - 'makedirs': Create a new directory; requires the path of the directory.
@@ -365,31 +366,14 @@
             with open(operation.path, "w") as file:
                 file.write(operation.content)
         elif operation.operation == "chmod":
             os.chmod(operation.path, operation.mode)
         elif operation.operation == "rename":
             os.rename(operation.path, operation.content)
 
-def init_project():
-    """initialize a new project by creating index.json file"""
-    if os.path.exists("index.json"):
-        print("The 'index.json' file already exists. Please edit the existing file.")
-        return
-    
-    index_data = {
-        "details": {
-            "title": "Project Title",
-            "description": "Project Description",
-            "steps": [],
-        }
-    }
-    with open("index.json", "w") as index_file:
-        json.dump(index_data, index_file, ensure_ascii=False, indent=4)
-    print("Project initialized successfully. Please edit the 'index.json' file to add steps.")
-
 def main():
     """
     This function orchestrates the entire process of adding a new step to the scenario,
     from taking user input to updating the file system and the index.json file.
     It ensures that the 'index.json' file is present, gathers the current directory structure,
     prompts the user for the new step's title and number, calculates the necessary file operations,
     and applies those changes to the file system and the index.json file.
```

### Comparing `killercoda_cli-1.0.8/tests/test_cli.py` & `killercoda_cli-1.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.8/tests/test_integration_cli.py` & `killercoda_cli-1.1.0/tests/test_integration_cli.py`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.8/.gitignore` & `killercoda_cli-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.8/LICENSE.txt` & `killercoda_cli-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.8/README.md` & `killercoda_cli-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.8/pyproject.toml` & `killercoda_cli-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 [project]
 name = "killercoda-cli"
 dynamic = ["version"]
 description = 'A CLI helper for writing killercoda scenarios and managing steps'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
+dependencies = [
+    "inquirer",
+]
 keywords = []
 authors = [
   { name = "Piotr Zaniewski", email = "piotrzan@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
@@ -20,15 +23,14 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = []
 
 [project.urls]
 Documentation = "https://github.com/unknown/killercoda-cli#readme"
 Issues = "https://github.com/unknown/killercoda-cli/issues"
 Source = "https://github.com/unknown/killercoda-cli"
 
 [project.scripts]
```

### Comparing `killercoda_cli-1.0.8/PKG-INFO` & `killercoda_cli-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: killercoda-cli
-Version: 1.0.8
+Version: 1.1.0
 Summary: A CLI helper for writing killercoda scenarios and managing steps
 Project-URL: Documentation, https://github.com/unknown/killercoda-cli#readme
 Project-URL: Issues, https://github.com/unknown/killercoda-cli/issues
 Project-URL: Source, https://github.com/unknown/killercoda-cli
 Author-email: Piotr Zaniewski <piotrzan@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Requires-Dist: inquirer
 Description-Content-Type: text/markdown
 
 # killercoda-cli
 
 [![PyPI - Version](https://img.shields.io/pypi/v/killercoda-cli.svg)](https://pypi.org/project/killercoda-cli)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/killercoda-cli.svg)](https://pypi.org/project/killercoda-cli)
 [![codecov](https://codecov.io/gh/Piotr1215/killercoda-cli/graph/badge.svg?token=2NVHJY2T3L)](https://codecov.io/gh/Piotr1215/killercoda-cli)
```

