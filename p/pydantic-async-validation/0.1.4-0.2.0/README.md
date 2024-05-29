# Comparing `tmp/pydantic_async_validation-0.1.4.tar.gz` & `tmp/pydantic_async_validation-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_async_validation-0.1.4.tar", max compression
+gzip compressed data, was "pydantic_async_validation-0.2.0.tar", max compression
```

## Comparing `pydantic_async_validation-0.1.4.tar` & `pydantic_async_validation-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2024-04-17 07:34:45.528515 pydantic_async_validation-0.1.4/LICENSE
--rw-r--r--   0        0        0     9031 2024-04-17 07:34:45.528515 pydantic_async_validation-0.1.4/README.md
--rw-r--r--   0        0        0      374 2024-04-17 07:34:45.528515 pydantic_async_validation-0.1.4/pydantic_async_validation/__init__.py
--rw-r--r--   0        0        0      445 2024-04-17 07:34:45.528515 pydantic_async_validation-0.1.4/pydantic_async_validation/constants.py
--rw-r--r--   0        0        0      950 2024-04-17 07:34:45.528515 pydantic_async_validation-0.1.4/pydantic_async_validation/fastapi.py
--rw-r--r--   0        0        0     2491 2024-04-17 07:34:45.528515 pydantic_async_validation-0.1.4/pydantic_async_validation/metaclasses.py
--rw-r--r--   0        0        0     4998 2024-04-17 07:34:45.528515 pydantic_async_validation-0.1.4/pydantic_async_validation/mixins.py
--rw-r--r--   0        0        0        0 2024-04-17 07:34:45.528515 pydantic_async_validation-0.1.4/pydantic_async_validation/py.typed
--rw-r--r--   0        0        0     6347 2024-04-17 07:34:45.528515 pydantic_async_validation-0.1.4/pydantic_async_validation/utils.py
--rw-r--r--   0        0        0     2857 2024-04-17 07:34:45.528515 pydantic_async_validation-0.1.4/pydantic_async_validation/validators.py
--rw-r--r--   0        0        0     1172 2024-04-17 07:34:45.528515 pydantic_async_validation-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     9789 1970-01-01 00:00:00.000000 pydantic_async_validation-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-29 16:35:15.849498 pydantic_async_validation-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9187 2024-05-29 16:35:15.849498 pydantic_async_validation-0.2.0/README.md
+-rw-r--r--   0        0        0      374 2024-05-29 16:35:15.849498 pydantic_async_validation-0.2.0/pydantic_async_validation/__init__.py
+-rw-r--r--   0        0        0      445 2024-05-29 16:35:15.849498 pydantic_async_validation-0.2.0/pydantic_async_validation/constants.py
+-rw-r--r--   0        0        0     1770 2024-05-29 16:35:15.849498 pydantic_async_validation-0.2.0/pydantic_async_validation/fastapi.py
+-rw-r--r--   0        0        0     2487 2024-05-29 16:35:15.849498 pydantic_async_validation-0.2.0/pydantic_async_validation/metaclasses.py
+-rw-r--r--   0        0        0     5012 2024-05-29 16:35:15.849498 pydantic_async_validation-0.2.0/pydantic_async_validation/mixins.py
+-rw-r--r--   0        0        0        0 2024-05-29 16:35:15.849498 pydantic_async_validation-0.2.0/pydantic_async_validation/py.typed
+-rw-r--r--   0        0        0     6344 2024-05-29 16:35:15.849498 pydantic_async_validation-0.2.0/pydantic_async_validation/utils.py
+-rw-r--r--   0        0        0     2857 2024-05-29 16:35:15.849498 pydantic_async_validation-0.2.0/pydantic_async_validation/validators.py
+-rw-r--r--   0        0        0     1172 2024-05-29 16:35:15.849498 pydantic_async_validation-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9945 1970-01-01 00:00:00.000000 pydantic_async_validation-0.2.0/PKG-INFO
```

### Comparing `pydantic_async_validation-0.1.4/LICENSE` & `pydantic_async_validation-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_async_validation-0.1.4/README.md` & `pydantic_async_validation-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -175,20 +175,21 @@
 
 
 app = fastapi.FastAPI()
 
 @app.get("/return-http-422-on-async-validation-error")
 async def return_http_422_on_async_validation_error():
     instance = SomethingModel(...)
