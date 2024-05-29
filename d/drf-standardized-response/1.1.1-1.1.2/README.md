# Comparing `tmp/drf_standardized_response-1.1.1.tar.gz` & `tmp/drf_standardized_response-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_standardized_response-1.1.1.tar", last modified: Wed May  8 10:26:16 2024, max compression
+gzip compressed data, was "drf_standardized_response-1.1.2.tar", last modified: Wed May 29 05:05:15 2024, max compression
```

## Comparing `drf_standardized_response-1.1.1.tar` & `drf_standardized_response-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 10:26:16.880238 drf_standardized_response-1.1.1/
--rw-rw-rw-   0        0        0     1324 2024-05-05 12:23:50.000000 drf_standardized_response-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       60 2024-04-29 15:40:10.000000 drf_standardized_response-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7018 2024-05-08 10:26:16.879238 drf_standardized_response-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5911 2024-05-08 10:14:19.000000 drf_standardized_response-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 10:26:16.862333 drf_standardized_response-1.1.1/drf_standardized_response/
--rw-rw-rw-   0        0        0        0 2024-04-29 15:25:16.000000 drf_standardized_response-1.1.1/drf_standardized_response/__init__.py
--rw-rw-rw-   0        0        0      218 2024-05-05 12:28:04.000000 drf_standardized_response-1.1.1/drf_standardized_response/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:26:16.877238 drf_standardized_response-1.1.1/drf_standardized_response/openapi/
--rw-rw-rw-   0        0        0      185 2024-05-08 10:24:08.000000 drf_standardized_response-1.1.1/drf_standardized_response/openapi/__init__.py
--rw-rw-rw-   0        0        0     2873 2024-05-08 10:22:32.000000 drf_standardized_response-1.1.1/drf_standardized_response/openapi/mixins.py
--rw-rw-rw-   0        0        0      246 2024-05-08 10:09:43.000000 drf_standardized_response-1.1.1/drf_standardized_response/openapi/serializers.py
--rw-rw-rw-   0        0        0      535 2024-05-08 10:09:45.000000 drf_standardized_response-1.1.1/drf_standardized_response/openapi/utils.py
--rw-rw-rw-   0        0        0      800 2024-05-07 10:26:55.000000 drf_standardized_response-1.1.1/drf_standardized_response/renderers.py
--rw-rw-rw-   0        0        0     2888 2024-05-07 10:30:30.000000 drf_standardized_response-1.1.1/drf_standardized_response/response_standarizer.py
--rw-rw-rw-   0        0        0     2627 2024-05-05 16:04:30.000000 drf_standardized_response-1.1.1/drf_standardized_response/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:26:16.878238 drf_standardized_response-1.1.1/drf_standardized_response.egg-info/
--rw-rw-rw-   0        0        0     7018 2024-05-08 10:26:16.000000 drf_standardized_response-1.1.1/drf_standardized_response.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      688 2024-05-08 10:26:16.000000 drf_standardized_response-1.1.1/drf_standardized_response.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 10:26:16.000000 drf_standardized_response-1.1.1/drf_standardized_response.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-08 10:26:16.000000 drf_standardized_response-1.1.1/drf_standardized_response.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-08 10:26:16.000000 drf_standardized_response-1.1.1/drf_standardized_response.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      124 2024-05-06 03:07:32.000000 drf_standardized_response-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1002 2024-05-08 10:26:16.881289 drf_standardized_response-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      122 2024-05-06 03:07:26.000000 drf_standardized_response-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:05:15.399902 drf_standardized_response-1.1.2/
+-rw-rw-rw-   0        0        0     1324 2024-05-05 12:23:50.000000 drf_standardized_response-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0       60 2024-04-29 15:40:10.000000 drf_standardized_response-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7018 2024-05-29 05:05:15.399902 drf_standardized_response-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5911 2024-05-08 10:14:19.000000 drf_standardized_response-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 05:05:15.364317 drf_standardized_response-1.1.2/drf_standardized_response/
+-rw-rw-rw-   0        0        0        0 2024-04-29 15:25:16.000000 drf_standardized_response-1.1.2/drf_standardized_response/__init__.py
+-rw-rw-rw-   0        0        0      218 2024-05-05 12:28:04.000000 drf_standardized_response-1.1.2/drf_standardized_response/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:05:15.396615 drf_standardized_response-1.1.2/drf_standardized_response/openapi/
+-rw-rw-rw-   0        0        0      185 2024-05-08 10:24:08.000000 drf_standardized_response-1.1.2/drf_standardized_response/openapi/__init__.py
+-rw-rw-rw-   0        0        0     3301 2024-05-29 05:04:18.000000 drf_standardized_response-1.1.2/drf_standardized_response/openapi/mixins.py
+-rw-rw-rw-   0        0        0      246 2024-05-08 10:09:43.000000 drf_standardized_response-1.1.2/drf_standardized_response/openapi/serializers.py
+-rw-rw-rw-   0        0        0      535 2024-05-08 10:09:45.000000 drf_standardized_response-1.1.2/drf_standardized_response/openapi/utils.py
+-rw-rw-rw-   0        0        0      800 2024-05-07 10:26:55.000000 drf_standardized_response-1.1.2/drf_standardized_response/renderers.py
+-rw-rw-rw-   0        0        0     2888 2024-05-07 10:30:30.000000 drf_standardized_response-1.1.2/drf_standardized_response/response_standarizer.py
+-rw-rw-rw-   0        0        0     2627 2024-05-05 16:04:30.000000 drf_standardized_response-1.1.2/drf_standardized_response/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:05:15.398646 drf_standardized_response-1.1.2/drf_standardized_response.egg-info/
+-rw-rw-rw-   0        0        0     7018 2024-05-29 05:05:15.000000 drf_standardized_response-1.1.2/drf_standardized_response.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      688 2024-05-29 05:05:15.000000 drf_standardized_response-1.1.2/drf_standardized_response.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 05:05:15.000000 drf_standardized_response-1.1.2/drf_standardized_response.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-29 05:05:15.000000 drf_standardized_response-1.1.2/drf_standardized_response.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-29 05:05:15.000000 drf_standardized_response-1.1.2/drf_standardized_response.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      124 2024-05-06 03:07:32.000000 drf_standardized_response-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1002 2024-05-29 05:05:15.401904 drf_standardized_response-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      122 2024-05-06 03:07:26.000000 drf_standardized_response-1.1.2/setup.py
```

### Comparing `drf_standardized_response-1.1.1/LICENSE` & `drf_standardized_response-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-1.1.1/PKG-INFO` & `drf_standardized_response-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-standardized-response
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://github.com/HasanAshab/drf-standardized-response
 Author: Hasan Ashab
 Author-email: hasanashab.18205@example.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
