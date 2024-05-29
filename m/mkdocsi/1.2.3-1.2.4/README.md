# Comparing `tmp/mkdocsi-1.2.3.tar.gz` & `tmp/mkdocsi-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.2.3.tar", last modified: Wed May 29 08:26:08 2024, max compression
+gzip compressed data, was "mkdocsi-1.2.4.tar", last modified: Wed May 29 08:26:54 2024, max compression
```

## Comparing `mkdocsi-1.2.3.tar` & `mkdocsi-1.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:26:08.302839 mkdocsi-1.2.3/
--rw-r--r--   0 root         (0) root         (0)      577 2024-05-29 08:26:08.302839 mkdocsi-1.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-29 08:25:58.000000 mkdocsi-1.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:26:08.300840 mkdocsi-1.2.3/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)     1234 2024-05-29 08:25:58.000000 mkdocsi-1.2.3/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-29 08:25:58.000000 mkdocsi-1.2.3/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:26:08.302839 mkdocsi-1.2.3/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      577 2024-05-29 08:26:08.000000 mkdocsi-1.2.3/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-29 08:26:08.000000 mkdocsi-1.2.3/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 08:26:08.000000 mkdocsi-1.2.3/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-29 08:26:08.000000 mkdocsi-1.2.3/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 08:26:08.000000 mkdocsi-1.2.3/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 08:26:08.000000 mkdocsi-1.2.3/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 08:26:08.302839 mkdocsi-1.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-29 08:25:58.000000 mkdocsi-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:26:54.988298 mkdocsi-1.2.4/
+-rw-r--r--   0 root         (0) root         (0)      577 2024-05-29 08:26:54.988298 mkdocsi-1.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-29 08:26:45.000000 mkdocsi-1.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:26:54.986298 mkdocsi-1.2.4/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2024-05-29 08:26:45.000000 mkdocsi-1.2.4/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-29 08:26:45.000000 mkdocsi-1.2.4/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:26:54.988298 mkdocsi-1.2.4/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      577 2024-05-29 08:26:54.000000 mkdocsi-1.2.4/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-29 08:26:54.000000 mkdocsi-1.2.4/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 08:26:54.000000 mkdocsi-1.2.4/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-29 08:26:54.000000 mkdocsi-1.2.4/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 08:26:54.000000 mkdocsi-1.2.4/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 08:26:54.000000 mkdocsi-1.2.4/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 08:26:54.988298 mkdocsi-1.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-29 08:26:45.000000 mkdocsi-1.2.4/setup.py
```

### Comparing `mkdocsi-1.2.3/PKG-INFO` & `mkdocsi-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.2.3
+Version: 1.2.4
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.2.3/mkdocsi/Main.py` & `mkdocsi-1.2.4/mkdocsi/Main.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Template_mkdocs = mkdocsi.DEFAULT_MKDOCS
     if args.mkdocs is None  : 
         with open(args.mkdocs) as buff  : 
             Template_mkdocs = buff.read()
 
     if args.index is not None  : 
         with open(args.index,"r") as buff : 
-            print(buff.read() , file = open(os.path.join(args.docs ,"index"),"w"))
+            print(buff.read() , file = open(os.path.join(args.docs ,"index.md"),"w"))
 
     _MkdocsUtils = MkdocsUtils(docs_folder = args.docs  , Template_mkdocs = Template_mkdocs  ,site_name = site_name  )
 
     _MkdocsUtils.buildTree()
 
 if __name__ == "__main__":
     main()
```

### Comparing `mkdocsi-1.2.3/mkdocsi/__init__.py` & `mkdocsi-1.2.4/mkdocsi/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.2.3/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.2.4/mkdocsi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.2.3
+Version: 1.2.4
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.2.3/setup.py` & `mkdocsi-1.2.4/setup.py`

 * *Files identical despite different names*

