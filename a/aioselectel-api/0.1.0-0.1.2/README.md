# Comparing `tmp/aioselectel_api-0.1.0.tar.gz` & `tmp/aioselectel_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioselectel_api-0.1.0.tar", max compression
+gzip compressed data, was "aioselectel_api-0.1.2.tar", max compression
```

## Comparing `aioselectel_api-0.1.0.tar` & `aioselectel_api-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      108 2024-05-29 13:38:37.189072 aioselectel_api-0.1.0/aioselectel_api/__init__.py
--rw-r--r--   0        0        0      253 2024-05-29 14:27:10.069940 aioselectel_api-0.1.0/aioselectel_api/base_client.py
--rw-r--r--   0        0        0     4010 2024-05-29 14:22:32.428777 aioselectel_api-0.1.0/aioselectel_api/client.py
--rw-r--r--   0        0        0       68 2024-05-29 12:17:08.937064 aioselectel_api-0.1.0/aioselectel_api/config.py
--rw-r--r--   0        0        0      245 2024-05-29 14:30:16.568405 aioselectel_api-0.1.0/aioselectel_api/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-29 08:00:51.477077 aioselectel_api-0.1.0/aioselectel_api/services/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 12:23:31.469560 aioselectel_api-0.1.0/aioselectel_api/services/object_storage.py
--rw-r--r--   0        0        0     1294 2024-05-29 12:12:59.656500 aioselectel_api-0.1.0/aioselectel_api/session.py
--rw-r--r--   0        0        0     1087 2024-05-29 13:39:24.195503 aioselectel_api-0.1.0/LICENSE
--rw-r--r--   0        0        0      438 2024-05-29 12:48:06.431291 aioselectel_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      222 2024-05-29 13:57:06.086715 aioselectel_api-0.1.0/README.md
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 aioselectel_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/LICENSE
+-rw-r--r--   0        0        0      394 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/README.md
+-rw-r--r--   0        0        0      105 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/base_client.py
+-rw-r--r--   0        0        0     5221 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/client.py
+-rw-r--r--   0        0        0       67 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/config.py
+-rw-r--r--   0        0        0      365 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/services/object_storage.py
+-rw-r--r--   0        0        0     1251 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/session.py
+-rw-r--r--   0        0        0      417 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 aioselectel_api-0.1.2/PKG-INFO
```

### Comparing `aioselectel_api-0.1.0/aioselectel_api/session.py` & `aioselectel_api-0.1.2/aioselectel_api/session.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import aiohttp
-
-
-class ClientCreatorContext:
-    def __init__(self, coro):
-        self._coro = coro
-        self._client = None
-
-    async def __aenter__(self):
-        self._client = await self._coro
-        return await self._client.__aenter__()
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self._client.__aexit__(exc_type, exc_val, exc_tb)
-
-
-class SelectelSession:
-    def __init__(self, base_url):
-        self.base_url = base_url
-        self.session = aiohttp.ClientSession()
-
-    async def __aenter__(self):
-        return self
-
-    async def __aexit__(self, exc_type, exc, tb):
-        await self.session.close()
-
-    async def request(self, method, path, **kwargs):
-        url = f"{self.base_url}{path}"
-        async with self.session.request(method, url, **kwargs) as response:
-            return response
-
-    async def get(self, path, **kwargs):
-        return await self.request("GET", path, **kwargs)
-
-    async def post(self, path, **kwargs):
-        return await self.request("POST", path, **kwargs)
-
-    async def put(self, path, **kwargs):
-        return await self.request("PUT", path, **kwargs)
-
-    async def delete(self, path, **kwargs):
-        return await self.request("DELETE", path, **kwargs)
+import aiohttp
+
+
+class ClientCreatorContext:
+    def __init__(self, coro):
+        self._coro = coro
+        self._client = None
+
+    async def __aenter__(self):
+        self._client = await self._coro
+        return await self._client.__aenter__()
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self._client.__aexit__(exc_type, exc_val, exc_tb)
+
+
+class SelectelSession:
+    def __init__(self, base_url):
+        self.base_url = base_url
+        self.session = aiohttp.ClientSession()
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, exc_type, exc, tb):
+        await self.session.close()
+
+    async def request(self, method, path, **kwargs):
+        url = f"{self.base_url}{path}"
+        async with self.session.request(method, url, **kwargs) as response:
+            return response
+
+    async def get(self, path, **kwargs):
+        return await self.request("GET", path, **kwargs)
+
+    async def post(self, path, **kwargs):
+        return await self.request("POST", path, **kwargs)
+
+    async def put(self, path, **kwargs):
+        return await self.request("PUT", path, **kwargs)
+
+    async def delete(self, path, **kwargs):
+        return await self.request("DELETE", path, **kwargs)
```

### Comparing `aioselectel_api-0.1.0/PKG-INFO` & `aioselectel_api-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioselectel-api
-Version: 0.1.0
+Version: 0.1.2
 Summary: 
 Author: azamtoiri
 Author-email: azamtoiri@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -15,9 +15,9 @@
 Requires-Dist: environs (>=11.0.0,<12.0.0)
 Requires-Dist: pytest (>=8.2.1,<9.0.0)
 Requires-Dist: pytest-asyncio (>=0.23.7,<0.24.0)
 Description-Content-Type: text/markdown
 
 # Selectel async API
 
-[![aioselectel_api](https://github.com/azamtoiri/aioselectel_api/actions/workflows/python-publish.yml/badge.svg)](https://github.com/azamtoiri/aioselectel_api/actions/workflows/python-publish.yml)
+[![Pylint](https://github.com/azamtoiri/aioselectel_api/actions/workflows/pylint.yml/badge.svg)](https://github.com/azamtoiri/aioselectel_api/actions/workflows/pylint.yml) [![aioselectel_api](https://github.com/azamtoiri/aioselectel_api/actions/workflows/python-publish.yml/badge.svg)](https://github.com/azamtoiri/aioselectel_api/actions/workflows/python-publish.yml)
```

