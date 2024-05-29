# Comparing `tmp/ioxio_data_product_definition_tooling-0.5.0.tar.gz` & `tmp/ioxio_data_product_definition_tooling-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioxio_data_product_definition_tooling-0.5.0.tar", max compression
+gzip compressed data, was "ioxio_data_product_definition_tooling-0.6.0.tar", max compression
```

## Comparing `ioxio_data_product_definition_tooling-0.5.0.tar` & `ioxio_data_product_definition_tooling-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1496 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/LICENSE
--rw-r--r--   0        0        0      894 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/__init__.py
--rw-r--r--   0        0        0     2511 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/api_errors.py
--rw-r--r--   0        0        0      164 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/__init__.py
--rw-r--r--   0        0        0      639 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/cli.py
--rw-r--r--   0        0        0     9660 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/converter.py
--rw-r--r--   0        0        0    12524 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_air_quality.json
--rw-r--r--   0        0        0    11299 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_company_basic_info_errors.json
--rw-r--r--   0        0        0    12755 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_current_weather_required_headers.json
--rw-r--r--   0        0        0    11910 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_teapot_deprecated.json
--rw-r--r--   0        0        0      175 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/conftest.py
--rw-r--r--   0        0        0     1650 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/data/AirQuality/Current.py
--rw-r--r--   0        0        0     1007 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/data/Appliance/CoffeeBrewer.py
--rw-r--r--   0        0        0     1420 2024-02-08 11:58:02.413770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/data/Company/BasicInfo.py
--rw-r--r--   0        0        0     1667 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/data/Weather/Current/Metric.py
--rw-r--r--   0        0        0     2845 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/test_converter.py
--rw-r--r--   0        0        0      489 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/log.py
--rw-r--r--   0        0        0        0 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/__init__.py
--rw-r--r--   0        0        0     1736 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/cli.py
--rw-r--r--   0        0        0     6123 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/core.py
--rw-r--r--   0        0        0     2322 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/errors.py
--rw-r--r--   0        0        0      633 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/tests/conftest.py
--rw-r--r--   0        0        0    10172 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/tests/data/CompanyBasicInfo.json
--rw-r--r--   0        0        0     4234 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/tests/test_definition_versions.py
--rw-r--r--   0        0        0     6119 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/tests/test_definitions.py
--rw-r--r--   0        0        0      812 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/tests/test_utils.py
--rw-r--r--   0        0        0     1391 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/utils.py
--rw-r--r--   0        0        0     1076 2024-02-08 11:58:02.417770 ioxio_data_product_definition_tooling-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 ioxio_data_product_definition_tooling-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1496 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/LICENSE
+-rw-r--r--   0        0        0      894 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/__init__.py
+-rw-r--r--   0        0        0     2803 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/api_errors.py
+-rw-r--r--   0        0        0      164 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/__init__.py
+-rw-r--r--   0        0        0      639 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/cli.py
+-rw-r--r--   0        0        0     9673 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/converter.py
+-rw-r--r--   0        0        0    13212 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_air_quality.json
+-rw-r--r--   0        0        0    11987 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_company_basic_info_errors.json
+-rw-r--r--   0        0        0    13443 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_current_weather_required_headers.json
+-rw-r--r--   0        0        0    12598 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_teapot_deprecated.json
+-rw-r--r--   0        0        0      175 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/conftest.py
+-rw-r--r--   0        0        0     1650 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/data/AirQuality/Current.py
+-rw-r--r--   0        0        0     1007 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/data/Appliance/CoffeeBrewer.py
+-rw-r--r--   0        0        0     1420 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/data/Company/BasicInfo.py
+-rw-r--r--   0        0        0     1667 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/data/Weather/Current/Metric.py
+-rw-r--r--   0        0        0     2845 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/test_converter.py
+-rw-r--r--   0        0        0      489 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/log.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/__init__.py
+-rw-r--r--   0        0        0     1736 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/cli.py
+-rw-r--r--   0        0        0     6123 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/core.py
+-rw-r--r--   0        0        0     2322 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/errors.py
+-rw-r--r--   0        0        0      633 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/tests/conftest.py
+-rw-r--r--   0        0        0    10860 2024-05-29 13:55:21.953796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/tests/data/CompanyBasicInfo.json
+-rw-r--r--   0        0        0     4234 2024-05-29 13:55:21.957796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/tests/test_definition_versions.py
+-rw-r--r--   0        0        0     6119 2024-05-29 13:55:21.957796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/tests/test_definitions.py
+-rw-r--r--   0        0        0      812 2024-05-29 13:55:21.957796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/tests/test_utils.py
+-rw-r--r--   0        0        0     1391 2024-05-29 13:55:21.957796 ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/utils.py
+-rw-r--r--   0        0        0     1056 2024-05-29 13:55:21.957796 ioxio_data_product_definition_tooling-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1833 1970-01-01 00:00:00.000000 ioxio_data_product_definition_tooling-0.6.0/PKG-INFO
```

### Comparing `ioxio_data_product_definition_tooling-0.5.0/LICENSE` & `ioxio_data_product_definition_tooling-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/README.md` & `ioxio_data_product_definition_tooling-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/api_errors.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/api_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Predefined errors that the product gateway or productizers can return.
 
 These errors can not be overridden by the data product definition itself.
 """
+
 from pydantic import BaseModel, Field
 
 
 class BaseApiError(BaseModel):
     __status__: int
 
     @classmethod
@@ -36,14 +37,27 @@
 class NotFound(ApiError):
     __status__ = 404
 
 
 # Note: 422 is added automatically by FastAPI
 
 
+class RateLimitExceeded(BaseApiError):
+    """
+    This response is reserved by Product Gateway.
+    """
+
+    __status__ = 429
+    message: str = Field(
+        "Rate limit exceeded",
+        title="Error message",
+        description="Error description",
+    )
+
+
 class DataSourceNotFound(BaseApiError):
     """
     This response is reserved by Product Gateway.
     """
 
     __status__ = 444
     message: str = Field(
@@ -103,14 +117,15 @@
 
 DATA_PRODUCT_ERRORS = {
     resp.__status__: resp.get_response_spec()
     for resp in [
         Unauthorized,
         Forbidden,
         NotFound,
+        RateLimitExceeded,
         DataSourceNotFound,
         DataSourceError,
         BadGateway,
         ServiceUnavailable,
         GatewayTimeout,
         DoesNotConformToDefinition,
     ]
```

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/cli.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/cli.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/converter.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,26 @@
     BaseModel,
     ConfigDict,
     Field,
     GetJsonSchemaHandler,
     ValidationError,
     field_validator,
 )
+from pydantic.alias_generators import to_camel
 from pydantic.json_schema import JsonSchemaValue
 from pydantic_core import core_schema
 from rich import print
 from semver import Version
-from stringcase import camelcase
 from typing_extensions import Annotated
 
 from definition_tooling.api_errors import DATA_PRODUCT_ERRORS
 
 
 class CamelCaseModel(BaseModel):
-    model_config = ConfigDict(alias_generator=camelcase, populate_by_name=True)
+    model_config = ConfigDict(alias_generator=to_camel, populate_by_name=True)
 
 
 class ErrorModel(BaseModel):
     """
     Wrapper used for error responses, see ErrorResponse decorator for more details.
 
     Encapsulates the actual model and a description for the error.
