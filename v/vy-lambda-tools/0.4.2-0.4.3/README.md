# Comparing `tmp/vy_lambda_tools-0.4.2.tar.gz` & `tmp/vy_lambda_tools-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vy_lambda_tools-0.4.2.tar", max compression
+gzip compressed data, was "vy_lambda_tools-0.4.3.tar", max compression
```

## Comparing `vy_lambda_tools-0.4.2.tar` & `vy_lambda_tools-0.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       88 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/README.adoc
--rw-r--r--   0        0        0      605 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/__init__.py
--rw-r--r--   0        0        0      904 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/configuration.py
--rw-r--r--   0        0        0      217 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/feature_flag/__init__.py
--rw-r--r--   0        0        0     1988 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/feature_flag/base.py
--rw-r--r--   0        0        0     3519 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/feature_flag/providers.py
--rw-r--r--   0        0        0      312 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/__init__.py
--rw-r--r--   0        0        0     4020 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/api_gateway.py
--rw-r--r--   0        0        0     1205 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/dynamodb.py
--rw-r--r--   0        0        0      857 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/handler.py
--rw-r--r--   0        0        0     2850 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/sqs.py
--rw-r--r--   0        0        0     2360 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/instrumentation.py
--rw-r--r--   0        0        0        0 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/py.typed
--rw-r--r--   0        0        0     7217 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/routing.py
--rw-r--r--   0        0        0     4957 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/test_helpers.py
--rw-r--r--   0        0        0      446 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/types.py
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 vy_lambda_tools-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       88 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/README.adoc
+-rw-r--r--   0        0        0      605 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/__init__.py
+-rw-r--r--   0        0        0      904 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/configuration.py
+-rw-r--r--   0        0        0      217 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/feature_flag/__init__.py
+-rw-r--r--   0        0        0     1988 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/feature_flag/base.py
+-rw-r--r--   0        0        0     3519 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/feature_flag/providers.py
+-rw-r--r--   0        0        0      312 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/handlers/__init__.py
+-rw-r--r--   0        0        0     4147 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/handlers/api_gateway.py
+-rw-r--r--   0        0        0     1205 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/handlers/dynamodb.py
+-rw-r--r--   0        0        0      857 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/handlers/handler.py
+-rw-r--r--   0        0        0     2850 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/handlers/sqs.py
+-rw-r--r--   0        0        0     2360 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/instrumentation.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/py.typed
+-rw-r--r--   0        0        0     7217 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/routing.py
+-rw-r--r--   0        0        0     4957 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/test_helpers.py
+-rw-r--r--   0        0        0      446 2024-05-29 10:13:26.000000 vy_lambda_tools-0.4.3/vy_lambda_tools/types.py
+-rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 vy_lambda_tools-0.4.3/PKG-INFO
```

### Comparing `vy_lambda_tools-0.4.2/pyproject.toml` & `vy_lambda_tools-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vy-lambda-tools"
-version = "0.4.2"
+version = "0.4.3"
 description = ""
 authors = ["Nicolas Harlem Eide <nicolas@harlemeide.net>"]
 readme = "README.adoc"
 packages = [{include = "vy_lambda_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `vy_lambda_tools-0.4.2/vy_lambda_tools/configuration.py` & `vy_lambda_tools-0.4.3/vy_lambda_tools/configuration.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.2/vy_lambda_tools/feature_flag/base.py` & `vy_lambda_tools-0.4.3/vy_lambda_tools/feature_flag/base.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.2/vy_lambda_tools/feature_flag/providers.py` & `vy_lambda_tools-0.4.3/vy_lambda_tools/feature_flag/providers.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/api_gateway.py` & `vy_lambda_tools-0.4.3/vy_lambda_tools/handlers/api_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 @dataclass
 class HTTPRequest:
     path_parameters: dict[str, Any] = dataclasses.field(default_factory=dict)
     query_parameters: dict[str, Any] = dataclasses.field(default_factory=dict)
     body: dict[str, Any] = dataclasses.field(default_factory=dict)
     account_id: Optional[str] = None
     jwt: Optional[APIGatewayEventAuthorizer] = None
+    headers: dict[str, str] = dataclasses.field(default_factory=dict)
 
 
 HTTPResponse = tuple[int, Union[Any, dict[str, Any]]]
 
 
 class JSONEncoderWithSetSupport(json.JSONEncoder):
     def default(self, o: Any) -> Any:
@@ -81,14 +82,15 @@
 
         return HTTPRequest(
             body=body,
             path_parameters=path_parameters,
             query_parameters=query_parameters,
             account_id=api_gw_event.request_context.identity.account_id,
             jwt=jwt,
+            headers=api_gw_event.resolved_headers_field,
         )
 
     def handle_error(self, exception: Exception) -> HTTPResponse:
         status_code = self.allowed_errors.get(type(exception), 500)
 
         if status_code == 500:
             message = "An unexpected error happened"
```

### Comparing `vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/dynamodb.py` & `vy_lambda_tools-0.4.3/vy_lambda_tools/handlers/dynamodb.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/handler.py` & `vy_lambda_tools-0.4.3/vy_lambda_tools/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/sqs.py` & `vy_lambda_tools-0.4.3/vy_lambda_tools/handlers/sqs.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.2/vy_lambda_tools/instrumentation.py` & `vy_lambda_tools-0.4.3/vy_lambda_tools/instrumentation.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.2/vy_lambda_tools/routing.py` & `vy_lambda_tools-0.4.3/vy_lambda_tools/routing.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.2/vy_lambda_tools/test_helpers.py` & `vy_lambda_tools-0.4.3/vy_lambda_tools/test_helpers.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.2/PKG-INFO` & `vy_lambda_tools-0.4.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vy-lambda-tools
-Version: 0.4.2
+Version: 0.4.3
 Summary: 
 Author: Nicolas Harlem Eide
 Author-email: nicolas@harlemeide.net
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aws-lambda-powertools (>=2.32.0,<3.0.0)
```

