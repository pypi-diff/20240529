# Comparing `tmp/schemafunc-0.3.0.tar.gz` & `tmp/schemafunc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemafunc-0.3.0.tar", max compression
+gzip compressed data, was "schemafunc-0.3.1.tar", max compression
```

## Comparing `schemafunc-0.3.0.tar` & `schemafunc-0.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2024-04-11 16:31:26.401239 schemafunc-0.3.0/LICENSE
--rw-r--r--   0        0        0     1139 2024-05-28 18:48:29.945819 schemafunc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6614 2024-04-14 16:41:56.673792 schemafunc-0.3.0/README.md
--rw-r--r--   0        0        0    19796 2024-05-28 18:46:08.076593 schemafunc-0.3.0/src/schemafunc.py
--rw-r--r--   0        0        0     7625 1970-01-01 00:00:00.000000 schemafunc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-11 16:31:26.401239 schemafunc-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1139 2024-05-29 15:58:09.678785 schemafunc-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6614 2024-04-14 16:41:56.673792 schemafunc-0.3.1/README.md
+-rw-r--r--   0        0        0    20090 2024-05-29 15:55:59.934239 schemafunc-0.3.1/src/schemafunc.py
+-rw-r--r--   0        0        0     7625 1970-01-01 00:00:00.000000 schemafunc-0.3.1/PKG-INFO
```

### Comparing `schemafunc-0.3.0/LICENSE` & `schemafunc-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schemafunc-0.3.0/pyproject.toml` & `schemafunc-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schemafunc"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python function-to-LLM tool maker."
 authors = ["Dustin Wyatt <dustin.wyatt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dmwyatt/schemafunc"
 
 keywords = ["python", "openai", "llm", "language-model", "schema", "function", "tool"]
```

### Comparing `schemafunc-0.3.0/README.md` & `schemafunc-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `schemafunc-0.3.0/src/schemafunc.py` & `schemafunc-0.3.1/src/schemafunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,38 @@
             "tool_choice": {
                 "type": "function",
                 "function": {"name": self.schema["function"]["name"]},
             },
         }
 
 
-def add_schemafunc(_func=None, **schema_kwargs):
+P = typing.ParamSpec("P")
+R = typing.TypeVar("R")
+
+
+class HasSchemaFuncAttribute(typing.Protocol[P, R]):
+    schemafunc: FunctionMetadata
+
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
+        ...
+
+
+def add_schemafunc(_func=None, **schema_kwargs) -> HasSchemaFuncAttribute[P, R]:
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         if not hasattr(wrapper, "function_metadata"):
             wrapper.schemafunc = FunctionMetadata(func, **schema_kwargs)
 
             # force evaluation of the cached properties so that we raise errors like
             # `NoDocstringError` at definition time
             # TODO: Maybe just drop the cached properties functionality?
+            # noinspection PyStatementEffect
             wrapper.schemafunc.openai_tool_kwargs
 
         return wrapper
 
     if _func is not None:
         return decorator(_func)
     else:
```

### Comparing `schemafunc-0.3.0/PKG-INFO` & `schemafunc-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemafunc
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python function-to-LLM tool maker.
 Home-page: https://github.com/dmwyatt/schemafunc
 License: MIT
 Keywords: python,openai,llm,language-model,schema,function,tool
 Author: Dustin Wyatt
 Author-email: dustin.wyatt@gmail.com
 Requires-Python: >=3.8.10,<4.0.0
```