```

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_air_quality.json` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_air_quality.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953187003968254%*

 * *Differences: {"'components'": "{'schemas': {'RateLimitExceeded': OrderedDict([('description', 'This response is "*

 * *                 "reserved by Product Gateway.'), ('properties', OrderedDict([('message', "*

 * *                 "OrderedDict([('default', 'Rate limit exceeded'), ('description', 'Error "*

 * *                 "description'), ('title', 'Error message'), ('type', 'string')]))])), ('title', "*

 * *                 "'RateLimitExceeded'), ('type', 'object')])}}",*

 * * "'paths'": "{'/AirQuality/Current': {'post': {'responses': {'4 […]*

```diff
@@ -193,14 +193,27 @@
                 "required": [
                     "type",
                     "message"
                 ],
                 "title": "NotFound",
                 "type": "object"
             },
+            "RateLimitExceeded": {
+                "description": "This response is reserved by Product Gateway.",
+                "properties": {
+                    "message": {
+                        "default": "Rate limit exceeded",
+                        "description": "Error description",
+                        "title": "Error message",
+                        "type": "string"
+                    }
+                },
+                "title": "RateLimitExceeded",
+                "type": "object"
+            },
             "ServiceUnavailable": {
                 "description": "This response is reserved by Product Gateway.",
                 "properties": {
                     "message": {
                         "default": "",
                         "description": "Error description",
                         "title": "Error message",
@@ -377,14 +390,24 @@
                                 "schema": {
                                     "$ref": "#/components/schemas/HTTPValidationError"
                                 }
                             }
                         },
                         "description": "Validation Error"
                     },
+                    "429": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/RateLimitExceeded"
+                                }
+                            }
+                        },
+                        "description": "Too Many Requests"
+                    },
                     "444": {
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "$ref": "#/components/schemas/DataSourceNotFound"
                                 }
                             }
```

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_company_basic_info_errors.json` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_company_basic_info_errors.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949752938034189%*

 * *Differences: {"'components'": "{'schemas': {'RateLimitExceeded': OrderedDict([('description', 'This response is "*

 * *                 "reserved by Product Gateway.'), ('properties', OrderedDict([('message', "*

 * *                 "OrderedDict([('default', 'Rate limit exceeded'), ('description', 'Error "*

 * *                 "description'), ('title', 'Error message'), ('type', 'string')]))])), ('title', "*

 * *                 "'RateLimitExceeded'), ('type', 'object')])}}",*

 * * "'paths'": "{'/Company/BasicInfo': {'post': {'responses': {'42 […]*

```diff
@@ -166,14 +166,27 @@
                 "required": [
                     "type",
                     "message"
                 ],
                 "title": "NotFound",
                 "type": "object"
             },
