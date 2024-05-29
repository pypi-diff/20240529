# Comparing `tmp/omicidx-1.8.0.tar.gz` & `tmp/omicidx-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omicidx-1.8.0.tar", max compression
+gzip compressed data, was "omicidx-1.8.1.tar", max compression
```

## Comparing `omicidx-1.8.0.tar` & `omicidx-1.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2021-10-07 20:33:57.811472 omicidx-1.8.0/README.md
--rw-r--r--   0        0        0     9854 2022-06-12 18:49:26.440659 omicidx-1.8.0/omicidx/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0    47492 2022-06-12 20:15:47.493331 omicidx-1.8.0/omicidx/Untitled.ipynb
--rw-r--r--   0        0        0       19 2021-08-23 17:51:36.154366 omicidx-1.8.0/omicidx/__init__.py
--rw-r--r--   0        0        0     7776 2023-08-29 19:38:15.106229 omicidx-1.8.0/omicidx/biosample.py
--rw-r--r--   0        0        0        0 2021-08-23 17:51:36.154811 omicidx-1.8.0/omicidx/geo/__init__.py
--rw-r--r--   0        0        0    19681 2023-08-29 19:40:11.125549 omicidx-1.8.0/omicidx/geo/parser.py
--rw-r--r--   0        0        0     3164 2023-08-29 19:40:10.856437 omicidx-1.8.0/omicidx/geo/pydantic_models.py
--rw-r--r--   0        0        0     2080 2022-05-21 02:59:44.471856 omicidx-1.8.0/omicidx/geo/webutils.py
--rw-r--r--   0        0        0        0 2021-08-23 17:51:36.155471 omicidx-1.8.0/omicidx/ontologies/__init__.py
--rw-r--r--   0        0        0     1399 2023-08-29 19:40:10.756086 omicidx-1.8.0/omicidx/ontologies/utils.py
--rw-r--r--   0        0        0     4668 2023-08-29 19:40:10.893033 omicidx-1.8.0/omicidx/schema_tools.py
--rw-r--r--   0        0        0        2 2021-08-23 17:51:36.156881 omicidx-1.8.0/omicidx/scripts/__init__.py
--rw-r--r--   0        0        0     5725 2022-08-15 18:06:45.378444 omicidx-1.8.0/omicidx/scripts/cli.py
--rw-r--r--   0        0        0     1718 2023-08-29 19:38:15.106393 omicidx-1.8.0/omicidx/scripts/geo.py
--rwxr-xr-x   0        0        0     2001 2023-08-29 19:40:10.815847 omicidx-1.8.0/omicidx/scripts/sra_entity_to_json.py
--rw-r--r--   0        0        0        0 2021-08-23 17:51:36.157285 omicidx-1.8.0/omicidx/sra/__init__.py
--rw-r--r--   0        0        0     1669 2023-08-29 19:40:10.803307 omicidx-1.8.0/omicidx/sra/ebiutils.py
--rw-r--r--   0        0        0    35506 2022-12-12 14:55:40.313193 omicidx-1.8.0/omicidx/sra/parser.py
--rw-r--r--   0        0        0     4377 2023-08-29 19:40:10.921071 omicidx-1.8.0/omicidx/sra/pydantic_models.py
--rw-r--r--   0        0        0     2074 2023-08-29 19:40:10.834785 omicidx-1.8.0/omicidx/utils.py
--rw-r--r--   0        0        0     1602 2023-11-10 11:56:34.625264 omicidx-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 omicidx-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2021-10-07 20:33:57.811472 omicidx-1.8.1/README.md
+-rw-r--r--   0        0        0     9854 2022-06-12 18:49:26.440659 omicidx-1.8.1/omicidx/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0    47492 2022-06-12 20:15:47.493331 omicidx-1.8.1/omicidx/Untitled.ipynb
+-rw-r--r--   0        0        0       19 2021-08-23 17:51:36.154366 omicidx-1.8.1/omicidx/__init__.py
+-rw-r--r--   0        0        0     7776 2023-08-29 19:38:15.106229 omicidx-1.8.1/omicidx/biosample.py
+-rw-r--r--   0        0        0        0 2021-08-23 17:51:36.154811 omicidx-1.8.1/omicidx/geo/__init__.py
+-rw-r--r--   0        0        0    19681 2023-08-29 19:40:11.125549 omicidx-1.8.1/omicidx/geo/parser.py
+-rw-r--r--   0        0        0     3648 2023-11-10 12:30:47.246952 omicidx-1.8.1/omicidx/geo/pydantic_models.py
+-rw-r--r--   0        0        0     2080 2022-05-21 02:59:44.471856 omicidx-1.8.1/omicidx/geo/webutils.py
+-rw-r--r--   0        0        0        0 2021-08-23 17:51:36.155471 omicidx-1.8.1/omicidx/ontologies/__init__.py
+-rw-r--r--   0        0        0     1399 2023-08-29 19:40:10.756086 omicidx-1.8.1/omicidx/ontologies/utils.py
+-rw-r--r--   0        0        0     4668 2023-08-29 19:40:10.893033 omicidx-1.8.1/omicidx/schema_tools.py
+-rw-r--r--   0        0        0        2 2021-08-23 17:51:36.156881 omicidx-1.8.1/omicidx/scripts/__init__.py
+-rw-r--r--   0        0        0     5725 2022-08-15 18:06:45.378444 omicidx-1.8.1/omicidx/scripts/cli.py
+-rw-r--r--   0        0        0     1718 2023-08-29 19:38:15.106393 omicidx-1.8.1/omicidx/scripts/geo.py
+-rwxr-xr-x   0        0        0     2001 2023-08-29 19:40:10.815847 omicidx-1.8.1/omicidx/scripts/sra_entity_to_json.py
+-rw-r--r--   0        0        0        0 2021-08-23 17:51:36.157285 omicidx-1.8.1/omicidx/sra/__init__.py
+-rw-r--r--   0        0        0     1669 2023-08-29 19:40:10.803307 omicidx-1.8.1/omicidx/sra/ebiutils.py
+-rw-r--r--   0        0        0    35506 2022-12-12 14:55:40.313193 omicidx-1.8.1/omicidx/sra/parser.py
+-rw-r--r--   0        0        0     4377 2023-08-29 19:40:10.921071 omicidx-1.8.1/omicidx/sra/pydantic_models.py
+-rw-r--r--   0        0        0     2074 2023-08-29 19:40:10.834785 omicidx-1.8.1/omicidx/utils.py
+-rw-r--r--   0        0        0     1602 2023-11-10 12:34:36.611250 omicidx-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 omicidx-1.8.1/PKG-INFO
```

### Comparing `omicidx-1.8.0/omicidx/.ipynb_checkpoints/Untitled-checkpoint.ipynb` & `omicidx-1.8.1/omicidx/.ipynb_checkpoints/Untitled-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/omicidx/Untitled.ipynb` & `omicidx-1.8.1/omicidx/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/omicidx/biosample.py` & `omicidx-1.8.1/omicidx/biosample.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/omicidx/geo/parser.py` & `omicidx-1.8.1/omicidx/geo/parser.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/omicidx/geo/webutils.py` & `omicidx-1.8.1/omicidx/geo/webutils.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/omicidx/ontologies/utils.py` & `omicidx-1.8.1/omicidx/ontologies/utils.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/omicidx/schema_tools.py` & `omicidx-1.8.1/omicidx/schema_tools.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/omicidx/scripts/cli.py` & `omicidx-1.8.1/omicidx/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/omicidx/scripts/geo.py` & `omicidx-1.8.1/omicidx/scripts/geo.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/omicidx/scripts/sra_entity_to_json.py` & `omicidx-1.8.1/omicidx/scripts/sra_entity_to_json.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/omicidx/sra/ebiutils.py` & `omicidx-1.8.1/omicidx/sra/ebiutils.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/omicidx/sra/parser.py` & `omicidx-1.8.1/omicidx/sra/parser.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/omicidx/sra/pydantic_models.py` & `omicidx-1.8.1/omicidx/sra/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/omicidx/utils.py` & `omicidx-1.8.1/omicidx/utils.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.8.0/pyproject.toml` & `omicidx-1.8.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.dephell.main]
 from = {format = "poetry", path = "pyproject.toml"}
 to = {format = "setuppy", path = "setup.py"}
 
 [tool.poetry]
 name = "omicidx"
-version = "1.8.0"
+version = "1.8.1"
 readme = "README.md"
 description = """The OmicIDX project collects, reprocesses, and then republishes metadata from multiple public genomics repositories. Included are the NCBI SRA, Biosample, and GEO databases. Publication is via the cloud data warehouse platform Bigquery, a set of performant search and retrieval APIs, and a set of json-format files for easy incorporation into other projects."""
 authors = ["Sean Davis <seandavi@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/omicidx/omicidx-parsers"
 keywords = ["genomics", "bioinformatics", "open data", "API"]
```

### Comparing `omicidx-1.8.0/PKG-INFO` & `omicidx-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omicidx
-Version: 1.8.0
+Version: 1.8.1
 Summary: The OmicIDX project collects, reprocesses, and then republishes metadata from multiple public genomics repositories. Included are the NCBI SRA, Biosample, and GEO databases. Publication is via the cloud data warehouse platform Bigquery, a set of performant search and retrieval APIs, and a set of json-format files for easy incorporation into other projects.
 Home-page: https://github.com/omicidx/omicidx-parsers
 License: MIT
 Keywords: genomics,bioinformatics,open data,API
 Author: Sean Davis
 Author-email: seandavi@gmail.com
 Requires-Python: >=3.8
```

