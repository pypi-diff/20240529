# Comparing `tmp/sdx_topology_validator-1.1.0.tar.gz` & `tmp/sdx_topology_validator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdx_topology_validator-1.1.0.tar", last modified: Wed May 29 11:52:43 2024, max compression
+gzip compressed data, was "sdx_topology_validator-1.1.1.tar", last modified: Wed May 29 19:02:39 2024, max compression
```

## Comparing `sdx_topology_validator-1.1.0.tar` & `sdx_topology_validator-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 11:52:43.533860 sdx_topology_validator-1.1.0/
--rw-rw-rw-   0        0        0     2226 2024-05-29 11:52:43.531111 sdx_topology_validator-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1878 2024-05-29 11:45:46.000000 sdx_topology_validator-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 11:52:43.474599 sdx_topology_validator-1.1.0/sdx_topology_validator/
--rw-rw-rw-   0        0        0      131 2024-05-29 11:19:32.000000 sdx_topology_validator-1.1.0/sdx_topology_validator/__init__.py
--rw-rw-rw-   0        0        0      979 2024-05-29 11:35:13.000000 sdx_topology_validator-1.1.0/sdx_topology_validator/sdx_topology_validator.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:52:43.530127 sdx_topology_validator-1.1.0/sdx_topology_validator.egg-info/
--rw-rw-rw-   0        0        0     2226 2024-05-29 11:52:43.000000 sdx_topology_validator-1.1.0/sdx_topology_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-05-29 11:52:43.000000 sdx_topology_validator-1.1.0/sdx_topology_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 11:52:43.000000 sdx_topology_validator-1.1.0/sdx_topology_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-29 11:52:43.000000 sdx_topology_validator-1.1.0/sdx_topology_validator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-29 11:52:43.000000 sdx_topology_validator-1.1.0/sdx_topology_validator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 11:52:43.534873 sdx_topology_validator-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      486 2024-05-29 11:45:52.000000 sdx_topology_validator-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:02:39.637336 sdx_topology_validator-1.1.1/
+-rw-rw-rw-   0        0        0     2228 2024-05-29 19:02:39.636348 sdx_topology_validator-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1880 2024-05-29 19:02:04.000000 sdx_topology_validator-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 19:02:39.569008 sdx_topology_validator-1.1.1/sdx_topology_validator/
+-rw-rw-rw-   0        0        0      131 2024-05-29 11:19:32.000000 sdx_topology_validator-1.1.1/sdx_topology_validator/__init__.py
+-rw-rw-rw-   0        0        0     1029 2024-05-29 18:55:54.000000 sdx_topology_validator-1.1.1/sdx_topology_validator/sdx_topology_validator.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:02:39.635337 sdx_topology_validator-1.1.1/sdx_topology_validator.egg-info/
+-rw-rw-rw-   0        0        0     2228 2024-05-29 19:02:39.000000 sdx_topology_validator-1.1.1/sdx_topology_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-05-29 19:02:39.000000 sdx_topology_validator-1.1.1/sdx_topology_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 19:02:39.000000 sdx_topology_validator-1.1.1/sdx_topology_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-29 19:02:39.000000 sdx_topology_validator-1.1.1/sdx_topology_validator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-29 19:02:39.000000 sdx_topology_validator-1.1.1/sdx_topology_validator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 19:02:39.638336 sdx_topology_validator-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      586 2024-05-29 18:57:22.000000 sdx_topology_validator-1.1.1/setup.py
```

### Comparing `sdx_topology_validator-1.1.0/PKG-INFO` & `sdx_topology_validator-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdx_topology_validator
-Version: 1.1.0
+Version: 1.1.1
 Summary: Validates the converted topology against the given OpenAPI specifications
 Author: Sai Krishna Voruganti
 Author-email: saikrishnavoruganti@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
 Requires-Dist: jsonref
 Requires-Dist: jsonschema
@@ -36,12 +36,12 @@
 The function named 'resolve_references' that takes a single parameter 'openapi_spec', resolves any JSON references in the OpenAPI specification, ensuring that all $ref fields are fully expanded.  
 
 The function named 'get_validator_schema' that takes a single parameter, which is the value returned by the function 'resolve_references'.   This function extracts and returns the JSON schema used for validating the request body of the /validator endpoint from the OpenAPI specification.  
 
 The function named 'validate' that take one parameter: data.  
 The first parameter 'data' takes json data as input and validates the given data against the provided JSON schema and returns the result of the validation.     
 
