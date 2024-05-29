# Comparing `tmp/valorantstore-5.0.0.0.tar.gz` & `tmp/valorantstore-6.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valorantstore-5.0.0.0.tar", last modified: Mon Apr 29 19:30:39 2024, max compression
+gzip compressed data, was "valorantstore-6.0.0.0.tar", last modified: Wed May 29 13:54:41 2024, max compression
```

## Comparing `valorantstore-5.0.0.0.tar` & `valorantstore-6.0.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 19:30:39.085384 valorantstore-5.0.0.0/
--rw-rw-rw-   0        0        0     1091 2023-08-14 12:55:11.000000 valorantstore-5.0.0.0/LICENSE
--rw-rw-rw-   0        0        0    19053 2024-04-29 19:30:39.084378 valorantstore-5.0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    18457 2024-04-29 19:18:21.000000 valorantstore-5.0.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 19:30:39.085384 valorantstore-5.0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      912 2024-04-29 19:24:05.000000 valorantstore-5.0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 19:30:39.074818 valorantstore-5.0.0.0/valorantstore/
--rw-rw-rw-   0        0        0    14421 2024-04-29 19:24:05.000000 valorantstore-5.0.0.0/valorantstore/ValorantStore.py
--rw-rw-rw-   0        0        0      364 2023-08-14 14:17:39.000000 valorantstore-5.0.0.0/valorantstore/ValorantStoreException.py
--rw-rw-rw-   0        0        0      128 2023-08-14 14:17:39.000000 valorantstore-5.0.0.0/valorantstore/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 19:30:39.082882 valorantstore-5.0.0.0/valorantstore.egg-info/
--rw-rw-rw-   0        0        0    19053 2024-04-29 19:30:39.000000 valorantstore-5.0.0.0/valorantstore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-04-29 19:30:39.000000 valorantstore-5.0.0.0/valorantstore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 19:30:39.000000 valorantstore-5.0.0.0/valorantstore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-29 19:30:39.000000 valorantstore-5.0.0.0/valorantstore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-29 19:30:39.000000 valorantstore-5.0.0.0/valorantstore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 13:54:41.640801 valorantstore-6.0.0.0/
+-rw-rw-rw-   0        0        0     1091 2024-05-14 22:37:14.000000 valorantstore-6.0.0.0/LICENSE
+-rw-rw-rw-   0        0        0    19053 2024-05-29 13:54:41.640801 valorantstore-6.0.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    18457 2024-05-14 22:37:14.000000 valorantstore-6.0.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 13:54:41.640801 valorantstore-6.0.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      912 2024-05-29 13:54:16.000000 valorantstore-6.0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:54:41.635781 valorantstore-6.0.0.0/valorantstore/
+-rw-rw-rw-   0        0        0    15085 2024-05-14 22:37:14.000000 valorantstore-6.0.0.0/valorantstore/ValorantStore.py
+-rw-rw-rw-   0        0        0      364 2024-05-14 22:37:14.000000 valorantstore-6.0.0.0/valorantstore/ValorantStoreException.py
+-rw-rw-rw-   0        0        0      128 2024-05-14 22:37:14.000000 valorantstore-6.0.0.0/valorantstore/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:54:41.639802 valorantstore-6.0.0.0/valorantstore.egg-info/
+-rw-rw-rw-   0        0        0    19053 2024-05-29 13:54:41.000000 valorantstore-6.0.0.0/valorantstore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-05-29 13:54:41.000000 valorantstore-6.0.0.0/valorantstore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 13:54:41.000000 valorantstore-6.0.0.0/valorantstore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-29 13:54:41.000000 valorantstore-6.0.0.0/valorantstore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-29 13:54:41.000000 valorantstore-6.0.0.0/valorantstore.egg-info/top_level.txt
```

### Comparing `valorantstore-5.0.0.0/LICENSE` & `valorantstore-6.0.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valorantstore-5.0.0.0/PKG-INFO` & `valorantstore-6.0.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valorantstore
-Version: 5.0.0.0
+Version: 6.0.0.0
 Summary: Python module to display your Valorant store
 Home-page: https://github.com/mahelbir/valorant-store
 Author: Mahmuthan Elbir
 Author-email: me@mahmuthanelbir.com.tr
 License: MIT
 Keywords: valorant store,valorant api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `valorantstore-5.0.0.0/README.md` & `valorantstore-6.0.0.0/README.md`

 * *Files identical despite different names*

