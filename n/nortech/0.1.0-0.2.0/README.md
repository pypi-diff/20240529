# Comparing `tmp/nortech-0.1.0.tar.gz` & `tmp/nortech-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nortech-0.1.0.tar", max compression
+gzip compressed data, was "nortech-0.2.0.tar", max compression
```

## Comparing `nortech-0.1.0.tar` & `nortech-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11357 2023-11-28 16:36:24.114062 nortech-0.1.0/LICENSE
--rw-r--r--   0        0        0     6228 2023-12-04 14:04:21.033886 nortech-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-12-03 13:52:48.203137 nortech-0.1.0/nortech/__init__.py
--rw-r--r--   0        0        0      264 2023-12-04 16:14:37.723473 nortech-0.1.0/nortech/datatools/__init__.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:51.232877 nortech-0.1.0/nortech/datatools/handlers/__init__.py
--rw-r--r--   0        0        0     2828 2023-12-04 17:38:39.495516 nortech-0.1.0/nortech/datatools/handlers/pandas.py
--rw-r--r--   0        0        0     5969 2023-12-04 17:38:36.825041 nortech-0.1.0/nortech/datatools/handlers/polars.py
--rw-r--r--   0        0        0     5200 2023-12-04 16:16:06.875409 nortech-0.1.0/nortech/datatools/repositories/S3.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:43.016646 nortech-0.1.0/nortech/datatools/repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:26.578689 nortech-0.1.0/nortech/datatools/services/__init__.py
--rw-r--r--   0        0        0      609 2023-12-04 16:16:14.399442 nortech-0.1.0/nortech/datatools/services/config.py
--rw-r--r--   0        0        0        0 2023-12-03 14:10:29.817430 nortech-0.1.0/nortech/datatools/values/__init__.py
--rw-r--r--   0        0        0      347 2023-12-03 19:51:26.287501 nortech-0.1.0/nortech/datatools/values/errors.py
--rw-r--r--   0        0        0     2159 2023-12-03 19:51:44.164402 nortech-0.1.0/nortech/datatools/values/signals.py
--rw-r--r--   0        0        0      510 2024-05-29 10:21:18.962630 nortech-0.1.0/nortech/derivers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.205309 nortech-0.1.0/nortech/derivers/gateways/__init__.py
--rw-r--r--   0        0        0     2735 2024-05-29 11:28:33.338226 nortech-0.1.0/nortech/derivers/gateways/customer_api.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.206598 nortech-0.1.0/nortech/derivers/handlers/__init__.py
--rw-r--r--   0        0        0     2467 2024-05-29 11:17:45.728370 nortech-0.1.0/nortech/derivers/handlers/deriver.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.203764 nortech-0.1.0/nortech/derivers/repositories/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.201516 nortech-0.1.0/nortech/derivers/services/__init__.py
--rw-r--r--   0        0        0      131 2024-05-29 09:45:01.201714 nortech-0.1.0/nortech/derivers/services/logger.py
--rw-r--r--   0        0        0     5431 2024-05-29 10:26:08.670198 nortech-0.1.0/nortech/derivers/services/operators.py
--rw-r--r--   0        0        0      276 2024-05-29 10:47:12.127163 nortech-0.1.0/nortech/derivers/services/physical_units.py
--rw-r--r--   0        0        0     4925 2024-05-29 09:46:25.353487 nortech-0.1.0/nortech/derivers/services/schema.py
--rw-r--r--   0        0        0     2288 2024-05-29 09:46:25.353623 nortech-0.1.0/nortech/derivers/services/visualize.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.197564 nortech-0.1.0/nortech/derivers/values/__init__.py
--rw-r--r--   0        0        0     1948 2024-05-29 11:12:50.690657 nortech-0.1.0/nortech/derivers/values/instance.py
--rw-r--r--   0        0        0     3918 2024-05-29 09:46:25.353139 nortech-0.1.0/nortech/derivers/values/physical_units.py
--rw-r--r--   0        0        0      351 2024-05-29 09:45:01.197672 nortech-0.1.0/nortech/derivers/values/physical_units_schema.py
--rw-r--r--   0        0        0     6007 2024-05-29 09:46:25.349173 nortech-0.1.0/nortech/derivers/values/schema.py
--rw-r--r--   0        0        0      764 2024-05-29 11:26:36.881224 nortech-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7195 1970-01-01 00:00:00.000000 nortech-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-28 16:36:24.114062 nortech-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6228 2023-12-04 14:04:21.033886 nortech-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-12-03 13:52:48.203137 nortech-0.2.0/nortech/__init__.py
+-rw-r--r--   0        0        0      264 2023-12-04 16:14:37.723473 nortech-0.2.0/nortech/datatools/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:51.232877 nortech-0.2.0/nortech/datatools/handlers/__init__.py
+-rw-r--r--   0        0        0     2828 2023-12-04 17:38:39.495516 nortech-0.2.0/nortech/datatools/handlers/pandas.py
+-rw-r--r--   0        0        0     5969 2023-12-04 17:38:36.825041 nortech-0.2.0/nortech/datatools/handlers/polars.py
+-rw-r--r--   0        0        0     5200 2023-12-04 16:16:06.875409 nortech-0.2.0/nortech/datatools/repositories/S3.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:43.016646 nortech-0.2.0/nortech/datatools/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:26.578689 nortech-0.2.0/nortech/datatools/services/__init__.py
+-rw-r--r--   0        0        0      609 2023-12-04 16:16:14.399442 nortech-0.2.0/nortech/datatools/services/config.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:10:29.817430 nortech-0.2.0/nortech/datatools/values/__init__.py
+-rw-r--r--   0        0        0      347 2023-12-03 19:51:26.287501 nortech-0.2.0/nortech/datatools/values/errors.py
+-rw-r--r--   0        0        0     2159 2023-12-03 19:51:44.164402 nortech-0.2.0/nortech/datatools/values/signals.py
+-rw-r--r--   0        0        0      510 2024-05-29 12:39:38.725679 nortech-0.2.0/nortech/derivers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.205309 nortech-0.2.0/nortech/derivers/gateways/__init__.py
+-rw-r--r--   0        0        0     2734 2024-05-29 12:34:42.265804 nortech-0.2.0/nortech/derivers/gateways/customer_api.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.206598 nortech-0.2.0/nortech/derivers/handlers/__init__.py
+-rw-r--r--   0        0        0     5637 2024-05-29 13:44:02.676884 nortech-0.2.0/nortech/derivers/handlers/deriver.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.203764 nortech-0.2.0/nortech/derivers/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.201516 nortech-0.2.0/nortech/derivers/services/__init__.py
+-rw-r--r--   0        0        0      131 2024-05-29 09:45:01.201714 nortech-0.2.0/nortech/derivers/services/logger.py
+-rw-r--r--   0        0        0     5431 2024-05-29 10:26:08.670198 nortech-0.2.0/nortech/derivers/services/operators.py
+-rw-r--r--   0        0        0      276 2024-05-29 10:47:12.127163 nortech-0.2.0/nortech/derivers/services/physical_units.py
+-rw-r--r--   0        0        0     3564 2024-05-29 12:58:49.727767 nortech-0.2.0/nortech/derivers/services/schema.py
+-rw-r--r--   0        0        0     2288 2024-05-29 09:46:25.353623 nortech-0.2.0/nortech/derivers/services/visualize.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.197564 nortech-0.2.0/nortech/derivers/values/__init__.py
+-rw-r--r--   0        0        0     1948 2024-05-29 11:12:50.690657 nortech-0.2.0/nortech/derivers/values/instance.py
+-rw-r--r--   0        0        0     3918 2024-05-29 09:46:25.353139 nortech-0.2.0/nortech/derivers/values/physical_units.py
+-rw-r--r--   0        0        0      351 2024-05-29 09:45:01.197672 nortech-0.2.0/nortech/derivers/values/physical_units_schema.py
+-rw-r--r--   0        0        0     6007 2024-05-29 09:46:25.349173 nortech-0.2.0/nortech/derivers/values/schema.py
+-rw-r--r--   0        0        0      764 2024-05-29 13:45:00.987415 nortech-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7195 1970-01-01 00:00:00.000000 nortech-0.2.0/PKG-INFO
```

### Comparing `nortech-0.1.0/LICENSE` & `nortech-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nortech-0.1.0/README.md` & `nortech-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nortech-0.1.0/nortech/datatools/handlers/pandas.py` & `nortech-0.2.0/nortech/datatools/handlers/pandas.py`

 * *Files identical despite different names*

### Comparing `nortech-0.1.0/nortech/datatools/handlers/polars.py` & `nortech-0.2.0/nortech/datatools/handlers/polars.py`

 * *Files identical despite different names*

### Comparing `nortech-0.1.0/nortech/datatools/repositories/S3.py` & `nortech-0.2.0/nortech/datatools/repositories/S3.py`

 * *Files identical despite different names*

### Comparing `nortech-0.1.0/nortech/datatools/services/config.py` & `nortech-0.2.0/nortech/datatools/services/config.py`

 * *Files identical despite different names*

### Comparing `nortech-0.1.0/nortech/datatools/values/signals.py` & `nortech-0.2.0/nortech/datatools/values/signals.py`

 * *Files identical despite different names*

### Comparing `nortech-0.1.0/nortech/derivers/gateways/customer_api.py` & `nortech-0.2.0/nortech/derivers/gateways/customer_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     DeriverInputType,
     DeriverOutputType,
 )
 from nortech.derivers.values.schema import ConfigurationType, DeriverSchemaDAG
 
 
 class CustomerAPI(BaseSettings):
