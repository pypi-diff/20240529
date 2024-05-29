# Comparing `tmp/tromero_tailor-0.0.18.tar.gz` & `tmp/tromero_tailor-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tromero_tailor-0.0.18.tar", last modified: Wed May 22 13:25:38 2024, max compression
+gzip compressed data, was "tromero_tailor-0.0.19.tar", last modified: Wed May 29 14:31:02 2024, max compression
```

## Comparing `tromero_tailor-0.0.18.tar` & `tromero_tailor-0.0.19.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-22 13:25:38.219743 tromero_tailor-0.0.18/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-22 13:25:38.219514 tromero_tailor-0.0.18/PKG-INFO
--rw-r--r--   0 tadhgamin   (501) staff       (20)      942 2024-04-08 16:49:32.000000 tromero_tailor-0.0.18/README.md
--rw-r--r--   0 tadhgamin   (501) staff       (20)       38 2024-05-22 13:25:38.219785 tromero_tailor-0.0.18/setup.cfg
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1633 2024-05-22 13:25:25.000000 tromero_tailor-0.0.18/setup.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-22 13:25:38.217361 tromero_tailor-0.0.18/tests/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     3672 2024-04-17 14:55:07.000000 tromero_tailor-0.0.18/tests/test.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-22 13:25:38.218295 tromero_tailor-0.0.18/tromero_tailor/
--rw-r--r--   0 tadhgamin   (501) staff       (20)       30 2024-04-08 15:07:54.000000 tromero_tailor-0.0.18/tromero_tailor/__init__.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)     2131 2024-05-22 13:25:19.000000 tromero_tailor-0.0.18/tromero_tailor/tromero_requests.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)      446 2024-04-12 11:06:15.000000 tromero_tailor-0.0.18/tromero_tailor/tromero_utils.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)     3247 2024-05-22 12:24:04.000000 tromero_tailor-0.0.18/tromero_tailor/wrapper.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-22 13:25:38.219193 tromero_tailor-0.0.18/tromero_tailor.egg-info/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-22 13:25:38.000000 tromero_tailor-0.0.18/tromero_tailor.egg-info/PKG-INFO
--rw-r--r--   0 tadhgamin   (501) staff       (20)      341 2024-05-22 13:25:38.000000 tromero_tailor-0.0.18/tromero_tailor.egg-info/SOURCES.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)        1 2024-05-22 13:25:38.000000 tromero_tailor-0.0.18/tromero_tailor.egg-info/dependency_links.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)      304 2024-05-22 13:25:38.000000 tromero_tailor-0.0.18/tromero_tailor.egg-info/requires.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)       15 2024-05-22 13:25:38.000000 tromero_tailor-0.0.18/tromero_tailor.egg-info/top_level.txt
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-29 14:31:02.619495 tromero_tailor-0.0.19/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-29 14:31:02.619288 tromero_tailor-0.0.19/PKG-INFO
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      942 2024-04-08 16:49:32.000000 tromero_tailor-0.0.19/README.md
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       38 2024-05-29 14:31:02.619540 tromero_tailor-0.0.19/setup.cfg
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1633 2024-05-29 14:31:01.000000 tromero_tailor-0.0.19/setup.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-29 14:31:02.617430 tromero_tailor-0.0.19/tests/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     3672 2024-04-17 14:55:07.000000 tromero_tailor-0.0.19/tests/test.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-29 14:31:02.618270 tromero_tailor-0.0.19/tromero_tailor/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       30 2024-04-08 15:07:54.000000 tromero_tailor-0.0.19/tromero_tailor/__init__.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     2131 2024-05-22 13:25:19.000000 tromero_tailor-0.0.19/tromero_tailor/tromero_requests.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      446 2024-04-12 11:06:15.000000 tromero_tailor-0.0.19/tromero_tailor/tromero_utils.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     4935 2024-05-29 13:10:17.000000 tromero_tailor-0.0.19/tromero_tailor/wrapper.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-29 14:31:02.619033 tromero_tailor-0.0.19/tromero_tailor.egg-info/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-29 14:31:02.000000 tromero_tailor-0.0.19/tromero_tailor.egg-info/PKG-INFO
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      341 2024-05-29 14:31:02.000000 tromero_tailor-0.0.19/tromero_tailor.egg-info/SOURCES.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)        1 2024-05-29 14:31:02.000000 tromero_tailor-0.0.19/tromero_tailor.egg-info/dependency_links.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      304 2024-05-29 14:31:02.000000 tromero_tailor-0.0.19/tromero_tailor.egg-info/requires.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       15 2024-05-29 14:31:02.000000 tromero_tailor-0.0.19/tromero_tailor.egg-info/top_level.txt
```

### Comparing `tromero_tailor-0.0.18/PKG-INFO` & `tromero_tailor-0.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tromero_tailor
-Version: 0.0.18
+Version: 0.0.19
 Summary: A short description of your package
 Home-page: http://yourpackagehomepage.com
 Author: Tromero
 Author-email: tadhg.amin@tromero.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tromero_tailor-0.0.18/README.md` & `tromero_tailor-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.18/setup.py` & `tromero_tailor-0.0.19/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tromero_tailor",  # Replace with your package name
-    version="0.0.18",  # Replace with your package's version
+    version="0.0.19",  # Replace with your package's version
     author="Tromero",  # Replace with your name
     author_email="tadhg.amin@tromero.ai",  # Replace with your email address
     description="A short description of your package",  # Provide a short description
     long_description=open('README.md').read(),  # This will read your long description from README.md
     long_description_content_type='text/markdown',  # Indicates that the long description is in Markdown
     url="http://yourpackagehomepage.com",  # Replace with the URL to your package's homepage
     license="MIT",  # Replace with your chosen license
```

### Comparing `tromero_tailor-0.0.18/tests/test.py` & `tromero_tailor-0.0.19/tests/test.py`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.18/tromero_tailor/tromero_requests.py` & `tromero_tailor-0.0.19/tromero_tailor/tromero_requests.py`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.18/tromero_tailor.egg-info/PKG-INFO` & `tromero_tailor-0.0.19/tromero_tailor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tromero_tailor
-Version: 0.0.18
+Version: 0.0.19
 Summary: A short description of your package
 Home-page: http://yourpackagehomepage.com
 Author: Tromero
 Author-email: tadhg.amin@tromero.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

