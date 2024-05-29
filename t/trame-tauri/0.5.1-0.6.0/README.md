# Comparing `tmp/trame-tauri-0.5.1.tar.gz` & `tmp/trame-tauri-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-tauri-0.5.1.tar", last modified: Fri May 24 21:01:36 2024, max compression
+gzip compressed data, was "trame-tauri-0.6.0.tar", last modified: Wed May 29 19:52:43 2024, max compression
```

## Comparing `trame-tauri-0.5.1.tar` & `trame-tauri-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/
--rw-r--r--   0 root         (0) root         (0)      583 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2518 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1736 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      925 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.110781 trame-tauri-0.5.1/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.110781 trame-tauri-0.5.1/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame/modules/tauri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame/widgets/tauri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/trame_tauri/
--rw-r--r--   0 root         (0) root         (0)       93 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame_tauri/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/trame_tauri/module/
--rw-r--r--   0 root         (0) root         (0)      199 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame_tauri/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/trame_tauri/module/serve/
--rw-r--r--   0 root         (0) root         (0)    36186 2024-05-24 21:01:32.000000 trame-tauri-0.5.1/trame_tauri/module/serve/trame-tauri.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/trame_tauri/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame_tauri/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7776 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame_tauri/widgets/tauri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/trame_tauri.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2518 2024-05-24 21:01:36.000000 trame-tauri-0.5.1/trame_tauri.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-05-24 21:01:36.000000 trame-tauri-0.5.1/trame_tauri.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 21:01:36.000000 trame-tauri-0.5.1/trame_tauri.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-24 21:01:36.000000 trame-tauri-0.5.1/trame_tauri.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-24 21:01:36.000000 trame-tauri-0.5.1/trame_tauri.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 19:52:43.252752 trame-tauri-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-29 19:52:19.000000 trame-tauri-0.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-29 19:52:19.000000 trame-tauri-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-05-29 19:52:43.252752 trame-tauri-0.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1736 2024-05-29 19:52:19.000000 trame-tauri-0.6.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      925 2024-05-29 19:52:43.252752 trame-tauri-0.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 19:52:19.000000 trame-tauri-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 19:52:43.248752 trame-tauri-0.6.0/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-29 19:52:19.000000 trame-tauri-0.6.0/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 19:52:43.248752 trame-tauri-0.6.0/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-29 19:52:19.000000 trame-tauri-0.6.0/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-29 19:52:19.000000 trame-tauri-0.6.0/trame/modules/tauri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 19:52:43.248752 trame-tauri-0.6.0/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-29 19:52:19.000000 trame-tauri-0.6.0/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      135 2024-05-29 19:52:19.000000 trame-tauri-0.6.0/trame/widgets/tauri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 19:52:43.248752 trame-tauri-0.6.0/trame_tauri/
+-rw-r--r--   0 root         (0) root         (0)       93 2024-05-29 19:52:19.000000 trame-tauri-0.6.0/trame_tauri/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 19:52:43.248752 trame-tauri-0.6.0/trame_tauri/module/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-05-29 19:52:19.000000 trame-tauri-0.6.0/trame_tauri/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 19:52:43.252752 trame-tauri-0.6.0/trame_tauri/module/serve/
+-rw-r--r--   0 root         (0) root         (0)    36198 2024-05-29 19:52:39.000000 trame-tauri-0.6.0/trame_tauri/module/serve/trame-tauri.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 19:52:43.252752 trame-tauri-0.6.0/trame_tauri/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-29 19:52:19.000000 trame-tauri-0.6.0/trame_tauri/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7776 2024-05-29 19:52:19.000000 trame-tauri-0.6.0/trame_tauri/widgets/tauri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 19:52:43.248752 trame-tauri-0.6.0/trame_tauri.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-05-29 19:52:43.000000 trame-tauri-0.6.0/trame_tauri.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-29 19:52:43.000000 trame-tauri-0.6.0/trame_tauri.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 19:52:43.000000 trame-tauri-0.6.0/trame_tauri.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-29 19:52:43.000000 trame-tauri-0.6.0/trame_tauri.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-29 19:52:43.000000 trame-tauri-0.6.0/trame_tauri.egg-info/top_level.txt
```

### Comparing `trame-tauri-0.5.1/LICENSE` & `trame-tauri-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-tauri-0.5.1/PKG-INFO` & `trame-tauri-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-tauri
-Version: 0.5.1
+Version: 0.6.0
 Summary: Helper widget to provide simpler integration with Tauri
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-tauri-0.5.1/README.rst` & `trame-tauri-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `trame-tauri-0.5.1/setup.cfg` & `trame-tauri-0.6.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-tauri
-version = 0.5.1
+version = 0.6.0
 description = Helper widget to provide simpler integration with Tauri
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `trame-tauri-0.5.1/trame_tauri/module/serve/trame-tauri.umd.js` & `trame-tauri-0.6.0/trame_tauri/module/serve/trame-tauri.umd.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1359,15 +1359,17 @@
                         position: i.value,
                         size: r.value
                     })
                 }), m.once("tauri://error", function(o) {
                     console.error("Tauri window error"), console.error(o)
                 }), _.push(m.onCloseRequested(o => {
                     e("closed"), t.preventClose && o.preventDefault()
-                })), _.push(m.onFileDropEvent(o => {
+                })), _.push(m.onFileDropEvent(({
+                    payload: o
+                }) => {
                     e("fileDrop", o)
                 })), _.push(m.onFocusChanged(({
                     payload: o
                 }) => {
                     e("focusChanged", o)
                 })), _.push(m.onMenuClicked(({
                     payload: o
```

### Comparing `trame-tauri-0.5.1/trame_tauri/widgets/tauri.py` & `trame-tauri-0.6.0/trame_tauri/widgets/tauri.py`

 * *Files identical despite different names*

### Comparing `trame-tauri-0.5.1/trame_tauri.egg-info/PKG-INFO` & `trame-tauri-0.6.0/trame_tauri.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-tauri
-Version: 0.5.1
+Version: 0.6.0
 Summary: Helper widget to provide simpler integration with Tauri
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