-Note: Make sure that 'validator.yaml' the yaml_spec_file is present in the current directory, where you are validating the json data.  
+Note: 'validator.yaml' the yaml_spec_file is packaged with 'sdx-topology-validator' module, so no need of having it from the user side.  
 
 Example of usage:    
 from sdx_topology_validator import validate      
 validation_result = validate(data)
```

### Comparing `sdx_topology_validator-1.1.0/README.md` & `sdx_topology_validator-1.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 The function named 'resolve_references' that takes a single parameter 'openapi_spec', resolves any JSON references in the OpenAPI specification, ensuring that all $ref fields are fully expanded.  
 
 The function named 'get_validator_schema' that takes a single parameter, which is the value returned by the function 'resolve_references'.   This function extracts and returns the JSON schema used for validating the request body of the /validator endpoint from the OpenAPI specification.  
 
 The function named 'validate' that take one parameter: data.  
 The first parameter 'data' takes json data as input and validates the given data against the provided JSON schema and returns the result of the validation.     
 
-Note: Make sure that 'validator.yaml' the yaml_spec_file is present in the current directory, where you are validating the json data.  
+Note: 'validator.yaml' the yaml_spec_file is packaged with 'sdx-topology-validator' module, so no need of having it from the user side.  
 
 Example of usage:    
 from sdx_topology_validator import validate      
 validation_result = validate(data)
```

### Comparing `sdx_topology_validator-1.1.0/sdx_topology_validator/sdx_topology_validator.py` & `sdx_topology_validator-1.1.1/sdx_topology_validator/sdx_topology_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import yaml
-import jsonref 
+import jsonref
 from jsonschema import validate as json_validate
 from jsonschema.exceptions import ValidationError
+import importlib.resources as pkg_resources
 
-def load_openapi_schema(file_path):
-    with open(file_path, 'r') as file:
+def load_openapi_schema():
+    with pkg_resources.open_text(__name__, 'validator.yaml') as file:
         openapi_spec = yaml.safe_load(file)
     return openapi_spec
 
 def resolve_references(openapi_spec):
     return jsonref.JsonRef.replace_refs(openapi_spec)
 
 def get_validator_schema(openapi_spec):
     return openapi_spec['paths']['/validator']['post']['requestBody']['content']['application/json']['schema']
 
 def validate(data):
     """Validate the converted topology data against the OpenAPI schema."""
-    validator_schema = get_validator_schema(resolve_references(load_openapi_schema('./validator.yaml')))
+    validator_schema = get_validator_schema(resolve_references(load_openapi_schema()))
     try:
         json_validate(data, validator_schema)
         return {"result": "Validated Successfully", "status_code": 200}
     except ValidationError as e:
-        return {"result": f"Validation Error: {e.message}", "status_code": 400}
+        return {"result": f"Validation Error: {e.message}", "status_code": 400}
```

### Comparing `sdx_topology_validator-1.1.0/sdx_topology_validator.egg-info/PKG-INFO` & `sdx_topology_validator-1.1.1/sdx_topology_validator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdx_topology_validator
-Version: 1.1.0
+Version: 1.1.1
 Summary: Validates the converted topology against the given OpenAPI specifications
 Author: Sai Krishna Voruganti
 Author-email: saikrishnavoruganti@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
 Requires-Dist: jsonref
 Requires-Dist: jsonschema
@@ -36,12 +36,12 @@
 The function named 'resolve_references' that takes a single parameter 'openapi_spec', resolves any JSON references in the OpenAPI specification, ensuring that all $ref fields are fully expanded.  
 
 The function named 'get_validator_schema' that takes a single parameter, which is the value returned by the function 'resolve_references'.   This function extracts and returns the JSON schema used for validating the request body of the /validator endpoint from the OpenAPI specification.  
 
 The function named 'validate' that take one parameter: data.  
 The first parameter 'data' takes json data as input and validates the given data against the provided JSON schema and returns the result of the validation.     
 
-Note: Make sure that 'validator.yaml' the yaml_spec_file is present in the current directory, where you are validating the json data.  
+Note: 'validator.yaml' the yaml_spec_file is packaged with 'sdx-topology-validator' module, so no need of having it from the user side.  
 
 Example of usage:    
 from sdx_topology_validator import validate      
 validation_result = validate(data)
```

