# Comparing `tmp/mkdocsi-1.1.4.tar.gz` & `tmp/mkdocsi-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.1.4.tar", last modified: Tue May 28 22:04:19 2024, max compression
+gzip compressed data, was "mkdocsi-1.1.5.tar", last modified: Tue May 28 22:04:36 2024, max compression
```

## Comparing `mkdocsi-1.1.4.tar` & `mkdocsi-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:04:19.362017 mkdocsi-1.1.4/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 22:04:19.361017 mkdocsi-1.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 22:04:08.000000 mkdocsi-1.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:04:19.359017 mkdocsi-1.1.4/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 22:04:08.000000 mkdocsi-1.1.4/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     6417 2024-05-28 22:04:08.000000 mkdocsi-1.1.4/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:04:19.361017 mkdocsi-1.1.4/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 22:04:19.000000 mkdocsi-1.1.4/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 22:04:19.000000 mkdocsi-1.1.4/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 22:04:19.000000 mkdocsi-1.1.4/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 22:04:19.000000 mkdocsi-1.1.4/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 22:04:19.000000 mkdocsi-1.1.4/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 22:04:19.000000 mkdocsi-1.1.4/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 22:04:19.362017 mkdocsi-1.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 22:04:08.000000 mkdocsi-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:04:36.721873 mkdocsi-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 22:04:36.721873 mkdocsi-1.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 22:04:26.000000 mkdocsi-1.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:04:36.719873 mkdocsi-1.1.5/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 22:04:26.000000 mkdocsi-1.1.5/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6415 2024-05-28 22:04:26.000000 mkdocsi-1.1.5/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 22:04:36.720873 mkdocsi-1.1.5/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 22:04:36.000000 mkdocsi-1.1.5/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 22:04:36.000000 mkdocsi-1.1.5/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 22:04:36.000000 mkdocsi-1.1.5/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 22:04:36.000000 mkdocsi-1.1.5/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 22:04:36.000000 mkdocsi-1.1.5/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 22:04:36.000000 mkdocsi-1.1.5/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 22:04:36.721873 mkdocsi-1.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 22:04:26.000000 mkdocsi-1.1.5/setup.py
```

### Comparing `mkdocsi-1.1.4/PKG-INFO` & `mkdocsi-1.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.1.4
+Version: 1.1.5
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.1.4/mkdocsi/__init__.py` & `mkdocsi-1.1.5/mkdocsi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             self.Template_mkdocs = Template_mkdocs 
         else  : 
             self.Template_mkdocs = DEFAULT_MKDOCS 
         self.docs_folder = os.path.abspath(docs_folder)  
         self.new_mkdocsfile = os.path.join(self.docs_folder ,"..", "mkdocs.yml")
         self.mkdocs_data = yaml.safe_load(self.Template_mkdocs)
         if not ('nav' in self.mkdocs_data.keys()) : self.mkdocs_data['nav'] = [{"Tags" : "Tags.md"}]
-        if not any(('Tags' in i.keys())  for i in self.mkdocs_data['nav']  ]) : 
+        if not any(('Tags' in i.keys())  for i in self.mkdocs_data['nav'] ) : 
             self.mkdocs_data['nav'].append({"Tags" : "Tags.md"})
 
 
     def make_safe(self) : 
         Tags_md = os.path.join(self.docs_folder , "Tags.md")
         if not os.path.exists(Tags_md) : 
             print("<!-- material/tags { scope: true } -->" , file = open(Tags_md , "w"))
```

### Comparing `mkdocsi-1.1.4/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.1.5/mkdocsi.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.1.4
+Version: 1.1.5
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.1.4/setup.py` & `mkdocsi-1.1.5/setup.py`

 * *Files identical despite different names*

