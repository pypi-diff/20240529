# Comparing `tmp/bigeye_sdk-0.4.81.tar.gz` & `tmp/bigeye_sdk-0.4.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigeye_sdk-0.4.81.tar", max compression
+gzip compressed data, was "bigeye_sdk-0.4.82.tar", max compression
```

## Comparing `bigeye_sdk-0.4.81.tar` & `bigeye_sdk-0.4.82.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     2092 2024-03-26 20:10:15.103396 bigeye_sdk-0.4.81/LICENSE
--rw-r--r--   0        0        0      873 2024-03-26 20:10:15.103476 bigeye_sdk-0.4.81/README.md
--rw-r--r--   0        0        0     3727 2024-03-26 20:10:15.103593 bigeye_sdk-0.4.81/bigeye_sdk/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 20:10:15.103676 bigeye_sdk-0.4.81/bigeye_sdk/__version__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.103753 bigeye_sdk-0.4.81/bigeye_sdk/authentication/__init__.py
--rw-r--r--   0        0        0    20437 2024-05-23 15:35:27.066145 bigeye_sdk-0.4.81/bigeye_sdk/authentication/api_authentication.py
--rw-r--r--   0        0        0    12761 2024-04-16 21:02:55.536986 bigeye_sdk-0.4.81/bigeye_sdk/authentication/config.py
--rw-r--r--   0        0        0     1182 2024-03-26 20:10:15.104056 bigeye_sdk-0.4.81/bigeye_sdk/authentication/credentials.py
--rw-r--r--   0        0        0      734 2024-03-26 20:10:15.104126 bigeye_sdk-0.4.81/bigeye_sdk/authentication/enums.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.104202 bigeye_sdk-0.4.81/bigeye_sdk/bigconfig_validation/__init__.py
--rw-r--r--   0        0        0    11104 2024-05-23 15:35:27.067204 bigeye_sdk-0.4.81/bigeye_sdk/bigconfig_validation/big_config_reports.py
--rw-r--r--   0        0        0     8116 2024-03-26 20:10:15.104508 bigeye_sdk-0.4.81/bigeye_sdk/bigconfig_validation/validation_context.py
--rw-r--r--   0        0        0     1579 2024-03-26 20:10:15.104585 bigeye_sdk-0.4.81/bigeye_sdk/bigconfig_validation/validation_functions.py
--rw-r--r--   0        0        0      736 2024-03-26 20:10:15.104656 bigeye_sdk-0.4.81/bigeye_sdk/bigconfig_validation/validation_models.py
--rw-r--r--   0        0        0     9363 2024-05-14 19:46:32.468012 bigeye_sdk-0.4.81/bigeye_sdk/bigconfig_validation/yaml_model_base.py
--rw-r--r--   0        0        0     3900 2024-03-26 20:10:15.104890 bigeye_sdk-0.4.81/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.104964 bigeye_sdk-0.4.81/bigeye_sdk/class_ext/__init__.py
--rw-r--r--   0        0        0      233 2024-03-26 20:10:15.105053 bigeye_sdk-0.4.81/bigeye_sdk/class_ext/dataclass_ext.py
--rw-r--r--   0        0        0      402 2024-03-26 20:10:15.105125 bigeye_sdk-0.4.81/bigeye_sdk/class_ext/enum_ext.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.105194 bigeye_sdk-0.4.81/bigeye_sdk/client/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 20:10:15.105276 bigeye_sdk-0.4.81/bigeye_sdk/client/base_client.py
--rw-r--r--   0        0        0    39844 2024-05-22 20:48:45.142950 bigeye_sdk-0.4.81/bigeye_sdk/client/datawatch_client.py
--rw-r--r--   0        0        0      201 2024-03-26 20:10:15.105478 bigeye_sdk-0.4.81/bigeye_sdk/client/enum.py
--rw-r--r--   0        0        0    54966 2024-05-23 15:35:27.068571 bigeye_sdk-0.4.81/bigeye_sdk/client/generated_datawatch_client.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.105719 bigeye_sdk-0.4.81/bigeye_sdk/controller/__init__.py
--rw-r--r--   0        0        0     2666 2024-03-26 20:10:15.105839 bigeye_sdk-0.4.81/bigeye_sdk/controller/delta_controller.py
--rw-r--r--   0        0        0    15116 2024-05-23 15:35:27.069489 bigeye_sdk-0.4.81/bigeye_sdk/controller/lineage_controller.py
--rw-r--r--   0        0        0     3209 2024-03-26 20:10:15.106039 bigeye_sdk-0.4.81/bigeye_sdk/controller/metric_controller.py
--rw-r--r--   0        0        0    42347 2024-05-23 15:35:27.069854 bigeye_sdk-0.4.81/bigeye_sdk/controller/metric_suite_controller.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.106304 bigeye_sdk-0.4.81/bigeye_sdk/decorators/__init__.py
--rw-r--r--   0        0        0      307 2024-03-26 20:10:15.106404 bigeye_sdk-0.4.81/bigeye_sdk/decorators/dataclass_decorators.py
--rw-r--r--   0        0        0       97 2024-03-26 20:10:15.106520 bigeye_sdk-0.4.81/bigeye_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0     1582 2024-03-26 20:10:15.106598 bigeye_sdk-0.4.81/bigeye_sdk/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.106671 bigeye_sdk-0.4.81/bigeye_sdk/functions/__init__.py
--rw-r--r--   0        0        0     4469 2024-03-26 20:10:15.106799 bigeye_sdk-0.4.81/bigeye_sdk/functions/athena.py
--rw-r--r--   0        0        0     5202 2024-03-26 20:10:15.106912 bigeye_sdk-0.4.81/bigeye_sdk/functions/aws.py
--rw-r--r--   0        0        0     2450 2024-03-26 20:10:15.106994 bigeye_sdk-0.4.81/bigeye_sdk/functions/bigconfig_functions.py
--rw-r--r--   0        0        0     3469 2024-03-26 20:10:15.107087 bigeye_sdk-0.4.81/bigeye_sdk/functions/casing.py
--rw-r--r--   0        0        0     3215 2024-03-26 20:10:15.107178 bigeye_sdk-0.4.81/bigeye_sdk/functions/core_py_functs.py
--rw-r--r--   0        0        0      370 2024-03-26 20:10:15.107269 bigeye_sdk-0.4.81/bigeye_sdk/functions/dbt.py
--rw-r--r--   0        0        0     4580 2024-03-26 20:10:15.107401 bigeye_sdk-0.4.81/bigeye_sdk/functions/delta_functions.py
--rw-r--r--   0        0        0     2814 2024-03-26 20:10:15.107482 bigeye_sdk-0.4.81/bigeye_sdk/functions/file_functs.py
--rw-r--r--   0        0        0      706 2024-03-26 20:10:15.107556 bigeye_sdk-0.4.81/bigeye_sdk/functions/helpers.py
--rw-r--r--   0        0        0      410 2024-03-26 20:10:15.107645 bigeye_sdk-0.4.81/bigeye_sdk/functions/issue_functions.py
--rw-r--r--   0        0        0    21897 2024-03-26 20:10:15.107751 bigeye_sdk-0.4.81/bigeye_sdk/functions/metric_functions.py
--rw-r--r--   0        0        0     2701 2024-03-26 20:10:15.107850 bigeye_sdk-0.4.81/bigeye_sdk/functions/metric_run_functions.py
--rw-r--r--   0        0        0     1825 2024-05-23 15:35:27.070248 bigeye_sdk-0.4.81/bigeye_sdk/functions/notifications.py
--rw-r--r--   0        0        0     1227 2024-03-26 20:10:15.107923 bigeye_sdk-0.4.81/bigeye_sdk/functions/s3.py
--rw-r--r--   0        0        0     1796 2024-05-23 15:35:27.070390 bigeye_sdk-0.4.81/bigeye_sdk/functions/schema_change_functions.py
--rw-r--r--   0        0        0     1676 2024-03-26 20:10:15.107998 bigeye_sdk-0.4.81/bigeye_sdk/functions/schema_functions.py
--rw-r--r--   0        0        0     5377 2024-04-16 21:02:55.537393 bigeye_sdk-0.4.81/bigeye_sdk/functions/search_and_match_functions.py
--rw-r--r--   0        0        0     4031 2024-03-26 20:10:15.108209 bigeye_sdk-0.4.81/bigeye_sdk/functions/table_functions.py
--rw-r--r--   0        0        0     1701 2024-03-26 20:10:15.108284 bigeye_sdk-0.4.81/bigeye_sdk/functions/urlfuncts.py
--rw-r--r--   0        0        0     2459 2024-04-16 21:02:55.537542 bigeye_sdk-0.4.81/bigeye_sdk/functions/version.py
--rw-r--r--   0        0        0        0 2024-05-23 18:02:41.599139 bigeye_sdk-0.4.81/bigeye_sdk/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 18:02:41.599248 bigeye_sdk-0.4.81/bigeye_sdk/generated/com/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 18:02:41.599355 bigeye_sdk-0.4.81/bigeye_sdk/generated/com/bigeye/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 18:02:41.599438 bigeye_sdk-0.4.81/bigeye_sdk/generated/com/bigeye/models/__init__.py
--rw-r--r--   0        0        0   282764 2024-05-23 18:02:41.599550 bigeye_sdk-0.4.81/bigeye_sdk/generated/com/bigeye/models/generated.py
--rw-r--r--   0        0        0        0 2024-05-23 18:02:41.601241 bigeye_sdk-0.4.81/bigeye_sdk/generated/google/__init__.py
--rw-r--r--   0        0        0    14816 2024-05-23 18:02:41.601404 bigeye_sdk-0.4.81/bigeye_sdk/generated/google/api.py
--rw-r--r--   0        0        0      995 2024-05-23 15:35:27.073747 bigeye_sdk-0.4.81/bigeye_sdk/log/__init__.py
--rw-r--r--   0        0        0        1 2024-03-26 20:10:15.109559 bigeye_sdk-0.4.81/bigeye_sdk/model/__init__.py
--rw-r--r--   0        0        0      492 2024-03-26 20:10:15.109643 bigeye_sdk-0.4.81/bigeye_sdk/model/base_datawatch_facade.py
--rw-r--r--   0        0        0    37552 2024-05-14 19:46:32.468851 bigeye_sdk-0.4.81/bigeye_sdk/model/big_config.py
--rw-r--r--   0        0        0      778 2024-03-26 20:10:15.109855 bigeye_sdk-0.4.81/bigeye_sdk/model/collection_models.py
--rw-r--r--   0        0        0      872 2024-03-26 20:10:15.109935 bigeye_sdk-0.4.81/bigeye_sdk/model/dbt_manifest.py
--rw-r--r--   0        0        0     4518 2024-03-26 20:10:15.110060 bigeye_sdk-0.4.81/bigeye_sdk/model/dbt_schema.py
--rw-r--r--   0        0        0     5521 2024-05-14 11:15:09.573368 bigeye_sdk-0.4.81/bigeye_sdk/model/delta_facade.py
--rw-r--r--   0        0        0       89 2024-03-26 20:10:15.110260 bigeye_sdk-0.4.81/bigeye_sdk/model/enums.py
--rw-r--r--   0        0        0     9459 2024-03-26 20:10:15.110414 bigeye_sdk-0.4.81/bigeye_sdk/model/metric_facade.py
--rw-r--r--   0        0        0    11200 2024-05-23 15:35:27.074297 bigeye_sdk-0.4.81/bigeye_sdk/model/protobuf_enum_facade.py
--rw-r--r--   0        0        0      221 2024-03-26 20:10:15.110628 bigeye_sdk-0.4.81/bigeye_sdk/model/protobuf_extensions.py
--rw-r--r--   0        0        0    56945 2024-05-22 20:48:45.147415 bigeye_sdk-0.4.81/bigeye_sdk/model/protobuf_message_facade.py
--rw-r--r--   0        0        0     6142 2024-05-23 15:35:27.074413 bigeye_sdk-0.4.81/bigeye_sdk/model/schema_change.py
--rw-r--r--   0        0        0      865 2024-03-26 20:10:15.110847 bigeye_sdk-0.4.81/bigeye_sdk/model/sla_models.py
--rw-r--r--   0        0        0     7599 2024-05-22 20:55:06.179834 bigeye_sdk-0.4.81/bigeye_sdk/serializable.py
--rw-r--r--   0        0        0     3396 2024-05-23 18:01:52.225153 bigeye_sdk-0.4.81/pyproject.toml
--rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.81/PKG-INFO
+-rw-r--r--   0        0        0     2092 2024-03-26 20:10:15.103396 bigeye_sdk-0.4.82/LICENSE
+-rw-r--r--   0        0        0      873 2024-03-26 20:10:15.103476 bigeye_sdk-0.4.82/README.md
+-rw-r--r--   0        0        0     3727 2024-03-26 20:10:15.103593 bigeye_sdk-0.4.82/bigeye_sdk/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 20:10:15.103676 bigeye_sdk-0.4.82/bigeye_sdk/__version__.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.103753 bigeye_sdk-0.4.82/bigeye_sdk/authentication/__init__.py
+-rw-r--r--   0        0        0    20444 2024-05-29 15:10:38.210557 bigeye_sdk-0.4.82/bigeye_sdk/authentication/api_authentication.py
+-rw-r--r--   0        0        0    12761 2024-04-16 21:02:55.536986 bigeye_sdk-0.4.82/bigeye_sdk/authentication/config.py
+-rw-r--r--   0        0        0     1182 2024-03-26 20:10:15.104056 bigeye_sdk-0.4.82/bigeye_sdk/authentication/credentials.py
+-rw-r--r--   0        0        0      734 2024-03-26 20:10:15.104126 bigeye_sdk-0.4.82/bigeye_sdk/authentication/enums.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.104202 bigeye_sdk-0.4.82/bigeye_sdk/bigconfig_validation/__init__.py
+-rw-r--r--   0        0        0    11104 2024-05-24 16:34:30.566749 bigeye_sdk-0.4.82/bigeye_sdk/bigconfig_validation/big_config_reports.py
+-rw-r--r--   0        0        0     8116 2024-03-26 20:10:15.104508 bigeye_sdk-0.4.82/bigeye_sdk/bigconfig_validation/validation_context.py
+-rw-r--r--   0        0        0     1579 2024-03-26 20:10:15.104585 bigeye_sdk-0.4.82/bigeye_sdk/bigconfig_validation/validation_functions.py
+-rw-r--r--   0        0        0      736 2024-03-26 20:10:15.104656 bigeye_sdk-0.4.82/bigeye_sdk/bigconfig_validation/validation_models.py
+-rw-r--r--   0        0        0     9363 2024-05-14 19:46:32.468012 bigeye_sdk-0.4.82/bigeye_sdk/bigconfig_validation/yaml_model_base.py
+-rw-r--r--   0        0        0     3900 2024-03-26 20:10:15.104890 bigeye_sdk-0.4.82/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.104964 bigeye_sdk-0.4.82/bigeye_sdk/class_ext/__init__.py
+-rw-r--r--   0        0        0      233 2024-03-26 20:10:15.105053 bigeye_sdk-0.4.82/bigeye_sdk/class_ext/dataclass_ext.py
+-rw-r--r--   0        0        0      402 2024-03-26 20:10:15.105125 bigeye_sdk-0.4.82/bigeye_sdk/class_ext/enum_ext.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.105194 bigeye_sdk-0.4.82/bigeye_sdk/client/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 20:10:15.105276 bigeye_sdk-0.4.82/bigeye_sdk/client/base_client.py
+-rw-r--r--   0        0        0    42799 2024-05-29 15:10:38.211243 bigeye_sdk-0.4.82/bigeye_sdk/client/datawatch_client.py
+-rw-r--r--   0        0        0      201 2024-03-26 20:10:15.105478 bigeye_sdk-0.4.82/bigeye_sdk/client/enum.py
+-rw-r--r--   0        0        0    59247 2024-05-29 15:10:38.211797 bigeye_sdk-0.4.82/bigeye_sdk/client/generated_datawatch_client.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.105719 bigeye_sdk-0.4.82/bigeye_sdk/controller/__init__.py
+-rw-r--r--   0        0        0     2666 2024-03-26 20:10:15.105839 bigeye_sdk-0.4.82/bigeye_sdk/controller/delta_controller.py
+-rw-r--r--   0        0        0    15116 2024-05-29 15:10:14.885554 bigeye_sdk-0.4.82/bigeye_sdk/controller/lineage_controller.py
+-rw-r--r--   0        0        0     3209 2024-03-26 20:10:15.106039 bigeye_sdk-0.4.82/bigeye_sdk/controller/metric_controller.py
+-rw-r--r--   0        0        0    42347 2024-05-24 16:34:30.567656 bigeye_sdk-0.4.82/bigeye_sdk/controller/metric_suite_controller.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.106304 bigeye_sdk-0.4.82/bigeye_sdk/decorators/__init__.py
+-rw-r--r--   0        0        0      307 2024-03-26 20:10:15.106404 bigeye_sdk-0.4.82/bigeye_sdk/decorators/dataclass_decorators.py
+-rw-r--r--   0        0        0       97 2024-03-26 20:10:15.106520 bigeye_sdk-0.4.82/bigeye_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     1582 2024-03-26 20:10:15.106598 bigeye_sdk-0.4.82/bigeye_sdk/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.106671 bigeye_sdk-0.4.82/bigeye_sdk/functions/__init__.py
+-rw-r--r--   0        0        0     4469 2024-03-26 20:10:15.106799 bigeye_sdk-0.4.82/bigeye_sdk/functions/athena.py
+-rw-r--r--   0        0        0     5202 2024-03-26 20:10:15.106912 bigeye_sdk-0.4.82/bigeye_sdk/functions/aws.py
+-rw-r--r--   0        0        0     2450 2024-03-26 20:10:15.106994 bigeye_sdk-0.4.82/bigeye_sdk/functions/bigconfig_functions.py
+-rw-r--r--   0        0        0     3469 2024-03-26 20:10:15.107087 bigeye_sdk-0.4.82/bigeye_sdk/functions/casing.py
+-rw-r--r--   0        0        0     3215 2024-03-26 20:10:15.107178 bigeye_sdk-0.4.82/bigeye_sdk/functions/core_py_functs.py
+-rw-r--r--   0        0        0      370 2024-03-26 20:10:15.107269 bigeye_sdk-0.4.82/bigeye_sdk/functions/dbt.py
+-rw-r--r--   0        0        0     4580 2024-03-26 20:10:15.107401 bigeye_sdk-0.4.82/bigeye_sdk/functions/delta_functions.py
+-rw-r--r--   0        0        0     2814 2024-03-26 20:10:15.107482 bigeye_sdk-0.4.82/bigeye_sdk/functions/file_functs.py
+-rw-r--r--   0        0        0      706 2024-03-26 20:10:15.107556 bigeye_sdk-0.4.82/bigeye_sdk/functions/helpers.py
+-rw-r--r--   0        0        0      410 2024-03-26 20:10:15.107645 bigeye_sdk-0.4.82/bigeye_sdk/functions/issue_functions.py
+-rw-r--r--   0        0        0    21897 2024-03-26 20:10:15.107751 bigeye_sdk-0.4.82/bigeye_sdk/functions/metric_functions.py
+-rw-r--r--   0        0        0     2701 2024-03-26 20:10:15.107850 bigeye_sdk-0.4.82/bigeye_sdk/functions/metric_run_functions.py
+-rw-r--r--   0        0        0     1825 2024-05-24 16:34:30.567791 bigeye_sdk-0.4.82/bigeye_sdk/functions/notifications.py
+-rw-r--r--   0        0        0     1227 2024-03-26 20:10:15.107923 bigeye_sdk-0.4.82/bigeye_sdk/functions/s3.py
+-rw-r--r--   0        0        0     1796 2024-05-24 16:34:30.568083 bigeye_sdk-0.4.82/bigeye_sdk/functions/schema_change_functions.py
+-rw-r--r--   0        0        0     1676 2024-03-26 20:10:15.107998 bigeye_sdk-0.4.82/bigeye_sdk/functions/schema_functions.py
+-rw-r--r--   0        0        0     5377 2024-04-16 21:02:55.537393 bigeye_sdk-0.4.82/bigeye_sdk/functions/search_and_match_functions.py
+-rw-r--r--   0        0        0     4031 2024-03-26 20:10:15.108209 bigeye_sdk-0.4.82/bigeye_sdk/functions/table_functions.py
+-rw-r--r--   0        0        0     1701 2024-03-26 20:10:15.108284 bigeye_sdk-0.4.82/bigeye_sdk/functions/urlfuncts.py
+-rw-r--r--   0        0        0     2459 2024-04-16 21:02:55.537542 bigeye_sdk-0.4.82/bigeye_sdk/functions/version.py
+-rw-r--r--   0        0        0        0 2024-05-29 15:20:43.352638 bigeye_sdk-0.4.82/bigeye_sdk/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 15:20:43.352748 bigeye_sdk-0.4.82/bigeye_sdk/generated/com/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 15:20:43.352874 bigeye_sdk-0.4.82/bigeye_sdk/generated/com/bigeye/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 15:20:43.352963 bigeye_sdk-0.4.82/bigeye_sdk/generated/com/bigeye/models/__init__.py
+-rw-r--r--   0        0        0   287145 2024-05-29 15:20:43.353084 bigeye_sdk-0.4.82/bigeye_sdk/generated/com/bigeye/models/generated.py
+-rw-r--r--   0        0        0        0 2024-05-29 15:20:43.354410 bigeye_sdk-0.4.82/bigeye_sdk/generated/google/__init__.py
+-rw-r--r--   0        0        0    14816 2024-05-29 15:20:43.354537 bigeye_sdk-0.4.82/bigeye_sdk/generated/google/api.py
+-rw-r--r--   0        0        0      995 2024-05-24 16:34:30.568243 bigeye_sdk-0.4.82/bigeye_sdk/log/__init__.py
+-rw-r--r--   0        0        0        1 2024-03-26 20:10:15.109559 bigeye_sdk-0.4.82/bigeye_sdk/model/__init__.py
+-rw-r--r--   0        0        0      492 2024-03-26 20:10:15.109643 bigeye_sdk-0.4.82/bigeye_sdk/model/base_datawatch_facade.py
+-rw-r--r--   0        0        0    37552 2024-05-14 19:46:32.468851 bigeye_sdk-0.4.82/bigeye_sdk/model/big_config.py
+-rw-r--r--   0        0        0      778 2024-03-26 20:10:15.109855 bigeye_sdk-0.4.82/bigeye_sdk/model/collection_models.py
+-rw-r--r--   0        0        0      872 2024-03-26 20:10:15.109935 bigeye_sdk-0.4.82/bigeye_sdk/model/dbt_manifest.py
+-rw-r--r--   0        0        0     4518 2024-03-26 20:10:15.110060 bigeye_sdk-0.4.82/bigeye_sdk/model/dbt_schema.py
+-rw-r--r--   0        0        0     5521 2024-05-14 11:15:09.573368 bigeye_sdk-0.4.82/bigeye_sdk/model/delta_facade.py
+-rw-r--r--   0        0        0       89 2024-03-26 20:10:15.110260 bigeye_sdk-0.4.82/bigeye_sdk/model/enums.py
+-rw-r--r--   0        0        0     9459 2024-03-26 20:10:15.110414 bigeye_sdk-0.4.82/bigeye_sdk/model/metric_facade.py
+-rw-r--r--   0        0        0    11200 2024-05-24 16:34:30.568479 bigeye_sdk-0.4.82/bigeye_sdk/model/protobuf_enum_facade.py
+-rw-r--r--   0        0        0      221 2024-03-26 20:10:15.110628 bigeye_sdk-0.4.82/bigeye_sdk/model/protobuf_extensions.py
+-rw-r--r--   0        0        0    56944 2024-05-29 15:10:38.214021 bigeye_sdk-0.4.82/bigeye_sdk/model/protobuf_message_facade.py
+-rw-r--r--   0        0        0     6142 2024-05-24 16:34:30.568664 bigeye_sdk-0.4.82/bigeye_sdk/model/schema_change.py
+-rw-r--r--   0        0        0      865 2024-03-26 20:10:15.110847 bigeye_sdk-0.4.82/bigeye_sdk/model/sla_models.py
+-rw-r--r--   0        0        0     7599 2024-05-22 20:55:06.179834 bigeye_sdk-0.4.82/bigeye_sdk/serializable.py
+-rw-r--r--   0        0        0     3419 2024-05-29 15:11:06.358061 bigeye_sdk-0.4.82/pyproject.toml
+-rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.82/PKG-INFO
```

### Comparing `bigeye_sdk-0.4.81/LICENSE` & `bigeye_sdk-0.4.82/LICENSE`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/README.md` & `bigeye_sdk-0.4.82/README.md`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/__init__.py` & `bigeye_sdk-0.4.82/bigeye_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/authentication/api_authentication.py` & `bigeye_sdk-0.4.82/bigeye_sdk/authentication/api_authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 class ApiAuth(YamlSerializable):
 
     @abc.abstractmethod
     def get_auth_headers(self):
         pass
 
     @classmethod
