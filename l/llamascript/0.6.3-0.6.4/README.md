# Comparing `tmp/llamascript-0.6.3.tar.gz` & `tmp/llamascript-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamascript-0.6.3.tar", last modified: Sun May 26 01:50:27 2024, max compression
+gzip compressed data, was "llamascript-0.6.4.tar", last modified: Wed May 29 14:47:41 2024, max compression
```

## Comparing `llamascript-0.6.3.tar` & `llamascript-0.6.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:50:27.361544 llamascript-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-26 01:50:23.000000 llamascript-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-26 01:50:27.361544 llamascript-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-26 01:50:23.000000 llamascript-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:50:27.357544 llamascript-0.6.3/llamascript/
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-26 01:50:23.000000 llamascript-0.6.3/llamascript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:50:27.357544 llamascript-0.6.3/llamascript.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-26 01:50:27.000000 llamascript-0.6.3/llamascript.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-26 01:50:27.000000 llamascript-0.6.3/llamascript.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:50:27.000000 llamascript-0.6.3/llamascript.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-26 01:50:27.000000 llamascript-0.6.3/llamascript.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-26 01:50:27.000000 llamascript-0.6.3/llamascript.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 01:50:27.000000 llamascript-0.6.3/llamascript.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 01:50:27.361544 llamascript-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-26 01:50:23.000000 llamascript-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:47:41.664721 llamascript-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-29 14:47:35.000000 llamascript-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-29 14:47:41.664721 llamascript-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-29 14:47:35.000000 llamascript-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:47:41.664721 llamascript-0.6.4/llamascript/
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-05-29 14:47:35.000000 llamascript-0.6.4/llamascript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:47:41.664721 llamascript-0.6.4/llamascript.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-29 14:47:41.000000 llamascript-0.6.4/llamascript.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-29 14:47:41.000000 llamascript-0.6.4/llamascript.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:47:41.000000 llamascript-0.6.4/llamascript.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-29 14:47:41.000000 llamascript-0.6.4/llamascript.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 14:47:41.000000 llamascript-0.6.4/llamascript.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 14:47:41.000000 llamascript-0.6.4/llamascript.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:47:41.664721 llamascript-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-29 14:47:35.000000 llamascript-0.6.4/setup.py
```

### Comparing `llamascript-0.6.3/LICENSE` & `llamascript-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llamascript-0.6.3/PKG-INFO` & `llamascript-0.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamascript
-Version: 0.6.3
+Version: 0.6.4
 Summary: No-code AI chatbot using Ollama.
 Home-page: https://github.com/WolfTheDeveloper/llamascript
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,14 +25,16 @@
 [![Upload to PyPi](https://github.com/Project-Llama/llamascript/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Project-Llama/llamascript/actions/workflows/python-publish.yml)
 [![CodeQL](https://github.com/Project-Llama/llamascript/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/Project-Llama/llamascript/actions/workflows/github-code-scanning/codeql)
 
 [![VS Code Extension Downloads](https://img.shields.io/visual-studio-marketplace/d/WolfTheDev.llamascript?label=VS-Code%20Downloads)](https://marketplace.visualstudio.com/items?itemName=WolfTheDev.llamascript)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/Project-Llama/llamascript?label=Commits)
 ![GitHub License](https://img.shields.io/github/license/Project-Llama/llamascript?label=License)
 
+[![Discord](https://img.shields.io/badge/Join-Logo?style=flat&logo=discord&label=Discord&color=%235865F2)](http://discord.com/invite/RJ9ZDPM2Fx)
+
 LlamaScript is a no-code AI chatbot using Ollama.
 
 ## Table of Contents
 - [LlamaScript](#llamascript)
   - [Installation](#installation)
   - [Usage](#usage)
   - [License](#license)
```

### Comparing `llamascript-0.6.3/README.md` & `llamascript-0.6.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 [![Upload to PyPi](https://github.com/Project-Llama/llamascript/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Project-Llama/llamascript/actions/workflows/python-publish.yml)
 [![CodeQL](https://github.com/Project-Llama/llamascript/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/Project-Llama/llamascript/actions/workflows/github-code-scanning/codeql)
 
 [![VS Code Extension Downloads](https://img.shields.io/visual-studio-marketplace/d/WolfTheDev.llamascript?label=VS-Code%20Downloads)](https://marketplace.visualstudio.com/items?itemName=WolfTheDev.llamascript)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/Project-Llama/llamascript?label=Commits)
 ![GitHub License](https://img.shields.io/github/license/Project-Llama/llamascript?label=License)
 
+[![Discord](https://img.shields.io/badge/Join-Logo?style=flat&logo=discord&label=Discord&color=%235865F2)](http://discord.com/invite/RJ9ZDPM2Fx)
+
 LlamaScript is a no-code AI chatbot using Ollama.
 
 ## Table of Contents
 - [LlamaScript](#llamascript)
   - [Installation](#installation)
   - [Usage](#usage)
   - [License](#license)
```

### Comparing `llamascript-0.6.3/llamascript/__init__.py` & `llamascript-0.6.4/llamascript/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.3"
+__version__ = "0.6.4"
 
 import asyncio
 import ollama
 import logging
 import sys
 import subprocess
 import os
@@ -176,18 +176,14 @@
         action="version",
         version=f"LlamaScript version {__version__}",
         help="Display version information",
     )
 
     args = parser.parse_args()
 
-    if args.version:
-        print(f"llamascript version {__version__}")
-        sys.exit(0)
-
     if not (args.file_name.endswith(".llama") or args.file_name == "llama"):
         logging.error("Invalid file type. Please provide a .llama or llama file.")
         print("Invalid file type. Please provide a .llama or llama file.")
         sys.exit(1)
 
     try:
         l = llama()
```

### Comparing `llamascript-0.6.3/llamascript.egg-info/PKG-INFO` & `llamascript-0.6.4/llamascript.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamascript
-Version: 0.6.3
+Version: 0.6.4
 Summary: No-code AI chatbot using Ollama.
 Home-page: https://github.com/WolfTheDeveloper/llamascript
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,14 +25,16 @@
 [![Upload to PyPi](https://github.com/Project-Llama/llamascript/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Project-Llama/llamascript/actions/workflows/python-publish.yml)
 [![CodeQL](https://github.com/Project-Llama/llamascript/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/Project-Llama/llamascript/actions/workflows/github-code-scanning/codeql)
 
 [![VS Code Extension Downloads](https://img.shields.io/visual-studio-marketplace/d/WolfTheDev.llamascript?label=VS-Code%20Downloads)](https://marketplace.visualstudio.com/items?itemName=WolfTheDev.llamascript)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/Project-Llama/llamascript?label=Commits)
 ![GitHub License](https://img.shields.io/github/license/Project-Llama/llamascript?label=License)
 
+[![Discord](https://img.shields.io/badge/Join-Logo?style=flat&logo=discord&label=Discord&color=%235865F2)](http://discord.com/invite/RJ9ZDPM2Fx)
+
 LlamaScript is a no-code AI chatbot using Ollama.
 
 ## Table of Contents
 - [LlamaScript](#llamascript)
   - [Installation](#installation)
   - [Usage](#usage)
   - [License](#license)
```

### Comparing `llamascript-0.6.3/setup.py` & `llamascript-0.6.4/setup.py`

 * *Files identical despite different names*