### Comparing `valorantstore-5.0.0.0/setup.py` & `valorantstore-6.0.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 pkg_name = "valorantstore"
 setuptools.setup(
     name=pkg_name,
-    version="5.0.0.0",
+    version="6.0.0.0",
     author="Mahmuthan Elbir",
     author_email="me@mahmuthanelbir.com.tr",
     description="Python module to display your Valorant store",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['valorant store', 'valorant api'],
     license="MIT",
```

### Comparing `valorantstore-5.0.0.0/valorantstore/ValorantStore.py` & `valorantstore-6.0.0.0/valorantstore/ValorantStore.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 import base64
 import json
 import pickle
 from os import path, getcwd, remove, mkdir
 from time import time
 
+import ssl
+from requests.adapters import HTTPAdapter
+from urllib3.poolmanager import PoolManager
 import cfscrape
 import requests
 
 from valorantstore.ValorantStoreException import ValorantStoreException
 
+class TLSv1_2Adapter(HTTPAdapter):
+    def init_poolmanager(self, connections, maxsize, block=False, **pool_kwargs):
+        context = ssl.SSLContext(ssl.PROTOCOL_TLS)
+        context.options |= ssl.OP_NO_TLSv1 | ssl.OP_NO_TLSv1_1 | ssl.OP_NO_TLSv1_3 | ssl.OP_NO_SSLv2 | ssl.OP_NO_SSLv3
+        #Only allow TLSv1.2(只允許TLSv1.2)
+        self.poolmanager = PoolManager(num_pools=connections, maxsize=maxsize, block=block, ssl_context=context, **pool_kwargs)
 
 class ValorantStore:
     __auth = {}
 
     def __init__(self, username: str, password: str, region: str = "eu", sess_path: str = None, proxy=None):
         self.__username = username.lower().strip()
         self.__password = password
@@ -137,14 +146,15 @@
 
     @property
     def cookie_file(self) -> str:
         return self.__cookie_file
 
     def __login(self):
         scraper = cfscrape.create_scraper()
+        scraper.mount('https://', TLSv1_2Adapter())
         if self.__proxy:
             scraper.proxies = {
                 'http': self.__proxy,
                 'https': self.__proxy,
             }
         if path.isfile(self.__cookie_file):
             try:
@@ -163,15 +173,16 @@
                 remove(self.__cookie_file)
                 return self.__login()
         else:
             cookie_response = scraper.post("https://auth.riotgames.com/api/v1/authorization", json={
                 "client_id": "play-valorant-web-prod",
                 "nonce": "1",
                 "redirect_uri": "https://playvalorant.com/opt_in",
-                "response_type": "token id_token"
+                "response_type": "token id_token",
+                "scope": "account openid"
             }, timeout=15)
             try:
                 cookie = cookie_response.json()
             except Exception:
                 raise ValorantStoreException("cookie", "request", cookie_response)
             if "type" not in cookie:
                 raise ValorantStoreException("cookie", "request", cookie_response)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `valorantstore-5.0.0.0/valorantstore.egg-info/PKG-INFO` & `valorantstore-6.0.0.0/valorantstore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valorantstore
-Version: 5.0.0.0
+Version: 6.0.0.0
 Summary: Python module to display your Valorant store
 Home-page: https://github.com/mahelbir/valorant-store
 Author: Mahmuthan Elbir
 Author-email: me@mahmuthanelbir.com.tr
 License: MIT
 Keywords: valorant store,valorant api
 Classifier: Programming Language :: Python :: 3
```

