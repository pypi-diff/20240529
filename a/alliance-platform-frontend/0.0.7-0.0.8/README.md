# Comparing `tmp/alliance_platform_frontend-0.0.7.tar.gz` & `tmp/alliance_platform_frontend-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alliance_platform_frontend-0.0.7.tar", last modified: Thu May 16 19:21:10 2024, max compression
+gzip compressed data, was "alliance_platform_frontend-0.0.8.tar", last modified: Wed May 29 00:53:09 2024, max compression
```

## Comparing `alliance_platform_frontend-0.0.7.tar` & `alliance_platform_frontend-0.0.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     2946 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/README.md
--rw-r--r--   0        0        0       22 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/__init__.py
--rw-r--r--   0        0        0     1265 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/button.py
--rw-r--r--   0        0        0     1944 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/date_picker.py
--rw-r--r--   0        0        0     2524 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/icon.py
--rw-r--r--   0        0        0     1528 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/inline_alert.py
--rw-r--r--   0        0        0     2141 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/menubar.py
--rw-r--r--   0        0        0      914 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/misc.py
--rw-r--r--   0        0        0     1720 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/pagination.py
--rw-r--r--   0        0        0     3070 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/table.py
--rw-r--r--   0        0        0     1225 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/time_input.py
--rw-r--r--   0        0        0     1243 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/utils.py
--rw-r--r--   0        0        0      358 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/apps.py
--rw-r--r--   0        0        0      633 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/__init__.py
--rw-r--r--   0        0        0     2402 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/asset_registry.py
--rw-r--r--   0        0        0    16050 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/base.py
--rw-r--r--   0        0        0    17210 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/context.py
--rw-r--r--   0        0        0     2507 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/middleware.py
--rw-r--r--   0        0        0    13537 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/ssr.py
--rw-r--r--   0        0        0     7051 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/vanilla_extract.py
--rw-r--r--   0        0        0    34218 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/vite.py
--rw-r--r--   0        0        0      175 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/vitePreload.ts
--rw-r--r--   0        0        0    11144 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/dom_possible_standard_names.py
--rw-r--r--   0        0        0        0 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/forms/__init__.py
--rw-r--r--   0        0        0     1620 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/forms/renderers.py
--rw-r--r--   0        0        0     5340 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/management/commands/extract_frontend_assets.py
--rw-r--r--   0        0        0     9471 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/prop_handlers.py
--rw-r--r--   0        0        0        0 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/py.typed
--rw-r--r--   0        0        0     8806 2024-05-16 19:20:48.861013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/settings.py
--rw-r--r--   0        0        0     2684 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/templates/bundler_dev_check.html
--rw-r--r--   0        0        0        0 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/templatetags/__init__.py
--rw-r--r--   0        0        0     5451 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/templatetags/alliance_ui.py
--rw-r--r--   0        0        0    13141 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/templatetags/bundler.py
--rw-r--r--   0        0        0     8972 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/templatetags/form.py
--rw-r--r--   0        0        0    63721 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/templatetags/react.py
--rw-r--r--   0        0        0     4316 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/templatetags/vanilla_extract.py
--rw-r--r--   0        0        0     3283 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/alliance_platform/frontend/util.py
--rw-r--r--   0        0        0     2331 2024-05-16 19:21:10.789618 alliance_platform_frontend-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     2503 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/tests/fixtures/build_test/manifest.json
--rw-r--r--   0        0        0       39 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/tests/fixtures/development-css-mappings/login_css_ts.json
--rw-r--r--   0        0        0       30 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/tests/fixtures/production-css-mappings/login_css_ts.json
--rw-r--r--   0        0        0      648 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/tests/fixtures/server_build_test/manifest.json
--rw-r--r--   0        0        0     7955 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/tests/test_alliance_ui_templatetags.py
--rw-r--r--   0        0        0    12764 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/tests/test_bundler.py
--rw-r--r--   0        0        0    41823 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/tests/test_bundler_templatetags.py
--rw-r--r--   0        0        0     5837 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/tests/test_context.py
--rw-r--r--   0        0        0      721 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     2384 2024-05-16 19:20:48.865013 alliance_platform_frontend-0.0.7/tests/test_utils/bundler.py
--rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 alliance_platform_frontend-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2946 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/README.md
+-rw-r--r--   0        0        0       22 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/__init__.py
+-rw-r--r--   0        0        0     1265 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/button.py
+-rw-r--r--   0        0        0     1944 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/date_picker.py
+-rw-r--r--   0        0        0     2524 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/icon.py
+-rw-r--r--   0        0        0     1528 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/inline_alert.py
+-rw-r--r--   0        0        0     2141 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/menubar.py
+-rw-r--r--   0        0        0      914 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/misc.py
+-rw-r--r--   0        0        0     1720 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/pagination.py
+-rw-r--r--   0        0        0     3070 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/table.py
+-rw-r--r--   0        0        0     1225 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/time_input.py
+-rw-r--r--   0        0        0     1243 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/utils.py
+-rw-r--r--   0        0        0      358 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/apps.py
+-rw-r--r--   0        0        0      633 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/__init__.py
+-rw-r--r--   0        0        0     2402 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/asset_registry.py
+-rw-r--r--   0        0        0    16209 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/base.py
+-rw-r--r--   0        0        0    17603 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/context.py
+-rw-r--r--   0        0        0     2507 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/middleware.py
+-rw-r--r--   0        0        0    13544 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/ssr.py
+-rw-r--r--   0        0        0     7051 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/vanilla_extract.py
+-rw-r--r--   0        0        0    34928 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/vite.py
+-rw-r--r--   0        0        0      175 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/vitePreload.ts
+-rw-r--r--   0        0        0    11144 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/dom_possible_standard_names.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/forms/__init__.py
+-rw-r--r--   0        0        0     1620 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/forms/renderers.py
+-rw-r--r--   0        0        0     5340 2024-05-29 00:52:33.748732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/management/commands/extract_frontend_assets.py
+-rw-r--r--   0        0        0     9471 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/prop_handlers.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/py.typed
+-rw-r--r--   0        0        0     8988 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/settings.py
+-rw-r--r--   0        0        0     2684 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/templates/bundler_dev_check.html
+-rw-r--r--   0        0        0        0 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/templatetags/__init__.py
+-rw-r--r--   0        0        0     5451 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/templatetags/alliance_ui.py
+-rw-r--r--   0        0        0    13141 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/templatetags/bundler.py
+-rw-r--r--   0        0        0     8972 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/templatetags/form.py
+-rw-r--r--   0        0        0    64016 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/templatetags/react.py
+-rw-r--r--   0        0        0     4316 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/templatetags/vanilla_extract.py
+-rw-r--r--   0        0        0     3283 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/alliance_platform/frontend/util.py
+-rw-r--r--   0        0        0     2331 2024-05-29 00:53:09.720814 alliance_platform_frontend-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     2503 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/tests/fixtures/build_test/manifest.json
+-rw-r--r--   0        0        0       39 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/tests/fixtures/development-css-mappings/login_css_ts.json
+-rw-r--r--   0        0        0       30 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/tests/fixtures/production-css-mappings/login_css_ts.json
+-rw-r--r--   0        0        0      648 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/tests/fixtures/server_build_test/manifest.json
+-rw-r--r--   0        0        0     7955 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/tests/test_alliance_ui_templatetags.py
+-rw-r--r--   0        0        0    12764 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/tests/test_bundler.py
+-rw-r--r--   0        0        0    42181 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/tests/test_bundler_templatetags.py
+-rw-r--r--   0        0        0     5837 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/tests/test_context.py
+-rw-r--r--   0        0        0      721 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     2384 2024-05-29 00:52:33.752732 alliance_platform_frontend-0.0.8/tests/test_utils/bundler.py
+-rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 alliance_platform_frontend-0.0.8/PKG-INFO
```

### Comparing `alliance_platform_frontend-0.0.7/README.md` & `alliance_platform_frontend-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/button.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/button.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/date_picker.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/date_picker.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/icon.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/icon.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/inline_alert.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/inline_alert.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/menubar.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/menubar.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/misc.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/misc.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/pagination.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/pagination.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/table.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/table.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/time_input.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/time_input.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/alliance_ui/utils.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/alliance_ui/utils.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/__init__.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/__init__.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/asset_registry.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/asset_registry.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/base.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,18 @@
     #: A list of :class:`~alliance_platform.frontend.bundler.base.PathResolver` instances used to resolve paths
     path_resolvers: list[PathResolver]
 
     def __init__(self, root_dir: Path, path_resolvers: list[PathResolver]):
         self.root_dir = root_dir
         self.path_resolvers = path_resolvers
 
