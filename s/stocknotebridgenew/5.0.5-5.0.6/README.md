# Comparing `tmp/stocknotebridgenew-5.0.5.tar.gz` & `tmp/stocknotebridgenew-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stocknotebridgenew-5.0.5.tar", last modified: Wed May 29 08:19:19 2024, max compression
+gzip compressed data, was "stocknotebridgenew-5.0.6.tar", last modified: Wed May 29 12:21:06 2024, max compression
```

## Comparing `stocknotebridgenew-5.0.5.tar` & `stocknotebridgenew-5.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-29 08:19:19.521163 stocknotebridgenew-5.0.5/
--rwxrwxrwx   0 root         (0) wheel        (0)     1082 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.5/LICENSE
--rwxrwxrwx   0 root         (0) wheel        (0)       25 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-29 08:19:19.521362 stocknotebridgenew-5.0.5/PKG-INFO
--rwxrwxrwx   0 root         (0) wheel        (0)    43188 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.5/README.md
--rwxrwxrwx   0 root         (0) wheel        (0)      108 2024-05-29 08:19:19.521644 stocknotebridgenew-5.0.5/setup.cfg
--rwxrwxrwx   0 root         (0) wheel        (0)      906 2024-05-29 08:19:03.000000 stocknotebridgenew-5.0.5/setup.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-29 08:19:19.517283 stocknotebridgenew-5.0.5/snapi_py_client/
--rwxrwxrwx   0 root         (0) wheel        (0)        0 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.5/snapi_py_client/__init__.py
--rwxrwxrwx   0 root         (0) wheel        (0)    26717 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.5/snapi_py_client/api_client.py
--rwxrwxrwx   0 root         (0) wheel        (0)     9294 2024-05-28 10:03:09.000000 stocknotebridgenew-5.0.5/snapi_py_client/configuration.py
--rwxrwxrwx   0 root         (0) wheel        (0)    14674 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.5/snapi_py_client/rest.py
--rwxrwxrwx   0 root         (0) wheel        (0)   236992 2024-05-29 08:18:26.000000 stocknotebridgenew-5.0.5/snapi_py_client/snapi_bridge.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-29 08:19:19.520986 stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/
--rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-29 08:19:19.000000 stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) wheel        (0)      404 2024-05-29 08:19:19.000000 stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) wheel        (0)        1 2024-05-29 08:19:19.000000 stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) wheel        (0)       37 2024-05-29 08:19:19.000000 stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/requires.txt
--rw-r--r--   0 root         (0) wheel        (0)       16 2024-05-29 08:19:19.000000 stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/top_level.txt
+drwxr-xr-x   0 mohammad.arsh   (502) wheel        (0)        0 2024-05-29 12:21:06.937843 stocknotebridgenew-5.0.6/
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)     1082 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.6/LICENSE
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)       25 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.6/MANIFEST.in
+-rw-r--r--   0 mohammad.arsh   (502) wheel        (0)      817 2024-05-29 12:21:06.937909 stocknotebridgenew-5.0.6/PKG-INFO
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)    43188 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.6/README.md
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)      108 2024-05-29 12:21:06.938130 stocknotebridgenew-5.0.6/setup.cfg
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)      906 2024-05-29 12:20:54.000000 stocknotebridgenew-5.0.6/setup.py
+drwxr-xr-x   0 mohammad.arsh   (502) wheel        (0)        0 2024-05-29 12:21:06.936442 stocknotebridgenew-5.0.6/snapi_py_client/
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)        0 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.6/snapi_py_client/__init__.py
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)    26717 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.6/snapi_py_client/api_client.py
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)     9289 2024-05-29 12:19:43.000000 stocknotebridgenew-5.0.6/snapi_py_client/configuration.py
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)    14674 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.6/snapi_py_client/rest.py
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)   236992 2024-05-29 08:18:26.000000 stocknotebridgenew-5.0.6/snapi_py_client/snapi_bridge.py
+drwxr-xr-x   0 mohammad.arsh   (502) wheel        (0)        0 2024-05-29 12:21:06.937737 stocknotebridgenew-5.0.6/stocknotebridgenew.egg-info/
+-rw-r--r--   0 mohammad.arsh   (502) wheel        (0)      817 2024-05-29 12:21:06.000000 stocknotebridgenew-5.0.6/stocknotebridgenew.egg-info/PKG-INFO
+-rw-r--r--   0 mohammad.arsh   (502) wheel        (0)      404 2024-05-29 12:21:06.000000 stocknotebridgenew-5.0.6/stocknotebridgenew.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammad.arsh   (502) wheel        (0)        1 2024-05-29 12:21:06.000000 stocknotebridgenew-5.0.6/stocknotebridgenew.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammad.arsh   (502) wheel        (0)       37 2024-05-29 12:21:06.000000 stocknotebridgenew-5.0.6/stocknotebridgenew.egg-info/requires.txt
+-rw-r--r--   0 mohammad.arsh   (502) wheel        (0)       16 2024-05-29 12:21:06.000000 stocknotebridgenew-5.0.6/stocknotebridgenew.egg-info/top_level.txt
```

### Comparing `stocknotebridgenew-5.0.5/LICENSE` & `stocknotebridgenew-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.5/PKG-INFO` & `stocknotebridgenew-5.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocknotebridgenew
-Version: 5.0.5
+Version: 5.0.6
 Summary: official python library for Stocknote APIs
 Home-page: https://github.com/samco-sdk/Python-SDK
 Author: Samco Securities Limited
 Author-email: apisupport@samco.in
 License: MIT License
 Keywords: stocknote api,stocknote python sdk,samco api trading,samco algo trading,stock markets samco
 Platform: UNKNOWN
