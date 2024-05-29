# Comparing `tmp/flatpack-3.5.5.tar.gz` & `tmp/flatpack-3.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.5.5.tar", last modified: Wed May 29 16:05:04 2024, max compression
+gzip compressed data, was "flatpack-3.5.6.tar", last modified: Wed May 29 16:21:12 2024, max compression
```

## Comparing `flatpack-3.5.5.tar` & `flatpack-3.5.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 16:05:04.073852 flatpack-3.5.5/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.5.5/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 16:05:04.073508 flatpack-3.5.5/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5019 2024-05-27 13:05:21.000000 flatpack-3.5.5/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 16:05:04.069914 flatpack-3.5.5/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.5.5/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.5.5/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.5.5/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.5.5/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 16:05:04.071773 flatpack-3.5.5/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.5.5/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     3489 2024-05-26 03:22:42.000000 flatpack-3.5.5/flatpack/engines/engine_llama_cpp.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.5.5/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.5.5/flatpack/load_engines.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-05-25 14:16:18.000000 flatpack-3.5.5/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    36263 2024-05-29 16:04:50.000000 flatpack-3.5.5/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 16:05:04.072682 flatpack-3.5.5/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.5.5/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.5.5/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.5.5/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.5.5/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.5.5/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.5.5/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     8911 2024-05-26 02:17:11.000000 flatpack-3.5.5/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 16:05:04.073038 flatpack-3.5.5/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 16:05:04.000000 flatpack-3.5.5/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-29 16:05:04.000000 flatpack-3.5.5/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-29 16:05:04.000000 flatpack-3.5.5/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-29 16:05:04.000000 flatpack-3.5.5/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      249 2024-05-29 16:05:04.000000 flatpack-3.5.5/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-29 16:05:04.000000 flatpack-3.5.5/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-29 16:05:04.073946 flatpack-3.5.5/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)      992 2024-05-29 16:04:57.000000 flatpack-3.5.5/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 16:21:12.233218 flatpack-3.5.6/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.5.6/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 16:21:12.232890 flatpack-3.5.6/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5019 2024-05-27 13:05:21.000000 flatpack-3.5.6/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 16:21:12.228850 flatpack-3.5.6/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.5.6/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.5.6/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.5.6/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.5.6/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 16:21:12.231152 flatpack-3.5.6/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.5.6/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     3489 2024-05-26 03:22:42.000000 flatpack-3.5.6/flatpack/engines/engine_llama_cpp.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.5.6/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       53 2024-05-29 16:20:58.000000 flatpack-3.5.6/flatpack/load_engines.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       60 2024-05-29 16:21:02.000000 flatpack-3.5.6/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    36263 2024-05-29 16:04:50.000000 flatpack-3.5.6/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 16:21:12.232128 flatpack-3.5.6/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.5.6/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.5.6/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.5.6/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.5.6/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.5.6/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.5.6/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     8911 2024-05-26 02:17:11.000000 flatpack-3.5.6/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 16:21:12.232502 flatpack-3.5.6/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 16:21:12.000000 flatpack-3.5.6/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-29 16:21:12.000000 flatpack-3.5.6/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-29 16:21:12.000000 flatpack-3.5.6/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-29 16:21:12.000000 flatpack-3.5.6/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      249 2024-05-29 16:21:12.000000 flatpack-3.5.6/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-29 16:21:12.000000 flatpack-3.5.6/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-29 16:21:12.233295 flatpack-3.5.6/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      992 2024-05-29 16:21:04.000000 flatpack-3.5.6/setup.py
```

### Comparing `flatpack-3.5.5/LICENSE` & `flatpack-3.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.5/PKG-INFO` & `flatpack-3.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.5.5
+Version: 3.5.6
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.5.5/README.md` & `flatpack-3.5.6/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.5/flatpack/agent_manager.py` & `flatpack-3.5.6/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.5/flatpack/datasets.py` & `flatpack-3.5.6/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.5/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.5.6/flatpack/engines/engine_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.5/flatpack/instructions.py` & `flatpack-3.5.6/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.5/flatpack/main.py` & `flatpack-3.5.6/flatpack/main.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.5/flatpack/modules/lstm.py` & `flatpack-3.5.6/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.5/flatpack/modules/rnn.py` & `flatpack-3.5.6/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.5/flatpack/parsers.py` & `flatpack-3.5.6/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.5/flatpack/vector_manager.py` & `flatpack-3.5.6/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.5/flatpack.egg-info/PKG-INFO` & `flatpack-3.5.6/flatpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.5.5
+Version: 3.5.6
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.5.5/flatpack.egg-info/SOURCES.txt` & `flatpack-3.5.6/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.5/setup.py` & `flatpack-3.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.5.5",
+    version="3.5.6",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "fastapi==0.110.2",
         "hnswlib==0.8.0",
         "httpx==0.27.0",
```

