# Comparing `tmp/mkdocsi-1.1.7.tar.gz` & `tmp/mkdocsi-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.1.7.tar", last modified: Tue May 28 22:13:01 2024, max compression
+gzip compressed data, was "mkdocsi-1.1.8.tar", last modified: Tue May 28 22:14:30 2024, max compression
```

## Comparing `mkdocsi-1.1.7.tar` & `mkdocsi-1.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:13:01.241742 mkdocsi-1.1.7/
--rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:13:01.241742 mkdocsi-1.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-28 22:12:51.000000 mkdocsi-1.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:13:01.239742 mkdocsi-1.1.7/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 22:12:51.000000 mkdocsi-1.1.7/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     6256 2024-05-28 22:12:51.000000 mkdocsi-1.1.7/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:13:01.240742 mkdocsi-1.1.7/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:13:01.000000 mkdocsi-1.1.7/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 22:13:01.000000 mkdocsi-1.1.7/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 22:13:01.000000 mkdocsi-1.1.7/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 22:13:01.000000 mkdocsi-1.1.7/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 22:13:01.000000 mkdocsi-1.1.7/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 22:13:01.000000 mkdocsi-1.1.7/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 22:13:01.241742 mkdocsi-1.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 22:12:51.000000 mkdocsi-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:14:30.795986 mkdocsi-1.1.8/
+-rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:14:30.795986 mkdocsi-1.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-28 22:14:20.000000 mkdocsi-1.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:14:30.793986 mkdocsi-1.1.8/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 22:14:20.000000 mkdocsi-1.1.8/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6321 2024-05-28 22:14:20.000000 mkdocsi-1.1.8/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:14:30.794986 mkdocsi-1.1.8/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:14:30.000000 mkdocsi-1.1.8/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 22:14:30.000000 mkdocsi-1.1.8/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 22:14:30.000000 mkdocsi-1.1.8/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 22:14:30.000000 mkdocsi-1.1.8/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 22:14:30.000000 mkdocsi-1.1.8/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 22:14:30.000000 mkdocsi-1.1.8/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 22:14:30.795986 mkdocsi-1.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 22:14:20.000000 mkdocsi-1.1.8/setup.py
```

### Comparing `mkdocsi-1.1.7/PKG-INFO` & `mkdocsi-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.1.7
+Version: 1.1.8
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.1.7/mkdocsi/__init__.py` & `mkdocsi-1.1.8/mkdocsi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 
 
     def make_safe(self) : 
         Tags_md = os.path.join(self.docs_folder , "Tags.md")
         if not os.path.exists(Tags_md) : 
             print("<!-- material/tags { scope: true } -->" , file = open(Tags_md , "w"))
+            self.mkdocs_data['nav'].append({"Tags" : "Tags.md"})
 
 
     def __repr__(self) : 
         return json.dumps(self.mkdocs_data , indent = 4 )
 
     def buildTree(self) : 
         self.make_safe()
```

### Comparing `mkdocsi-1.1.7/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.1.8/mkdocsi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.1.7
+Version: 1.1.8
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.1.7/setup.py` & `mkdocsi-1.1.8/setup.py`

 * *Files identical despite different names*