+            "RateLimitExceeded": {
+                "description": "This response is reserved by Product Gateway.",
+                "properties": {
+                    "message": {
+                        "default": "Rate limit exceeded",
+                        "description": "Error description",
+                        "title": "Error message",
+                        "type": "string"
+                    }
+                },
+                "title": "RateLimitExceeded",
+                "type": "object"
+            },
             "ServiceUnavailable": {
                 "description": "This response is reserved by Product Gateway.",
                 "properties": {
                     "message": {
                         "default": "",
                         "description": "Error description",
                         "title": "Error message",
@@ -331,14 +344,24 @@
                                 "schema": {
                                     "$ref": "#/components/schemas/UnavailableForLegalReasonsResponse"
                                 }
                             }
                         },
                         "description": "Unavailable for some legal reasons"
                     },
+                    "429": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/RateLimitExceeded"
+                                }
+                            }
+                        },
+                        "description": "Too Many Requests"
+                    },
                     "444": {
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "$ref": "#/components/schemas/DataSourceNotFound"
                                 }
                             }
```

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_current_weather_required_headers.json` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_current_weather_required_headers.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953187003968254%*

 * *Differences: {"'components'": "{'schemas': {'RateLimitExceeded': OrderedDict([('description', 'This response is "*

 * *                 "reserved by Product Gateway.'), ('properties', OrderedDict([('message', "*

 * *                 "OrderedDict([('default', 'Rate limit exceeded'), ('description', 'Error "*

 * *                 "description'), ('title', 'Error message'), ('type', 'string')]))])), ('title', "*

 * *                 "'RateLimitExceeded'), ('type', 'object')])}}",*

 * * "'paths'": "{'/Weather/Current/Metric': {'post': {'responses': […]*

```diff
@@ -210,14 +210,27 @@
                 "required": [
                     "type",
                     "message"
                 ],
                 "title": "NotFound",
                 "type": "object"
             },
+            "RateLimitExceeded": {
+                "description": "This response is reserved by Product Gateway.",
+                "properties": {
+                    "message": {
+                        "default": "Rate limit exceeded",
+                        "description": "Error description",
+                        "title": "Error message",
+                        "type": "string"
+                    }
+                },
+                "title": "RateLimitExceeded",
+                "type": "object"
+            },
             "ServiceUnavailable": {
                 "description": "This response is reserved by Product Gateway.",
                 "properties": {
                     "message": {
                         "default": "",
                         "description": "Error description",
                         "title": "Error message",
@@ -392,14 +405,24 @@
                                 "schema": {
                                     "$ref": "#/components/schemas/HTTPValidationError"
                                 }
                             }
                         },
                         "description": "Validation Error"
                     },
+                    "429": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/RateLimitExceeded"
+                                }
+                            }
+                        },
+                        "description": "Too Many Requests"
+                    },
                     "444": {
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "$ref": "#/components/schemas/DataSourceNotFound"
                                 }
                             }
```

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_teapot_deprecated.json` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/__snapshots__/test_converter/test_teapot_deprecated.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9956616300366301%*

 * *Differences: {"'components'": "{'schemas': {'RateLimitExceeded': OrderedDict([('description', 'This response is "*

 * *                 "reserved by Product Gateway.'), ('properties', OrderedDict([('message', "*

 * *                 "OrderedDict([('default', 'Rate limit exceeded'), ('description', 'Error "*

 * *                 "description'), ('title', 'Error message'), ('type', 'string')]))])), ('title', "*

 * *                 "'RateLimitExceeded'), ('type', 'object')])}}",*

 * * "'paths'": "{'/Appliance/CoffeeBrewer': {'post': {'responses': […]*

```diff
@@ -155,14 +155,27 @@
                 "required": [
                     "type",
                     "message"
                 ],
                 "title": "NotFound",
                 "type": "object"
             },
