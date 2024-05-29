# Comparing `tmp/airbyte-source-kyve-0.2.0.tar.gz` & `tmp/airbyte_source_kyve-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-kyve-0.2.0.tar", last modified: Wed Jan 31 12:32:10 2024, max compression
+gzip compressed data, was "airbyte_source_kyve-0.2.1.tar", max compression
```

## Comparing `airbyte-source-kyve-0.2.0.tar` & `airbyte_source_kyve-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,9 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 12:32:10.065131 airbyte-source-kyve-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     2586 2024-01-31 12:32:10.065131 airbyte-source-kyve-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2255 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 12:32:10.065131 airbyte-source-kyve-0.2.0/airbyte_source_kyve.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2586 2024-01-31 12:32:10.000000 airbyte-source-kyve-0.2.0/airbyte_source_kyve.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2024-01-31 12:32:10.000000 airbyte-source-kyve-0.2.0/airbyte_source_kyve.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 12:32:10.000000 airbyte-source-kyve-0.2.0/airbyte_source_kyve.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-01-31 12:32:10.000000 airbyte-source-kyve-0.2.0/airbyte_source_kyve.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-31 12:32:10.000000 airbyte-source-kyve-0.2.0/airbyte_source_kyve.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       41 2024-01-31 12:32:10.000000 airbyte-source-kyve-0.2.0/airbyte_source_kyve.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 12:32:10.061131 airbyte-source-kyve-0.2.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       49 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      911 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)      125 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/integration_tests/config.json
--rw-r--r--   0 root         (0) root         (0)      257 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      334 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/integration_tests/incremental_catalog.json
--rw-r--r--   0 root         (0) root         (0)       20 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      129 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/integration_tests/multiple_pools_config.json
--rw-r--r--   0 root         (0) root         (0)     2421 2024-01-31 12:32:10.069131 airbyte-source-kyve-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      915 2024-01-31 12:32:08.000000 airbyte-source-kyve-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 12:32:10.061131 airbyte-source-kyve-0.2.0/source_kyve/
--rw-r--r--   0 root         (0) root         (0)      120 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/source_kyve/__init__.py
--rw-r--r--   0 root         (0) root         (0)      224 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/source_kyve/run.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/source_kyve/source.py
--rw-r--r--   0 root         (0) root         (0)     1383 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/source_kyve/spec.yaml
--rw-r--r--   0 root         (0) root         (0)     6841 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/source_kyve/stream.py
--rw-r--r--   0 root         (0) root         (0)      321 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/source_kyve/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 12:32:10.065131 airbyte-source-kyve-0.2.0/unit_tests/
--rw-r--r--   0 root         (0) root         (0)     1687 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1605190 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/unit_tests/test_data.py
--rw-r--r--   0 root         (0) root         (0)     2351 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/unit_tests/test_incremental_streams.py
--rw-r--r--   0 root         (0) root         (0)      533 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)     8767 2024-01-31 12:18:13.000000 airbyte-source-kyve-0.2.0/unit_tests/test_streams.py
+-rw-r--r--   0        0        0     4460 2024-05-29 12:04:43.000000 airbyte_source_kyve-0.2.1/README.md
+-rw-r--r--   0        0        0      731 2024-05-29 13:20:21.582315 airbyte_source_kyve-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-05-29 12:04:43.000000 airbyte_source_kyve-0.2.1/source_kyve/__init__.py
+-rw-r--r--   0        0        0      224 2024-05-29 12:04:43.000000 airbyte_source_kyve-0.2.1/source_kyve/run.py
+-rw-r--r--   0        0        0     1840 2024-05-29 12:04:43.000000 airbyte_source_kyve-0.2.1/source_kyve/source.py
+-rw-r--r--   0        0        0     1383 2024-05-29 12:04:43.000000 airbyte_source_kyve-0.2.1/source_kyve/spec.yaml
+-rw-r--r--   0        0        0     6841 2024-05-29 12:04:43.000000 airbyte_source_kyve-0.2.1/source_kyve/stream.py
+-rw-r--r--   0        0        0      321 2024-05-29 12:04:43.000000 airbyte_source_kyve-0.2.1/source_kyve/utils.py
+-rw-r--r--   0        0        0     5158 1970-01-01 00:00:00.000000 airbyte_source_kyve-0.2.1/PKG-INFO
```

### Comparing `airbyte-source-kyve-0.2.0/source_kyve/source.py` & `airbyte_source_kyve-0.2.1/source_kyve/source.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-kyve-0.2.0/source_kyve/spec.yaml` & `airbyte_source_kyve-0.2.1/source_kyve/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-kyve-0.2.0/source_kyve/stream.py` & `airbyte_source_kyve-0.2.1/source_kyve/stream.py`

 * *Files identical despite different names*