-    def load(cls, auth_file: str, workspace: str = 'DEFAULT') -> ApiAuth:
+    def load(cls, auth_file: str = None, workspace: str = 'DEFAULT') -> ApiAuth:
         auth_file = cls.find_user_credentials(auth_file)
         if os.path.isfile(auth_file):
             if auth_file.lower().endswith('.json'):
                 return cls.load_from_json_file(auth_file)
             else:
                 return cls.load_from_ini_file(auth_file,workspace)
         else:
```

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/authentication/config.py` & `bigeye_sdk-0.4.82/bigeye_sdk/authentication/config.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/authentication/credentials.py` & `bigeye_sdk-0.4.82/bigeye_sdk/authentication/credentials.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/authentication/enums.py` & `bigeye_sdk-0.4.82/bigeye_sdk/authentication/enums.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/bigconfig_validation/big_config_reports.py` & `bigeye_sdk-0.4.82/bigeye_sdk/bigconfig_validation/big_config_reports.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/bigconfig_validation/validation_context.py` & `bigeye_sdk-0.4.82/bigeye_sdk/bigconfig_validation/validation_context.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/bigconfig_validation/validation_functions.py` & `bigeye_sdk-0.4.82/bigeye_sdk/bigconfig_validation/validation_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/bigconfig_validation/validation_models.py` & `bigeye_sdk-0.4.82/bigeye_sdk/bigconfig_validation/validation_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/bigconfig_validation/yaml_model_base.py` & `bigeye_sdk-0.4.82/bigeye_sdk/bigconfig_validation/yaml_model_base.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py` & `bigeye_sdk-0.4.82/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/client/datawatch_client.py` & `bigeye_sdk-0.4.82/bigeye_sdk/client/datawatch_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,16 @@
     CatalogAttributeResponse,
     GetCatalogAttributeRequest,
     UpsertDeltaRequest,
     Delta,
     UpsertDeltaResponse,
     OwnableType,
     SetObjectOwnerRequest,
-    ObjectOwnerResponse, SendDbtCoreRunInfoResponse, SendDbtCoreRunInfoRequest,
+    ObjectOwnerResponse, SendDbtCoreRunInfoResponse, SendDbtCoreRunInfoRequest, CustomRuleBulkRequest, BulkResponse,
+    CustomRulesThresholdType, MetricSchedule, CreateCustomRuleRequest, CustomRule, CustomRuleInfo,
 )
 from bigeye_sdk.log import get_logger
 from bigeye_sdk.model.delta_facade import SimpleDeltaConfiguration
 from bigeye_sdk.model.metric_facade import SimpleUpsertMetricRequest
 from bigeye_sdk.model.protobuf_enum_facade import SimpleCatalogEntityType
 from bigeye_sdk.model.protobuf_extensions import MetricDebugQueries
 
@@ -894,7 +895,71 @@
         request.run_results_json = run_results_json
         request.project_url = project_url
         request.job_url = job_url
         request.job_run_url = job_run_url
 
         response = self._call_datawatch(Method.POST, url=url, body=request.to_json())
         return SendDbtCoreRunInfoResponse().from_dict(response)
+
+    def bulk_run_rules(self, rule_ids: List[int]) -> BulkResponse:
+        """Run a list of rules"""
+        url = '/api/v1/custom-rules/bulk'
+        request = CustomRuleBulkRequest()
+        request.is_run = True
+        request.where.ids = rule_ids
+
+        response = self._call_datawatch(Method.POST, url=url, body=request.to_json())
+        return BulkResponse().from_dict(response)
+
+    def upsert_custom_rule(self,
+                           rule_id: Optional[int] = None,
+                           warehouse_id: Optional[int] = None,
+                           name: Optional[str] = None,
+                           sql: Optional[str] = None,
+                           threshold_type: Optional[CustomRulesThresholdType] = None,
+                           upper_threshold: Optional[float] = None,
+                           lower_threshold: Optional[float] = None,
+                           collection_ids: Optional[List[int]] = None,
+                           schedule: Optional[MetricSchedule] = None,
+                           owner_id: Optional[int] = None) -> CustomRuleInfo:
+        """Upsert a custom rule."""
+        if not rule_id or rule_id == 0:
+            if not warehouse_id or not name or not sql or not threshold_type:
+                raise Exception("For new rules, the warehouse_id, name, sql, and threshold_type fields are required.")
+
+            return self.create_custom_rule(
+                warehouse_id=warehouse_id,
+                name=name,
+                sql=sql,
+                threshold_type=threshold_type,
+                upper_threshold=upper_threshold,
+                lower_threshold=lower_threshold,
+                collection_ids=collection_ids,
+                schedule=schedule,
+                owner_id=owner_id
+            )
+
+        else:
+            custom_rule = self.get_rule_by_id(rule_id=rule_id).custom_rule
+
+            if name is not None:
+                custom_rule.name = name
+            if sql is not None:
+                custom_rule.sql = sql
+            if threshold_type is not None:
+                custom_rule.threshold_type = threshold_type
+            if upper_threshold is not None:
+                custom_rule.upper_threshold = upper_threshold
+            if lower_threshold is not None:
+                custom_rule.lower_threshold = lower_threshold
+            if collection_ids is not None:
+                custom_rule.collection_ids = collection_ids
+            if schedule is not None:
+                custom_rule.metric_schedule = schedule
+            if owner_id is not None:
+                owner = [u for u in self.get_users().users if u.id == owner_id][0]
+                custom_rule.owner = owner
+
+            return self.edit_custom_rule(
+                custom_rule=custom_rule,
+                rule_id=rule_id
+            )
```

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/client/generated_datawatch_client.py` & `bigeye_sdk-0.4.82/bigeye_sdk/client/generated_datawatch_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,15 +124,17 @@
     Delta,
     GetDeltaInfosResponse,
     RelationshipType,
     LineageEdgeV2,
     CreateLineageEdgeV2Request,
     GetColumnListRequest,
     GetColumnListResponse,
