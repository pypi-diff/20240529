# Comparing `tmp/stocknotebridgenew-5.0.4.tar.gz` & `tmp/stocknotebridgenew-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stocknotebridgenew-5.0.4.tar", last modified: Tue May 28 10:03:37 2024, max compression
+gzip compressed data, was "stocknotebridgenew-5.0.5.tar", last modified: Wed May 29 08:19:19 2024, max compression
```

## Comparing `stocknotebridgenew-5.0.4.tar` & `stocknotebridgenew-5.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 10:03:37.194451 stocknotebridgenew-5.0.4/
--rwxrwxrwx   0 root         (0) wheel        (0)     1082 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.4/LICENSE
--rwxrwxrwx   0 root         (0) wheel        (0)       25 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-28 10:03:37.194508 stocknotebridgenew-5.0.4/PKG-INFO
--rwxrwxrwx   0 root         (0) wheel        (0)    43188 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.4/README.md
--rwxrwxrwx   0 root         (0) wheel        (0)      108 2024-05-28 10:03:37.194723 stocknotebridgenew-5.0.4/setup.cfg
--rwxrwxrwx   0 root         (0) wheel        (0)      906 2024-05-28 10:03:33.000000 stocknotebridgenew-5.0.4/setup.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 10:03:37.192837 stocknotebridgenew-5.0.4/snapi_py_client/
--rwxrwxrwx   0 root         (0) wheel        (0)        0 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.4/snapi_py_client/__init__.py
--rwxrwxrwx   0 root         (0) wheel        (0)    26717 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.4/snapi_py_client/api_client.py
--rwxrwxrwx   0 root         (0) wheel        (0)     9294 2024-05-28 10:03:09.000000 stocknotebridgenew-5.0.4/snapi_py_client/configuration.py
--rwxrwxrwx   0 root         (0) wheel        (0)    14674 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.4/snapi_py_client/rest.py
--rwxrwxrwx   0 root         (0) wheel        (0)   236960 2024-05-28 07:32:47.000000 stocknotebridgenew-5.0.4/snapi_py_client/snapi_bridge.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-28 10:03:37.194342 stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/
--rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-28 10:03:37.000000 stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) wheel        (0)      404 2024-05-28 10:03:37.000000 stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) wheel        (0)        1 2024-05-28 10:03:37.000000 stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) wheel        (0)       37 2024-05-28 10:03:37.000000 stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/requires.txt
--rw-r--r--   0 root         (0) wheel        (0)       16 2024-05-28 10:03:37.000000 stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-29 08:19:19.521163 stocknotebridgenew-5.0.5/
+-rwxrwxrwx   0 root         (0) wheel        (0)     1082 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.5/LICENSE
+-rwxrwxrwx   0 root         (0) wheel        (0)       25 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-29 08:19:19.521362 stocknotebridgenew-5.0.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) wheel        (0)    43188 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.5/README.md
+-rwxrwxrwx   0 root         (0) wheel        (0)      108 2024-05-29 08:19:19.521644 stocknotebridgenew-5.0.5/setup.cfg
+-rwxrwxrwx   0 root         (0) wheel        (0)      906 2024-05-29 08:19:03.000000 stocknotebridgenew-5.0.5/setup.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-29 08:19:19.517283 stocknotebridgenew-5.0.5/snapi_py_client/
+-rwxrwxrwx   0 root         (0) wheel        (0)        0 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.5/snapi_py_client/__init__.py
+-rwxrwxrwx   0 root         (0) wheel        (0)    26717 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.5/snapi_py_client/api_client.py
+-rwxrwxrwx   0 root         (0) wheel        (0)     9294 2024-05-28 10:03:09.000000 stocknotebridgenew-5.0.5/snapi_py_client/configuration.py
+-rwxrwxrwx   0 root         (0) wheel        (0)    14674 2024-05-27 13:30:50.000000 stocknotebridgenew-5.0.5/snapi_py_client/rest.py
+-rwxrwxrwx   0 root         (0) wheel        (0)   236992 2024-05-29 08:18:26.000000 stocknotebridgenew-5.0.5/snapi_py_client/snapi_bridge.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2024-05-29 08:19:19.520986 stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/
+-rw-r--r--   0 root         (0) wheel        (0)      817 2024-05-29 08:19:19.000000 stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) wheel        (0)      404 2024-05-29 08:19:19.000000 stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) wheel        (0)        1 2024-05-29 08:19:19.000000 stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) wheel        (0)       37 2024-05-29 08:19:19.000000 stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/requires.txt
+-rw-r--r--   0 root         (0) wheel        (0)       16 2024-05-29 08:19:19.000000 stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/top_level.txt
```

### Comparing `stocknotebridgenew-5.0.4/LICENSE` & `stocknotebridgenew-5.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.4/PKG-INFO` & `stocknotebridgenew-5.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocknotebridgenew
-Version: 5.0.4
+Version: 5.0.5
 Summary: official python library for Stocknote APIs
 Home-page: https://github.com/samco-sdk/Python-SDK
 Author: Samco Securities Limited
 Author-email: apisupport@samco.in
 License: MIT License
 Keywords: stocknote api,stocknote python sdk,samco api trading,samco algo trading,stock markets samco
 Platform: UNKNOWN
