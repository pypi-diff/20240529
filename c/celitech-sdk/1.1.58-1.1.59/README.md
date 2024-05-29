# Comparing `tmp/celitech_sdk-1.1.58.tar.gz` & `tmp/celitech_sdk-1.1.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celitech_sdk-1.1.58.tar", last modified: Fri May 17 11:29:05 2024, max compression
+gzip compressed data, was "celitech_sdk-1.1.59.tar", last modified: Wed May 29 10:59:22 2024, max compression
```

## Comparing `celitech_sdk-1.1.58.tar` & `celitech_sdk-1.1.59.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.423221 celitech_sdk-1.1.58/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.427221 celitech_sdk-1.1.58/src/celitech/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.427221 celitech_sdk-1.1.58/src/celitech/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/models/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/create_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/create_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/edit_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/edit_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/get_esim_device_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/get_esim_history_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/get_esim_mac_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/get_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/get_purchase_consumption_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/list_destinations_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/list_packages_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/list_purchases_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/top_up_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/top_up_esim_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/utils/cast_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/utils/json_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/net/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/environment/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/net/headers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/headers/base_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/net/request_chain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/hook_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/http_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/request_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/src/celitech/net/transport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/transport/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/transport/request_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/transport/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/transport/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/transport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/src/celitech/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/e_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/purchases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/src/celitech/services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/utils/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/utils/default_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/src/celitech_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-05-17 11:29:05.000000 celitech_sdk-1.1.58/src/celitech_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-17 11:29:05.000000 celitech_sdk-1.1.58/src/celitech_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 11:29:05.000000 celitech_sdk-1.1.58/src/celitech_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:29:05.000000 celitech_sdk-1.1.58/src/celitech_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 11:29:05.000000 celitech_sdk-1.1.58/src/celitech_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.574464 celitech_sdk-1.1.59/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-05-29 10:59:22.570464 celitech_sdk-1.1.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17345 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:59:22.574464 celitech_sdk-1.1.59/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.558464 celitech_sdk-1.1.59/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.562464 celitech_sdk-1.1.59/src/celitech/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.562464 celitech_sdk-1.1.59/src/celitech/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.566464 celitech_sdk-1.1.59/src/celitech/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/create_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/create_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/edit_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/edit_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/get_esim_device_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/get_esim_history_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/get_esim_mac_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/get_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/get_purchase_consumption_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/list_destinations_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/list_packages_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/list_purchases_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/top_up_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/top_up_esim_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.566464 celitech_sdk-1.1.59/src/celitech/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/utils/cast_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/models/utils/json_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.566464 celitech_sdk-1.1.59/src/celitech/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.566464 celitech_sdk-1.1.59/src/celitech/net/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/environment/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.566464 celitech_sdk-1.1.59/src/celitech/net/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/headers/base_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.566464 celitech_sdk-1.1.59/src/celitech/net/request_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/request_chain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.566464 celitech_sdk-1.1.59/src/celitech/net/request_chain/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/request_chain/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/request_chain/handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/request_chain/handlers/hook_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/request_chain/handlers/http_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/request_chain/handlers/retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/request_chain/request_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.570464 celitech_sdk-1.1.59/src/celitech/net/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/transport/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/transport/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/transport/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/transport/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/net/transport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.570464 celitech_sdk-1.1.59/src/celitech/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/services/destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/services/e_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/services/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/services/purchases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.570464 celitech_sdk-1.1.59/src/celitech/services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/services/utils/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/services/utils/default_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-29 10:59:09.000000 celitech_sdk-1.1.59/src/celitech/services/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:59:22.570464 celitech_sdk-1.1.59/src/celitech_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-05-29 10:59:22.000000 celitech_sdk-1.1.59/src/celitech_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-29 10:59:22.000000 celitech_sdk-1.1.59/src/celitech_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:59:22.000000 celitech_sdk-1.1.59/src/celitech_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 10:59:22.000000 celitech_sdk-1.1.59/src/celitech_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 10:59:22.000000 celitech_sdk-1.1.59/src/celitech_sdk.egg-info/top_level.txt
```

### Comparing `celitech_sdk-1.1.58/LICENSE` & `celitech_sdk-1.1.59/LICENSE`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/PKG-INFO` & `celitech_sdk-1.1.59/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-Metadata-Version: 2.1
-Name: celitech-sdk
-Version: 1.1.58
-Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-
-# Celitech Python SDK 1.1.58
+# Celitech Python SDK 1.1.59
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.58
+- SDK version: 1.1.59
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -102,24 +92,24 @@
 List of available packages
 
 - HTTP Method: `GET`
 - Endpoint: `/packages`
 
 **Parameters**
 
-| Name         | Type  | Required | Description                |
-| :----------- | :---- | :------: | :------------------------- |
-| destination  | str   |    ❌    | List of available packages |
-| start_date   | str   |    ❌    | List of available packages |
-| end_date     | str   |    ❌    | List of available packages |
-| after_cursor | str   |    ❌    | List of available packages |
-| limit        | float |    ❌    | List of available packages |
-| start_time   | int   |    ❌    | List of available packages |
-| end_time     | int   |    ❌    | List of available packages |
-| duration     | float |    ❌    | List of available packages |
+| Name         | Type  | Required | Description                                                                                                                                                                                                         |
+| :----------- | :---- | :------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| destination  | str   |    ❌    | ISO representation of the package's destination.                                                                                                                                                                    |
+| start_date   | str   |    ❌    | Start date of the package's validity in the format 'yyyy-MM-dd'. This date can be set to the current day or any day within the next 12 months.                                                                      |
+| end_date     | str   |    ❌    | End date of the package's validity in the format 'yyyy-MM-dd'. End date can be maximum 90 days after Start date.                                                                                                    |
+| after_cursor | str   |    ❌    | To get the next batch of results, use this parameter. It tells the API where to start fetching data after the last item you received. It helps you avoid repeats and efficiently browse through large sets of data. |
+| limit        | float |    ❌    | Maximum number of packages to be returned in the response. The value must be greater than 0 and less than or equal to 160. If not provided, the default value is 20                                                 |
+| start_time   | int   |    ❌    | Epoch value representing the start time of the package's validity. This timestamp can be set to the current time or any time within the next 12 months                                                              |
+| end_time     | int   |    ❌    | Epoch value representing the end time of the package's validity. End time can be maximum 90 days after Start time                                                                                                   |
+| duration     | float |    ❌    | Duration in seconds for the package's validity. If this parameter is present, it will override the startTime and endTime parameters. The maximum duration for a package's validity period is 90 days                |
 
 **Return Type**
 
 `ListPackagesOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -152,23 +142,23 @@
 This endpoint can be used to list all the successful purchases made between a given interval.
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases`
 
 **Parameters**
 
-| Name         | Type  | Required | Description                                                                                   |
-| :----------- | :---- | :------: | :-------------------------------------------------------------------------------------------- |
-| iccid        | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after_date   | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| before_date  | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after_cursor | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| limit        | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after        | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| before       | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| Name         | Type  | Required | Description                                                                                                                                                                                                         |
+| :----------- | :---- | :------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| iccid        | str   |    ❌    | ID of the eSIM                                                                                                                                                                                                      |
+| after_date   | str   |    ❌    | Start date of the interval for filtering purchases in the format 'yyyy-MM-dd'                                                                                                                                       |
+| before_date  | str   |    ❌    | End date of the interval for filtering purchases in the format 'yyyy-MM-dd'                                                                                                                                         |
+| after_cursor | str   |    ❌    | To get the next batch of results, use this parameter. It tells the API where to start fetching data after the last item you received. It helps you avoid repeats and efficiently browse through large sets of data. |
+| limit        | float |    ❌    | Maximum number of purchases to be returned in the response. The value must be greater than 0 and less than or equal to 100. If not provided, the default value is 20                                                |
+| after        | float |    ❌    | Epoch value representing the start of the time interval for filtering purchases                                                                                                                                     |
+| before       | float |    ❌    | Epoch value representing the end of the time interval for filtering purchases                                                                                                                                       |
 
 **Return Type**
 
 `ListPurchasesOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -305,17 +295,17 @@
 This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages.
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases/{purchaseId}/consumption`
 
 **Parameters**
 
-| Name        | Type | Required | Description                                                                                                                                                                      |
-| :---------- | :--- | :------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| purchase_id | str  |    ✅    | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
+| Name        | Type | Required | Description        |
+| :---------- | :--- | :------: | :----------------- |
+| purchase_id | str  |    ✅    | ID of the purchase |
 
 **Return Type**
 
 `GetPurchaseConsumptionOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -347,17 +337,17 @@
 Get status from eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim`
 
 **Parameters**
 
-| Name  | Type | Required | Description          |
-| :---- | :--- | :------: | :------------------- |
-| iccid | str  |    ✅    | Get status from eSIM |
+| Name  | Type | Required | Description    |
+| :---- | :--- | :------: | :------------- |
+| iccid | str  |    ✅    | ID of the eSIM |
 
 **Return Type**
 
 `GetEsimOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -378,17 +368,17 @@
 Get device info from an installed eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/device`
 
 **Parameters**
 
-| Name  | Type | Required | Description                            |
-| :---- | :--- | :------: | :------------------------------------- |
-| iccid | str  |    ✅    | Get device info from an installed eSIM |
+| Name  | Type | Required | Description    |
+| :---- | :--- | :------: | :------------- |
+| iccid | str  |    ✅    | ID of the eSIM |
 
 **Return Type**
 
 `GetEsimDeviceOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -409,17 +399,17 @@
 Get history from an eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/history`
 
 **Parameters**
 
-| Name  | Type | Required | Description              |
-| :---- | :--- | :------: | :----------------------- |
-| iccid | str  |    ✅    | Get history from an eSIM |
+| Name  | Type | Required | Description    |
+| :---- | :--- | :------: | :------------- |
+| iccid | str  |    ✅    | ID of the eSIM |
 
 **Return Type**
 
 `GetEsimHistoryOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -440,17 +430,17 @@
 Get MAC from eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/mac`
 
 **Parameters**
 
-| Name  | Type | Required | Description       |
-| :---- | :--- | :------: | :---------------- |
-| iccid | str  |    ✅    | Get MAC from eSIM |
+| Name  | Type | Required | Description    |
+| :---- | :--- | :------: | :------------- |
+| iccid | str  |    ✅    | ID of the eSIM |
 
 **Return Type**
 
 `GetEsimMacOkResponse`
 
 **Example Usage Code Snippet**
```

