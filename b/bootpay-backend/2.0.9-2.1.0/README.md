# Comparing `tmp/bootpay_backend-2.0.9.tar.gz` & `tmp/bootpay_backend-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootpay_backend-2.0.9.tar", last modified: Mon May 27 07:43:49 2024, max compression
+gzip compressed data, was "bootpay_backend-2.1.0.tar", last modified: Wed May 29 07:46:31 2024, max compression
```

## Comparing `bootpay_backend-2.0.9.tar` & `bootpay_backend-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 taesupyoon   (501) staff       (20)        0 2024-05-27 07:43:49.927452 bootpay_backend-2.0.9/
--rw-r--r--   0 taesupyoon   (501) staff       (20)     1063 2024-05-27 06:11:15.000000 bootpay_backend-2.0.9/LICENSE
--rw-r--r--   0 taesupyoon   (501) staff       (20)    14273 2024-05-27 07:43:49.927297 bootpay_backend-2.0.9/PKG-INFO
--rw-r--r--   0 taesupyoon   (501) staff       (20)    12917 2024-05-27 06:11:15.000000 bootpay_backend-2.0.9/README.md
-drwxr-xr-x   0 taesupyoon   (501) staff       (20)        0 2024-05-27 07:43:49.925871 bootpay_backend-2.0.9/bootpay_backend/
--rw-r--r--   0 taesupyoon   (501) staff       (20)       70 2024-05-27 06:11:15.000000 bootpay_backend-2.0.9/bootpay_backend/__init__.py
--rw-r--r--   0 taesupyoon   (501) staff       (20)      447 2024-05-27 06:11:15.000000 bootpay_backend-2.0.9/bootpay_backend/bankcode.py
--rw-r--r--   0 taesupyoon   (501) staff       (20)    14014 2024-05-27 07:12:15.000000 bootpay_backend-2.0.9/bootpay_backend/rest_client.py
-drwxr-xr-x   0 taesupyoon   (501) staff       (20)        0 2024-05-27 07:43:49.927068 bootpay_backend-2.0.9/bootpay_backend.egg-info/
--rw-r--r--   0 taesupyoon   (501) staff       (20)    14273 2024-05-27 07:43:49.000000 bootpay_backend-2.0.9/bootpay_backend.egg-info/PKG-INFO
--rw-r--r--   0 taesupyoon   (501) staff       (20)      355 2024-05-27 07:43:49.000000 bootpay_backend-2.0.9/bootpay_backend.egg-info/SOURCES.txt
--rw-r--r--   0 taesupyoon   (501) staff       (20)        1 2024-05-27 07:43:49.000000 bootpay_backend-2.0.9/bootpay_backend.egg-info/dependency_links.txt
--rw-r--r--   0 taesupyoon   (501) staff       (20)        1 2024-05-27 07:43:49.000000 bootpay_backend-2.0.9/bootpay_backend.egg-info/not-zip-safe
--rw-r--r--   0 taesupyoon   (501) staff       (20)       95 2024-05-27 07:43:49.000000 bootpay_backend-2.0.9/bootpay_backend.egg-info/requires.txt
--rw-r--r--   0 taesupyoon   (501) staff       (20)       16 2024-05-27 07:43:49.000000 bootpay_backend-2.0.9/bootpay_backend.egg-info/top_level.txt
--rw-r--r--   0 taesupyoon   (501) staff       (20)       79 2024-05-27 07:43:49.927633 bootpay_backend-2.0.9/setup.cfg
--rw-r--r--   0 taesupyoon   (501) staff       (20)     1833 2024-05-27 07:40:44.000000 bootpay_backend-2.0.9/setup.py
+drwxr-xr-x   0 taesupyoon   (501) staff       (20)        0 2024-05-29 07:46:31.012117 bootpay_backend-2.1.0/
+-rw-r--r--   0 taesupyoon   (501) staff       (20)     1063 2024-05-27 06:11:15.000000 bootpay_backend-2.1.0/LICENSE
+-rw-r--r--   0 taesupyoon   (501) staff       (20)    14273 2024-05-29 07:46:31.011983 bootpay_backend-2.1.0/PKG-INFO
+-rw-r--r--   0 taesupyoon   (501) staff       (20)    12917 2024-05-27 06:11:15.000000 bootpay_backend-2.1.0/README.md
+drwxr-xr-x   0 taesupyoon   (501) staff       (20)        0 2024-05-29 07:46:31.010570 bootpay_backend-2.1.0/bootpay_backend/
+-rw-r--r--   0 taesupyoon   (501) staff       (20)       70 2024-05-27 06:11:15.000000 bootpay_backend-2.1.0/bootpay_backend/__init__.py
+-rw-r--r--   0 taesupyoon   (501) staff       (20)      447 2024-05-27 06:11:15.000000 bootpay_backend-2.1.0/bootpay_backend/bankcode.py
+-rw-r--r--   0 taesupyoon   (501) staff       (20)    15057 2024-05-29 07:40:08.000000 bootpay_backend-2.1.0/bootpay_backend/rest_client.py
+drwxr-xr-x   0 taesupyoon   (501) staff       (20)        0 2024-05-29 07:46:31.011753 bootpay_backend-2.1.0/bootpay_backend.egg-info/
+-rw-r--r--   0 taesupyoon   (501) staff       (20)    14273 2024-05-29 07:46:30.000000 bootpay_backend-2.1.0/bootpay_backend.egg-info/PKG-INFO
+-rw-r--r--   0 taesupyoon   (501) staff       (20)      355 2024-05-29 07:46:30.000000 bootpay_backend-2.1.0/bootpay_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 taesupyoon   (501) staff       (20)        1 2024-05-29 07:46:30.000000 bootpay_backend-2.1.0/bootpay_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 taesupyoon   (501) staff       (20)        1 2024-05-27 07:43:49.000000 bootpay_backend-2.1.0/bootpay_backend.egg-info/not-zip-safe
+-rw-r--r--   0 taesupyoon   (501) staff       (20)       95 2024-05-29 07:46:30.000000 bootpay_backend-2.1.0/bootpay_backend.egg-info/requires.txt
+-rw-r--r--   0 taesupyoon   (501) staff       (20)       16 2024-05-29 07:46:30.000000 bootpay_backend-2.1.0/bootpay_backend.egg-info/top_level.txt
+-rw-r--r--   0 taesupyoon   (501) staff       (20)       79 2024-05-29 07:46:31.012301 bootpay_backend-2.1.0/setup.cfg
+-rw-r--r--   0 taesupyoon   (501) staff       (20)     1833 2024-05-29 07:40:14.000000 bootpay_backend-2.1.0/setup.py
```

### Comparing `bootpay_backend-2.0.9/LICENSE` & `bootpay_backend-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bootpay_backend-2.0.9/PKG-INFO` & `bootpay_backend-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootpay-backend
-Version: 2.0.9
+Version: 2.1.0
 Summary: bootpay server side plugin for python
 Home-page: https://github.com/bootpay/backend-python/tree/2-x-development
 Author: bootpay <bootpay.co.kr@gmail.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bootpay_backend-2.0.9/README.md` & `bootpay_backend-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bootpay_backend-2.0.9/bootpay_backend/rest_client.py` & `bootpay_backend-2.1.0/bootpay_backend/rest_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class BootpayBackend:
     BASE_URL = {
         'development': 'https://dev-api.bootpay.co.kr/v2',
         'stage': 'https://stage-api.bootpay.co.kr/v2',
         'production': 'https://api.bootpay.co.kr/v2'
     }
     API_VERSION = '5.0.0'
