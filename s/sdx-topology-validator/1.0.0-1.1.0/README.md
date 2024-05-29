# Comparing `tmp/sdx_topology_validator-1.0.0.tar.gz` & `tmp/sdx_topology_validator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdx_topology_validator-1.0.0.tar", last modified: Wed May 22 14:55:24 2024, max compression
+gzip compressed data, was "sdx_topology_validator-1.1.0.tar", last modified: Wed May 29 11:52:43 2024, max compression
```

## Comparing `sdx_topology_validator-1.0.0.tar` & `sdx_topology_validator-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 14:55:24.443092 sdx_topology_validator-1.0.0/
--rw-rw-rw-   0        0        0      433 2024-05-22 14:55:24.441457 sdx_topology_validator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       85 2024-05-20 20:43:28.000000 sdx_topology_validator-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 14:55:24.397705 sdx_topology_validator-1.0.0/sdx_topology_validator/
--rw-rw-rw-   0        0        0      131 2024-05-22 14:46:19.000000 sdx_topology_validator-1.0.0/sdx_topology_validator/__init__.py
--rw-rw-rw-   0        0        0      889 2024-05-20 18:53:05.000000 sdx_topology_validator-1.0.0/sdx_topology_validator/sdx_topology_validator.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:55:24.439469 sdx_topology_validator-1.0.0/sdx_topology_validator.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-22 14:55:24.000000 sdx_topology_validator-1.0.0/sdx_topology_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-05-22 14:55:24.000000 sdx_topology_validator-1.0.0/sdx_topology_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 14:55:24.000000 sdx_topology_validator-1.0.0/sdx_topology_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-22 14:55:24.000000 sdx_topology_validator-1.0.0/sdx_topology_validator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-22 14:55:24.000000 sdx_topology_validator-1.0.0/sdx_topology_validator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 14:55:24.443092 sdx_topology_validator-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      486 2024-05-22 14:53:21.000000 sdx_topology_validator-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:52:43.533860 sdx_topology_validator-1.1.0/
+-rw-rw-rw-   0        0        0     2226 2024-05-29 11:52:43.531111 sdx_topology_validator-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1878 2024-05-29 11:45:46.000000 sdx_topology_validator-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 11:52:43.474599 sdx_topology_validator-1.1.0/sdx_topology_validator/
+-rw-rw-rw-   0        0        0      131 2024-05-29 11:19:32.000000 sdx_topology_validator-1.1.0/sdx_topology_validator/__init__.py
+-rw-rw-rw-   0        0        0      979 2024-05-29 11:35:13.000000 sdx_topology_validator-1.1.0/sdx_topology_validator/sdx_topology_validator.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:52:43.530127 sdx_topology_validator-1.1.0/sdx_topology_validator.egg-info/
+-rw-rw-rw-   0        0        0     2226 2024-05-29 11:52:43.000000 sdx_topology_validator-1.1.0/sdx_topology_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-05-29 11:52:43.000000 sdx_topology_validator-1.1.0/sdx_topology_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:52:43.000000 sdx_topology_validator-1.1.0/sdx_topology_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-29 11:52:43.000000 sdx_topology_validator-1.1.0/sdx_topology_validator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-29 11:52:43.000000 sdx_topology_validator-1.1.0/sdx_topology_validator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:52:43.534873 sdx_topology_validator-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      486 2024-05-29 11:45:52.000000 sdx_topology_validator-1.1.0/setup.py
```

### Comparing `sdx_topology_validator-1.0.0/sdx_topology_validator/sdx_topology_validator.py` & `sdx_topology_validator-1.1.0/sdx_topology_validator/sdx_topology_validator.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 def resolve_references(openapi_spec):
     return jsonref.JsonRef.replace_refs(openapi_spec)
 
 def get_validator_schema(openapi_spec):
     return openapi_spec['paths']['/validator']['post']['requestBody']['content']['application/json']['schema']
 
-def validate(data, schema):
+def validate(data):
     """Validate the converted topology data against the OpenAPI schema."""
+    validator_schema = get_validator_schema(resolve_references(load_openapi_schema('./validator.yaml')))
     try:
-        json_validate(instance=data, schema=schema)
+        json_validate(data, validator_schema)
         return {"result": "Validated Successfully", "status_code": 200}
     except ValidationError as e:
-        return {"result": f"Validation Error: {e.message}", "status_code": 400}
+        return {"result": f"Validation Error: {e.message}", "status_code": 400}
```

