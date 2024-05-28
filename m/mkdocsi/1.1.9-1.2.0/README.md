# Comparing `tmp/mkdocsi-1.1.9.tar.gz` & `tmp/mkdocsi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.1.9.tar", last modified: Tue May 28 22:24:13 2024, max compression
+gzip compressed data, was "mkdocsi-1.2.0.tar", last modified: Tue May 28 22:27:51 2024, max compression
```

## Comparing `mkdocsi-1.1.9.tar` & `mkdocsi-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:24:13.504952 mkdocsi-1.1.9/
--rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:24:13.504952 mkdocsi-1.1.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-28 22:24:04.000000 mkdocsi-1.1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:24:13.502952 mkdocsi-1.1.9/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-28 22:24:04.000000 mkdocsi-1.1.9/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     6602 2024-05-28 22:24:04.000000 mkdocsi-1.1.9/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:24:13.503952 mkdocsi-1.1.9/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:24:13.000000 mkdocsi-1.1.9/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 22:24:13.000000 mkdocsi-1.1.9/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 22:24:13.000000 mkdocsi-1.1.9/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 22:24:13.000000 mkdocsi-1.1.9/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 22:24:13.000000 mkdocsi-1.1.9/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 22:24:13.000000 mkdocsi-1.1.9/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 22:24:13.504952 mkdocsi-1.1.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 22:24:04.000000 mkdocsi-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:27:51.013217 mkdocsi-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:27:51.013217 mkdocsi-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-28 22:27:41.000000 mkdocsi-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:27:51.011217 mkdocsi-1.2.0/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-28 22:27:41.000000 mkdocsi-1.2.0/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6607 2024-05-28 22:27:41.000000 mkdocsi-1.2.0/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:27:51.012217 mkdocsi-1.2.0/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:27:50.000000 mkdocsi-1.2.0/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 22:27:50.000000 mkdocsi-1.2.0/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 22:27:50.000000 mkdocsi-1.2.0/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 22:27:50.000000 mkdocsi-1.2.0/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 22:27:50.000000 mkdocsi-1.2.0/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 22:27:50.000000 mkdocsi-1.2.0/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 22:27:51.013217 mkdocsi-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 22:27:41.000000 mkdocsi-1.2.0/setup.py
```

### Comparing `mkdocsi-1.1.9/PKG-INFO` & `mkdocsi-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.1.9
+Version: 1.2.0
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.1.9/mkdocsi/__init__.py` & `mkdocsi-1.2.0/mkdocsi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
       icon: material/brightness-4
       name: Switch to light mode
 
 """
 
 class MkdocsUtils : 
     def __init__(self , docs_folder  ,  Template_mkdocs   = None , site_name = None ) : 
-        self.site_name = name 
+        self.site_name = site_name 
         if Template_mkdocs is not None : 
             self.Template_mkdocs = Template_mkdocs 
         else  : 
             self.Template_mkdocs = DEFAULT_MKDOCS 
         self.docs_folder = os.path.abspath(docs_folder)  
         self.new_mkdocsfile = os.path.join(self.docs_folder ,"..", "mkdocs.yml")
         self.mkdocs_data = yaml.safe_load(self.Template_mkdocs)
```

### Comparing `mkdocsi-1.1.9/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.2.0/mkdocsi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.1.9
+Version: 1.2.0
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.1.9/setup.py` & `mkdocsi-1.2.0/setup.py`

 * *Files identical despite different names*

