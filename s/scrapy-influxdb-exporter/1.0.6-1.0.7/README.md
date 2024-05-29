# Comparing `tmp/scrapy-influxdb-exporter-1.0.6.tar.gz` & `tmp/scrapy_influxdb_exporter-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-influxdb-exporter-1.0.6.tar", last modified: Sat Apr  6 15:36:26 2024, max compression
+gzip compressed data, was "scrapy_influxdb_exporter-1.0.7.tar", last modified: Wed May 29 10:26:24 2024, max compression
```

## Comparing `scrapy-influxdb-exporter-1.0.6.tar` & `scrapy_influxdb_exporter-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:36:26.745947 scrapy-influxdb-exporter-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-06 15:36:22.000000 scrapy-influxdb-exporter-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-06 15:36:26.745947 scrapy-influxdb-exporter-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-06 15:36:22.000000 scrapy-influxdb-exporter-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-06 15:36:22.000000 scrapy-influxdb-exporter-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:36:26.745947 scrapy-influxdb-exporter-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:36:26.741948 scrapy-influxdb-exporter-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:36:26.745947 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:36:22.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-06 15:36:22.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-06 15:36:22.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter/statscollectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:36:26.745947 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-06 15:36:26.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-06 15:36:26.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:36:26.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 15:36:26.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-06 15:36:26.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:26:24.476918 scrapy_influxdb_exporter-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-29 10:26:20.000000 scrapy_influxdb_exporter-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-29 10:26:24.476918 scrapy_influxdb_exporter-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-29 10:26:20.000000 scrapy_influxdb_exporter-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-29 10:26:20.000000 scrapy_influxdb_exporter-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:26:24.476918 scrapy_influxdb_exporter-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:26:24.476918 scrapy_influxdb_exporter-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:26:24.476918 scrapy_influxdb_exporter-1.0.7/src/scrapy_influxdb_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:26:20.000000 scrapy_influxdb_exporter-1.0.7/src/scrapy_influxdb_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-29 10:26:20.000000 scrapy_influxdb_exporter-1.0.7/src/scrapy_influxdb_exporter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-29 10:26:20.000000 scrapy_influxdb_exporter-1.0.7/src/scrapy_influxdb_exporter/statscollectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:26:24.476918 scrapy_influxdb_exporter-1.0.7/src/scrapy_influxdb_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-29 10:26:24.000000 scrapy_influxdb_exporter-1.0.7/src/scrapy_influxdb_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-29 10:26:24.000000 scrapy_influxdb_exporter-1.0.7/src/scrapy_influxdb_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:26:24.000000 scrapy_influxdb_exporter-1.0.7/src/scrapy_influxdb_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 10:26:24.000000 scrapy_influxdb_exporter-1.0.7/src/scrapy_influxdb_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 10:26:24.000000 scrapy_influxdb_exporter-1.0.7/src/scrapy_influxdb_exporter.egg-info/top_level.txt
```

### Comparing `scrapy-influxdb-exporter-1.0.6/LICENSE` & `scrapy_influxdb_exporter-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-influxdb-exporter-1.0.6/PKG-INFO` & `scrapy_influxdb_exporter-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-influxdb-exporter
-Version: 1.0.6
+Version: 1.0.7
 Summary: A simple package to export Scrapy spider stats to InfluxDB
 Author-email: Stefano Fusai <stefanofusai@gmail.com>
 Project-URL: Homepage, https://github.com/stefanofusai/scrapy-influxdb-exporter
 Project-URL: Repository, https://github.com/stefanofusai/scrapy-influxdb-exporter
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `scrapy-influxdb-exporter-1.0.6/README.md` & `scrapy_influxdb_exporter-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `scrapy-influxdb-exporter-1.0.6/pyproject.toml` & `scrapy_influxdb_exporter-1.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scrapy-influxdb-exporter"
-version = "1.0.6"
+version = "1.0.7"
 authors = [{ "name" = "Stefano Fusai", "email" = "stefanofusai@gmail.com" }]
 description = "A simple package to export Scrapy spider stats to InfluxDB"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = ["influxdb3-python", "scrapy"]
 
 [project.urls]
```

### Comparing `scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter/statscollectors.py` & `scrapy_influxdb_exporter-1.0.7/src/scrapy_influxdb_exporter/statscollectors.py`

 * *Files identical despite different names*

### Comparing `scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/PKG-INFO` & `scrapy_influxdb_exporter-1.0.7/src/scrapy_influxdb_exporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-influxdb-exporter
-Version: 1.0.6
+Version: 1.0.7
 Summary: A simple package to export Scrapy spider stats to InfluxDB
 Author-email: Stefano Fusai <stefanofusai@gmail.com>
 Project-URL: Homepage, https://github.com/stefanofusai/scrapy-influxdb-exporter
 Project-URL: Repository, https://github.com/stefanofusai/scrapy-influxdb-exporter
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

