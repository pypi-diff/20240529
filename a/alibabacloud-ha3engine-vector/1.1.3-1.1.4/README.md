# Comparing `tmp/alibabacloud_ha3engine_vector-1.1.3.tar.gz` & `tmp/alibabacloud_ha3engine_vector-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ha3engine_vector-1.1.3.tar", last modified: Wed Mar 13 04:26:07 2024, max compression
+gzip compressed data, was "dist/alibabacloud_ha3engine_vector-1.1.4.tar", last modified: Wed May 29 08:50:40 2024, max compression
```

## Comparing `alibabacloud_ha3engine_vector-1.1.3.tar` & `alibabacloud_ha3engine_vector-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/
--rw-r--r--   0 root         (0) root         (0)      909 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/alibabacloud_ha3engine_vector/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/alibabacloud_ha3engine_vector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19093 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/alibabacloud_ha3engine_vector/client.py
--rw-r--r--   0 root         (0) root         (0)    17154 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/alibabacloud_ha3engine_vector/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/alibabacloud_ha3engine_vector.egg-info/
--rw-r--r--   0 root         (0) root         (0)      909 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/alibabacloud_ha3engine_vector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      394 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/alibabacloud_ha3engine_vector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/alibabacloud_ha3engine_vector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      171 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/alibabacloud_ha3engine_vector.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/alibabacloud_ha3engine_vector.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2646 2024-03-13 04:26:07.000000 alibabacloud_ha3engine_vector-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)      909 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/alibabacloud_ha3engine_vector/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/alibabacloud_ha3engine_vector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19157 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/alibabacloud_ha3engine_vector/client.py
+-rw-r--r--   0 root         (0) root         (0)    17154 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/alibabacloud_ha3engine_vector/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/alibabacloud_ha3engine_vector.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      909 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/alibabacloud_ha3engine_vector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/alibabacloud_ha3engine_vector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/alibabacloud_ha3engine_vector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/alibabacloud_ha3engine_vector.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/alibabacloud_ha3engine_vector.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2597 2024-05-29 08:50:40.000000 alibabacloud_ha3engine_vector-1.1.4/setup.py
```

### Comparing `alibabacloud_ha3engine_vector-1.1.3/PKG-INFO` & `alibabacloud_ha3engine_vector-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ha3engine_vector
-Version: 1.1.3
+Version: 1.1.4
 Summary: Alibaba Cloud Ha3engine-Vector SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-ha3-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,ha3engine,vector
```

### Comparing `alibabacloud_ha3engine_vector-1.1.3/alibabacloud_ha3engine_vector/client.py` & `alibabacloud_ha3engine_vector-1.1.4/alibabacloud_ha3engine_vector/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,34 +394,34 @@
         data_source_name: str,
         key_field: str,
         request: ha_3engine_vector_models.PushDocumentsRequest,
     ) -> ha_3engine_vector_models.PushDocumentsResponse:
         """
         支持新增、更新、删除 等操作，以及对应批量操作
         """
-        request.headers = {
+        request.headers = TeaCore.merge({
             'X-Opensearch-Swift-PK-Field': key_field
-        }
+        }, request.headers)
         return TeaCore.from_map(
             ha_3engine_vector_models.PushDocumentsResponse(),
             self._request('POST', f'/update/{data_source_name}/actions/bulk', None, request.headers, request.body, self.build_runtime_options())
         )
 
     async def push_documents_async(
         self,
         data_source_name: str,
         key_field: str,
         request: ha_3engine_vector_models.PushDocumentsRequest,
     ) -> ha_3engine_vector_models.PushDocumentsResponse:
         """
         支持新增、更新、删除 等操作，以及对应批量操作
         """
-        request.headers = {
+        request.headers = TeaCore.merge({
             'X-Opensearch-Swift-PK-Field': key_field
-        }
+        }, request.headers)
         return TeaCore.from_map(
             ha_3engine_vector_models.PushDocumentsResponse(),
             await self._request_async('POST', f'/update/{data_source_name}/actions/bulk', None, request.headers, request.body, await self.build_runtime_options_async())
         )
 
     def push_documents_with_swift(
         self,
```

### Comparing `alibabacloud_ha3engine_vector-1.1.3/alibabacloud_ha3engine_vector/models.py` & `alibabacloud_ha3engine_vector-1.1.4/alibabacloud_ha3engine_vector/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_ha3engine_vector-1.1.3/alibabacloud_ha3engine_vector.egg-info/PKG-INFO` & `alibabacloud_ha3engine_vector-1.1.4/alibabacloud_ha3engine_vector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ha3engine-vector
-Version: 1.1.3
+Version: 1.1.4
 Summary: Alibaba Cloud Ha3engine-Vector SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-ha3-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,ha3engine,vector
```

### Comparing `alibabacloud_ha3engine_vector-1.1.3/setup.py` & `alibabacloud_ha3engine_vector-1.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,31 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ha3engine_vector.
 
-Created on 13/03/2024
+Created on 29/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ha3engine_vector"
 NAME = "alibabacloud_ha3engine_vector" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Ha3engine-Vector SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-ha3-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
     "alibabacloud_darabonba_string>=0.0.4, <1.0.0",
-    "alibabacloud_darabonba_encode_util>=0.0.2, <1.0.0",
-    "alibabacloud_darabonba_map>=0.0.1, <1.0.0"
+    "alibabacloud_darabonba_encode_util>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