### Comparing `celitech_sdk-1.1.58/README.md` & `celitech_sdk-1.1.59/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,23 @@
-# Celitech Python SDK 1.1.58
+Metadata-Version: 2.1
+Name: celitech-sdk
+Version: 1.1.59
+Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+
+# Celitech Python SDK 1.1.59
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.58
+- SDK version: 1.1.59
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -92,24 +102,24 @@
 List of available packages
 
 - HTTP Method: `GET`
 - Endpoint: `/packages`
 
 **Parameters**
 
-| Name         | Type  | Required | Description                |
-| :----------- | :---- | :------: | :------------------------- |
-| destination  | str   |    ❌    | List of available packages |
-| start_date   | str   |    ❌    | List of available packages |
-| end_date     | str   |    ❌    | List of available packages |
-| after_cursor | str   |    ❌    | List of available packages |
-| limit        | float |    ❌    | List of available packages |
-| start_time   | int   |    ❌    | List of available packages |
-| end_time     | int   |    ❌    | List of available packages |
-| duration     | float |    ❌    | List of available packages |
+| Name         | Type  | Required | Description                                                                                                                                                                                                         |
+| :----------- | :---- | :------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| destination  | str   |    ❌    | ISO representation of the package's destination.                                                                                                                                                                    |
+| start_date   | str   |    ❌    | Start date of the package's validity in the format 'yyyy-MM-dd'. This date can be set to the current day or any day within the next 12 months.                                                                      |
+| end_date     | str   |    ❌    | End date of the package's validity in the format 'yyyy-MM-dd'. End date can be maximum 90 days after Start date.                                                                                                    |
+| after_cursor | str   |    ❌    | To get the next batch of results, use this parameter. It tells the API where to start fetching data after the last item you received. It helps you avoid repeats and efficiently browse through large sets of data. |
+| limit        | float |    ❌    | Maximum number of packages to be returned in the response. The value must be greater than 0 and less than or equal to 160. If not provided, the default value is 20                                                 |
+| start_time   | int   |    ❌    | Epoch value representing the start time of the package's validity. This timestamp can be set to the current time or any time within the next 12 months                                                              |
+| end_time     | int   |    ❌    | Epoch value representing the end time of the package's validity. End time can be maximum 90 days after Start time                                                                                                   |
+| duration     | float |    ❌    | Duration in seconds for the package's validity. If this parameter is present, it will override the startTime and endTime parameters. The maximum duration for a package's validity period is 90 days                |
 
 **Return Type**
 
 `ListPackagesOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -142,23 +152,23 @@
 This endpoint can be used to list all the successful purchases made between a given interval.
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases`
 
 **Parameters**
 