-    with ensure_request_validation_errors():
+    with ensure_request_validation_errors("body"):  # use body as error location prefix
         await instance.model_async_validate()
 ```
 
 You may also use `ensure_request_validation_errors` to do additional validation on the request data using normal
-pydantic validation and converting those `ValidationError`s to `RequestValidationError`s. 😉
+pydantic validation and converting those `ValidationError`s to `RequestValidationError`s. Use the `prefix`
+parameter to mimic the FastAPI behaviour regarding using "body" for POST body data for example. 😉
 
 **Note:** When using FastAPI you should install `pydantic-async-validation` using
 `pip install pydantic-async-validation[fastapi]` to ensure FastAPI is installed in a compatible version.
 
 # Contributing
 
 If you want to contribute to this project, feel free to just fork the project,
```

### Comparing `pydantic_async_validation-0.1.4/pydantic_async_validation/fastapi.py` & `pydantic_async_validation-0.2.0/pydantic_async_validation/fastapi.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,36 @@
 from contextlib import contextmanager
-from typing import Generator
+from typing import Generator, List, Optional, Tuple, Union
 
 from fastapi.exceptions import RequestValidationError
 from pydantic import ValidationError
+from pydantic_core import ErrorDetails
+
+
+def _prefix_request_errors(
+    prefix: Tuple[Union[int, str], ...],
+    errors: List[ErrorDetails],
+) -> List[ErrorDetails]:
+    """Add prefix to errors in preparation for request validation error conversion."""
+
+    return [
+        {
+            **error,
+            # Just add prefix
+            'loc': (*prefix, *error.get('loc', [])),
+        }
+        for error
+        in errors
+    ]
 
 
 @contextmanager
-def ensure_request_validation_errors() -> Generator[None, None, None]:
+def ensure_request_validation_errors(
+    prefix: Optional[Union[Tuple[Union[int, str], ...], str]] = None,
+) -> Generator[None, None, None]:
     """
     Converter for `ValidationError` to `RequestValidationError`.
 
     This will convert any ValidationError's inside the called code into
     RequestValidationErrors which will trigger HTTP 422 responses in
     FastAPI. This is useful for when you want to do extra validation in
     your code that is not covered by FastAPI's normal request parameter
@@ -24,8 +44,18 @@
         some_code_doing_extra_validation()  # for example async validation
     ```
     """
 
     try:
         yield
     except ValidationError as O_o:
-        raise RequestValidationError(errors=O_o.errors()) from O_o
+        prepared_errors = O_o.errors(include_url=False)
+
+        if prefix is None:
+            raise RequestValidationError(errors=prepared_errors) from O_o
+
+        if isinstance(prefix, str):
+            prefix = (prefix,)
+
+        raise RequestValidationError(
+            errors=_prefix_request_errors(prefix, prepared_errors),
+        ) from O_o
```

### Comparing `pydantic_async_validation-0.1.4/pydantic_async_validation/metaclasses.py` & `pydantic_async_validation-0.2.0/pydantic_async_validation/metaclasses.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         namespace: dict[str, Any],
         **kwargs: Any,
     ) -> Any:
         async_field_validators: List[Tuple[List[str], ValidationInfo]] = []
         async_model_validators: List[ValidationInfo] = []
 
         async_field_validator_fields: Optional[List[str]]