-    URL: str = Field(default="https://api.apps.nor.tech/")
+    URL: str = Field(default="https://api.apps.nor.tech")
     TOKEN: str
 
     model_config = SettingsConfigDict(env_prefix="CUSTOMER_API_")
 
 
 class CreateDeriver(
     BaseModel, Generic[DeriverInputType, DeriverOutputType, ConfigurationType]
```

### Comparing `nortech-0.1.0/nortech/derivers/services/operators.py` & `nortech-0.2.0/nortech/derivers/services/operators.py`

 * *Files identical despite different names*

### Comparing `nortech-0.1.0/nortech/derivers/services/visualize.py` & `nortech-0.2.0/nortech/derivers/services/visualize.py`

 * *Files identical despite different names*

### Comparing `nortech-0.1.0/nortech/derivers/values/instance.py` & `nortech-0.2.0/nortech/derivers/values/instance.py`

 * *Files identical despite different names*

### Comparing `nortech-0.1.0/nortech/derivers/values/physical_units.py` & `nortech-0.2.0/nortech/derivers/values/physical_units.py`

 * *Files identical despite different names*

### Comparing `nortech-0.1.0/nortech/derivers/values/schema.py` & `nortech-0.2.0/nortech/derivers/values/schema.py`

 * *Files identical despite different names*

### Comparing `nortech-0.1.0/pyproject.toml` & `nortech-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nortech"
-version = "0.1.0"
+version = "0.2.0"
 description = "The official Python library for Nortech AI"
 authors = ["Nortech AI <info@nortech.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://nortech.ai/"
 repository = "https://github.com/Nortech-ai/nortech-python"
```

### Comparing `nortech-0.1.0/PKG-INFO` & `nortech-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nortech
-Version: 0.1.0
+Version: 0.2.0
 Summary: The official Python library for Nortech AI
 Home-page: https://nortech.ai/
 License: Apache-2.0
 Author: Nortech AI
 Author-email: info@nortech.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

