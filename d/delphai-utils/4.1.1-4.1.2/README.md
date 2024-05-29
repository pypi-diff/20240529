# Comparing `tmp/delphai_utils-4.1.1.tar.gz` & `tmp/delphai_utils-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphai_utils-4.1.1.tar", max compression
+gzip compressed data, was "delphai_utils-4.1.2.tar", max compression
```

## Comparing `delphai_utils-4.1.1.tar` & `delphai_utils-4.1.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0       22 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/__init__.py
--rw-r--r--   0        0        0      936 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/aio.py
--rw-r--r--   0        0        0     3842 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/authorization.py
--rw-r--r--   0        0        0      495 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/authorization_test.py
--rw-r--r--   0        0        0     2069 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/caching.py
--rw-r--r--   0        0        0     1313 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/config.py
--rw-r--r--   0        0        0    13924 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/constants/companies.py
--rw-r--r--   0        0        0     1389 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/db.py
--rw-r--r--   0        0        0      549 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/elasticsearch.py
--rw-r--r--   0        0        0     9347 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/faust.py
--rw-r--r--   0        0        0      481 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/formatting.py
--rw-r--r--   0        0        0     6728 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/gateway.py
--rw-r--r--   0        0        0     4796 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/grpc_client.py
--rw-r--r--   0        0        0     3687 2024-05-14 12:02:22.912610 delphai_utils-4.1.1/delphai_utils/grpc_server.py
--rw-r--r--   0        0        0     1532 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/interceptors/authentication.py
--rw-r--r--   0        0        0     5218 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/interceptors/metrics.py
--rw-r--r--   0        0        0     1482 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/keycloak.py
--rw-r--r--   0        0        0     1410 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/logging.py
--rw-r--r--   0        0        0     7182 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/monitoring.py
--rw-r--r--   0        0        0     2926 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/patches.py
--rw-r--r--   0        0        0      119 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/__init__.py
--rw-r--r--   0        0        0    10360 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/client.py
--rw-r--r--   0        0        0      393 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/errors.py
--rw-r--r--   0        0        0     4954 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/metrics.py
--rw-r--r--   0        0        0     2492 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/models.py
--rw-r--r--   0        0        0    10649 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/server.py
--rw-r--r--   0        0        0     2830 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/types.py
--rw-r--r--   0        0        0      693 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/rpc/utils.py
--rw-r--r--   0        0        0      582 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/strings/similarity.py
--rw-r--r--   0        0        0     4106 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/users.py
--rw-r--r--   0        0        0     2608 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/utils.py
--rw-r--r--   0        0        0      435 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/validation.py
--rw-r--r--   0        0        0    43882 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/delphai_utils/validator.py
--rw-r--r--   0        0        0     3196 2024-05-14 12:02:22.916610 delphai_utils-4.1.1/pyproject.toml
--rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 delphai_utils-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-05-29 08:40:01.246932 delphai_utils-4.1.2/delphai_utils/__init__.py
+-rw-r--r--   0        0        0      936 2024-05-29 08:40:01.246932 delphai_utils-4.1.2/delphai_utils/aio.py
+-rw-r--r--   0        0        0     3842 2024-05-29 08:40:01.246932 delphai_utils-4.1.2/delphai_utils/authorization.py
+-rw-r--r--   0        0        0      495 2024-05-29 08:40:01.246932 delphai_utils-4.1.2/delphai_utils/authorization_test.py
+-rw-r--r--   0        0        0     2069 2024-05-29 08:40:01.246932 delphai_utils-4.1.2/delphai_utils/caching.py
+-rw-r--r--   0        0        0     1313 2024-05-29 08:40:01.246932 delphai_utils-4.1.2/delphai_utils/config.py
+-rw-r--r--   0        0        0    13924 2024-05-29 08:40:01.246932 delphai_utils-4.1.2/delphai_utils/constants/companies.py
+-rw-r--r--   0        0        0     1389 2024-05-29 08:40:01.246932 delphai_utils-4.1.2/delphai_utils/db.py
+-rw-r--r--   0        0        0      549 2024-05-29 08:40:01.246932 delphai_utils-4.1.2/delphai_utils/elasticsearch.py
+-rw-r--r--   0        0        0     9347 2024-05-29 08:40:01.246932 delphai_utils-4.1.2/delphai_utils/faust.py
+-rw-r--r--   0        0        0      481 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/formatting.py
+-rw-r--r--   0        0        0     6728 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/gateway.py
+-rw-r--r--   0        0        0     4796 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/grpc_client.py
+-rw-r--r--   0        0        0     3687 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/grpc_server.py
+-rw-r--r--   0        0        0     1532 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/interceptors/authentication.py
+-rw-r--r--   0        0        0     5218 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/interceptors/metrics.py
+-rw-r--r--   0        0        0     1482 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/keycloak.py
+-rw-r--r--   0        0        0     1410 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/logging.py
+-rw-r--r--   0        0        0     7182 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/monitoring.py
+-rw-r--r--   0        0        0     2926 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/patches.py
+-rw-r--r--   0        0        0      119 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/rpc/__init__.py
+-rw-r--r--   0        0        0    10201 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/rpc/client.py
+-rw-r--r--   0        0        0      912 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/rpc/connection_manager.py
+-rw-r--r--   0        0        0      393 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/rpc/errors.py
+-rw-r--r--   0        0        0     4954 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/rpc/metrics.py
+-rw-r--r--   0        0        0     2492 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/rpc/models.py
+-rw-r--r--   0        0        0    11173 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/rpc/server.py
+-rw-r--r--   0        0        0     2830 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/rpc/types.py
+-rw-r--r--   0        0        0      441 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/rpc/utils.py
+-rw-r--r--   0        0        0      582 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/strings/similarity.py
+-rw-r--r--   0        0        0     4106 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/users.py
+-rw-r--r--   0        0        0     2608 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/utils.py
+-rw-r--r--   0        0        0      435 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/validation.py
+-rw-r--r--   0        0        0    43882 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/delphai_utils/validator.py
+-rw-r--r--   0        0        0     3196 2024-05-29 08:40:01.250932 delphai_utils-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 delphai_utils-4.1.2/PKG-INFO
```

### Comparing `delphai_utils-4.1.1/delphai_utils/aio.py` & `delphai_utils-4.1.2/delphai_utils/aio.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/authorization.py` & `delphai_utils-4.1.2/delphai_utils/authorization.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/caching.py` & `delphai_utils-4.1.2/delphai_utils/caching.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/config.py` & `delphai_utils-4.1.2/delphai_utils/config.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/constants/companies.py` & `delphai_utils-4.1.2/delphai_utils/constants/companies.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/db.py` & `delphai_utils-4.1.2/delphai_utils/db.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/elasticsearch.py` & `delphai_utils-4.1.2/delphai_utils/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/faust.py` & `delphai_utils-4.1.2/delphai_utils/faust.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/gateway.py` & `delphai_utils-4.1.2/delphai_utils/gateway.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/grpc_client.py` & `delphai_utils-4.1.2/delphai_utils/grpc_client.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/grpc_server.py` & `delphai_utils-4.1.2/delphai_utils/grpc_server.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/interceptors/authentication.py` & `delphai_utils-4.1.2/delphai_utils/interceptors/authentication.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/interceptors/metrics.py` & `delphai_utils-4.1.2/delphai_utils/interceptors/metrics.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/keycloak.py` & `delphai_utils-4.1.2/delphai_utils/keycloak.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/logging.py` & `delphai_utils-4.1.2/delphai_utils/logging.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/monitoring.py` & `delphai_utils-4.1.2/delphai_utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/patches.py` & `delphai_utils-4.1.2/delphai_utils/patches.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/rpc/client.py` & `delphai_utils-4.1.2/delphai_utils/rpc/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 import uuid
 import weakref
 
 from typing import Any, Dict, Optional
 
 from . import errors
 from . import metrics