-    MetricInfo, GetTableListResponse, GetTableListRequest
+    MetricInfo, GetTableListResponse, GetTableListRequest, GetCustomRuleListResponse,
+    CreateCustomRuleRequest, CustomRule, MetricSchedule, CustomRulesThresholdType, UpdateCustomRuleRequest,
+    CustomRuleInfo, TimeInterval, TimeIntervalType
 )
 
 
 # create logger
 from bigeye_sdk.log import get_logger
 from bigeye_sdk.model.protobuf_enum_facade import SimpleFieldType, SimpleMetricTemplateParameterType, \
  SimpleWorkflowProcessingStatus, SimpleTableSortField, SimpleSortDirection
@@ -1389,7 +1391,100 @@
         return BulkResponse().from_dict(response)
 
     def get_columns(self, table_ids: List[int] = [], column_ids: List[int] = []) -> GetColumnListResponse:
         url = '/api/v1/columns/fetch'
         request = GetColumnListRequest(table_ids=table_ids, column_ids=column_ids)
         response = self._call_datawatch(Method.POST, url=url, body=request.to_json())
         return GetColumnListResponse().from_dict(response)
+
+    def create_custom_rule(self,
+                           warehouse_id: int,
+                           name: str,
+                           sql: str,
+                           threshold_type: CustomRulesThresholdType = None,
+                           upper_threshold: Optional[float] = None,
+                           lower_threshold: Optional[float] = None,
+                           collection_ids: Optional[List[int]] = None,
+                           schedule: Optional[MetricSchedule] = None,
+                           owner_id: Optional[int] = None) -> CustomRuleInfo:
+        """Create a new custom rule."""
+        url = '/api/v1/custom-rules'
+        rule = CustomRule()
+        rule.warehouse_id = warehouse_id
+        rule.name = name
+        rule.sql = sql
+        rule.threshold_type = threshold_type
+        rule.upper_threshold = upper_threshold
+        rule.lower_threshold = lower_threshold
+        rule.collection_ids = collection_ids or []
+
+        if not schedule:
+            rule.metric_schedule = MetricSchedule(
+                schedule_frequency=TimeInterval(
+                    interval_type=TimeIntervalType.HOURS_TIME_INTERVAL_TYPE,
+                    interval_value=24
+                )
+            )
+        else:
+            rule.metric_schedule = schedule
+
+        if owner_id:
+            owner = [u for u in self.get_users().users if u.id == owner_id][0]
+            rule.owner = owner
+
+        request = CreateCustomRuleRequest()
+        request.custom_rule = rule
+
+        # this is done so that default 0 values are not removed when converting to json
+        request_dict = request.to_dict()
+        request_dict["customRule"]["upperThreshold"] = upper_threshold
+        request_dict["customRule"]["lowerThreshold"] = lower_threshold
+        request_json = json.dumps(request_dict)
+
+        response = self._call_datawatch(Method.POST, url=url, body=request_json)
+        return CustomRuleInfo().from_dict(response)
+
+    def edit_custom_rule(self,
+                         custom_rule: CustomRule,
+                         rule_id: int) -> CustomRuleInfo:
+        """Edit an existing custom rule."""
+        url = f'/api/v1/custom-rules/{rule_id}'
+        request = UpdateCustomRuleRequest()
+        request.custom_rule = custom_rule
+        request.id = rule_id
+
+        # this is done so that default 0 values are not removed when converting to json
+        request_dict = request.to_dict()
+        request_dict["customRule"]["upperThreshold"] = request.custom_rule.upper_threshold
+        request_dict["customRule"]["lowerThreshold"] = request.custom_rule.lower_threshold
+        request_json = json.dumps(request_dict)
+
+        response = self._call_datawatch(Method.PUT, url=url, body=request_json)
+        return CustomRuleInfo().from_dict(response)
+
+    def get_rule_by_id(self, rule_id: int) -> CustomRuleInfo:
+        """Get a single rule by ID."""
+        url = f'/api/v1/custom-rules/{rule_id}'
+        response = self._call_datawatch(Method.GET, url=url)
+        return CustomRuleInfo().from_dict(response)
+
+    def get_rules(self, warehouse_id: int) -> GetCustomRuleListResponse:
+        """Get all rules for a given warehouse"""
+        url = f'/api/v1/custom-rules/warehouse/{warehouse_id}'
+        response = self._call_datawatch(Method.GET, url=url)
+
+        rlist_current = GetCustomRuleListResponse().from_dict(response)
+        rlist_total = GetCustomRuleListResponse()
+        rlist_total.custom_rules.extend(rlist_current.custom_rules)
+
+        while rlist_current.pagination_info.next_cursor:
+            response.page_cursor = rlist_current.pagination_info.next_cursor
+            response = self._call_datawatch(Method.POST, url=url, body=response.to_json())
+            rlist_current = GetCustomRuleListResponse().from_dict(response)
+            rlist_total.custom_rules.extend(rlist_current.custom_rules)
+
+        return rlist_total
+
+    def delete_custom_rule(self, id: int):
+        """Delete a custom rule."""
+        url = f'/api/v1/custom-rules/{id}'
+        return self._call_datawatch(Method.DELETE, url=url)
```

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/controller/delta_controller.py` & `bigeye_sdk-0.4.82/bigeye_sdk/controller/delta_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/controller/lineage_controller.py` & `bigeye_sdk-0.4.82/bigeye_sdk/controller/lineage_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/controller/metric_controller.py` & `bigeye_sdk-0.4.82/bigeye_sdk/controller/metric_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/controller/metric_suite_controller.py` & `bigeye_sdk-0.4.82/bigeye_sdk/controller/metric_suite_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/exceptions/exceptions.py` & `bigeye_sdk-0.4.82/bigeye_sdk/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/athena.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/athena.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/aws.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/aws.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/bigconfig_functions.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/bigconfig_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/casing.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/casing.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/core_py_functs.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/core_py_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/delta_functions.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/delta_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/file_functs.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/file_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/helpers.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/helpers.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/metric_functions.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/metric_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/metric_run_functions.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/metric_run_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/notifications.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/notifications.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/s3.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/s3.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/schema_change_functions.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/schema_change_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/schema_functions.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/schema_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/search_and_match_functions.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/search_and_match_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/table_functions.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/table_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/urlfuncts.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/urlfuncts.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/functions/version.py` & `bigeye_sdk-0.4.82/bigeye_sdk/functions/version.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/generated/com/bigeye/models/generated.py` & `bigeye_sdk-0.4.82/bigeye_sdk/generated/com/bigeye/models/generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1242,15 +1242,15 @@
     ignore_fields: bool = betterproto.bool_field(7)
     workspace_id: int = betterproto.int32_field(8)
     include_data_node_ids: bool = betterproto.bool_field(9)
 
 
 @dataclass
 class MetricHistoryDataPoint(betterproto.Message):
-    epoch_seconds: int = betterproto.int32_field(1)
+    epoch_seconds: int = betterproto.int64_field(1)
     value: float = betterproto.double_field(2)
     lower_threshold: float = betterproto.double_field(3)
     upper_threshold: float = betterproto.double_field(4)
     run_status: "MetricRunStatus" = betterproto.enum_field(5)
     should_use_for_training: bool = betterproto.bool_field(6)
 
 
@@ -4191,14 +4191,19 @@
 
 @dataclass
 class SinglePathParamWorkspaceIdRequest(betterproto.Message):
     workspace_id: int = betterproto.int32_field(1)
 
 
 @dataclass
+class SinglePathParamWarehouseIdRequest(betterproto.Message):
+    warehouse_id: int = betterproto.int32_field(1)
+
+
+@dataclass
 class WorkspaceListResponse(betterproto.Message):
     workspaces: List["Workspace"] = betterproto.message_field(1)
 
 
 @dataclass
 class CreateOrUpdateWorkspaceRequest(betterproto.Message):
     name: str = betterproto.string_field(1)
@@ -4207,14 +4212,40 @@
 @dataclass
 class UpdateWorkspaceRequestWrapper(betterproto.Message):
     workspace_id: int = betterproto.int32_field(1)
     request: "CreateOrUpdateWorkspaceRequest" = betterproto.message_field(2)
 
 
 @dataclass
+class PersonalApiKeyInfo(betterproto.Message):
+    id: int = betterproto.int32_field(1)
+    name: str = betterproto.string_field(2)
+    description: str = betterproto.string_field(3)
+    created_at: int = betterproto.int64_field(4)
+    last_used_at: int = betterproto.int64_field(5)
+
+
+@dataclass
+class CreatePersonalApiKeyRequest(betterproto.Message):
+    name: str = betterproto.string_field(1)
+    description: str = betterproto.string_field(2)
+
+
+@dataclass
+class CreatePersonalApiKeyResponse(betterproto.Message):
+    info: "PersonalApiKeyInfo" = betterproto.message_field(1)
+    api_key: str = betterproto.string_field(2)
+
+
+@dataclass
+class ListPersonalApiKeyResponse(betterproto.Message):
+    keys: List["PersonalApiKeyInfo"] = betterproto.message_field(1)
+
+
+@dataclass
 class SinglePathParamRoleIdRequest(betterproto.Message):
     role_id: int = betterproto.int32_field(1)
 
 
 @dataclass
 class RevisionInfo(betterproto.Message):
     type: "RevisionType" = betterproto.enum_field(1)
@@ -4742,14 +4773,19 @@
 @dataclass
 class GetCustomRuleListResponse(betterproto.Message):
     custom_rules: List["CustomRuleInfo"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
 
 @dataclass
+class SinglePathParamCustomRuleIdRequest(betterproto.Message):
+    custom_rule_id: int = betterproto.int32_field(1)
+
+
+@dataclass
 class MetricRunHistoryProviderRequest(betterproto.Message):
     metric_identifier: "MetricIdentifier" = betterproto.message_field(1)
 
 
 @dataclass
 class MetricConfigurationProviderRequest(betterproto.Message):
     metric_id: int = betterproto.int32_field(1)
@@ -4813,14 +4849,20 @@
     )
     metric_configuration_provider_request: "MetricConfigurationProviderRequest" = (
         betterproto.message_field(2)
     )
 
 
 @dataclass
+class TrainingRequest(betterproto.Message):
+    monocle_model_request: "MonocleModelRequest" = betterproto.message_field(1)
+    retries: int = betterproto.int32_field(2)
+
+
+@dataclass
 class AutoThresholdRequestV2(betterproto.Message):
     monocle_model_request: "MonocleModelRequest" = betterproto.message_field(1)
     prediction_epoch_seconds: List[int] = betterproto.int32_field(2)
     force_online: bool = betterproto.bool_field(3)
 
 
 @dataclass
@@ -8084,14 +8126,113 @@
         return await self._unary_unary(
             "/com.bigeye.models.generated.RoleService/GetRole",
             request,
             RoleV2,
         )
 
 
+class CustomRuleServiceStub(betterproto.ServiceStub):
+    """Custom Rules"""
+
+    async def create_custom_rule(
+        self, *, custom_rule: Optional["CustomRule"] = None
+    ) -> CustomRuleInfo:
+        """Create a custom rule"""
+
+        request = CreateCustomRuleRequest()
+        if custom_rule is not None:
+            request.custom_rule = custom_rule
+
+        return await self._unary_unary(
+            "/com.bigeye.models.generated.CustomRuleService/CreateCustomRule",
+            request,
+            CustomRuleInfo,
+        )
+
+    async def update_custom_rule(
+        self, *, id: int = 0, custom_rule: Optional["CustomRule"] = None
+    ) -> CustomRuleInfo:
+        """Update a custom rule"""
+
+        request = UpdateCustomRuleRequest()
+        request.id = id
+        if custom_rule is not None:
+            request.custom_rule = custom_rule
+
+        return await self._unary_unary(
+            "/com.bigeye.models.generated.CustomRuleService/UpdateCustomRule",
+            request,
+            CustomRuleInfo,
+        )
+
+    async def get_custom_rule(self, *, custom_rule_id: int = 0) -> CustomRuleInfo:
+        """Get a custom rule"""
+
+        request = SinglePathParamCustomRuleIdRequest()
+        request.custom_rule_id = custom_rule_id
+
+        return await self._unary_unary(
+            "/com.bigeye.models.generated.CustomRuleService/GetCustomRule",
+            request,
+            CustomRuleInfo,
+        )
+
+    async def run_custom_rule(self, *, custom_rule_id: int = 0) -> CustomRuleInfo:
+        """Run a custom rule"""
+
+        request = SinglePathParamCustomRuleIdRequest()
+        request.custom_rule_id = custom_rule_id
+
+        return await self._unary_unary(
+            "/com.bigeye.models.generated.CustomRuleService/RunCustomRule",
+            request,
+            CustomRuleInfo,
+        )
+
+    async def delete_custom_rule(self, *, custom_rule_id: int = 0) -> Empty:
+        """Delete a custom rule"""
+
+        request = SinglePathParamCustomRuleIdRequest()
+        request.custom_rule_id = custom_rule_id
+
+        return await self._unary_unary(
+            "/com.bigeye.models.generated.CustomRuleService/DeleteCustomRule",
+            request,
+            Empty,
+        )
+
+    async def get_custom_rules_for_collection(
+        self, *, collection_id: int = 0
+    ) -> GetCustomRuleListResponse:
+        """Get all custom rules for a collection"""
+
+        request = SinglePathParamCollectionIdRequest()
+        request.collection_id = collection_id
+
+        return await self._unary_unary(
+            "/com.bigeye.models.generated.CustomRuleService/GetCustomRulesForCollection",
+            request,
+            GetCustomRuleListResponse,
+        )
+
+    async def get_custom_rules_for_warehouse(
+        self, *, warehouse_id: int = 0
+    ) -> GetCustomRuleListResponse:
+        """Get all custom rules for a warehouse"""
+
+        request = SinglePathParamWarehouseIdRequest()
+        request.warehouse_id = warehouse_id
+
+        return await self._unary_unary(
+            "/com.bigeye.models.generated.CustomRuleService/GetCustomRulesForWarehouse",
+            request,
+            GetCustomRuleListResponse,
+        )
+
+
 class GroupServiceStub(betterproto.ServiceStub):
     """Groups"""
 
     async def create_group(
         self, *, name: str = "", idp_groups: List[str] = []
     ) -> Group:
         """Create a group"""
```

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/generated/google/api.py` & `bigeye_sdk-0.4.82/bigeye_sdk/generated/google/api.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/log/__init__.py` & `bigeye_sdk-0.4.82/bigeye_sdk/log/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/model/big_config.py` & `bigeye_sdk-0.4.82/bigeye_sdk/model/big_config.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/model/collection_models.py` & `bigeye_sdk-0.4.82/bigeye_sdk/model/collection_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/model/dbt_manifest.py` & `bigeye_sdk-0.4.82/bigeye_sdk/model/dbt_manifest.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/model/dbt_schema.py` & `bigeye_sdk-0.4.82/bigeye_sdk/model/dbt_schema.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/model/delta_facade.py` & `bigeye_sdk-0.4.82/bigeye_sdk/model/delta_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/model/metric_facade.py` & `bigeye_sdk-0.4.82/bigeye_sdk/model/metric_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/model/protobuf_enum_facade.py` & `bigeye_sdk-0.4.82/bigeye_sdk/model/protobuf_enum_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/model/protobuf_message_facade.py` & `bigeye_sdk-0.4.82/bigeye_sdk/model/protobuf_message_facade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1285,8 +1285,7 @@
         if self.rct_overrides:
             if len(self.rct_overrides) == 1 and self.rct_overrides[0] == "FULL_SCAN":
                 builder.rct_overrides = ["bigeye-no-rct"]
             else:
                 builder.rct_overrides = self.rct_overrides
 
         return builder
