# Comparing `tmp/azure-appconfiguration-provider-1.1.0b3.tar.gz` & `tmp/azure-appconfiguration-provider-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-appconfiguration-provider-1.1.0b3.tar", last modified: Tue Dec 19 19:39:41 2023, max compression
+gzip compressed data, was "azure-appconfiguration-provider-1.2.0.tar", last modified: Tue May 28 16:36:37 2024, max compression
```

## Comparing `azure-appconfiguration-provider-1.1.0b3.tar` & `azure-appconfiguration-provider-1.2.0.tar`

### file list

```diff
@@ -1,56 +1,60 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-19 19:39:41.175974 azure-appconfiguration-provider-1.1.0b3/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3525 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      284 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    12602 2023-12-19 19:39:41.175974 azure-appconfiguration-provider-1.1.0b3/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7942 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-19 19:39:41.171974 azure-appconfiguration-provider-1.1.0b3/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-19 19:39:41.171974 azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-19 19:39:41.171974 azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      691 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27975 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/_azureappconfigurationprovider.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      825 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/_constants.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2659 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/_models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      407 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/_user_agent.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      329 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-19 19:39:41.171974 azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      458 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24069 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/aio/_azureappconfigurationproviderasync.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-19 19:39:41.175974 azure-appconfiguration-provider-1.1.0b3/azure_appconfiguration_provider.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    12602 2023-12-19 19:39:41.000000 azure-appconfiguration-provider-1.1.0b3/azure_appconfiguration_provider.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1615 2023-12-19 19:39:41.000000 azure-appconfiguration-provider-1.1.0b3/azure_appconfiguration_provider.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-12-19 19:39:41.000000 azure-appconfiguration-provider-1.1.0b3/azure_appconfiguration_provider.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-12-19 19:39:40.000000 azure-appconfiguration-provider-1.1.0b3/azure_appconfiguration_provider.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      115 2023-12-19 19:39:41.000000 azure-appconfiguration-provider-1.1.0b3/azure_appconfiguration_provider.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2023-12-19 19:39:41.000000 azure-appconfiguration-provider-1.1.0b3/azure_appconfiguration_provider.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       99 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/pyproject.toml
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-19 19:39:41.171974 azure-appconfiguration-provider-1.1.0b3/samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2082 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/samples/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1356 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/samples/aad_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1606 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/samples/async_aad_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1471 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/samples/async_connection_string_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1301 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/samples/async_key_vault_reference_provided_clients_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1206 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/samples/async_key_vault_reference_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1260 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/samples/connection_string_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1043 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/samples/key_vault_reference_customized_clients_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      985 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/samples/key_vault_reference_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1965 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/samples/refresh_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2367 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/samples/sample_utilities.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-12-19 19:39:41.175974 azure-appconfiguration-provider-1.1.0b3/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2757 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-19 19:39:41.175974 azure-appconfiguration-provider-1.1.0b3/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1758 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/tests/async_preparers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5553 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/tests/asynctestcase.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1631 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/tests/conftest.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3021 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/tests/preparers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5179 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/tests/test_async_provider.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5146 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/tests/test_async_provider_aad.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5236 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/tests/test_async_provider_refresh.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5388 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/tests/test_provider.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4728 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/tests/test_provider_aad.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4869 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/tests/test_provider_backoff.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4164 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/tests/test_provider_refresh.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6677 2023-12-19 19:38:55.000000 azure-appconfiguration-provider-1.1.0b3/tests/testcase.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 16:36:37.928516 azure-appconfiguration-provider-1.2.0/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4611 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      284 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15274 2024-05-28 16:36:37.928516 azure-appconfiguration-provider-1.2.0/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9692 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 16:36:37.920517 azure-appconfiguration-provider-1.2.0/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 16:36:37.920517 azure-appconfiguration-provider-1.2.0/azure/appconfiguration/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/azure/appconfiguration/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 16:36:37.924517 azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      691 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36839 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/_azureappconfigurationprovider.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1382 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/_constants.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2659 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/_models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      407 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/_user_agent.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      327 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 16:36:37.924517 azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      458 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    31845 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/aio/_azureappconfigurationproviderasync.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 16:36:37.924517 azure-appconfiguration-provider-1.2.0/azure_appconfiguration_provider.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15274 2024-05-28 16:36:37.000000 azure-appconfiguration-provider-1.2.0/azure_appconfiguration_provider.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1769 2024-05-28 16:36:37.000000 azure-appconfiguration-provider-1.2.0/azure_appconfiguration_provider.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-28 16:36:37.000000 azure-appconfiguration-provider-1.2.0/azure_appconfiguration_provider.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-28 16:36:37.000000 azure-appconfiguration-provider-1.2.0/azure_appconfiguration_provider.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       79 2024-05-28 16:36:37.000000 azure-appconfiguration-provider-1.2.0/azure_appconfiguration_provider.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-05-28 16:36:37.000000 azure-appconfiguration-provider-1.2.0/azure_appconfiguration_provider.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       60 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/pyproject.toml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 16:36:37.928516 azure-appconfiguration-provider-1.2.0/samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2082 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/samples/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1356 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/samples/aad_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1602 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/samples/async_aad_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1467 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/samples/async_connection_string_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1293 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/samples/async_key_vault_reference_provided_clients_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1202 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/samples/async_key_vault_reference_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1256 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/samples/connection_string_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1035 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/samples/key_vault_reference_customized_clients_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      981 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/samples/key_vault_reference_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1980 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/samples/refresh_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2427 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/samples/refresh_sample_feature_flags.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2436 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/samples/sample_utilities.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-05-28 16:36:37.928516 azure-appconfiguration-provider-1.2.0/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2723 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 16:36:37.928516 azure-appconfiguration-provider-1.2.0/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1758 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/async_preparers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6694 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/asynctestcase.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1526 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/conftest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2866 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/preparers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5224 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/test_async_provider.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5149 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/test_async_provider_aad.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2145 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/test_async_provider_feature_management.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6057 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/test_async_provider_refresh.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/test_constants.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5486 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/test_provider.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4826 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/test_provider_aad.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4869 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/test_provider_backoff.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1903 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/test_provider_feature_management.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4884 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/test_provider_refresh.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7932 2024-05-28 16:34:51.000000 azure-appconfiguration-provider-1.2.0/tests/testcase.py
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/CHANGELOG.md` & `azure-appconfiguration-provider-1.2.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 # Release History
 
+## 1.2.0 (2024-05-24)
+
+### Features Added
+
+* Enable loading of feature flags with `feature_flag_enabled`
+* Select Feature Flags to load with `feature_flag_selectors`
+* Enable/Disable Feature Flag Refresh with `feature_flag_refresh_enabled`
+
+### Bugs Fixed
+
+* Fixes issue where loading configurations were slower due to returning a copy of the configurations.
+
+## 1.1.0 (2024-01-29)
+
+### Features Added
+
+* New API for Azure App Configuration Provider, `refresh`, which can be used to refresh the configuration from the Azure App Configuration service. `refresh` by default can check every 30 seconds for changes to specified sentinel keys. If a change is detected then all configurations are reloaded. Sentinel keys can be set by passing a list of `SentinelKey`'s to `refresh_on`.
+* Added new options `on_refresh_success` and `on_refresh_failure` callbacks to the load method. These callbacks are called when the refresh method successfully refreshes the configuration or fails to refresh the configuration.
+
+### Bugs Fixed
+
+* Verifies that the `refresh_interval` is at least 1 second.
+
 ## 1.1.0b3 (2023-12-19)
 
 ### Features Added
 
 - Added on_refresh_success callback to load method. This callback is called when the refresh method successfully refreshes the configuration.
 - Added minimum up time. This is the minimum amount of time the provider will try to be up before throwing an error. This is to prevent quick restart loops.
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/LICENSE` & `azure-appconfiguration-provider-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-provider-1.1.0b3/PKG-INFO` & `azure-appconfiguration-provider-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: azure-appconfiguration-provider
-Version: 1.1.0b3
+Version: 1.2.0
 Summary: Microsoft App Configuration Provider Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/appconfiguration/azure-appconfiguration-provider
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: msrest>=0.6.21
-Requires-Dist: azure-core<2.0.0,>=1.25.0
-Requires-Dist: azure-appconfiguration<2.0.0,>=1.4.0
-Requires-Dist: azure-keyvault-secrets<5.0.0,>=4.3.0
 
 # Azure App Configuration Python Provider client library for Python
 
 Azure App Configuration is a managed service that helps developers centralize their application configurations simply and securely. This provider adds additional functionality above the azure-sdk-for-python.
 
 Using the provider enables loading sets of configurations from an Azure App Configuration store in a managed way.
 
@@ -65,26 +61,26 @@
 
 ### Features
 
 Currently the Azure App Configuration Provider enables:
 
 * Connecting to an App Configuration Store using a connection string or Azure Active Directory.
 * Selecting multiple sets of configurations using `SettingSelector`.
+* Loading Feature Flags
 * Dynamic Refresh
 * Trim prefixes off key names.
 * Resolving Key Vault References, requires AAD.
 * Secret Resolver, resolve Key Vault References locally without connecting to Key Vault.
 * Json Content Type
 
 #### Future Features
 
 List of features we are going to add to the Python Provider in the future.
 
 * Geo-Replication support
-* Feature Management
 * Configuration Placeholders
 
 ## Examples
 
 ### Selecting configurations
 
 You can refine or expand the configurations loaded from your store by using `SettingSelector`s. Setting selectors provide a way to pass a key filter and label filter into the provider.
@@ -191,14 +187,44 @@
     return "From Secret Resolver"
 
 key_vault_options = AzureAppConfigurationKeyVaultOptions(
     secret_resolver=secret_resolver)
 config = load(endpoint=endpoint, credential=DefaultAzureCredential(), key_vault_options=key_vault_options)
 ```
 
+## Loading Feature Flags
+
+Feature Flags can be loaded from config stores using the provider. Feature flags are loaded as a dictionary of key/value pairs stored in the provider under the `feature_management`, then `feature_flags`.
+
+```python
+config = load(endpoint=endpoint, credential=DefaultAzureCredential(), feature_flags_enabled=True)
+alpha = config["feature_management"]["feature_flags"]["Alpha"]
+print(alpha["enabled"])
+```
+
+By default all feature flags with no label are loaded when `feature_flags_enabled` is set to `True`. . If you want to load feature flags with a specific label you can use `SettingSelector` to filter the feature flags.
+
+```python
+from azure.appconfiguration.provider import load, SettingSelector
+
+config = load(endpoint=endpoint, credential=DefaultAzureCredential(), feature_flags_enabled=True, feature_flag_selectors=[SettingSelector(key_filter="*", label_filter="dev")])
+alpha = config["feature_management"]["feature_flags"]["Alpha"]
+print(alpha["enabled"])
+```
+
+To enable refresh for feature flags you need to enable refresh. This will allow the provider to refresh feature flags the same way it refreshes configurations. Unlike configurations, all loaded feature flags are monitored for changes and will cause a refresh. Refresh of configuration settings and feature flags are independent of each other. Both are trigged by the `refresh` method, but a feature flag changing will not cause a refresh of configurations and vice versa. Also, if refresh for configuration settings is not enabled, feature flags can still be enabled for refresh.
+
+```python
+config = load(endpoint=endpoint, credential=DefaultAzureCredential(), feature_flags_enabled=True, feature_flag_refresh_enabled=True)
+
+...
+
+config.refresh()
+```
+
 ## Key concepts
 
 ## Troubleshooting
 
 ## Next steps
 
 Check out our Django and Flask examples to see how to use the provider in a web application.
@@ -226,14 +252,37 @@
 
 [azure_cli]: https://learn.microsoft.com/cli/azure/appconfig
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 
 
 # Release History
 
+## 1.2.0 (2024-05-24)
+
+### Features Added
+
+* Enable loading of feature flags with `feature_flag_enabled`
+* Select Feature Flags to load with `feature_flag_selectors`
+* Enable/Disable Feature Flag Refresh with `feature_flag_refresh_enabled`
+
+### Bugs Fixed
+
+* Fixes issue where loading configurations were slower due to returning a copy of the configurations.
+
+## 1.1.0 (2024-01-29)
+
+### Features Added
+
+* New API for Azure App Configuration Provider, `refresh`, which can be used to refresh the configuration from the Azure App Configuration service. `refresh` by default can check every 30 seconds for changes to specified sentinel keys. If a change is detected then all configurations are reloaded. Sentinel keys can be set by passing a list of `SentinelKey`'s to `refresh_on`.
+* Added new options `on_refresh_success` and `on_refresh_failure` callbacks to the load method. These callbacks are called when the refresh method successfully refreshes the configuration or fails to refresh the configuration.
+
+### Bugs Fixed
+
+* Verifies that the `refresh_interval` is at least 1 second.
+
 ## 1.1.0b3 (2023-12-19)
 
 ### Features Added
 
 - Added on_refresh_success callback to load method. This callback is called when the refresh method successfully refreshes the configuration.
 - Added minimum up time. This is the minimum amount of time the provider will try to be up before throwing an error. This is to prevent quick restart loops.
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/README.md` & `azure-appconfiguration-provider-1.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -38,26 +38,26 @@
 
 ### Features
 
 Currently the Azure App Configuration Provider enables:
 
 * Connecting to an App Configuration Store using a connection string or Azure Active Directory.
 * Selecting multiple sets of configurations using `SettingSelector`.
+* Loading Feature Flags
 * Dynamic Refresh
 * Trim prefixes off key names.
 * Resolving Key Vault References, requires AAD.
 * Secret Resolver, resolve Key Vault References locally without connecting to Key Vault.
 * Json Content Type
 
 #### Future Features
 
 List of features we are going to add to the Python Provider in the future.
 
 * Geo-Replication support
-* Feature Management
 * Configuration Placeholders
 
 ## Examples
 
 ### Selecting configurations
 
 You can refine or expand the configurations loaded from your store by using `SettingSelector`s. Setting selectors provide a way to pass a key filter and label filter into the provider.
@@ -164,14 +164,44 @@
     return "From Secret Resolver"
 
 key_vault_options = AzureAppConfigurationKeyVaultOptions(
     secret_resolver=secret_resolver)
 config = load(endpoint=endpoint, credential=DefaultAzureCredential(), key_vault_options=key_vault_options)
 ```
 
