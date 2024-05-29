# Comparing `tmp/stocknotebridgenew-5.0.2.tar.gz` & `tmp/stocknotebridgenew-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stocknotebridgenew-5.0.2.tar", last modified: Tue May 28 07:04:43 2024, max compression
+gzip compressed data, was "stocknotebridgenew-5.0.4.tar", last modified: Tue May 28 10:03:37 2024, max compression
```

## Comparing `stocknotebridgenew-5.0.2.tar` & `stocknotebridgenew-5.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 07:04:43.543575 stocknotebridgenew-5.0.2/
--rwxrwxrwx   0 root         (0) wheel        (0)     1082 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.2/LICENSE
--rwxrwxrwx   0 root         (0) wheel        (0)       25 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-28 07:04:43.543630 stocknotebridgenew-5.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) wheel        (0)    43188 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.2/README.md
--rwxrwxrwx   0 root         (0) wheel        (0)      108 2024-05-28 07:04:43.543828 stocknotebridgenew-5.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) wheel        (0)      906 2024-05-28 07:04:24.000000 stocknotebridgenew-5.0.2/setup.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 07:04:43.541983 stocknotebridgenew-5.0.2/snapi_py_client/
--rwxrwxrwx   0 root         (0) wheel        (0)        0 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.2/snapi_py_client/__init__.py
--rwxrwxrwx   0 root         (0) wheel        (0)    26717 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.2/snapi_py_client/api_client.py
--rwxrwxrwx   0 root         (0) wheel        (0)     9289 2024-05-27 13:31:39.000000 stocknotebridgenew-5.0.2/snapi_py_client/configuration.py
--rwxrwxrwx   0 root         (0) wheel        (0)    14674 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.2/snapi_py_client/rest.py
--rwxrwxrwx   0 root         (0) wheel        (0)   236960 2024-05-28 06:54:33.000000 stocknotebridgenew-5.0.2/snapi_py_client/snapi_bridge.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 07:04:43.543479 stocknotebridgenew-5.0.2/stocknotebridgenew.egg-info/
--rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-28 07:04:43.000000 stocknotebridgenew-5.0.2/stocknotebridgenew.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) wheel        (0)      404 2024-05-28 07:04:43.000000 stocknotebridgenew-5.0.2/stocknotebridgenew.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) wheel        (0)        1 2024-05-28 07:04:43.000000 stocknotebridgenew-5.0.2/stocknotebridgenew.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) wheel        (0)       37 2024-05-28 07:04:43.000000 stocknotebridgenew-5.0.2/stocknotebridgenew.egg-info/requires.txt
--rw-r--r--   0 root         (0) wheel        (0)       16 2024-05-28 07:04:43.000000 stocknotebridgenew-5.0.2/stocknotebridgenew.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 10:03:37.194451 stocknotebridgenew-5.0.4/
+-rwxrwxrwx   0 root         (0) wheel        (0)     1082 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.4/LICENSE
+-rwxrwxrwx   0 root         (0) wheel        (0)       25 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-28 10:03:37.194508 stocknotebridgenew-5.0.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) wheel        (0)    43188 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.4/README.md
+-rwxrwxrwx   0 root         (0) wheel        (0)      108 2024-05-28 10:03:37.194723 stocknotebridgenew-5.0.4/setup.cfg
+-rwxrwxrwx   0 root         (0) wheel        (0)      906 2024-05-28 10:03:33.000000 stocknotebridgenew-5.0.4/setup.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 10:03:37.192837 stocknotebridgenew-5.0.4/snapi_py_client/
+-rwxrwxrwx   0 root         (0) wheel        (0)        0 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.4/snapi_py_client/__init__.py
+-rwxrwxrwx   0 root         (0) wheel        (0)    26717 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.4/snapi_py_client/api_client.py
+-rwxrwxrwx   0 root         (0) wheel        (0)     9294 2024-05-28 10:03:09.000000 stocknotebridgenew-5.0.4/snapi_py_client/configuration.py
+-rwxrwxrwx   0 root         (0) wheel        (0)    14674 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.4/snapi_py_client/rest.py
+-rwxrwxrwx   0 root         (0) wheel        (0)   236960 2024-05-28 07:32:47.000000 stocknotebridgenew-5.0.4/snapi_py_client/snapi_bridge.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 10:03:37.194342 stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/
+-rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-28 10:03:37.000000 stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) wheel        (0)      404 2024-05-28 10:03:37.000000 stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) wheel        (0)        1 2024-05-28 10:03:37.000000 stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) wheel        (0)       37 2024-05-28 10:03:37.000000 stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/requires.txt
+-rw-r--r--   0 root         (0) wheel        (0)       16 2024-05-28 10:03:37.000000 stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/top_level.txt
```

### Comparing `stocknotebridgenew-5.0.2/LICENSE` & `stocknotebridgenew-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.2/PKG-INFO` & `stocknotebridgenew-5.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocknotebridgenew
-Version: 5.0.2
+Version: 5.0.4
 Summary: official python library for Stocknote APIs
 Home-page: https://github.com/samco-sdk/Python-SDK
 Author: Samco Securities Limited
 Author-email: apisupport@samco.in
 License: MIT License
 Keywords: stocknote api,stocknote python sdk,samco api trading,samco algo trading,stock markets samco
 Platform: UNKNOWN
