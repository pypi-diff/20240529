# Comparing `tmp/atacama-0.1.4.tar.gz` & `tmp/atacama-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atacama-0.1.4.tar", max compression
+gzip compressed data, was "atacama-1.0.0.tar", max compression
```

## Comparing `atacama-0.1.4.tar` & `atacama-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       27 2024-05-22 20:25:41.510126 atacama-0.1.4/README_PUBLIC.md
--rw-r--r--   0        0        0       66 2024-05-22 20:25:41.510126 atacama-0.1.4/atacama/__init__.py
--rw-r--r--   0        0        0    19166 2024-05-22 20:25:41.510126 atacama-0.1.4/atacama/client.py
--rw-r--r--   0        0        0      523 2024-05-22 20:25:41.510126 atacama-0.1.4/atacama/exceptions.py
--rw-r--r--   0        0        0      816 2024-05-22 20:25:41.510126 atacama-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 atacama-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       27 2024-05-29 17:25:51.537525 atacama-1.0.0/README_PUBLIC.md
+-rw-r--r--   0        0        0       66 2024-05-29 17:25:51.537525 atacama-1.0.0/atacama/__init__.py
+-rw-r--r--   0        0        0    19166 2024-05-29 17:25:51.537525 atacama-1.0.0/atacama/client.py
+-rw-r--r--   0        0        0      523 2024-05-29 17:25:51.537525 atacama-1.0.0/atacama/exceptions.py
+-rw-r--r--   0        0        0      816 2024-05-29 17:25:51.541525 atacama-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 atacama-1.0.0/PKG-INFO
```

### Comparing `atacama-0.1.4/atacama/client.py` & `atacama-1.0.0/atacama/client.py`

 * *Files identical despite different names*

### Comparing `atacama-0.1.4/atacama/exceptions.py` & `atacama-1.0.0/atacama/exceptions.py`

 * *Files identical despite different names*

### Comparing `atacama-0.1.4/pyproject.toml` & `atacama-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atacama"
-version = "0.1.4"
+version = "1.0.0"
 description = "Python API for LLM"
 authors = ["Virtualitics Engineering <dev@virtualitics.com>"]
 license = "MIT LICENSE"
 packages = [{include = "atacama"}]
 classifiers=[
     "Programming Language :: Python :: 3",
     "Operating System :: Microsoft :: Windows :: Windows 10",
```

### Comparing `atacama-0.1.4/PKG-INFO` & `atacama-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atacama
-Version: 0.1.4
+Version: 1.0.0
 Summary: Python API for LLM
 License: MIT
 Author: Virtualitics Engineering
 Author-email: dev@virtualitics.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
```