+            "RateLimitExceeded": {
+                "description": "This response is reserved by Product Gateway.",
+                "properties": {
+                    "message": {
+                        "default": "Rate limit exceeded",
+                        "description": "Error description",
+                        "title": "Error message",
+                        "type": "string"
+                    }
+                },
+                "title": "RateLimitExceeded",
+                "type": "object"
+            },
             "ServiceUnavailable": {
                 "description": "This response is reserved by Product Gateway.",
                 "properties": {
                     "message": {
                         "default": "",
                         "description": "Error description",
                         "title": "Error message",
@@ -374,14 +387,24 @@
                                 "schema": {
                                     "$ref": "#/components/schemas/HTTPValidationError"
                                 }
                             }
                         },
                         "description": "Validation Error"
                     },
+                    "429": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/RateLimitExceeded"
+                                }
+                            }
+                        },
+                        "description": "Too Many Requests"
+                    },
                     "444": {
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "$ref": "#/components/schemas/DataSourceNotFound"
                                 }
                             }
```

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/data/AirQuality/Current.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/data/AirQuality/Current.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/data/Appliance/CoffeeBrewer.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/data/Appliance/CoffeeBrewer.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/data/Company/BasicInfo.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/data/Company/BasicInfo.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/data/Weather/Current/Metric.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/data/Weather/Current/Metric.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/converter/tests/test_converter.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/converter/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/cli.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/cli.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/core.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/core.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/errors.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/errors.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/tests/conftest.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/tests/data/CompanyBasicInfo.json` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/tests/data/CompanyBasicInfo.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949752938034189%*

 * *Differences: {"'components'": "{'schemas': {'RateLimitExceeded': OrderedDict([('description', 'This response is "*

 * *                 "reserved by Product Gateway.'), ('properties', OrderedDict([('message', "*

 * *                 "OrderedDict([('default', 'Rate limit exceeded'), ('description', 'Error "*

 * *                 "description'), ('title', 'Error message'), ('type', 'string')]))])), ('title', "*

 * *                 "'RateLimitExceeded'), ('type', 'object')])}}",*

 * * "'paths'": "{'/Company/BasicInfo': {'post': {'responses': {'42 […]*

```diff
@@ -155,14 +155,27 @@
                 "required": [
                     "type",
                     "message"
                 ],
                 "title": "NotFound",
                 "type": "object"
             },
+            "RateLimitExceeded": {
+                "description": "This response is reserved by Product Gateway.",
+                "properties": {
+                    "message": {
+                        "default": "Rate limit exceeded",
+                        "description": "Error description",
+                        "title": "Error message",
+                        "type": "string"
+                    }
+                },
+                "title": "RateLimitExceeded",
+                "type": "object"
+            },
             "ServiceUnavailable": {
                 "properties": {
                     "message": {
                         "description": "Error description",
                         "title": "Error message",
                         "type": "string"
                     }
@@ -309,14 +322,24 @@
                                 "schema": {
                                     "$ref": "#/components/schemas/UnavailableForLegalReasonsResponse"
                                 }
                             }
                         },
                         "description": "Unavailable for some legal reasons"
                     },
+                    "429": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/RateLimitExceeded"
+                                }
+                            }
+                        },
+                        "description": "Too Many Requests"
+                    },
                     "444": {
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "$ref": "#/components/schemas/DataSourceNotFound"
                                 }
                             }
```

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/tests/test_definition_versions.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/tests/test_definition_versions.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/tests/test_definitions.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/tests/test_utils.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/definition_tooling/validator/utils.py` & `ioxio_data_product_definition_tooling-0.6.0/definition_tooling/validator/utils.py`

 * *Files identical despite different names*

### Comparing `ioxio_data_product_definition_tooling-0.5.0/pyproject.toml` & `ioxio_data_product_definition_tooling-0.6.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ioxio-data-product-definition-tooling"
-version = "0.5.0"
+version = "0.6.0"
 description = "IOXIO Data Product Definition Tooling"
 authors = ["IOXIO Ltd"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/ioxio-dataspace/ioxio-data-product-definition-tooling"
 packages = [
     {include="definition_tooling", from="."},
@@ -12,30 +12,29 @@
 
 [tool.poetry.scripts]
 convert-definitions = "definition_tooling.converter.cli:cli"
 validate-definitions = "definition_tooling.validator.cli:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.9.0,<4"
-typer = {extras = ["all"], version = "^0.9.0"}
-deepdiff = "^6.7.1"
-fastapi = "^0.109.2"
-stringcase = "^1.2.0"
-pydantic = {version = "^2.6.1", extras = ["email"]}
+typer = {version = "^0.12.3", extras = ["all"]}
+deepdiff = "^7.0.1"
+fastapi = "^0.111.0"
+pydantic = {version = "^2.7.1", extras = ["email"]}
 semver = "^3.0.2"
 
 [tool.poetry.group.dev.dependencies]
-isort = "^5.12.0"
-pytest = "^7.3.1"
-pytest-asyncio = "^0.21.0"
-flake8 = "^6.0.0"
-mypy = "^1.3.0"
-black = "^23.3.0"
-syrupy = "^4.0.2"
-invoke = "^2.1.2"
+isort = "^5.13.2"
+pytest = "^8.2.1"
+pytest-asyncio = "^0.23.7"
+flake8 = "^7.0.0"
+mypy = "^1.10.0"
+black = "^24.4.2"
+syrupy = "^4.6.1"
+invoke = "^2.2.0"
 
 [tool.skjold]
 report_only = false
 sources = ["pyup", "gemnasium"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `ioxio_data_product_definition_tooling-0.5.0/PKG-INFO` & `ioxio_data_product_definition_tooling-0.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: ioxio-data-product-definition-tooling
-Version: 0.5.0
+Version: 0.6.0
 Summary: IOXIO Data Product Definition Tooling
 Home-page: https://github.com/ioxio-dataspace/ioxio-data-product-definition-tooling
 License: BSD-3-Clause
 Author: IOXIO Ltd
 Requires-Python: >=3.9.0,<4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: deepdiff (>=6.7.1,<7.0.0)
-Requires-Dist: fastapi (>=0.109.2,<0.110.0)
-Requires-Dist: pydantic[email] (>=2.6.1,<3.0.0)
+Requires-Dist: deepdiff (>=7.0.1,<8.0.0)
+Requires-Dist: fastapi (>=0.111.0,<0.112.0)
+Requires-Dist: pydantic[email] (>=2.7.1,<3.0.0)
 Requires-Dist: semver (>=3.0.2,<4.0.0)
-Requires-Dist: stringcase (>=1.2.0,<2.0.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
 Project-URL: Repository, https://github.com/ioxio-dataspace/ioxio-data-product-definition-tooling
 Description-Content-Type: text/markdown
 
 # IOXIO® Data Product Definitions tooling
 
 Tools for managing Data Product definitions
```