```

### Comparing `stocknotebridgenew-5.0.5/README.md` & `stocknotebridgenew-5.0.6/README.md`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.5/setup.py` & `stocknotebridgenew-5.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='stocknotebridgenew',
-version='5.0.5',
+version='5.0.6',
 description='official python library for Stocknote APIs',
 url='https://github.com/samco-sdk/Python-SDK',
 install_requires=['future', 'requests','websocket-client','six'],
 author='Samco Securities Limited',
 author_email='apisupport@samco.in',
 license='MIT License',
 packages=['snapi_py_client'],
```

### Comparing `stocknotebridgenew-5.0.5/snapi_py_client/api_client.py` & `stocknotebridgenew-5.0.6/snapi_py_client/api_client.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.5/snapi_py_client/configuration.py` & `stocknotebridgenew-5.0.6/snapi_py_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         """Constructor"""
         if self._default:
             for key in self._default.__dict__.keys():
                 self.__dict__[key] = copy.copy(self._default.__dict__[key])
             return
 
         # Default Base url
-        self.host = "https://beta-tradeapi.samco.in"
+        self.host = "https://tradeapi.samco.in"
         # Temp file folder for downloading files
         self.temp_folder_path = None
 
         # Authentication Settings
         # dict to store API key(s)
         self.api_key = {}
         # dict to store API prefix (e.g. Bearer)
```

### Comparing `stocknotebridgenew-5.0.5/snapi_py_client/rest.py` & `stocknotebridgenew-5.0.6/snapi_py_client/rest.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.5/snapi_py_client/snapi_bridge.py` & `stocknotebridgenew-5.0.6/snapi_py_client/snapi_bridge.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/PKG-INFO` & `stocknotebridgenew-5.0.6/stocknotebridgenew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocknotebridgenew
-Version: 5.0.5
+Version: 5.0.6
 Summary: official python library for Stocknote APIs
 Home-page: https://github.com/samco-sdk/Python-SDK
 Author: Samco Securities Limited
 Author-email: apisupport@samco.in
 License: MIT License
 Keywords: stocknote api,stocknote python sdk,samco api trading,samco algo trading,stock markets samco
 Platform: UNKNOWN
```

