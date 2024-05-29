# Comparing `tmp/lato-0.9.2.tar.gz` & `tmp/lato-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lato-0.9.2.tar", max compression
+gzip compressed data, was "lato-0.9.3.tar", max compression
```

## Comparing `lato-0.9.2.tar` & `lato-0.9.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1077 2023-11-29 13:50:48.751282 lato-0.9.2/LICENSE
--rw-r--r--   0        0        0    11960 2024-03-04 22:53:22.257455 lato-0.9.2/README.md
--rw-r--r--   0        0        0     1344 2024-03-04 22:53:22.257875 lato-0.9.2/lato/__init__.py
--rw-r--r--   0        0        0     6958 2024-03-04 22:53:22.258298 lato-0.9.2/lato/application.py
--rw-r--r--   0        0        0     3422 2024-03-04 22:53:22.258662 lato-0.9.2/lato/application_module.py
--rw-r--r--   0        0        0      797 2024-03-04 22:53:22.259012 lato-0.9.2/lato/compositon.py
--rw-r--r--   0        0        0     8665 2024-03-04 22:53:22.259455 lato-0.9.2/lato/dependency_provider.py
--rw-r--r--   0        0        0      420 2024-02-28 14:16:32.596645 lato-0.9.2/lato/message.py
--rw-r--r--   0        0        0     1360 2024-03-04 22:53:22.259844 lato-0.9.2/lato/testing.py
--rw-r--r--   0        0        0     8736 2024-03-04 22:53:22.260216 lato-0.9.2/lato/transaction_context.py
--rw-r--r--   0        0        0      140 2024-03-04 22:53:22.260352 lato-0.9.2/lato/types.py
--rw-r--r--   0        0        0      420 2023-12-07 15:20:34.564378 lato-0.9.2/lato/utils.py
--rw-r--r--   0        0        0     1150 2024-03-07 17:16:32.649659 lato-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    12934 1970-01-01 00:00:00.000000 lato-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-11-29 13:50:48.751282 lato-0.9.3/LICENSE
+-rw-r--r--   0        0        0    11959 2024-03-07 17:24:19.771136 lato-0.9.3/README.md
+-rw-r--r--   0        0        0     1344 2024-03-04 22:53:22.257875 lato-0.9.3/lato/__init__.py
+-rw-r--r--   0        0        0     6958 2024-03-04 22:53:22.258298 lato-0.9.3/lato/application.py
+-rw-r--r--   0        0        0     3422 2024-03-04 22:53:22.258662 lato-0.9.3/lato/application_module.py
+-rw-r--r--   0        0        0      797 2024-03-04 22:53:22.259012 lato-0.9.3/lato/compositon.py
+-rw-r--r--   0        0        0     8665 2024-03-04 22:53:22.259455 lato-0.9.3/lato/dependency_provider.py
+-rw-r--r--   0        0        0      420 2024-02-28 14:16:32.596645 lato-0.9.3/lato/message.py
+-rw-r--r--   0        0        0       65 2024-03-06 16:47:15.020320 lato-0.9.3/lato/py.typed
+-rw-r--r--   0        0        0     1360 2024-03-04 22:53:22.259844 lato-0.9.3/lato/testing.py
+-rw-r--r--   0        0        0     8736 2024-03-04 22:53:22.260216 lato-0.9.3/lato/transaction_context.py
+-rw-r--r--   0        0        0      140 2024-03-04 22:53:22.260352 lato-0.9.3/lato/types.py
+-rw-r--r--   0        0        0      420 2023-12-07 15:20:34.564378 lato-0.9.3/lato/utils.py
+-rw-r--r--   0        0        0     1150 2024-03-07 22:28:40.681367 lato-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    12933 1970-01-01 00:00:00.000000 lato-0.9.3/PKG-INFO
```

### Comparing `lato-0.9.2/LICENSE` & `lato-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lato-0.9.2/README.md` & `lato-0.9.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Lato is a Python microframework designed for building **modular monoliths** and **loosely coupled** applications.
 Based on dependency injection and Python 3.6+ type hints.
 
 ---
 
 **Documentation**: <a href="https://lato.readthedocs.io" target="_blank">https://lato.readthedocs.io</a>
 
-**Source Code**: <a href="https://github.com/pgorecki/lato" target="_blank">https://github.com/pgorecki/lator</a>
+**Source Code**: <a href="https://github.com/pgorecki/lato" target="_blank">https://github.com/pgorecki/lato</a>
 
 ---
 
 ## Features
 
 - **Modularity**: Organize your application into smaller, independent modules for better maintainability.
```

### Comparing `lato-0.9.2/lato/__init__.py` & `lato-0.9.3/lato/__init__.py`

 * *Files identical despite different names*

### Comparing `lato-0.9.2/lato/application.py` & `lato-0.9.3/lato/application.py`

 * *Files identical despite different names*

### Comparing `lato-0.9.2/lato/application_module.py` & `lato-0.9.3/lato/application_module.py`

 * *Files identical despite different names*

### Comparing `lato-0.9.2/lato/compositon.py` & `lato-0.9.3/lato/compositon.py`

 * *Files identical despite different names*

### Comparing `lato-0.9.2/lato/dependency_provider.py` & `lato-0.9.3/lato/dependency_provider.py`

 * *Files identical despite different names*

### Comparing `lato-0.9.2/lato/testing.py` & `lato-0.9.3/lato/testing.py`

 * *Files identical despite different names*

### Comparing `lato-0.9.2/lato/transaction_context.py` & `lato-0.9.3/lato/transaction_context.py`

 * *Files identical despite different names*

### Comparing `lato-0.9.2/pyproject.toml` & `lato-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lato"
-version = "0.9.2"
+version = "0.9.3"
 description = "Lato is a Python microframework designed for building modular monoliths and loosely coupled applications."
 authors = ["Przemysław Górecki <przemyslaw.gorecki@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/pgorecki/lato"
 homepage = "https://github.com/pgorecki/lato"
 documentation = "https://lato.readthedocs.io"
 classifiers = [
```

### Comparing `lato-0.9.2/PKG-INFO` & `lato-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lato
-Version: 0.9.2
+Version: 0.9.3
 Summary: Lato is a Python microframework designed for building modular monoliths and loosely coupled applications.
 Home-page: https://github.com/pgorecki/lato
 License: MIT
 Author: Przemysław Górecki
 Author-email: przemyslaw.gorecki@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -33,15 +33,15 @@
 Lato is a Python microframework designed for building **modular monoliths** and **loosely coupled** applications.
 Based on dependency injection and Python 3.6+ type hints.
 
 ---
 
 **Documentation**: <a href="https://lato.readthedocs.io" target="_blank">https://lato.readthedocs.io</a>
 
-**Source Code**: <a href="https://github.com/pgorecki/lato" target="_blank">https://github.com/pgorecki/lator</a>
+**Source Code**: <a href="https://github.com/pgorecki/lato" target="_blank">https://github.com/pgorecki/lato</a>
 
 ---
 
 ## Features
 
 - **Modularity**: Organize your application into smaller, independent modules for better maintainability.
```