+    def is_ssr_enabled(self) -> bool:
+        """Should return true if server side rendering is enabled and supported by this bundler"""
+        return False
+
     def is_development(self) -> bool:
         """Should return true if running in development mode"""
         raise NotImplementedError
 
     def get_url(self, path: Path | str):
         """Return the URL to load the specified asset at ``path``"""
         raise NotImplementedError
```

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/context.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,21 +242,27 @@
         if not hasattr(GLOBAL_BUNDLER_ASSET_CONTEXT, "contexts") or not GLOBAL_BUNDLER_ASSET_CONTEXT.contexts:
             raise NoActiveBundlerAssetContext("No context currently active")
         return GLOBAL_BUNDLER_ASSET_CONTEXT.contexts[-1]
 
     def queue_ssr(self, item: SSRItem) -> str:
         """Queue an item for server side rendering
 
+        Note that if the current bundler does not support SSR, this will have no effect. You can safely call it still
+        and output the placeholder HTML comment, it just will not be replaced with anything.
+
         Args:
             item: The item to render
 
         Returns:
             A string which is the placeholder that should be outputted in the HTML. It will be replaced by
             :class:`~alliance_platform.frontend.bundler.middleware.BundlerAssetContextMiddleware`.
         """
+        if not get_bundler().is_ssr_enabled():
+            # Include a comment to make it clear SSR is not enabled to assist debugging
+            return "<!-- SSR NOT ENABLED -->"
         if not self.is_middleware_registered:
             raise ValueError(
                 "`queue_ssr` cannot be used without `BundlerAssetContextMiddleware`. Add 'alliance_platform.frontend.bundler.middleware.BundlerAssetContextMiddleware' to `MIDDLEWARE`."
             )
         placeholder = f"<!-- ___SSR_PLACEHOLDER_{len(self.ssr_queue)}___ -->"
         self.ssr_queue[placeholder] = item
         return placeholder
```

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/middleware.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/middleware.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/ssr.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/ssr.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         in preview or production.
         """
 
         # If dev the rendering happens in dev-server.ts
         bundler = get_bundler()
         ssr_url = bundler.get_ssr_url()
         if not ssr_url:
-            logger.error("Can not perform SSR, no SSR URL defined. Set PRODUCTION_SSR_URL env var.")
+            logger.error("Can not perform SSR, no SSR URL defined. Set `production_ssr_url` on the bundler.")
             return None
         try:
             json_payload = json.dumps(payload, cls=DjangoJSONEncoder)
             ssr_response = requests.post(
                 ssr_url,
                 data=json_payload,
                 headers={"Content-Type": "application/json", **bundler.get_ssr_headers()},
@@ -246,17 +246,17 @@
                 except JSONDecodeError:
                     logger.error(
                         f"Failed to decode JSON from server rendering, content received: {ssr_response.content.decode()}"
                     )
         except TypeError:
             logger.exception(f"Failed to encode JSON for server rendering. Payload was: {payload}")
         except requests.exceptions.Timeout:
-            logger.error("Timed out connecting to vite server for rendering")
+            logger.error("Timed out connecting to SSR server for rendering")
         except requests.exceptions.ConnectionError:
-            logger.error("Failed to connect to vite server for rendering - is it running?")
+            logger.error("Failed to connect to SSR server for rendering - is it running?")
         return None
 
     def process(self, content: str | bytes, global_context: dict):
         if not self.ssr_queue:
             return content
         ssr_context = SSRSerializerContext(get_bundler())
         # items are serialized first so that `ssr_context` can be populated with the required imports
```

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/vanilla_extract.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/vanilla_extract.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/bundler/vite.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/bundler/vite.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,15 +262,14 @@
 
 class ViteBundler(BaseBundler):
     """Bundler implementation for `Vite <https://vitejs.dev/>`_.
 
     Args:
         root_dir: The root path everything sits under; all other paths are resolved relative to this
         path_resolvers: A list of :class:`~alliance_platform.frontend.bundler.base.PathResolver` instances used to resolve paths
