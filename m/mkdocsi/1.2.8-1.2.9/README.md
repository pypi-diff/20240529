# Comparing `tmp/mkdocsi-1.2.8.tar.gz` & `tmp/mkdocsi-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.2.8.tar", last modified: Wed May 29 08:44:31 2024, max compression
+gzip compressed data, was "mkdocsi-1.2.9.tar", last modified: Wed May 29 08:46:05 2024, max compression
```

## Comparing `mkdocsi-1.2.8.tar` & `mkdocsi-1.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:44:31.748996 mkdocsi-1.2.8/
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-29 08:44:31.747996 mkdocsi-1.2.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-29 08:44:22.000000 mkdocsi-1.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:44:31.746996 mkdocsi-1.2.8/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-29 08:44:22.000000 mkdocsi-1.2.8/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-29 08:44:22.000000 mkdocsi-1.2.8/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:44:31.747996 mkdocsi-1.2.8/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-29 08:44:31.000000 mkdocsi-1.2.8/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-29 08:44:31.000000 mkdocsi-1.2.8/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 08:44:31.000000 mkdocsi-1.2.8/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-29 08:44:31.000000 mkdocsi-1.2.8/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 08:44:31.000000 mkdocsi-1.2.8/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 08:44:31.000000 mkdocsi-1.2.8/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 08:44:31.748996 mkdocsi-1.2.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-29 08:44:22.000000 mkdocsi-1.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:46:05.591750 mkdocsi-1.2.9/
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-29 08:46:05.591750 mkdocsi-1.2.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-29 08:45:56.000000 mkdocsi-1.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:46:05.589750 mkdocsi-1.2.9/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-29 08:45:56.000000 mkdocsi-1.2.9/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-29 08:45:56.000000 mkdocsi-1.2.9/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:46:05.591750 mkdocsi-1.2.9/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-29 08:46:05.000000 mkdocsi-1.2.9/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-29 08:46:05.000000 mkdocsi-1.2.9/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 08:46:05.000000 mkdocsi-1.2.9/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-29 08:46:05.000000 mkdocsi-1.2.9/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 08:46:05.000000 mkdocsi-1.2.9/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 08:46:05.000000 mkdocsi-1.2.9/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 08:46:05.591750 mkdocsi-1.2.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-29 08:45:56.000000 mkdocsi-1.2.9/setup.py
```

### Comparing `mkdocsi-1.2.8/PKG-INFO` & `mkdocsi-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.2.8
+Version: 1.2.9
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.2.8/mkdocsi/Main.py` & `mkdocsi-1.2.9/mkdocsi/Main.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,13 +18,13 @@
         with open(args.mkdocs) as buff  : 
             Template_mkdocs = buff.read()
 
     if args.index is not None  : 
         with open(args.index,"r") as buff : 
             print(buff.read() , file = open(os.path.join(args.docs ,"index.md"),"w"))
 
-    _MkdocsUtils = MkdocsUtils(docs_folder = args.docs  , Template_mkdocs = Template_mkdocs  ,site_name = site_name  )
+    _MkdocsUtils = mkdocsi.MkdocsUtils(docs_folder = args.docs  , Template_mkdocs = Template_mkdocs  ,site_name = site_name  )
 
     _MkdocsUtils.buildTree()
 
 if __name__ == "__main__":
     main()
```

### Comparing `mkdocsi-1.2.8/mkdocsi/__init__.py` & `mkdocsi-1.2.9/mkdocsi/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.2.8/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.2.9/mkdocsi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.2.8
+Version: 1.2.9
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.2.8/setup.py` & `mkdocsi-1.2.9/setup.py`

 * *Files identical despite different names*

