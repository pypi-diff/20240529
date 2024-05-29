# Comparing `tmp/zyte_api-0.5.2.tar.gz` & `tmp/zyte_api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyte_api-0.5.2.tar", last modified: Fri May 10 15:20:09 2024, max compression
+gzip compressed data, was "zyte_api-0.6.0.tar", last modified: Wed May 29 13:50:37 2024, max compression
```

## Comparing `zyte_api-0.5.2.tar` & `zyte_api-0.6.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:09.593583 zyte_api-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-10 15:19:57.000000 zyte_api-0.5.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-10 15:19:57.000000 zyte_api-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-10 15:19:57.000000 zyte_api-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-10 15:20:09.593583 zyte_api-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-10 15:19:57.000000 zyte_api-0.5.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-10 15:19:57.000000 zyte_api-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-10 15:20:09.593583 zyte_api-0.5.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-05-10 15:19:57.000000 zyte_api-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:09.589583 zyte_api-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/mockserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     8269 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:09.589583 zyte_api-0.5.2/zyte_api/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:09.593583 zyte_api-0.5.2/zyte_api/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/aio/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/aio/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/apikey.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:09.593583 zyte_api-0.5.2/zyte_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-10 15:20:09.000000 zyte_api-0.5.2/zyte_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 15:20:09.000000 zyte_api-0.5.2/zyte_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:20:09.000000 zyte_api-0.5.2/zyte_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 15:20:09.000000 zyte_api-0.5.2/zyte_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-10 15:20:09.000000 zyte_api-0.5.2/zyte_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 15:20:09.000000 zyte_api-0.5.2/zyte_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:37.481418 zyte_api-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-29 13:50:29.000000 zyte_api-0.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-29 13:50:29.000000 zyte_api-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-29 13:50:29.000000 zyte_api-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-29 13:50:37.481418 zyte_api-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-29 13:50:29.000000 zyte_api-0.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-29 13:50:29.000000 zyte_api-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-29 13:50:37.481418 zyte_api-0.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-05-29 13:50:29.000000 zyte_api-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:37.477418 zyte_api-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:29.000000 zyte_api-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 13:50:29.000000 zyte_api-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-29 13:50:29.000000 zyte_api-0.6.0/tests/mockserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-05-29 13:50:29.000000 zyte_api-0.6.0/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8269 2024-05-29 13:50:29.000000 zyte_api-0.6.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15076 2024-05-29 13:50:29.000000 zyte_api-0.6.0/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-05-29 13:50:29.000000 zyte_api-0.6.0/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-29 13:50:29.000000 zyte_api-0.6.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:37.477418 zyte_api-0.6.0/zyte_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:37.481418 zyte_api-0.6.0/zyte_api/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/aio/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/aio/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/apikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-29 13:50:29.000000 zyte_api-0.6.0/zyte_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:50:37.481418 zyte_api-0.6.0/zyte_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-29 13:50:37.000000 zyte_api-0.6.0/zyte_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-29 13:50:37.000000 zyte_api-0.6.0/zyte_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:50:37.000000 zyte_api-0.6.0/zyte_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-29 13:50:37.000000 zyte_api-0.6.0/zyte_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-29 13:50:37.000000 zyte_api-0.6.0/zyte_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 13:50:37.000000 zyte_api-0.6.0/zyte_api.egg-info/top_level.txt
```

### Comparing `zyte_api-0.5.2/LICENSE` & `zyte_api-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/PKG-INFO` & `zyte_api-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-api
-Version: 0.5.2
+Version: 0.6.0
 Summary: Python interface to Zyte API
 Home-page: https://github.com/zytedata/python-zyte-api
 Author: Zyte Group Ltd
 Author-email: opensource@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte_api-0.5.2/README.rst` & `zyte_api-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/setup.py` & `zyte_api-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/tests/mockserver.py` & `zyte_api-0.6.0/tests/mockserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 
         url = request_data["url"]
         domain = urlparse(url).netloc
         if domain == "e429.example":
             request.setResponseCode(429)
             response_data = {"status": 429, "type": "/limits/over-user-limit"}
             return json.dumps(response_data).encode()
+        if domain == "e500.example":
+            request.setResponseCode(500)
+            return ""
         if domain == "e520.example":
             request.setResponseCode(520)
             response_data = {"status": 520, "type": "/download/temporary-error"}
             return json.dumps(response_data).encode()
         if domain == "e521.example":
             request.setResponseCode(521)
             response_data = {"status": 521, "type": "/download/internal-error"}
```

### Comparing `zyte_api-0.5.2/tests/test_async.py` & `zyte_api-0.6.0/tests/test_async.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import asyncio
 from unittest.mock import AsyncMock
 
 import pytest
-from tenacity import AsyncRetrying
 
