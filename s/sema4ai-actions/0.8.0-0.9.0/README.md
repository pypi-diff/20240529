# Comparing `tmp/sema4ai_actions-0.8.0.tar.gz` & `tmp/sema4ai_actions-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema4ai_actions-0.8.0.tar", max compression
+gzip compressed data, was "sema4ai_actions-0.9.0.tar", max compression
```

## Comparing `sema4ai_actions-0.8.0.tar` & `sema4ai_actions-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     2971 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/README.md
--rw-r--r--   0        0        0      877 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5588 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/__init__.py
--rw-r--r--   0        0        0       80 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/__main__.py
--rw-r--r--   0        0        0    16310 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_action.py
--rw-r--r--   0        0        0     7567 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_action_context.py
--rw-r--r--   0        0        0    11652 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_args_dispatcher.py
--rw-r--r--   0        0        0     1494 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_callback.py
--rw-r--r--   0        0        0     8339 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_collect_actions.py
--rw-r--r--   0        0        0    35568 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_commands.py
--rw-r--r--   0        0        0     2276 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_config.py
--rw-r--r--   0        0        0      331 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_constants.py
--rw-r--r--   0        0        0        0 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_customization/__init__.py
--rw-r--r--   0        0        0     2722 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_customization/_extension_points.py
--rw-r--r--   0        0        0     9922 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_customization/_plugin_manager.py
--rw-r--r--   0        0        0      220 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_exceptions.py
--rw-r--r--   0        0        0     5638 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_fixtures.py
--rw-r--r--   0        0        0     2500 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_hooks.py
--rw-r--r--   0        0        0     7491 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_interrupts.py
--rw-r--r--   0        0        0     1367 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_lifecycle.py
--rw-r--r--   0        0        0    13368 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_lint_action.py
--rw-r--r--   0        0        0     1082 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_log_auto_setup.py
--rw-r--r--   0        0        0     3074 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_log_output_setup.py
--rw-r--r--   0        0        0     6342 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_managed_parameters.py
--rw-r--r--   0        0        0     6023 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_protocols.py
--rw-r--r--   0        0        0    13813 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_remove_refs.py
--rw-r--r--   0        0        0     2906 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_request.py
--rw-r--r--   0        0        0     1023 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_request_impl.py
--rw-r--r--   0        0        0     1116 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_response.py
--rw-r--r--   0        0        0     6615 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_secret/__init__.py
--rw-r--r--   0        0        0     5153 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_secret/_oauth2_secret.py
--rw-r--r--   0        0        0     2678 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_secret/_secret.py
--rw-r--r--   0        0        0     3134 2024-05-23 13:51:24.510320 sema4ai_actions-0.8.0/src/sema4ai/actions/api.py
--rw-r--r--   0        0        0     2277 2024-05-23 13:51:24.510320 sema4ai_actions-0.8.0/src/sema4ai/actions/cli.py
--rw-r--r--   0        0        0        0 2024-05-23 13:51:24.510320 sema4ai_actions-0.8.0/src/sema4ai/actions/py.typed
--rw-r--r--   0        0        0     3825 1970-01-01 00:00:00.000000 sema4ai_actions-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2971 2024-05-29 11:57:21.125873 sema4ai_actions-0.9.0/README.md
+-rw-r--r--   0        0        0      877 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5588 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/__main__.py
+-rw-r--r--   0        0        0    16250 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_action.py
+-rw-r--r--   0        0        0     7567 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_action_context.py
+-rw-r--r--   0        0        0    11652 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_args_dispatcher.py
+-rw-r--r--   0        0        0     1494 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_callback.py
+-rw-r--r--   0        0        0     8339 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_collect_actions.py
+-rw-r--r--   0        0        0    35933 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_commands.py
+-rw-r--r--   0        0        0     2276 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_config.py
+-rw-r--r--   0        0        0      331 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_constants.py
+-rw-r--r--   0        0        0        0 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_customization/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_customization/_extension_points.py
+-rw-r--r--   0        0        0     9922 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_customization/_plugin_manager.py
+-rw-r--r--   0        0        0      220 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_exceptions.py
+-rw-r--r--   0        0        0     5638 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_fixtures.py
+-rw-r--r--   0        0        0     2500 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_hooks.py
+-rw-r--r--   0        0        0     7491 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_interrupts.py
+-rw-r--r--   0        0        0     1367 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_lifecycle.py
+-rw-r--r--   0        0        0    13368 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_lint_action.py
+-rw-r--r--   0        0        0     1082 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_log_auto_setup.py
+-rw-r--r--   0        0        0     3074 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_log_output_setup.py
+-rw-r--r--   0        0        0     6342 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_managed_parameters.py
+-rw-r--r--   0        0        0     6023 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_protocols.py
+-rw-r--r--   0        0        0    13813 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_remove_refs.py
+-rw-r--r--   0        0        0     2906 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_request.py
+-rw-r--r--   0        0        0     1023 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_request_impl.py
+-rw-r--r--   0        0        0     1116 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_response.py
+-rw-r--r--   0        0        0     6615 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_secret/__init__.py
+-rw-r--r--   0        0        0     5813 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_secret/_oauth2_secret.py
+-rw-r--r--   0        0        0     2678 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_secret/_secret.py
+-rw-r--r--   0        0        0     1375 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/_variables_scope.py
+-rw-r--r--   0        0        0     3134 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/api.py
+-rw-r--r--   0        0        0     2277 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/cli.py
+-rw-r--r--   0        0        0        0 2024-05-29 11:57:21.129873 sema4ai_actions-0.9.0/src/sema4ai/actions/py.typed
+-rw-r--r--   0        0        0     3825 1970-01-01 00:00:00.000000 sema4ai_actions-0.9.0/PKG-INFO
```

### Comparing `sema4ai_actions-0.8.0/README.md` & `sema4ai_actions-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/pyproject.toml` & `sema4ai_actions-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sema4ai-actions"
-version = "0.8.0"
+version = "0.9.0"
 description = "Sema4AI Actions"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/Sema4AI/actions/"
 license = "Apache-2.0"