```

### Comparing `drf_standardized_response-1.1.1/README.md` & `drf_standardized_response-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-1.1.1/drf_standardized_response/openapi/mixins.py` & `drf_standardized_response-1.1.2/drf_standardized_response/openapi/mixins.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from drf_standardized_response.settings import package_settings
 
 
 class StandardizedSchemaMixin:
     def _get_response_for_code(
         self, serializer, status_code, media_types=None, direction="response"
     ):
+        is_array = False
         dummy_request = RequestFactory().get(self.path)
         self._response_standardizer = (
             package_settings.RESPONSE_STANDARDIZER_CLASS(
                 view=self._view,
                 request=dummy_request,
             )
         )
@@ -21,35 +22,43 @@
         )
         if not (content := response.get("content")):
             return response
         if "application/json" not in content:
             return response
 
         schema = content["application/json"]["schema"]
-        reference = schema.get("$ref", schema.get("items", {}).get("$ref"))
+
+        if "items" in schema:
+            is_array = True
+            reference = schema.get("items", {}).get("$ref")
+        else:
+            reference = schema.get("$ref")
         if not reference:
             return response
         if "ErrorResponse" in reference:
             return response
 
         if isinstance(serializer, OpenApiResponse):
             serializer = serializer.response
         serializer_meta = getattr(serializer, "Meta", {})
 
         if not (
             getattr(serializer_meta, "should_standardize_schema", True)
             and self._response_standardizer.should_standardize()
         ):
             return response
+        print(self.path, schema)
 
-        formatted_schema = self._standardize_response_schema(reference)
+        formatted_schema = self._standardize_response_schema(
+            reference, is_array
+        )
         content["application/json"]["schema"] = formatted_schema
         return response
 
-    def _standardize_response_schema(self, reference):
+    def _standardize_response_schema(self, reference, is_array):
         dummy_response = Response(status=200)
         standardized_schema = {
             "type": "object",
             "properties": {
                 "success": {"type": "boolean"},
                 "message": {"type": "string"},
             },
@@ -59,14 +68,21 @@
             return {
                 "allOf": [
                     {"$ref": reference},
                     standardized_schema,
                 ]
             }
 
+        if is_array:
+            standardized_schema["properties"]["data"] = {
+                "type": "array",
+                "items": {"$ref": reference},
+            }
+            return standardized_schema
+
         schema_name = reference.split("/")[-1]
         schema_key = (schema_name, "schemas")
         schema = self.registry._components[schema_key].schema
         unwrapped_fields = (
             self._response_standardizer.get_wrapping_excluded_fields()
         )
         unwrapped_data = {
```

### Comparing `drf_standardized_response-1.1.1/drf_standardized_response/openapi/utils.py` & `drf_standardized_response-1.1.2/drf_standardized_response/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-1.1.1/drf_standardized_response/renderers.py` & `drf_standardized_response-1.1.2/drf_standardized_response/renderers.py`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-1.1.1/drf_standardized_response/response_standarizer.py` & `drf_standardized_response-1.1.2/drf_standardized_response/response_standarizer.py`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-1.1.1/drf_standardized_response/settings.py` & `drf_standardized_response-1.1.2/drf_standardized_response/settings.py`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-1.1.1/drf_standardized_response.egg-info/PKG-INFO` & `drf_standardized_response-1.1.2/drf_standardized_response.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-standardized-response
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://github.com/HasanAshab/drf-standardized-response
 Author: Hasan Ashab
 Author-email: hasanashab.18205@example.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
```

### Comparing `drf_standardized_response-1.1.1/drf_standardized_response.egg-info/SOURCES.txt` & `drf_standardized_response-1.1.2/drf_standardized_response.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-1.1.1/setup.cfg` & `drf_standardized_response-1.1.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 7266 2d73 7461 6e64 6172 6469   = drf-standardi
 00000020: 7a65 642d 7265 7370 6f6e 7365 0d0a 7665  zed-response..ve
-00000030: 7273 696f 6e20 3d20 312e 312e 310d 0a6c  rsion = 1.1.1..l
+00000030: 7273 696f 6e20 3d20 312e 312e 320d 0a6c  rsion = 1.1.2..l
 00000040: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000050: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
 00000060: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
 00000070: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
 00000080: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
 00000090: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
 000000a0: 6769 7468 7562 2e63 6f6d 2f48 6173 616e  github.com/Hasan
```