+## Loading Feature Flags
+
+Feature Flags can be loaded from config stores using the provider. Feature flags are loaded as a dictionary of key/value pairs stored in the provider under the `feature_management`, then `feature_flags`.
+
+```python
+config = load(endpoint=endpoint, credential=DefaultAzureCredential(), feature_flags_enabled=True)
+alpha = config["feature_management"]["feature_flags"]["Alpha"]
+print(alpha["enabled"])
+```
+
+By default all feature flags with no label are loaded when `feature_flags_enabled` is set to `True`. . If you want to load feature flags with a specific label you can use `SettingSelector` to filter the feature flags.
+
+```python
+from azure.appconfiguration.provider import load, SettingSelector
+
+config = load(endpoint=endpoint, credential=DefaultAzureCredential(), feature_flags_enabled=True, feature_flag_selectors=[SettingSelector(key_filter="*", label_filter="dev")])
+alpha = config["feature_management"]["feature_flags"]["Alpha"]
+print(alpha["enabled"])
+```
+
+To enable refresh for feature flags you need to enable refresh. This will allow the provider to refresh feature flags the same way it refreshes configurations. Unlike configurations, all loaded feature flags are monitored for changes and will cause a refresh. Refresh of configuration settings and feature flags are independent of each other. Both are trigged by the `refresh` method, but a feature flag changing will not cause a refresh of configurations and vice versa. Also, if refresh for configuration settings is not enabled, feature flags can still be enabled for refresh.
+
+```python
+config = load(endpoint=endpoint, credential=DefaultAzureCredential(), feature_flags_enabled=True, feature_flag_refresh_enabled=True)
+
+...
+
+config.refresh()
+```
+
 ## Key concepts
 
 ## Troubleshooting
 
 ## Next steps
 
 Check out our Django and Flask examples to see how to use the provider in a web application.
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/__init__.py` & `azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/_azureappconfigurationprovider.py` & `azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/aio/_azureappconfigurationproviderasync.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,162 +1,195 @@
 # ------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
-import copy
-import os
 import json
-import random
-import time
-import datetime
 from threading import Lock
+import datetime
 import logging
 from typing import (
     Any,
+    Awaitable,
     Callable,
     Dict,
-    Iterable,
     Mapping,
     Optional,
     overload,
     List,
     Tuple,
     TYPE_CHECKING,
     Union,
+    Iterator,
+    KeysView,
+    ItemsView,
+    ValuesView,
+    TypeVar,
 )
