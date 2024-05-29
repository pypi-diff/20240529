# Comparing `tmp/pygmailcleaner-0.1.0.tar.gz` & `tmp/pygmailcleaner-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmailcleaner-0.1.0.tar", max compression
+gzip compressed data, was "pygmailcleaner-0.1.1.tar", max compression
```

## Comparing `pygmailcleaner-0.1.0.tar` & `pygmailcleaner-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4166 2024-05-27 17:15:23.085854 pygmailcleaner-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-26 17:26:47.824688 pygmailcleaner-0.1.0/pygmailcleaner/__init__.py
--rw-r--r--   0        0        0     7634 2024-05-26 22:06:23.067439 pygmailcleaner-0.1.0/pygmailcleaner/main.py
--rw-r--r--   0        0        0       90 2024-05-26 17:26:57.786320 pygmailcleaner-0.1.0/pygmailcleaner/utils/__init__.py
--rw-r--r--   0        0        0     6095 2024-05-26 10:51:27.664423 pygmailcleaner-0.1.0/pygmailcleaner/utils/cli.py
--rw-r--r--   0        0        0      833 2024-03-12 20:49:07.871059 pygmailcleaner-0.1.0/pygmailcleaner/utils/commands.py
--rw-r--r--   0        0        0      572 2024-05-26 10:49:26.184643 pygmailcleaner-0.1.0/pygmailcleaner/utils/formatting.py
--rw-r--r--   0        0        0     3277 2024-05-26 17:29:18.600232 pygmailcleaner-0.1.0/pygmailcleaner/utils/smpt.py
--rw-r--r--   0        0        0     1735 2024-02-11 16:40:37.113845 pygmailcleaner-0.1.0/pygmailcleaner/utils/testing.py
--rw-r--r--   0        0        0      516 2024-05-27 08:13:01.184118 pygmailcleaner-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4751 1970-01-01 00:00:00.000000 pygmailcleaner-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4165 2024-05-29 21:46:49.622527 pygmailcleaner-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 21:46:49.622527 pygmailcleaner-0.1.1/pygmailcleaner/__init__.py
+-rw-r--r--   0        0        0     7634 2024-05-29 21:46:49.622527 pygmailcleaner-0.1.1/pygmailcleaner/main.py
+-rw-r--r--   0        0        0       90 2024-05-29 21:46:49.622527 pygmailcleaner-0.1.1/pygmailcleaner/utils/__init__.py
+-rw-r--r--   0        0        0     6095 2024-05-29 21:46:49.622527 pygmailcleaner-0.1.1/pygmailcleaner/utils/cli.py
+-rw-r--r--   0        0        0      833 2024-05-29 21:46:49.622527 pygmailcleaner-0.1.1/pygmailcleaner/utils/commands.py
+-rw-r--r--   0        0        0      572 2024-05-29 21:46:49.622527 pygmailcleaner-0.1.1/pygmailcleaner/utils/formatting.py
+-rw-r--r--   0        0        0     3277 2024-05-29 21:46:49.622527 pygmailcleaner-0.1.1/pygmailcleaner/utils/smpt.py
+-rw-r--r--   0        0        0     1735 2024-05-29 21:46:49.622527 pygmailcleaner-0.1.1/pygmailcleaner/utils/testing.py
+-rw-r--r--   0        0        0      516 2024-05-29 21:46:49.622527 pygmailcleaner-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4750 1970-01-01 00:00:00.000000 pygmailcleaner-0.1.1/PKG-INFO
```

### Comparing `pygmailcleaner-0.1.0/README.md` & `pygmailcleaner-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -134,10 +134,10 @@
 
 ## License
 
 This project is licensed under the MIT License.
 
 ## Contact
 
-For any questions or issues, please contact [your-email@gmail.com].
+For any questions or issues, please contact [ruperarup@gmail.com].
 
 Thank you for using PyGmailCleaner!
```

### Comparing `pygmailcleaner-0.1.0/pygmailcleaner/main.py` & `pygmailcleaner-0.1.1/pygmailcleaner/main.py`

 * *Files identical despite different names*

### Comparing `pygmailcleaner-0.1.0/pygmailcleaner/utils/cli.py` & `pygmailcleaner-0.1.1/pygmailcleaner/utils/cli.py`

 * *Files identical despite different names*

### Comparing `pygmailcleaner-0.1.0/pygmailcleaner/utils/commands.py` & `pygmailcleaner-0.1.1/pygmailcleaner/utils/commands.py`

 * *Files identical despite different names*

### Comparing `pygmailcleaner-0.1.0/pygmailcleaner/utils/formatting.py` & `pygmailcleaner-0.1.1/pygmailcleaner/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pygmailcleaner-0.1.0/pygmailcleaner/utils/smpt.py` & `pygmailcleaner-0.1.1/pygmailcleaner/utils/smpt.py`

 * *Files identical despite different names*

### Comparing `pygmailcleaner-0.1.0/pygmailcleaner/utils/testing.py` & `pygmailcleaner-0.1.1/pygmailcleaner/utils/testing.py`

 * *Files identical despite different names*

### Comparing `pygmailcleaner-0.1.0/pyproject.toml` & `pygmailcleaner-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygmailcleaner"
-version = "0.1.0"
+version = "0.1.1"
 description = "A tool to clear out your gmail inbox"
 authors = ["Rupert Arup <rupertarup@gmail.com>"]
 packages = [{include = "pygmailcleaner"}]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
```

### Comparing `pygmailcleaner-0.1.0/PKG-INFO` & `pygmailcleaner-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmailcleaner
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool to clear out your gmail inbox
 License: MIT
 Author: Rupert Arup
 Author-email: rupertarup@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -151,10 +151,10 @@
 
 ## License
 
 This project is licensed under the MIT License.
 
 ## Contact
 
-For any questions or issues, please contact [your-email@gmail.com].
+For any questions or issues, please contact [ruperarup@gmail.com].
 
 Thank you for using PyGmailCleaner!
```