-from zyte_api import AsyncZyteAPI, RequestError
-from zyte_api._retry import RetryFactory
+from zyte_api import AggressiveRetryFactory, AsyncZyteAPI, RequestError
 from zyte_api.aio.client import AsyncClient
 from zyte_api.apikey import NoApiKey
 from zyte_api.errors import ParsedError
 from zyte_api.utils import USER_AGENT
 
-from .mockserver import DropResource, MockServer
-
 
 @pytest.mark.parametrize(
     ("client_cls",),
     (
         (AsyncZyteAPI,),
         (AsyncClient,),
     ),
@@ -68,54 +64,14 @@
     }
     actual_result = await getattr(client, get_method)(
         {"url": "https://a.example", "httpResponseBody": True}
     )
     assert actual_result == expected_result
 
 
-UNSET = object()
-
-
-class OutlierException(RuntimeError):
-    pass
-
-
-@pytest.mark.parametrize(
-    ("client_cls", "get_method"),
-    (
-        (AsyncZyteAPI, "get"),
-        (AsyncClient, "request_raw"),
-    ),
-)
-@pytest.mark.parametrize(
-    ("value", "exception"),
-    (
-        (UNSET, OutlierException),
-        (True, OutlierException),
-        (False, RequestError),
-    ),
-)
-@pytest.mark.asyncio
-async def test_get_handle_retries(client_cls, get_method, value, exception, mockserver):
-    kwargs = {}
-    if value is not UNSET:
-        kwargs["handle_retries"] = value
-
-    def broken_stop(_):
-        raise OutlierException
-
-    retrying = AsyncRetrying(stop=broken_stop)
-    client = client_cls(api_key="a", api_url=mockserver.urljoin("/"), retrying=retrying)
-    with pytest.raises(exception):
-        await getattr(client, get_method)(
-            {"url": "https://exception.example", "browserHtml": True},
-            **kwargs,
-        )
-
-
 @pytest.mark.parametrize(
     ("client_cls", "get_method"),
     (
         (AsyncZyteAPI, "get"),
         (AsyncClient, "request_raw"),
     ),
 )
@@ -231,140 +187,14 @@
         if isinstance(actual_result, Exception):
             assert Exception in expected_results
         else:
             assert actual_result in expected_results
 
 
 @pytest.mark.parametrize(
-    ("client_cls", "get_method"),
-    (
-        (AsyncZyteAPI, "get"),
-        (AsyncClient, "request_raw"),
-    ),
-)
-@pytest.mark.parametrize(
-    ("subdomain", "waiter"),
-    (
-        ("e429", "throttling"),
-        ("e520", "temporary_download_error"),
-    ),
-)
-@pytest.mark.asyncio
-async def test_retry_wait(client_cls, get_method, subdomain, waiter, mockserver):
-    def broken_wait(self, retry_state):
-        raise OutlierException
-
-    class CustomRetryFactory(RetryFactory):
-        pass
-
-    setattr(CustomRetryFactory, f"{waiter}_wait", broken_wait)
-
-    retrying = CustomRetryFactory().build()
-    client = client_cls(api_key="a", api_url=mockserver.urljoin("/"), retrying=retrying)
-    with pytest.raises(OutlierException):
-        await getattr(client, get_method)(
-            {"url": f"https://{subdomain}.example", "browserHtml": True},
-        )
-
-
-@pytest.mark.parametrize(
-    ("client_cls", "get_method"),
-    (
-        (AsyncZyteAPI, "get"),
-        (AsyncClient, "request_raw"),
-    ),
-)
-@pytest.mark.asyncio
-async def test_retry_wait_network_error(client_cls, get_method):
-    waiter = "network_error"
-
-    def broken_wait(self, retry_state):
-        raise OutlierException
-
-    class CustomRetryFactory(RetryFactory):
-        pass
-
-    setattr(CustomRetryFactory, f"{waiter}_wait", broken_wait)
-
-    retrying = CustomRetryFactory().build()
-    with MockServer(resource=DropResource) as mockserver:
-        client = client_cls(
-            api_key="a", api_url=mockserver.urljoin("/"), retrying=retrying
-        )
-        with pytest.raises(OutlierException):
-            await getattr(client, get_method)(
-                {"url": "https://example.com", "browserHtml": True},
-            )
-
-
-@pytest.mark.parametrize(
-    ("client_cls", "get_method"),
-    (
-        (AsyncZyteAPI, "get"),
-        (AsyncClient, "request_raw"),
-    ),
-)
-@pytest.mark.parametrize(
-    ("subdomain", "stopper"),
-    (
-        ("e429", "throttling"),
-        ("e520", "temporary_download_error"),
-    ),
-)
-@pytest.mark.asyncio
-async def test_retry_stop(client_cls, get_method, subdomain, stopper, mockserver):
-    def broken_stop(self, retry_state):
-        raise OutlierException
-
-    class CustomRetryFactory(RetryFactory):
-        def wait(self, retry_state):
-            return None
-
-    setattr(CustomRetryFactory, f"{stopper}_stop", broken_stop)
-
-    retrying = CustomRetryFactory().build()
-    client = client_cls(api_key="a", api_url=mockserver.urljoin("/"), retrying=retrying)
-    with pytest.raises(OutlierException):
-        await getattr(client, get_method)(
-            {"url": f"https://{subdomain}.example", "browserHtml": True},
-        )
-
-
-@pytest.mark.parametrize(
-    ("client_cls", "get_method"),
-    (
-        (AsyncZyteAPI, "get"),
-        (AsyncClient, "request_raw"),
-    ),
-)
-@pytest.mark.asyncio
-async def test_retry_stop_network_error(client_cls, get_method):
-    stopper = "network_error"
-
-    def broken_stop(self, retry_state):
-        raise OutlierException
-
-    class CustomRetryFactory(RetryFactory):
-        def wait(self, retry_state):
-            return None
-
-    setattr(CustomRetryFactory, f"{stopper}_stop", broken_stop)
-
-    retrying = CustomRetryFactory().build()
-    with MockServer(resource=DropResource) as mockserver:
-        client = client_cls(
-            api_key="a", api_url=mockserver.urljoin("/"), retrying=retrying
-        )
-        with pytest.raises(OutlierException):
-            await getattr(client, get_method)(
-                {"url": "https://example.com", "browserHtml": True},
-            )
-
-
-@pytest.mark.parametrize(
     ("client_cls", "get_method", "iter_method"),
     (
         (AsyncZyteAPI, "get", "iter"),
         (AsyncClient, "request_raw", "request_parallel_as_completed"),
     ),
 )
 @pytest.mark.asyncio