-
```

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/model/schema_change.py` & `bigeye_sdk-0.4.82/bigeye_sdk/model/schema_change.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/model/sla_models.py` & `bigeye_sdk-0.4.82/bigeye_sdk/model/sla_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/bigeye_sdk/serializable.py` & `bigeye_sdk-0.4.82/bigeye_sdk/serializable.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.81/pyproject.toml` & `bigeye_sdk-0.4.82/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bigeye-sdk"
-version = "0.4.81"
+version = "0.4.82"
 description = "Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically."
 license = "Proprietary"
 authors = ["Bigeye <support@bigeye.com>"]
 readme = "README.md"
 homepage = "https://docs.bigeye.com/docs"
 
 [[tool.poetry.source]]
@@ -34,14 +34,15 @@
 types-PyYAML = "^6.0.11"
 boto3 = "^1.26.7"
 botocore = "^1.29.7"
 rich = ">=12.4.4"
 typer = "^0.12.3"
 secretstorage = "^3.3.3"
 slack_sdk = "^3.2.7"
+deprecated = "^1.2.14"
 
 [tool.poetry.dev-dependencies]
 markupsafe = "^2.0.1"
 grpcio = "^1.48.1"
 grpcio-tools = "^1.48.1"
 poethepoet = "^0.24.3"
 pylint = "^2.15.2"
```

### Comparing `bigeye_sdk-0.4.81/PKG-INFO` & `bigeye_sdk-0.4.82/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigeye-sdk
-Version: 0.4.81
+Version: 0.4.82
 Summary: Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically.
 Home-page: https://docs.bigeye.com/docs
 License: Proprietary
 Author: Bigeye
 Author-email: support@bigeye.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: Other/Proprietary License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: betterproto[compiler] (>=1.2.5,<2.0.0)
 Requires-Dist: boto3 (>=1.26.7,<2.0.0)
 Requires-Dist: botocore (>=1.29.7,<2.0.0)
+Requires-Dist: deprecated (>=1.2.14,<2.0.0)
 Requires-Dist: grpclib (>=0.4.2,<0.5.0)
 Requires-Dist: keyring (>=24.3.1,<25.0.0)
 Requires-Dist: lz4 (>=4.0.1,<5.0.0)
 Requires-Dist: pycryptodomex (>=3.20.0,<4.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: pydantic-yaml (>=1.0.0,<2.0.0)
 Requires-Dist: rapidfuzz (>=3.1.1,<4.0.0)
```