```

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/__init__.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 from ._fixtures import setup, teardown
 from ._protocols import IAction, Status
 from ._request import Request
 from ._response import ActionError, Response
 from ._secret import OAuth2Secret, Secret
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @overload
 def action(func: Callable) -> Callable:
     ...
```

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_action.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_action.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,88 @@
     str: "string",
     int: "integer",
     float: "number",
     bool: "boolean",
 }
 
 
+def get_provider_and_scope_from_annotation_args(
+    annotation_args, filename: str, name: str
+) -> tuple[str, list[str]]:
+    from typing import get_args, get_origin
+
+    from sema4ai.actions._exceptions import ActionsCollectError
+
+    error_message = f"""
+Invalid OAuth2Secret annotation found.
+
+The OAuth2Secret must be parametrized with 2 arguments, 
+the first being a Literal with the provider name 
+(i.e.: `Literal["google"]`) 
+and the second a list with one Literal with the (multiple) scopes that are required
+(i.e.: `list[Literal["scope1", "scope2", ...]])
+
+Full Example for a parameter named `google_secret` requiring google sheets 
+and google drive scopes:
+
+google_secret: OAuth2Secret[
+    Literal["google"],
+    list[
+        Literal[
+            "https://www.googleapis.com/auth/drive.readonly",
+            "https://www.googleapis.com/auth/spreadsheets.readonly",
+        ]
+    ],
+]
+
+File with @action: {filename}
+@action name: {name}
+"""
+    if not annotation_args or len(annotation_args) != 2:
+        raise ActionsCollectError(error_message)
+
+    provider = annotation_args[0]
+    scopes = annotation_args[1]
+    if get_origin(provider) != Literal:
+        raise ActionsCollectError(f"First parameter is not a Literal.\n{error_message}")
+    if get_origin(scopes) not in (list, List):
+        raise ActionsCollectError(f"Second parameter is not a list.\n{error_message}")
+    provider_args = get_args(provider)
+    if not provider_args or len(provider_args) != 1:
+        raise ActionsCollectError(
+            f"First parameter does not have a single provider argument.\n{error_message}"
+        )
+    provider_str = provider_args[0]
+    if not isinstance(provider_str, str):
+        raise ActionsCollectError(
+            f"First parameter Literal does not have a string.\n{error_message}"
+        )
+
+    scope_args = get_args(scopes)
+    if not scope_args or len(scope_args) != 1:
+        raise ActionsCollectError(
+            f"Second parameter is not a list with a single Literal.\n{error_message}"
+        )
+
+    scope_args_literal = scope_args[0]
+    if get_origin(scope_args_literal) != Literal:
+        raise ActionsCollectError(
+            f"Second parameter is not a list with a single Literal.\n{error_message}"
+        )
+
+    scope_strs = get_args(scope_args_literal)
+    for entry in scope_strs:
+        if not isinstance(entry, str):
+            raise ActionsCollectError(
+                f"Second parameter is not a list with a literal with strings.\n{error_message}"
+            )
+
+    return provider_str, list(scope_strs)
+
+
 class Action:
     def __init__(
         self,
         pm: PluginManager,
         module_name: str,
         module_file: str,
         method: typing.Callable,
@@ -104,102 +178,38 @@
 
         if param_name:
             properties["title"] = param_name.replace("_", " ").title()
         return properties
 
     @property
     def managed_params_schema(self) -> Dict[str, Any]:
-        from typing import get_args, get_origin
+        from typing import get_args
 
         from sema4ai.actions._commands import _get_managed_param_type, _is_managed_param
-        from sema4ai.actions._exceptions import ActionsCollectError
 
         managed_params_schema: Dict[str, Any] = {}
         sig = inspect.signature(self.method)
 
         param_name_to_description = self._get_param_name_to_description()
         for param in sig.parameters.values():
             if _is_managed_param(self._pm, param.name, param=param):
                 tp = _get_managed_param_type(self._pm, param.name, param=param).__name__
 
                 dct: dict[str, Any] = {"type": tp}
                 if tp == "OAuth2Secret":
                     # In this case we need to make some introspection to get additional information
                     # on the type (provider, scopes, ...)
                     annotation_args = get_args(param.annotation)
-                    error_message = f"""
-Invalid OAuth2Secret annotation found.
-
-The OAuth2Secret must be parametrized with 2 arguments, 
-the first being a Literal with the provider name 
-(i.e.: `Literal["google"]`) 
-and the second a list with one Literal with the (multiple) scopes that are required
-(i.e.: `list[Literal["scope1", "scope2", ...]])
-
-Full Example for a parameter named `google_secret` requiring google sheets 
-and google drive scopes:
-
-google_secret: OAuth2Secret[
-    Literal["google"],
-    list[
-        Literal[
-            "https://www.googleapis.com/auth/drive.readonly",
-            "https://www.googleapis.com/auth/spreadsheets.readonly",
-        ]
-    ],
-]
-
-File with @action: {self.filename}
-@action name: {self.name}
-"""
-                    if not annotation_args or len(annotation_args) != 2:
-                        raise ActionsCollectError(error_message)
-
-                    provider = annotation_args[0]
-                    scopes = annotation_args[1]
-                    if get_origin(provider) != Literal:
-                        raise ActionsCollectError(
-                            f"First parameter is not a Literal.\n{error_message}"
-                        )
-                    if get_origin(scopes) not in (list, List):
-                        raise ActionsCollectError(
-                            f"Second parameter is not a list.\n{error_message}"
-                        )
-                    provider_args = get_args(provider)
-                    if not provider_args or len(provider_args) != 1:
-                        raise ActionsCollectError(
-                            f"First parameter does not have a single provider argument.\n{error_message}"
-                        )
-                    provider_str = provider_args[0]
-                    if not isinstance(provider_str, str):
-                        raise ActionsCollectError(
-                            f"First parameter Literal does not have a string.\n{error_message}"
-                        )
-
+                    (
+                        provider_str,
+                        scope_strs,
+                    ) = get_provider_and_scope_from_annotation_args(
+                        annotation_args, self.filename, self.name
+                    )
                     dct["provider"] = provider_str
-
-                    scope_args = get_args(scopes)
-                    if not scope_args or len(scope_args) != 1:
-                        raise ActionsCollectError(
-                            f"Second parameter is not a list with a single Literal.\n{error_message}"
-                        )
-
-                    scope_args_literal = scope_args[0]
-                    if get_origin(scope_args_literal) != Literal:
-                        raise ActionsCollectError(
-                            f"Second parameter is not a list with a single Literal.\n{error_message}"
-                        )
-
-                    scope_strs = get_args(scope_args_literal)
-                    for entry in scope_strs:
-                        if not isinstance(entry, str):
-                            raise ActionsCollectError(
-                                f"Second parameter is not a list with a literal with strings.\n{error_message}"
-                            )
-
                     dct["scopes"] = scope_strs
 
                 desc = param_name_to_description.get(param.name)
                 if desc:
                     dct["description"] = desc
                 managed_params_schema[param.name] = dct
 
@@ -247,15 +257,19 @@
                 method_name, param.name, param_type, description, "parameter"
             )
             properties[param.name] = param_properties
 
             if param.default is inspect.Parameter.empty:
                 required.append(param.name)
             else:
-                param_properties["default"] = param.default
+                default = param.default
+                if hasattr(default, "model_dump"):
+                    # Support for pydantic
+                    default = default.model_dump()
+                param_properties["default"] = default
 
         if required:
             schema["required"] = required
 
         return schema
 
     @property
@@ -433,15 +447,15 @@
                 )
 
                 self.show(
                     "".join(traceback.format_exception(*action.exc_info)),
                     kind=self.KIND_TRACEBACK,
                 )
 
-        if self._print_result and action.status == Status.PASS:
+        if self._print_result and result is not None:
             show("result:", kind=self.KIND_IMPORTANT)
             try:
                 dump = result
                 if hasattr(result, "model_dump"):
                     # Support for pydantic
                     dump = result.model_dump()
```

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_action_context.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_action_context.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_args_dispatcher.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_args_dispatcher.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_callback.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_callback.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_collect_actions.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_collect_actions.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_commands.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -655,14 +655,17 @@
 
 def _validate_and_convert_kwargs(
     pm: PluginManager, action: IAction, kwargs: Dict[str, Any]
 ) -> Dict[str, Any]:
     from typing import get_type_hints
 
     from sema4ai.actions._exceptions import InvalidArgumentsError
+    from sema4ai.actions._variables_scope import (
+        create_validate_and_convert_kwargs_scope,
+    )
 
     target_method = action.method
     sig = inspect.signature(target_method)
     type_hints = get_type_hints(target_method)
     method_name = target_method.__code__.co_name
     new_kwargs: Dict[str, Any] = {}
 
@@ -673,52 +676,55 @@
         if param_type is None:
             # If not given, default to `str`.
             if is_managed_param:
                 param_type = _get_managed_param_type(pm, param.name, param=param)
             else:
                 param_type = str
 
-        if param.default is inspect.Parameter.empty:
-            # It's required, so, let's see if it's in the kwargs.
-            if not is_managed_param:
-                if param_name not in kwargs:
-                    raise InvalidArgumentsError(
-                        f"Error. The parameter `{param_name}` was not defined in the input."
-                    )
+        with create_validate_and_convert_kwargs_scope(
+            param_name=param_name, param_type=param_type
+        ):
+            if param.default is inspect.Parameter.empty:
+                # It's required, so, let's see if it's in the kwargs.
+                if not is_managed_param:
+                    if param_name not in kwargs:
+                        raise InvalidArgumentsError(
+                            f"Error. The parameter `{param_name}` was not defined in the input."
+                        )
 
-        passed_value = kwargs.get(param_name, inspect.Parameter.empty)
+            passed_value = kwargs.get(param_name, inspect.Parameter.empty)
 
-        if passed_value is not inspect.Parameter.empty:
-            if param_type not in SUPPORTED_TYPES_IN_SCHEMA:
-                model_validate = getattr(param_type, "model_validate", None)
-                if model_validate is not None:
-                    # Support for pydantic models.
-                    try:
-                        created = model_validate(passed_value)
-                    except Exception as e:
-                        msg = f"(error converting received json contents to pydantic model: {e}."
+            if passed_value is not inspect.Parameter.empty:
+                if param_type not in SUPPORTED_TYPES_IN_SCHEMA:
+                    model_validate = getattr(param_type, "model_validate", None)
+                    if model_validate is not None:
+                        # Support for pydantic models.
+                        try:
+                            created = model_validate(passed_value)
+                        except Exception as e:
+                            msg = f"Error converting received json contents to pydantic model: {e}."
+                            raise InvalidArgumentsError(
+                                f"It's not possible to call: '{method_name}' because the passed arguments don't match the expected signature.\n{msg}"
+                            )
+                        new_kwargs[param_name] = created
+                        continue
+                    else:
                         raise InvalidArgumentsError(
-                            f"It's not possible to call: '{method_name}' because the passed arguments don't match the expected signature.\n{msg}"
+                            f"Error. The param type '{param_type.__name__}' in '{method_name}' is not supported. Supported parameter types: str, int, float, bool and pydantic.Model."
                         )
-                    new_kwargs[param_name] = created
-                    continue
-                else:
+
+                check_type = param_type
+                if param_type == float:
+                    check_type = (float, int)
+                if not isinstance(passed_value, check_type):
                     raise InvalidArgumentsError(
-                        f"Error. The param type '{param_type.__name__}' in '{method_name}' is not supported. Supported parameter types: str, int, float, bool and pydantic.Model."
+                        f"Error. Expected the parameter: `{param_name}` to be of type: {param_type.__name__}. Found type: {type(passed_value).__name__}."
                     )
 
-            check_type = param_type
-            if param_type == float:
-                check_type = (float, int)
-            if not isinstance(passed_value, check_type):
-                raise InvalidArgumentsError(
-                    f"Error. Expected the parameter: `{param_name}` to be of type: {param_type.__name__}. Found type: {type(passed_value).__name__}."
-                )
-
-            new_kwargs[param_name] = passed_value
+                new_kwargs[param_name] = passed_value
 
     new_kwargs = _inject_managed_params(pm, sig, new_kwargs, kwargs)
     error_message = ""
     try:
         sig.bind(**new_kwargs)
     except Exception as e:
         error_message = f"It's not possible to call: '{method_name}' because the passed arguments don't match the expected signature.\nError: {e}"
```

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_config.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_config.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_customization/_extension_points.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_customization/_extension_points.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_customization/_plugin_manager.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_customization/_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_fixtures.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_fixtures.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_hooks.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_hooks.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_interrupts.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_interrupts.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_lifecycle.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_lint_action.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_lint_action.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_log_auto_setup.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_log_output_setup.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_managed_parameters.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_managed_parameters.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_protocols.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_protocols.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_remove_refs.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_remove_refs.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_request.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_request.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_request_impl.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_request_impl.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_response.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_response.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_secret/__init__.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_secret/_oauth2_secret.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_secret/_oauth2_secret.py`

 * *Files 10% similar despite different names*

```diff
@@ -146,26 +146,45 @@
     """
 
     def __init__(self, value: dict):
         """
         Args:
             value: A dict with the values meant to be wrapped in this class.
         """
+        from sema4ai.actions._action import get_provider_and_scope_from_annotation_args
+        from sema4ai.actions._variables_scope import (
+            get_validate_and_convert_kwargs_scope,
+        )
 
         access_token = value.get("access_token")
         if not access_token:
             raise KeyError(
                 "Error. The `access_token` key is required to build an OAuth2Secret, but it wasn't passed."
             )
+
+        validate_and_convert_scope = get_validate_and_convert_kwargs_scope()
+
         provider = value.get("provider")
-        if not provider:
-            raise KeyError(
-                "Error. The `provider` key is required to build an OAuth2Secret, but it wasn't passed."
-            )
         scopes = value.get("scopes")
-        if not scopes:
-            raise KeyError(
-                "Error. The `scopes` key is required to build an OAuth2Secret, but it wasn't passed."
-            )
+        if not scopes or not provider:
+            if validate_and_convert_scope is not None:
+                from typing import get_args
+
+                # Use default values from the type hints.
+                args = get_args(validate_and_convert_scope.param_type)
+                (
+                    provider_from_args,
+                    scopes_from_args,
+                ) = get_provider_and_scope_from_annotation_args(
+                    args, "<unavailable>", "<unavailable>"
+                )
+
+                if not provider:
+                    provider = provider_from_args
+
+                if not scopes:
+                    scopes = scopes_from_args
 
         metadata = value.get("metadata")  # This is optional
-        super().__init__(provider, scopes, access_token, metadata)
+        super().__init__(
+            provider or "<unavailable>", scopes or [], access_token, metadata
+        )
```

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/_secret/_secret.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/_secret/_secret.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/api.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/api.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/src/sema4ai/actions/cli.py` & `sema4ai_actions-0.9.0/src/sema4ai/actions/cli.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.8.0/PKG-INFO` & `sema4ai_actions-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema4ai-actions
-Version: 0.8.0
+Version: 0.9.0
 Summary: Sema4AI Actions
 Home-page: https://github.com/Sema4AI/actions/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