-| Name         | Type  | Required | Description                                                                                   |
-| :----------- | :---- | :------: | :-------------------------------------------------------------------------------------------- |
-| iccid        | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after_date   | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| before_date  | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after_cursor | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| limit        | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after        | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| before       | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| Name         | Type  | Required | Description                                                                                                                                                                                                         |
+| :----------- | :---- | :------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| iccid        | str   |    ❌    | ID of the eSIM                                                                                                                                                                                                      |
+| after_date   | str   |    ❌    | Start date of the interval for filtering purchases in the format 'yyyy-MM-dd'                                                                                                                                       |
+| before_date  | str   |    ❌    | End date of the interval for filtering purchases in the format 'yyyy-MM-dd'                                                                                                                                         |
+| after_cursor | str   |    ❌    | To get the next batch of results, use this parameter. It tells the API where to start fetching data after the last item you received. It helps you avoid repeats and efficiently browse through large sets of data. |
+| limit        | float |    ❌    | Maximum number of purchases to be returned in the response. The value must be greater than 0 and less than or equal to 100. If not provided, the default value is 20                                                |
+| after        | float |    ❌    | Epoch value representing the start of the time interval for filtering purchases                                                                                                                                     |
+| before       | float |    ❌    | Epoch value representing the end of the time interval for filtering purchases                                                                                                                                       |
 
 **Return Type**
 
 `ListPurchasesOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -295,17 +305,17 @@
 This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages.
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases/{purchaseId}/consumption`
 
 **Parameters**
 
