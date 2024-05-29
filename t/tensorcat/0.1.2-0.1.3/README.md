# Comparing `tmp/tensorcat-0.1.2.tar.gz` & `tmp/tensorcat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcat-0.1.2.tar", max compression
+gzip compressed data, was "tensorcat-0.1.3.tar", max compression
```

## Comparing `tensorcat-0.1.2.tar` & `tensorcat-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     5058 2024-04-26 03:47:48.996699 tensorcat-0.1.2/README.md
--rw-r--r--   0        0        0      460 2024-04-26 03:56:12.720285 tensorcat-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       72 2024-04-22 08:44:47.453857 tensorcat-0.1.2/tensorcat/__init__.py
--rw-r--r--   0        0        0     2001 2024-04-22 08:44:47.453976 tensorcat-0.1.2/tensorcat/cli.py
--rw-r--r--   0        0        0     2477 2024-04-22 08:44:47.454112 tensorcat-0.1.2/tensorcat/iterm2.py
--rw-r--r--   0        0        0     5952 2024-04-22 08:44:47.454301 tensorcat-0.1.2/tensorcat/tensorcat.py
--rw-r--r--   0        0        0     5693 1970-01-01 00:00:00.000000 tensorcat-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5058 2024-05-29 18:32:07.278912 tensorcat-0.1.3/README.md
+-rw-r--r--   0        0        0      405 2024-05-29 18:32:07.286912 tensorcat-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-05-29 18:32:07.286912 tensorcat-0.1.3/tensorcat/__init__.py
+-rw-r--r--   0        0        0     2001 2024-05-29 18:32:07.286912 tensorcat-0.1.3/tensorcat/cli.py
+-rw-r--r--   0        0        0     2477 2024-05-29 18:32:07.286912 tensorcat-0.1.3/tensorcat/iterm2.py
+-rw-r--r--   0        0        0     5952 2024-05-29 18:32:07.286912 tensorcat-0.1.3/tensorcat/tensorcat.py
+-rw-r--r--   0        0        0     5693 1970-01-01 00:00:00.000000 tensorcat-0.1.3/PKG-INFO
```

### Comparing `tensorcat-0.1.2/README.md` & `tensorcat-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tensorcat-0.1.2/tensorcat/cli.py` & `tensorcat-0.1.3/tensorcat/cli.py`

 * *Files identical despite different names*

### Comparing `tensorcat-0.1.2/tensorcat/iterm2.py` & `tensorcat-0.1.3/tensorcat/iterm2.py`

 * *Files identical despite different names*

### Comparing `tensorcat-0.1.2/tensorcat/tensorcat.py` & `tensorcat-0.1.3/tensorcat/tensorcat.py`

 * *Files identical despite different names*

### Comparing `tensorcat-0.1.2/PKG-INFO` & `tensorcat-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: tensorcat
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Zhengyu Yang
 Author-email: 25852061+zhengyu-yang@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: iPython (>=8.4.0,<9.0.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
-Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Description-Content-Type: text/markdown
 
 # tensorcat
 
 This utility provides an easy way to display an image/tensor/array in the terminal, notebook, and Python interpreter/debugger. It supports both batched and non-batched input and will automatically deduce its format (BCHW, HWC) and range (0-1, 0-255).
 
 ## How
```

