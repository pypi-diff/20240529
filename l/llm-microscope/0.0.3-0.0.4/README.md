# Comparing `tmp/llm_microscope-0.0.3.tar.gz` & `tmp/llm_microscope-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_microscope-0.0.3.tar", last modified: Wed May 29 11:31:09 2024, max compression
+gzip compressed data, was "llm_microscope-0.0.4.tar", last modified: Wed May 29 11:33:47 2024, max compression
```

## Comparing `llm_microscope-0.0.3.tar` & `llm_microscope-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-05-29 11:31:09.499246 llm_microscope-0.0.3/
--rw-r--r--   0 matthew    (501) staff       (20)    11372 2024-05-22 10:44:00.000000 llm_microscope-0.0.3/LICENSE
--rw-r--r--   0 matthew    (501) staff       (20)      680 2024-05-29 11:31:09.499140 llm_microscope-0.0.3/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)      202 2024-05-22 10:46:59.000000 llm_microscope-0.0.3/README.md
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-05-29 11:31:09.498529 llm_microscope-0.0.3/llm_microscope/
--rw-r--r--   0 matthew    (501) staff       (20)       25 2024-05-22 11:11:06.000000 llm_microscope-0.0.3/llm_microscope/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)     4012 2024-05-29 11:30:02.000000 llm_microscope-0.0.3/llm_microscope/functions.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-05-29 11:31:09.499007 llm_microscope-0.0.3/llm_microscope.egg-info/
--rw-r--r--   0 matthew    (501) staff       (20)      680 2024-05-29 11:31:09.000000 llm_microscope-0.0.3/llm_microscope.egg-info/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)      270 2024-05-29 11:31:09.000000 llm_microscope-0.0.3/llm_microscope.egg-info/SOURCES.txt
--rw-r--r--   0 matthew    (501) staff       (20)        1 2024-05-29 11:31:09.000000 llm_microscope-0.0.3/llm_microscope.egg-info/dependency_links.txt
--rw-r--r--   0 matthew    (501) staff       (20)       13 2024-05-29 11:31:09.000000 llm_microscope-0.0.3/llm_microscope.egg-info/requires.txt
--rw-r--r--   0 matthew    (501) staff       (20)       15 2024-05-29 11:31:09.000000 llm_microscope-0.0.3/llm_microscope.egg-info/top_level.txt
--rw-r--r--   0 matthew    (501) staff       (20)       38 2024-05-29 11:31:09.499280 llm_microscope-0.0.3/setup.cfg
--rw-r--r--   0 matthew    (501) staff       (20)      715 2024-05-29 11:30:34.000000 llm_microscope-0.0.3/setup.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-05-29 11:33:47.083831 llm_microscope-0.0.4/
+-rw-r--r--   0 matthew    (501) staff       (20)    11372 2024-05-22 10:44:00.000000 llm_microscope-0.0.4/LICENSE
+-rw-r--r--   0 matthew    (501) staff       (20)      680 2024-05-29 11:33:47.083714 llm_microscope-0.0.4/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)      202 2024-05-22 10:46:59.000000 llm_microscope-0.0.4/README.md
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-05-29 11:33:47.082968 llm_microscope-0.0.4/llm_microscope/
+-rw-r--r--   0 matthew    (501) staff       (20)       25 2024-05-22 11:11:06.000000 llm_microscope-0.0.4/llm_microscope/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)     4012 2024-05-29 11:30:02.000000 llm_microscope-0.0.4/llm_microscope/functions.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-05-29 11:33:47.083567 llm_microscope-0.0.4/llm_microscope.egg-info/
+-rw-r--r--   0 matthew    (501) staff       (20)      680 2024-05-29 11:33:47.000000 llm_microscope-0.0.4/llm_microscope.egg-info/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)      270 2024-05-29 11:33:47.000000 llm_microscope-0.0.4/llm_microscope.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew    (501) staff       (20)        1 2024-05-29 11:33:47.000000 llm_microscope-0.0.4/llm_microscope.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew    (501) staff       (20)       13 2024-05-29 11:33:47.000000 llm_microscope-0.0.4/llm_microscope.egg-info/requires.txt
+-rw-r--r--   0 matthew    (501) staff       (20)       15 2024-05-29 11:33:47.000000 llm_microscope-0.0.4/llm_microscope.egg-info/top_level.txt
+-rw-r--r--   0 matthew    (501) staff       (20)       38 2024-05-29 11:33:47.083925 llm_microscope-0.0.4/setup.cfg
+-rw-r--r--   0 matthew    (501) staff       (20)      715 2024-05-29 11:33:16.000000 llm_microscope-0.0.4/setup.py
```

### Comparing `llm_microscope-0.0.3/LICENSE` & `llm_microscope-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_microscope-0.0.3/PKG-INFO` & `llm_microscope-0.0.4/llm_microscope.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: llm_microscope
-Version: 0.0.3
+Name: llm-microscope
+Version: 0.0.4
 Summary: Official implementation of the LLM-analysis functions for the paper "Your Transformer is Secretly Linear"
 Home-page: https://github.com/AIRI-Institute/LLM-Microscope
 Author: Matvey Mikhalchuk
 Author-email: mikhalchuk@airi.net
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `llm_microscope-0.0.3/llm_microscope/functions.py` & `llm_microscope-0.0.4/llm_microscope/functions.py`

 * *Files identical despite different names*

### Comparing `llm_microscope-0.0.3/llm_microscope.egg-info/PKG-INFO` & `llm_microscope-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: llm-microscope
-Version: 0.0.3
+Name: llm_microscope
+Version: 0.0.4
 Summary: Official implementation of the LLM-analysis functions for the paper "Your Transformer is Secretly Linear"
 Home-page: https://github.com/AIRI-Institute/LLM-Microscope
 Author: Matvey Mikhalchuk
 Author-email: mikhalchuk@airi.net
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `llm_microscope-0.0.3/setup.py` & `llm_microscope-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = [
 	"torch>=2.1.0"
 ]
 
 setuptools.setup(
 	name="llm_microscope",
-	version="0.0.3",
+	version="0.0.4",
 	author="Matvey Mikhalchuk",
 	author_email="mikhalchuk@airi.net",
 	description="Official implementation of the LLM-analysis functions for the paper \"Your Transformer is Secretly Linear\"",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/AIRI-Institute/LLM-Microscope",
 	packages=setuptools.find_packages(),
```