-| Name        | Type | Required | Description                                                                                                                                                                      |
-| :---------- | :--- | :------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| purchase_id | str  |    ✅    | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
+| Name        | Type | Required | Description        |
+| :---------- | :--- | :------: | :----------------- |
+| purchase_id | str  |    ✅    | ID of the purchase |
 
 **Return Type**
 
 `GetPurchaseConsumptionOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -337,17 +347,17 @@
 Get status from eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim`
 
 **Parameters**
 
-| Name  | Type | Required | Description          |
-| :---- | :--- | :------: | :------------------- |
-| iccid | str  |    ✅    | Get status from eSIM |
+| Name  | Type | Required | Description    |
+| :---- | :--- | :------: | :------------- |
+| iccid | str  |    ✅    | ID of the eSIM |
 
 **Return Type**
 
 `GetEsimOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -368,17 +378,17 @@
 Get device info from an installed eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/device`
 
 **Parameters**
 
-| Name  | Type | Required | Description                            |
-| :---- | :--- | :------: | :------------------------------------- |
-| iccid | str  |    ✅    | Get device info from an installed eSIM |
+| Name  | Type | Required | Description    |
+| :---- | :--- | :------: | :------------- |
+| iccid | str  |    ✅    | ID of the eSIM |
 
 **Return Type**
 
 `GetEsimDeviceOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -399,17 +409,17 @@
 Get history from an eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/history`
 
 **Parameters**
 