```

### Comparing `stocknotebridgenew-5.0.2/README.md` & `stocknotebridgenew-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.2/setup.py` & `stocknotebridgenew-5.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='stocknotebridgenew',
-version='5.0.2',
+version='5.0.4',
 description='official python library for Stocknote APIs',
 url='https://github.com/samco-sdk/Python-SDK',
 install_requires=['future', 'requests','websocket-client','six'],
 author='Samco Securities Limited',
 author_email='apisupport@samco.in',
 license='MIT License',
 packages=['snapi_py_client'],
```

### Comparing `stocknotebridgenew-5.0.2/snapi_py_client/api_client.py` & `stocknotebridgenew-5.0.4/snapi_py_client/api_client.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.2/snapi_py_client/configuration.py` & `stocknotebridgenew-5.0.4/snapi_py_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         """Constructor"""
         if self._default:
             for key in self._default.__dict__.keys():
                 self.__dict__[key] = copy.copy(self._default.__dict__[key])
             return
 
         # Default Base url
-        self.host = "https://tradeapi.samco.in"
+        self.host = "https://beta-tradeapi.samco.in"
         # Temp file folder for downloading files
         self.temp_folder_path = None
 
         # Authentication Settings
         # dict to store API key(s)
         self.api_key = {}
         # dict to store API prefix (e.g. Bearer)
```

### Comparing `stocknotebridgenew-5.0.2/snapi_py_client/rest.py` & `stocknotebridgenew-5.0.4/snapi_py_client/rest.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.2/snapi_py_client/snapi_bridge.py` & `stocknotebridgenew-5.0.4/snapi_py_client/snapi_bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     PRODUCT_BO = "BO"
     
     
     # Exchanges
     EXCHANGE_NSE = "NSE"
     EXCHANGE_BSE = "BSE"
     EXCHANGE_NFO = "NFO"
-    EXCHANGE_MCX = "BFO"
+    EXCHANGE_BFO = "BFO"
     EXCHANGE_CDS = "CDS"
     EXCHANGE_MCX = "MCX"
     
     
     # Transaction type
     TRANSACTION_TYPE_BUY = "BUY"
     TRANSACTION_TYPE_SELL = "SELL"
```

### Comparing `stocknotebridgenew-5.0.2/stocknotebridgenew.egg-info/PKG-INFO` & `stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocknotebridgenew
-Version: 5.0.2
+Version: 5.0.4
 Summary: official python library for Stocknote APIs
 Home-page: https://github.com/samco-sdk/Python-SDK
 Author: Samco Securities Limited
 Author-email: apisupport@samco.in
 License: MIT License
 Keywords: stocknote api,stocknote python sdk,samco api trading,samco algo trading,stock markets samco
 Platform: UNKNOWN
```

