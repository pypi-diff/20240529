# Comparing `tmp/hahomematic-2024.5.4.tar.gz` & `tmp/hahomematic-2024.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.5.4.tar", last modified: Thu May 23 14:45:58 2024, max compression
+gzip compressed data, was "hahomematic-2024.5.5.tar", last modified: Wed May 29 17:57:46 2024, max compression
```

## Comparing `hahomematic-2024.5.4.tar` & `hahomematic-2024.5.5.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:58.415328 hahomematic-2024.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-23 14:45:58.415328 hahomematic-2024.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:58.403328 hahomematic-2024.5.4/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/async_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:58.403328 hahomematic-2024.5.4/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18130 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/caches/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:58.403328 hahomematic-2024.5.4/hahomematic/central/
--rw-r--r--   0 runner    (1001) docker     (127)    55193 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/central/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/central/command_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/central/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/central/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:58.403328 hahomematic-2024.5.4/hahomematic/client/
--rw-r--r--   0 runner    (1001) docker     (127)    46155 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/client/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/client/xml_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:58.407328 hahomematic-2024.5.4/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:58.407328 hahomematic-2024.5.4/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26320 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    27110 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30203 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    13069 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    44099 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33434 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    30311 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:58.411328 hahomematic-2024.5.4/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:58.411328 hahomematic-2024.5.4/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    14151 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:58.411328 hahomematic-2024.5.4/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:58.415328 hahomematic-2024.5.4/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-23 14:45:58.000000 hahomematic-2024.5.4/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-23 14:45:58.000000 hahomematic-2024.5.4/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:45:58.000000 hahomematic-2024.5.4/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:45:58.000000 hahomematic-2024.5.4/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-23 14:45:58.000000 hahomematic-2024.5.4/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 14:45:58.000000 hahomematic-2024.5.4/hahomematic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:58.411328 hahomematic-2024.5.4/hahomematic_support/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/hahomematic_support/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-23 14:45:58.415328 hahomematic-2024.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:45:58.415328 hahomematic-2024.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_central_pydevccu.py
--rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    35513 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    39142 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    17156 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-23 14:45:33.000000 hahomematic-2024.5.4/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:46.202524 hahomematic-2024.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-29 17:57:46.202524 hahomematic-2024.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:46.186524 hahomematic-2024.5.5/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/async_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:46.190524 hahomematic-2024.5.5/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18130 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/caches/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:46.190524 hahomematic-2024.5.5/hahomematic/central/
+-rw-r--r--   0 runner    (1001) docker     (127)    55193 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/central/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/central/command_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/central/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/central/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:46.190524 hahomematic-2024.5.5/hahomematic/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    46155 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/client/json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/client/xml_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:46.190524 hahomematic-2024.5.5/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:46.194524 hahomematic-2024.5.5/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26320 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27110 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30203 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13069 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44099 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33434 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30311 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:46.194524 hahomematic-2024.5.5/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:46.198524 hahomematic-2024.5.5/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14151 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:46.198524 hahomematic-2024.5.5/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:46.202524 hahomematic-2024.5.5/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-29 17:57:46.000000 hahomematic-2024.5.5/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-29 17:57:46.000000 hahomematic-2024.5.5/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:57:46.000000 hahomematic-2024.5.5/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:57:45.000000 hahomematic-2024.5.5/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-29 17:57:46.000000 hahomematic-2024.5.5/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 17:57:46.000000 hahomematic-2024.5.5/hahomematic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:46.198524 hahomematic-2024.5.5/hahomematic_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/hahomematic_support/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-29 17:57:46.202524 hahomematic-2024.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:57:46.202524 hahomematic-2024.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_central_pydevccu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35513 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39142 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17156 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-29 17:57:22.000000 hahomematic-2024.5.5/tests/test_text.py
```

### Comparing `hahomematic-2024.5.4/LICENSE` & `hahomematic-2024.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/PKG-INFO` & `hahomematic-2024.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.5.4
+Version: 2024.5.5
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.5.4/README.md` & `hahomematic-2024.5.5/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/__init__.py` & `hahomematic-2024.5.5/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/async_support.py` & `hahomematic-2024.5.5/hahomematic/async_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/caches/dynamic.py` & `hahomematic-2024.5.5/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/caches/persistent.py` & `hahomematic-2024.5.5/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/caches/visibility.py` & `hahomematic-2024.5.5/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/central/__init__.py` & `hahomematic-2024.5.5/hahomematic/central/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/central/command_queue.py` & `hahomematic-2024.5.5/hahomematic/central/command_queue.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/central/decorators.py` & `hahomematic-2024.5.5/hahomematic/central/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/central/xml_rpc_server.py` & `hahomematic-2024.5.5/hahomematic/central/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/client/__init__.py` & `hahomematic-2024.5.5/hahomematic/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/client/json_rpc.py` & `hahomematic-2024.5.5/hahomematic/client/json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/client/xml_rpc.py` & `hahomematic-2024.5.5/hahomematic/client/xml_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/config.py` & `hahomematic-2024.5.5/hahomematic/config.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/const.py` & `hahomematic-2024.5.5/hahomematic/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,15 +484,15 @@
     "HM-RCV-50",
     "HMW-RCV-50",
     "HmIP-RCV-50",
 )
 
 VIRTUAL_REMOTE_ADDRESSES: Final[tuple[str, ...]] = (
     "BidCoS-RF",
-    "HMW-RCV-50",
+    "BidCoS-Wir",
     "HmIP-RCV-1",
 )
 
 
 @dataclass(frozen=True, kw_only=True, slots=True)
 class HubData:
     """Dataclass for hub entities."""
