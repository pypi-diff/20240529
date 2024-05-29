# Comparing `tmp/alibabacloud_gateway_pop_py2-0.0.3.tar.gz` & `tmp/alibabacloud_gateway_pop_py2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gateway_pop_py2-0.0.3.tar", last modified: Wed Mar  6 14:38:09 2024, max compression
+gzip compressed data, was "dist/alibabacloud_gateway_pop_py2-0.0.4.tar", last modified: Wed May 29 12:02:32 2024, max compression
```

## Comparing `alibabacloud_gateway_pop_py2-0.0.3.tar` & `alibabacloud_gateway_pop_py2-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 14:38:09.000000 alibabacloud_gateway_pop_py2-0.0.3/
--rw-r--r--   0 root         (0) root         (0)     1020 2024-03-06 14:38:09.000000 alibabacloud_gateway_pop_py2-0.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 14:38:09.000000 alibabacloud_gateway_pop_py2-0.0.3/alibabacloud_gateway_pop/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-06 14:38:08.000000 alibabacloud_gateway_pop_py2-0.0.3/alibabacloud_gateway_pop/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13591 2024-03-06 14:38:08.000000 alibabacloud_gateway_pop_py2-0.0.3/alibabacloud_gateway_pop/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 14:38:09.000000 alibabacloud_gateway_pop_py2-0.0.3/alibabacloud_gateway_pop_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1020 2024-03-06 14:38:09.000000 alibabacloud_gateway_pop_py2-0.0.3/alibabacloud_gateway_pop_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      339 2024-03-06 14:38:09.000000 alibabacloud_gateway_pop_py2-0.0.3/alibabacloud_gateway_pop_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-06 14:38:09.000000 alibabacloud_gateway_pop_py2-0.0.3/alibabacloud_gateway_pop_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      464 2024-03-06 14:38:09.000000 alibabacloud_gateway_pop_py2-0.0.3/alibabacloud_gateway_pop_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-06 14:38:09.000000 alibabacloud_gateway_pop_py2-0.0.3/alibabacloud_gateway_pop_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-06 14:38:09.000000 alibabacloud_gateway_pop_py2-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3230 2024-03-06 14:38:08.000000 alibabacloud_gateway_pop_py2-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:02:32.000000 alibabacloud_gateway_pop_py2-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-29 12:02:32.000000 alibabacloud_gateway_pop_py2-0.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:02:32.000000 alibabacloud_gateway_pop_py2-0.0.4/alibabacloud_gateway_pop/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 12:02:31.000000 alibabacloud_gateway_pop_py2-0.0.4/alibabacloud_gateway_pop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14215 2024-05-29 12:02:31.000000 alibabacloud_gateway_pop_py2-0.0.4/alibabacloud_gateway_pop/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:02:32.000000 alibabacloud_gateway_pop_py2-0.0.4/alibabacloud_gateway_pop_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-29 12:02:32.000000 alibabacloud_gateway_pop_py2-0.0.4/alibabacloud_gateway_pop_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      339 2024-05-29 12:02:32.000000 alibabacloud_gateway_pop_py2-0.0.4/alibabacloud_gateway_pop_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 12:02:32.000000 alibabacloud_gateway_pop_py2-0.0.4/alibabacloud_gateway_pop_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-29 12:02:32.000000 alibabacloud_gateway_pop_py2-0.0.4/alibabacloud_gateway_pop_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-29 12:02:32.000000 alibabacloud_gateway_pop_py2-0.0.4/alibabacloud_gateway_pop_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 12:02:32.000000 alibabacloud_gateway_pop_py2-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3230 2024-05-29 12:02:31.000000 alibabacloud_gateway_pop_py2-0.0.4/setup.py
```

### Comparing `alibabacloud_gateway_pop_py2-0.0.3/PKG-INFO` & `alibabacloud_gateway_pop_py2-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gateway_pop_py2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Alibaba Cloud POP SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,pop,py2
```

### Comparing `alibabacloud_gateway_pop_py2-0.0.3/alibabacloud_gateway_pop/client.py` & `alibabacloud_gateway_pop_py2-0.0.4/alibabacloud_gateway_pop/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,25 +66,36 @@
                     request.headers['content-type'] = 'application/x-www-form-urlencoded'
         if UtilClient.equal_string(signature_algorithm, self._sm_3):
             request.headers['x-acs-content-sm3'] = hashed_request_payload
         else:
             request.headers['x-acs-content-sha256'] = hashed_request_payload
         if not UtilClient.equal_string(request.auth_type, 'Anonymous'):
             credential = request.credential
-            access_key_id = credential.get_access_key_id()
-            access_key_secret = credential.get_access_key_secret()
-            security_token = credential.get_security_token()
-            if not UtilClient.empty(security_token):
-                request.headers['x-acs-accesskey-id'] = access_key_id
-                request.headers['x-acs-security-token'] = security_token
-            date_new = StringClient.sub_string(date, 0, 10)
-            date_new = StringClient.replace(date_new, '-', '', None)
-            region = self.get_region(request.product_id, config.endpoint)
-            signingkey = self.get_signingkey(signature_algorithm, access_key_secret, request.product_id, region, date_new)
-            request.headers['Authorization'] = self.get_authorization(request.pathname, request.method, request.query, request.headers, signature_algorithm, hashed_request_payload, access_key_id, signingkey, request.product_id, region, date_new)
+            if UtilClient.is_unset(credential):
+                raise TeaException({
+                    'code': 'ParameterMissing',
+                    'message': "'config.credential' can not be unset"
+                })
+            auth_type = credential.get_type()
+            if UtilClient.equal_string(auth_type, 'bearer'):
+                bearer_token = credential.get_bearer_token()
+                request.headers['x-acs-bearer-token'] = bearer_token
+                request.headers['Authorization'] = 'Bearer %s' % TeaConverter.to_unicode(bearer_token)
+            else:
+                access_key_id = credential.get_access_key_id()
+                access_key_secret = credential.get_access_key_secret()
+                security_token = credential.get_security_token()
+                if not UtilClient.empty(security_token):
+                    request.headers['x-acs-accesskey-id'] = access_key_id
+                    request.headers['x-acs-security-token'] = security_token
+                date_new = StringClient.sub_string(date, 0, 10)
+                date_new = StringClient.replace(date_new, '-', '', None)
+                region = self.get_region(request.product_id, config.endpoint)
+                signingkey = self.get_signingkey(signature_algorithm, access_key_secret, request.product_id, region, date_new)
+                request.headers['Authorization'] = self.get_authorization(request.pathname, request.method, request.query, request.headers, signature_algorithm, hashed_request_payload, access_key_id, signingkey, request.product_id, region, date_new)
 
     def modify_response(self, context, attribute_map):
         request = context.request
         response = context.response
         if UtilClient.is_4xx(response.status_code) or UtilClient.is_5xx(response.status_code):
             _res = UtilClient.read_as_json(response.body)
             err = UtilClient.assert_as_map(_res)
```

### Comparing `alibabacloud_gateway_pop_py2-0.0.3/alibabacloud_gateway_pop_py2.egg-info/PKG-INFO` & `alibabacloud_gateway_pop_py2-0.0.4/alibabacloud_gateway_pop_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gateway-pop-py2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Alibaba Cloud POP SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,pop,py2
```

### Comparing `alibabacloud_gateway_pop_py2-0.0.3/setup.py` & `alibabacloud_gateway_pop_py2-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gateway_pop_py2.
 
-Created on 06/03/2024
+Created on 29/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gateway_pop"
 NAME = "alibabacloud_gateway_pop_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud POP SDK Library for Python2"
```

