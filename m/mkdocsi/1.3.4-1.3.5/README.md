# Comparing `tmp/mkdocsi-1.3.4.tar.gz` & `tmp/mkdocsi-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.3.4.tar", last modified: Wed May 29 09:45:26 2024, max compression
+gzip compressed data, was "mkdocsi-1.3.5.tar", last modified: Wed May 29 09:52:00 2024, max compression
```

## Comparing `mkdocsi-1.3.4.tar` & `mkdocsi-1.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:45:26.173071 mkdocsi-1.3.4/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 09:45:26.173071 mkdocsi-1.3.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-29 09:45:16.000000 mkdocsi-1.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:45:26.171071 mkdocsi-1.3.4/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)     1060 2024-05-29 09:45:16.000000 mkdocsi-1.3.4/mkdocsi/ __main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-29 09:45:16.000000 mkdocsi-1.3.4/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-29 09:45:16.000000 mkdocsi-1.3.4/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:45:26.172071 mkdocsi-1.3.4/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 09:45:26.000000 mkdocsi-1.3.4/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      263 2024-05-29 09:45:26.000000 mkdocsi-1.3.4/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 09:45:26.000000 mkdocsi-1.3.4/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-05-29 09:45:26.000000 mkdocsi-1.3.4/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 09:45:26.000000 mkdocsi-1.3.4/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 09:45:26.000000 mkdocsi-1.3.4/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 09:45:26.173071 mkdocsi-1.3.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3046 2024-05-29 09:45:16.000000 mkdocsi-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:52:00.822642 mkdocsi-1.3.5/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 09:52:00.822642 mkdocsi-1.3.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-29 09:51:51.000000 mkdocsi-1.3.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:52:00.820642 mkdocsi-1.3.5/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-29 09:51:51.000000 mkdocsi-1.3.5/mkdocsi/ __main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-29 09:51:51.000000 mkdocsi-1.3.5/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-29 09:51:51.000000 mkdocsi-1.3.5/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:52:00.822642 mkdocsi-1.3.5/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 09:52:00.000000 mkdocsi-1.3.5/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      263 2024-05-29 09:52:00.000000 mkdocsi-1.3.5/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 09:52:00.000000 mkdocsi-1.3.5/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-29 09:52:00.000000 mkdocsi-1.3.5/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 09:52:00.000000 mkdocsi-1.3.5/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 09:52:00.000000 mkdocsi-1.3.5/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 09:52:00.822642 mkdocsi-1.3.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2024-05-29 09:51:51.000000 mkdocsi-1.3.5/setup.py
```

### Comparing `mkdocsi-1.3.4/PKG-INFO` & `mkdocsi-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.3.4
+Version: 1.3.5
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.3.4/README.md` & `mkdocsi-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.3.4/mkdocsi/ __main__.py` & `mkdocsi-1.3.5/mkdocsi/Main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
         with open(args.index,"r") as buff : 
             print(buff.read() , file = open(os.path.join(args.docs ,"index.md"),"w"))
 
     _MkdocsUtils = mkdocsi.MkdocsUtils(docs_folder = args.docs  , Template_mkdocs = Template_mkdocs  ,site_name = args.site_name 
     _MkdocsUtils.buildTree()
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `mkdocsi-1.3.4/mkdocsi/Main.py` & `mkdocsi-1.3.5/mkdocsi/ __main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,9 +21,7 @@
     if args.index is not None  : 
         with open(args.index,"r") as buff : 
             print(buff.read() , file = open(os.path.join(args.docs ,"index.md"),"w"))
 
     _MkdocsUtils = mkdocsi.MkdocsUtils(docs_folder = args.docs  , Template_mkdocs = Template_mkdocs  ,site_name = args.site_name 
     _MkdocsUtils.buildTree()
 
-if __name__ == "__main__":
-    main()
```

### Comparing `mkdocsi-1.3.4/mkdocsi/__init__.py` & `mkdocsi-1.3.5/mkdocsi/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.3.4/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.3.5/mkdocsi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.3.4
+Version: 1.3.5
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.3.4/setup.py` & `mkdocsi-1.3.5/setup.py`

 * *Files identical despite different names*