-| Name  | Type | Required | Description              |
-| :---- | :--- | :------: | :----------------------- |
-| iccid | str  |    ✅    | Get history from an eSIM |
+| Name  | Type | Required | Description    |
+| :---- | :--- | :------: | :------------- |
+| iccid | str  |    ✅    | ID of the eSIM |
 
 **Return Type**
 
 `GetEsimHistoryOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -430,17 +440,17 @@
 Get MAC from eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/mac`
 
 **Parameters**
 
-| Name  | Type | Required | Description       |
-| :---- | :--- | :------: | :---------------- |
-| iccid | str  |    ✅    | Get MAC from eSIM |
+| Name  | Type | Required | Description    |
+| :---- | :--- | :------: | :------------- |
+| iccid | str  |    ✅    | ID of the eSIM |
 
 **Return Type**
 
 `GetEsimMacOkResponse`
 
 **Example Usage Code Snippet**
```

### Comparing `celitech_sdk-1.1.58/src/celitech/hooks/hook.py` & `celitech_sdk-1.1.59/src/celitech/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/__init__.py` & `celitech_sdk-1.1.59/src/celitech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/base.py` & `celitech_sdk-1.1.59/src/celitech/models/base.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/create_purchase_ok_response.py` & `celitech_sdk-1.1.59/src/celitech/models/create_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/create_purchase_request.py` & `celitech_sdk-1.1.59/src/celitech/models/create_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/edit_purchase_ok_response.py` & `celitech_sdk-1.1.59/src/celitech/models/edit_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/edit_purchase_request.py` & `celitech_sdk-1.1.59/src/celitech/models/edit_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/get_esim_device_ok_response.py` & `celitech_sdk-1.1.59/src/celitech/models/get_esim_device_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/get_esim_history_ok_response.py` & `celitech_sdk-1.1.59/src/celitech/models/get_esim_history_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/get_esim_mac_ok_response.py` & `celitech_sdk-1.1.59/src/celitech/models/get_esim_mac_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/get_esim_ok_response.py` & `celitech_sdk-1.1.59/src/celitech/models/get_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/get_purchase_consumption_ok_response.py` & `celitech_sdk-1.1.59/src/celitech/models/get_purchase_consumption_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/list_destinations_ok_response.py` & `celitech_sdk-1.1.59/src/celitech/models/list_destinations_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/list_packages_ok_response.py` & `celitech_sdk-1.1.59/src/celitech/models/list_packages_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/list_purchases_ok_response.py` & `celitech_sdk-1.1.59/src/celitech/models/list_purchases_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/top_up_esim_ok_response.py` & `celitech_sdk-1.1.59/src/celitech/models/top_up_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/top_up_esim_request.py` & `celitech_sdk-1.1.59/src/celitech/models/top_up_esim_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/utils/cast_models.py` & `celitech_sdk-1.1.59/src/celitech/models/utils/cast_models.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/models/utils/json_map.py` & `celitech_sdk-1.1.59/src/celitech/models/utils/json_map.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/base_handler.py` & `celitech_sdk-1.1.59/src/celitech/net/request_chain/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/hook_handler.py` & `celitech_sdk-1.1.59/src/celitech/net/request_chain/handlers/hook_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/http_handler.py` & `celitech_sdk-1.1.59/src/celitech/net/request_chain/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/retry_handler.py` & `celitech_sdk-1.1.59/src/celitech/net/request_chain/handlers/retry_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/net/request_chain/request_chain.py` & `celitech_sdk-1.1.59/src/celitech/net/request_chain/request_chain.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/net/transport/request.py` & `celitech_sdk-1.1.59/src/celitech/net/transport/request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/net/transport/request_error.py` & `celitech_sdk-1.1.59/src/celitech/net/transport/request_error.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/net/transport/response.py` & `celitech_sdk-1.1.59/src/celitech/net/transport/response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/net/transport/serializer.py` & `celitech_sdk-1.1.59/src/celitech/net/transport/serializer.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/net/transport/utils.py` & `celitech_sdk-1.1.59/src/celitech/net/transport/utils.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/sdk.py` & `celitech_sdk-1.1.59/src/celitech/sdk.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/services/destinations.py` & `celitech_sdk-1.1.59/src/celitech/services/destinations.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/services/e_sim.py` & `celitech_sdk-1.1.59/src/celitech/services/e_sim.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/services/packages.py` & `celitech_sdk-1.1.59/src/celitech/services/packages.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/services/purchases.py` & `celitech_sdk-1.1.59/src/celitech/services/purchases.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/services/utils/base_service.py` & `celitech_sdk-1.1.59/src/celitech/services/utils/base_service.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/services/utils/default_headers.py` & `celitech_sdk-1.1.59/src/celitech/services/utils/default_headers.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech/services/utils/validator.py` & `celitech_sdk-1.1.59/src/celitech/services/utils/validator.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.58/src/celitech_sdk.egg-info/PKG-INFO` & `celitech_sdk-1.1.59/src/celitech_sdk.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: celitech-sdk
-Version: 1.1.58
+Version: 1.1.59
 Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Celitech Python SDK 1.1.58
