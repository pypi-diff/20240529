# Comparing `tmp/anydata-0.1.1.tar.gz` & `tmp/anydata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anydata-0.1.1.tar", max compression
+gzip compressed data, was "anydata-0.1.2.tar", max compression
```

## Comparing `anydata-0.1.1.tar` & `anydata-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-04-01 21:27:17.734610 anydata-0.1.1/LICENSE
--rw-r--r--   0        0        0     3393 2024-04-13 02:44:50.881249 anydata-0.1.1/README.md
--rw-r--r--   0        0        0       70 2024-04-05 23:57:59.131667 anydata-0.1.1/anydata/__init__.py
--rw-r--r--   0        0        0    18782 2024-04-27 19:11:50.495308 anydata-0.1.1/anydata/core/dataapi.py
--rw-r--r--   0        0        0    11126 2024-04-27 14:45:59.271171 anydata-0.1.1/anydata/core/endpoint.py
--rw-r--r--   0        0        0     6146 2024-04-05 23:57:59.132977 anydata-0.1.1/anydata/engine/functions.py
--rw-r--r--   0        0        0      377 2024-04-05 23:57:59.133267 anydata-0.1.1/anydata/engine/models.py
--rw-r--r--   0        0        0     1303 2024-04-05 23:57:59.133579 anydata-0.1.1/anydata/engine/prompts/system_prompts.py
--rw-r--r--   0        0        0     1159 2024-04-05 23:57:59.133974 anydata-0.1.1/anydata/engine/prompts/user_prompts.py
--rw-r--r--   0        0        0       93 2024-04-07 06:53:49.947855 anydata-0.1.1/anydata/exceptions.py
--rw-r--r--   0        0        0    11192 2024-04-27 17:45:13.060192 anydata-0.1.1/anydata/parsers/openapi.py
--rw-r--r--   0        0        0     2084 2024-04-27 19:10:03.996974 anydata-0.1.1/anydata/parsers/response_parser.py
--rw-r--r--   0        0        0     4510 2024-04-05 23:57:59.135519 anydata-0.1.1/anydata/schemas/core.py
--rw-r--r--   0        0        0     2637 2024-04-05 23:57:59.136123 anydata-0.1.1/anydata/schemas/openapi.py
--rw-r--r--   0        0        0      745 2024-04-27 19:29:48.001539 anydata-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4176 1970-01-01 00:00:00.000000 anydata-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 21:27:17.734610 anydata-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7263 2024-05-29 18:52:48.771528 anydata-0.1.2/README.md
+-rw-r--r--   0        0        0       70 2024-04-05 23:57:59.131667 anydata-0.1.2/anydata/__init__.py
+-rw-r--r--   0        0        0    18857 2024-04-27 20:29:40.147604 anydata-0.1.2/anydata/core/dataapi.py
+-rw-r--r--   0        0        0    11126 2024-04-27 14:45:59.271171 anydata-0.1.2/anydata/core/endpoint.py
+-rw-r--r--   0        0        0     6147 2024-05-29 00:09:25.599995 anydata-0.1.2/anydata/engine/functions.py
+-rw-r--r--   0        0        0      377 2024-04-05 23:57:59.133267 anydata-0.1.2/anydata/engine/models.py
+-rw-r--r--   0        0        0     1303 2024-04-05 23:57:59.133579 anydata-0.1.2/anydata/engine/prompts/system_prompts.py
+-rw-r--r--   0        0        0     1159 2024-04-05 23:57:59.133974 anydata-0.1.2/anydata/engine/prompts/user_prompts.py
+-rw-r--r--   0        0        0       93 2024-04-07 06:53:49.947855 anydata-0.1.2/anydata/exceptions.py
+-rw-r--r--   0        0        0    11193 2024-04-27 20:29:40.043978 anydata-0.1.2/anydata/parsers/openapi.py
+-rw-r--r--   0        0        0     2098 2024-04-27 20:29:40.146736 anydata-0.1.2/anydata/parsers/response_parser.py
+-rw-r--r--   0        0        0     4510 2024-04-05 23:57:59.135519 anydata-0.1.2/anydata/schemas/core.py
+-rw-r--r--   0        0        0     2637 2024-04-05 23:57:59.136123 anydata-0.1.2/anydata/schemas/openapi.py
+-rw-r--r--   0        0        0      763 2024-05-29 21:51:26.431104 anydata-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8078 1970-01-01 00:00:00.000000 anydata-0.1.2/PKG-INFO
```

### Comparing `anydata-0.1.1/LICENSE` & `anydata-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anydata-0.1.1/anydata/core/dataapi.py` & `anydata-0.1.2/anydata/core/dataapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     is_guidance = True
 except ImportError:
     is_guidance = False
 
 if is_guidance:
     from ..engine.functions import dataapi_from_prompt, evaluate_unsuccessful_response
 
