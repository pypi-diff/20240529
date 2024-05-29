# Comparing `tmp/ai_helpers_pyspark_utils-0.1.0a0.tar.gz` & `tmp/ai_helpers_pyspark_utils-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_helpers_pyspark_utils-0.1.0a0.tar", max compression
+gzip compressed data, was "ai_helpers_pyspark_utils-0.1.0a1.tar", max compression
```

## Comparing `ai_helpers_pyspark_utils-0.1.0a0.tar` & `ai_helpers_pyspark_utils-0.1.0a1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1322 2024-05-29 11:44:39.549677 ai_helpers_pyspark_utils-0.1.0a0/README.md
--rw-r--r--   0        0        0     1743 2024-05-29 13:19:04.569716 ai_helpers_pyspark_utils-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      447 2024-05-29 12:41:56.192753 ai_helpers_pyspark_utils-0.1.0a0/pyspark_utils/__init__.py
--rw-r--r--   0        0        0     3331 2024-05-29 12:44:47.904079 ai_helpers_pyspark_utils-0.1.0a0/pyspark_utils/utils.py
--rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 ai_helpers_pyspark_utils-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1333 2024-05-29 15:03:51.599158 ai_helpers_pyspark_utils-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1743 2024-05-29 15:03:51.599158 ai_helpers_pyspark_utils-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      447 2024-05-29 15:03:51.599158 ai_helpers_pyspark_utils-0.1.0a1/pyspark_utils/__init__.py
+-rw-r--r--   0        0        0     3331 2024-05-29 15:03:51.599158 ai_helpers_pyspark_utils-0.1.0a1/pyspark_utils/utils.py
+-rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 ai_helpers_pyspark_utils-0.1.0a1/PKG-INFO
```

### Comparing `ai_helpers_pyspark_utils-0.1.0a0/README.md` & `ai_helpers_pyspark_utils-0.1.0a1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   - [Contributing](#contributing)
 
 ## Installation
 
 You can install the `pyspark-utils` module via pip:
 
 ```bash
-pip install pyspark-utils
+pip install ai-helpers-pyspark-utils
 ```
 
 ## Getting Started
 
 First, import the module in your Python script:
 
 ```python
```

### Comparing `ai_helpers_pyspark_utils-0.1.0a0/pyproject.toml` & `ai_helpers_pyspark_utils-0.1.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-helpers-pyspark-utils"
-version = "0.1.0a0"
+version = "0.1.0a1"
 description = "Common pyspark utils"
 authors = ["Corentin Vasseur <vasseur.corentin@gmail.com>"]
 packages = [{ include = "pyspark_utils" }]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
```

### Comparing `ai_helpers_pyspark_utils-0.1.0a0/pyspark_utils/utils.py` & `ai_helpers_pyspark_utils-0.1.0a1/pyspark_utils/utils.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_pyspark_utils-0.1.0a0/PKG-INFO` & `ai_helpers_pyspark_utils-0.1.0a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-helpers-pyspark-utils
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Common pyspark utils
 Author: Corentin Vasseur
 Author-email: vasseur.corentin@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -28,15 +28,15 @@
   - [Contributing](#contributing)
 
 ## Installation
 
 You can install the `pyspark-utils` module via pip:
 
 ```bash
-pip install pyspark-utils
+pip install ai-helpers-pyspark-utils
 ```
 
 ## Getting Started
 
 First, import the module in your Python script:
 
 ```python
```