+# Celitech Python SDK 1.1.59
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.58
+- SDK version: 1.1.59
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -102,24 +102,24 @@
 List of available packages
 
 - HTTP Method: `GET`
 - Endpoint: `/packages`
 
 **Parameters**
 
-| Name         | Type  | Required | Description                |
-| :----------- | :---- | :------: | :------------------------- |
-| destination  | str   |    ❌    | List of available packages |
-| start_date   | str   |    ❌    | List of available packages |
-| end_date     | str   |    ❌    | List of available packages |
-| after_cursor | str   |    ❌    | List of available packages |
-| limit        | float |    ❌    | List of available packages |
-| start_time   | int   |    ❌    | List of available packages |
-| end_time     | int   |    ❌    | List of available packages |
-| duration     | float |    ❌    | List of available packages |
+| Name         | Type  | Required | Description                                                                                                                                                                                                         |
+| :----------- | :---- | :------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| destination  | str   |    ❌    | ISO representation of the package's destination.                                                                                                                                                                    |
+| start_date   | str   |    ❌    | Start date of the package's validity in the format 'yyyy-MM-dd'. This date can be set to the current day or any day within the next 12 months.                                                                      |
+| end_date     | str   |    ❌    | End date of the package's validity in the format 'yyyy-MM-dd'. End date can be maximum 90 days after Start date.                                                                                                    |
+| after_cursor | str   |    ❌    | To get the next batch of results, use this parameter. It tells the API where to start fetching data after the last item you received. It helps you avoid repeats and efficiently browse through large sets of data. |
+| limit        | float |    ❌    | Maximum number of packages to be returned in the response. The value must be greater than 0 and less than or equal to 160. If not provided, the default value is 20                                                 |
+| start_time   | int   |    ❌    | Epoch value representing the start time of the package's validity. This timestamp can be set to the current time or any time within the next 12 months                                                              |
+| end_time     | int   |    ❌    | Epoch value representing the end time of the package's validity. End time can be maximum 90 days after Start time                                                                                                   |
+| duration     | float |    ❌    | Duration in seconds for the package's validity. If this parameter is present, it will override the startTime and endTime parameters. The maximum duration for a package's validity period is 90 days                |
 
 **Return Type**
 
 `ListPackagesOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -152,23 +152,23 @@
 This endpoint can be used to list all the successful purchases made between a given interval.
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases`
 
 **Parameters**
 