```

### Comparing `stocknotebridgenew-5.0.4/README.md` & `stocknotebridgenew-5.0.5/README.md`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.4/setup.py` & `stocknotebridgenew-5.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='stocknotebridgenew',
-version='5.0.4',
+version='5.0.5',
 description='official python library for Stocknote APIs',
 url='https://github.com/samco-sdk/Python-SDK',
 install_requires=['future', 'requests','websocket-client','six'],
 author='Samco Securities Limited',
 author_email='apisupport@samco.in',
 license='MIT License',
 packages=['snapi_py_client'],
```

### Comparing `stocknotebridgenew-5.0.4/snapi_py_client/api_client.py` & `stocknotebridgenew-5.0.5/snapi_py_client/api_client.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.4/snapi_py_client/configuration.py` & `stocknotebridgenew-5.0.5/snapi_py_client/configuration.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.4/snapi_py_client/rest.py` & `stocknotebridgenew-5.0.5/snapi_py_client/rest.py`

 * *Files identical despite different names*

### Comparing `stocknotebridgenew-5.0.4/snapi_py_client/snapi_bridge.py` & `stocknotebridgenew-5.0.5/snapi_py_client/snapi_bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1158,25 +1158,26 @@
             raise ValueError("Missing the required parameter `x_session_token` when calling `market_depth`")
     
         # Set up header parameters
         header_params = {'x-session-token': x_session_token, 'Accept': 'application/json', 'Content-Type': 'application/json'}
 
         # Set up body parameters if provided
         body_params = kwargs.get('body')
+        print(body_params)
 
         # API call
         return self.api_client.call_api(
             '/quote/multiQuote', 'POST',
             path_params={},
             query_params=[],
             header_params=header_params,
             body=body_params,
             post_params=[],
             files={},
-            response_type='AddGttResponse',
+            response_type='multiQuoteResponse',
             auth_settings=[],
             async_req=kwargs.get('async_req'),
             _return_http_data_only=kwargs.get('_return_http_data_only'),
             _preload_content=kwargs.get('_preload_content', True),
             _request_timeout=kwargs.get('_request_timeout'),
             collection_formats={}
         )
```

### Comparing `stocknotebridgenew-5.0.4/stocknotebridgenew.egg-info/PKG-INFO` & `stocknotebridgenew-5.0.5/stocknotebridgenew.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocknotebridgenew
-Version: 5.0.4
+Version: 5.0.5
 Summary: official python library for Stocknote APIs
 Home-page: https://github.com/samco-sdk/Python-SDK
 Author: Samco Securities Limited
 Author-email: apisupport@samco.in
 License: MIT License
 Keywords: stocknote api,stocknote python sdk,samco api trading,samco algo trading,stock markets samco
 Platform: UNKNOWN
```