+from .connection_manager import get_connection
 from .models import Request, Response
 from .server import request_context
 from .types import AbstractOptions, Message, Priority
-from .utils import clean_service_name, fix_message_timestamp, make_connection_name
+from .utils import clean_service_name, fix_message_timestamp
 
 
 logger = logging.getLogger(__name__)
 
 
 class Options(AbstractOptions):
     timeout: Optional[float] = 60
@@ -55,19 +56,17 @@
     __getitem__ = __getattr__ = get_service
 
     async def _ensure_connection(self):
         async with self._client_lock:
             if self._connection and self._channel:
                 return
 
-            connection_url = aio_pika.connection.make_url(self._connection_string)
-            if not connection_url.query.get("name"):
-                connection_url %= {"name": make_connection_name(self._client_name)}
-
-            self._connection = await aio_pika.connect_robust(connection_url)
+            self._connection = await get_connection(
+                self._connection_string, self._client_name
+            )
             self._channel = await self._connection.channel(on_return_raises=True)
 
     async def _ensure_reply_queue(self):
         await self._ensure_connection()
 
         async with self._client_lock:
             if self._reply_queue:
@@ -80,18 +79,18 @@
                 auto_delete=True,
             )
             await queue.consume(fix_message_timestamp(self._on_message))
 
             self._reply_queue = queue
 
     async def stop(self):
-        connection = self._connection
-        if connection:
+        channel = self._channel
+        if channel:
             self._reset()