-    SDK_VERSION = '2.0.9'
+    SDK_VERSION = '2.1.0'
 
     def __init__(self, application_id, private_key, mode='production'):
         self.application_id = application_id
         self.private_key = private_key
         self.mode = mode
         self.token = None
         self.api_version = self.API_VERSION
@@ -112,26 +112,49 @@
             "user": user,
             "metadata": metadata
         })
 
     # request subscribe card payment
     # Comment by GOSOMI
     def request_subscribe_card_payment(self, billing_key='', order_name='', price=0, tax_free=0, card_quota='00',
-                                       card_interest=None, order_id='', items=None, user=None, extra=None):
+                                       card_interest=None, order_id='', items=None, user=None, extra=None,
+                                       feedback_url=None, content_type=None):
         return self.__request(method='post', url=self.__entrypoints('subscribe/payment'), data={
             "billing_key": billing_key,
             "order_name": order_name,
             "price": price,
             "tax_free": tax_free,
             "card_quota": card_quota,
             "card_interest": card_interest,
             "order_id": order_id,
             "items": items,
             "user": user,
-            "extra": extra
+            "extra": extra,
+            "feedback_url": feedback_url,
+            "content_type": content_type
+        })
+
+    # request subscribe payment
+    # Comment by ehowlsla
+    def request_subscribe_payment(self, billing_key='', order_name='', price=0, tax_free=0, card_quota='00',
+                                       card_interest=None, order_id='', items=None, user=None, extra=None,
+                                       feedback_url=None, content_type=None):
+        return self.__request(method='post', url=self.__entrypoints('subscribe/payment'), data={
+            "billing_key": billing_key,
+            "order_name": order_name,
+            "price": price,
+            "tax_free": tax_free,
+            "card_quota": card_quota,
+            "card_interest": card_interest,
+            "order_id": order_id,
+            "items": items,
+            "user": user,
+            "extra": extra,
+            "feedback_url": feedback_url,
+            "content_type": content_type
         })
 
     # destroy billing key
     # Comment by GOSOMI
     def destroy_billing_key(self, billing_key=''):
         return self.__request(method='delete', url=self.__entrypoints(f'subscribe/billing_key/{billing_key}'))
```

### Comparing `bootpay_backend-2.0.9/bootpay_backend.egg-info/PKG-INFO` & `bootpay_backend-2.1.0/bootpay_backend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootpay-backend
-Version: 2.0.9
+Version: 2.1.0
 Summary: bootpay server side plugin for python
 Home-page: https://github.com/bootpay/backend-python/tree/2-x-development
 Author: bootpay <bootpay.co.kr@gmail.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bootpay_backend-2.0.9/setup.py` & `bootpay_backend-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name = 'bootpay-backend',
-    version = '2.0.9',
+    version = '2.1.0',
     description = 'bootpay server side plugin for python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'bootpay <bootpay.co.kr@gmail.com>',
     packages = setuptools.find_packages(),
     keyword = ['pg', '결제연동', 'bootpay', 'payment'],
     install_requires=[
```

