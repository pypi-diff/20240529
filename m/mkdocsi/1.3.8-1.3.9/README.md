# Comparing `tmp/mkdocsi-1.3.8.tar.gz` & `tmp/mkdocsi-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.3.8.tar", last modified: Wed May 29 10:03:44 2024, max compression
+gzip compressed data, was "mkdocsi-1.3.9.tar", last modified: Wed May 29 10:19:09 2024, max compression
```

## Comparing `mkdocsi-1.3.8.tar` & `mkdocsi-1.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:03:44.223803 mkdocsi-1.3.8/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:03:44.223803 mkdocsi-1.3.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-29 10:03:34.000000 mkdocsi-1.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:03:44.221803 mkdocsi-1.3.8/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)     7334 2024-05-29 10:03:34.000000 mkdocsi-1.3.8/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:03:44.223803 mkdocsi-1.3.8/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:03:44.000000 mkdocsi-1.3.8/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      226 2024-05-29 10:03:44.000000 mkdocsi-1.3.8/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 10:03:44.000000 mkdocsi-1.3.8/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-05-29 10:03:44.000000 mkdocsi-1.3.8/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 10:03:44.000000 mkdocsi-1.3.8/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 10:03:44.000000 mkdocsi-1.3.8/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 10:03:44.223803 mkdocsi-1.3.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3049 2024-05-29 10:03:34.000000 mkdocsi-1.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:19:09.436380 mkdocsi-1.3.9/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:19:09.436380 mkdocsi-1.3.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-29 10:18:59.000000 mkdocsi-1.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:19:09.434379 mkdocsi-1.3.9/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)     7687 2024-05-29 10:18:59.000000 mkdocsi-1.3.9/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:19:09.436380 mkdocsi-1.3.9/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:19:09.000000 mkdocsi-1.3.9/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      226 2024-05-29 10:19:09.000000 mkdocsi-1.3.9/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 10:19:09.000000 mkdocsi-1.3.9/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-05-29 10:19:09.000000 mkdocsi-1.3.9/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 10:19:09.000000 mkdocsi-1.3.9/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 10:19:09.000000 mkdocsi-1.3.9/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 10:19:09.436380 mkdocsi-1.3.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2024-05-29 10:18:59.000000 mkdocsi-1.3.9/setup.py
```

### Comparing `mkdocsi-1.3.8/PKG-INFO` & `mkdocsi-1.3.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.3.8
+Version: 1.3.9
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.3.8/README.md` & `mkdocsi-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.3.8/mkdocsi/__init__.py` & `mkdocsi-1.3.9/mkdocsi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,21 +62,29 @@
         if self.site_name is not None  : 
             self.mkdocs_data['site_name'] = self.site_name 
         Tags_md = os.path.join(self.docs_folder , "Tags.md")
         if not os.path.exists(Tags_md) : 
             print("<!-- material/tags { scope: true } -->" , file = open(Tags_md , "w"))
             self.mkdocs_data['nav'].append({"Tags" : "Tags.md"})
 
+    def cleanNav(self , nav) : 
+        cleaned_nav = list() : 
+        set_keys = sorted({ k for i in nav for k , v in i.items() })
+        new_nav = { k : v for k , v in i for i in nav }
+        new_nav = [{ k : v } for k , v in new_nav.items()]
+        return new_nav
+        
 
     def __repr__(self) : 
         return json.dumps(self.mkdocs_data , indent = 4 )
 
     def buildTree(self) : 
         self.make_safe()
         self.mkdocs_data['nav'].extend(self.get_md_files_tree())
+        self.mkdocs_data['nav'] = self.cleanNav(self.mkdocs_data['nav'])
         with open(self.new_mkdocsfile, 'w') as file:                                                                                                                                                       
             yaml.dump(self.mkdocs_data, file, default_flow_style=False)       
                                                                                                                                                                                           
     def to_camel_case(self , snake_str):                                                                                                                                                                  
         components = snake_str.split('_')                                                                                                                                                     
         return " ".join(components)
```

### Comparing `mkdocsi-1.3.8/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.3.9/mkdocsi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.3.8
+Version: 1.3.9
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.3.8/setup.py` & `mkdocsi-1.3.9/setup.py`

 * *Files identical despite different names*

