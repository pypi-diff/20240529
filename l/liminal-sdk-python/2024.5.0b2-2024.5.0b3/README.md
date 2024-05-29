# Comparing `tmp/liminal_sdk_python-2024.5.0b2.tar.gz` & `tmp/liminal_sdk_python-2024.5.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liminal_sdk_python-2024.5.0b2.tar", max compression
+gzip compressed data, was "liminal_sdk_python-2024.5.0b3.tar", max compression
```

## Comparing `liminal_sdk_python-2024.5.0b2.tar` & `liminal_sdk_python-2024.5.0b3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/LICENSE
--rw-r--r--   0        0        0    12308 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/README.md
--rw-r--r--   0        0        0       82 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/__init__.py
--rw-r--r--   0        0        0      524 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/auth/__init__.py
--rw-r--r--   0        0        0       34 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/auth/microsoft/__init__.py
--rw-r--r--   0        0        0     2961 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/auth/microsoft/device_code_flow.py
--rw-r--r--   0        0        0      849 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/auth/microsoft/models.py
--rw-r--r--   0        0        0    10159 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/client.py
--rw-r--r--   0        0        0      165 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/const.py
--rw-r--r--   0        0        0       45 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/endpoints/__init__.py
--rw-r--r--   0        0        0     2275 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/endpoints/llm/__init__.py
--rw-r--r--   0        0        0     2064 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/endpoints/llm/models.py
--rw-r--r--   0        0        0      437 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/endpoints/llm/schemas.py
--rw-r--r--   0        0        0     7957 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/endpoints/prompt/__init__.py
--rw-r--r--   0        0        0     3322 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/endpoints/prompt/models.py
--rw-r--r--   0        0        0      960 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/endpoints/prompt/schemas.py
--rw-r--r--   0        0        0     2562 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/endpoints/thread/__init__.py
--rw-r--r--   0        0        0     2130 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/endpoints/thread/models.py
--rw-r--r--   0        0        0      733 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/endpoints/thread/schemas.py
--rw-r--r--   0        0        0      400 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/errors.py
--rw-r--r--   0        0        0       22 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/helpers/__init__.py
--rw-r--r--   0        0        0      374 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/helpers/model.py
--rw-r--r--   0        0        0      394 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/helpers/schema.py
--rw-r--r--   0        0        0      109 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/liminal/helpers/typing.py
--rw-r--r--   0        0        0    13912 2024-05-22 21:19:48.176579 liminal_sdk_python-2024.5.0b2/pyproject.toml
--rw-r--r--   0        0        0    13432 1970-01-01 00:00:00.000000 liminal_sdk_python-2024.5.0b2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/LICENSE
+-rw-r--r--   0        0        0    12308 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/README.md
+-rw-r--r--   0        0        0       82 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/__init__.py
+-rw-r--r--   0        0        0      524 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/auth/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/auth/microsoft/__init__.py
+-rw-r--r--   0        0        0     2961 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/auth/microsoft/device_code_flow.py
+-rw-r--r--   0        0        0      849 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/auth/microsoft/models.py
+-rw-r--r--   0        0        0    10159 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/client.py
+-rw-r--r--   0        0        0      165 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/const.py
+-rw-r--r--   0        0        0       45 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/__init__.py
+-rw-r--r--   0        0        0     2275 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/llm/__init__.py
+-rw-r--r--   0        0        0     2064 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/llm/models.py
+-rw-r--r--   0        0        0      437 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/llm/schemas.py
+-rw-r--r--   0        0        0     7957 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/prompt/__init__.py
+-rw-r--r--   0        0        0     3597 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/prompt/models.py
+-rw-r--r--   0        0        0      960 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/prompt/schemas.py
+-rw-r--r--   0        0        0     2563 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/thread/__init__.py
+-rw-r--r--   0        0        0     2130 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/thread/models.py
+-rw-r--r--   0        0        0      733 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/thread/schemas.py
+-rw-r--r--   0        0        0      400 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/errors.py
+-rw-r--r--   0        0        0       22 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/helpers/__init__.py
+-rw-r--r--   0        0        0      374 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/helpers/model.py
+-rw-r--r--   0        0        0      394 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/helpers/schema.py
+-rw-r--r--   0        0        0      109 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/helpers/typing.py
+-rw-r--r--   0        0        0    13892 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/pyproject.toml
+-rw-r--r--   0        0        0    13432 1970-01-01 00:00:00.000000 liminal_sdk_python-2024.5.0b3/PKG-INFO
```

### Comparing `liminal_sdk_python-2024.5.0b2/LICENSE` & `liminal_sdk_python-2024.5.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b2/README.md` & `liminal_sdk_python-2024.5.0b3/README.md`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b2/liminal/auth/__init__.py` & `liminal_sdk_python-2024.5.0b3/liminal/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b2/liminal/auth/microsoft/device_code_flow.py` & `liminal_sdk_python-2024.5.0b3/liminal/auth/microsoft/device_code_flow.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b2/liminal/auth/microsoft/models.py` & `liminal_sdk_python-2024.5.0b3/liminal/auth/microsoft/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b2/liminal/client.py` & `liminal_sdk_python-2024.5.0b3/liminal/client.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b2/liminal/endpoints/llm/__init__.py` & `liminal_sdk_python-2024.5.0b3/liminal/endpoints/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b2/liminal/endpoints/llm/models.py` & `liminal_sdk_python-2024.5.0b3/liminal/endpoints/llm/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b2/liminal/endpoints/prompt/__init__.py` & `liminal_sdk_python-2024.5.0b3/liminal/endpoints/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b2/liminal/endpoints/prompt/models.py` & `liminal_sdk_python-2024.5.0b3/liminal/endpoints/prompt/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,27 +38,29 @@
 @dataclass(frozen=True, kw_only=True)
 class CleanseData(BaseModel):
     """Define the result of a cleanse request."""
 
     items: list[CleansedToken]
     # Represents the prompt with the sensitive data replaced with cleansed tokens:
     text: str
-    items_hashed: list[CleansedToken]
+    items_hashed: list[CleansedToken] = field(
+        metadata=field_options(alias="itemsHashed")
+    )
     # Represents the prompt with the sensitive data replaced with hashed tokens (which
     # are help in mapping):
-    text_hashed: str
+    text_hashed: str = field(metadata=field_options(alias="textHashed"))
 
 
 @dataclass(frozen=True, kw_only=True)
 class CleansedToken(BaseModel):
     """Define a cleansed token."""
 
     start: int
     end: int
-    entity_type: str
+    entity_type: str = field(metadata=field_options(alias="entityType"))
 
 
 @dataclass(frozen=True, kw_only=True)
 class HydrateData(BaseModel):
     """Define the result of a hydration request."""
 
     items: list[HydratedToken]
@@ -66,25 +68,25 @@
 
 
 @dataclass(frozen=True, kw_only=True)
 class HydratedToken(BaseModel):
     """Define a hydrated token."""
 
     end: int
-    entity_type: str
+    entity_type: str = field(metadata=field_options(alias="entityType"))
     start: int
 
 
 @dataclass(frozen=True, kw_only=True)
 class ReidentifiedToken(BaseModel):
     """Define a reidentified token."""
 
     start: int
     end: int
-    entity_type: str
+    entity_type: str = field(metadata=field_options(alias="entityType"))
     text: str
 
 
 @dataclass(frozen=True, kw_only=True)
 class StreamResponseChunk(BaseModel):
     """Define a streaming response chunk."""
```

