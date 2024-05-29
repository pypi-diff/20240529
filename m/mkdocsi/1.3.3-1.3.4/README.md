# Comparing `tmp/mkdocsi-1.3.3.tar.gz` & `tmp/mkdocsi-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.3.3.tar", last modified: Wed May 29 08:57:10 2024, max compression
+gzip compressed data, was "mkdocsi-1.3.4.tar", last modified: Wed May 29 09:45:26 2024, max compression
```

## Comparing `mkdocsi-1.3.3.tar` & `mkdocsi-1.3.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:57:10.019937 mkdocsi-1.3.3/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 08:57:10.019937 mkdocsi-1.3.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-29 08:57:00.000000 mkdocsi-1.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:57:10.017937 mkdocsi-1.3.3/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-29 08:57:00.000000 mkdocsi-1.3.3/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-29 08:57:00.000000 mkdocsi-1.3.3/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:57:10.018937 mkdocsi-1.3.3/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 08:57:09.000000 mkdocsi-1.3.3/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-29 08:57:09.000000 mkdocsi-1.3.3/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 08:57:09.000000 mkdocsi-1.3.3/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-29 08:57:09.000000 mkdocsi-1.3.3/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 08:57:09.000000 mkdocsi-1.3.3/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 08:57:09.000000 mkdocsi-1.3.3/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 08:57:10.019937 mkdocsi-1.3.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-29 08:57:00.000000 mkdocsi-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:45:26.173071 mkdocsi-1.3.4/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 09:45:26.173071 mkdocsi-1.3.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-29 09:45:16.000000 mkdocsi-1.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:45:26.171071 mkdocsi-1.3.4/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2024-05-29 09:45:16.000000 mkdocsi-1.3.4/mkdocsi/ __main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-29 09:45:16.000000 mkdocsi-1.3.4/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-29 09:45:16.000000 mkdocsi-1.3.4/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:45:26.172071 mkdocsi-1.3.4/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 09:45:26.000000 mkdocsi-1.3.4/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      263 2024-05-29 09:45:26.000000 mkdocsi-1.3.4/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 09:45:26.000000 mkdocsi-1.3.4/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-29 09:45:26.000000 mkdocsi-1.3.4/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-29 09:45:26.000000 mkdocsi-1.3.4/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 09:45:26.000000 mkdocsi-1.3.4/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 09:45:26.173071 mkdocsi-1.3.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2024-05-29 09:45:16.000000 mkdocsi-1.3.4/setup.py
```

### Comparing `mkdocsi-1.3.3/PKG-INFO` & `mkdocsi-1.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.3.3
+Version: 1.3.4
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.3.3/README.md` & `mkdocsi-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.3.3/mkdocsi/Main.py` & `mkdocsi-1.3.4/mkdocsi/Main.py`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.3.3/mkdocsi/__init__.py` & `mkdocsi-1.3.4/mkdocsi/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.3.3/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.3.4/mkdocsi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.3.3
+Version: 1.3.4
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.3.3/setup.py` & `mkdocsi-1.3.4/setup.py`

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
-                    f'{self.name} = {self.name}.Main:main'
+                    f'{self.name} = {self.name}.__main__:main'
                 ]
             }
         )
     def get_versions(self) : 
         response = requests.get(f"https://pypi.org/pypi/{self.name}/json")
         version = self.start_version
         if response.status_code == 200 :
```

