# Comparing `tmp/airbyte_source_sap_fieldglass-0.1.1.tar.gz` & `tmp/airbyte_source_sap_fieldglass-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_sap_fieldglass-0.1.1.tar", max compression
+gzip compressed data, was "airbyte_source_sap_fieldglass-0.1.2.tar", max compression
```

## Comparing `airbyte_source_sap_fieldglass-0.1.1.tar` & `airbyte_source_sap_fieldglass-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,7 @@
--rw-r--r--   0        0        0     4640 2024-05-21 05:04:27.000000 airbyte_source_sap_fieldglass-0.1.1/README.md
--rw-r--r--   0        0        0      790 2024-05-21 05:41:03.082890 airbyte_source_sap_fieldglass-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      138 2024-05-21 05:04:27.000000 airbyte_source_sap_fieldglass-0.1.1/source_sap_fieldglass/__init__.py
--rw-r--r--   0        0        0      837 2024-05-21 05:04:27.000000 airbyte_source_sap_fieldglass-0.1.1/source_sap_fieldglass/manifest.yaml
--rw-r--r--   0        0        0      252 2024-05-21 05:04:27.000000 airbyte_source_sap_fieldglass-0.1.1/source_sap_fieldglass/run.py
--rw-r--r--   0        0        0     8479 2024-05-21 05:04:27.000000 airbyte_source_sap_fieldglass-0.1.1/source_sap_fieldglass/schemas/data.json
--rw-r--r--   0        0        0      482 2024-05-21 05:04:27.000000 airbyte_source_sap_fieldglass-0.1.1/source_sap_fieldglass/source.py
--rw-r--r--   0        0        0      354 2024-05-21 05:04:27.000000 airbyte_source_sap_fieldglass-0.1.1/source_sap_fieldglass/spec.yaml
--rw-r--r--   0        0        0     5367 1970-01-01 00:00:00.000000 airbyte_source_sap_fieldglass-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4640 2024-05-28 21:11:20.000000 airbyte_source_sap_fieldglass-0.1.2/README.md
+-rw-r--r--   0        0        0      790 2024-05-28 23:57:30.235735 airbyte_source_sap_fieldglass-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      138 2024-05-28 21:11:20.000000 airbyte_source_sap_fieldglass-0.1.2/source_sap_fieldglass/__init__.py
+-rw-r--r--   0        0        0     9466 2024-05-28 21:11:20.000000 airbyte_source_sap_fieldglass-0.1.2/source_sap_fieldglass/manifest.yaml
+-rw-r--r--   0        0        0      239 2024-05-28 21:11:20.000000 airbyte_source_sap_fieldglass-0.1.2/source_sap_fieldglass/run.py
+-rw-r--r--   0        0        0      482 2024-05-28 21:11:20.000000 airbyte_source_sap_fieldglass-0.1.2/source_sap_fieldglass/source.py
+-rw-r--r--   0        0        0     5367 1970-01-01 00:00:00.000000 airbyte_source_sap_fieldglass-0.1.2/PKG-INFO
```

### Comparing `airbyte_source_sap_fieldglass-0.1.1/README.md` & `airbyte_source_sap_fieldglass-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_sap_fieldglass-0.1.1/pyproject.toml` & `airbyte_source_sap_fieldglass-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.1.1"
+version = "0.1.2"
 name = "airbyte-source-sap-fieldglass"
 description = "Source implementation for Sap Fieldglass."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_sap_fieldglass-0.1.1/PKG-INFO` & `airbyte_source_sap_fieldglass-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-sap-fieldglass
-Version: 0.1.1
+Version: 0.1.2
 Summary: Source implementation for Sap Fieldglass.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

