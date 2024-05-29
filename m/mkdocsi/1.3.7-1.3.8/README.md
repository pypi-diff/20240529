# Comparing `tmp/mkdocsi-1.3.7.tar.gz` & `tmp/mkdocsi-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.3.7.tar", last modified: Wed May 29 10:01:57 2024, max compression
+gzip compressed data, was "mkdocsi-1.3.8.tar", last modified: Wed May 29 10:03:44 2024, max compression
```

## Comparing `mkdocsi-1.3.7.tar` & `mkdocsi-1.3.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:01:57.397129 mkdocsi-1.3.7/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:01:57.397129 mkdocsi-1.3.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-29 10:01:47.000000 mkdocsi-1.3.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:01:57.395129 mkdocsi-1.3.7/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)     7332 2024-05-29 10:01:47.000000 mkdocsi-1.3.7/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:01:57.396129 mkdocsi-1.3.7/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:01:57.000000 mkdocsi-1.3.7/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      226 2024-05-29 10:01:57.000000 mkdocsi-1.3.7/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 10:01:57.000000 mkdocsi-1.3.7/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-29 10:01:57.000000 mkdocsi-1.3.7/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 10:01:57.000000 mkdocsi-1.3.7/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 10:01:57.000000 mkdocsi-1.3.7/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 10:01:57.397129 mkdocsi-1.3.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3047 2024-05-29 10:01:47.000000 mkdocsi-1.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:03:44.223803 mkdocsi-1.3.8/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:03:44.223803 mkdocsi-1.3.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-29 10:03:34.000000 mkdocsi-1.3.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:03:44.221803 mkdocsi-1.3.8/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)     7334 2024-05-29 10:03:34.000000 mkdocsi-1.3.8/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 10:03:44.223803 mkdocsi-1.3.8/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 10:03:44.000000 mkdocsi-1.3.8/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      226 2024-05-29 10:03:44.000000 mkdocsi-1.3.8/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 10:03:44.000000 mkdocsi-1.3.8/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-05-29 10:03:44.000000 mkdocsi-1.3.8/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 10:03:44.000000 mkdocsi-1.3.8/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 10:03:44.000000 mkdocsi-1.3.8/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 10:03:44.223803 mkdocsi-1.3.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2024-05-29 10:03:34.000000 mkdocsi-1.3.8/setup.py
```

### Comparing `mkdocsi-1.3.7/PKG-INFO` & `mkdocsi-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.3.7
+Version: 1.3.8
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.3.7/README.md` & `mkdocsi-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.3.7/mkdocsi/__init__.py` & `mkdocsi-1.3.8/mkdocsi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 
 
 
 
 
 
-def BashCalledMain():
+def __ENTRY__POINT__():
     parser = argparse.ArgumentParser()
     parser.add_argument('--index',  type = str , default= None  , required = False )
     parser.add_argument('--docs',  type = str , default= os.path.join(os.getcwd() , "docs")  , required = False )
     parser.add_argument('--mkdocs', type = str , default= None   , required = False )
     parser.add_argument('--site_name',  type = str , default= os.path.basename(os.getcwd())   , required = False)
 
     args = parser.parse_args()
```

### Comparing `mkdocsi-1.3.7/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.3.8/mkdocsi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.3.7
+Version: 1.3.8
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.3.7/setup.py` & `mkdocsi-1.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             classifiers=[
                 'Programming Language :: Python :: 3',
                 'License :: OSI Approved :: MIT License',
                 'Operating System :: OS Independent',
             ],
             entry_points={
                 'console_scripts': [
-                    f'{self.name} = {self.name}:BashCalledMain'
+                    f'{self.name} = {self.name}:__ENTRY__POINT__'
                 ]
             }
         )
     def get_versions(self) : 
         response = requests.get(f"https://pypi.org/pypi/{self.name}/json")
         version = self.start_version
         if response.status_code == 200 :
```

