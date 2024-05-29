# Comparing `tmp/pycorewlan-1.0.0.tar.gz` & `tmp/pycorewlan-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycorewlan-1.0.0.tar", last modified: Wed May 29 11:57:13 2024, max compression
+gzip compressed data, was "pycorewlan-1.0.1.tar", last modified: Wed May 29 12:05:24 2024, max compression
```

## Comparing `pycorewlan-1.0.0.tar` & `pycorewlan-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 lawsonoates   (501) staff       (20)        0 2024-05-29 11:57:13.623755 pycorewlan-1.0.0/
--rw-r--r--   0 lawsonoates   (501) staff       (20)     1076 2024-05-27 08:58:59.000000 pycorewlan-1.0.0/LICENSE.txt
--rw-r--r--   0 lawsonoates   (501) staff       (20)       65 2024-05-27 11:28:04.000000 pycorewlan-1.0.0/MANIFEST.in
--rw-r--r--   0 lawsonoates   (501) staff       (20)     1200 2024-05-29 11:57:13.623691 pycorewlan-1.0.0/PKG-INFO
--rw-r--r--   0 lawsonoates   (501) staff       (20)      615 2024-05-29 11:53:07.000000 pycorewlan-1.0.0/README.md
--rw-r--r--   0 lawsonoates   (501) staff       (20)       89 2024-05-27 09:06:43.000000 pycorewlan-1.0.0/pyproject.toml
--rw-r--r--   0 lawsonoates   (501) staff       (20)      694 2024-05-29 11:57:13.623997 pycorewlan-1.0.0/setup.cfg
-drwxr-xr-x   0 lawsonoates   (501) staff       (20)        0 2024-05-29 11:57:13.617572 pycorewlan-1.0.0/src/
-drwxr-xr-x   0 lawsonoates   (501) staff       (20)        0 2024-05-29 11:57:13.622777 pycorewlan-1.0.0/src/pyCoreWLAN/
--rw-r--r--   0 lawsonoates   (501) staff       (20)     1253 2024-05-10 07:18:20.000000 pycorewlan-1.0.0/src/pyCoreWLAN/CWChannel.pyi
--rw-r--r--   0 lawsonoates   (501) staff       (20)     5708 2024-05-27 07:59:11.000000 pycorewlan-1.0.0/src/pyCoreWLAN/CWConfiguration.pyi
--rw-r--r--   0 lawsonoates   (501) staff       (20)    19968 2024-05-21 06:49:19.000000 pycorewlan-1.0.0/src/pyCoreWLAN/CWInterface.pyi
--rw-r--r--   0 lawsonoates   (501) staff       (20)     4205 2024-05-18 06:26:51.000000 pycorewlan-1.0.0/src/pyCoreWLAN/CWNetwork.pyi
--rw-r--r--   0 lawsonoates   (501) staff       (20)     3360 2024-05-21 06:32:50.000000 pycorewlan-1.0.0/src/pyCoreWLAN/CWNetworkProfile.pyi
--rw-r--r--   0 lawsonoates   (501) staff       (20)     4618 2024-05-27 08:40:39.000000 pycorewlan-1.0.0/src/pyCoreWLAN/CWWiFiClient.pyi
--rw-r--r--   0 lawsonoates   (501) staff       (20)      232 2024-05-27 08:01:49.000000 pycorewlan-1.0.0/src/pyCoreWLAN/CoreWLAN.pyi
--rw-r--r--   0 lawsonoates   (501) staff       (20)     3535 2024-05-21 06:45:08.000000 pycorewlan-1.0.0/src/pyCoreWLAN/CoreWLANConstants.pyi
--rw-r--r--   0 lawsonoates   (501) staff       (20)     9709 2024-05-21 06:48:55.000000 pycorewlan-1.0.0/src/pyCoreWLAN/CoreWLANTypes.pyi
--rw-r--r--   0 lawsonoates   (501) staff       (20)     8267 2024-05-27 07:35:33.000000 pycorewlan-1.0.0/src/pyCoreWLAN/CoreWLANUtil.pyi
--rw-r--r--   0 lawsonoates   (501) staff       (20)      582 2024-05-27 08:10:50.000000 pycorewlan-1.0.0/src/pyCoreWLAN/FoundationTypes.pyi
--rw-r--r--   0 lawsonoates   (501) staff       (20)        0 2024-05-27 09:01:15.000000 pycorewlan-1.0.0/src/pyCoreWLAN/__init__.py
-drwxr-xr-x   0 lawsonoates   (501) staff       (20)        0 2024-05-29 11:57:13.623487 pycorewlan-1.0.0/src/pyCoreWLAN.egg-info/
--rw-r--r--   0 lawsonoates   (501) staff       (20)     1200 2024-05-29 11:57:13.000000 pycorewlan-1.0.0/src/pyCoreWLAN.egg-info/PKG-INFO
--rw-r--r--   0 lawsonoates   (501) staff       (20)      594 2024-05-29 11:57:13.000000 pycorewlan-1.0.0/src/pyCoreWLAN.egg-info/SOURCES.txt
--rw-r--r--   0 lawsonoates   (501) staff       (20)        1 2024-05-29 11:57:13.000000 pycorewlan-1.0.0/src/pyCoreWLAN.egg-info/dependency_links.txt
--rw-r--r--   0 lawsonoates   (501) staff       (20)       11 2024-05-29 11:57:13.000000 pycorewlan-1.0.0/src/pyCoreWLAN.egg-info/top_level.txt
+drwxr-xr-x   0 lawsonoates   (501) staff       (20)        0 2024-05-29 12:05:24.301621 pycorewlan-1.0.1/
+-rw-r--r--   0 lawsonoates   (501) staff       (20)     1076 2024-05-27 08:58:59.000000 pycorewlan-1.0.1/LICENSE.txt
+-rw-r--r--   0 lawsonoates   (501) staff       (20)       65 2024-05-27 11:28:04.000000 pycorewlan-1.0.1/MANIFEST.in
+-rw-r--r--   0 lawsonoates   (501) staff       (20)     1276 2024-05-29 12:05:24.301541 pycorewlan-1.0.1/PKG-INFO
+-rw-r--r--   0 lawsonoates   (501) staff       (20)      691 2024-05-29 12:02:23.000000 pycorewlan-1.0.1/README.md
+-rw-r--r--   0 lawsonoates   (501) staff       (20)       89 2024-05-27 09:06:43.000000 pycorewlan-1.0.1/pyproject.toml
+-rw-r--r--   0 lawsonoates   (501) staff       (20)      694 2024-05-29 12:05:24.301862 pycorewlan-1.0.1/setup.cfg
+drwxr-xr-x   0 lawsonoates   (501) staff       (20)        0 2024-05-29 12:05:24.298210 pycorewlan-1.0.1/src/
+drwxr-xr-x   0 lawsonoates   (501) staff       (20)        0 2024-05-29 12:05:24.300645 pycorewlan-1.0.1/src/pyCoreWLAN/
+-rw-r--r--   0 lawsonoates   (501) staff       (20)     1253 2024-05-10 07:18:20.000000 pycorewlan-1.0.1/src/pyCoreWLAN/CWChannel.pyi
+-rw-r--r--   0 lawsonoates   (501) staff       (20)     5708 2024-05-27 07:59:11.000000 pycorewlan-1.0.1/src/pyCoreWLAN/CWConfiguration.pyi
+-rw-r--r--   0 lawsonoates   (501) staff       (20)    19968 2024-05-21 06:49:19.000000 pycorewlan-1.0.1/src/pyCoreWLAN/CWInterface.pyi
+-rw-r--r--   0 lawsonoates   (501) staff       (20)     4205 2024-05-18 06:26:51.000000 pycorewlan-1.0.1/src/pyCoreWLAN/CWNetwork.pyi
+-rw-r--r--   0 lawsonoates   (501) staff       (20)     3360 2024-05-21 06:32:50.000000 pycorewlan-1.0.1/src/pyCoreWLAN/CWNetworkProfile.pyi
+-rw-r--r--   0 lawsonoates   (501) staff       (20)     4618 2024-05-27 08:40:39.000000 pycorewlan-1.0.1/src/pyCoreWLAN/CWWiFiClient.pyi
+-rw-r--r--   0 lawsonoates   (501) staff       (20)      232 2024-05-27 08:01:49.000000 pycorewlan-1.0.1/src/pyCoreWLAN/CoreWLAN.pyi
+-rw-r--r--   0 lawsonoates   (501) staff       (20)     3535 2024-05-21 06:45:08.000000 pycorewlan-1.0.1/src/pyCoreWLAN/CoreWLANConstants.pyi
+-rw-r--r--   0 lawsonoates   (501) staff       (20)     9709 2024-05-21 06:48:55.000000 pycorewlan-1.0.1/src/pyCoreWLAN/CoreWLANTypes.pyi
+-rw-r--r--   0 lawsonoates   (501) staff       (20)     8267 2024-05-27 07:35:33.000000 pycorewlan-1.0.1/src/pyCoreWLAN/CoreWLANUtil.pyi
+-rw-r--r--   0 lawsonoates   (501) staff       (20)      582 2024-05-27 08:10:50.000000 pycorewlan-1.0.1/src/pyCoreWLAN/FoundationTypes.pyi
+-rw-r--r--   0 lawsonoates   (501) staff       (20)        0 2024-05-27 09:01:15.000000 pycorewlan-1.0.1/src/pyCoreWLAN/__init__.py
+drwxr-xr-x   0 lawsonoates   (501) staff       (20)        0 2024-05-29 12:05:24.301333 pycorewlan-1.0.1/src/pyCoreWLAN.egg-info/
+-rw-r--r--   0 lawsonoates   (501) staff       (20)     1276 2024-05-29 12:05:24.000000 pycorewlan-1.0.1/src/pyCoreWLAN.egg-info/PKG-INFO
+-rw-r--r--   0 lawsonoates   (501) staff       (20)      594 2024-05-29 12:05:24.000000 pycorewlan-1.0.1/src/pyCoreWLAN.egg-info/SOURCES.txt
+-rw-r--r--   0 lawsonoates   (501) staff       (20)        1 2024-05-29 12:05:24.000000 pycorewlan-1.0.1/src/pyCoreWLAN.egg-info/dependency_links.txt
+-rw-r--r--   0 lawsonoates   (501) staff       (20)       11 2024-05-29 12:05:24.000000 pycorewlan-1.0.1/src/pyCoreWLAN.egg-info/top_level.txt
```

### Comparing `pycorewlan-1.0.0/LICENSE.txt` & `pycorewlan-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycorewlan-1.0.0/PKG-INFO` & `pycorewlan-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: pyCoreWLAN
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package that provides stubs for the PyObjC CoreWLAN Wrapper.
 Home-page: https://github.com/lawsonoates/pyCoreWLAN
 Author: Lawson Oates
 Project-URL: Bug Tracker, https://github.com/lawsonoates/pyCoreWLAN/issues
 Project-URL: repository, https://github.com/lawsonoates/pyCoreWLAN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# pyCoreWLAN
