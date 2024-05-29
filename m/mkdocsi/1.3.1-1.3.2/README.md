# Comparing `tmp/mkdocsi-1.3.1.tar.gz` & `tmp/mkdocsi-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.3.1.tar", last modified: Wed May 29 08:49:41 2024, max compression
+gzip compressed data, was "mkdocsi-1.3.2.tar", last modified: Wed May 29 08:55:45 2024, max compression
```

## Comparing `mkdocsi-1.3.1.tar` & `mkdocsi-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:49:41.334180 mkdocsi-1.3.1/
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-29 08:49:41.334180 mkdocsi-1.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-29 08:49:31.000000 mkdocsi-1.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:49:41.332180 mkdocsi-1.3.1/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-29 08:49:31.000000 mkdocsi-1.3.1/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-29 08:49:31.000000 mkdocsi-1.3.1/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:49:41.334180 mkdocsi-1.3.1/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-29 08:49:41.000000 mkdocsi-1.3.1/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-29 08:49:41.000000 mkdocsi-1.3.1/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 08:49:41.000000 mkdocsi-1.3.1/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-29 08:49:41.000000 mkdocsi-1.3.1/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 08:49:41.000000 mkdocsi-1.3.1/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 08:49:41.000000 mkdocsi-1.3.1/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 08:49:41.334180 mkdocsi-1.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-29 08:49:31.000000 mkdocsi-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:55:45.930725 mkdocsi-1.3.2/
+-rw-r--r--   0 root         (0) root         (0)      890 2024-05-29 08:55:45.929725 mkdocsi-1.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      413 2024-05-29 08:55:37.000000 mkdocsi-1.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:55:45.927725 mkdocsi-1.3.2/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-29 08:55:37.000000 mkdocsi-1.3.2/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-29 08:55:37.000000 mkdocsi-1.3.2/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:55:45.929725 mkdocsi-1.3.2/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      890 2024-05-29 08:55:45.000000 mkdocsi-1.3.2/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-29 08:55:45.000000 mkdocsi-1.3.2/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 08:55:45.000000 mkdocsi-1.3.2/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-29 08:55:45.000000 mkdocsi-1.3.2/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 08:55:45.000000 mkdocsi-1.3.2/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 08:55:45.000000 mkdocsi-1.3.2/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 08:55:45.930725 mkdocsi-1.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-29 08:55:37.000000 mkdocsi-1.3.2/setup.py
```

### Comparing `mkdocsi-1.3.1/PKG-INFO` & `mkdocsi-1.3.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.3.1
+Version: 1.3.2
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,12 +17,16 @@
 
 ## Installation : 
 ```bash
 pip install mkdocsi
 ```
 
 ## Quick start : 
-* 
+all agumenst passed are optionnals  : 
 ```bash
 python -m mkdocsi --docs=./docs --index=./README.md --site_name=documentation --mkdocs=./mkdocs.yml
+```
+when it come to doc repo git its handy to consider README.md as home page and have `docs` folder have all makdown files 
 
+```bash
+mkdocsi --docs=./docs --index=./README.md 
 ```
```

### Comparing `mkdocsi-1.3.1/mkdocsi/Main.py` & `mkdocsi-1.3.2/mkdocsi/Main.py`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.3.1/mkdocsi/__init__.py` & `mkdocsi-1.3.2/mkdocsi/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.3.1/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.3.2/mkdocsi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.3.1
+Version: 1.3.2
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,12 +17,16 @@
 
 ## Installation : 
 ```bash
 pip install mkdocsi
 ```
 
 ## Quick start : 
-* 
+all agumenst passed are optionnals  : 
 ```bash
 python -m mkdocsi --docs=./docs --index=./README.md --site_name=documentation --mkdocs=./mkdocs.yml
+```
+when it come to doc repo git its handy to consider README.md as home page and have `docs` folder have all makdown files 
 
+```bash
+mkdocsi --docs=./docs --index=./README.md 
 ```
```

### Comparing `mkdocsi-1.3.1/setup.py` & `mkdocsi-1.3.2/setup.py`

 * *Files identical despite different names*

