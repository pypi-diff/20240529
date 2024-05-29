# Comparing `tmp/mkdocsi-1.2.5.tar.gz` & `tmp/mkdocsi-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.2.5.tar", last modified: Wed May 29 08:33:51 2024, max compression
+gzip compressed data, was "mkdocsi-1.2.6.tar", last modified: Wed May 29 08:38:44 2024, max compression
```

## Comparing `mkdocsi-1.2.5.tar` & `mkdocsi-1.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:33:51.477001 mkdocsi-1.2.5/
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-29 08:33:51.477001 mkdocsi-1.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-29 08:33:42.000000 mkdocsi-1.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:33:51.475001 mkdocsi-1.2.5/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)     1237 2024-05-29 08:33:42.000000 mkdocsi-1.2.5/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-29 08:33:42.000000 mkdocsi-1.2.5/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:33:51.476001 mkdocsi-1.2.5/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-29 08:33:51.000000 mkdocsi-1.2.5/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-29 08:33:51.000000 mkdocsi-1.2.5/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 08:33:51.000000 mkdocsi-1.2.5/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-29 08:33:51.000000 mkdocsi-1.2.5/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 08:33:51.000000 mkdocsi-1.2.5/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 08:33:51.000000 mkdocsi-1.2.5/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 08:33:51.477001 mkdocsi-1.2.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-29 08:33:42.000000 mkdocsi-1.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:38:44.505818 mkdocsi-1.2.6/
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-29 08:38:44.505818 mkdocsi-1.2.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-29 08:38:35.000000 mkdocsi-1.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:38:44.503818 mkdocsi-1.2.6/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-29 08:38:35.000000 mkdocsi-1.2.6/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-29 08:38:35.000000 mkdocsi-1.2.6/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:38:44.504818 mkdocsi-1.2.6/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-29 08:38:44.000000 mkdocsi-1.2.6/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-29 08:38:44.000000 mkdocsi-1.2.6/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 08:38:44.000000 mkdocsi-1.2.6/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-29 08:38:44.000000 mkdocsi-1.2.6/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 08:38:44.000000 mkdocsi-1.2.6/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 08:38:44.000000 mkdocsi-1.2.6/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 08:38:44.505818 mkdocsi-1.2.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-29 08:38:35.000000 mkdocsi-1.2.6/setup.py
```

### Comparing `mkdocsi-1.2.5/PKG-INFO` & `mkdocsi-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.2.5
+Version: 1.2.6
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.2.5/mkdocsi/__init__.py` & `mkdocsi-1.2.6/mkdocsi/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.2.5/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.2.6/mkdocsi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.2.5
+Version: 1.2.6
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.2.5/setup.py` & `mkdocsi-1.2.6/setup.py`

 * *Files identical despite different names*