### Comparing `liminal_sdk_python-2024.5.0b2/liminal/endpoints/prompt/schemas.py` & `liminal_sdk_python-2024.5.0b3/liminal/endpoints/prompt/schemas.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b2/liminal/endpoints/thread/__init__.py` & `liminal_sdk_python-2024.5.0b3/liminal/endpoints/thread/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         Args:
         ----
             model_instance_id: The model instance id.
             name: The name of the thread.
 
         Returns:
         -------
-            A Thread object representing the creatd thread.
+            A Thread object representing the created thread.
 
         """
         response = cast(
             CreateThreadResponse,
             await self._request_and_validate(
                 "POST",
                 "/api/v1/threads",
```

### Comparing `liminal_sdk_python-2024.5.0b2/liminal/endpoints/thread/models.py` & `liminal_sdk_python-2024.5.0b3/liminal/endpoints/thread/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b2/liminal/endpoints/thread/schemas.py` & `liminal_sdk_python-2024.5.0b3/liminal/endpoints/thread/schemas.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b2/pyproject.toml` & `liminal_sdk_python-2024.5.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.poetry]
 name = "liminal-sdk-python"
-version = "2024.05.0b2"
+version = "2024.05.0b3"
 description = "The Liminal SDK for Python"
 readme = "README.md"
 authors = ["Aaron Bach <ab@liminal.ai>"]
 license = "Apache-2.0"
 repository = "https://github.com/liminal-ai-security/liminal-sdk-python"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -58,28 +58,27 @@
 httpx = "0.27.0"
 msal = "1.28.0"
 python = "^3.11.8"
 mashumaro = "3.13"
 
 [tool.poetry.group.dev.dependencies]
 blacken-docs = "1.16.0"
-codespell = "2.2.6"
+codespell = "2.3.0"
 coverage = {version = "7.5.1", extras = ["toml"]}
 darglint = "1.8.1"
 mypy = "1.10.0"
 packaging = "==24.0"
 pre-commit = "3.7.1"
 pre-commit-hooks = "4.6.0"
 pylint = "3.2.2"
 pytest = "8.2.1"
 pytest-asyncio = "0.23.7"
 pytest-cov = "5.0.0"
 pytest-httpx = "0.30.0"
-ruff = "0.4.4"
-ruff-lsp = "0.0.53"
+ruff = "0.4.5"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/liminal-ai-security/liminal-sdk-python/issues"
 Changelog = "https://github.com/liminal-ai-security/liminal-sdk-python/releases"
 
 [tool.pylint.BASIC]
 class-const-naming-style = "any"
```

### Comparing `liminal_sdk_python-2024.5.0b2/PKG-INFO` & `liminal_sdk_python-2024.5.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liminal-sdk-python
-Version: 2024.5.0b2
+Version: 2024.5.0b3
 Summary: The Liminal SDK for Python
 Home-page: https://github.com/liminal-ai-security/liminal-sdk-python
 License: Apache-2.0
 Author: Aaron Bach
 Author-email: ab@liminal.ai
 Requires-Python: >=3.11.8,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

