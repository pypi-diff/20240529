# Comparing `tmp/basketball_reference_webscrapper-0.1.6.tar.gz` & `tmp/basketball_reference_webscrapper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basketball_reference_webscrapper-0.1.6.tar", max compression
+gzip compressed data, was "basketball_reference_webscrapper-0.1.7.tar", max compression
```

## Comparing `basketball_reference_webscrapper-0.1.6.tar` & `basketball_reference_webscrapper-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      120 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/constants/__init__.py
--rw-r--r--   0        0        0     1223 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/constants/team_city_refdata.csv
--rw-r--r--   0        0        0        0 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/data_models/__init_.py
--rw-r--r--   0        0        0      213 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/data_models/feature_model.py
--rw-r--r--   0        0        0     1769 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/params.yaml
--rw-r--r--   0        0        0        0 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/utils/__init__.py
--rw-r--r--   0        0        0     1075 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/utils/logs.py
--rw-r--r--   0        0        0     7683 2024-05-28 11:57:13.476094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/webscrapping_basketball_reference.py
--rw-r--r--   0        0        0      958 2024-05-28 11:57:13.476094 basketball_reference_webscrapper-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 basketball_reference_webscrapper-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      120 2024-05-28 12:00:27.404805 basketball_reference_webscrapper-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 12:00:27.404805 basketball_reference_webscrapper-0.1.7/basketball_reference_webscrapper/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:00:27.404805 basketball_reference_webscrapper-0.1.7/basketball_reference_webscrapper/constants/__init__.py
+-rw-r--r--   0        0        0     1223 2024-05-28 12:00:27.404805 basketball_reference_webscrapper-0.1.7/basketball_reference_webscrapper/constants/team_city_refdata.csv
+-rw-r--r--   0        0        0        0 2024-05-28 12:00:27.404805 basketball_reference_webscrapper-0.1.7/basketball_reference_webscrapper/data_models/__init_.py
+-rw-r--r--   0        0        0      213 2024-05-28 12:00:27.404805 basketball_reference_webscrapper-0.1.7/basketball_reference_webscrapper/data_models/feature_model.py
+-rw-r--r--   0        0        0     1769 2024-05-28 12:00:27.404805 basketball_reference_webscrapper-0.1.7/basketball_reference_webscrapper/params.yaml
+-rw-r--r--   0        0        0        0 2024-05-28 12:00:27.404805 basketball_reference_webscrapper-0.1.7/basketball_reference_webscrapper/utils/__init__.py
+-rw-r--r--   0        0        0     1075 2024-05-28 12:00:27.404805 basketball_reference_webscrapper-0.1.7/basketball_reference_webscrapper/utils/logs.py
+-rw-r--r--   0        0        0     7683 2024-05-28 12:00:27.404805 basketball_reference_webscrapper-0.1.7/basketball_reference_webscrapper/webscrapping_basketball_reference.py
+-rw-r--r--   0        0        0      958 2024-05-28 12:00:27.404805 basketball_reference_webscrapper-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 basketball_reference_webscrapper-0.1.7/PKG-INFO
```

### Comparing `basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/constants/team_city_refdata.csv` & `basketball_reference_webscrapper-0.1.7/basketball_reference_webscrapper/constants/team_city_refdata.csv`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/params.yaml` & `basketball_reference_webscrapper-0.1.7/basketball_reference_webscrapper/params.yaml`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/utils/logs.py` & `basketball_reference_webscrapper-0.1.7/basketball_reference_webscrapper/utils/logs.py`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/webscrapping_basketball_reference.py` & `basketball_reference_webscrapper-0.1.7/basketball_reference_webscrapper/webscrapping_basketball_reference.py`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.1.6/pyproject.toml` & `basketball_reference_webscrapper-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "basketball-reference-webscrapper"
-version = "0.1.6"
+version = "0.1.7"
 description = "Python package for Basketball Reference that gathers data by scraping the website"
 authors = ["Yannick Flores <yannick.flores1992@gmail.com>"]
 readme = "README.md"
 exclude = ["tests", "docs"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `basketball_reference_webscrapper-0.1.6/PKG-INFO` & `basketball_reference_webscrapper-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basketball-reference-webscrapper
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for Basketball Reference that gathers data by scraping the website
 Author: Yannick Flores
 Author-email: yannick.flores1992@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