-            await connection.close()
+            await channel.close()
 
     async def call(
         self,
         service_name: str,
         method_name: str,
         arguments: Optional[Dict[str, Any]] = None,
         options: Optional[Options] = None,
```

### Comparing `delphai_utils-4.1.1/delphai_utils/rpc/metrics.py` & `delphai_utils-4.1.2/delphai_utils/rpc/metrics.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/rpc/models.py` & `delphai_utils-4.1.2/delphai_utils/rpc/models.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/rpc/server.py` & `delphai_utils-4.1.2/delphai_utils/rpc/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 import socket
 import time
 
 from typing import Optional
 
 from . import errors
 from . import metrics
+from .connection_manager import get_connection
 from .models import Request, Response
 from .types import Message, Priority, RequestContext
-from .utils import clean_service_name, fix_message_timestamp, make_connection_name
+from .utils import clean_service_name, fix_message_timestamp
 
 
 logger = logging.getLogger(__name__)
 
 request_context = contextvars.ContextVar("request_context", default=None)
 
 
@@ -36,31 +37,59 @@
 
     def _reset(self):
         self._connection = None
         self._channel = None
         self._exchange = None
         self._queue = None
 
-    def bind(self, handler):
-        if handler.__name__ in self._handlers:
-            raise KeyError(f"Handler {handler.__name__} already defined")
+    def bind(self, handler=None, *, name=None):
+        """
+        Binds to be exposed handlers (functions) to RPC server instance:
+
+        @server.bind
+        def add(*, a: float, b: float) -> float:
+            ...
+
+        # or
+
+        def sub(*, a: float, b: float) -> float:
+            ...
+
+        server.bind(sub)
+
+        # or
+
+        @server.bind(name="mul")
+        def multiply(*, a: float, b: float) -> float:
+            ...
+
+        """
+
+        def decorator(handler):
+            self._bind_handler(handler=handler, name=name)
+            return handler
+
+        return decorator(handler) if handler else decorator
+
+    def _bind_handler(self, *, handler=None, name=None):
+        handler_name = name or handler.__name__
+        if handler_name in self._handlers:
+            raise KeyError(f"Handler {handler_name} already defined")
 
         if hasattr(handler, "raw_function"):
             # Unwrap `pydantic.validate_call` decorator
             handler = handler.raw_function
 
         self._validate_handler(handler)
 
-        self._handlers[handler.__name__] = pydantic.validate_call(
+        self._handlers[handler_name] = pydantic.validate_call(
             handler,
             validate_return=True,
         )
 
-        return handler
-
     def _validate_handler(self, handler):
         if not inspect.iscoroutinefunction(handler):
             raise TypeError("Handlers must be coroutine functions")
 
         positional_only = []
         positional_or_keyword = []
 
@@ -91,18 +120,17 @@
                 self.__class__,
             )
 
     async def start(self, connection_string, prefetch_count=1):
         if self._connection:
             raise RuntimeError("Already started")
 
-        connection_url = aio_pika.connection.make_url(connection_string)
-        if not connection_url.query.get("name"):
-            connection_url %= {"name": make_connection_name(self._service_name)}
-        connection = self._connection = await aio_pika.connect_robust(connection_url)
+        connection = self._connection = await get_connection(
+            connection_string, self._service_name
+        )
         channel = self._channel = await connection.channel()
         await channel.set_qos(prefetch_count=prefetch_count)
 
         exchange = self._exchange = await channel.declare_exchange(
             name=f"service.{self._service_name}",
             type=aio_pika.ExchangeType.TOPIC,
             durable=True,
@@ -119,18 +147,18 @@
 
         await queue.bind(exchange, "#")
         await queue.consume(fix_message_timestamp(self._on_message))
 
         logger.info("RPC server is consuming messages from `%s`", queue)
 
     async def stop(self):
-        connection = self._connection
-        if connection:
+        channel = self._channel
+        if channel:
             self._reset()
-            await connection.close()
+            await channel.close()
 
     async def serve_forever(self, connection_string, prefetch_count=1):
         await self.start(connection_string, prefetch_count=prefetch_count)
         try:
             await asyncio.Future()
         finally:
             await self.stop()
```

### Comparing `delphai_utils-4.1.1/delphai_utils/rpc/types.py` & `delphai_utils-4.1.2/delphai_utils/rpc/types.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/strings/similarity.py` & `delphai_utils-4.1.2/delphai_utils/strings/similarity.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/users.py` & `delphai_utils-4.1.2/delphai_utils/users.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/utils.py` & `delphai_utils-4.1.2/delphai_utils/utils.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/delphai_utils/validator.py` & `delphai_utils-4.1.2/delphai_utils/validator.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-4.1.1/pyproject.toml` & `delphai_utils-4.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "delphai-utils"
-version = "4.1.1"
+version = "4.1.2"
 description = "delphai backend utilities"
 authors = ["Barath Kumar <barath@delphai.com>"]
 homepage = "https://github.com/delphai/delphai-utils"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiokafka = { version = "0.7.2", optional = true }
```

### Comparing `delphai_utils-4.1.1/PKG-INFO` & `delphai_utils-4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphai-utils
-Version: 4.1.1
+Version: 4.1.2
 Summary: delphai backend utilities
 Home-page: https://github.com/delphai/delphai-utils
 Author: Barath Kumar
 Author-email: barath@delphai.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

