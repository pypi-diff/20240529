# Comparing `tmp/flatpack-3.5.2.tar.gz` & `tmp/flatpack-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.5.2.tar", last modified: Wed May 29 14:33:54 2024, max compression
+gzip compressed data, was "flatpack-3.5.3.tar", last modified: Wed May 29 14:47:45 2024, max compression
```

## Comparing `flatpack-3.5.2.tar` & `flatpack-3.5.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:33:54.933303 flatpack-3.5.2/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.5.2/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 14:33:54.933009 flatpack-3.5.2/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5019 2024-05-27 13:05:21.000000 flatpack-3.5.2/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:33:54.930396 flatpack-3.5.2/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.5.2/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.5.2/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.5.2/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.5.2/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:33:54.931798 flatpack-3.5.2/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.5.2/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     3489 2024-05-26 03:22:42.000000 flatpack-3.5.2/flatpack/engines/engine_llama_cpp.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.5.2/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.5.2/flatpack/load_engines.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-05-25 14:16:18.000000 flatpack-3.5.2/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    36256 2024-05-29 14:32:57.000000 flatpack-3.5.2/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:33:54.932324 flatpack-3.5.2/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.5.2/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.5.2/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.5.2/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.5.2/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.5.2/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.5.2/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     8911 2024-05-26 02:17:11.000000 flatpack-3.5.2/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:33:54.932593 flatpack-3.5.2/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 14:33:54.000000 flatpack-3.5.2/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-29 14:33:54.000000 flatpack-3.5.2/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-29 14:33:54.000000 flatpack-3.5.2/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-29 14:33:54.000000 flatpack-3.5.2/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      249 2024-05-29 14:33:54.000000 flatpack-3.5.2/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-29 14:33:54.000000 flatpack-3.5.2/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-29 14:33:54.933373 flatpack-3.5.2/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)      992 2024-05-29 13:36:26.000000 flatpack-3.5.2/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:47:45.136839 flatpack-3.5.3/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.5.3/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 14:47:45.136573 flatpack-3.5.3/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5019 2024-05-27 13:05:21.000000 flatpack-3.5.3/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:47:45.133886 flatpack-3.5.3/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.5.3/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.5.3/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.5.3/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.5.3/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:47:45.135405 flatpack-3.5.3/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.5.3/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     3489 2024-05-26 03:22:42.000000 flatpack-3.5.3/flatpack/engines/engine_llama_cpp.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.5.3/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.5.3/flatpack/load_engines.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-05-25 14:16:18.000000 flatpack-3.5.3/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    36279 2024-05-29 14:47:31.000000 flatpack-3.5.3/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:47:45.135953 flatpack-3.5.3/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.5.3/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.5.3/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.5.3/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.5.3/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.5.3/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.5.3/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     8911 2024-05-26 02:17:11.000000 flatpack-3.5.3/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-29 14:47:45.136226 flatpack-3.5.3/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-29 14:47:45.000000 flatpack-3.5.3/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-29 14:47:45.000000 flatpack-3.5.3/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-29 14:47:45.000000 flatpack-3.5.3/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-29 14:47:45.000000 flatpack-3.5.3/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      249 2024-05-29 14:47:45.000000 flatpack-3.5.3/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-29 14:47:45.000000 flatpack-3.5.3/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-29 14:47:45.136900 flatpack-3.5.3/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      992 2024-05-29 14:45:20.000000 flatpack-3.5.3/setup.py
```

### Comparing `flatpack-3.5.2/LICENSE` & `flatpack-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.2/PKG-INFO` & `flatpack-3.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.5.2
+Version: 3.5.3
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.5.2/README.md` & `flatpack-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.2/flatpack/agent_manager.py` & `flatpack-3.5.3/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.2/flatpack/datasets.py` & `flatpack-3.5.3/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.2/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.5.3/flatpack/engines/engine_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.2/flatpack/instructions.py` & `flatpack-3.5.3/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.2/flatpack/main.py` & `flatpack-3.5.3/flatpack/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,17 @@
             filedata = file.read()
 
         newdata = re.sub(pattern, replacement, filedata)
 
         with open(file_path, 'w') as file:
             file.write(newdata)
 
-    print(f"Contents of template copied to {flatpack_name}.")
+    shutil.rmtree(template_dir)
+
+    print(f"Successfully created {flatpack_name}.")
 
 
 def fpk_display_disclaimer(directory_name: str, local: bool):
     """Display a disclaimer message with details about a specific flatpack.
 
     Args:
         directory_name (str): Name of the flatpack directory.
```

### Comparing `flatpack-3.5.2/flatpack/modules/lstm.py` & `flatpack-3.5.3/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.2/flatpack/modules/rnn.py` & `flatpack-3.5.3/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.2/flatpack/parsers.py` & `flatpack-3.5.3/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.2/flatpack/vector_manager.py` & `flatpack-3.5.3/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.2/flatpack.egg-info/PKG-INFO` & `flatpack-3.5.3/flatpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.5.2
+Version: 3.5.3
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.5.2/flatpack.egg-info/SOURCES.txt` & `flatpack-3.5.3/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.2/setup.py` & `flatpack-3.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.5.2",
+    version="3.5.3",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "fastapi==0.110.2",
         "hnswlib==0.8.0",
         "httpx==0.27.0",
```