-        async_field_validator_config: "Optional[ValidationInfo]"
-        async_model_validator_config: "Optional[ValidationInfo]"
+        async_field_validator_config: Optional[ValidationInfo]
+        async_model_validator_config: Optional[ValidationInfo]
 
         for base in bases:
             async_field_validators += getattr(
                 base,
                 ASYNC_FIELD_VALIDATORS_KEY,
                 [],
             )
```

### Comparing `pydantic_async_validation-0.1.4/pydantic_async_validation/mixins.py` & `pydantic_async_validation-0.2.0/pydantic_async_validation/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             # Direct child instance
             if isinstance(attribute_value, AsyncValidationModelMixin):
                 await extend_with_validation_errors_by(
                     (attribute_name,),
                     attribute_value,
                 )
             # List of child instances
-            if isinstance(attribute_value, list):
+            if isinstance(attribute_value, (list, set, tuple)):
                 for index, item in enumerate(attribute_value):
                     if isinstance(item, AsyncValidationModelMixin):
                         await extend_with_validation_errors_by(
                             (attribute_name, index),
                             item,
                         )
             # Dict of child instances
```

### Comparing `pydantic_async_validation-0.1.4/pydantic_async_validation/utils.py` & `pydantic_async_validation-0.2.0/pydantic_async_validation/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             self, value=value, config=config,
         )
     if args == {'field', 'config'}:
         return lambda self, value, field, config: validator_func(  # noqa: ARG005
             self, field=field, config=config,
         )
 
-    # args == {'value', 'field', 'validator'}
+    # args == {'value', 'field', 'config'}
     return lambda self, value, field, config: validator_func(
         self, value=value, field=field, config=config,
     )
 
 
 def make_generic_model_validator(validator_func: Callable) -> Callable:
     """
```

### Comparing `pydantic_async_validation-0.1.4/pydantic_async_validation/validators.py` & `pydantic_async_validation-0.2.0/pydantic_async_validation/validators.py`

 * *Files identical despite different names*

### Comparing `pydantic_async_validation-0.1.4/pyproject.toml` & `pydantic_async_validation-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-async-validation"
-version = "0.1.4"
+version = "0.2.0"
 description = "Add async validation to pydantic"
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pydantic_async_validation"}]
 
 [tool.poetry.dependencies]
@@ -18,15 +18,15 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.1.2,<9.0.0"
 pytest-cov = ">=3,<6"
 pytest-asyncio = ">=0.21.1,<0.24.0"
 tox = ">=3.26,<5.0"
 httpx = ">=0.24.1,<0.28.0"
-ruff = ">=0.2.0,<0.4.0"
+ruff = ">=0.2.0,<0.5.0"
 pyright = ">=1.1.350,<1.2"
 
 [tool.ruff]
 line-length = 115
 target-version = "py38"
 output-format = "grouped"
```

### Comparing `pydantic_async_validation-0.1.4/PKG-INFO` & `pydantic_async_validation-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-async-validation
-Version: 0.1.4
+Version: 0.2.0
 Summary: Add async validation to pydantic
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -196,20 +196,21 @@
 
 
 app = fastapi.FastAPI()
 
 @app.get("/return-http-422-on-async-validation-error")
 async def return_http_422_on_async_validation_error():
     instance = SomethingModel(...)
-    with ensure_request_validation_errors():
+    with ensure_request_validation_errors("body"):  # use body as error location prefix
         await instance.model_async_validate()
 ```
 
 You may also use `ensure_request_validation_errors` to do additional validation on the request data using normal
-pydantic validation and converting those `ValidationError`s to `RequestValidationError`s. 😉
+pydantic validation and converting those `ValidationError`s to `RequestValidationError`s. Use the `prefix`
+parameter to mimic the FastAPI behaviour regarding using "body" for POST body data for example. 😉
 
 **Note:** When using FastAPI you should install `pydantic-async-validation` using
 `pip install pydantic-async-validation[fastapi]` to ensure FastAPI is installed in a compatible version.
 
 # Contributing
 
 If you want to contribute to this project, feel free to just fork the project,
```

