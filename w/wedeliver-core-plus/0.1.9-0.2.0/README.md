# Comparing `tmp/wedeliver_core_plus-0.1.9.tar.gz` & `tmp/wedeliver_core_plus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/wedeliver_core_plus/dist/.tmp-p5vzlq1w/wedeliver_core_plus-0.1.9.tar", last modified: Sun May 12 11:24:34 2024, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/wedeliver_core_plus/dist/.tmp-9zk9lkru/wedeliver_core_plus-0.2.0.tar", last modified: Wed May 29 16:16:18 2024, max compression
```

## Comparing `wedeliver_core_plus-0.1.9.tar` & `wedeliver_core_plus-0.2.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/amazon/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/kafka_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/kafka_producers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/kafka_producers/send_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/kafka_producers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/kafka_producers/send_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/system_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-12 11:24:28.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-12 11:24:34.000000 wedeliver_core_plus-0.1.9/wedeliver_core_plus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/amazon/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/kafka_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/kafka_producers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/kafka_producers/send_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/kafka_producers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/kafka_producers/send_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/system_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-29 16:16:12.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-29 16:16:18.000000 wedeliver_core_plus-0.2.0/wedeliver_core_plus.egg-info/top_level.txt
```

### Comparing `wedeliver_core_plus-0.1.9/PKG-INFO` & `wedeliver_core_plus-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedeliver_core_plus
-Version: 0.1.9
+Version: 0.2.0
 Summary: wedeliver_core_plus package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `wedeliver_core_plus-0.1.9/setup.py` & `wedeliver_core_plus-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "Flask-SQLAlchemy",
     "flask-marshmallow",
     "confluent-kafka",
     "requests",
     "python-dotenv",
 ]
 
-# some more details
+# Some more details
 CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Internet",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="wedeliver_core_plus",
-    version="0.1.9",
+    version="0.2.0",
     description="wedeliver_core_plus package",
     long_description="""# Markdown supported!\n\n* wedeliver core plus\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
```

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/__init__.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/app_decorators/app_entry.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/app_decorators/app_entry.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/app_decorators/handle_auth.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/app_decorators/handle_auth.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/app_decorators/handle_exceptions.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/app_decorators/handle_exceptions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/app_decorators/handle_response.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/app_decorators/serializer.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/app_decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/base.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/base.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/acl_enum.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/acl_enum.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/amazon/get_file_url.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/amazon/get_file_url.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/amazon/get_s3_client.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/amazon/get_s3_client.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/amazon/upload_file.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/amazon/upload_file.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/atomic_transactions.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/atomic_transactions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/atomic_transactions_v2.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/atomic_transactions_v2.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/auth.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/config.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/database/base_model.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/database/base_model.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/database/log_model.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/database/log_model.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/enums.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/exceptions.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/fetch_relational_data.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/fetch_relational_data.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/filters.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/format_exception.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/format_exception.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/get_embedded_function.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/get_obj_value.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/get_obj_value.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/kafka_listener.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/kafka_listener.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/kafka_producer.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/kafka_producer.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/kafka_producers/notification_center.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/kafka_producers/notification_center.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/log_config.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/log_config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/micro_fetcher.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/micro_fetcher.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/search_function.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/security.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/security.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/service_config.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/service_config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/sql.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/sql.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/time.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/time.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/validate_mobile_number.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/validate_mobile_number.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus/helpers/validate_parameters.py` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus.egg-info/PKG-INFO` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedeliver-core-plus
-Version: 0.1.9
+Version: 0.2.0
 Summary: wedeliver_core_plus package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `wedeliver_core_plus-0.1.9/wedeliver_core_plus.egg-info/SOURCES.txt` & `wedeliver_core_plus-0.2.0/wedeliver_core_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