-| Name         | Type  | Required | Description                                                                                   |
-| :----------- | :---- | :------: | :-------------------------------------------------------------------------------------------- |
-| iccid        | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after_date   | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| before_date  | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after_cursor | str   |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| limit        | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| after        | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
-| before       | float |    ❌    | This endpoint can be used to list all the successful purchases made between a given interval. |
+| Name         | Type  | Required | Description                                                                                                                                                                                                         |
+| :----------- | :---- | :------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| iccid        | str   |    ❌    | ID of the eSIM                                                                                                                                                                                                      |
+| after_date   | str   |    ❌    | Start date of the interval for filtering purchases in the format 'yyyy-MM-dd'                                                                                                                                       |
+| before_date  | str   |    ❌    | End date of the interval for filtering purchases in the format 'yyyy-MM-dd'                                                                                                                                         |
+| after_cursor | str   |    ❌    | To get the next batch of results, use this parameter. It tells the API where to start fetching data after the last item you received. It helps you avoid repeats and efficiently browse through large sets of data. |
+| limit        | float |    ❌    | Maximum number of purchases to be returned in the response. The value must be greater than 0 and less than or equal to 100. If not provided, the default value is 20                                                |
+| after        | float |    ❌    | Epoch value representing the start of the time interval for filtering purchases                                                                                                                                     |
+| before       | float |    ❌    | Epoch value representing the end of the time interval for filtering purchases                                                                                                                                       |
 
 **Return Type**
 
 `ListPurchasesOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -305,17 +305,17 @@
 This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages.
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases/{purchaseId}/consumption`
 
 **Parameters**
 
-| Name        | Type | Required | Description                                                                                                                                                                      |
-| :---------- | :--- | :------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| purchase_id | str  |    ✅    | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
+| Name        | Type | Required | Description        |
+| :---------- | :--- | :------: | :----------------- |
+| purchase_id | str  |    ✅    | ID of the purchase |
 
 **Return Type**
 
 `GetPurchaseConsumptionOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -347,17 +347,17 @@
 Get status from eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim`
 
 **Parameters**
 
-| Name  | Type | Required | Description          |
-| :---- | :--- | :------: | :------------------- |
-| iccid | str  |    ✅    | Get status from eSIM |
+| Name  | Type | Required | Description    |
+| :---- | :--- | :------: | :------------- |
+| iccid | str  |    ✅    | ID of the eSIM |
 
 **Return Type**
 
 `GetEsimOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -378,17 +378,17 @@
 Get device info from an installed eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/device`
 
 **Parameters**
 
-| Name  | Type | Required | Description                            |
-| :---- | :--- | :------: | :------------------------------------- |
-| iccid | str  |    ✅    | Get device info from an installed eSIM |
+| Name  | Type | Required | Description    |
+| :---- | :--- | :------: | :------------- |
+| iccid | str  |    ✅    | ID of the eSIM |
 
 **Return Type**
 
 `GetEsimDeviceOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -409,17 +409,17 @@
 Get history from an eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/history`
 
 **Parameters**
 
-| Name  | Type | Required | Description              |
-| :---- | :--- | :------: | :----------------------- |
-| iccid | str  |    ✅    | Get history from an eSIM |
+| Name  | Type | Required | Description    |
+| :---- | :--- | :------: | :------------- |
+| iccid | str  |    ✅    | ID of the eSIM |
 
 **Return Type**
 
 `GetEsimHistoryOkResponse`
 
 **Example Usage Code Snippet**
 
@@ -440,17 +440,17 @@
 Get MAC from eSIM
 
 - HTTP Method: `GET`
 - Endpoint: `/esim/{iccid}/mac`
 
 **Parameters**
 
-| Name  | Type | Required | Description       |
-| :---- | :--- | :------: | :---------------- |
-| iccid | str  |    ✅    | Get MAC from eSIM |
+| Name  | Type | Required | Description    |
+| :---- | :--- | :------: | :------------- |
+| iccid | str  |    ✅    | ID of the eSIM |
 
 **Return Type**
 
 `GetEsimMacOkResponse`
 
 **Example Usage Code Snippet**
```

### Comparing `celitech_sdk-1.1.58/src/celitech_sdk.egg-info/SOURCES.txt` & `celitech_sdk-1.1.59/src/celitech_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