+
 class DataAPI(ABCDataAPI):
     def __init__(
         self,
         base_url: str,
         openapi: Optional[Union[str, dict, OpenAPI]] = None,
         shared_params: Optional[dict] = None,
         shared_headers: Optional[dict] = None,
@@ -95,15 +96,17 @@
         self.auth = auth
         self.timeout = timeout
         self.allow_redirects = allow_redirects
         self.stream = stream
         self.verify = verify
         self.cert = cert
         if lm:
-            assert is_guidance, ImportError("Please install the 'guidance' package using `pip install guidance` to use language models.")
+            assert is_guidance, ImportError(
+                "Please install the 'guidance' package using `pip install guidance` to use language models."
+            )
             assert isinstance(
                 lm, Model
             ), "Language model must be a valid initiliazied `guidance.models.Model` object."
             self.lm = lm
 
     def __setitem__(self, key, value) -> None:
         """
@@ -146,15 +149,17 @@
 
     def set_lm(self, lm: Model) -> None:
         """Set the language model for the DataAPI.
 
         Args:
             lm (Model): Language model for the DataAPI.
         """
-        assert is_guidance, ImportError("Please install the 'guidance' package using `pip install guidance` to use language models.")
+        assert is_guidance, ImportError(
+            "Please install the 'guidance' package using `pip install guidance` to use language models."
+        )
         assert isinstance(
             lm, Model
         ), "Language model must be a valid initiliazied `guidance.models.Model` object."
         self.lm = lm
 
     def set_shared_params(self, params: dict, propagate: bool = True) -> None:
         """
@@ -270,15 +275,17 @@
 
         Args:
             prompt (str): Natural language prompt to determine the Endpoint relative URL, method, and parameters.
             alias (Optional[str], optional): Alias to access the Endpoint from the parent DataAPI object. Defaults to None.
             echo (bool, optional): Print the language model outputs during endpoint instantiation. Defaults to False.
         """
         # TODO: Implement retries with backoff
-        assert is_guidance, ImportError("Please install the 'guidance' package using `pip install guidance` to use this method.")
+        assert is_guidance, ImportError(
+            "Please install the 'guidance' package using `pip install guidance` to use this method."
+        )
         assert self.openapi, "An OpenAPI specification is needed for a smart_add_endpoint. Please define one with the .set_openapi() method."
         assert (
             self.lm is not None
         ), "A language model is needed for a smart_add_endpoint. Please define one with the the .set_lm() method."
         stateless_lm = self.lm.copy()
         stateless_lm.echo = echo
         try:
```

### Comparing `anydata-0.1.1/anydata/core/endpoint.py` & `anydata-0.1.2/anydata/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `anydata-0.1.1/anydata/engine/functions.py` & `anydata-0.1.2/anydata/engine/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional
 import guidance
 from guidance import gen, system, user, assistant, select
+
 from ..parsers.openapi import OpenAPI
 from ..engine.prompts.system_prompts import (
     RELATIVE_URL_FETCHER,
     REST_API_OPERATION_FETCHER,
     REST_API_PARAMETERS_FETCHER,
 )
 from ..engine.prompts.user_prompts import (
```

### Comparing `anydata-0.1.1/anydata/engine/prompts/system_prompts.py` & `anydata-0.1.2/anydata/engine/prompts/system_prompts.py`

 * *Files identical despite different names*

### Comparing `anydata-0.1.1/anydata/engine/prompts/user_prompts.py` & `anydata-0.1.2/anydata/engine/prompts/user_prompts.py`

 * *Files identical despite different names*

### Comparing `anydata-0.1.1/anydata/parsers/openapi.py` & `anydata-0.1.2/anydata/parsers/openapi.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -275,8 +275,8 @@
             "info": self.info_summary(excluded_info_properties),
             "servers": self.servers_summary(excluded_server_properties),
             "paths": self.paths_summary(
                 excluded_operation_properties,
                 exclude_non_2XX_responses,
                 resolve_parameter_references,
             ),
-        }
+        }
```

### Comparing `anydata-0.1.1/anydata/parsers/response_parser.py` & `anydata-0.1.2/anydata/parsers/response_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     is_pandas = False
 
 
 def dataframe_from_array_of_dicts(array: list) -> "pd.DataFrame":
     """
     Returns a pandas DataFrame from an array of dictionaries.
     """
-    assert is_pandas, ImportError("Please install the 'pandas' package using `pip install pandas` to use this function.")
+    assert is_pandas, ImportError(
+        "Please install the 'pandas' package using `pip install pandas` to use this function."
+    )
     try:
         return pd.DataFrame.from_dict(array, orient="columns")
     except Exception as e:
         print(
             f"An error occurred while converting the array of type {type(array)} into a DataFrame: {e}"
         )
         raise
```

### Comparing `anydata-0.1.1/anydata/schemas/core.py` & `anydata-0.1.2/anydata/schemas/core.py`

 * *Files identical despite different names*

### Comparing `anydata-0.1.1/anydata/schemas/openapi.py` & `anydata-0.1.2/anydata/schemas/openapi.py`

 * *Files identical despite different names*

### Comparing `anydata-0.1.1/pyproject.toml` & `anydata-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 name = "anydata"
-version = "0.1.1"
+version = "0.1.2"
 description = "Smart framework to interact with and fetch data from REST APIs."
 authors = ["Erich Silva <erich@esilva.io>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
 dataclasses-json = "^0.6.4"
 pyyaml = "^6.0.1"
-guidance = { version = "^0.1.13", optional = true }
-
-[tool.poetry.extras]
-guidance = ["guidance"]
+guidance = { version = "=0.1.13", optional = true }
+pandas = "^2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 ruff = "^0.1.0"
 python-dotenv = "^1.0.1"
 pre-commit = "^3.7.0"
 
+[tool.poetry.extras]
+guidance = ["guidance"]
+
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 "anydata/engine/models.py" = ["F401"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