-        server_build_dir: The directory SSR files are outputted to (see ``yarn build:ssr``)
         build_dir: The directory client side files are outputted to (see ``yarn build:client``)
         server_host: The hostname used for the dev server (e.g. ``127.0.0.1``)
         server_port: The port used for the dev server (e.g. ``5173``)
         server_protocol: The protocol used for the dev server (``http`` or ``https``)
         server_resolve_package_url: The URL, handled by the dev server, to use to resolve package requests in dev mode. This is
             only used for packages in /node_modules/ so that we can use the optimized versions of packages that Vite generates.
             Without this, you encounter errors like "Outdated Optimized Deps". The dev server should handle requests to this
@@ -286,61 +285,72 @@
                     // Convert the filesystem path to a web-accessible path
                     const url = path.join(vite.config.base, relativePath);
                     res.redirect(302, url);
                 });
         mode: The mode the bundler is running in; one of ``development``, ``production`` or ``preview``
         wait_for_server: Function that can be passed that will be called before requesting assets for server. This function
             should handle waiting until the dev server is ready before returning (e.g. by polling the server status)
-        production_ssr_url: URL for SSR (only used in production mode)
+        disable_ssr: Set to ``True`` to disable SSR entirely. Defaults to ``False``.
+        server_build_dir: The directory SSR files are outputted to (see ``yarn build:ssr``). Required unless ``disable_ssr`` is ``True``.
+        production_ssr_url: URL for SSR (only used in production mode). Required unless ``disable_ssr`` is ``True``.
 
     """
 
-    #: Directory server side rendering (SSR) files are compiled to
-    server_build_dir: Path
+    #: Directory server side rendering (SSR) files are compiled to. May be ``None`` if ``disable_ssr`` is ``True``.
+    server_build_dir: Path | None
     #: Directory client side files are compiled to
     build_dir: Path
     #: Manifest for SSR (only available when in production mode)
     server_build_manifest: ViteManifest
     #: Manifest for client build (only available when in production mode)
     build_manifest: ViteManifest
     #: The mode bundler is running in; either 'development', 'production' or 'preview'
     mode: str
     #: URL for SSR (only used in production mode)
     production_ssr_url: str | None
     #: Function that can be passed that will be called before requesting assets for server.
     wait_for_server: Callable[[], None] | None = None
     #: Path to the vite metdata JSON file that we use in dev to resolve optimised deps
     vite_metadata_path: Path
+    #: Can be set to disable SSR entirely
+    disable_ssr: bool = False
 
     def __init__(
         self,
         *,
         root_dir: Path,
         path_resolvers: list[PathResolver],
-        server_build_dir: Path,
         build_dir: Path,
         server_host: str,
         server_port: str,
         server_protocol: str,
         server_resolve_package_url: str,
         mode: str,
-        production_ssr_url: str | None = None,
         wait_for_server: Callable[[], None] | None = None,
+        disable_ssr: bool = False,
+        # These options are not required if ``disable_ssr`` is ``True``
+        server_build_dir: Path | None = None,
+        production_ssr_url: str | None = None,
     ):
-        self.wait_for_server = wait_for_server
         valid_modes = ["development", "production", "preview"]
         if mode not in valid_modes:
             raise ValueError(f"'mode' must be one of {', '.join(valid_modes)}, received: '{mode}'")
+        if not server_build_dir and not disable_ssr:
+            raise ValueError("server_build_dir must be set if SSR is enabled")
         super().__init__(root_dir, path_resolvers)
+
+        self.disable_ssr = disable_ssr
+        self.wait_for_server = wait_for_server
         self.mode = mode
         self.server_build_dir = server_build_dir
         self.build_dir = build_dir
         self.node_modules_dir = ap_frontend_settings.NODE_MODULES_DIR
         if self.mode != "development":
-            self.server_build_manifest = ViteManifest(self.root_dir, server_build_dir / "manifest.json")
+            if server_build_dir:
+                self.server_build_manifest = ViteManifest(self.root_dir, server_build_dir / "manifest.json")
             self.build_manifest = ViteManifest(self.root_dir, build_dir / "manifest.json")
         self.dev_server_url_base = ""
         self.dev_server_url = ""
         self.production_ssr_url = production_ssr_url
         if mode == "development":
             static_url = settings.STATIC_URL
             if not static_url:
@@ -359,14 +369,17 @@
                 self.dev_server_url_base, server_resolve_package_url
             )
             if not self.dev_server_resolve_package_url.endswith("/"):
                 self.dev_server_resolve_package_url += "/"
         elif mode == "preview":
             self.preview_url = f"{server_protocol}://{server_host}:{server_port}"
 
+    def is_ssr_enabled(self) -> bool:
+        return not self.disable_ssr
+
     def resolve_url(self, path: Path | str):
         """Resolve a URL to use to serve the specified ``path``
 
         In development this will be served from the dev server and in production from ``STATIC_URL``
         """
         if self.wait_for_server:
             self.wait_for_server()
```

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/dom_possible_standard_names.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/dom_possible_standard_names.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/forms/renderers.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/forms/renderers.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/management/commands/extract_frontend_assets.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/management/commands/extract_frontend_assets.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/prop_handlers.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/prop_handlers.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/settings.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
     FRONTEND_ASSET_REGISTRY: Union[str, "FrontendAssetRegistry"]
     #: A list of either ``re.Pattern`` or a :class:`~pathlib.Path`. If a template directory matches any entry it will be excluded from :class:`extract_frontend_assets <alliance_platform.frontend.management.commands.extract_frontend_assets.Command>`.
     #:
     #: If a :class:`~pathlib.Path` is used it will be checked if the directory starts with that path. Otherwise a ``re.Pattern`` will exclude a directory if it matches.
     EXTRACT_ASSETS_EXCLUDE_DIRS: tuple[Path | str, Pattern[str]]
     #: If set to a truthy value :func:`~alliance_platform.frontend.templatetags.bundler.bundler_dev_checks` will not display any HTML error, the error will only be available in the Django dev console.
     BUNDLER_DISABLE_DEV_CHECK_HTML: bool | None
-    #: The path to the node_modules directory. This is used by ViteBundler to resolve optimized deps, and extract_frontend_assets to determine when an import comes from node_modules directly.
+    #: The path to the node_modules directory. This is used by ViteBundler to resolve optimized deps, and extract_frontend_assets to determine when an import comes from node_modules directly. It is used
+    #: by some codegen post processors to run node scripts (e.g. prettier or eslint). It is not used in production, so the directory does not need to exist in production.
     NODE_MODULES_DIR: Path | str
     #: The directory production assets exists in. This directory should include the Vanilla Extract mappings.
     PRODUCTION_DIR: Path
     #: Any custom prop handlers to use for react components. This can be a string import path to a list of prop handlers, or the list directly.
     REACT_PROP_HANDLERS: str | list[type["ComponentProp"]]
     #: File that is used to render React components using the ``react`` tag. This file should export a function named ``renderComponent`` and a function ``createElement`` (this can just be re-exported from React).
     REACT_RENDER_COMPONENT_FILE: Path | str
```

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/templates/bundler_dev_check.html` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/templates/bundler_dev_check.html`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/templatetags/alliance_ui.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/templatetags/alliance_ui.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/templatetags/bundler.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/templatetags/bundler.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/templatetags/form.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/templatetags/form.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/templatetags/react.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/templatetags/react.py`

 * *Files 1% similar despite different names*

```diff
@@ -955,14 +955,19 @@
 
     def resolve_prop(self, value, context: Context):
         """Handles resolving values to a type that can be serialized
 
         If you add new :class:`~alliance_platform.frontend.prop_handlers.ComponentProp` there must a case here
         to convert values to the new type.
         """
+
+        # In the case of raw HTML that is transformed with the ``convert_html_string`` function we need to handle
+        # the case of a template node being used as a prop, e.g. ``<a href="{% url 'some-url' %}">``.
+        if isinstance(value, Node):
+            value = value.render(context)
         if isinstance(value, DeferredProp):
             value = value.resolve(context)
         if isinstance(value, (ChildrenList, NodeList)):
             children: list[str | NestedComponentProp] = []
             for child in value:
                 if isinstance(child, ComponentNode):
                     # We could remove this branch - it's an optimisation of the below. We know the node type here
```

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/templatetags/vanilla_extract.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/templatetags/vanilla_extract.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/alliance_platform/frontend/util.py` & `alliance_platform_frontend-0.0.8/alliance_platform/frontend/util.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/pyproject.toml` & `alliance_platform_frontend-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 include = [
     "alliance_platform/frontend/py.typed",
 ]
-version = "0.0.7"
+version = "0.0.8"
 
 [project.license]
 text = "BSD-2-Clause"
 
 [project.urls]
 issues = "https://github.com/AllianceSoftware/alliance-platform-py/issues"
 homepage = "https://github.com/AllianceSoftware/alliance-platform-py/packages/ap-frontend"
```

### Comparing `alliance_platform_frontend-0.0.7/tests/fixtures/build_test/manifest.json` & `alliance_platform_frontend-0.0.8/tests/fixtures/build_test/manifest.json`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/tests/fixtures/server_build_test/manifest.json` & `alliance_platform_frontend-0.0.8/tests/fixtures/server_build_test/manifest.json`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/tests/test_alliance_ui_templatetags.py` & `alliance_platform_frontend-0.0.8/tests/test_alliance_ui_templatetags.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/tests/test_bundler.py` & `alliance_platform_frontend-0.0.8/tests/test_bundler.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/tests/test_bundler_templatetags.py` & `alliance_platform_frontend-0.0.8/tests/test_bundler_templatetags.py`

 * *Files 0% similar despite different names*

```diff
@@ -929,7 +929,16 @@
     def test_html_in_var_nested(self):
         self.assertComponentEqual(
             """
             {% component "div" %}{{ text }}{% endcomponent %}""",
             """<div><strong>Should not be <i>escaped</i></strong></div>""",
             text=mark_safe("<strong>Should not be <i>escaped</i></strong>"),
         )
+
+    def test_html_template_node_props(self):
+        """Tests that a template node is resolved when used as a prop to raw HTML"""
+        self.assertComponentEqual(
+            """
+            {% component "div" %}<a href="{{ url }}">Test</a>{% endcomponent %}""",
+            """<div><a href="/test/">Test</a></div>""",
+            url="/test/",
+        )
```

### Comparing `alliance_platform_frontend-0.0.7/tests/test_context.py` & `alliance_platform_frontend-0.0.8/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/tests/test_utils/__init__.py` & `alliance_platform_frontend-0.0.8/tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/tests/test_utils/bundler.py` & `alliance_platform_frontend-0.0.8/tests/test_utils/bundler.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.7/PKG-INFO` & `alliance_platform_frontend-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alliance-platform-frontend
-Version: 0.0.7
+Version: 0.0.8
 Summary: Django integration for Frontend Bundlers & React
 Keywords: django,alliance,alliancesoftware
 Home-page: https://github.com/AllianceSoftware/alliance-platform-py/packages/ap-frontend
 Author-Email: Alliance Software <support@alliancesoftware.com.au>
 License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