```

### Comparing `hahomematic-2024.5.4/hahomematic/converter.py` & `hahomematic-2024.5.5/hahomematic/converter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/exceptions.py` & `hahomematic-2024.5.5/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/hmcli.py` & `hahomematic-2024.5.5/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/performance.py` & `hahomematic-2024.5.5/hahomematic/performance.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/__init__.py` & `hahomematic-2024.5.5/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/custom/__init__.py` & `hahomematic-2024.5.5/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/custom/climate.py` & `hahomematic-2024.5.5/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/custom/const.py` & `hahomematic-2024.5.5/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/custom/cover.py` & `hahomematic-2024.5.5/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/custom/definition.py` & `hahomematic-2024.5.5/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/custom/entity.py` & `hahomematic-2024.5.5/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/custom/light.py` & `hahomematic-2024.5.5/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/custom/lock.py` & `hahomematic-2024.5.5/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/custom/siren.py` & `hahomematic-2024.5.5/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/custom/support.py` & `hahomematic-2024.5.5/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/custom/switch.py` & `hahomematic-2024.5.5/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/decorators.py` & `hahomematic-2024.5.5/hahomematic/platforms/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/device.py` & `hahomematic-2024.5.5/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/entity.py` & `hahomematic-2024.5.5/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/event.py` & `hahomematic-2024.5.5/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/generic/__init__.py` & `hahomematic-2024.5.5/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/generic/action.py` & `hahomematic-2024.5.5/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2024.5.5/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/generic/button.py` & `hahomematic-2024.5.5/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/generic/entity.py` & `hahomematic-2024.5.5/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/generic/number.py` & `hahomematic-2024.5.5/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/generic/select.py` & `hahomematic-2024.5.5/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/generic/sensor.py` & `hahomematic-2024.5.5/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/generic/switch.py` & `hahomematic-2024.5.5/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/hub/__init__.py` & `hahomematic-2024.5.5/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2024.5.5/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/hub/button.py` & `hahomematic-2024.5.5/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/hub/entity.py` & `hahomematic-2024.5.5/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/hub/number.py` & `hahomematic-2024.5.5/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/hub/select.py` & `hahomematic-2024.5.5/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/hub/sensor.py` & `hahomematic-2024.5.5/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/hub/text.py` & `hahomematic-2024.5.5/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/support.py` & `hahomematic-2024.5.5/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/platforms/update.py` & `hahomematic-2024.5.5/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2024.5.5/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2024.5.5/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2024.5.5/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic/support.py` & `hahomematic-2024.5.5/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic.egg-info/PKG-INFO` & `hahomematic-2024.5.5/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.5.4
+Version: 2024.5.5
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.5.4/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2024.5.5/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/hahomematic_support/client_local.py` & `hahomematic-2024.5.5/hahomematic_support/client_local.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/pyproject.toml` & `hahomematic-2024.5.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=69.2.0", "wheel~=0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2024.5.4"
+version     = "2024.5.5"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

### Comparing `hahomematic-2024.5.4/tests/test_action.py` & `hahomematic-2024.5.5/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_binary_sensor.py` & `hahomematic-2024.5.5/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_button.py` & `hahomematic-2024.5.5/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_central.py` & `hahomematic-2024.5.5/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_central_pydevccu.py` & `hahomematic-2024.5.5/tests/test_central_pydevccu.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_climate.py` & `hahomematic-2024.5.5/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_cover.py` & `hahomematic-2024.5.5/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_decorator.py` & `hahomematic-2024.5.5/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_device.py` & `hahomematic-2024.5.5/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_entity.py` & `hahomematic-2024.5.5/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_event.py` & `hahomematic-2024.5.5/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_json_rpc.py` & `hahomematic-2024.5.5/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_light.py` & `hahomematic-2024.5.5/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_lock.py` & `hahomematic-2024.5.5/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_number.py` & `hahomematic-2024.5.5/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_select.py` & `hahomematic-2024.5.5/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_sensor.py` & `hahomematic-2024.5.5/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_siren.py` & `hahomematic-2024.5.5/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_support.py` & `hahomematic-2024.5.5/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_switch.py` & `hahomematic-2024.5.5/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.4/tests/test_text.py` & `hahomematic-2024.5.5/tests/test_text.py`

 * *Files identical despite different names*

