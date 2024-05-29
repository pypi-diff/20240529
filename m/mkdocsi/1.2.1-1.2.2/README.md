# Comparing `tmp/mkdocsi-1.2.1.tar.gz` & `tmp/mkdocsi-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.2.1.tar", last modified: Tue May 28 22:31:29 2024, max compression
+gzip compressed data, was "mkdocsi-1.2.2.tar", last modified: Wed May 29 08:23:21 2024, max compression
```

## Comparing `mkdocsi-1.2.1.tar` & `mkdocsi-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:31:29.902556 mkdocsi-1.2.1/
--rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:31:29.902556 mkdocsi-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-28 22:31:20.000000 mkdocsi-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:31:29.900556 mkdocsi-1.2.1/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)      338 2024-05-28 22:31:20.000000 mkdocsi-1.2.1/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     6639 2024-05-28 22:31:20.000000 mkdocsi-1.2.1/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:31:29.901556 mkdocsi-1.2.1/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      577 2024-05-28 22:31:29.000000 mkdocsi-1.2.1/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 22:31:29.000000 mkdocsi-1.2.1/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 22:31:29.000000 mkdocsi-1.2.1/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 22:31:29.000000 mkdocsi-1.2.1/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 22:31:29.000000 mkdocsi-1.2.1/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 22:31:29.000000 mkdocsi-1.2.1/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 22:31:29.902556 mkdocsi-1.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 22:31:20.000000 mkdocsi-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:23:21.488118 mkdocsi-1.2.2/
+-rw-r--r--   0 root         (0) root         (0)      577 2024-05-29 08:23:21.488118 mkdocsi-1.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-29 08:23:11.000000 mkdocsi-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:23:21.486118 mkdocsi-1.2.2/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2024-05-29 08:23:11.000000 mkdocsi-1.2.2/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-29 08:23:11.000000 mkdocsi-1.2.2/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:23:21.487118 mkdocsi-1.2.2/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      577 2024-05-29 08:23:21.000000 mkdocsi-1.2.2/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-29 08:23:21.000000 mkdocsi-1.2.2/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 08:23:21.000000 mkdocsi-1.2.2/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-29 08:23:21.000000 mkdocsi-1.2.2/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 08:23:21.000000 mkdocsi-1.2.2/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 08:23:21.000000 mkdocsi-1.2.2/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 08:23:21.488118 mkdocsi-1.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-29 08:23:11.000000 mkdocsi-1.2.2/setup.py
```

### Comparing `mkdocsi-1.2.1/PKG-INFO` & `mkdocsi-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.2.1
+Version: 1.2.2
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.2.1/mkdocsi/__init__.py` & `mkdocsi-1.2.2/mkdocsi/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,13 +93,9 @@
                         tree.append({item: subtree})                                                                                                                                               
                 elif item.endswith('.md'):                                                                                                                                                         
                     base_name = os.path.splitext(item)[0]                                                                                                                                          
                     camel_case_name = self.to_camel_case(base_name)                                                                                                                                     
                     tree.append({camel_case_name: relative_path})                                                                                                                                  
             return tree                                                                                                                                                                            
                                                                                                                                                                                                 
-        return walk_dir(self.docs_folder)    
+        return walk_dir(self.docs_folder)   
 
-
-def generate_site(docs_folder = os.path.join(os.getcwd() , "docs"), Template_mkdocs   = None , site_name = os.path.dirname(os.getcwd()) ) : 
-    _MkdocsUtils = MkdocsUtils(docs_folder = docs_folder , Template_mkdocs = Template_mkdocs  ,site_name = site_name  )
-    _MkdocsUtils.buildTree()
```

### Comparing `mkdocsi-1.2.1/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.2.2/mkdocsi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.2.1
+Version: 1.2.2
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.2.1/setup.py` & `mkdocsi-1.2.2/setup.py`

 * *Files identical despite different names*

