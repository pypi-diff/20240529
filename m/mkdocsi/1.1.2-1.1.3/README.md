# Comparing `tmp/mkdocsi-1.1.2.tar.gz` & `tmp/mkdocsi-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.1.2.tar", last modified: Tue May 28 21:54:14 2024, max compression
+gzip compressed data, was "mkdocsi-1.1.3.tar", last modified: Tue May 28 22:00:17 2024, max compression
```

## Comparing `mkdocsi-1.1.2.tar` & `mkdocsi-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:54:14.331757 mkdocsi-1.1.2/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 21:54:14.330757 mkdocsi-1.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 21:54:04.000000 mkdocsi-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:54:14.328757 mkdocsi-1.1.2/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 21:54:04.000000 mkdocsi-1.1.2/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     6275 2024-05-28 21:54:04.000000 mkdocsi-1.1.2/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:54:14.330757 mkdocsi-1.1.2/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 21:54:14.000000 mkdocsi-1.1.2/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 21:54:14.000000 mkdocsi-1.1.2/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 21:54:14.000000 mkdocsi-1.1.2/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 21:54:14.000000 mkdocsi-1.1.2/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 21:54:14.000000 mkdocsi-1.1.2/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 21:54:14.000000 mkdocsi-1.1.2/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 21:54:14.331757 mkdocsi-1.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 21:54:04.000000 mkdocsi-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:00:17.595046 mkdocsi-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 22:00:17.594046 mkdocsi-1.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 22:00:08.000000 mkdocsi-1.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:00:17.592046 mkdocsi-1.1.3/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 22:00:08.000000 mkdocsi-1.1.3/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6275 2024-05-28 22:00:08.000000 mkdocsi-1.1.3/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:00:17.594046 mkdocsi-1.1.3/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 22:00:17.000000 mkdocsi-1.1.3/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 22:00:17.000000 mkdocsi-1.1.3/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 22:00:17.000000 mkdocsi-1.1.3/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 22:00:17.000000 mkdocsi-1.1.3/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 22:00:17.000000 mkdocsi-1.1.3/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 22:00:17.000000 mkdocsi-1.1.3/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 22:00:17.595046 mkdocsi-1.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 22:00:08.000000 mkdocsi-1.1.3/setup.py
```

### Comparing `mkdocsi-1.1.2/PKG-INFO` & `mkdocsi-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.1.2
+Version: 1.1.3
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.1.2/mkdocsi/__init__.py` & `mkdocsi-1.1.3/mkdocsi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self.docs_folder = os.path.abspath(docs_folder)  
         self.new_mkdocsfile = os.path.join(self.docs_folder ,"..", "mkdocs.yml")
         self.mkdocs_data = yaml.safe_load(self.Template_mkdocs)
         if not ('nav' in self.mkdocs_data.keys()) : self.mkdocs_data['nav'] = list()
 
     def make_safe(self) : 
         Tags_md = os.path.join(self.docs_folder , "Tags.md")
-        if not os.path.isfile(Tags_md) : 
+        if not os.path.exists(Tags_md) : 
             print("<!-- material/tags { scope: true } -->" , file = open(Tags_md , "w"))
 
 
     def __repr__(self) : 
         return json.dumps(self.mkdocs_data , indent = 4 )
 
     def buildTree(self) :
```

### Comparing `mkdocsi-1.1.2/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.1.3/mkdocsi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.1.2
+Version: 1.1.3
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.1.2/setup.py` & `mkdocsi-1.1.3/setup.py`

 * *Files identical despite different names*

