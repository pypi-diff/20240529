# Comparing `tmp/dtfilterthumbor-0.5.0.tar.gz` & `tmp/dtfilterthumbor-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfilterthumbor-0.5.0.tar", last modified: Thu Aug 18 11:31:24 2022, max compression
+gzip compressed data, was "dtfilterthumbor-1.0.0.tar", last modified: Wed May 29 04:26:05 2024, max compression
```

## Comparing `dtfilterthumbor-0.5.0.tar` & `dtfilterthumbor-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 11:31:24.296930 dtfilterthumbor-0.5.0/
--rw-r--r--   0 root         (0) root         (0)     1123 2022-08-18 11:31:24.295930 dtfilterthumbor-0.5.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      333 2022-08-18 10:54:04.000000 dtfilterthumbor-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 11:31:24.291930 dtfilterthumbor-0.5.0/dtfilterthumbor/
--rw-rw-r--   0 root         (0) root         (0)      270 2022-08-18 10:54:04.000000 dtfilterthumbor-0.5.0/dtfilterthumbor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7395 2022-08-18 10:54:04.000000 dtfilterthumbor-0.5.0/dtfilterthumbor/dtwatermark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 11:31:24.294930 dtfilterthumbor-0.5.0/dtfilterthumbor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1123 2022-08-18 11:31:24.000000 dtfilterthumbor-0.5.0/dtfilterthumbor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      233 2022-08-18 11:31:24.000000 dtfilterthumbor-0.5.0/dtfilterthumbor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-18 11:31:24.000000 dtfilterthumbor-0.5.0/dtfilterthumbor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-08-18 11:31:24.000000 dtfilterthumbor-0.5.0/dtfilterthumbor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-18 11:31:24.297930 dtfilterthumbor-0.5.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1289 2022-08-18 11:15:27.000000 dtfilterthumbor-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 04:26:05.810181 dtfilterthumbor-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-05-29 04:26:05.810181 dtfilterthumbor-1.0.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      333 2024-05-29 04:25:26.000000 dtfilterthumbor-1.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 04:26:05.809181 dtfilterthumbor-1.0.0/dtfilterthumbor/
+-rw-rw-r--   0 root         (0) root         (0)      322 2024-05-29 04:25:26.000000 dtfilterthumbor-1.0.0/dtfilterthumbor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7395 2024-05-29 04:25:26.000000 dtfilterthumbor-1.0.0/dtfilterthumbor/dtwatermark.py
+-rw-rw-r--   0 root         (0) root         (0)     7416 2024-05-29 04:25:26.000000 dtfilterthumbor-1.0.0/dtfilterthumbor/dtwatermark2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 04:26:05.810181 dtfilterthumbor-1.0.0/dtfilterthumbor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-05-29 04:26:05.000000 dtfilterthumbor-1.0.0/dtfilterthumbor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      265 2024-05-29 04:26:05.000000 dtfilterthumbor-1.0.0/dtfilterthumbor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 04:26:05.000000 dtfilterthumbor-1.0.0/dtfilterthumbor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-29 04:26:05.000000 dtfilterthumbor-1.0.0/dtfilterthumbor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 04:26:05.810181 dtfilterthumbor-1.0.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1289 2024-05-29 04:25:26.000000 dtfilterthumbor-1.0.0/setup.py
```

### Comparing `dtfilterthumbor-0.5.0/PKG-INFO` & `dtfilterthumbor-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfilterthumbor
-Version: 0.5.0
+Version: 1.0.0
 Summary: dan tri filter
 Home-page: https://medium-multiply.readthedocs.io/
 Author: xuantrangk54
 Author-email: xuantrangk54@gmail.com
 License: MIT
 Description: # DantriFilter docs
```

### Comparing `dtfilterthumbor-0.5.0/dtfilterthumbor/dtwatermark.py` & `dtfilterthumbor-1.0.0/dtfilterthumbor/dtwatermark.py`

 * *Files identical despite different names*

### Comparing `dtfilterthumbor-0.5.0/dtfilterthumbor.egg-info/PKG-INFO` & `dtfilterthumbor-1.0.0/dtfilterthumbor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfilterthumbor
-Version: 0.5.0
+Version: 1.0.0
 Summary: dan tri filter
 Home-page: https://medium-multiply.readthedocs.io/
 Author: xuantrangk54
 Author-email: xuantrangk54@gmail.com
 License: MIT
 Description: # DantriFilter docs
```

### Comparing `dtfilterthumbor-0.5.0/setup.py` & `dtfilterthumbor-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="dtfilterthumbor",
-    version="0.5.0",
+    version="1.0.0",
     description="dan tri filter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://medium-multiply.readthedocs.io/",
     author="xuantrangk54",
     author_email="xuantrangk54@gmail.com",
     license="MIT",
```