-from azure.appconfiguration import (  # pylint:disable=no-name-in-module
-    AzureAppConfigurationClient,
+
+from azure.appconfiguration import (  # type: ignore # pylint:disable=no-name-in-module
     FeatureFlagConfigurationSetting,
     SecretReferenceConfigurationSetting,
+    ConfigurationSetting,
 )
+from azure.appconfiguration.aio import AzureAppConfigurationClient
+from azure.keyvault.secrets.aio import SecretClient
+from azure.keyvault.secrets import KeyVaultSecretIdentifier
 from azure.core import MatchConditions
 from azure.core.exceptions import HttpResponseError, ServiceRequestError, ServiceResponseError
-from azure.keyvault.secrets import SecretClient, KeyVaultSecretIdentifier
-from ._models import AzureAppConfigurationKeyVaultOptions, SettingSelector
-from ._constants import (
+
+from .._models import AzureAppConfigurationKeyVaultOptions, SettingSelector
+from .._constants import (
     FEATURE_MANAGEMENT_KEY,
+    FEATURE_FLAG_KEY,
     FEATURE_FLAG_PREFIX,
-    REQUEST_TRACING_DISABLED_ENVIRONMENT_VARIABLE,
-    ServiceFabricEnvironmentVariable,
-    AzureFunctionEnvironmentVariable,
-    AzureWebAppEnvironmentVariable,
-    ContainerAppEnvironmentVariable,
-    KubernetesEnvironmentVariable,
     EMPTY_LABEL,
+    PERCENTAGE_FILTER_NAMES,
+    TIME_WINDOW_FILTER_NAMES,
+    TARGETING_FILTER_NAMES,
+    CUSTOM_FILTER_KEY,
+    PERCENTAGE_FILTER_KEY,
+    TIME_WINDOW_FILTER_KEY,
+    TARGETING_FILTER_KEY,
+)
+from .._azureappconfigurationprovider import (
+    _is_json_content_type,
+    _get_headers,
+    _RefreshTimer,
+    _build_sentinel,
+    _delay_failure,
 )
-from ._user_agent import USER_AGENT
+from .._user_agent import USER_AGENT
 
 if TYPE_CHECKING:
-    from azure.core.credentials import TokenCredential
-
-JSON = Union[str, Mapping[str, Any]]  # pylint: disable=unsubscriptable-object
+    from azure.core.credentials_async import AsyncTokenCredential
 
-logger = logging.getLogger(__name__)
-
-min_uptime = 5
+JSON = Mapping[str, Any]  # pylint: disable=unsubscriptable-object
+_T = TypeVar("_T")
 
 
 @overload
-def load(
+async def load(  # pylint: disable=docstring-keyword-should-match-keyword-only
     endpoint: str,
-    credential: "TokenCredential",
+    credential: "AsyncTokenCredential",
     *,
     selects: Optional[List[SettingSelector]] = None,
     trim_prefixes: Optional[List[str]] = None,
+    keyvault_credential: Optional["AsyncTokenCredential"] = None,
+    keyvault_client_configs: Optional[Mapping[str, JSON]] = None,
+    secret_resolver: Optional[Callable[[str], str]] = None,
     key_vault_options: Optional[AzureAppConfigurationKeyVaultOptions] = None,
     refresh_on: Optional[List[Tuple[str, str]]] = None,
     refresh_interval: int = 30,
     on_refresh_success: Optional[Callable] = None,
-    on_refresh_error: Optional[Callable[[Exception], None]] = None,
+    on_refresh_error: Optional[Callable[[Exception], Awaitable[None]]] = None,
     **kwargs
 ) -> "AzureAppConfigurationProvider":
     """
     Loads configuration settings from Azure App Configuration into a Python application.
 
     :param str endpoint: Endpoint for App Configuration resource.
     :param credential: Credential for App Configuration resource.
-    :type credential: ~azure.core.credentials.TokenCredential
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :keyword selects: List of setting selectors to filter configuration settings
     :paramtype selects: Optional[List[~azure.appconfiguration.provider.SettingSelector]]
     :keyword trim_prefixes: List of prefixes to trim from configuration keys
     :paramtype trim_prefixes: Optional[List[str]]
     :keyword keyvault_credential: A credential for authenticating with the key vault. This is optional if
      keyvault_client_configs is provided.
-    :paramtype keyvault_credential: ~azure.core.credentials.TokenCredential
+    :paramtype keyvault_credential: ~azure.core.credentials_async.AsyncTokenCredential
     :keyword keyvault_client_configs: A Mapping of SecretClient endpoints to client configurations from
      azure-keyvault-secrets. This is optional if keyvault_credential is provided. If a credential isn't provided a
      credential will need to be in each set for each.
     :paramtype keyvault_client_configs: Mapping[str, Mapping]
     :keyword secret_resolver: A function that takes a URI and returns a value.
     :paramtype secret_resolver: Callable[[str], str]
     :keyword refresh_on: One or more settings whose modification will trigger a full refresh after a fixed interval.
     This should be a list of Key-Label pairs for specific settings (filters and wildcards are not supported).
     :paramtype refresh_on: List[Tuple[str, str]]
     :keyword int refresh_interval: The minimum time in seconds between when a call to `refresh` will actually trigger a
      service call to update the settings. Default value is 30 seconds.
-    :paramtype on_refresh_success: Optional[Callable]
     :keyword on_refresh_success: Optional callback to be invoked when a change is found and a successful refresh has
     happened.
-    :paramtype on_refresh_error: Optional[Callable[[Exception], None]]
+    :paramtype on_refresh_success: Optional[Callable]
     :keyword on_refresh_error: Optional callback to be invoked when an error occurs while refreshing settings. If not
     specified, errors will be raised.
+    :paramtype on_refresh_error: Optional[Callable[[Exception], Awaitable[None]]]
+    :keyword feature_flag_enabled: Optional flag to enable or disable the loading of feature flags. Default is False.
+    :paramtype feature_flag_enabled: bool
+    :keyword feature_flag_selectors: Optional list of selectors to filter feature flags. By default will load all
+    feature flags without a label.
+    :paramtype feature_flag_selectors: List[SettingSelector]
+    :keyword feature_flag_refresh_enabled: Optional flag to enable or disable the refresh of feature flags. Default is
+    False.
+    :paramtype feature_flag_refresh_enabled: bool
     """
 
 
 @overload
-def load(
+async def load(  # pylint: disable=docstring-keyword-should-match-keyword-only
     *,
     connection_string: str,
     selects: Optional[List[SettingSelector]] = None,
     trim_prefixes: Optional[List[str]] = None,
+    keyvault_credential: Optional["AsyncTokenCredential"] = None,
+    keyvault_client_configs: Optional[Mapping[str, JSON]] = None,
+    secret_resolver: Optional[Callable[[str], str]] = None,
     key_vault_options: Optional[AzureAppConfigurationKeyVaultOptions] = None,
     refresh_on: Optional[List[Tuple[str, str]]] = None,
     refresh_interval: int = 30,
     on_refresh_success: Optional[Callable] = None,
-    on_refresh_error: Optional[Callable[[Exception], None]] = None,
+    on_refresh_error: Optional[Callable[[Exception], Awaitable[None]]] = None,
     **kwargs
 ) -> "AzureAppConfigurationProvider":
     """
     Loads configuration settings from Azure App Configuration into a Python application.
 
     :keyword str connection_string: Connection string for App Configuration resource.
     :keyword selects: List of setting selectors to filter configuration settings
     :paramtype selects: Optional[List[~azure.appconfiguration.provider.SettingSelector]]
     :keyword trim_prefixes: List of prefixes to trim from configuration keys
     :paramtype trim_prefixes: Optional[List[str]]
     :keyword keyvault_credential: A credential for authenticating with the key vault. This is optional if
      keyvault_client_configs is provided.
-    :paramtype keyvault_credential: ~azure.core.credentials.TokenCredential
+    :paramtype keyvault_credential: ~azure.core.credentials_async.AsyncTokenCredential
     :keyword keyvault_client_configs: A Mapping of SecretClient endpoints to client configurations from
      azure-keyvault-secrets. This is optional if keyvault_credential is provided. If a credential isn't provided a
      credential will need to be in each set for each.
     :paramtype keyvault_client_configs: Mapping[str, Mapping]
     :keyword secret_resolver: A function that takes a URI and returns a value.
     :paramtype secret_resolver: Callable[[str], str]
     :keyword refresh_on: One or more settings whose modification will trigger a full refresh after a fixed interval.
     This should be a list of Key-Label pairs for specific settings (filters and wildcards are not supported).
     :paramtype refresh_on: List[Tuple[str, str]]
     :keyword int refresh_interval: The minimum time in seconds between when a call to `refresh` will actually trigger a
      service call to update the settings. Default value is 30 seconds.
-    :paramtype on_refresh_success: Optional[Callable]
     :keyword on_refresh_success: Optional callback to be invoked when a change is found and a successful refresh has
-     happened.
-    :paramtype on_refresh_error: Optional[Callable[[Exception], None]]
+    happened.
+    :paramtype on_refresh_success: Optional[Callable]
     :keyword on_refresh_error: Optional callback to be invoked when an error occurs while refreshing settings. If not
-    specified, errors will be raised.
+     specified, errors will be raised.
+    :paramtype on_refresh_error: Optional[Callable[[Exception], Awaitable[None]]]
+    :keyword feature_flag_enabled: Optional flag to enable or disable the loading of feature flags. Default is False.
+    :paramtype feature_flag_enabled: bool
+    :keyword feature_flag_selectors: Optional list of selectors to filter feature flags. By default will load all
+     feature flags without a label.
+    :paramtype feature_flag_selectors: List[SettingSelector]
+    :keyword feature_flag_refresh_enabled: Optional flag to enable or disable the refresh of feature flags. Default is
+     False.
+    :paramtype feature_flag_refresh_enabled: bool
     """
 
 
-def load(*args, **kwargs) -> "AzureAppConfigurationProvider":
+async def load(*args, **kwargs) -> "AzureAppConfigurationProvider":
     # pylint:disable=protected-access
 
     # Start by parsing kwargs
     endpoint: Optional[str] = kwargs.pop("endpoint", None)
-    credential: Optional["TokenCredential"] = kwargs.pop("credential", None)
+    credential: Optional["AsyncTokenCredential"] = kwargs.pop("credential", None)
     connection_string: Optional[str] = kwargs.pop("connection_string", None)
     key_vault_options: Optional[AzureAppConfigurationKeyVaultOptions] = kwargs.pop("key_vault_options", None)
     start_time = datetime.datetime.now()
 
     # Update endpoint and credential if specified positionally.
     if len(args) > 2:
         raise TypeError(
@@ -187,82 +220,47 @@
     if kwargs.get("keyvault_credential") is not None and kwargs.get("secret_resolver") is not None:
         raise ValueError("A keyvault credential and secret resolver can't both be configured.")
 
     headers = _get_headers("Startup", **kwargs)
     provider = _buildprovider(
         connection_string, endpoint, credential, uses_key_vault="UsesKeyVault" in headers, **kwargs
     )
+
     try:
-        provider._load_all(headers=headers)
+        await provider._load_all(headers=headers)
     except Exception as e:
         _delay_failure(start_time)
         raise e
 
     # Refresh-All sentinels are not updated on load_all, as they are not necessarily included in the provider.
     for (key, label), etag in provider._refresh_on.items():
         if not etag:
             try:
-                sentinel = provider._client.get_configuration_setting(key, label, headers=headers)
-                provider._refresh_on[(key, label)] = sentinel.etag
+                sentinel = await provider._client.get_configuration_setting(key, label, headers=headers)  # type: ignore
+                provider._refresh_on[(key, label)] = sentinel.etag  # type: ignore
             except HttpResponseError as e:
                 if e.status_code == 404:
                     # If the sentinel is not found a refresh should be triggered when it is created.
                     logging.debug(
                         "WatchKey key: %s label %s was configured but not found. Refresh will be triggered if created.",
                         key,
                         label,
                     )
+                    provider._refresh_on[(key, label)] = None  # type: ignore
                 else:
                     _delay_failure(start_time)
                     raise e
             except Exception as e:
                 _delay_failure(start_time)
                 raise e
     return provider
 
 
-def _delay_failure(start_time: datetime.datetime) -> None:
-    # We want to make sure we are up a minimum amount of time before we kill the process. Otherwise, we could get stuck
-    # in a quick restart loop.
-    min_time = datetime.timedelta(seconds=min_uptime)
-    current_time = datetime.datetime.now()
-    if current_time - start_time < min_time:
-        time.sleep((min_time - (current_time - start_time)).total_seconds())
-
-
-def _get_headers(request_type, **kwargs) -> str:
-    headers = kwargs.pop("headers", {})
-    if os.environ.get(REQUEST_TRACING_DISABLED_ENVIRONMENT_VARIABLE, default="").lower() != "true":
-        correlation_context = "RequestType=" + request_type
-        if (
-            "keyvault_credential" in kwargs
-            or "keyvault_client_configs" in kwargs
-            or "secret_resolver" in kwargs
-            or kwargs.pop("uses_key_vault", False)
-        ):
-            correlation_context += ",UsesKeyVault"
-        host_type = ""
-        if AzureFunctionEnvironmentVariable in os.environ:
-            host_type = "AzureFunction"
-        elif AzureWebAppEnvironmentVariable in os.environ:
-            host_type = "AzureWebApp"
-        elif ContainerAppEnvironmentVariable in os.environ:
-            host_type = "ContainerApp"
-        elif KubernetesEnvironmentVariable in os.environ:
-            host_type = "Kubernetes"
-        elif ServiceFabricEnvironmentVariable in os.environ:
-            host_type = "ServiceFabric"
-        if host_type:
-            correlation_context += ",Host=" + host_type
-        headers["Correlation-Context"] = correlation_context
-    return headers
-
-
 def _buildprovider(
-    connection_string: Optional[str], endpoint: Optional[str], credential: Optional["TokenCredential"], **kwargs
+    connection_string: Optional[str], endpoint: Optional[str], credential: Optional["AsyncTokenCredential"], **kwargs
 ) -> "AzureAppConfigurationProvider":
     # pylint:disable=protected-access
     provider = AzureAppConfigurationProvider(**kwargs)
     retry_total = kwargs.pop("retry_total", 2)
     retry_backoff_max = kwargs.pop("retry_backoff_max", 60)
 
     if "user_agent" in kwargs:
@@ -275,26 +273,28 @@
             connection_string,
             user_agent=user_agent,
             retry_total=retry_total,
             retry_backoff_max=retry_backoff_max,
             **kwargs
         )
         return provider
-    provider._client = AzureAppConfigurationClient(
-        endpoint,
-        credential,
-        user_agent=user_agent,
-        retry_total=retry_total,
-        retry_backoff_max=retry_backoff_max,
-        **kwargs
-    )
-    return provider
+    if endpoint is not None and credential is not None:
+        provider._client = AzureAppConfigurationClient(
+            endpoint,
+            credential,
+            user_agent=user_agent,
+            retry_total=retry_total,
+            retry_backoff_max=retry_backoff_max,
+            **kwargs
+        )
+        return provider
+    raise ValueError("Please pass either endpoint and credential, or a connection string.")
 
 
-def _resolve_keyvault_reference(
+async def _resolve_keyvault_reference(
     config: "SecretReferenceConfigurationSetting", provider: "AzureAppConfigurationProvider"
 ) -> str:
     # pylint:disable=protected-access
     if not (provider._keyvault_credential or provider._keyvault_client_configs or provider._secret_resolver):
         raise ValueError(
             """
             Either a credential to Key Vault, custom Key Vault client, or a secret resolver must be set to resolve Key
@@ -316,311 +316,346 @@
     credential = vault_config.pop("credential", provider._keyvault_credential)
 
     if referenced_client is None and credential is not None:
         referenced_client = SecretClient(vault_url=vault_url, credential=credential, **vault_config)
         provider._secret_clients[vault_url] = referenced_client
 
     if referenced_client:
-        return referenced_client.get_secret(keyvault_identifier.name, version=keyvault_identifier.version).value
+        secret_value = (
+            await referenced_client.get_secret(keyvault_identifier.name, version=keyvault_identifier.version)
+        ).value
+        if secret_value is not None:
+            return secret_value
 
     if provider._secret_resolver:
-        return provider._secret_resolver(config.secret_id)
+        resolved = provider._secret_resolver(config.secret_id)
+        try:
+            # Secret resolver was async
+            return await resolved
+        except TypeError:
+            # Secret resolver was sync
+            return resolved
 
     raise ValueError("No Secret Client found for Key Vault reference %s" % (vault_url))
 
 
-def _is_json_content_type(content_type: str) -> bool:
-    if not content_type:
-        return False
-
-    content_type = content_type.strip().lower()
-    mime_type = content_type.split(";")[0].strip()
-
-    type_parts = mime_type.split("/")
-    if len(type_parts) != 2:
-        return False
-
-    (main_type, sub_type) = type_parts
-    if main_type != "application":
-        return False
-
-    sub_types = sub_type.split("+")
-    if "json" in sub_types:
-        return True
-
-    return False
-
-
-def _build_sentinel(setting: Union[str, Tuple[str, str]]) -> Tuple[str, str]:
-    try:
-        key, label = setting
-    except IndexError:
-        key = setting
-        label = EMPTY_LABEL
-    if "*" in key or "*" in label:
-        raise ValueError("Wildcard key or label filters are not supported for refresh.")
-    return key, label
-
-
-class _RefreshTimer:
-    """
-    A timer that tracks the next refresh time and the number of attempts.
-    """
-
-    def __init__(self, **kwargs):
-        self._interval: int = kwargs.pop("refresh_interval", 30)
-        self._next_refresh_time: float = time.time() + self._interval
-        self._attempts: int = 1
-        self._min_backoff: int = (
-            kwargs.pop("min_backoff", 30) if kwargs.get("min_backoff", 30) <= self._interval else self._interval
-        )
-        self._max_backoff: int = 600 if 600 <= self._interval else self._interval
-
-    def reset(self) -> None:
-        self._next_refresh_time = time.time() + self._interval
-        self._attempts = 1
-
-    def backoff(self) -> None:
-        self._next_refresh_time = time.time() + self._calculate_backoff() / 1000
-        self._attempts += 1
-
-    def needs_refresh(self) -> bool:
-        return time.time() >= self._next_refresh_time
-
-    def _calculate_backoff(self) -> float:
-        max_attempts = 63
-        millisecond = 1000  # 1 Second in milliseconds
-
-        min_backoff_milliseconds = self._min_backoff * millisecond
-        max_backoff_milliseconds = self._max_backoff * millisecond
-
-        if self._max_backoff <= self._min_backoff:
-            return min_backoff_milliseconds
-
-        calculated_milliseconds = max(1, min_backoff_milliseconds) * (1 << min(self._attempts, max_attempts))
-
-        if calculated_milliseconds > max_backoff_milliseconds or calculated_milliseconds <= 0:
-            calculated_milliseconds = max_backoff_milliseconds
-
-        return min_backoff_milliseconds + (
-            random.uniform(0.0, 1.0) * (calculated_milliseconds - min_backoff_milliseconds)
-        )
-
-
 class AzureAppConfigurationProvider(Mapping[str, Union[str, JSON]]):  # pylint: disable=too-many-instance-attributes
     """
     Provides a dictionary-like interface to Azure App Configuration settings. Enables loading of sets of configuration
     settings from Azure App Configuration into a Python application. Enables trimming of prefixes from configuration
     keys. Enables resolution of Key Vault references in configuration settings.
     """
 
     def __init__(self, **kwargs) -> None:
         self._dict: Dict[str, str] = {}
-        self._trim_prefixes: List[str] = []
         self._client: Optional[AzureAppConfigurationClient] = None
         self._secret_clients: Dict[str, SecretClient] = {}
         self._selects: List[SettingSelector] = kwargs.pop(
             "selects", [SettingSelector(key_filter="*", label_filter=EMPTY_LABEL)]
         )
 
         trim_prefixes: List[str] = kwargs.pop("trim_prefixes", [])
-        self._trim_prefixes = sorted(trim_prefixes, key=len, reverse=True)
+        self._trim_prefixes: List[str] = sorted(trim_prefixes, key=len, reverse=True)
 
         refresh_on: List[Tuple[str, str]] = kwargs.pop("refresh_on", None) or []
-        self._refresh_on: Mapping[Tuple[str, str] : Optional[str]] = {_build_sentinel(s): None for s in refresh_on}
+        self._refresh_on: Mapping[Tuple[str, str], Optional[str]] = {_build_sentinel(s): None for s in refresh_on}
         self._refresh_timer: _RefreshTimer = _RefreshTimer(**kwargs)
         self._on_refresh_success: Optional[Callable] = kwargs.pop("on_refresh_success", None)
-        self._on_refresh_error: Optional[Callable[[Exception], None]] = kwargs.pop("on_refresh_error", None)
+        self._on_refresh_error: Optional[Union[Callable[[Exception], Awaitable[None]], None]] = kwargs.pop(
+            "on_refresh_error", None
+        )
         self._keyvault_credential = kwargs.pop("keyvault_credential", None)
         self._secret_resolver = kwargs.pop("secret_resolver", None)
         self._keyvault_client_configs = kwargs.pop("keyvault_client_configs", {})
         self._uses_key_vault = (
             self._keyvault_credential is not None
-            or self._keyvault_client_configs is not None
+            or (self._keyvault_client_configs is not None and len(self._keyvault_client_configs) > 0)
             or self._secret_resolver is not None
         )
+        self._feature_flag_enabled = kwargs.pop("feature_flag_enabled", False)
+        self._feature_flag_selectors = kwargs.pop("feature_flag_selectors", [SettingSelector(key_filter="*")])
+        self._refresh_on_feature_flags: Mapping[Tuple[str, str], Optional[str]] = {}
+        self._feature_flag_refresh_timer: _RefreshTimer = _RefreshTimer(**kwargs)
+        self._feature_flag_refresh_enabled = kwargs.pop("feature_flag_refresh_enabled", False)
+        self._feature_filter_usage: Mapping[str, bool] = {}
         self._update_lock = Lock()
         self._refresh_lock = Lock()
 
-    def refresh(self, **kwargs) -> None:
-        if not self._refresh_on:
-            logging.debug("Refresh called but no refresh options set.")
+    async def refresh(self, **kwargs) -> None:
+        if not self._refresh_on and not self._feature_flag_refresh_enabled:
+            logging.debug("Refresh called but no refresh enabled.")
             return
         if not self._refresh_timer.needs_refresh():
             logging.debug("Refresh called but refresh interval not elapsed.")
             return
         if not self._refresh_lock.acquire(blocking=False):  # pylint: disable= consider-using-with
             logging.debug("Refresh called but refresh already in progress.")
             return
         success = False
         need_refresh = False
         try:
-            updated_sentinel_keys = dict(self._refresh_on)
-            headers = _get_headers("Watch", uses_key_vault=self._uses_key_vault, **kwargs)
-            for (key, label), etag in updated_sentinel_keys.items():
-                try:
-                    updated_sentinel = self._client.get_configuration_setting(
-                        key=key,
-                        label=label,
-                        etag=etag,
-                        match_condition=MatchConditions.IfModified,
-                        headers=headers,
-                        **kwargs
-                    )
-                    if updated_sentinel is not None:
-                        logging.debug(
-                            "Refresh all triggered by key: %s label %s.",
-                            key,
-                            label,
-                        )
-                        need_refresh = True
-
-                        updated_sentinel_keys[(key, label)] = updated_sentinel.etag
-                except HttpResponseError as e:
-                    if e.status_code == 404:
-                        if etag is not None:
-                            # If the sentinel is not found, it means the key/label was deleted, so we should refresh
-                            logging.debug("Refresh all triggered by key: %s label %s.", key, label)
-                            need_refresh = True
-                            updated_sentinel_keys[(key, label)] = None
-                    else:
-                        raise e
-            # Need to only update once, no matter how many sentinels are updated
-            if need_refresh:
-                self._load_all(headers=headers, sentinel_keys=updated_sentinel_keys, **kwargs)
+            if self._refresh_on:
+                need_refresh = await self._refresh_configuration_settings(**kwargs)
+            if self._feature_flag_refresh_enabled:
+                need_refresh = await self._refresh_feature_flags(**kwargs) or need_refresh
             # Even if we don't need to refresh, we should reset the timer
             self._refresh_timer.reset()
             success = True
         except (ServiceRequestError, ServiceResponseError, HttpResponseError) as e:
             # If we get an error we should retry sooner than the next refresh interval
             if self._on_refresh_error:
-                self._on_refresh_error(e)
+                await self._on_refresh_error(e)
                 return
             raise
         finally:
             self._refresh_lock.release()
             if not success:
                 self._refresh_timer.backoff()
             elif need_refresh and self._on_refresh_success:
-                self._on_refresh_success()
+                await self._on_refresh_success()
 
-    def _load_all(self, **kwargs):
+    async def _refresh_configuration_settings(self, **kwargs) -> bool:
+        need_refresh = False
+        updated_sentinel_keys = dict(self._refresh_on)
+        headers = _get_headers(
+            "Watch",
+            uses_key_vault=self._uses_key_vault,
+            feature_filters_used=self._feature_filter_usage,
+            uses_feature_flags=self._feature_flag_enabled,
+            **kwargs
+        )
+        for (key, label), etag in updated_sentinel_keys.items():
+            changed, updated_sentinel = await self._check_configuration_setting(
+                key=key, label=label, etag=etag, headers=headers, **kwargs
+            )
+            if changed:
+                need_refresh = True
+            if updated_sentinel is not None:
+                updated_sentinel_keys[(key, label)] = updated_sentinel.etag
+        # Need to only update once, no matter how many sentinels are updated
+        if need_refresh:
+            configuration_settings, sentinel_keys = await self._load_configuration_settings(**kwargs)
+            if self._feature_flag_enabled:
+                configuration_settings[FEATURE_MANAGEMENT_KEY] = self._dict[FEATURE_MANAGEMENT_KEY]
+            with self._update_lock:
+                self._refresh_on = sentinel_keys
+                self._dict = configuration_settings
+        return need_refresh
+
+    async def _refresh_feature_flags(self, **kwargs) -> bool:
+        feature_flag_sentinel_keys = dict(self._refresh_on_feature_flags)
+        headers = _get_headers(
+            "Watch",
+            uses_key_vault=self._uses_key_vault,
+            feature_filters_used=self._feature_filter_usage,
+            uses_feature_flags=self._feature_flag_enabled,
+            **kwargs
+        )
+        for (key, label), etag in feature_flag_sentinel_keys.items():
+            changed = await self._check_configuration_setting(
+                key=key, label=label, etag=etag, headers=headers, **kwargs
+            )
+            if changed:
+                feature_flags, feature_flag_sentinel_keys = await self._load_feature_flags(**kwargs)
+                with self._update_lock:
+                    updated_configurations: Dict[str, Any] = {}
+                    updated_configurations[FEATURE_MANAGEMENT_KEY] = {}
+                    updated_configurations[FEATURE_MANAGEMENT_KEY][FEATURE_FLAG_KEY] = feature_flags
+                    self._dict.update(updated_configurations)
+                self._refresh_on_feature_flags = feature_flag_sentinel_keys
+                return True
+        return False
+
+    async def _check_configuration_setting(
+        self, key, label, etag, headers, **kwargs
+    ) -> Tuple[bool, Union[ConfigurationSetting, None]]:
+        """
+        Checks if the configuration setting have been updated since the last refresh.
+
+        :param str key: key to check for chances
+        :param str label: label to check for changes
+        :param str etag: etag to check for changes
+        :param Mapping[str, str] headers: headers to use for the request
+        :return: A tuple with the first item being true/false if a change is detected. The second item is the updated
+        value if a change was detected.
+        :rtype: Tuple[bool, Union[ConfigurationSetting, None]]
+        """
+        try:
+            updated_sentinel = await self._client.get_configuration_setting(  # type: ignore
+                key=key, label=label, etag=etag, match_condition=MatchConditions.IfModified, headers=headers, **kwargs
+            )
+            if updated_sentinel is not None:
+                logging.debug(
+                    "Refresh all triggered by key: %s label %s.",
+                    key,
+                    label,
+                )
+                return True, updated_sentinel
+        except HttpResponseError as e:
+            if e.status_code == 404:
+                if etag is not None:
+                    # If the sentinel is not found, it means the key/label was deleted, so we should refresh
+                    logging.debug("Refresh all triggered by key: %s label %s.", key, label)
+                    return True, None
+            else:
+                raise e
+        return False, None
+
+    async def _load_all(self, **kwargs):
+        configuration_settings, sentinel_keys = await self._load_configuration_settings(**kwargs)
+        if self._feature_flag_enabled:
+            feature_flags, feature_flag_sentinel_keys = await self._load_feature_flags(**kwargs)
+            configuration_settings[FEATURE_MANAGEMENT_KEY] = {}
+            configuration_settings[FEATURE_MANAGEMENT_KEY][FEATURE_FLAG_KEY] = feature_flags
+            self._refresh_on_feature_flags = feature_flag_sentinel_keys
+        with self._update_lock:
+            self._refresh_on = sentinel_keys
+            self._dict = configuration_settings
+
+    async def _load_configuration_settings(self, **kwargs):
         configuration_settings = {}
         sentinel_keys = kwargs.pop("sentinel_keys", self._refresh_on)
         for select in self._selects:
             configurations = self._client.list_configuration_settings(
                 key_filter=select.key_filter, label_filter=select.label_filter, **kwargs
             )
-            for config in configurations:
-                key = self._process_key_name(config)
-                value = self._process_key_value(config)
+            async for config in configurations:
                 if isinstance(config, FeatureFlagConfigurationSetting):
-                    feature_management = configuration_settings.get(FEATURE_MANAGEMENT_KEY, {})
-                    feature_management[key] = value
-                    if FEATURE_MANAGEMENT_KEY not in configuration_settings:
-                        configuration_settings[FEATURE_MANAGEMENT_KEY] = feature_management
+                    # Feature flags are ignored when loaded by Selects, as they are selected from
+                    # `feature_flag_selectors`
+                    pass
                 else:
+                    key = self._process_key_name(config)
+                    value = await self._process_key_value(config)
                     configuration_settings[key] = value
                 # Every time we run load_all, we should update the etag of our refresh sentinels
                 # so they stay up-to-date.
                 # Sentinel keys will have unprocessed key names, so we need to use the original key.
                 if (config.key, config.label) in self._refresh_on:
                     sentinel_keys[(config.key, config.label)] = config.etag
-        self._refresh_on = sentinel_keys
-        with self._update_lock:
-            self._dict = configuration_settings
+        return configuration_settings, sentinel_keys
+
+    async def _load_feature_flags(self, **kwargs):
+        feature_flag_sentinel_keys = {}
+        loaded_feature_flags = []
+        # Needs to be removed unknown keyword argument for list_configuration_settings
+        kwargs.pop("sentinel_keys", None)
+        filters_used = {}
+        for select in self._feature_flag_selectors:
+            feature_flags = self._client.list_configuration_settings(
+                key_filter=FEATURE_FLAG_PREFIX + select.key_filter, label_filter=select.label_filter, **kwargs
+            )
+            async for feature_flag in feature_flags:
+                loaded_feature_flags.append(json.loads(feature_flag.value))
+
+                if self._feature_flag_refresh_enabled:
+                    feature_flag_sentinel_keys[(feature_flag.key, feature_flag.label)] = feature_flag.etag
+                if feature_flag.filters:
+                    for filter in feature_flag.filters:
+                        if filter.get("name") in PERCENTAGE_FILTER_NAMES:
+                            filters_used[PERCENTAGE_FILTER_KEY] = True
+                        elif filter.get("name") in TIME_WINDOW_FILTER_NAMES:
+                            filters_used[TIME_WINDOW_FILTER_KEY] = True
+                        elif filter.get("name") in TARGETING_FILTER_NAMES:
+                            filters_used[TARGETING_FILTER_KEY] = True
+                        else:
+                            filters_used[CUSTOM_FILTER_KEY] = True
+        self._feature_filter_usage = filters_used
+
+        return loaded_feature_flags, feature_flag_sentinel_keys
 
     def _process_key_name(self, config):
         trimmed_key = config.key
         # Trim the key if it starts with one of the prefixes provided
         for trim in self._trim_prefixes:
             if config.key.startswith(trim):
                 trimmed_key = config.key[len(trim) :]
                 break
-        if isinstance(config, FeatureFlagConfigurationSetting) and trimmed_key.startswith(FEATURE_FLAG_PREFIX):
-            return trimmed_key[len(FEATURE_FLAG_PREFIX) :]
         return trimmed_key
 
-    def _process_key_value(self, config):
+    async def _process_key_value(self, config):
         if isinstance(config, SecretReferenceConfigurationSetting):
-            return _resolve_keyvault_reference(config, self)
+            return await _resolve_keyvault_reference(config, self)
         if _is_json_content_type(config.content_type) and not isinstance(config, FeatureFlagConfigurationSetting):
             # Feature flags are of type json, but don't treat them as such
             try:
                 return json.loads(config.value)
             except json.JSONDecodeError:
                 # If the value is not a valid JSON, treat it like regular string value
                 return config.value
         return config.value
 
-    def __getitem__(self, key: str) -> str:
+    def __getitem__(self, key: str) -> Any:
         # pylint:disable=docstring-missing-param,docstring-missing-return,docstring-missing-rtype
         """
         Returns the value of the specified key.
         """
         return self._dict[key]
 
-    def __iter__(self) -> Iterable[str]:
+    def __iter__(self) -> Iterator[str]:
         return self._dict.__iter__()
 
     def __len__(self) -> int:
         return len(self._dict)
 
     def __contains__(self, __x: object) -> bool:
         # pylint:disable=docstring-missing-param,docstring-missing-return,docstring-missing-rtype
         """
         Returns True if the configuration settings contains the specified key.
         """
         return self._dict.__contains__(__x)
 
-    def keys(self) -> Iterable[str]:
+    def keys(self) -> KeysView[str]:
         """
         Returns a list of keys loaded from Azure App Configuration.
 
         :return: A list of keys loaded from Azure App Configuration.
-        :rtype: Iterable[str]
+        :rtype: KeysView[str]
         """
-        with self._update_lock:
-            return list(self._dict.keys())
+        return self._dict.keys()
 
-    def items(self) -> Iterable[Tuple[str, Union[str, JSON]]]:
+    def items(self) -> ItemsView[str, Union[str, Mapping[str, Any]]]:
         """
         Returns a set-like object of key-value pairs loaded from Azure App Configuration. Any values that are Key Vault
          references will be resolved.
 
         :return: A set-like object of key-value pairs loaded from Azure App Configuration.
-        :rtype: Iterable[Tuple[str, Union[str, JSON]]]
+        :rtype: ItemsView[str, Union[str, Mapping[str, Any]]]
         """
-        with self._update_lock:
-            return copy.deepcopy(self._dict.items())
+        return self._dict.items()
 
-    def values(self) -> Iterable[Union[str, JSON]]:
+    def values(self) -> ValuesView[Union[str, Mapping[str, Any]]]:
         """
         Returns a list of values loaded from Azure App Configuration. Any values that are Key Vault references will be
         resolved.
 
         :return: A list of values loaded from Azure App Configuration. The values are either Strings or JSON objects,
-        based on there content type.
-        :rtype: Iterable[[str], [JSON]]
+         based on there content type.
+        :rtype: ValuesView[Union[str, Mapping[str, Any]]]
         """
-        with self._update_lock:
-            return copy.deepcopy(list((self._dict.values())))
+        return self._dict.values()
+
+    @overload
+    def get(self, key: str, default: None = None) -> Union[str, JSON, None]: ...
 
-    def get(self, key: str, default: Optional[str] = None) -> Union[str, JSON]:
+    @overload
+    def get(self, key: str, default: Union[str, JSON, _T]) -> Union[str, JSON, _T]:  # pylint: disable=signature-differs
+        ...
+
+    def get(self, key: str, default: Optional[Union[str, JSON, _T]] = None) -> Union[str, JSON, _T, None]:
         """
         Returns the value of the specified key. If the key does not exist, returns the default value.
 
         :param str key: The key of the value to get.
         :param default: The default value to return.
         :type: str or None
         :return: The value of the specified key.
         :rtype: Union[str, JSON]
         """
-        with self._update_lock:
-            return copy.deepcopy(self._dict.get(key, default))
+        return self._dict.get(key, default)
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, AzureAppConfigurationProvider):
             return False
         if self._dict != other._dict:
             return False
         if self._trim_prefixes != other._trim_prefixes:
@@ -628,25 +663,25 @@
         if self._client != other._client:
             return False
         return True
 
     def __ne__(self, other: Any) -> bool:
         return not self == other
 
-    def close(self) -> None:
+    async def close(self) -> None:
         """
         Closes the connection to Azure App Configuration.
         """
         for client in self._secret_clients.values():
-            client.close()
-        self._client.close()
+            await client.close()
+        await self._client.close()  # type: ignore
 
-    def __enter__(self) -> "AzureAppConfigurationProvider":
-        self._client.__enter__()
+    async def __aenter__(self) -> "AzureAppConfigurationProvider":
+        await self._client.__aenter__()  # type: ignore
         for client in self._secret_clients.values():
-            client.__enter__()
+            await client.__aenter__()
         return self
 
-    def __exit__(self, *args) -> None:
-        self._client.__exit__(*args)
+    async def __aexit__(self, *args) -> None:
+        await self._client.__aexit__(*args)  # type: ignore
         for client in self._secret_clients.values():
-            client.__exit__()
+            await client.__aexit__()
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/azure/appconfiguration/provider/_models.py` & `azure-appconfiguration-provider-1.2.0/azure/appconfiguration/provider/_models.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-provider-1.1.0b3/azure_appconfiguration_provider.egg-info/PKG-INFO` & `azure-appconfiguration-provider-1.2.0/azure_appconfiguration_provider.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: azure-appconfiguration-provider
-Version: 1.1.0b3
+Version: 1.2.0
 Summary: Microsoft App Configuration Provider Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/appconfiguration/azure-appconfiguration-provider
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: msrest>=0.6.21
-Requires-Dist: azure-core<2.0.0,>=1.25.0
-Requires-Dist: azure-appconfiguration<2.0.0,>=1.4.0
-Requires-Dist: azure-keyvault-secrets<5.0.0,>=4.3.0
 
 # Azure App Configuration Python Provider client library for Python
 
 Azure App Configuration is a managed service that helps developers centralize their application configurations simply and securely. This provider adds additional functionality above the azure-sdk-for-python.
 
 Using the provider enables loading sets of configurations from an Azure App Configuration store in a managed way.
 
@@ -65,26 +61,26 @@
 
 ### Features
 
 Currently the Azure App Configuration Provider enables:
 
 * Connecting to an App Configuration Store using a connection string or Azure Active Directory.
 * Selecting multiple sets of configurations using `SettingSelector`.
+* Loading Feature Flags
 * Dynamic Refresh
 * Trim prefixes off key names.
 * Resolving Key Vault References, requires AAD.
 * Secret Resolver, resolve Key Vault References locally without connecting to Key Vault.
 * Json Content Type
 
 #### Future Features
 
 List of features we are going to add to the Python Provider in the future.
 
 * Geo-Replication support
-* Feature Management
 * Configuration Placeholders
 
 ## Examples
 
 ### Selecting configurations
 
 You can refine or expand the configurations loaded from your store by using `SettingSelector`s. Setting selectors provide a way to pass a key filter and label filter into the provider.
@@ -191,14 +187,44 @@
     return "From Secret Resolver"
 
 key_vault_options = AzureAppConfigurationKeyVaultOptions(
     secret_resolver=secret_resolver)
 config = load(endpoint=endpoint, credential=DefaultAzureCredential(), key_vault_options=key_vault_options)
 ```
 
+## Loading Feature Flags
+
+Feature Flags can be loaded from config stores using the provider. Feature flags are loaded as a dictionary of key/value pairs stored in the provider under the `feature_management`, then `feature_flags`.
+
+```python
+config = load(endpoint=endpoint, credential=DefaultAzureCredential(), feature_flags_enabled=True)
+alpha = config["feature_management"]["feature_flags"]["Alpha"]
+print(alpha["enabled"])
+```
+
+By default all feature flags with no label are loaded when `feature_flags_enabled` is set to `True`. . If you want to load feature flags with a specific label you can use `SettingSelector` to filter the feature flags.
+
+```python
+from azure.appconfiguration.provider import load, SettingSelector
+
+config = load(endpoint=endpoint, credential=DefaultAzureCredential(), feature_flags_enabled=True, feature_flag_selectors=[SettingSelector(key_filter="*", label_filter="dev")])
+alpha = config["feature_management"]["feature_flags"]["Alpha"]
+print(alpha["enabled"])
+```
+
+To enable refresh for feature flags you need to enable refresh. This will allow the provider to refresh feature flags the same way it refreshes configurations. Unlike configurations, all loaded feature flags are monitored for changes and will cause a refresh. Refresh of configuration settings and feature flags are independent of each other. Both are trigged by the `refresh` method, but a feature flag changing will not cause a refresh of configurations and vice versa. Also, if refresh for configuration settings is not enabled, feature flags can still be enabled for refresh.
+
+```python
+config = load(endpoint=endpoint, credential=DefaultAzureCredential(), feature_flags_enabled=True, feature_flag_refresh_enabled=True)
+
+...
+
+config.refresh()
+```
+
 ## Key concepts
 
 ## Troubleshooting
 
 ## Next steps
 
 Check out our Django and Flask examples to see how to use the provider in a web application.
@@ -226,14 +252,37 @@
 
 [azure_cli]: https://learn.microsoft.com/cli/azure/appconfig
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 
 
 # Release History
 
+## 1.2.0 (2024-05-24)
+
+### Features Added
+
+* Enable loading of feature flags with `feature_flag_enabled`
+* Select Feature Flags to load with `feature_flag_selectors`
+* Enable/Disable Feature Flag Refresh with `feature_flag_refresh_enabled`
+
+### Bugs Fixed
+
+* Fixes issue where loading configurations were slower due to returning a copy of the configurations.
+
+## 1.1.0 (2024-01-29)
+
+### Features Added
+
+* New API for Azure App Configuration Provider, `refresh`, which can be used to refresh the configuration from the Azure App Configuration service. `refresh` by default can check every 30 seconds for changes to specified sentinel keys. If a change is detected then all configurations are reloaded. Sentinel keys can be set by passing a list of `SentinelKey`'s to `refresh_on`.
+* Added new options `on_refresh_success` and `on_refresh_failure` callbacks to the load method. These callbacks are called when the refresh method successfully refreshes the configuration or fails to refresh the configuration.
+
+### Bugs Fixed
+
+* Verifies that the `refresh_interval` is at least 1 second.
+
 ## 1.1.0b3 (2023-12-19)
 
 ### Features Added
 
 - Added on_refresh_success callback to load method. This callback is called when the refresh method successfully refreshes the configuration.
 - Added minimum up time. This is the minimum amount of time the provider will try to be up before throwing an error. This is to prevent quick restart loops.
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/azure_appconfiguration_provider.egg-info/SOURCES.txt` & `azure-appconfiguration-provider-1.2.0/azure_appconfiguration_provider.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,20 +27,24 @@
 samples/async_connection_string_sample.py
 samples/async_key_vault_reference_provided_clients_sample.py
 samples/async_key_vault_reference_sample.py
 samples/connection_string_sample.py
 samples/key_vault_reference_customized_clients_sample.py
 samples/key_vault_reference_sample.py
 samples/refresh_sample.py
+samples/refresh_sample_feature_flags.py
 samples/sample_utilities.py
 tests/async_preparers.py
 tests/asynctestcase.py
 tests/conftest.py
 tests/preparers.py
 tests/test_async_provider.py
 tests/test_async_provider_aad.py
+tests/test_async_provider_feature_management.py
 tests/test_async_provider_refresh.py
+tests/test_constants.py
 tests/test_provider.py
 tests/test_provider_aad.py
 tests/test_provider_backoff.py
+tests/test_provider_feature_management.py
 tests/test_provider_refresh.py
 tests/testcase.py
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/samples/README.md` & `azure-appconfiguration-provider-1.2.0/samples/README.md`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-provider-1.1.0b3/samples/aad_sample.py` & `azure-appconfiguration-provider-1.2.0/samples/aad_sample.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 # Connecting to Azure App Configuration using AAD
 config = load(endpoint=endpoint, credential=credential, **kwargs)
 
 print(config["message"])
 
 # Connecting to Azure App Configuration using AAD and trim key prefixes
-trimmed = {"test."}
+trimmed = ["test."]
 config = load(endpoint=endpoint, credential=credential, trim_prefixes=trimmed, **kwargs)
 
 print(config["message"])
 
 # Connection to Azure App Configuration using SettingSelector
-selects = {SettingSelector(key_filter="message*")}
+selects = [SettingSelector(key_filter="message*")]
 config = load(endpoint=endpoint, credential=credential, selects=selects, **kwargs)
 
 print("message found: " + str("message" in config))
 print("test.message found: " + str("test.message" in config))
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/samples/async_aad_sample.py` & `azure-appconfiguration-provider-1.2.0/samples/async_aad_sample.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 from azure.appconfiguration.provider.aio import load
 from azure.appconfiguration.provider import SettingSelector
 import os
 from sample_utilities import get_authority, get_audience, get_credential, get_client_modifications
 
 
 async def main():
-    endpoint = os.environ.get("APPCONFIGURATION_ENDPOINT_STRING")
+    endpoint = os.environ["APPCONFIGURATION_ENDPOINT_STRING"]
     authority = get_authority(endpoint)
     credential = get_credential(authority, is_async=True)
     kwargs = get_client_modifications()
 
     # Connecting to Azure App Configuration using AAD
     config = await load(endpoint=endpoint, credential=credential, **kwargs)
     print(config["message"])
 
     # Connecting to Azure App Configuration using AAD and trim key prefixes
-    trimmed = {"test."}
+    trimmed = ["test."]
     config = await load(endpoint=endpoint, credential=credential, trim_prefixes=trimmed, **kwargs)
 
     print(config["message"])
 
     # Connection to Azure App Configuration using SettingSelector
-    selects = {SettingSelector(key_filter="message*")}
+    selects = [SettingSelector(key_filter="message*")]
     config = await load(endpoint=endpoint, credential=credential, selects=selects, **kwargs)
 
     print("message found: " + str("message" in config))
     print("test.message found: " + str("test.message" in config))
 
     await credential.close()
     await config.close()
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/samples/async_connection_string_sample.py` & `azure-appconfiguration-provider-1.2.0/samples/connection_string_sample.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 # ------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
-import asyncio
-from azure.appconfiguration.provider.aio import load
-from azure.appconfiguration.provider import SettingSelector
+
+from azure.appconfiguration.provider import load, SettingSelector
 from sample_utilities import get_client_modifications
 import os
 
+kwargs = get_client_modifications()
+connection_string = os.environ["APPCONFIGURATION_CONNECTION_STRING"]
 
-async def main():
-    kwargs = get_client_modifications()
-    connection_string = os.environ.get("APPCONFIGURATION_CONNECTION_STRING")
-
-    # Connecting to Azure App Configuration using connection string
-    config = await load(connection_string=connection_string, **kwargs)
-
-    print(config["message"])
-    print(config["my_json"]["key"])
-
-    # Connecting to Azure App Configuration using connection string and trimmed key prefixes
-    trimmed = {"test."}
-    config = await load(connection_string=connection_string, trim_prefixes=trimmed, **kwargs)
+# Connecting to Azure App Configuration using connection string
+config = load(connection_string=connection_string, **kwargs)
 
-    print(config["message"])
+print(config["message"])
+print(config["my_json"]["key"])
 
-    # Connection to Azure App Configuration using SettingSelector
-    selects = {SettingSelector(key_filter="message*")}
-    config = await load(connection_string=connection_string, selects=selects, **kwargs)
+# Connecting to Azure App Configuration using connection string and trimmed key prefixes
+trimmed = ["test."]
+config = load(connection_string=connection_string, trim_prefixes=trimmed, **kwargs)
 
-    print("message found: " + str("message" in config))
-    print("test.message found: " + str("test.message" in config))
+print(config["message"])
 
+# Connection to Azure App Configuration using SettingSelector
+selects = [SettingSelector(key_filter="message*")]
+config = load(connection_string=connection_string, selects=selects, **kwargs)
 
-if __name__ == "__main__":
-    asyncio.run(main())
+print("message found: " + str("message" in config))
+print("test.message found: " + str("test.message" in config))
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/samples/async_key_vault_reference_provided_clients_sample.py` & `azure-appconfiguration-provider-1.2.0/samples/key_vault_reference_sample.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,22 @@
 # ------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 
-import asyncio
-from azure.appconfiguration.provider.aio import load
-from azure.appconfiguration.provider import SettingSelector
+from azure.appconfiguration.provider import load, SettingSelector
 import os
-from sample_utilities import get_authority, get_credential, get_client_modifications
+from sample_utilities import get_authority, get_audience, get_credential, get_client_modifications
 
+endpoint = os.environ["APPCONFIGURATION_ENDPOINT_STRING"]
+authority = get_authority(endpoint)
+audience = get_audience(authority)
+credential = get_credential(authority)
+kwargs = get_client_modifications()
 
-async def main():
-    endpoint = os.environ.get("APPCONFIGURATION_ENDPOINT_STRING")
-    key_vault_uri = os.environ.get("KEYVAULT_URL")
-    authority = get_authority(endpoint)
-    credential = get_credential(authority, is_async=True)
-    kwargs = get_client_modifications()
+# Connection to Azure App Configuration using AAD and Resolving Key Vault References
+selects = [SettingSelector(key_filter="*", label_filter="prod")]
 
-    # Connection to Azure App Configuration using AAD with Provided Client
-    client_configs = {key_vault_uri: {"credential": credential}}
-    selects = {SettingSelector(key_filter="*", label_filter="prod")}
-    config = await load(
-        endpoint=endpoint, credential=credential, selects=selects, keyvault_client_configs=client_configs, **kwargs
-    )
+config = load(endpoint=endpoint, credential=credential, keyvault_credential=credential, selects=selects, **kwargs)
 
-    print(config["secret"])
-
-    await credential.close()
-    await config.close()
-
-
-if __name__ == "__main__":
-    asyncio.run(main())
+print(config["secret"])
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/samples/async_key_vault_reference_sample.py` & `azure-appconfiguration-provider-1.2.0/samples/async_key_vault_reference_sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from azure.appconfiguration.provider.aio import load
 from azure.appconfiguration.provider import SettingSelector
 import os
 from sample_utilities import get_authority, get_audience, get_credential, get_client_modifications
 
 
 async def main():
-    endpoint = os.environ.get("APPCONFIGURATION_ENDPOINT_STRING")
+    endpoint = os.environ["APPCONFIGURATION_ENDPOINT_STRING"]
     authority = get_authority(endpoint)
     credential = get_credential(authority, is_async=True)
     kwargs = get_client_modifications()
 
     # Connection to Azure App Configuration using AAD and Resolving Key Vault References
-    selects = {SettingSelector(key_filter="*", label_filter="prod")}
+    selects = [SettingSelector(key_filter="*", label_filter="prod")]
 
     config = await load(
         endpoint=endpoint, credential=credential, keyvault_credential=credential, selects=selects, **kwargs
     )
 
     print(config["secret"])
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/samples/key_vault_reference_customized_clients_sample.py` & `azure-appconfiguration-provider-1.2.0/samples/key_vault_reference_customized_clients_sample.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 # license information.
 # -------------------------------------------------------------------------
 
 from azure.appconfiguration.provider import load, SettingSelector
 import os
 from sample_utilities import get_authority, get_credential, get_client_modifications
 
-endpoint = os.environ.get("APPCONFIGURATION_ENDPOINT_STRING")
-key_vault_uri = os.environ.get("KEYVAULT_URL")
+endpoint = os.environ["APPCONFIGURATION_ENDPOINT_STRING"]
+key_vault_uri = os.environ["KEYVAULT_URL"]
 authority = get_authority(endpoint)
 credential = get_credential(authority)
 kwargs = get_client_modifications()
 
 # Connection to Azure App Configuration using AAD with Provided Client
 client_configs = {key_vault_uri: {"credential": credential}}
-selects = {SettingSelector(key_filter="*", label_filter="prod")}
+selects = [SettingSelector(key_filter="*", label_filter="prod")]
 config = load(
     endpoint=endpoint, credential=credential, keyvault_client_configs=client_configs, selects=selects, **kwargs
 )
 
 print(config["secret"])
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/samples/refresh_sample.py` & `azure-appconfiguration-provider-1.2.0/samples/refresh_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 from azure.appconfiguration.provider import load, WatchKey
-from azure.appconfiguration import (
+from azure.appconfiguration import (  # type:ignore
     AzureAppConfigurationClient,
     ConfigurationSetting,
 )
 from sample_utilities import get_client_modifications
 import os
 import time
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/samples/sample_utilities.py` & `azure-appconfiguration-provider-1.2.0/samples/sample_utilities.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,51 +11,54 @@
     - get_authority(): get authority of the ConfigurationClient
     - get_audience(): get audience of the ConfigurationClient
     - get_credential(): get credential of the ConfigurationClient
     It is not a file expected to run independently.
 """
 
 import os
-from azure.identity import AzureAuthorityHosts, ClientSecretCredential
+from azure.identity import AzureAuthorityHosts, ClientSecretCredential, InteractiveBrowserCredential
 from azure.identity.aio import ClientSecretCredential as AsyncClientSecretCredential
 
 
 def get_authority(endpoint):
     # cSpell:ignore azconfig
     if ".azconfig.io" in endpoint:
         return AzureAuthorityHosts.AZURE_PUBLIC_CLOUD
     if ".azconfig.azure.cn" in endpoint:
         return AzureAuthorityHosts.AZURE_CHINA
     if ".azconfig.azure.us" in endpoint:
         return AzureAuthorityHosts.AZURE_GOVERNMENT
+    if ".azconfig-test.io" in endpoint:
+        return "login.azure-test.net"
     raise ValueError(f"Endpoint ({endpoint}) could not be understood")
 
 
 def get_audience(authority):
     if authority == AzureAuthorityHosts.AZURE_PUBLIC_CLOUD:
         return "https://management.azure.com"
     if authority == AzureAuthorityHosts.AZURE_CHINA:
         return "https://management.chinacloudapi.cn"
     if authority == AzureAuthorityHosts.AZURE_GOVERNMENT:
         return "https://management.usgovcloudapi.net"
+    if authority == "login.azure-test.net":
+        return "https://management.azure-test.net"
 
 
 def get_credential(authority, **kwargs):
     if kwargs.pop("is_async", False):
         return AsyncClientSecretCredential(
-            tenant_id=os.environ.get("APPCONFIGURATION_TENANT_ID"),
-            client_id=os.environ.get("APPCONFIGURATION_CLIENT_ID"),
-            client_secret=os.environ.get("APPCONFIGURATION_CLIENT_SECRET"),
+            tenant_id=os.environ["APPCONFIGURATION_TENANT_ID"],
+            client_id=os.environ["APPCONFIGURATION_CLIENT_ID"],
+            client_secret=os.environ["APPCONFIGURATION_CLIENT_SECRET"],
             authority=authority,
+            validate_authority=False,
         )
-    return ClientSecretCredential(
-        tenant_id=os.environ.get("APPCONFIGURATION_TENANT_ID"),
-        client_id=os.environ.get("APPCONFIGURATION_CLIENT_ID"),
-        client_secret=os.environ.get("APPCONFIGURATION_CLIENT_SECRET"),
+    return InteractiveBrowserCredential(
         authority=authority,
+        validate_authority=False,
     )
 
 
 def get_client_modifications():
     modifications = {}
     modifications["user_agent"] = "SDK/Sample"
     return modifications
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/setup.py` & `azure-appconfiguration-provider-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,28 +53,27 @@
     long_description_content_type="text/markdown",
     license="MIT License",
     author="Microsoft Corporation",
     author_email="azpysdkhelp@microsoft.com",
     url="https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/appconfiguration/azure-appconfiguration-provider",
     keywords="azure, azure sdk",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
     zip_safe=False,
     packages=find_packages(exclude=exclude_packages),
     python_requires=">=3.6",
     install_requires=[
-        "msrest>=0.6.21",
-        "azure-core<2.0.0,>=1.25.0",
-        "azure-appconfiguration<2.0.0,>=1.4.0",
-        "azure-keyvault-secrets<5.0.0,>=4.3.0",
+        "azure-core>=1.28.0",
+        "azure-appconfiguration>=1.6.0",
+        "azure-keyvault-secrets>=4.3.0",
     ],
 )
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/tests/async_preparers.py` & `azure-appconfiguration-provider-1.2.0/tests/async_preparers.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-provider-1.1.0b3/tests/asynctestcase.py` & `azure-appconfiguration-provider-1.2.0/tests/asynctestcase.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 # coding: utf-8
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-import asyncio
 from devtools_testutils import AzureRecordedTestCase
 from azure.appconfiguration.aio import AzureAppConfigurationClient
-from azure.appconfiguration import ConfigurationSetting, FeatureFlagConfigurationSetting
 from testcase import get_configs
 from azure.appconfiguration.provider.aio import load
 from azure.appconfiguration.provider import SettingSelector, AzureAppConfigurationKeyVaultOptions
+from test_constants import FEATURE_MANAGEMENT_KEY, FEATURE_FLAG_KEY
 
 
 class AppConfigTestCase(AzureRecordedTestCase):
-    import asyncio
-
     async def create_aad_client(
         self,
         appconfiguration_endpoint_string,
         trim_prefixes=[],
         selects={SettingSelector(key_filter="*", label_filter="\0")},
         keyvault_secret_url=None,
         refresh_on=None,
         refresh_interval=30,
         secret_resolver=None,
         key_vault_options=None,
         on_refresh_success=None,
+        feature_flag_enabled=False,
+        feature_flag_refresh_enabled=False,
     ):
         cred = self.get_credential(AzureAppConfigurationClient, is_async=True)
 
         if not secret_resolver and keyvault_secret_url:
             keyvault_cred = cred
         else:
             keyvault_cred = None
@@ -46,66 +45,76 @@
                 trim_prefixes=trim_prefixes,
                 selects=selects,
                 refresh_on=refresh_on,
                 refresh_interval=refresh_interval,
                 user_agent="SDK/Integration",
                 keyvault_credential=keyvault_cred,
                 on_refresh_success=on_refresh_success,
+                feature_flag_enabled=feature_flag_enabled,
+                feature_flag_refresh_enabled=feature_flag_refresh_enabled,
             )
         if key_vault_options:
             if not key_vault_options.secret_resolver:
                 key_vault_options = AzureAppConfigurationKeyVaultOptions(credential=cred)
             return await load(
                 credential=cred,
                 endpoint=appconfiguration_endpoint_string,
                 trim_prefixes=trim_prefixes,
                 selects=selects,
                 refresh_on=refresh_on,
                 refresh_interval=refresh_interval,
                 user_agent="SDK/Integration",
                 key_vault_options=key_vault_options,
                 on_refresh_success=on_refresh_success,
+                feature_flag_enabled=feature_flag_enabled,
+                feature_flag_refresh_enabled=feature_flag_refresh_enabled,
             )
         return await load(
             credential=cred,
             endpoint=appconfiguration_endpoint_string,
             trim_prefixes=trim_prefixes,
             selects=selects,
             refresh_on=refresh_on,
             refresh_interval=refresh_interval,
             user_agent="SDK/Integration",
             secret_resolver=secret_resolver,
             on_refresh_success=on_refresh_success,
+            feature_flag_enabled=feature_flag_enabled,
+            feature_flag_refresh_enabled=feature_flag_refresh_enabled,
         )
 
     async def create_client(
         self,
         appconfiguration_connection_string,
         trim_prefixes=[],
         selects={SettingSelector(key_filter="*", label_filter="\0")},
         keyvault_secret_url=None,
         refresh_on=None,
         refresh_interval=30,
         secret_resolver=None,
         key_vault_options=None,
         on_refresh_success=None,
+        feature_flag_enabled=False,
+        feature_flag_refresh_enabled=False,
     ):
         client = AzureAppConfigurationClient.from_connection_string(appconfiguration_connection_string)
         await setup_configs(client, keyvault_secret_url)
 
         if not secret_resolver and keyvault_secret_url and not key_vault_options:
             return await load(
                 connection_string=appconfiguration_connection_string,
                 trim_prefixes=trim_prefixes,
                 selects=selects,
                 refresh_on=refresh_on,
                 refresh_interval=refresh_interval,
                 user_agent="SDK/Integration",
                 keyvault_credential=self.get_credential(AzureAppConfigurationClient, is_async=True),
                 on_refresh_success=on_refresh_success,
+                feature_flag_enabled=feature_flag_enabled,
+                feature_flag_refresh_enabled=feature_flag_refresh_enabled,
             )
         if key_vault_options:
             if not key_vault_options.secret_resolver:
                 key_vault_options = AzureAppConfigurationKeyVaultOptions(
                     credential=self.get_credential(AzureAppConfigurationClient, is_async=True)
                 )
             return await load(
@@ -113,24 +122,35 @@
                 trim_prefixes=trim_prefixes,
                 selects=selects,
                 refresh_on=refresh_on,
                 refresh_interval=refresh_interval,
                 user_agent="SDK/Integration",
                 key_vault_options=key_vault_options,
                 on_refresh_success=on_refresh_success,
+                feature_flag_enabled=feature_flag_enabled,
+                feature_flag_refresh_enabled=feature_flag_refresh_enabled,
             )
         return await load(
             connection_string=appconfiguration_connection_string,
             trim_prefixes=trim_prefixes,
             selects=selects,
             refresh_on=refresh_on,
             refresh_interval=refresh_interval,
             user_agent="SDK/Integration",
             secret_resolver=secret_resolver,
             on_refresh_success=on_refresh_success,
+            feature_flag_enabled=feature_flag_enabled,
+            feature_flag_refresh_enabled=feature_flag_refresh_enabled,
         )
 
 
 async def setup_configs(client, keyvault_secret_url):
     async with client:
         for config in get_configs(keyvault_secret_url):
             await client.set_configuration_setting(config)
+
+
+def has_feature_flag(client, feature_id, enabled=False):
+    for feature_flag in client[FEATURE_MANAGEMENT_KEY][FEATURE_FLAG_KEY]:
+        if feature_flag["id"] == feature_id:
+            return feature_flag["enabled"] == enabled
+    return False
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/tests/preparers.py` & `azure-appconfiguration-provider-1.2.0/tests/preparers.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 AppConfigProviderPreparer = functools.partial(
     EnvironmentVariableLoader,
     "appconfiguration",
     keyvault_secret_url="https://fake-keyvault.vault.azure.net/secrets/fake-secret/",
     appconfiguration_keyvault_secret_url="https://fake-keyvault.vault.azure.net/secrets/fake-secret/",
     appconfiguration_connection_string="Endpoint=https://fake-endpoint.azconfig.io;Id=0-l4-s0:h5htBaY5Z1LwFz50bIQv;Secret=lamefakesecretlamefakesecretlamefakesecrett=",
     appconfiguration_endpoint_string="https://fake-endpoint.azconfig.io",
-    appconfiguration_client_id="fake-client-id",
-    appconfiguration_client_secret="fake-client-secret",
-    appconfiguration_tenant_id="fake-tenant-id",
 )
 
 
 def app_config_decorator(func, **kwargs):
     @AppConfigProviderPreparer()
     def wrapper(*args, **kwargs):
         appconfiguration_connection_string = kwargs.pop("appconfiguration_connection_string")
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/tests/test_async_provider.py` & `azure-appconfiguration-provider-1.2.0/tests/test_async_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-from azure.appconfiguration.provider.aio import load
 from azure.appconfiguration.provider import SettingSelector, AzureAppConfigurationKeyVaultOptions
 from devtools_testutils.aio import recorded_by_proxy_async
 from async_preparers import app_config_decorator_async
-from asynctestcase import AppConfigTestCase
+from asynctestcase import AppConfigTestCase, has_feature_flag
+from test_constants import FEATURE_MANAGEMENT_KEY
 
 
 class TestAppConfigurationProvider(AppConfigTestCase):
     # method: provider_creation
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_provider_creation(self, appconfiguration_connection_string, appconfiguration_keyvault_secret_url):
         async with await self.create_client(
-            appconfiguration_connection_string, keyvault_secret_url=appconfiguration_keyvault_secret_url
+            appconfiguration_connection_string,
+            keyvault_secret_url=appconfiguration_keyvault_secret_url,
+            feature_flag_enabled=True,
         ) as client:
             assert client["message"] == "hi"
             assert client["my_json"]["key"] == "value"
-            assert "FeatureManagementFeatureFlags" in client
-            assert "Alpha" in client["FeatureManagementFeatureFlags"]
+            assert FEATURE_MANAGEMENT_KEY in client
+            assert has_feature_flag(client, "Alpha")
 
     # method: provider_trim_prefixes
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_provider_trim_prefixes(
         self, appconfiguration_connection_string, appconfiguration_keyvault_secret_url
     ):
         trimmed = {"test."}
         async with await self.create_client(
             appconfiguration_connection_string,
             trim_prefixes=trimmed,
             keyvault_secret_url=appconfiguration_keyvault_secret_url,
+            feature_flag_enabled=True,
         ) as client:
             assert client["message"] == "hi"
             assert client["my_json"]["key"] == "value"
             assert client["trimmed"] == "key"
             assert "test.trimmed" not in client
-            assert "FeatureManagementFeatureFlags" in client
-            assert "Alpha" in client["FeatureManagementFeatureFlags"]
+            assert FEATURE_MANAGEMENT_KEY in client
+            assert has_feature_flag(client, "Alpha")
 
     # method: provider_selectors
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_provider_selectors(self, appconfiguration_connection_string, appconfiguration_keyvault_secret_url):
         selects = {SettingSelector(key_filter="message*", label_filter="dev")}
         async with await self.create_client(
             appconfiguration_connection_string,
             selects=selects,
             keyvault_secret_url=appconfiguration_keyvault_secret_url,
         ) as client:
             assert client["message"] == "test"
             assert "test.trimmed" not in client
-            assert "FeatureManagementFeatureFlags" not in client
+            assert FEATURE_MANAGEMENT_KEY not in client
 
     # method: provider_selectors
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_provider_key_vault_reference(
         self, appconfiguration_connection_string, appconfiguration_keyvault_secret_url
     ):
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/tests/test_async_provider_aad.py` & `azure-appconfiguration-provider-1.2.0/tests/test_async_provider_aad.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-from azure.appconfiguration.provider.aio import load
 from azure.appconfiguration.provider import SettingSelector, AzureAppConfigurationKeyVaultOptions
 from devtools_testutils.aio import recorded_by_proxy_async
-from azure.appconfiguration.aio import AzureAppConfigurationClient
 from async_preparers import app_config_decorator_async
-from asynctestcase import AppConfigTestCase
+from asynctestcase import AppConfigTestCase, has_feature_flag
+from test_constants import FEATURE_MANAGEMENT_KEY
 
 
 class TestAppConfigurationProvider(AppConfigTestCase):
     # method: provider_creation_aad
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_provider_creation_aad(self, appconfiguration_endpoint_string, appconfiguration_keyvault_secret_url):
         async with await self.create_aad_client(
-            appconfiguration_endpoint_string, keyvault_secret_url=appconfiguration_keyvault_secret_url
+            appconfiguration_endpoint_string,
+            keyvault_secret_url=appconfiguration_keyvault_secret_url,
+            feature_flag_enabled=True,
         ) as client:
             assert client.get("message") == "hi"
             assert client["my_json"]["key"] == "value"
-            assert "FeatureManagementFeatureFlags" in client
-            assert "Alpha" in client["FeatureManagementFeatureFlags"]
+            assert FEATURE_MANAGEMENT_KEY in client
+            assert has_feature_flag(client, "Alpha")
 
     # method: provider_trim_prefixes
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_provider_trim_prefixes(self, appconfiguration_endpoint_string, appconfiguration_keyvault_secret_url):
         trimmed = {"test."}
         async with await self.create_aad_client(
             appconfiguration_endpoint_string,
             trim_prefixes=trimmed,
             keyvault_secret_url=appconfiguration_keyvault_secret_url,
+            feature_flag_enabled=True,
         ) as client:
             assert client["message"] == "hi"
             assert client["my_json"]["key"] == "value"
             assert client["trimmed"] == "key"
-            assert "FeatureManagementFeatureFlags" in client
-            assert "Alpha" in client["FeatureManagementFeatureFlags"]
+            assert FEATURE_MANAGEMENT_KEY in client
+            assert has_feature_flag(client, "Alpha")
 
     # method: provider_selectors
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_provider_selectors(self, appconfiguration_endpoint_string, appconfiguration_keyvault_secret_url):
         selects = {SettingSelector(key_filter="message*", label_filter="dev")}
         async with await self.create_aad_client(
-            appconfiguration_endpoint_string, selects=selects, keyvault_secret_url=appconfiguration_keyvault_secret_url
+            appconfiguration_endpoint_string,
+            selects=selects,
+            keyvault_secret_url=appconfiguration_keyvault_secret_url,
         ) as client:
             assert client["message"] == "test"
             assert "test.trimmed" not in client
-            assert "FeatureManagementFeatureFlags" not in client
+            assert FEATURE_MANAGEMENT_KEY not in client
 
     # method: provider_selectors
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_provider_key_vault_reference(
         self, appconfiguration_endpoint_string, appconfiguration_keyvault_secret_url
     ):
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/tests/test_async_provider_refresh.py` & `azure-appconfiguration-provider-1.2.0/tests/test_async_provider_refresh.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import unittest
 import pytest
 import sys
 
 from azure.appconfiguration.provider import WatchKey
 from devtools_testutils.aio import recorded_by_proxy_async
 from async_preparers import app_config_decorator_async
-from asynctestcase import AppConfigTestCase
-
+from asynctestcase import AppConfigTestCase, has_feature_flag
+from test_constants import FEATURE_MANAGEMENT_KEY
 
 try:
     # Python 3.7 does not support AsyncMock
     from unittest.mock import AsyncMock
 
     class TestAppConfigurationProvider(AppConfigTestCase, unittest.TestCase):
         # method: refresh
@@ -28,46 +28,58 @@
             mock_callback = AsyncMock()
             async with await self.create_aad_client(
                 appconfiguration_endpoint_string,
                 keyvault_secret_url=appconfiguration_keyvault_secret_url,
                 refresh_on=[WatchKey("refresh_message")],
                 refresh_interval=1,
                 on_refresh_success=mock_callback,
+                feature_flag_enabled=True,
+                feature_flag_refresh_enabled=True,
             ) as client:
                 assert client["refresh_message"] == "original value"
                 assert client["my_json"]["key"] == "value"
-                assert "FeatureManagementFeatureFlags" in client
-                assert "Alpha" in client["FeatureManagementFeatureFlags"]
+                assert FEATURE_MANAGEMENT_KEY in client
+                assert has_feature_flag(client, "Alpha")
                 setting = await client._client.get_configuration_setting(key="refresh_message")
                 setting.value = "updated value"
+                feature_flag = await client._client.get_configuration_setting(key=".appconfig.featureflag/Alpha")
+                feature_flag.enabled = True
                 await client._client.set_configuration_setting(setting)
+                await client._client.set_configuration_setting(feature_flag)
 
                 # Waiting for the refresh interval to pass
                 time.sleep(2)
 
                 await client.refresh()
                 assert client["refresh_message"] == "updated value"
+                assert has_feature_flag(client, "Alpha", True)
                 assert mock_callback.call_count == 1
 
                 setting.value = "original value"
+                feature_flag.enabled = False
                 await client._client.set_configuration_setting(setting)
+                await client._client.set_configuration_setting(feature_flag)
 
                 # Waiting for the refresh interval to pass
                 time.sleep(2)
 
                 await client.refresh()
                 assert client["refresh_message"] == "original value"
+                assert has_feature_flag(client, "Alpha", False)
                 assert mock_callback.call_count == 2
 
                 setting.value = "updated value 2"
+                feature_flag.enabled = True
                 await client._client.set_configuration_setting(setting)
+                await client._client.set_configuration_setting(feature_flag)
 
                 # Not waiting for the refresh interval to pass
                 await client.refresh()
                 assert client["refresh_message"] == "original value"
+                assert has_feature_flag(client, "Alpha", False)
                 assert mock_callback.call_count == 2
 
                 setting.value = "original value"
                 await client._client.set_configuration_setting(setting)
 
                 await client.refresh()
                 assert client["refresh_message"] == "original value"
@@ -80,20 +92,21 @@
         @pytest.mark.asyncio
         async def test_empty_refresh(self, appconfiguration_endpoint_string, appconfiguration_keyvault_secret_url):
             mock_callback = AsyncMock()
             async with await self.create_aad_client(
                 appconfiguration_endpoint_string,
                 keyvault_secret_url=appconfiguration_keyvault_secret_url,
                 on_refresh_success=mock_callback,
+                feature_flag_enabled=True,
             ) as client:
                 assert client["refresh_message"] == "original value"
                 assert client["non_refreshed_message"] == "Static"
                 assert client["my_json"]["key"] == "value"
-                assert "FeatureManagementFeatureFlags" in client
-                assert "Alpha" in client["FeatureManagementFeatureFlags"]
+                assert FEATURE_MANAGEMENT_KEY in client
+                assert has_feature_flag(client, "Alpha")
                 setting = await client._client.get_configuration_setting(key="refresh_message")
                 setting.value = "updated value"
                 await client._client.set_configuration_setting(setting)
                 static_setting = await client._client.get_configuration_setting(key="non_refreshed_message")
                 static_setting.value = "updated static"
                 await client._client.set_configuration_setting(static_setting)
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/tests/test_provider.py` & `azure-appconfiguration-provider-1.2.0/tests/test_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,68 +2,72 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 from azure.appconfiguration.provider import SettingSelector, AzureAppConfigurationKeyVaultOptions
 from devtools_testutils import recorded_by_proxy
 from preparers import app_config_decorator
-from testcase import AppConfigTestCase
+from testcase import AppConfigTestCase, has_feature_flag
 import datetime
 from unittest.mock import patch
+from test_constants import FEATURE_MANAGEMENT_KEY
 
 from azure.appconfiguration.provider._azureappconfigurationprovider import _delay_failure
 
 
 def sleep(seconds):
     assert isinstance(seconds, float)
 
 
 class TestAppConfigurationProvider(AppConfigTestCase):
     # method: provider_creation
     @recorded_by_proxy
     @app_config_decorator
     def test_provider_creation(self, appconfiguration_connection_string, appconfiguration_keyvault_secret_url):
         client = self.create_client(
-            appconfiguration_connection_string, keyvault_secret_url=appconfiguration_keyvault_secret_url
+            appconfiguration_connection_string,
+            keyvault_secret_url=appconfiguration_keyvault_secret_url,
+            feature_flag_enabled=True,
         )
         assert client["message"] == "hi"
         assert client["my_json"]["key"] == "value"
-        assert "FeatureManagementFeatureFlags" in client
-        assert "Alpha" in client["FeatureManagementFeatureFlags"]
+        assert FEATURE_MANAGEMENT_KEY in client
+        assert has_feature_flag(client, "Alpha")
 
     # method: provider_trim_prefixes
     @recorded_by_proxy
     @app_config_decorator
     def test_provider_trim_prefixes(self, appconfiguration_connection_string, appconfiguration_keyvault_secret_url):
         trimmed = {"test."}
         client = self.create_client(
             appconfiguration_connection_string,
             trim_prefixes=trimmed,
             keyvault_secret_url=appconfiguration_keyvault_secret_url,
+            feature_flag_enabled=True,
         )
         assert client["message"] == "hi"
         assert client["my_json"]["key"] == "value"
         assert client["trimmed"] == "key"
         assert "test.trimmed" not in client
-        assert "FeatureManagementFeatureFlags" in client
-        assert "Alpha" in client["FeatureManagementFeatureFlags"]
+        assert FEATURE_MANAGEMENT_KEY in client
+        assert has_feature_flag(client, "Alpha")
 
     # method: provider_selectors
     @recorded_by_proxy
     @app_config_decorator
     def test_provider_selectors(self, appconfiguration_connection_string, appconfiguration_keyvault_secret_url):
         selects = {SettingSelector(key_filter="message*", label_filter="dev")}
         client = self.create_client(
             appconfiguration_connection_string,
             selects=selects,
             keyvault_secret_url=appconfiguration_keyvault_secret_url,
         )
         assert client["message"] == "test"
         assert "test.trimmed" not in client
-        assert "FeatureManagementFeatureFlags" not in client
+        assert FEATURE_MANAGEMENT_KEY not in client
 
     # method: provider_selectors
     @recorded_by_proxy
     @app_config_decorator
     def test_provider_key_vault_reference(
         self, appconfiguration_connection_string, appconfiguration_keyvault_secret_url
     ):
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/tests/test_provider_aad.py` & `azure-appconfiguration-provider-1.2.0/tests/test_provider_aad.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,58 +2,62 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 from azure.appconfiguration.provider import SettingSelector, AzureAppConfigurationKeyVaultOptions
 from devtools_testutils import recorded_by_proxy
 from preparers import app_config_decorator_aad
-from testcase import AppConfigTestCase
+from testcase import AppConfigTestCase, has_feature_flag
+from test_constants import FEATURE_MANAGEMENT_KEY
 
 
 class TestAppConfigurationProvider(AppConfigTestCase):
     # method: provider_creation_aad
     @recorded_by_proxy
     @app_config_decorator_aad
     def test_provider_creation_aad(self, appconfiguration_endpoint_string, appconfiguration_keyvault_secret_url):
         client = self.create_aad_client(
-            appconfiguration_endpoint_string, keyvault_secret_url=appconfiguration_keyvault_secret_url
+            appconfiguration_endpoint_string,
+            keyvault_secret_url=appconfiguration_keyvault_secret_url,
+            feature_flag_enabled=True,
         )
         assert client["message"] == "hi"
         assert client["my_json"]["key"] == "value"
-        assert "FeatureManagementFeatureFlags" in client
-        assert "Alpha" in client["FeatureManagementFeatureFlags"]
+        assert FEATURE_MANAGEMENT_KEY in client
+        assert has_feature_flag(client, "Alpha")
 
     # method: provider_trim_prefixes
     @recorded_by_proxy
     @app_config_decorator_aad
     def test_provider_trim_prefixes(self, appconfiguration_endpoint_string, appconfiguration_keyvault_secret_url):
         trimmed = {"test."}
         client = self.create_aad_client(
             appconfiguration_endpoint_string,
             trim_prefixes=trimmed,
             keyvault_secret_url=appconfiguration_keyvault_secret_url,
+            feature_flag_enabled=True,
         )
         assert client["message"] == "hi"
         assert client["my_json"]["key"] == "value"
         assert client["trimmed"] == "key"
         assert "test.trimmed" not in client
-        assert "FeatureManagementFeatureFlags" in client
-        assert "Alpha" in client["FeatureManagementFeatureFlags"]
+        assert FEATURE_MANAGEMENT_KEY in client
+        assert has_feature_flag(client, "Alpha")
 
     # method: provider_selectors
     @recorded_by_proxy
     @app_config_decorator_aad
     def test_provider_selectors(self, appconfiguration_endpoint_string, appconfiguration_keyvault_secret_url):
         selects = {SettingSelector(key_filter="message*", label_filter="dev")}
         client = self.create_aad_client(
             appconfiguration_endpoint_string, selects=selects, keyvault_secret_url=appconfiguration_keyvault_secret_url
         )
         assert client["message"] == "test"
         assert "test.trimmed" not in client
-        assert "FeatureManagementFeatureFlags" not in client
+        assert FEATURE_MANAGEMENT_KEY not in client
 
     # method: provider_selectors
     @recorded_by_proxy
     @app_config_decorator_aad
     def test_provider_key_vault_reference(self, appconfiguration_endpoint_string, appconfiguration_keyvault_secret_url):
         selects = {SettingSelector(key_filter="*", label_filter="prod")}
         client = self.create_aad_client(
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/tests/test_provider_backoff.py` & `azure-appconfiguration-provider-1.2.0/tests/test_provider_backoff.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-provider-1.1.0b3/tests/test_provider_refresh.py` & `azure-appconfiguration-provider-1.2.0/tests/test_provider_refresh.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,80 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 import time
 import unittest
+import pytest
 from unittest.mock import Mock
 from azure.appconfiguration.provider import WatchKey
 from devtools_testutils import recorded_by_proxy
 from preparers import app_config_decorator_aad
-from testcase import AppConfigTestCase
+from testcase import AppConfigTestCase, has_feature_flag
+from test_constants import FEATURE_MANAGEMENT_KEY
 
 
 class TestAppConfigurationProvider(AppConfigTestCase, unittest.TestCase):
     # method: refresh
     @recorded_by_proxy
     @app_config_decorator_aad
     def test_refresh(self, appconfiguration_endpoint_string, appconfiguration_keyvault_secret_url):
         mock_callback = Mock()
         client = self.create_aad_client(
             appconfiguration_endpoint_string,
             keyvault_secret_url=appconfiguration_keyvault_secret_url,
             refresh_on=[WatchKey("refresh_message")],
             refresh_interval=1,
             on_refresh_success=mock_callback,
+            feature_flag_enabled=True,
+            feature_flag_refresh_enabled=True,
         )
         assert client["refresh_message"] == "original value"
         assert client["my_json"]["key"] == "value"
-        assert "FeatureManagementFeatureFlags" in client
-        assert "Alpha" in client["FeatureManagementFeatureFlags"]
+        assert FEATURE_MANAGEMENT_KEY in client
+        assert has_feature_flag(client, "Alpha")
 
         setting = client._client.get_configuration_setting(key="refresh_message")
         setting.value = "updated value"
+        feature_flag = client._client.get_configuration_setting(key=".appconfig.featureflag/Alpha")
+        feature_flag.enabled = True
         client._client.set_configuration_setting(setting)
+        client._client.set_configuration_setting(feature_flag)
 
         # Waiting for the refresh interval to pass
         time.sleep(2)
 
         client.refresh()
         assert client["refresh_message"] == "updated value"
+        assert has_feature_flag(client, "Alpha", True)
         assert mock_callback.call_count == 1
 
         setting.value = "original value"
+        feature_flag.enabled = False
         client._client.set_configuration_setting(setting)
+        client._client.set_configuration_setting(feature_flag)
 
         # Waiting for the refresh interval to pass
         time.sleep(2)
 
         client.refresh()
         assert client["refresh_message"] == "original value"
+        assert has_feature_flag(client, "Alpha", False)
         assert mock_callback.call_count == 2
 
         setting.value = "updated value 2"
+        feature_flag.enabled = True
         client._client.set_configuration_setting(setting)
+        client._client.set_configuration_setting(feature_flag)
 
         # Not waiting for the refresh interval to pass
         client.refresh()
         assert client["refresh_message"] == "original value"
+        assert has_feature_flag(client, "Alpha", False)
         assert mock_callback.call_count == 2
 
         setting.value = "original value"
         client._client.set_configuration_setting(setting)
 
         client.refresh()
         assert client["refresh_message"] == "original value"
@@ -71,20 +85,21 @@
     @app_config_decorator_aad
     def test_empty_refresh(self, appconfiguration_endpoint_string, appconfiguration_keyvault_secret_url):
         mock_callback = Mock()
         client = self.create_aad_client(
             appconfiguration_endpoint_string,
             keyvault_secret_url=appconfiguration_keyvault_secret_url,
             on_refresh_success=mock_callback,
+            feature_flag_enabled=True,
         )
         assert client["refresh_message"] == "original value"
         assert client["non_refreshed_message"] == "Static"
         assert client["my_json"]["key"] == "value"
-        assert "FeatureManagementFeatureFlags" in client
-        assert "Alpha" in client["FeatureManagementFeatureFlags"]
+        assert FEATURE_MANAGEMENT_KEY in client
+        assert has_feature_flag(client, "Alpha")
 
         setting = client._client.get_configuration_setting(key="refresh_message")
         setting.value = "updated value"
         client._client.set_configuration_setting(setting)
         static_setting = client._client.get_configuration_setting(key="non_refreshed_message")
         static_setting.value = "updated static"
         client._client.set_configuration_setting(static_setting)
```

### Comparing `azure-appconfiguration-provider-1.1.0b3/tests/testcase.py` & `azure-appconfiguration-provider-1.2.0/tests/testcase.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 from devtools_testutils import AzureRecordedTestCase
 from azure.appconfiguration import AzureAppConfigurationClient, ConfigurationSetting, FeatureFlagConfigurationSetting
 from azure.appconfiguration.provider import SettingSelector, load, AzureAppConfigurationKeyVaultOptions
-import os
+from test_constants import FEATURE_MANAGEMENT_KEY, FEATURE_FLAG_KEY
 
 
 class AppConfigTestCase(AzureRecordedTestCase):
     def create_aad_client(
         self,
         appconfiguration_endpoint_string,
         trim_prefixes=[],
         selects={SettingSelector(key_filter="*", label_filter="\0")},
         keyvault_secret_url=None,
         refresh_on=None,
         refresh_interval=30,
         secret_resolver=None,
         key_vault_options=None,
         on_refresh_success=None,
+        feature_flag_enabled=False,
+        feature_flag_refresh_enabled=False,
     ):
         cred = self.get_credential(AzureAppConfigurationClient)
         client = AzureAppConfigurationClient(appconfiguration_endpoint_string, cred)
         setup_configs(client, keyvault_secret_url)
 
         if not secret_resolver and keyvault_secret_url and not key_vault_options:
             keyvault_cred = cred
@@ -35,66 +37,76 @@
                 trim_prefixes=trim_prefixes,
                 selects=selects,
                 refresh_on=refresh_on,
                 refresh_interval=refresh_interval,
                 user_agent="SDK/Integration",
                 keyvault_credential=keyvault_cred,
                 on_refresh_success=on_refresh_success,
+                feature_flag_enabled=feature_flag_enabled,
+                feature_flag_refresh_enabled=feature_flag_refresh_enabled,
             )
         if key_vault_options:
             if not key_vault_options.secret_resolver:
                 key_vault_options = AzureAppConfigurationKeyVaultOptions(credential=cred)
             return load(
                 credential=cred,
                 endpoint=appconfiguration_endpoint_string,
                 trim_prefixes=trim_prefixes,
                 selects=selects,
                 refresh_on=refresh_on,
                 refresh_interval=refresh_interval,
                 user_agent="SDK/Integration",
                 key_vault_options=key_vault_options,
                 on_refresh_success=on_refresh_success,
+                feature_flag_enabled=feature_flag_enabled,
+                feature_flag_refresh_enabled=feature_flag_refresh_enabled,
             )
         return load(
             credential=cred,
             endpoint=appconfiguration_endpoint_string,
             trim_prefixes=trim_prefixes,
             selects=selects,
             refresh_on=refresh_on,
             refresh_interval=refresh_interval,
             user_agent="SDK/Integration",
             secret_resolver=secret_resolver,
             on_refresh_success=on_refresh_success,
+            feature_flag_enabled=feature_flag_enabled,
+            feature_flag_refresh_enabled=feature_flag_refresh_enabled,
         )
 
     def create_client(
         self,
         appconfiguration_connection_string,
         trim_prefixes=[],
         selects={SettingSelector(key_filter="*", label_filter="\0")},
         keyvault_secret_url=None,
         refresh_on=None,
         refresh_interval=30,
         secret_resolver=None,
         key_vault_options=None,
         on_refresh_success=None,
+        feature_flag_enabled=False,
+        feature_flag_refresh_enabled=False,
     ):
         client = AzureAppConfigurationClient.from_connection_string(appconfiguration_connection_string)
         setup_configs(client, keyvault_secret_url)
 
         if not secret_resolver and keyvault_secret_url and not key_vault_options:
             return load(
                 connection_string=appconfiguration_connection_string,
                 trim_prefixes=trim_prefixes,
                 selects=selects,
                 refresh_on=refresh_on,
                 refresh_interval=refresh_interval,
                 user_agent="SDK/Integration",
                 keyvault_credential=self.get_credential(AzureAppConfigurationClient),
                 on_refresh_success=on_refresh_success,
+                feature_flag_enabled=feature_flag_enabled,
+                feature_flag_refresh_enabled=feature_flag_refresh_enabled,
             )
         if key_vault_options:
             if not key_vault_options.secret_resolver:
                 key_vault_options = AzureAppConfigurationKeyVaultOptions(
                     credential=self.get_credential(AzureAppConfigurationClient)
                 )
             return load(
@@ -102,24 +114,28 @@
                 trim_prefixes=trim_prefixes,
                 selects=selects,
                 refresh_on=refresh_on,
                 refresh_interval=refresh_interval,
                 user_agent="SDK/Integration",
                 key_vault_options=key_vault_options,
                 on_refresh_success=on_refresh_success,
+                feature_flag_enabled=feature_flag_enabled,
+                feature_flag_refresh_enabled=feature_flag_refresh_enabled,
             )
         return load(
             connection_string=appconfiguration_connection_string,
             trim_prefixes=trim_prefixes,
             selects=selects,
             refresh_on=refresh_on,
             refresh_interval=refresh_interval,
             user_agent="SDK/Integration",
             secret_resolver=secret_resolver,
             on_refresh_success=on_refresh_success,
+            feature_flag_enabled=feature_flag_enabled,
+            feature_flag_refresh_enabled=feature_flag_refresh_enabled,
         )
 
 
 def setup_configs(client, keyvault_secret_url):
     for config in get_configs(keyvault_secret_url):
         client.set_configuration_setting(config)
 
@@ -163,7 +179,14 @@
 
 def create_feature_flag_config_setting(key, label, enabled):
     return FeatureFlagConfigurationSetting(
         feature_id=key,
         label=label,
         enabled=enabled,
     )
+
+
+def has_feature_flag(client, feature_id, enabled=False):
+    for feature_flag in client[FEATURE_MANAGEMENT_KEY][FEATURE_FLAG_KEY]:
+        if feature_flag["id"] == feature_id:
+            return feature_flag["enabled"] == enabled
+    return False
```

