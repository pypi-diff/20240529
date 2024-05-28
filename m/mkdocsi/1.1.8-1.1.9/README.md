# Comparing `tmp/mkdocsi-1.1.8.tar.gz` & `tmp/mkdocsi-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.1.8.tar", last modified: Tue May 28 22:14:30 2024, max compression
+gzip compressed data, was "mkdocsi-1.1.9.tar", last modified: Tue May 28 22:24:13 2024, max compression
```

## Comparing `mkdocsi-1.1.8.tar` & `mkdocsi-1.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:14:30.795986 mkdocsi-1.1.8/
--rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:14:30.795986 mkdocsi-1.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-28 22:14:20.000000 mkdocsi-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:14:30.793986 mkdocsi-1.1.8/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 22:14:20.000000 mkdocsi-1.1.8/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     6321 2024-05-28 22:14:20.000000 mkdocsi-1.1.8/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:14:30.794986 mkdocsi-1.1.8/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:14:30.000000 mkdocsi-1.1.8/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 22:14:30.000000 mkdocsi-1.1.8/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 22:14:30.000000 mkdocsi-1.1.8/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 22:14:30.000000 mkdocsi-1.1.8/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 22:14:30.000000 mkdocsi-1.1.8/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 22:14:30.000000 mkdocsi-1.1.8/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 22:14:30.795986 mkdocsi-1.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 22:14:20.000000 mkdocsi-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:24:13.504952 mkdocsi-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:24:13.504952 mkdocsi-1.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-28 22:24:04.000000 mkdocsi-1.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:24:13.502952 mkdocsi-1.1.9/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-28 22:24:04.000000 mkdocsi-1.1.9/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6602 2024-05-28 22:24:04.000000 mkdocsi-1.1.9/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:24:13.503952 mkdocsi-1.1.9/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:24:13.000000 mkdocsi-1.1.9/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 22:24:13.000000 mkdocsi-1.1.9/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 22:24:13.000000 mkdocsi-1.1.9/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 22:24:13.000000 mkdocsi-1.1.9/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 22:24:13.000000 mkdocsi-1.1.9/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 22:24:13.000000 mkdocsi-1.1.9/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 22:24:13.504952 mkdocsi-1.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 22:24:04.000000 mkdocsi-1.1.9/setup.py
```

### Comparing `mkdocsi-1.1.8/PKG-INFO` & `mkdocsi-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.1.8
+Version: 1.1.9
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.1.8/mkdocsi/__init__.py` & `mkdocsi-1.1.9/mkdocsi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     tags_file: Tags.md
     listings_sort_by: "!!python/name:material.plugins.tags.item_url"
 - search:
     pipeline:
     - stemmer
     - stopWordFilter
     - trimmer
-site_name: Issam MHADHBI
+site_name: Genrated Docs
 theme:
   features:
   - search.share
   - content.code.copy
   - content.code.select
   name: material
   palette:
@@ -40,27 +40,30 @@
     toggle:
       icon: material/brightness-4
       name: Switch to light mode
 
 """
 
 class MkdocsUtils : 
-    def __init__(self , docs_folder  ,  Template_mkdocs   = None ) : 
+    def __init__(self , docs_folder  ,  Template_mkdocs   = None , site_name = None ) : 
+        self.site_name = name 
         if Template_mkdocs is not None : 
             self.Template_mkdocs = Template_mkdocs 
         else  : 
             self.Template_mkdocs = DEFAULT_MKDOCS 
         self.docs_folder = os.path.abspath(docs_folder)  
         self.new_mkdocsfile = os.path.join(self.docs_folder ,"..", "mkdocs.yml")
         self.mkdocs_data = yaml.safe_load(self.Template_mkdocs)
         if not ('nav' in self.mkdocs_data.keys()) : self.mkdocs_data['nav'] = list()
 
 
 
     def make_safe(self) : 
+        if self.site_name is not None  : 
+            self.mkdocs_data['site_name'] = self.site_name 
         Tags_md = os.path.join(self.docs_folder , "Tags.md")
         if not os.path.exists(Tags_md) : 
             print("<!-- material/tags { scope: true } -->" , file = open(Tags_md , "w"))
             self.mkdocs_data['nav'].append({"Tags" : "Tags.md"})
 
 
     def __repr__(self) : 
@@ -92,10 +95,10 @@
                     camel_case_name = self.to_camel_case(base_name)                                                                                                                                     
                     tree.append({camel_case_name: relative_path})                                                                                                                                  
             return tree                                                                                                                                                                            
                                                                                                                                                                                                 
         return walk_dir(self.docs_folder)    
 
 
-def generate_site(docs_folder, Template_mkdocs_file   = None ) : 
-    _MkdocsUtils = MkdocsUtils(docs_folder, Template_mkdocs_file)
+def generate_site(docs_folder = os.path.join(os.getcwd() , "docs"), Template_mkdocs   = None , site_name = os.path.dirname(os.getcwd()) ) : 
+    _MkdocsUtils = MkdocsUtils(docs_folder = docs_folder , Template_mkdocs = Template_mkdocs  ,site_name = site_name  )
     _MkdocsUtils.buildTree()
```

### Comparing `mkdocsi-1.1.8/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.1.9/mkdocsi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.1.8
+Version: 1.1.9
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.1.8/setup.py` & `mkdocsi-1.1.9/setup.py`

 * *Files identical despite different names*