@@ -478,7 +308,14 @@
 
     assert len(actual_results) == len(expected_results)
     for actual_result in actual_results:
         if isinstance(actual_result, Exception):
             assert Exception in expected_results
         else:
             assert actual_result in expected_results
+
+
+def test_retrying_class():
+    """A descriptive exception is raised when creating a client with an
+    AsyncRetrying subclass or similar instead of an instance of it."""
+    with pytest.raises(ValueError):
+        AsyncZyteAPI(api_key="foo", retrying=AggressiveRetryFactory)
```

### Comparing `zyte_api-0.5.2/tests/test_main.py` & `zyte_api-0.6.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/tests/test_sync.py` & `zyte_api-0.6.0/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/tests/test_utils.py` & `zyte_api-0.6.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/zyte_api/__main__.py` & `zyte_api-0.6.0/zyte_api/__main__.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/zyte_api/_async.py` & `zyte_api-0.6.0/zyte_api/_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,19 @@
         *,
         api_key=None,
         api_url=API_URL,
         n_conn=15,
         retrying: Optional[AsyncRetrying] = None,
         user_agent: Optional[str] = None,
     ):
+        if retrying is not None and not isinstance(retrying, AsyncRetrying):
+            raise ValueError(
+                "The retrying parameter, if defined, must be an instance of "
+                "AsyncRetrying."
+            )
         self.api_key = get_apikey(api_key)
         self.api_url = api_url
         self.n_conn = n_conn
         self.agg_stats = AggStats()
         self.retrying = retrying or zyte_api_retrying
         self.user_agent = user_agent or USER_AGENT
         self._semaphore = asyncio.Semaphore(n_conn)
```

### Comparing `zyte_api-0.5.2/zyte_api/_errors.py` & `zyte_api-0.6.0/zyte_api/_errors.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/zyte_api/_sync.py` & `zyte_api-0.6.0/zyte_api/_sync.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/zyte_api/_utils.py` & `zyte_api-0.6.0/zyte_api/_utils.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/zyte_api/aio/__init__.py` & `zyte_api-0.6.0/zyte_api/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/zyte_api/apikey.py` & `zyte_api-0.6.0/zyte_api/apikey.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/zyte_api/errors.py` & `zyte_api-0.6.0/zyte_api/errors.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/zyte_api/stats.py` & `zyte_api-0.6.0/zyte_api/stats.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/zyte_api/utils.py` & `zyte_api-0.6.0/zyte_api/utils.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.2/zyte_api.egg-info/PKG-INFO` & `zyte_api-0.6.0/zyte_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-api
-Version: 0.5.2
+Version: 0.6.0
 Summary: Python interface to Zyte API
 Home-page: https://github.com/zytedata/python-zyte-api
 Author: Zyte Group Ltd
 Author-email: opensource@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte_api-0.5.2/zyte_api.egg-info/SOURCES.txt` & `zyte_api-0.6.0/zyte_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

