# Comparing `tmp/mkdocsi-1.3.6.tar.gz` & `tmp/mkdocsi-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.3.6.tar", last modified: Wed May 29 10:00:02 2024, max compression
+gzip compressed data, was "mkdocsi-1.3.7.tar", last modified: Wed May 29 10:01:57 2024, max compression
```

## Comparing `mkdocsi-1.3.6.tar` & `mkdocsi-1.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:00:02.354066 mkdocsi-1.3.6/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:00:02.354066 mkdocsi-1.3.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-29 09:59:52.000000 mkdocsi-1.3.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:00:02.352066 mkdocsi-1.3.6/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)     7332 2024-05-29 09:59:52.000000 mkdocsi-1.3.6/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:00:02.354066 mkdocsi-1.3.6/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:00:02.000000 mkdocsi-1.3.6/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      226 2024-05-29 10:00:02.000000 mkdocsi-1.3.6/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 10:00:02.000000 mkdocsi-1.3.6/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-29 10:00:02.000000 mkdocsi-1.3.6/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 10:00:02.000000 mkdocsi-1.3.6/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 10:00:02.000000 mkdocsi-1.3.6/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 10:00:02.354066 mkdocsi-1.3.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3047 2024-05-29 09:59:52.000000 mkdocsi-1.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:01:57.397129 mkdocsi-1.3.7/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:01:57.397129 mkdocsi-1.3.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-29 10:01:47.000000 mkdocsi-1.3.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:01:57.395129 mkdocsi-1.3.7/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)     7332 2024-05-29 10:01:47.000000 mkdocsi-1.3.7/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:01:57.396129 mkdocsi-1.3.7/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:01:57.000000 mkdocsi-1.3.7/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      226 2024-05-29 10:01:57.000000 mkdocsi-1.3.7/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 10:01:57.000000 mkdocsi-1.3.7/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-29 10:01:57.000000 mkdocsi-1.3.7/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 10:01:57.000000 mkdocsi-1.3.7/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 10:01:57.000000 mkdocsi-1.3.7/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 10:01:57.397129 mkdocsi-1.3.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2024-05-29 10:01:47.000000 mkdocsi-1.3.7/setup.py
```

### Comparing `mkdocsi-1.3.6/PKG-INFO` & `mkdocsi-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.3.6
+Version: 1.3.7
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.3.6/README.md` & `mkdocsi-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.3.6/mkdocsi/__init__.py` & `mkdocsi-1.3.7/mkdocsi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,9 +120,9 @@
         with open(args.mkdocs) as buff  : 
             Template_mkdocs = buff.read()
 
     if args.index is not None  : 
         with open(args.index,"r") as buff : 
             print(buff.read() , file = open(os.path.join(args.docs ,"index.md"),"w"))
 
-    _MkdocsUtils = MkdocsUtils(docs_folder = args.docs  , Template_mkdocs = Template_mkdocs  ,site_name = args.site_name 
+    _MkdocsUtils = MkdocsUtils(docs_folder = args.docs  , Template_mkdocs = Template_mkdocs  ,site_name = args.site_name)
     _MkdocsUtils.buildTree()
```

### Comparing `mkdocsi-1.3.6/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.3.7/mkdocsi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.3.6
+Version: 1.3.7
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.3.6/setup.py` & `mkdocsi-1.3.7/setup.py`

 * *Files identical despite different names*

