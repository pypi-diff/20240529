# Comparing `tmp/pycolbertdb-0.2.0.tar.gz` & `tmp/pycolbertdb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycolbertdb-0.2.0.tar", max compression
+gzip compressed data, was "pycolbertdb-0.2.1.tar", max compression
```

## Comparing `pycolbertdb-0.2.0.tar` & `pycolbertdb-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1496 2024-05-29 20:39:24.412784 pycolbertdb-0.2.0/LICENSE
--rw-r--r--   0        0        0     1092 2024-05-29 20:39:24.412784 pycolbertdb-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-29 20:39:24.412784 pycolbertdb-0.2.0/pycolbertdb/__init__.py
--rw-r--r--   0        0        0    10186 2024-05-29 20:39:24.412784 pycolbertdb-0.2.0/pycolbertdb/client.py
--rw-r--r--   0        0        0     2229 2024-05-29 20:39:24.412784 pycolbertdb-0.2.0/pycolbertdb/models.py
--rw-r--r--   0        0        0      518 2024-05-29 20:39:24.412784 pycolbertdb-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 pycolbertdb-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1496 2024-05-29 20:40:27.583827 pycolbertdb-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1092 2024-05-29 20:40:27.583827 pycolbertdb-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 20:40:27.583827 pycolbertdb-0.2.1/pycolbertdb/__init__.py
+-rw-r--r--   0        0        0    10186 2024-05-29 20:40:27.583827 pycolbertdb-0.2.1/pycolbertdb/client.py
+-rw-r--r--   0        0        0     2229 2024-05-29 20:40:27.583827 pycolbertdb-0.2.1/pycolbertdb/models.py
+-rw-r--r--   0        0        0      518 2024-05-29 20:40:27.583827 pycolbertdb-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 pycolbertdb-0.2.1/PKG-INFO
```

### Comparing `pycolbertdb-0.2.0/LICENSE` & `pycolbertdb-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycolbertdb-0.2.0/README.md` & `pycolbertdb-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pycolbertdb-0.2.0/pycolbertdb/client.py` & `pycolbertdb-0.2.1/pycolbertdb/client.py`

 * *Files identical despite different names*

### Comparing `pycolbertdb-0.2.0/pycolbertdb/models.py` & `pycolbertdb-0.2.1/pycolbertdb/models.py`

 * *Files identical despite different names*

### Comparing `pycolbertdb-0.2.0/pyproject.toml` & `pycolbertdb-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycolbertdb"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python client for colbertdb"
 authors = ["Ryan Sloan <rysloan4@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `pycolbertdb-0.2.0/PKG-INFO` & `pycolbertdb-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycolbertdb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python client for colbertdb
 License: MIT
 Author: Ryan Sloan
 Author-email: rysloan4@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