+# `pyCoreWLAN`
 
 Provides Python stubs for the Apple [CoreWLAN](https://developer.apple.com/documentation/corewlan) framework and should be used alongside the CoreWLAN wrappers provided by [PyObjC](https://github.com/ronaldoussoren/pyobjc).
 Provides code completion and docstring hints equivalent to the CoreWLAN
 documentation. Intended to work with VS Code Intellisense with Pylance installed.
 
-## Installation
+## Installation & Usage
+
+Install `pyCoreWLAN` as follows:
+
+```
+pip install pyCoreWLAN
+```
 
 For use with VSCode, update the settings to include the path to the package if using a virtual environment.
 
 ```json
 {
   "python.analysis.stubPath": "./.venv/lib/python3.10/site-packages/pyCoreWLAN"
 }
```

### Comparing `pycorewlan-1.0.0/README.md` & `pycorewlan-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-# pyCoreWLAN
+# `pyCoreWLAN`
 
 Provides Python stubs for the Apple [CoreWLAN](https://developer.apple.com/documentation/corewlan) framework and should be used alongside the CoreWLAN wrappers provided by [PyObjC](https://github.com/ronaldoussoren/pyobjc).
 Provides code completion and docstring hints equivalent to the CoreWLAN
 documentation. Intended to work with VS Code Intellisense with Pylance installed.
 
-## Installation
+## Installation & Usage
+
+Install `pyCoreWLAN` as follows:
+
+```
+pip install pyCoreWLAN
+```
 
 For use with VSCode, update the settings to include the path to the package if using a virtual environment.
 
 ```json
 {
   "python.analysis.stubPath": "./.venv/lib/python3.10/site-packages/pyCoreWLAN"
 }
```

### Comparing `pycorewlan-1.0.0/setup.cfg` & `pycorewlan-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyCoreWLAN
-version = 1.0.0
+version = 1.0.1
 author = Lawson Oates
 description = A Python package that provides stubs for the PyObjC CoreWLAN Wrapper.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/lawsonoates/pyCoreWLAN
 project_urls = 
 	Bug Tracker = https://github.com/lawsonoates/pyCoreWLAN/issues
```

### Comparing `pycorewlan-1.0.0/src/pyCoreWLAN/CWChannel.pyi` & `pycorewlan-1.0.1/src/pyCoreWLAN/CWChannel.pyi`

 * *Files identical despite different names*

### Comparing `pycorewlan-1.0.0/src/pyCoreWLAN/CWConfiguration.pyi` & `pycorewlan-1.0.1/src/pyCoreWLAN/CWConfiguration.pyi`

 * *Files identical despite different names*

### Comparing `pycorewlan-1.0.0/src/pyCoreWLAN/CWInterface.pyi` & `pycorewlan-1.0.1/src/pyCoreWLAN/CWInterface.pyi`

 * *Files identical despite different names*

### Comparing `pycorewlan-1.0.0/src/pyCoreWLAN/CWNetwork.pyi` & `pycorewlan-1.0.1/src/pyCoreWLAN/CWNetwork.pyi`

 * *Files identical despite different names*

### Comparing `pycorewlan-1.0.0/src/pyCoreWLAN/CWNetworkProfile.pyi` & `pycorewlan-1.0.1/src/pyCoreWLAN/CWNetworkProfile.pyi`

 * *Files identical despite different names*

### Comparing `pycorewlan-1.0.0/src/pyCoreWLAN/CWWiFiClient.pyi` & `pycorewlan-1.0.1/src/pyCoreWLAN/CWWiFiClient.pyi`

 * *Files identical despite different names*

### Comparing `pycorewlan-1.0.0/src/pyCoreWLAN/CoreWLANConstants.pyi` & `pycorewlan-1.0.1/src/pyCoreWLAN/CoreWLANConstants.pyi`

 * *Files identical despite different names*

### Comparing `pycorewlan-1.0.0/src/pyCoreWLAN/CoreWLANTypes.pyi` & `pycorewlan-1.0.1/src/pyCoreWLAN/CoreWLANTypes.pyi`

 * *Files identical despite different names*

### Comparing `pycorewlan-1.0.0/src/pyCoreWLAN/CoreWLANUtil.pyi` & `pycorewlan-1.0.1/src/pyCoreWLAN/CoreWLANUtil.pyi`

 * *Files identical despite different names*

### Comparing `pycorewlan-1.0.0/src/pyCoreWLAN/FoundationTypes.pyi` & `pycorewlan-1.0.1/src/pyCoreWLAN/FoundationTypes.pyi`

 * *Files identical despite different names*

### Comparing `pycorewlan-1.0.0/src/pyCoreWLAN.egg-info/PKG-INFO` & `pycorewlan-1.0.1/src/pyCoreWLAN.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: pyCoreWLAN
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package that provides stubs for the PyObjC CoreWLAN Wrapper.
 Home-page: https://github.com/lawsonoates/pyCoreWLAN
 Author: Lawson Oates
 Project-URL: Bug Tracker, https://github.com/lawsonoates/pyCoreWLAN/issues
 Project-URL: repository, https://github.com/lawsonoates/pyCoreWLAN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# pyCoreWLAN
+# `pyCoreWLAN`
 
 Provides Python stubs for the Apple [CoreWLAN](https://developer.apple.com/documentation/corewlan) framework and should be used alongside the CoreWLAN wrappers provided by [PyObjC](https://github.com/ronaldoussoren/pyobjc).
 Provides code completion and docstring hints equivalent to the CoreWLAN
 documentation. Intended to work with VS Code Intellisense with Pylance installed.
 
-## Installation
+## Installation & Usage
+
+Install `pyCoreWLAN` as follows:
+
+```
+pip install pyCoreWLAN
+```
 
 For use with VSCode, update the settings to include the path to the package if using a virtual environment.
 
 ```json
 {
   "python.analysis.stubPath": "./.venv/lib/python3.10/site-packages/pyCoreWLAN"
 }
```

### Comparing `pycorewlan-1.0.0/src/pyCoreWLAN.egg-info/SOURCES.txt` & `pycorewlan-1.0.1/src/pyCoreWLAN.egg-info/SOURCES.txt`

 * *Files identical despite different names*

