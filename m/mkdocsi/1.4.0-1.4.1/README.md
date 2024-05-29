# Comparing `tmp/mkdocsi-1.4.0.tar.gz` & `tmp/mkdocsi-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.4.0.tar", last modified: Wed May 29 10:30:59 2024, max compression
+gzip compressed data, was "mkdocsi-1.4.1.tar", last modified: Wed May 29 10:33:10 2024, max compression
```

## Comparing `mkdocsi-1.4.0.tar` & `mkdocsi-1.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:30:59.973379 mkdocsi-1.4.0/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:30:59.973379 mkdocsi-1.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-29 10:30:50.000000 mkdocsi-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:30:59.971379 mkdocsi-1.4.0/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)     7685 2024-05-29 10:30:50.000000 mkdocsi-1.4.0/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:30:59.973379 mkdocsi-1.4.0/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:30:59.000000 mkdocsi-1.4.0/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      226 2024-05-29 10:30:59.000000 mkdocsi-1.4.0/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 10:30:59.000000 mkdocsi-1.4.0/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-05-29 10:30:59.000000 mkdocsi-1.4.0/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 10:30:59.000000 mkdocsi-1.4.0/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 10:30:59.000000 mkdocsi-1.4.0/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 10:30:59.973379 mkdocsi-1.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3049 2024-05-29 10:30:50.000000 mkdocsi-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:33:10.265871 mkdocsi-1.4.1/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:33:10.265871 mkdocsi-1.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-29 10:33:00.000000 mkdocsi-1.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:33:10.263871 mkdocsi-1.4.1/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)     7693 2024-05-29 10:33:00.000000 mkdocsi-1.4.1/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:33:10.264871 mkdocsi-1.4.1/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:33:10.000000 mkdocsi-1.4.1/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      226 2024-05-29 10:33:10.000000 mkdocsi-1.4.1/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 10:33:10.000000 mkdocsi-1.4.1/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-05-29 10:33:10.000000 mkdocsi-1.4.1/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 10:33:10.000000 mkdocsi-1.4.1/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 10:33:10.000000 mkdocsi-1.4.1/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 10:33:10.265871 mkdocsi-1.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2024-05-29 10:33:00.000000 mkdocsi-1.4.1/setup.py
```

### Comparing `mkdocsi-1.4.0/PKG-INFO` & `mkdocsi-1.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.4.0
+Version: 1.4.1
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.4.0/README.md` & `mkdocsi-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.4.0/mkdocsi/__init__.py` & `mkdocsi-1.4.1/mkdocsi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         if not os.path.exists(Tags_md) : 
             print("<!-- material/tags { scope: true } -->" , file = open(Tags_md , "w"))
             self.mkdocs_data['nav'].append({"Tags" : "Tags.md"})
 
     def cleanNav(self , nav) : 
         cleaned_nav = list() 
         set_keys = sorted({ k for i in nav for k , v in i.items() })
-        new_nav = { k : v for k , v in i for i in nav }
+        new_nav = { k : v for k , v in i.items() for i in nav }
         new_nav = [{ k : v } for k , v in new_nav.items()]
         return new_nav
         
 
     def __repr__(self) : 
         return json.dumps(self.mkdocs_data , indent = 4 )
```

### Comparing `mkdocsi-1.4.0/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.4.1/mkdocsi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.4.0
+Version: 1.4.1
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.4.0/setup.py` & `mkdocsi-1.4.1/setup.py`

 * *Files identical despite different names*

