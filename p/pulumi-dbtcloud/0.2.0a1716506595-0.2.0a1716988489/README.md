# Comparing `tmp/pulumi_dbtcloud-0.2.0a1716506595.tar.gz` & `tmp/pulumi_dbtcloud-0.2.0a1716988489.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_dbtcloud-0.2.0a1716506595.tar", last modified: Thu May 23 23:41:21 2024, max compression
+gzip compressed data, was "pulumi_dbtcloud-0.2.0a1716988489.tar", last modified: Wed May 29 13:17:16 2024, max compression
```

## Comparing `pulumi_dbtcloud-0.2.0a1716506595.tar` & `pulumi_dbtcloud-0.2.0a1716988489.tar`

### file list

```diff
@@ -1,69 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:41:21.983166 pulumi_dbtcloud-0.2.0a1716506595/
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-23 23:41:21.983166 pulumi_dbtcloud-0.2.0a1716506595/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:41:21.983166 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    58952 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/big_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/big_query_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:41:21.983166 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    44015 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/databricks_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    29643 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    14311 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/environment_variable_job_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    14286 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/extended_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    24535 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/fabric_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26070 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/fabric_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_azure_dev_ops_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_azure_dev_ops_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_big_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_big_query_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_databricks_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_extended_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_postgres_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_service_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_snowflake_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    15719 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    68381 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/license_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    29421 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22244 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/postgres_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project_artefacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    38478 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/service_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    28611 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/snowflake_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    21154 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:41:21.983166 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-23 23:41:21.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-23 23:41:21.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:41:21.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 23:41:21.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 23:41:21.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 23:41:21.983166 pulumi_dbtcloud-0.2.0a1716506595/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:16.172694 pulumi_dbtcloud-0.2.0a1716988489/
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-29 13:17:16.172694 pulumi_dbtcloud-0.2.0a1716988489/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:16.172694 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59512 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/big_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/big_query_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:16.172694 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46115 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21215 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/databricks_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30802 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/environment_variable_job_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/extended_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25219 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/fabric_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28372 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/fabric_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_azure_dev_ops_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_azure_dev_ops_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_big_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_big_query_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_databricks_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_extended_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_postgres_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_service_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_snowflake_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15306 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/group_partial_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69766 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/license_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30185 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16495 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29966 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/partial_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22632 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/postgres_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project_artefacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    47259 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15033 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/service_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29051 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/snowflake_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21500 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:16.172694 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-29 13:17:16.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-29 13:17:16.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:17:16.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 13:17:16.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 13:17:16.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:17:16.176694 pulumi_dbtcloud-0.2.0a1716988489/setup.cfg
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/PKG-INFO` & `pulumi_dbtcloud-0.2.0a1716988489/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_dbtcloud
-Version: 0.2.0a1716506595
+Version: 0.2.0a1716988489
 Summary: A Pulumi package for creating and managing dbt Cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-dbtcloud
 Keywords: pulumi,dbtcloud,dbt,cloud,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/README.md` & `pulumi_dbtcloud-0.2.0a1716988489/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/__init__.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from .get_azure_dev_ops_repository import *
 from .get_big_query_connection import *
 from .get_big_query_credential import *
 from .get_connection import *
 from .get_databricks_credential import *
 from .get_environment import *
 from .get_environment_variable import *
+from .get_environments import *
 from .get_extended_attributes import *
 from .get_group import *
 from .get_group_users import *
 from .get_job import *
 from .get_notification import *
 from .get_postgres_credential import *
 from .get_privatelink_endpoint import *
@@ -34,17 +35,19 @@
 from .get_repository import *
 from .get_service_token import *
 from .get_snowflake_credential import *
 from .get_user import *
 from .get_user_groups import *
 from .get_webhook import *
 from .group import *
+from .group_partial_permissions import *
 from .job import *
 from .license_map import *
 from .notification import *
+from .partial_notification import *
 from .postgres_credential import *
 from .project import *
 from .project_artefacts import *
 from .project_connection import *
 from .project_repository import *
 from .provider import *
 from .repository import *
@@ -151,14 +154,22 @@
   "fqn": "pulumi_dbtcloud",
   "classes": {
    "dbtcloud:index/group:Group": "Group"
   }
  },
  {
   "pkg": "dbtcloud",
+  "mod": "index/groupPartialPermissions",
+  "fqn": "pulumi_dbtcloud",
+  "classes": {
+   "dbtcloud:index/groupPartialPermissions:GroupPartialPermissions": "GroupPartialPermissions"
+  }
+ },
+ {
+  "pkg": "dbtcloud",
   "mod": "index/job",
   "fqn": "pulumi_dbtcloud",
   "classes": {
    "dbtcloud:index/job:Job": "Job"
   }
  },
  {
@@ -175,14 +186,22 @@
   "fqn": "pulumi_dbtcloud",
   "classes": {
    "dbtcloud:index/notification:Notification": "Notification"
   }
  },
  {
   "pkg": "dbtcloud",
+  "mod": "index/partialNotification",
+  "fqn": "pulumi_dbtcloud",
+  "classes": {
+   "dbtcloud:index/partialNotification:PartialNotification": "PartialNotification"
+  }
+ },
+ {
+  "pkg": "dbtcloud",
   "mod": "index/postgresCredential",
   "fqn": "pulumi_dbtcloud",
   "classes": {
    "dbtcloud:index/postgresCredential:PostgresCredential": "PostgresCredential"
   }
  },
  {
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/_inputs.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/_inputs.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
     'GroupGroupPermissionArgs',
+    'GroupPartialPermissionsGroupPermissionArgs',
     'JobJobCompletionTriggerConditionArgs',
     'ServiceTokenServiceTokenPermissionArgs',
 ]
 
 @pulumi.input_type
 class GroupGroupPermissionArgs:
     def __init__(__self__, *,
@@ -63,14 +64,67 @@
         """
         return pulumi.get(self, "project_id")
 
     @project_id.setter
     def project_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "project_id", value)
 
+
+@pulumi.input_type
+class GroupPartialPermissionsGroupPermissionArgs:
+    def __init__(__self__, *,
+                 all_projects: pulumi.Input[bool],
+                 permission_set: pulumi.Input[str],
+                 project_id: Optional[pulumi.Input[int]] = None):
+        """
+        :param pulumi.Input[bool] all_projects: Whether access should be provided for all projects or not.
+        :param pulumi.Input[str] permission_set: Set of permissions to apply. The permissions allowed are the same as the ones for the `Group` resource.
+        :param pulumi.Input[int] project_id: Project ID to apply this permission to for this group.
+        """
+        pulumi.set(__self__, "all_projects", all_projects)
+        pulumi.set(__self__, "permission_set", permission_set)
+        if project_id is not None:
+            pulumi.set(__self__, "project_id", project_id)
+
+    @property
+    @pulumi.getter(name="allProjects")
+    def all_projects(self) -> pulumi.Input[bool]:
+        """
+        Whether access should be provided for all projects or not.
+        """
+        return pulumi.get(self, "all_projects")
+
+    @all_projects.setter
+    def all_projects(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "all_projects", value)
+
+    @property
+    @pulumi.getter(name="permissionSet")
+    def permission_set(self) -> pulumi.Input[str]:
+        """
+        Set of permissions to apply. The permissions allowed are the same as the ones for the `Group` resource.
+        """
+        return pulumi.get(self, "permission_set")
+
+    @permission_set.setter
+    def permission_set(self, value: pulumi.Input[str]):
+        pulumi.set(self, "permission_set", value)
+
+    @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        Project ID to apply this permission to for this group.
+        """
+        return pulumi.get(self, "project_id")
+
+    @project_id.setter
+    def project_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "project_id", value)
+
 
 @pulumi.input_type
 class JobJobCompletionTriggerConditionArgs:
     def __init__(__self__, *,
                  job_id: pulumi.Input[int],
                  project_id: pulumi.Input[int],
                  statuses: pulumi.Input[Sequence[pulumi.Input[str]]]):
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/_utilities.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/big_query_connection.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/big_query_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -850,15 +850,14 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         my_connection = dbtcloud.BigQueryConnection("my_connection",
             project_id=dbt_project["id"],
             name="Project Name",
             type="bigquery",
             is_active=True,
             gcp_project_id="my-gcp-project-id",
             timeout_seconds=100,
@@ -890,14 +889,34 @@
             retries=3,
             application_id="oauth_application_id",
             application_secret="oauth_secret_id")
         ```
 
         ## Import
 
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_bigquery_connection.my_connection
+
+          id = "project_id:connection_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_bigquery_connection.my_connection
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
+
         ```sh
         $ pulumi import dbtcloud:index/bigQueryConnection:BigQueryConnection my_connection "project_id:connection_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/bigQueryConnection:BigQueryConnection my_connection 12345:6789
         ```
@@ -940,15 +959,14 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         my_connection = dbtcloud.BigQueryConnection("my_connection",
             project_id=dbt_project["id"],
             name="Project Name",
             type="bigquery",
             is_active=True,
             gcp_project_id="my-gcp-project-id",
             timeout_seconds=100,
@@ -980,14 +998,34 @@
             retries=3,
             application_id="oauth_application_id",
             application_secret="oauth_secret_id")
         ```
 
         ## Import
 
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_bigquery_connection.my_connection
+
+          id = "project_id:connection_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_bigquery_connection.my_connection
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
+
         ```sh
         $ pulumi import dbtcloud:index/bigQueryConnection:BigQueryConnection my_connection "project_id:connection_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/bigQueryConnection:BigQueryConnection my_connection 12345:6789
         ```
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/big_query_credential.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/big_query_credential.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,23 +181,42 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         my_credential = dbtcloud.BigQueryCredential("my_credential",
             project_id=dbt_project["id"],
             dataset="my_bq_dataset",
             num_threads=16)
         ```
 
         ## Import
 
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_bigquery_credential.my_credential
+
+          id = "project_id:credential_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_bigquery_credential.my_credential
+
+          id = "12345:5678"
+
+        }
+
+        using the older import command
+
         ```sh
         $ pulumi import dbtcloud:index/bigQueryCredential:BigQueryCredential my_credential "project_id:credential_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/bigQueryCredential:BigQueryCredential my_credential 12345:5678
         ```
@@ -218,23 +237,42 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         my_credential = dbtcloud.BigQueryCredential("my_credential",
             project_id=dbt_project["id"],
             dataset="my_bq_dataset",
             num_threads=16)
         ```
 
         ## Import
 
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_bigquery_credential.my_credential
+
+          id = "project_id:credential_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_bigquery_credential.my_credential
+
+          id = "12345:5678"
+
+        }
+
+        using the older import command
+
         ```sh
         $ pulumi import dbtcloud:index/bigQueryCredential:BigQueryCredential my_credential "project_id:credential_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/bigQueryCredential:BigQueryCredential my_credential 12345:5678
         ```
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/config/__init__.pyi` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/config/vars.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/connection.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,29 +33,29 @@
                  tunnel_enabled: Optional[pulumi.Input[bool]] = None,
                  warehouse: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Connection resource.
         :param pulumi.Input[str] database: Database name for the connection
         :param pulumi.Input[int] project_id: Project ID to create the connection in
         :param pulumi.Input[str] type: The type of connection
-        :param pulumi.Input[str] account: Account name for the connection
-        :param pulumi.Input[bool] allow_keep_alive: Whether or not the connection should allow client session keep alive
-        :param pulumi.Input[bool] allow_sso: Whether or not the connection should allow SSO
-        :param pulumi.Input[str] catalog: Catalog name if Unity Catalog is enabled in your Databricks workspace
+        :param pulumi.Input[str] account: Account name for the connection (for Snowflake)
+        :param pulumi.Input[bool] allow_keep_alive: Whether or not the connection should allow client session keep alive (for Snowflake)
+        :param pulumi.Input[bool] allow_sso: Whether or not the connection should allow SSO (for Snowflake)
+        :param pulumi.Input[str] catalog: Catalog name if Unity Catalog is enabled in your Databricks workspace (for Databricks)
         :param pulumi.Input[str] host_name: Host name for the connection, including Databricks cluster
-        :param pulumi.Input[str] http_path: The HTTP path of the Databricks cluster or SQL warehouse
+        :param pulumi.Input[str] http_path: The HTTP path of the Databricks cluster or SQL warehouse (for Databricks)
         :param pulumi.Input[bool] is_active: Whether the connection is active
         :param pulumi.Input[str] name: Connection name
-        :param pulumi.Input[str] oauth_client_id: OAuth client identifier
-        :param pulumi.Input[str] oauth_client_secret: OAuth client secret
+        :param pulumi.Input[str] oauth_client_id: OAuth client identifier (for Snowflake and Databricks)
+        :param pulumi.Input[str] oauth_client_secret: OAuth client secret (for Snowflake and Databricks)
         :param pulumi.Input[int] port: Port number to connect via
         :param pulumi.Input[str] private_link_endpoint_id: The ID of the PrivateLink connection. This ID can be found using the `privatelink_endpoint` data source
-        :param pulumi.Input[str] role: Role name for the connection
+        :param pulumi.Input[str] role: Role name for the connection (for Snowflake)
         :param pulumi.Input[bool] tunnel_enabled: Whether or not tunneling should be enabled on your database connection
-        :param pulumi.Input[str] warehouse: Warehouse name for the connection
+        :param pulumi.Input[str] warehouse: Warehouse name for the connection (for Snowflake)
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "project_id", project_id)
         pulumi.set(__self__, "type", type)
         if account is not None:
             pulumi.set(__self__, "account", account)
         if allow_keep_alive is not None:
@@ -123,51 +123,51 @@
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def account(self) -> Optional[pulumi.Input[str]]:
         """
-        Account name for the connection
+        Account name for the connection (for Snowflake)
         """
         return pulumi.get(self, "account")
 
     @account.setter
     def account(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "account", value)
 
     @property
     @pulumi.getter(name="allowKeepAlive")
     def allow_keep_alive(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether or not the connection should allow client session keep alive
+        Whether or not the connection should allow client session keep alive (for Snowflake)
         """
         return pulumi.get(self, "allow_keep_alive")
 
     @allow_keep_alive.setter
     def allow_keep_alive(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_keep_alive", value)
 
     @property
     @pulumi.getter(name="allowSso")
     def allow_sso(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether or not the connection should allow SSO
+        Whether or not the connection should allow SSO (for Snowflake)
         """
         return pulumi.get(self, "allow_sso")
 
     @allow_sso.setter
     def allow_sso(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_sso", value)
 
     @property
     @pulumi.getter
     def catalog(self) -> Optional[pulumi.Input[str]]:
         """
-        Catalog name if Unity Catalog is enabled in your Databricks workspace
+        Catalog name if Unity Catalog is enabled in your Databricks workspace (for Databricks)
         """
         return pulumi.get(self, "catalog")
 
     @catalog.setter
     def catalog(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "catalog", value)
 
@@ -183,15 +183,15 @@
     def host_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "host_name", value)
 
     @property
     @pulumi.getter(name="httpPath")
     def http_path(self) -> Optional[pulumi.Input[str]]:
         """
-        The HTTP path of the Databricks cluster or SQL warehouse
+        The HTTP path of the Databricks cluster or SQL warehouse (for Databricks)
         """
         return pulumi.get(self, "http_path")
 
     @http_path.setter
     def http_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "http_path", value)
 
@@ -219,27 +219,27 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="oauthClientId")
     def oauth_client_id(self) -> Optional[pulumi.Input[str]]:
         """
-        OAuth client identifier
+        OAuth client identifier (for Snowflake and Databricks)
         """
         return pulumi.get(self, "oauth_client_id")
 
     @oauth_client_id.setter
     def oauth_client_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "oauth_client_id", value)
 
     @property
     @pulumi.getter(name="oauthClientSecret")
     def oauth_client_secret(self) -> Optional[pulumi.Input[str]]:
         """
-        OAuth client secret
+        OAuth client secret (for Snowflake and Databricks)
         """
         return pulumi.get(self, "oauth_client_secret")
 
     @oauth_client_secret.setter
     def oauth_client_secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "oauth_client_secret", value)
 
@@ -267,15 +267,15 @@
     def private_link_endpoint_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "private_link_endpoint_id", value)
 
     @property
     @pulumi.getter
     def role(self) -> Optional[pulumi.Input[str]]:
         """
-        Role name for the connection
+        Role name for the connection (for Snowflake)
         """
         return pulumi.get(self, "role")
 
     @role.setter
     def role(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "role", value)
 
@@ -291,15 +291,15 @@
     def tunnel_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "tunnel_enabled", value)
 
     @property
     @pulumi.getter
     def warehouse(self) -> Optional[pulumi.Input[str]]:
         """
-        Warehouse name for the connection
+        Warehouse name for the connection (for Snowflake)
         """
         return pulumi.get(self, "warehouse")
 
     @warehouse.setter
     def warehouse(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "warehouse", value)
 
@@ -325,34 +325,34 @@
                  project_id: Optional[pulumi.Input[int]] = None,
                  role: Optional[pulumi.Input[str]] = None,
                  tunnel_enabled: Optional[pulumi.Input[bool]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  warehouse: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Connection resources.
-        :param pulumi.Input[str] account: Account name for the connection
-        :param pulumi.Input[int] adapter_id: Adapter id created for the Databricks connection
-        :param pulumi.Input[bool] allow_keep_alive: Whether or not the connection should allow client session keep alive
-        :param pulumi.Input[bool] allow_sso: Whether or not the connection should allow SSO
-        :param pulumi.Input[str] catalog: Catalog name if Unity Catalog is enabled in your Databricks workspace
+        :param pulumi.Input[str] account: Account name for the connection (for Snowflake)
+        :param pulumi.Input[int] adapter_id: Adapter id created for the Databricks connection (for Databricks)
+        :param pulumi.Input[bool] allow_keep_alive: Whether or not the connection should allow client session keep alive (for Snowflake)
+        :param pulumi.Input[bool] allow_sso: Whether or not the connection should allow SSO (for Snowflake)
+        :param pulumi.Input[str] catalog: Catalog name if Unity Catalog is enabled in your Databricks workspace (for Databricks)
         :param pulumi.Input[int] connection_id: Connection Identifier
         :param pulumi.Input[str] database: Database name for the connection
         :param pulumi.Input[str] host_name: Host name for the connection, including Databricks cluster
-        :param pulumi.Input[str] http_path: The HTTP path of the Databricks cluster or SQL warehouse
+        :param pulumi.Input[str] http_path: The HTTP path of the Databricks cluster or SQL warehouse (for Databricks)
         :param pulumi.Input[bool] is_active: Whether the connection is active
         :param pulumi.Input[str] name: Connection name
-        :param pulumi.Input[str] oauth_client_id: OAuth client identifier
-        :param pulumi.Input[str] oauth_client_secret: OAuth client secret
+        :param pulumi.Input[str] oauth_client_id: OAuth client identifier (for Snowflake and Databricks)
+        :param pulumi.Input[str] oauth_client_secret: OAuth client secret (for Snowflake and Databricks)
         :param pulumi.Input[int] port: Port number to connect via
         :param pulumi.Input[str] private_link_endpoint_id: The ID of the PrivateLink connection. This ID can be found using the `privatelink_endpoint` data source
         :param pulumi.Input[int] project_id: Project ID to create the connection in
-        :param pulumi.Input[str] role: Role name for the connection
+        :param pulumi.Input[str] role: Role name for the connection (for Snowflake)
         :param pulumi.Input[bool] tunnel_enabled: Whether or not tunneling should be enabled on your database connection
         :param pulumi.Input[str] type: The type of connection
-        :param pulumi.Input[str] warehouse: Warehouse name for the connection
+        :param pulumi.Input[str] warehouse: Warehouse name for the connection (for Snowflake)
         """
         if account is not None:
             pulumi.set(__self__, "account", account)
         if adapter_id is not None:
             pulumi.set(__self__, "adapter_id", adapter_id)
         if allow_keep_alive is not None:
             pulumi.set(__self__, "allow_keep_alive", allow_keep_alive)
@@ -391,63 +391,63 @@
         if warehouse is not None:
             pulumi.set(__self__, "warehouse", warehouse)
 
     @property
     @pulumi.getter
     def account(self) -> Optional[pulumi.Input[str]]:
         """
-        Account name for the connection
+        Account name for the connection (for Snowflake)
         """
         return pulumi.get(self, "account")
 
     @account.setter
     def account(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "account", value)
 
     @property
     @pulumi.getter(name="adapterId")
     def adapter_id(self) -> Optional[pulumi.Input[int]]:
         """
-        Adapter id created for the Databricks connection
+        Adapter id created for the Databricks connection (for Databricks)
         """
         return pulumi.get(self, "adapter_id")
 
     @adapter_id.setter
     def adapter_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "adapter_id", value)
 
     @property
     @pulumi.getter(name="allowKeepAlive")
     def allow_keep_alive(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether or not the connection should allow client session keep alive
+        Whether or not the connection should allow client session keep alive (for Snowflake)
         """
         return pulumi.get(self, "allow_keep_alive")
 
     @allow_keep_alive.setter
     def allow_keep_alive(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_keep_alive", value)
 
     @property
     @pulumi.getter(name="allowSso")
     def allow_sso(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether or not the connection should allow SSO
+        Whether or not the connection should allow SSO (for Snowflake)
         """
         return pulumi.get(self, "allow_sso")
 
     @allow_sso.setter
     def allow_sso(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_sso", value)
 
     @property
     @pulumi.getter
     def catalog(self) -> Optional[pulumi.Input[str]]:
         """
-        Catalog name if Unity Catalog is enabled in your Databricks workspace
+        Catalog name if Unity Catalog is enabled in your Databricks workspace (for Databricks)
         """
         return pulumi.get(self, "catalog")
 
     @catalog.setter
     def catalog(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "catalog", value)
 
@@ -487,15 +487,15 @@
     def host_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "host_name", value)
 
     @property
     @pulumi.getter(name="httpPath")
     def http_path(self) -> Optional[pulumi.Input[str]]:
         """
-        The HTTP path of the Databricks cluster or SQL warehouse
+        The HTTP path of the Databricks cluster or SQL warehouse (for Databricks)
         """
         return pulumi.get(self, "http_path")
 
     @http_path.setter
     def http_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "http_path", value)
 
@@ -523,27 +523,27 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="oauthClientId")
     def oauth_client_id(self) -> Optional[pulumi.Input[str]]:
         """
-        OAuth client identifier
+        OAuth client identifier (for Snowflake and Databricks)
         """
         return pulumi.get(self, "oauth_client_id")
 
     @oauth_client_id.setter
     def oauth_client_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "oauth_client_id", value)
 
     @property
     @pulumi.getter(name="oauthClientSecret")
     def oauth_client_secret(self) -> Optional[pulumi.Input[str]]:
         """
-        OAuth client secret
+        OAuth client secret (for Snowflake and Databricks)
         """
         return pulumi.get(self, "oauth_client_secret")
 
     @oauth_client_secret.setter
     def oauth_client_secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "oauth_client_secret", value)
 
@@ -583,15 +583,15 @@
     def project_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "project_id", value)
 
     @property
     @pulumi.getter
     def role(self) -> Optional[pulumi.Input[str]]:
         """
-        Role name for the connection
+        Role name for the connection (for Snowflake)
         """
         return pulumi.get(self, "role")
 
     @role.setter
     def role(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "role", value)
 
@@ -619,15 +619,15 @@
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def warehouse(self) -> Optional[pulumi.Input[str]]:
         """
-        Warehouse name for the connection
+        Warehouse name for the connection (for Snowflake)
         """
         return pulumi.get(self, "warehouse")
 
     @warehouse.setter
     def warehouse(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "warehouse", value)
 
@@ -664,72 +664,94 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         databricks = dbtcloud.Connection("databricks",
             project_id=dbt_project["id"],
             type="adapter",
             name="Databricks",
             database="",
             host_name="my-databricks-host.cloud.databricks.com",
             http_path="/my/path",
-            catalog="moo")
+            catalog="moo",
+            oauth_client_id="yourclientid",
+            oauth_client_secret="yourclientsecret")
         redshift = dbtcloud.Connection("redshift",
             project_id=dbt_project["id"],
             type="redshift",
             name="My Redshift Warehouse",
             database="my-database",
             port=5439,
             host_name="my-redshift-hostname")
         snowflake = dbtcloud.Connection("snowflake",
             project_id=dbt_project["id"],
             type="snowflake",
             name="My Snowflake warehouse",
             account="my-snowflake-account",
             database="MY_DATABASE",
             role="MY_ROLE",
-            warehouse="MY_WAREHOUSE")
+            warehouse="MY_WAREHOUSE",
+            oauth_client_id="yourclientid",
+            oauth_client_secret="yourclientsecret",
+            allow_sso=True)
         ```
 
         ## Import
 
-        Import using a project ID and connection ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_connection.test_connection
+
+          id = "project_id:connection_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_connection.test_connection
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/connection:Connection test_connection "project_id:connection_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/connection:Connection test_connection 12345:6789
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] account: Account name for the connection
-        :param pulumi.Input[bool] allow_keep_alive: Whether or not the connection should allow client session keep alive
-        :param pulumi.Input[bool] allow_sso: Whether or not the connection should allow SSO
-        :param pulumi.Input[str] catalog: Catalog name if Unity Catalog is enabled in your Databricks workspace
+        :param pulumi.Input[str] account: Account name for the connection (for Snowflake)
+        :param pulumi.Input[bool] allow_keep_alive: Whether or not the connection should allow client session keep alive (for Snowflake)
+        :param pulumi.Input[bool] allow_sso: Whether or not the connection should allow SSO (for Snowflake)
+        :param pulumi.Input[str] catalog: Catalog name if Unity Catalog is enabled in your Databricks workspace (for Databricks)
         :param pulumi.Input[str] database: Database name for the connection
         :param pulumi.Input[str] host_name: Host name for the connection, including Databricks cluster
-        :param pulumi.Input[str] http_path: The HTTP path of the Databricks cluster or SQL warehouse
+        :param pulumi.Input[str] http_path: The HTTP path of the Databricks cluster or SQL warehouse (for Databricks)
         :param pulumi.Input[bool] is_active: Whether the connection is active
         :param pulumi.Input[str] name: Connection name
-        :param pulumi.Input[str] oauth_client_id: OAuth client identifier
-        :param pulumi.Input[str] oauth_client_secret: OAuth client secret
+        :param pulumi.Input[str] oauth_client_id: OAuth client identifier (for Snowflake and Databricks)
+        :param pulumi.Input[str] oauth_client_secret: OAuth client secret (for Snowflake and Databricks)
         :param pulumi.Input[int] port: Port number to connect via
         :param pulumi.Input[str] private_link_endpoint_id: The ID of the PrivateLink connection. This ID can be found using the `privatelink_endpoint` data source
         :param pulumi.Input[int] project_id: Project ID to create the connection in
-        :param pulumi.Input[str] role: Role name for the connection
+        :param pulumi.Input[str] role: Role name for the connection (for Snowflake)
         :param pulumi.Input[bool] tunnel_enabled: Whether or not tunneling should be enabled on your database connection
         :param pulumi.Input[str] type: The type of connection
-        :param pulumi.Input[str] warehouse: Warehouse name for the connection
+        :param pulumi.Input[str] warehouse: Warehouse name for the connection (for Snowflake)
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ConnectionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -741,43 +763,65 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         databricks = dbtcloud.Connection("databricks",
             project_id=dbt_project["id"],
             type="adapter",
             name="Databricks",
             database="",
             host_name="my-databricks-host.cloud.databricks.com",
             http_path="/my/path",
-            catalog="moo")
+            catalog="moo",
+            oauth_client_id="yourclientid",
+            oauth_client_secret="yourclientsecret")
         redshift = dbtcloud.Connection("redshift",
             project_id=dbt_project["id"],
             type="redshift",
             name="My Redshift Warehouse",
             database="my-database",
             port=5439,
             host_name="my-redshift-hostname")
         snowflake = dbtcloud.Connection("snowflake",
             project_id=dbt_project["id"],
             type="snowflake",
             name="My Snowflake warehouse",
             account="my-snowflake-account",
             database="MY_DATABASE",
             role="MY_ROLE",
-            warehouse="MY_WAREHOUSE")
+            warehouse="MY_WAREHOUSE",
+            oauth_client_id="yourclientid",
+            oauth_client_secret="yourclientsecret",
+            allow_sso=True)
         ```
 
         ## Import
 
-        Import using a project ID and connection ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_connection.test_connection
+
+          id = "project_id:connection_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_connection.test_connection
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/connection:Connection test_connection "project_id:connection_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/connection:Connection test_connection 12345:6789
@@ -884,34 +928,34 @@
         """
         Get an existing Connection resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] account: Account name for the connection
-        :param pulumi.Input[int] adapter_id: Adapter id created for the Databricks connection
-        :param pulumi.Input[bool] allow_keep_alive: Whether or not the connection should allow client session keep alive
-        :param pulumi.Input[bool] allow_sso: Whether or not the connection should allow SSO
-        :param pulumi.Input[str] catalog: Catalog name if Unity Catalog is enabled in your Databricks workspace
+        :param pulumi.Input[str] account: Account name for the connection (for Snowflake)
+        :param pulumi.Input[int] adapter_id: Adapter id created for the Databricks connection (for Databricks)
+        :param pulumi.Input[bool] allow_keep_alive: Whether or not the connection should allow client session keep alive (for Snowflake)
+        :param pulumi.Input[bool] allow_sso: Whether or not the connection should allow SSO (for Snowflake)
+        :param pulumi.Input[str] catalog: Catalog name if Unity Catalog is enabled in your Databricks workspace (for Databricks)
         :param pulumi.Input[int] connection_id: Connection Identifier
         :param pulumi.Input[str] database: Database name for the connection
         :param pulumi.Input[str] host_name: Host name for the connection, including Databricks cluster
-        :param pulumi.Input[str] http_path: The HTTP path of the Databricks cluster or SQL warehouse
+        :param pulumi.Input[str] http_path: The HTTP path of the Databricks cluster or SQL warehouse (for Databricks)
         :param pulumi.Input[bool] is_active: Whether the connection is active
         :param pulumi.Input[str] name: Connection name
-        :param pulumi.Input[str] oauth_client_id: OAuth client identifier
-        :param pulumi.Input[str] oauth_client_secret: OAuth client secret
+        :param pulumi.Input[str] oauth_client_id: OAuth client identifier (for Snowflake and Databricks)
+        :param pulumi.Input[str] oauth_client_secret: OAuth client secret (for Snowflake and Databricks)
         :param pulumi.Input[int] port: Port number to connect via
         :param pulumi.Input[str] private_link_endpoint_id: The ID of the PrivateLink connection. This ID can be found using the `privatelink_endpoint` data source
         :param pulumi.Input[int] project_id: Project ID to create the connection in
-        :param pulumi.Input[str] role: Role name for the connection
+        :param pulumi.Input[str] role: Role name for the connection (for Snowflake)
         :param pulumi.Input[bool] tunnel_enabled: Whether or not tunneling should be enabled on your database connection
         :param pulumi.Input[str] type: The type of connection
-        :param pulumi.Input[str] warehouse: Warehouse name for the connection
+        :param pulumi.Input[str] warehouse: Warehouse name for the connection (for Snowflake)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ConnectionState.__new__(_ConnectionState)
 
         __props__.__dict__["account"] = account
         __props__.__dict__["adapter_id"] = adapter_id
@@ -935,47 +979,47 @@
         __props__.__dict__["warehouse"] = warehouse
         return Connection(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def account(self) -> pulumi.Output[Optional[str]]:
         """
-        Account name for the connection
+        Account name for the connection (for Snowflake)
         """
         return pulumi.get(self, "account")
 
     @property
     @pulumi.getter(name="adapterId")
     def adapter_id(self) -> pulumi.Output[int]:
         """
-        Adapter id created for the Databricks connection
+        Adapter id created for the Databricks connection (for Databricks)
         """
         return pulumi.get(self, "adapter_id")
 
     @property
     @pulumi.getter(name="allowKeepAlive")
     def allow_keep_alive(self) -> pulumi.Output[Optional[bool]]:
         """
-        Whether or not the connection should allow client session keep alive
+        Whether or not the connection should allow client session keep alive (for Snowflake)
         """
         return pulumi.get(self, "allow_keep_alive")
 
     @property
     @pulumi.getter(name="allowSso")
     def allow_sso(self) -> pulumi.Output[Optional[bool]]:
         """
-        Whether or not the connection should allow SSO
+        Whether or not the connection should allow SSO (for Snowflake)
         """
         return pulumi.get(self, "allow_sso")
 
     @property
     @pulumi.getter
     def catalog(self) -> pulumi.Output[Optional[str]]:
         """
-        Catalog name if Unity Catalog is enabled in your Databricks workspace
+        Catalog name if Unity Catalog is enabled in your Databricks workspace (for Databricks)
         """
         return pulumi.get(self, "catalog")
 
     @property
     @pulumi.getter(name="connectionId")
     def connection_id(self) -> pulumi.Output[int]:
         """
@@ -999,15 +1043,15 @@
         """
         return pulumi.get(self, "host_name")
 
     @property
     @pulumi.getter(name="httpPath")
     def http_path(self) -> pulumi.Output[Optional[str]]:
         """
-        The HTTP path of the Databricks cluster or SQL warehouse
+        The HTTP path of the Databricks cluster or SQL warehouse (for Databricks)
         """
         return pulumi.get(self, "http_path")
 
     @property
     @pulumi.getter(name="isActive")
     def is_active(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -1023,23 +1067,23 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="oauthClientId")
     def oauth_client_id(self) -> pulumi.Output[Optional[str]]:
         """
-        OAuth client identifier
+        OAuth client identifier (for Snowflake and Databricks)
         """
         return pulumi.get(self, "oauth_client_id")
 
     @property
     @pulumi.getter(name="oauthClientSecret")
     def oauth_client_secret(self) -> pulumi.Output[Optional[str]]:
         """
-        OAuth client secret
+        OAuth client secret (for Snowflake and Databricks)
         """
         return pulumi.get(self, "oauth_client_secret")
 
     @property
     @pulumi.getter
     def port(self) -> pulumi.Output[Optional[int]]:
         """
@@ -1063,15 +1107,15 @@
         """
         return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter
     def role(self) -> pulumi.Output[Optional[str]]:
         """
-        Role name for the connection
+        Role name for the connection (for Snowflake)
         """
         return pulumi.get(self, "role")
 
     @property
     @pulumi.getter(name="tunnelEnabled")
     def tunnel_enabled(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -1087,11 +1131,11 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def warehouse(self) -> pulumi.Output[Optional[str]]:
         """
-        Warehouse name for the connection
+        Warehouse name for the connection (for Snowflake)
         """
         return pulumi.get(self, "warehouse")
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/databricks_credential.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/databricks_credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,15 +278,14 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         # when using the Databricks adapter
         my_databricks_cred = dbtcloud.DatabricksCredential("my_databricks_cred",
             project_id=dbt_project["id"],
             adapter_id=my_databricks_connection["adapterId"],
             target_name="prod",
             token="abcdefgh",
             schema="my_schema",
@@ -299,15 +298,33 @@
             token="abcdefgh",
             schema="my_schema",
             adapter_type="spark")
         ```
 
         ## Import
 
-        Import using a project ID and credential ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_databricks_credential.my_databricks_credential
+
+          id = "project_id:credential_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_databricks_credential.my_databricks_credential
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/databricksCredential:DatabricksCredential my_databricks_credential "project_id:credential_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/databricksCredential:DatabricksCredential my_databricks_credential 12345:6789
@@ -332,15 +349,14 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         # when using the Databricks adapter
         my_databricks_cred = dbtcloud.DatabricksCredential("my_databricks_cred",
             project_id=dbt_project["id"],
             adapter_id=my_databricks_connection["adapterId"],
             target_name="prod",
             token="abcdefgh",
             schema="my_schema",
@@ -353,15 +369,33 @@
             token="abcdefgh",
             schema="my_schema",
             adapter_type="spark")
         ```
 
         ## Import
 
-        Import using a project ID and credential ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_databricks_credential.my_databricks_credential
+
+          id = "project_id:credential_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_databricks_credential.my_databricks_credential
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/databricksCredential:DatabricksCredential my_databricks_credential "project_id:credential_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/databricksCredential:DatabricksCredential my_databricks_credential 12345:6789
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/environment.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                  deployment_type: Optional[pulumi.Input[str]] = None,
                  extended_attributes_id: Optional[pulumi.Input[int]] = None,
                  is_active: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  use_custom_branch: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Environment resource.
-        :param pulumi.Input[str] dbt_version: Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` or `major.minor.0-pre`, e.g. `1.5.0-latest`
+        :param pulumi.Input[str] dbt_version: Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` (e.g. `1.5.0-latest`), `major.minor.0-pre` or `versionless`. In a future version of the provider `versionless` will be the default if no version is provided
         :param pulumi.Input[int] project_id: Project ID to create the environment in
         :param pulumi.Input[str] type: The type of environment (must be either development or deployment)
         :param pulumi.Input[int] credential_id: Credential ID to create the environment with. A credential is not required for development environments but is required for deployment environments
         :param pulumi.Input[str] custom_branch: Which custom branch to use in this environment
         :param pulumi.Input[str] deployment_type: The type of environment. Only valid for environments of type 'deployment' and for now can only be empty or set to 'production'
         :param pulumi.Input[int] extended_attributes_id: ID of the extended attributes for the environment
         :param pulumi.Input[bool] is_active: Whether the environment is active
@@ -55,15 +55,15 @@
         if use_custom_branch is not None:
             pulumi.set(__self__, "use_custom_branch", use_custom_branch)
 
     @property
     @pulumi.getter(name="dbtVersion")
     def dbt_version(self) -> pulumi.Input[str]:
         """
-        Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` or `major.minor.0-pre`, e.g. `1.5.0-latest`
+        Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` (e.g. `1.5.0-latest`), `major.minor.0-pre` or `versionless`. In a future version of the provider `versionless` will be the default if no version is provided
         """
         return pulumi.get(self, "dbt_version")
 
     @dbt_version.setter
     def dbt_version(self, value: pulumi.Input[str]):
         pulumi.set(self, "dbt_version", value)
 
@@ -190,15 +190,15 @@
                  project_id: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  use_custom_branch: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Environment resources.
         :param pulumi.Input[int] credential_id: Credential ID to create the environment with. A credential is not required for development environments but is required for deployment environments
         :param pulumi.Input[str] custom_branch: Which custom branch to use in this environment
-        :param pulumi.Input[str] dbt_version: Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` or `major.minor.0-pre`, e.g. `1.5.0-latest`
+        :param pulumi.Input[str] dbt_version: Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` (e.g. `1.5.0-latest`), `major.minor.0-pre` or `versionless`. In a future version of the provider `versionless` will be the default if no version is provided
         :param pulumi.Input[str] deployment_type: The type of environment. Only valid for environments of type 'deployment' and for now can only be empty or set to 'production'
         :param pulumi.Input[int] environment_id: Environment ID within the project
         :param pulumi.Input[int] extended_attributes_id: ID of the extended attributes for the environment
         :param pulumi.Input[bool] is_active: Whether the environment is active
         :param pulumi.Input[str] name: Environment name
         :param pulumi.Input[int] project_id: Project ID to create the environment in
         :param pulumi.Input[str] type: The type of environment (must be either development or deployment)
@@ -251,15 +251,15 @@
     def custom_branch(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_branch", value)
 
     @property
     @pulumi.getter(name="dbtVersion")
     def dbt_version(self) -> Optional[pulumi.Input[str]]:
         """
-        Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` or `major.minor.0-pre`, e.g. `1.5.0-latest`
+        Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` (e.g. `1.5.0-latest`), `major.minor.0-pre` or `versionless`. In a future version of the provider `versionless` will be the default if no version is provided
         """
         return pulumi.get(self, "dbt_version")
 
     @dbt_version.setter
     def dbt_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dbt_version", value)
 
@@ -379,15 +379,14 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         ci_environment = dbtcloud.Environment("ci_environment",
             dbt_version="1.6.0-latest",
             name="CI",
             project_id=dbt_project["id"],
             type="deployment",
             credential_id=ci_credential["credentialId"])
         # we can also set a deployment environment as being the production one
@@ -404,29 +403,47 @@
             name="Dev",
             project_id=dbt_project["id"],
             type="development")
         ```
 
         ## Import
 
-        Import using a project ID and environment ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_environment.prod_environment
+
+          id = "project_id:environment_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_environment.prod_environment
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/environment:Environment prod_environment "project_id:environment_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/environment:Environment prod_environment 12345:6789
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] credential_id: Credential ID to create the environment with. A credential is not required for development environments but is required for deployment environments
         :param pulumi.Input[str] custom_branch: Which custom branch to use in this environment
-        :param pulumi.Input[str] dbt_version: Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` or `major.minor.0-pre`, e.g. `1.5.0-latest`
+        :param pulumi.Input[str] dbt_version: Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` (e.g. `1.5.0-latest`), `major.minor.0-pre` or `versionless`. In a future version of the provider `versionless` will be the default if no version is provided
         :param pulumi.Input[str] deployment_type: The type of environment. Only valid for environments of type 'deployment' and for now can only be empty or set to 'production'
         :param pulumi.Input[int] extended_attributes_id: ID of the extended attributes for the environment
         :param pulumi.Input[bool] is_active: Whether the environment is active
         :param pulumi.Input[str] name: Environment name
         :param pulumi.Input[int] project_id: Project ID to create the environment in
         :param pulumi.Input[str] type: The type of environment (must be either development or deployment)
         :param pulumi.Input[bool] use_custom_branch: Whether to use a custom git branch in this environment
@@ -440,15 +457,14 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         ci_environment = dbtcloud.Environment("ci_environment",
             dbt_version="1.6.0-latest",
             name="CI",
             project_id=dbt_project["id"],
             type="deployment",
             credential_id=ci_credential["credentialId"])
         # we can also set a deployment environment as being the production one
@@ -465,15 +481,33 @@
             name="Dev",
             project_id=dbt_project["id"],
             type="development")
         ```
 
         ## Import
 
-        Import using a project ID and environment ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_environment.prod_environment
+
+          id = "project_id:environment_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_environment.prod_environment
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/environment:Environment prod_environment "project_id:environment_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/environment:Environment prod_environment 12345:6789
@@ -556,15 +590,15 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] credential_id: Credential ID to create the environment with. A credential is not required for development environments but is required for deployment environments
         :param pulumi.Input[str] custom_branch: Which custom branch to use in this environment
-        :param pulumi.Input[str] dbt_version: Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` or `major.minor.0-pre`, e.g. `1.5.0-latest`
+        :param pulumi.Input[str] dbt_version: Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` (e.g. `1.5.0-latest`), `major.minor.0-pre` or `versionless`. In a future version of the provider `versionless` will be the default if no version is provided
         :param pulumi.Input[str] deployment_type: The type of environment. Only valid for environments of type 'deployment' and for now can only be empty or set to 'production'
         :param pulumi.Input[int] environment_id: Environment ID within the project
         :param pulumi.Input[int] extended_attributes_id: ID of the extended attributes for the environment
         :param pulumi.Input[bool] is_active: Whether the environment is active
         :param pulumi.Input[str] name: Environment name
         :param pulumi.Input[int] project_id: Project ID to create the environment in
         :param pulumi.Input[str] type: The type of environment (must be either development or deployment)
@@ -603,15 +637,15 @@
         """
         return pulumi.get(self, "custom_branch")
 
     @property
     @pulumi.getter(name="dbtVersion")
     def dbt_version(self) -> pulumi.Output[str]:
         """
-        Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` or `major.minor.0-pre`, e.g. `1.5.0-latest`
+        Version number of dbt to use in this environment. It needs to be in the format `major.minor.0-latest` (e.g. `1.5.0-latest`), `major.minor.0-pre` or `versionless`. In a future version of the provider `versionless` will be the default if no version is provided
         """
         return pulumi.get(self, "dbt_version")
 
     @property
     @pulumi.getter(name="deploymentType")
     def deployment_type(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/environment_variable.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/environment_variable.py`

 * *Files 7% similar despite different names*

```diff
@@ -136,15 +136,14 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         dbt_my_env_var = dbtcloud.EnvironmentVariable("dbt_my_env_var",
             name="DBT_MY_ENV_VAR",
             project_id=dbt_project["id"],
             environment_values={
                 "project": "my_project_level_value",
                 "Dev": "my_env_level_value",
                 "CI": "my_ci_override_value",
@@ -156,15 +155,33 @@
                     ci_env,
                     prod_env,
                 ]))
         ```
 
         ## Import
 
-        Import using a project ID and environment variable name found in the URL and UI or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_environment_variable.test_environment_variable
+
+          id = "project_id:environment_variable_name"
+
+        }
+
+        import {
+
+          to = dbtcloud_environment_variable.test_environment_variable
+
+          id = "12345:DBT_ENV_VAR"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/environmentVariable:EnvironmentVariable test_environment_variable "project_id:environment_variable_name"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/environmentVariable:EnvironmentVariable test_environment_variable 12345:DBT_ENV_VAR
@@ -188,15 +205,14 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         dbt_my_env_var = dbtcloud.EnvironmentVariable("dbt_my_env_var",
             name="DBT_MY_ENV_VAR",
             project_id=dbt_project["id"],
             environment_values={
                 "project": "my_project_level_value",
                 "Dev": "my_env_level_value",
                 "CI": "my_ci_override_value",
@@ -208,15 +224,33 @@
                     ci_env,
                     prod_env,
                 ]))
         ```
 
         ## Import
 
-        Import using a project ID and environment variable name found in the URL and UI or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_environment_variable.test_environment_variable
+
+          id = "project_id:environment_variable_name"
+
+        }
+
+        import {
+
+          to = dbtcloud_environment_variable.test_environment_variable
+
+          id = "12345:DBT_ENV_VAR"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/environmentVariable:EnvironmentVariable test_environment_variable "project_id:environment_variable_name"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/environmentVariable:EnvironmentVariable test_environment_variable 12345:DBT_ENV_VAR
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/environment_variable_job_override.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/environment_variable_job_override.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,33 @@
             project_id=dbt_project["id"],
             job_definition_id=daily_job["id"],
             raw_value="my_override_value")
         ```
 
         ## Import
 
-        Import using a project ID, a job ID and the environment variable override ID
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_environment_variable_job_override.test_environment_variable_job_override
+
+          id = "project_id:job_id:environment_variable_override_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_environment_variable_job_override.test_environment_variable_job_override
+
+          id = "12345:678:123456"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/environmentVariableJobOverride:EnvironmentVariableJobOverride test_environment_variable_job_override "project_id:job_id:environment_variable_override_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/environmentVariableJobOverride:EnvironmentVariableJobOverride test_environment_variable_job_override 12345:678:123456
@@ -229,15 +247,33 @@
             project_id=dbt_project["id"],
             job_definition_id=daily_job["id"],
             raw_value="my_override_value")
         ```
 
         ## Import
 
-        Import using a project ID, a job ID and the environment variable override ID
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_environment_variable_job_override.test_environment_variable_job_override
+
+          id = "project_id:job_id:environment_variable_override_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_environment_variable_job_override.test_environment_variable_job_override
+
+          id = "12345:678:123456"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/environmentVariableJobOverride:EnvironmentVariableJobOverride test_environment_variable_job_override "project_id:job_id:environment_variable_override_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/environmentVariableJobOverride:EnvironmentVariableJobOverride test_environment_variable_job_override 12345:678:123456
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/extended_attributes.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/extended_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -135,15 +135,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  extended_attributes: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[int]] = None,
                  state: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        This resource allows setting extended attributes which can be assigned to a given environment ([see docs](https://docs.getdbt.com/docs/dbt-cloud-environments#extended-attributes-beta)).<br/><br/>In dbt Cloud those values are provided as YML but in the provider they need to be provided as JSON (see example below).
+        This resource allows setting extended attributes which can be assigned to a given environment ([see docs](https://docs.getdbt.com/docs/dbt-cloud-environments#extended-attributes)).<br/><br/>In dbt Cloud those values are provided as YML but in the provider they need to be provided as JSON (see example below).
 
         ## Example Usage
 
         ```python
         import pulumi
         import json
         import pulumi_dbtcloud as dbtcloud
@@ -169,15 +169,33 @@
             credential_id=dbt_credential_id,
             deployment_type="production",
             extended_attributes_id=my_attributes.extended_attributes_id)
         ```
 
         ## Import
 
-        Import using a project ID and extended attribute ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_extended_attributes.test_extended_attributes
+
+          id = "project_id_id:extended_attributes_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_extended_attributes.test_extended_attributes
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/extendedAttributes:ExtendedAttributes test_extended_attributes "project_id_id:extended_attributes_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/extendedAttributes:ExtendedAttributes test_extended_attributes 12345:6789
@@ -191,15 +209,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ExtendedAttributesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        This resource allows setting extended attributes which can be assigned to a given environment ([see docs](https://docs.getdbt.com/docs/dbt-cloud-environments#extended-attributes-beta)).<br/><br/>In dbt Cloud those values are provided as YML but in the provider they need to be provided as JSON (see example below).
+        This resource allows setting extended attributes which can be assigned to a given environment ([see docs](https://docs.getdbt.com/docs/dbt-cloud-environments#extended-attributes)).<br/><br/>In dbt Cloud those values are provided as YML but in the provider they need to be provided as JSON (see example below).
 
         ## Example Usage
 
         ```python
         import pulumi
         import json
         import pulumi_dbtcloud as dbtcloud
@@ -225,15 +243,33 @@
             credential_id=dbt_credential_id,
             deployment_type="production",
             extended_attributes_id=my_attributes.extended_attributes_id)
         ```
 
         ## Import
 
-        Import using a project ID and extended attribute ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_extended_attributes.test_extended_attributes
+
+          id = "project_id_id:extended_attributes_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_extended_attributes.test_extended_attributes
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/extendedAttributes:ExtendedAttributes test_extended_attributes "project_id_id:extended_attributes_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/extendedAttributes:ExtendedAttributes test_extended_attributes 12345:6789
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/fabric_connection.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/fabric_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,14 +341,34 @@
             database="my-database",
             port=1234,
             login_timeout=30)
         ```
 
         ## Import
 
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_fabric_connection.my_connection
+
+          id = "project_id:connection_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_fabric_connection.my_connection
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
+
         ```sh
         $ pulumi import dbtcloud:index/fabricConnection:FabricConnection my_connection "project_id:connection_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/fabricConnection:FabricConnection my_connection 12345:6789
         ```
@@ -386,14 +406,34 @@
             database="my-database",
             port=1234,
             login_timeout=30)
         ```
 
         ## Import
 
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_fabric_connection.my_connection
+
+          id = "project_id:connection_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_fabric_connection.my_connection
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
+
         ```sh
         $ pulumi import dbtcloud:index/fabricConnection:FabricConnection my_connection "project_id:connection_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/fabricConnection:FabricConnection my_connection 12345:6789
         ```
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/fabric_credential.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/fabric_credential.py`

 * *Files 3% similar despite different names*

```diff
@@ -342,17 +342,58 @@
                  schema_authorization: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
+        ```python
+        import pulumi
+        import pulumi_dbtcloud as dbtcloud
+
+        # when using AD authentication
+        my_fabric_cred_ad = dbtcloud.FabricCredential("my_fabric_cred_ad",
+            project_id=dbt_project["id"],
+            adapter_id=my_fabric_connection["adapterId"],
+            schema="my_schema",
+            user="my_user",
+            password="my_password",
+            schema_authorization="abcd")
+        # when using service principal authentication
+        my_fabric_cred_serv_princ = dbtcloud.FabricCredential("my_fabric_cred_serv_princ",
+            project_id=dbt_project["id"],
+            adapter_id=my_fabric_connection["adapterId"],
+            schema="my_schema",
+            client_id="my_client_id",
+            tenant_id="my_tenant_id",
+            client_secret="my_secret",
+            schema_authorization="abcd")
+        ```
+
         ## Import
 
-        Import using a project ID and credential ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_fabric_credential.my_fabric_credential
+
+          id = "project_id:credential_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_fabric_credential.my_fabric_credential
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/fabricCredential:FabricCredential my_fabric_credential "project_id:credential_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/fabricCredential:FabricCredential my_fabric_credential 12345:6789
@@ -375,17 +416,58 @@
     def __init__(__self__,
                  resource_name: str,
                  args: FabricCredentialArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
+        ```python
+        import pulumi
+        import pulumi_dbtcloud as dbtcloud
+
+        # when using AD authentication
+        my_fabric_cred_ad = dbtcloud.FabricCredential("my_fabric_cred_ad",
+            project_id=dbt_project["id"],
+            adapter_id=my_fabric_connection["adapterId"],
+            schema="my_schema",
+            user="my_user",
+            password="my_password",
+            schema_authorization="abcd")
+        # when using service principal authentication
+        my_fabric_cred_serv_princ = dbtcloud.FabricCredential("my_fabric_cred_serv_princ",
+            project_id=dbt_project["id"],
+            adapter_id=my_fabric_connection["adapterId"],
+            schema="my_schema",
+            client_id="my_client_id",
+            tenant_id="my_tenant_id",
+            client_secret="my_secret",
+            schema_authorization="abcd")
+        ```
+
         ## Import
 
-        Import using a project ID and credential ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_fabric_credential.my_fabric_credential
+
+          id = "project_id:credential_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_fabric_credential.my_fabric_credential
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/fabricCredential:FabricCredential my_fabric_credential "project_id:credential_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/fabricCredential:FabricCredential my_fabric_credential 12345:6789
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_azure_dev_ops_project.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_azure_dev_ops_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_azure_dev_ops_repository.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_azure_dev_ops_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_big_query_connection.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_big_query_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_big_query_credential.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_big_query_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_connection.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_databricks_credential.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_databricks_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_environment.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 ]
 
 @pulumi.output_type
 class GetEnvironmentResult:
     """
     A collection of values returned by getEnvironment.
     """
-    def __init__(__self__, credential_id=None, custom_branch=None, dbt_version=None, deployment_type=None, environment_id=None, extended_attributes_id=None, id=None, is_active=None, name=None, project_id=None, type=None, use_custom_branch=None):
-        if credential_id and not isinstance(credential_id, int):
-            raise TypeError("Expected argument 'credential_id' to be a int")
-        pulumi.set(__self__, "credential_id", credential_id)
+    def __init__(__self__, credentials_id=None, custom_branch=None, dbt_version=None, deployment_type=None, environment_id=None, extended_attributes_id=None, id=None, name=None, project_id=None, type=None, use_custom_branch=None):
+        if credentials_id and not isinstance(credentials_id, int):
+            raise TypeError("Expected argument 'credentials_id' to be a int")
+        pulumi.set(__self__, "credentials_id", credentials_id)
         if custom_branch and not isinstance(custom_branch, str):
             raise TypeError("Expected argument 'custom_branch' to be a str")
         pulumi.set(__self__, "custom_branch", custom_branch)
         if dbt_version and not isinstance(dbt_version, str):
             raise TypeError("Expected argument 'dbt_version' to be a str")
         pulumi.set(__self__, "dbt_version", dbt_version)
         if deployment_type and not isinstance(deployment_type, str):
@@ -39,43 +39,40 @@
         pulumi.set(__self__, "environment_id", environment_id)
         if extended_attributes_id and not isinstance(extended_attributes_id, int):
             raise TypeError("Expected argument 'extended_attributes_id' to be a int")
         pulumi.set(__self__, "extended_attributes_id", extended_attributes_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if is_active and not isinstance(is_active, bool):
-            raise TypeError("Expected argument 'is_active' to be a bool")
-        pulumi.set(__self__, "is_active", is_active)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
         if project_id and not isinstance(project_id, int):
             raise TypeError("Expected argument 'project_id' to be a int")
         pulumi.set(__self__, "project_id", project_id)
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
         if use_custom_branch and not isinstance(use_custom_branch, bool):
             raise TypeError("Expected argument 'use_custom_branch' to be a bool")
         pulumi.set(__self__, "use_custom_branch", use_custom_branch)
 
     @property
-    @pulumi.getter(name="credentialId")
-    def credential_id(self) -> int:
+    @pulumi.getter(name="credentialsId")
+    def credentials_id(self) -> int:
         """
-        Credential ID to create the environment with
+        The project ID to which the environment belong
         """
-        return pulumi.get(self, "credential_id")
+        return pulumi.get(self, "credentials_id")
 
     @property
     @pulumi.getter(name="customBranch")
     def custom_branch(self) -> str:
         """
-        Which custom branch to use in this environment
+        The type of deployment environment (currently 'production', 'staging' or empty)
         """
         return pulumi.get(self, "custom_branch")
 
     @property
     @pulumi.getter(name="dbtVersion")
     def dbt_version(self) -> str:
         """
@@ -83,23 +80,23 @@
         """
         return pulumi.get(self, "dbt_version")
 
     @property
     @pulumi.getter(name="deploymentType")
     def deployment_type(self) -> str:
         """
-        The type of deployment environment (currently 'production' or empty)
+        The name of the environment
         """
         return pulumi.get(self, "deployment_type")
 
     @property
     @pulumi.getter(name="environmentId")
     def environment_id(self) -> int:
         """
-        ID of the environment
+        The ID of the environment
         """
         return pulumi.get(self, "environment_id")
 
     @property
     @pulumi.getter(name="extendedAttributesId")
     def extended_attributes_id(self) -> int:
         """
@@ -112,42 +109,34 @@
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="isActive")
-    def is_active(self) -> bool:
-        """
-        Whether the environment is active
-        """
-        return pulumi.get(self, "is_active")
-
-    @property
     @pulumi.getter
     def name(self) -> str:
         """
-        Environment name
+        The name of the environment
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> int:
         """
-        Project ID to create the environment in
+        The project ID to which the environment belong
         """
         return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        The type of environment (must be either development or deployment)
+        The name of the environment
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="useCustomBranch")
     def use_custom_branch(self) -> bool:
         """
@@ -158,62 +147,62 @@
 
 class AwaitableGetEnvironmentResult(GetEnvironmentResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetEnvironmentResult(
-            credential_id=self.credential_id,
+            credentials_id=self.credentials_id,
             custom_branch=self.custom_branch,
             dbt_version=self.dbt_version,
             deployment_type=self.deployment_type,
             environment_id=self.environment_id,
             extended_attributes_id=self.extended_attributes_id,
             id=self.id,
-            is_active=self.is_active,
             name=self.name,
             project_id=self.project_id,
             type=self.type,
             use_custom_branch=self.use_custom_branch)
 
 
 def get_environment(environment_id: Optional[int] = None,
                     project_id: Optional[int] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetEnvironmentResult:
     """
-    Use this data source to access information about an existing resource.
+    Retrieve data for a single environment
+
 
-    :param int environment_id: ID of the environment
-    :param int project_id: Project ID to create the environment in
+    :param int environment_id: The ID of the environment
+    :param int project_id: The project ID to which the environment belong
     """
     __args__ = dict()
     __args__['environmentId'] = environment_id
     __args__['projectId'] = project_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('dbtcloud:index/getEnvironment:getEnvironment', __args__, opts=opts, typ=GetEnvironmentResult).value
 
     return AwaitableGetEnvironmentResult(
-        credential_id=pulumi.get(__ret__, 'credential_id'),
+        credentials_id=pulumi.get(__ret__, 'credentials_id'),
         custom_branch=pulumi.get(__ret__, 'custom_branch'),
         dbt_version=pulumi.get(__ret__, 'dbt_version'),
         deployment_type=pulumi.get(__ret__, 'deployment_type'),
         environment_id=pulumi.get(__ret__, 'environment_id'),
         extended_attributes_id=pulumi.get(__ret__, 'extended_attributes_id'),
         id=pulumi.get(__ret__, 'id'),
-        is_active=pulumi.get(__ret__, 'is_active'),
         name=pulumi.get(__ret__, 'name'),
         project_id=pulumi.get(__ret__, 'project_id'),
         type=pulumi.get(__ret__, 'type'),
         use_custom_branch=pulumi.get(__ret__, 'use_custom_branch'))
 
 
 @_utilities.lift_output_func(get_environment)
 def get_environment_output(environment_id: Optional[pulumi.Input[int]] = None,
                            project_id: Optional[pulumi.Input[int]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEnvironmentResult]:
     """
-    Use this data source to access information about an existing resource.
+    Retrieve data for a single environment
+
 
-    :param int environment_id: ID of the environment
-    :param int project_id: Project ID to create the environment in
+    :param int environment_id: The ID of the environment
+    :param int project_id: The project ID to which the environment belong
     """
     ...
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_environment_variable.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_environment_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_extended_attributes.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_extended_attributes.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_group.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_group_users.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_group_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_job.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         """
         return pulumi.get(self, "timeout_seconds")
 
     @property
     @pulumi.getter
     def triggers(self) -> Mapping[str, bool]:
         """
-        Flags for which types of triggers to use, keys of github*webhook, git*provider*webhook, schedule, custom*branch_only
+        Flags for which types of triggers to use, keys of github*webhook, git*provider*webhook, schedule, on*merge
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter(name="triggersOnDraftPr")
     def triggers_on_draft_pr(self) -> bool:
         """
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_notification.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_notification.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 
 @pulumi.output_type
 class GetNotificationResult:
     """
     A collection of values returned by getNotification.
     """
-    def __init__(__self__, external_email=None, id=None, notification_id=None, notification_type=None, on_cancels=None, on_failures=None, on_successes=None, user_id=None):
+    def __init__(__self__, external_email=None, id=None, notification_id=None, notification_type=None, on_cancels=None, on_failures=None, on_successes=None, slack_channel_id=None, slack_channel_name=None, state=None, user_id=None):
         if external_email and not isinstance(external_email, str):
             raise TypeError("Expected argument 'external_email' to be a str")
         pulumi.set(__self__, "external_email", external_email)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if notification_id and not isinstance(notification_id, int):
@@ -39,14 +39,23 @@
         pulumi.set(__self__, "on_cancels", on_cancels)
         if on_failures and not isinstance(on_failures, list):
             raise TypeError("Expected argument 'on_failures' to be a list")
         pulumi.set(__self__, "on_failures", on_failures)
         if on_successes and not isinstance(on_successes, list):
             raise TypeError("Expected argument 'on_successes' to be a list")
         pulumi.set(__self__, "on_successes", on_successes)
+        if slack_channel_id and not isinstance(slack_channel_id, str):
+            raise TypeError("Expected argument 'slack_channel_id' to be a str")
+        pulumi.set(__self__, "slack_channel_id", slack_channel_id)
+        if slack_channel_name and not isinstance(slack_channel_name, str):
+            raise TypeError("Expected argument 'slack_channel_name' to be a str")
+        pulumi.set(__self__, "slack_channel_name", slack_channel_name)
+        if state and not isinstance(state, int):
+            raise TypeError("Expected argument 'state' to be a int")
+        pulumi.set(__self__, "state", state)
         if user_id and not isinstance(user_id, int):
             raise TypeError("Expected argument 'user_id' to be a int")
         pulumi.set(__self__, "user_id", user_id)
 
     @property
     @pulumi.getter(name="externalEmail")
     def external_email(self) -> str:
@@ -63,23 +72,23 @@
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="notificationId")
     def notification_id(self) -> int:
         """
-        ID of the notification
+        The ID of the notification
         """
         return pulumi.get(self, "notification_id")
 
     @property
     @pulumi.getter(name="notificationType")
     def notification_type(self) -> int:
         """
-        Type of notification (1 = dbt Cloud user email (default): does not require an external*email ; 4 = external email: requires setting an external*email)
+        Type of notification (1 = dbt Cloud user email (default): does not require an external_email ; 2 = Slack channel: requires `slack_channel_id` and `slack_channel_name` ; 4 = external email: requires setting an `external_email`)
         """
         return pulumi.get(self, "notification_type")
 
     @property
     @pulumi.getter(name="onCancels")
     def on_cancels(self) -> Sequence[int]:
         """
@@ -100,14 +109,38 @@
     def on_successes(self) -> Sequence[int]:
         """
         List of job IDs to trigger the webhook on success
         """
         return pulumi.get(self, "on_successes")
 
     @property
+    @pulumi.getter(name="slackChannelId")
+    def slack_channel_id(self) -> str:
+        """
+        The ID of the Slack channel to receive the notification. It can be found at the bottom of the Slack channel settings
+        """
+        return pulumi.get(self, "slack_channel_id")
+
+    @property
+    @pulumi.getter(name="slackChannelName")
+    def slack_channel_name(self) -> str:
+        """
+        The name of the slack channel
+        """
+        return pulumi.get(self, "slack_channel_name")
+
+    @property
+    @pulumi.getter
+    def state(self) -> int:
+        """
+        State of the notification (1 = active (default), 2 = inactive)
+        """
+        return pulumi.get(self, "state")
+
+    @property
     @pulumi.getter(name="userId")
     def user_id(self) -> int:
         """
         Internal dbt Cloud User ID. Must be the user_id for an existing user even if the notification is an external one
         """
         return pulumi.get(self, "user_id")
 
@@ -121,58 +154,68 @@
             external_email=self.external_email,
             id=self.id,
             notification_id=self.notification_id,
             notification_type=self.notification_type,
             on_cancels=self.on_cancels,
             on_failures=self.on_failures,
             on_successes=self.on_successes,
+            slack_channel_id=self.slack_channel_id,
+            slack_channel_name=self.slack_channel_name,
+            state=self.state,
             user_id=self.user_id)
 
 
 def get_notification(notification_id: Optional[int] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNotificationResult:
     """
+    Retrieve notification details
+
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_dbtcloud as dbtcloud
 
     my_notification = dbtcloud.get_notification(notification_id=12345)
     ```
 
 
-    :param int notification_id: ID of the notification
+    :param int notification_id: The ID of the notification
     """
     __args__ = dict()
     __args__['notificationId'] = notification_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('dbtcloud:index/getNotification:getNotification', __args__, opts=opts, typ=GetNotificationResult).value
 
     return AwaitableGetNotificationResult(
         external_email=pulumi.get(__ret__, 'external_email'),
         id=pulumi.get(__ret__, 'id'),
         notification_id=pulumi.get(__ret__, 'notification_id'),
         notification_type=pulumi.get(__ret__, 'notification_type'),
         on_cancels=pulumi.get(__ret__, 'on_cancels'),
         on_failures=pulumi.get(__ret__, 'on_failures'),
         on_successes=pulumi.get(__ret__, 'on_successes'),
+        slack_channel_id=pulumi.get(__ret__, 'slack_channel_id'),
+        slack_channel_name=pulumi.get(__ret__, 'slack_channel_name'),
+        state=pulumi.get(__ret__, 'state'),
         user_id=pulumi.get(__ret__, 'user_id'))
 
 
 @_utilities.lift_output_func(get_notification)
 def get_notification_output(notification_id: Optional[pulumi.Input[int]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNotificationResult]:
     """
+    Retrieve notification details
+
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_dbtcloud as dbtcloud
 
     my_notification = dbtcloud.get_notification(notification_id=12345)
     ```
 
 
-    :param int notification_id: ID of the notification
+    :param int notification_id: The ID of the notification
     """
     ...
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_postgres_credential.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_postgres_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_privatelink_endpoint.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_project.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_repository.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 
     @property
     @pulumi.getter(name="fetchDeployKey")
     def fetch_deploy_key(self) -> Optional[bool]:
         """
         Whether we should return the public deploy key
         """
+        warnings.warn("""This field is deprecated and will be removed in a future version of the provider. The key is always fetched when the clone strategy is `deploy_key`""", DeprecationWarning)
+        pulumi.log.warn("""fetch_deploy_key is deprecated: This field is deprecated and will be removed in a future version of the provider. The key is always fetched when the clone strategy is `deploy_key`""")
+
         return pulumi.get(self, "fetch_deploy_key")
 
     @property
     @pulumi.getter(name="gitCloneStrategy")
     def git_clone_strategy(self) -> str:
         """
         Git clone strategy for the repository
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_service_token.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_service_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_snowflake_credential.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_snowflake_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_user.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,16 @@
             email=self.email,
             id=self.id)
 
 
 def get_user(email: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserResult:
     """
+    Retrieve user details
+
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_dbtcloud as dbtcloud
 
     my_user = dbtcloud.get_user(email="my_user@email.com")
@@ -81,14 +83,16 @@
         id=pulumi.get(__ret__, 'id'))
 
 
 @_utilities.lift_output_func(get_user)
 def get_user_output(email: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
     """
+    Retrieve user details
+
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_dbtcloud as dbtcloud
 
     my_user = dbtcloud.get_user(email="my_user@email.com")
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_user_groups.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_webhook.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/group.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/group.py`

 * *Files 8% similar despite different names*

```diff
@@ -189,23 +189,20 @@
                  assign_by_default: Optional[pulumi.Input[bool]] = None,
                  group_permissions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GroupGroupPermissionArgs']]]]] = None,
                  is_active: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  sso_mapping_groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
-        *Note*: Groups currently do not support updates, as per both the API and the UI.
-
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         tf_group1 = dbtcloud.Group("tf_group_1",
             name="TF Group 1",
             group_permissions=[
                 dbtcloud.GroupGroupPermissionArgs(
                     permission_set="member",
                     all_projects=True,
                 ),
@@ -215,22 +212,40 @@
                     project_id=dbt_project["id"],
                 ),
             ])
         ```
 
         ## Import
 
-        Import using a group ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_group.my_group
+
+          id = "group_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_group.my_group
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
-        $ pulumi import dbtcloud:index/group:Group test_group "group_id"
+        $ pulumi import dbtcloud:index/group:Group my_group "group_id"
         ```
 
         ```sh
-        $ pulumi import dbtcloud:index/group:Group test_group 12345
+        $ pulumi import dbtcloud:index/group:Group my_group 12345
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] assign_by_default: Whether or not to assign this group to users by default
         :param pulumi.Input[bool] is_active: Whether the group is active
         :param pulumi.Input[str] name: Group name
@@ -239,23 +254,20 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[GroupArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        *Note*: Groups currently do not support updates, as per both the API and the UI.
-
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         tf_group1 = dbtcloud.Group("tf_group_1",
             name="TF Group 1",
             group_permissions=[
                 dbtcloud.GroupGroupPermissionArgs(
                     permission_set="member",
                     all_projects=True,
                 ),
@@ -265,22 +277,40 @@
                     project_id=dbt_project["id"],
                 ),
             ])
         ```
 
         ## Import
 
-        Import using a group ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_group.my_group
+
+          id = "group_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_group.my_group
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
-        $ pulumi import dbtcloud:index/group:Group test_group "group_id"
+        $ pulumi import dbtcloud:index/group:Group my_group "group_id"
         ```
 
         ```sh
-        $ pulumi import dbtcloud:index/group:Group test_group 12345
+        $ pulumi import dbtcloud:index/group:Group my_group 12345
         ```
 
         :param str resource_name: The name of the resource.
         :param GroupArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/job.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                  timeout_seconds: Optional[pulumi.Input[int]] = None,
                  triggers_on_draft_pr: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Job resource.
         :param pulumi.Input[int] environment_id: Environment ID to create the job in
         :param pulumi.Input[Sequence[pulumi.Input[str]]] execute_steps: List of commands to execute for the job
         :param pulumi.Input[int] project_id: Project ID to create the job in
-        :param pulumi.Input[Mapping[str, pulumi.Input[bool]]] triggers: Flags for which types of triggers to use, possible values are `github_webhook`, `git_provider_webhook`, `schedule` and `custom_branch_only`. \\n\\n`custom_branch_only` is only relevant for CI jobs triggered automatically on PR creation to only trigger a job on a PR to the custom branch of the environment. To create a job in a 'deactivated' state, set all to `false`.
+        :param pulumi.Input[Mapping[str, pulumi.Input[bool]]] triggers: Flags for which types of triggers to use, the values are `github_webhook`, `git_provider_webhook`, `schedule` and `on_merge`. All flags should be listed and set with `true` or `false`. When `on_merge` is `true`, all the other values must be false.\\n\\n`custom_branch_only` used to be allowed but has been deprecated from the API. The jobs will use the custom branch of the environment. Please remove the `custom_branch_only` from your config. \\n\\nTo create a job in a 'deactivated' state, set all to `false`.
         :param pulumi.Input[str] dbt_version: Version number of dbt to use in this job, usually in the format 1.2.0-latest rather than core versions
         :param pulumi.Input[int] deferring_environment_id: Environment identifier that this job defers to (new deferring approach)
         :param pulumi.Input[int] deferring_job_id: Job identifier that this job defers to (legacy deferring approach)
         :param pulumi.Input[str] description: Description for the job
         :param pulumi.Input[bool] generate_docs: Flag for whether the job should generate documentation
         :param pulumi.Input[bool] is_active: Flag for whether the job is marked active or deleted. To create/keep a job in a 'deactivated' state, check  the `triggers` config.
         :param pulumi.Input['JobJobCompletionTriggerConditionArgs'] job_completion_trigger_condition: Which other job should trigger this job when it finishes, and on which conditions (sometimes referred as 'job chaining').
@@ -144,15 +144,15 @@
     def project_id(self, value: pulumi.Input[int]):
         pulumi.set(self, "project_id", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Input[Mapping[str, pulumi.Input[bool]]]:
         """
-        Flags for which types of triggers to use, possible values are `github_webhook`, `git_provider_webhook`, `schedule` and `custom_branch_only`. \\n\\n`custom_branch_only` is only relevant for CI jobs triggered automatically on PR creation to only trigger a job on a PR to the custom branch of the environment. To create a job in a 'deactivated' state, set all to `false`.
+        Flags for which types of triggers to use, the values are `github_webhook`, `git_provider_webhook`, `schedule` and `on_merge`. All flags should be listed and set with `true` or `false`. When `on_merge` is `true`, all the other values must be false.\\n\\n`custom_branch_only` used to be allowed but has been deprecated from the API. The jobs will use the custom branch of the environment. Please remove the `custom_branch_only` from your config. \\n\\nTo create a job in a 'deactivated' state, set all to `false`.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: pulumi.Input[Mapping[str, pulumi.Input[bool]]]):
         pulumi.set(self, "triggers", value)
 
@@ -430,15 +430,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[int]]] schedule_days: List of days of week as numbers (0 = Sunday, 7 = Saturday) to execute the job at if running on a schedule
         :param pulumi.Input[Sequence[pulumi.Input[int]]] schedule_hours: List of hours to execute the job at if running on a schedule
         :param pulumi.Input[int] schedule_interval: Number of hours between job executions if running on a schedule
         :param pulumi.Input[str] schedule_type: Type of schedule to use, one of every*day/ days*of*week/ custom*cron
         :param pulumi.Input[bool] self_deferring: Whether this job defers on a previous run of itself
         :param pulumi.Input[str] target_name: Target name for the dbt profile
         :param pulumi.Input[int] timeout_seconds: Number of seconds to allow the job to run before timing out
-        :param pulumi.Input[Mapping[str, pulumi.Input[bool]]] triggers: Flags for which types of triggers to use, possible values are `github_webhook`, `git_provider_webhook`, `schedule` and `custom_branch_only`. \\n\\n`custom_branch_only` is only relevant for CI jobs triggered automatically on PR creation to only trigger a job on a PR to the custom branch of the environment. To create a job in a 'deactivated' state, set all to `false`.
+        :param pulumi.Input[Mapping[str, pulumi.Input[bool]]] triggers: Flags for which types of triggers to use, the values are `github_webhook`, `git_provider_webhook`, `schedule` and `on_merge`. All flags should be listed and set with `true` or `false`. When `on_merge` is `true`, all the other values must be false.\\n\\n`custom_branch_only` used to be allowed but has been deprecated from the API. The jobs will use the custom branch of the environment. Please remove the `custom_branch_only` from your config. \\n\\nTo create a job in a 'deactivated' state, set all to `false`.
         :param pulumi.Input[bool] triggers_on_draft_pr: Whether the CI job should be automatically triggered on draft PRs
         """
         if dbt_version is not None:
             pulumi.set(__self__, "dbt_version", dbt_version)
         if deferring_environment_id is not None:
             pulumi.set(__self__, "deferring_environment_id", deferring_environment_id)
         if deferring_job_id is not None:
@@ -736,15 +736,15 @@
     def timeout_seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout_seconds", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[bool]]]]:
         """
-        Flags for which types of triggers to use, possible values are `github_webhook`, `git_provider_webhook`, `schedule` and `custom_branch_only`. \\n\\n`custom_branch_only` is only relevant for CI jobs triggered automatically on PR creation to only trigger a job on a PR to the custom branch of the environment. To create a job in a 'deactivated' state, set all to `false`.
+        Flags for which types of triggers to use, the values are `github_webhook`, `git_provider_webhook`, `schedule` and `on_merge`. All flags should be listed and set with `true` or `false`. When `on_merge` is `true`, all the other values must be false.\\n\\n`custom_branch_only` used to be allowed but has been deprecated from the API. The jobs will use the custom branch of the environment. Please remove the `custom_branch_only` from your config. \\n\\nTo create a job in a 'deactivated' state, set all to `false`.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[bool]]]]):
         pulumi.set(self, "triggers", value)
 
@@ -787,49 +787,48 @@
                  self_deferring: Optional[pulumi.Input[bool]] = None,
                  target_name: Optional[pulumi.Input[str]] = None,
                  timeout_seconds: Optional[pulumi.Input[int]] = None,
                  triggers: Optional[pulumi.Input[Mapping[str, pulumi.Input[bool]]]] = None,
                  triggers_on_draft_pr: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        > As of October 2023, CI improvements have been rolled out to dbt Cloud with minor impacts to some jobs:  [more info](https://docs.getdbt.com/docs/dbt-versions/release-notes/june-2023/ci-updates-phase1-rn).
+        > In October 2023, CI improvements have been rolled out to dbt Cloud with minor impacts to some jobs:  [more info](https://docs.getdbt.com/docs/dbt-versions/release-notes/june-2023/ci-updates-phase1-rn).
         <br/>
         <br/>
         Those improvements include modifications to deferral which was historically set at the job level and will now be set at the environment level.
         Deferral can still be set to "self" by setting `self_deferring` to `true` but with the new approach, deferral to other runs need to be done with `deferring_environment_id` instead of `deferring_job_id`.
 
-        > As of beginning of February 2024, job chaining with `job_completion_trigger_condition` is in private beta and not available to all users.
+        > New with 0.3.1, `triggers` now accepts a `on_merge` value to trigger jobs when code is merged in git. If `on_merge` is `true` all other triggers need to be `false`.
         <br/>
         <br/>
-        This notice will be removed once the feature is generally available.
+        For now, it is not a mandatory field, but it will be in a future version. Please add `on_merge` in your config or modules.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         # a job that has github_webhook and git_provider_webhook 
         # set to false will be categorized as a "Deploy Job"
         daily_job = dbtcloud.Job("daily_job",
             environment_id=prod_environment["environmentId"],
             execute_steps=["dbt build"],
             generate_docs=True,
             is_active=True,
             name="Daily job",
             num_threads=64,
             project_id=dbt_project["id"],
             run_generate_sources=True,
             target_name="default",
             triggers={
-                "custom_branch_only": False,
                 "github_webhook": False,
                 "git_provider_webhook": False,
                 "schedule": True,
+                "on_merge": False,
             },
             schedule_days=[
                 0,
                 1,
                 2,
                 3,
                 4,
@@ -846,18 +845,18 @@
             generate_docs=False,
             deferring_environment_id=prod_environment["environmentId"],
             name="CI Job",
             num_threads=32,
             project_id=dbt_project["id"],
             run_generate_sources=False,
             triggers={
-                "custom_branch_only": True,
                 "github_webhook": True,
                 "git_provider_webhook": True,
                 "schedule": False,
+                "on_merge": False,
             },
             schedule_days=[
                 0,
                 1,
                 2,
                 3,
                 4,
@@ -872,18 +871,18 @@
             execute_steps=["dbt build -s +my_model"],
             generate_docs=True,
             name="Downstream job in project 2",
             num_threads=32,
             project_id=dbt_project2["id"],
             run_generate_sources=True,
             triggers={
-                "custom_branch_only": False,
                 "github_webhook": False,
                 "git_provider_webhook": False,
                 "schedule": False,
+                "on_merge": False,
             },
             schedule_days=[
                 0,
                 1,
                 2,
                 3,
                 4,
@@ -896,22 +895,40 @@
                 project_id=dbt_project["id"],
                 statuses=["success"],
             ))
         ```
 
         ## Import
 
-        Import using a job ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_job.my_job
+
+          id = "job_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_job.my_job
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
-        $ pulumi import dbtcloud:index/job:Job test_job "job_id"
+        $ pulumi import dbtcloud:index/job:Job my_job "job_id"
         ```
 
         ```sh
-        $ pulumi import dbtcloud:index/job:Job test_job 12345
+        $ pulumi import dbtcloud:index/job:Job my_job 12345
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] dbt_version: Version number of dbt to use in this job, usually in the format 1.2.0-latest rather than core versions
         :param pulumi.Input[int] deferring_environment_id: Environment identifier that this job defers to (new deferring approach)
         :param pulumi.Input[int] deferring_job_id: Job identifier that this job defers to (legacy deferring approach)
@@ -929,59 +946,58 @@
         :param pulumi.Input[Sequence[pulumi.Input[int]]] schedule_days: List of days of week as numbers (0 = Sunday, 7 = Saturday) to execute the job at if running on a schedule
         :param pulumi.Input[Sequence[pulumi.Input[int]]] schedule_hours: List of hours to execute the job at if running on a schedule
         :param pulumi.Input[int] schedule_interval: Number of hours between job executions if running on a schedule
         :param pulumi.Input[str] schedule_type: Type of schedule to use, one of every*day/ days*of*week/ custom*cron
         :param pulumi.Input[bool] self_deferring: Whether this job defers on a previous run of itself
         :param pulumi.Input[str] target_name: Target name for the dbt profile
         :param pulumi.Input[int] timeout_seconds: Number of seconds to allow the job to run before timing out
-        :param pulumi.Input[Mapping[str, pulumi.Input[bool]]] triggers: Flags for which types of triggers to use, possible values are `github_webhook`, `git_provider_webhook`, `schedule` and `custom_branch_only`. \\n\\n`custom_branch_only` is only relevant for CI jobs triggered automatically on PR creation to only trigger a job on a PR to the custom branch of the environment. To create a job in a 'deactivated' state, set all to `false`.
+        :param pulumi.Input[Mapping[str, pulumi.Input[bool]]] triggers: Flags for which types of triggers to use, the values are `github_webhook`, `git_provider_webhook`, `schedule` and `on_merge`. All flags should be listed and set with `true` or `false`. When `on_merge` is `true`, all the other values must be false.\\n\\n`custom_branch_only` used to be allowed but has been deprecated from the API. The jobs will use the custom branch of the environment. Please remove the `custom_branch_only` from your config. \\n\\nTo create a job in a 'deactivated' state, set all to `false`.
         :param pulumi.Input[bool] triggers_on_draft_pr: Whether the CI job should be automatically triggered on draft PRs
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: JobArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        > As of October 2023, CI improvements have been rolled out to dbt Cloud with minor impacts to some jobs:  [more info](https://docs.getdbt.com/docs/dbt-versions/release-notes/june-2023/ci-updates-phase1-rn).
+        > In October 2023, CI improvements have been rolled out to dbt Cloud with minor impacts to some jobs:  [more info](https://docs.getdbt.com/docs/dbt-versions/release-notes/june-2023/ci-updates-phase1-rn).
         <br/>
         <br/>
         Those improvements include modifications to deferral which was historically set at the job level and will now be set at the environment level.
         Deferral can still be set to "self" by setting `self_deferring` to `true` but with the new approach, deferral to other runs need to be done with `deferring_environment_id` instead of `deferring_job_id`.
 
-        > As of beginning of February 2024, job chaining with `job_completion_trigger_condition` is in private beta and not available to all users.
+        > New with 0.3.1, `triggers` now accepts a `on_merge` value to trigger jobs when code is merged in git. If `on_merge` is `true` all other triggers need to be `false`.
         <br/>
         <br/>
-        This notice will be removed once the feature is generally available.
+        For now, it is not a mandatory field, but it will be in a future version. Please add `on_merge` in your config or modules.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         # a job that has github_webhook and git_provider_webhook 
         # set to false will be categorized as a "Deploy Job"
         daily_job = dbtcloud.Job("daily_job",
             environment_id=prod_environment["environmentId"],
             execute_steps=["dbt build"],
             generate_docs=True,
             is_active=True,
             name="Daily job",
             num_threads=64,
             project_id=dbt_project["id"],
             run_generate_sources=True,
             target_name="default",
             triggers={
-                "custom_branch_only": False,
                 "github_webhook": False,
                 "git_provider_webhook": False,
                 "schedule": True,
+                "on_merge": False,
             },
             schedule_days=[
                 0,
                 1,
                 2,
                 3,
                 4,
@@ -998,18 +1014,18 @@
             generate_docs=False,
             deferring_environment_id=prod_environment["environmentId"],
             name="CI Job",
             num_threads=32,
             project_id=dbt_project["id"],
             run_generate_sources=False,
             triggers={
-                "custom_branch_only": True,
                 "github_webhook": True,
                 "git_provider_webhook": True,
                 "schedule": False,
+                "on_merge": False,
             },
             schedule_days=[
                 0,
                 1,
                 2,
                 3,
                 4,
@@ -1024,18 +1040,18 @@
             execute_steps=["dbt build -s +my_model"],
             generate_docs=True,
             name="Downstream job in project 2",
             num_threads=32,
             project_id=dbt_project2["id"],
             run_generate_sources=True,
             triggers={
-                "custom_branch_only": False,
                 "github_webhook": False,
                 "git_provider_webhook": False,
                 "schedule": False,
+                "on_merge": False,
             },
             schedule_days=[
                 0,
                 1,
                 2,
                 3,
                 4,
@@ -1048,22 +1064,40 @@
                 project_id=dbt_project["id"],
                 statuses=["success"],
             ))
         ```
 
         ## Import
 
-        Import using a job ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_job.my_job
+
+          id = "job_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_job.my_job
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
-        $ pulumi import dbtcloud:index/job:Job test_job "job_id"
+        $ pulumi import dbtcloud:index/job:Job my_job "job_id"
         ```
 
         ```sh
-        $ pulumi import dbtcloud:index/job:Job test_job 12345
+        $ pulumi import dbtcloud:index/job:Job my_job 12345
         ```
 
         :param str resource_name: The name of the resource.
         :param JobArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -1197,15 +1231,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[int]]] schedule_days: List of days of week as numbers (0 = Sunday, 7 = Saturday) to execute the job at if running on a schedule
         :param pulumi.Input[Sequence[pulumi.Input[int]]] schedule_hours: List of hours to execute the job at if running on a schedule
         :param pulumi.Input[int] schedule_interval: Number of hours between job executions if running on a schedule
         :param pulumi.Input[str] schedule_type: Type of schedule to use, one of every*day/ days*of*week/ custom*cron
         :param pulumi.Input[bool] self_deferring: Whether this job defers on a previous run of itself
         :param pulumi.Input[str] target_name: Target name for the dbt profile
         :param pulumi.Input[int] timeout_seconds: Number of seconds to allow the job to run before timing out
-        :param pulumi.Input[Mapping[str, pulumi.Input[bool]]] triggers: Flags for which types of triggers to use, possible values are `github_webhook`, `git_provider_webhook`, `schedule` and `custom_branch_only`. \\n\\n`custom_branch_only` is only relevant for CI jobs triggered automatically on PR creation to only trigger a job on a PR to the custom branch of the environment. To create a job in a 'deactivated' state, set all to `false`.
+        :param pulumi.Input[Mapping[str, pulumi.Input[bool]]] triggers: Flags for which types of triggers to use, the values are `github_webhook`, `git_provider_webhook`, `schedule` and `on_merge`. All flags should be listed and set with `true` or `false`. When `on_merge` is `true`, all the other values must be false.\\n\\n`custom_branch_only` used to be allowed but has been deprecated from the API. The jobs will use the custom branch of the environment. Please remove the `custom_branch_only` from your config. \\n\\nTo create a job in a 'deactivated' state, set all to `false`.
         :param pulumi.Input[bool] triggers_on_draft_pr: Whether the CI job should be automatically triggered on draft PRs
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _JobState.__new__(_JobState)
 
         __props__.__dict__["dbt_version"] = dbt_version
@@ -1401,15 +1435,15 @@
         """
         return pulumi.get(self, "timeout_seconds")
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Mapping[str, bool]]:
         """
-        Flags for which types of triggers to use, possible values are `github_webhook`, `git_provider_webhook`, `schedule` and `custom_branch_only`. \\n\\n`custom_branch_only` is only relevant for CI jobs triggered automatically on PR creation to only trigger a job on a PR to the custom branch of the environment. To create a job in a 'deactivated' state, set all to `false`.
+        Flags for which types of triggers to use, the values are `github_webhook`, `git_provider_webhook`, `schedule` and `on_merge`. All flags should be listed and set with `true` or `false`. When `on_merge` is `true`, all the other values must be false.\\n\\n`custom_branch_only` used to be allowed but has been deprecated from the API. The jobs will use the custom branch of the environment. Please remove the `custom_branch_only` from your config. \\n\\nTo create a job in a 'deactivated' state, set all to `false`.
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter(name="triggersOnDraftPr")
     def triggers_on_draft_pr(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/license_map.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/license_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,22 +117,40 @@
         it_license_map = dbtcloud.LicenseMap("it_license_map",
             license_type="it",
             sso_license_mapping_groups=["IT-SSO-GROUP"])
         ```
 
         ## Import
 
-        Import using a license map ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_license_map.my_license_map
+
+          id = "license_map_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_license_map.my_license_map
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
-        $ pulumi import dbtcloud:index/licenseMap:LicenseMap test_license_map "license_map_id"
+        $ pulumi import dbtcloud:index/licenseMap:LicenseMap my_license_map "license_map_id"
         ```
 
         ```sh
-        $ pulumi import dbtcloud:index/licenseMap:LicenseMap test_license_map 12345
+        $ pulumi import dbtcloud:index/licenseMap:LicenseMap my_license_map 12345
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] license_type: License type
         :param pulumi.Input[Sequence[pulumi.Input[str]]] sso_license_mapping_groups: SSO license mapping group names for this group
         """
@@ -161,22 +179,40 @@
         it_license_map = dbtcloud.LicenseMap("it_license_map",
             license_type="it",
             sso_license_mapping_groups=["IT-SSO-GROUP"])
         ```
 
         ## Import
 
-        Import using a license map ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_license_map.my_license_map
+
+          id = "license_map_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_license_map.my_license_map
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
-        $ pulumi import dbtcloud:index/licenseMap:LicenseMap test_license_map "license_map_id"
+        $ pulumi import dbtcloud:index/licenseMap:LicenseMap my_license_map "license_map_id"
         ```
 
         ```sh
-        $ pulumi import dbtcloud:index/licenseMap:LicenseMap test_license_map 12345
+        $ pulumi import dbtcloud:index/licenseMap:LicenseMap my_license_map 12345
         ```
 
         :param str resource_name: The name of the resource.
         :param LicenseMapArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/notification.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/notification.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,21 +326,24 @@
                  on_successes: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  slack_channel_id: Optional[pulumi.Input[str]] = None,
                  slack_channel_name: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[int]] = None,
                  user_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
+        Setup notifications on jobs success/failure to internal users, external email addresses or Slack channels
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
         # dbt Cloud allows us to create internal and external notifications
+        #
         # an internal notification will send emails to the user mentioned in `user_id`
         #
         # NOTE: If internal notification settings already exist for a user, currently you MUST import
         # those first into the state file before you can create a new internal notification for that user.
         # Failure to do so, will result in the user losing access to existing notifications and dbt
         # support will need to be contacted to restore access.
         # cmd: terraform import dbtcloud_notification.prod_job_internal_notification <user_id>
@@ -370,15 +373,33 @@
             notification_type=2,
             slack_channel_id="C12345ABCDE",
             slack_channel_name="#my-awesome-channel")
         ```
 
         ## Import
 
-        Import using a notification ID
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_notification.my_notification
+
+          id = "notification_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_notification.my_notification
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/notification:Notification my_notification "notification_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/notification:Notification my_notification 12345
@@ -399,21 +420,24 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: NotificationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Setup notifications on jobs success/failure to internal users, external email addresses or Slack channels
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
         # dbt Cloud allows us to create internal and external notifications
+        #
         # an internal notification will send emails to the user mentioned in `user_id`
         #
         # NOTE: If internal notification settings already exist for a user, currently you MUST import
         # those first into the state file before you can create a new internal notification for that user.
         # Failure to do so, will result in the user losing access to existing notifications and dbt
         # support will need to be contacted to restore access.
         # cmd: terraform import dbtcloud_notification.prod_job_internal_notification <user_id>
@@ -443,15 +467,33 @@
             notification_type=2,
             slack_channel_id="C12345ABCDE",
             slack_channel_name="#my-awesome-channel")
         ```
 
         ## Import
 
-        Import using a notification ID
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_notification.my_notification
+
+          id = "notification_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_notification.my_notification
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/notification:Notification my_notification "notification_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/notification:Notification my_notification 12345
@@ -558,39 +600,39 @@
         """
         The external email to receive the notification
         """
         return pulumi.get(self, "external_email")
 
     @property
     @pulumi.getter(name="notificationType")
-    def notification_type(self) -> pulumi.Output[Optional[int]]:
+    def notification_type(self) -> pulumi.Output[int]:
         """
         Type of notification (1 = dbt Cloud user email (default): does not require an external_email ; 2 = Slack channel: requires `slack_channel_id` and `slack_channel_name` ; 4 = external email: requires setting an `external_email`)
         """
         return pulumi.get(self, "notification_type")
 
     @property
     @pulumi.getter(name="onCancels")
-    def on_cancels(self) -> pulumi.Output[Optional[Sequence[int]]]:
+    def on_cancels(self) -> pulumi.Output[Sequence[int]]:
         """
         List of job IDs to trigger the webhook on cancel
         """
         return pulumi.get(self, "on_cancels")
 
     @property
     @pulumi.getter(name="onFailures")
-    def on_failures(self) -> pulumi.Output[Optional[Sequence[int]]]:
+    def on_failures(self) -> pulumi.Output[Sequence[int]]:
         """
         List of job IDs to trigger the webhook on failure
         """
         return pulumi.get(self, "on_failures")
 
     @property
     @pulumi.getter(name="onSuccesses")
-    def on_successes(self) -> pulumi.Output[Optional[Sequence[int]]]:
+    def on_successes(self) -> pulumi.Output[Sequence[int]]:
         """
         List of job IDs to trigger the webhook on success
         """
         return pulumi.get(self, "on_successes")
 
     @property
     @pulumi.getter(name="slackChannelId")
@@ -606,15 +648,15 @@
         """
         The name of the slack channel
         """
         return pulumi.get(self, "slack_channel_name")
 
     @property
     @pulumi.getter
-    def state(self) -> pulumi.Output[Optional[int]]:
+    def state(self) -> pulumi.Output[int]:
         """
         State of the notification (1 = active (default), 2 = inactive)
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter(name="userId")
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/outputs.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/outputs.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
     'GroupGroupPermission',
+    'GroupPartialPermissionsGroupPermission',
     'JobJobCompletionTriggerCondition',
     'ServiceTokenServiceTokenPermission',
+    'GetEnvironmentsEnvironmentResult',
     'GetGroupUsersUserResult',
     'GetJobJobCompletionTriggerConditionResult',
     'GetServiceTokenServiceTokenPermissionResult',
 ]
 
 @pulumi.output_type
 class GroupGroupPermission(dict):
@@ -77,14 +79,76 @@
         """
         Project ID to apply this permission to for this group
         """
         return pulumi.get(self, "project_id")
 
 
 @pulumi.output_type
+class GroupPartialPermissionsGroupPermission(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "allProjects":
+            suggest = "all_projects"
+        elif key == "permissionSet":
+            suggest = "permission_set"
+        elif key == "projectId":
+            suggest = "project_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in GroupPartialPermissionsGroupPermission. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        GroupPartialPermissionsGroupPermission.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        GroupPartialPermissionsGroupPermission.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 all_projects: bool,
+                 permission_set: str,
+                 project_id: Optional[int] = None):
+        """
+        :param bool all_projects: Whether access should be provided for all projects or not.
+        :param str permission_set: Set of permissions to apply. The permissions allowed are the same as the ones for the `Group` resource.
+        :param int project_id: Project ID to apply this permission to for this group.
+        """
+        pulumi.set(__self__, "all_projects", all_projects)
+        pulumi.set(__self__, "permission_set", permission_set)
+        if project_id is not None:
+            pulumi.set(__self__, "project_id", project_id)
+
+    @property
+    @pulumi.getter(name="allProjects")
+    def all_projects(self) -> bool:
+        """
+        Whether access should be provided for all projects or not.
+        """
+        return pulumi.get(self, "all_projects")
+
+    @property
+    @pulumi.getter(name="permissionSet")
+    def permission_set(self) -> str:
+        """
+        Set of permissions to apply. The permissions allowed are the same as the ones for the `Group` resource.
+        """
+        return pulumi.get(self, "permission_set")
+
+    @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> Optional[int]:
+        """
+        Project ID to apply this permission to for this group.
+        """
+        return pulumi.get(self, "project_id")
+
+
+@pulumi.output_type
 class JobJobCompletionTriggerCondition(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "jobId":
             suggest = "job_id"
         elif key == "projectId":
@@ -198,14 +262,131 @@
         """
         Project ID to apply this permission to for this service token
         """
         return pulumi.get(self, "project_id")
 
 
 @pulumi.output_type
+class GetEnvironmentsEnvironmentResult(dict):
+    def __init__(__self__, *,
+                 credentials_id: int,
+                 custom_branch: str,
+                 dbt_version: str,
+                 deployment_type: str,
+                 environment_id: int,
+                 extended_attributes_id: int,
+                 name: str,
+                 project_id: int,
+                 type: str,
+                 use_custom_branch: bool):
+        """
+        :param int credentials_id: The project ID to which the environment belong
+        :param str custom_branch: The type of deployment environment (currently 'production', 'staging' or empty)
+        :param str dbt_version: Version number of dbt to use in this environment, usually in the format 1.2.0-latest rather than core versions
+        :param str deployment_type: The name of the environment
+        :param int environment_id: The ID of the environment
+        :param int extended_attributes_id: The ID of the extended attributes applied
+        :param str name: The name of the environment
+        :param int project_id: The project ID to which the environment belong
+        :param str type: The name of the environment
+        :param bool use_custom_branch: Whether to use a custom git branch in this environment
+        """
+        pulumi.set(__self__, "credentials_id", credentials_id)
+        pulumi.set(__self__, "custom_branch", custom_branch)
+        pulumi.set(__self__, "dbt_version", dbt_version)
+        pulumi.set(__self__, "deployment_type", deployment_type)
+        pulumi.set(__self__, "environment_id", environment_id)
+        pulumi.set(__self__, "extended_attributes_id", extended_attributes_id)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "project_id", project_id)
+        pulumi.set(__self__, "type", type)
+        pulumi.set(__self__, "use_custom_branch", use_custom_branch)
+
+    @property
+    @pulumi.getter(name="credentialsId")
+    def credentials_id(self) -> int:
+        """
+        The project ID to which the environment belong
+        """
+        return pulumi.get(self, "credentials_id")
+
+    @property
+    @pulumi.getter(name="customBranch")
+    def custom_branch(self) -> str:
+        """
+        The type of deployment environment (currently 'production', 'staging' or empty)
+        """
+        return pulumi.get(self, "custom_branch")
+
+    @property
+    @pulumi.getter(name="dbtVersion")
+    def dbt_version(self) -> str:
+        """
+        Version number of dbt to use in this environment, usually in the format 1.2.0-latest rather than core versions
+        """
+        return pulumi.get(self, "dbt_version")
+
+    @property
+    @pulumi.getter(name="deploymentType")
+    def deployment_type(self) -> str:
+        """
+        The name of the environment
+        """
+        return pulumi.get(self, "deployment_type")
+
+    @property
+    @pulumi.getter(name="environmentId")
+    def environment_id(self) -> int:
+        """
+        The ID of the environment
+        """
+        return pulumi.get(self, "environment_id")
+
+    @property
+    @pulumi.getter(name="extendedAttributesId")
+    def extended_attributes_id(self) -> int:
+        """
+        The ID of the extended attributes applied
+        """
+        return pulumi.get(self, "extended_attributes_id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        The name of the environment
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> int:
+        """
+        The project ID to which the environment belong
+        """
+        return pulumi.get(self, "project_id")
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        The name of the environment
+        """
+        return pulumi.get(self, "type")
+
+    @property
+    @pulumi.getter(name="useCustomBranch")
+    def use_custom_branch(self) -> bool:
+        """
+        Whether to use a custom git branch in this environment
+        """
+        return pulumi.get(self, "use_custom_branch")
+
+
+@pulumi.output_type
 class GetGroupUsersUserResult(dict):
     def __init__(__self__, *,
                  email: str,
                  id: int):
         pulumi.set(__self__, "email", email)
         pulumi.set(__self__, "id", id)
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/postgres_credential.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/postgres_credential.py`

 * *Files 5% similar despite different names*

```diff
@@ -312,28 +312,45 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         postgres_prod_credential = dbtcloud.PostgresCredential("postgres_prod_credential",
             is_active=True,
             project_id=dbt_project["id"],
             type="postgres",
             default_schema="my_schema",
             username="my_username",
             password="my_password",
             num_threads=16)
         ```
 
         ## Import
 
-        Import using a project ID and credential ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_postgres_credential.my_credential
+
+          id = "project_id:credential_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_postgres_credential.my_credential
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/postgresCredential:PostgresCredential my_credential "project_id:credential_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/postgresCredential:PostgresCredential my_credential 12345:6789
@@ -359,28 +376,45 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         postgres_prod_credential = dbtcloud.PostgresCredential("postgres_prod_credential",
             is_active=True,
             project_id=dbt_project["id"],
             type="postgres",
             default_schema="my_schema",
             username="my_username",
             password="my_password",
             num_threads=16)
         ```
 
         ## Import
 
-        Import using a project ID and credential ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_postgres_credential.my_credential
+
+          id = "project_id:credential_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_postgres_credential.my_credential
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/postgresCredential:PostgresCredential my_credential "project_id:credential_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/postgresCredential:PostgresCredential my_credential 12345:6789
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,31 +102,48 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         dbt_project = dbtcloud.Project("dbt_project", name="Analytics")
         dbt_project_with_subdir = dbtcloud.Project("dbt_project_with_subdir",
             name="Analytics in Subdir",
             dbt_project_subdirectory="/path")
         ```
 
         ## Import
 
-        Import using a project ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_project.my_project
+
+          id = "project_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_project.my_project
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
-        $ pulumi import dbtcloud:index/project:Project test_project "project_id"
+        $ pulumi import dbtcloud:index/project:Project my_project "project_id"
         ```
 
         ```sh
-        $ pulumi import dbtcloud:index/project:Project test_project 12345
+        $ pulumi import dbtcloud:index/project:Project my_project 12345
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] dbt_project_subdirectory: dbt project subdirectory path
         :param pulumi.Input[str] name: Project name
         """
@@ -139,31 +156,48 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         dbt_project = dbtcloud.Project("dbt_project", name="Analytics")
         dbt_project_with_subdir = dbtcloud.Project("dbt_project_with_subdir",
             name="Analytics in Subdir",
             dbt_project_subdirectory="/path")
         ```
 
         ## Import
 
-        Import using a project ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_project.my_project
+
+          id = "project_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_project.my_project
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
-        $ pulumi import dbtcloud:index/project:Project test_project "project_id"
+        $ pulumi import dbtcloud:index/project:Project my_project "project_id"
         ```
 
         ```sh
-        $ pulumi import dbtcloud:index/project:Project test_project 12345
+        $ pulumi import dbtcloud:index/project:Project my_project 12345
         ```
 
         :param str resource_name: The name of the resource.
         :param ProjectArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project_artefacts.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project_artefacts.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,24 +134,41 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         my_project_artefacts = dbtcloud.ProjectArtefacts("my_project_artefacts",
             project_id=dbt_project["id"],
             docs_job_id=prod_job["id"],
             freshness_job_id=prod_job["id"])
         ```
 
         ## Import
 
-        Import using a project ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_project_artefacts.my_artefacts
+
+          id = "project_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_project_artefacts.my_artefacts
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/projectArtefacts:ProjectArtefacts my_artefacts "project_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/projectArtefacts:ProjectArtefacts my_artefacts 12345
@@ -172,24 +189,41 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         my_project_artefacts = dbtcloud.ProjectArtefacts("my_project_artefacts",
             project_id=dbt_project["id"],
             docs_job_id=prod_job["id"],
             freshness_job_id=prod_job["id"])
         ```
 
         ## Import
 
-        Import using a project ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_project_artefacts.my_artefacts
+
+          id = "project_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_project_artefacts.my_artefacts
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/projectArtefacts:ProjectArtefacts my_artefacts "project_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/projectArtefacts:ProjectArtefacts my_artefacts 12345
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project_connection.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,23 +100,40 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         dbt_project_connection = dbtcloud.ProjectConnection("dbt_project_connection",
             project_id=dbt_project["id"],
             connection_id=dbt_connection["connectionId"])
         ```
 
         ## Import
 
-        Import using a project ID and Connection ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_project_connection.my_project
+
+          id = "project_id:connection_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_project_connection.my_project
+
+          id = "12345:5678"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/projectConnection:ProjectConnection my_project "project_id:connection_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/projectConnection:ProjectConnection my_project 12345:5678
@@ -136,23 +153,40 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         dbt_project_connection = dbtcloud.ProjectConnection("dbt_project_connection",
             project_id=dbt_project["id"],
             connection_id=dbt_connection["connectionId"])
         ```
 
         ## Import
 
-        Import using a project ID and Connection ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_project_connection.my_project
+
+          id = "project_id:connection_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_project_connection.my_project
+
+          id = "12345:5678"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/projectConnection:ProjectConnection my_project "project_id:connection_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/projectConnection:ProjectConnection my_project 12345:5678
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project_repository.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project_repository.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,29 +94,48 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  project_id: Optional[pulumi.Input[int]] = None,
                  repository_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
+        This resource allows you to link a dbt Cloud project to a git repository.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         dbt_project_repository = dbtcloud.ProjectRepository("dbt_project_repository",
             project_id=dbt_project["id"],
             repository_id=dbt_repository["repositoryId"])
         ```
 
         ## Import
 
-        Import using a project ID and Connection ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_project_repository.my_project
+
+          id = "project_id:repository_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_project_repository.my_project
+
+          id = "12345:5678"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/projectRepository:ProjectRepository my_project "project_id:repository_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/projectRepository:ProjectRepository my_project 12345:5678
@@ -130,29 +149,48 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        This resource allows you to link a dbt Cloud project to a git repository.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         dbt_project_repository = dbtcloud.ProjectRepository("dbt_project_repository",
             project_id=dbt_project["id"],
             repository_id=dbt_repository["repositoryId"])
         ```
 
         ## Import
 
-        Import using a project ID and Connection ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_project_repository.my_project
+
+          id = "project_id:repository_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_project_repository.my_project
+
+          id = "12345:5678"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/projectRepository:ProjectRepository my_project "project_id:repository_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/projectRepository:ProjectRepository my_project 12345:5678
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/provider.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,15 +143,17 @@
                 account_id = _utilities.get_env_int('DBT_CLOUD_ACCOUNT_ID')
             __props__.__dict__["account_id"] = pulumi.Output.from_input(account_id).apply(pulumi.runtime.to_json) if account_id is not None else None
             if host_url is None:
                 host_url = (_utilities.get_env('DBT_CLOUD_HOST_URL') or 'https://cloud.getdbt.com/api')
             __props__.__dict__["host_url"] = host_url
             if token is None:
                 token = _utilities.get_env('DBT_CLOUD_TOKEN')
-            __props__.__dict__["token"] = token
+            __props__.__dict__["token"] = None if token is None else pulumi.Output.secret(token)
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["token"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'dbtcloud',
             resource_name,
             __props__,
             opts)
 
     @property
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/repository.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,17 @@
         if azure_active_directory_project_id is not None:
             pulumi.set(__self__, "azure_active_directory_project_id", azure_active_directory_project_id)
         if azure_active_directory_repository_id is not None:
             pulumi.set(__self__, "azure_active_directory_repository_id", azure_active_directory_repository_id)
         if azure_bypass_webhook_registration_failure is not None:
             pulumi.set(__self__, "azure_bypass_webhook_registration_failure", azure_bypass_webhook_registration_failure)
         if fetch_deploy_key is not None:
+            warnings.warn("""This field is deprecated and will be removed in a future version of the provider, please remove it from your configuration. The key is always fetched when the clone strategy is `deploy_key`""", DeprecationWarning)
+            pulumi.log.warn("""fetch_deploy_key is deprecated: This field is deprecated and will be removed in a future version of the provider, please remove it from your configuration. The key is always fetched when the clone strategy is `deploy_key`""")
+        if fetch_deploy_key is not None:
             pulumi.set(__self__, "fetch_deploy_key", fetch_deploy_key)
         if git_clone_strategy is not None:
             pulumi.set(__self__, "git_clone_strategy", git_clone_strategy)
         if github_installation_id is not None:
             pulumi.set(__self__, "github_installation_id", github_installation_id)
         if gitlab_project_id is not None:
             pulumi.set(__self__, "gitlab_project_id", gitlab_project_id)
@@ -118,14 +121,17 @@
 
     @property
     @pulumi.getter(name="fetchDeployKey")
     def fetch_deploy_key(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether we should return the public deploy key - (for the `deploy_key` strategy)
         """
+        warnings.warn("""This field is deprecated and will be removed in a future version of the provider, please remove it from your configuration. The key is always fetched when the clone strategy is `deploy_key`""", DeprecationWarning)
+        pulumi.log.warn("""fetch_deploy_key is deprecated: This field is deprecated and will be removed in a future version of the provider, please remove it from your configuration. The key is always fetched when the clone strategy is `deploy_key`""")
+
         return pulumi.get(self, "fetch_deploy_key")
 
     @fetch_deploy_key.setter
     def fetch_deploy_key(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "fetch_deploy_key", value)
 
     @property
@@ -214,14 +220,17 @@
         if azure_active_directory_repository_id is not None:
             pulumi.set(__self__, "azure_active_directory_repository_id", azure_active_directory_repository_id)
         if azure_bypass_webhook_registration_failure is not None:
             pulumi.set(__self__, "azure_bypass_webhook_registration_failure", azure_bypass_webhook_registration_failure)
         if deploy_key is not None:
             pulumi.set(__self__, "deploy_key", deploy_key)
         if fetch_deploy_key is not None:
+            warnings.warn("""This field is deprecated and will be removed in a future version of the provider, please remove it from your configuration. The key is always fetched when the clone strategy is `deploy_key`""", DeprecationWarning)
+            pulumi.log.warn("""fetch_deploy_key is deprecated: This field is deprecated and will be removed in a future version of the provider, please remove it from your configuration. The key is always fetched when the clone strategy is `deploy_key`""")
+        if fetch_deploy_key is not None:
             pulumi.set(__self__, "fetch_deploy_key", fetch_deploy_key)
         if git_clone_strategy is not None:
             pulumi.set(__self__, "git_clone_strategy", git_clone_strategy)
         if github_installation_id is not None:
             pulumi.set(__self__, "github_installation_id", github_installation_id)
         if gitlab_project_id is not None:
             pulumi.set(__self__, "gitlab_project_id", gitlab_project_id)
@@ -286,14 +295,17 @@
 
     @property
     @pulumi.getter(name="fetchDeployKey")
     def fetch_deploy_key(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether we should return the public deploy key - (for the `deploy_key` strategy)
         """
+        warnings.warn("""This field is deprecated and will be removed in a future version of the provider, please remove it from your configuration. The key is always fetched when the clone strategy is `deploy_key`""", DeprecationWarning)
+        pulumi.log.warn("""fetch_deploy_key is deprecated: This field is deprecated and will be removed in a future version of the provider, please remove it from your configuration. The key is always fetched when the clone strategy is `deploy_key`""")
+
         return pulumi.get(self, "fetch_deploy_key")
 
     @fetch_deploy_key.setter
     def fetch_deploy_key(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "fetch_deploy_key", value)
 
     @property
@@ -406,35 +418,88 @@
                  github_installation_id: Optional[pulumi.Input[int]] = None,
                  gitlab_project_id: Optional[pulumi.Input[int]] = None,
                  is_active: Optional[pulumi.Input[bool]] = None,
                  project_id: Optional[pulumi.Input[int]] = None,
                  remote_url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        *Note*: Some upstream resources can be slow to create, so if creating a project at
-        the same time as the repository, it's recommended to use the `depends_on` meta argument.
+        This resource allows you to manage connections to git repositories in dbt Cloud.
+
+        By itself, this resource won't show you the repository in the dbt Cloud UI.
+        You will need to also set up a `ProjectRepository` resource as well to link your dbt Cloud project and the git repository.
 
         In order to find the `github_installation_id`, you can log in to dbt Cloud, replace `<dbt_cloud_url>` by your dbt Cloud
         URL and run the following commands in the Google Chrome console:
 
         Alternatively, you can go to the page `https://<dbt_cloud_url>/api/v2/integrations/github/installations/` and read the
         value of `id`  or use the `http` provider to retrieve it automatically like in the example below.
 
         ## Example Usage
 
-        ## Import
-
-        Import using a project ID and repository ID found in the URL or via the API.
+        ### repo cloned via the GitHub integration, manually entering the `github_installation_id`
+        resource "Repository" "github_repo" {
+          project_id             = dbtcloud_project.dbt_project.id
+          remote_url             = "git@github.com:<github_org>/<github_repo>.git"
+          github_installation_id = 9876
+          git_clone_strategy     = "github_app"
+        }
+
+        ### repo cloned via the GitHub integration, with auto-retrieval of the `github_installation_id`
+        # here, we assume that `token` and `host_url` are respectively accessible via `var.dbt_token` and `var.dbt_host_url`
+        # NOTE: the following requires connecting via a user token and can't be retrieved with a service token
+        data "http" "github_installations_response" {
+          url = format("%s/v2/integrations/github/installations/", var.dbt_host_url)
+          request_headers = {
+            Authorization = format("Bearer %s", var.dbt_token)
+          }
+        }
+
+        locals {
+          github_installation_id = jsondecode(data.http.github_installations_response.response_body)[0].id
+        }
+
+        resource "Repository" "github_repo_other" {
+          project_id             = dbtcloud_project.dbt_project.id
+          remote_url             = "git@github.com:<github_org>/<github_repo>.git"
+          github_installation_id = local.github_installation_id
+          git_clone_strategy     = "github_app"
+        }
+
+        ### repo cloned via the GitLab integration
+        # as of 15 Sept 2023 this resource requires using a user token and can't be set with a service token - CC-791
+        resource "Repository" "gitlab_repo" {
+          project_id         = dbtcloud_project.dbt_project.id
+          remote_url         = "<gitlab-group>/<gitlab-project>"
+          gitlab_project_id  = 8765
+          git_clone_strategy = "deploy_token"
+        }
+
+        ### repo cloned via the deploy token strategy
+        resource "Repository" "deploy_repo" {
+          project_id         = dbtcloud_project.dbt_project.id
+          remote_url         = "git://github.com/<github_org>/<github_repo>.git"
+          git_clone_strategy = "deploy_key"
+        }
+
+        ### repo cloned via the Azure Dev Ops integration
+        resource "Repository" "ado_repo" {
+          project_id = dbtcloud_project.dbt_project.id
+        # the following values can be added manually (IDs can be retrieved from the ADO API) or via data sources
+        # remote_url                              = "https://abc@dev.azure.com/abc/def/_git/my_repo"
+        # azure_active_directory_project_id       = "12345678-1234-1234-1234-1234567890ab"
+        # azure_active_directory_repository_id    = "87654321-4321-abcd-abcd-464327678642"
+          remote_url                                = data.dbtcloud_azure_dev_ops_repository.my_devops_repo.remote_url
+          azure_active_directory_repository_id      = data.dbtcloud_azure_dev_ops_repository.my_devops_repo.id
+          azure_active_directory_project_id         = data.dbtcloud_azure_dev_ops_project.my_devops_project.id
+          azure_bypass_webhook_registration_failure = false
+          git_clone_strategy                        = "azure_active_directory_app"
+        }
 
         ```sh
-        $ pulumi import dbtcloud:index/repository:Repository test_repository "project_id:repository_id"
-        ```
-
-        ```sh
-        $ pulumi import dbtcloud:index/repository:Repository test_repository 12345:6789
+        $ pulumi import dbtcloud:index/repository:Repository my_repository 12345:6789
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] azure_active_directory_project_id: The Azure Dev Ops project ID. It can be retrieved via the Azure API or using the data source `get_azure_dev_ops_project` and the project name - (for ADO native integration only)
         :param pulumi.Input[str] azure_active_directory_repository_id: The Azure Dev Ops repository ID. It can be retrieved via the Azure API or using the data source `get_azure_dev_ops_repository` along with the ADO Project ID and the repository name - (for ADO native integration only)
         :param pulumi.Input[bool] azure_bypass_webhook_registration_failure: If set to False (the default), the connection will fail if the service user doesn't have access to set webhooks (required for auto-triggering CI jobs). If set to True, the connection will be successful but no automated CI job will be triggered - (for ADO native integration only)
@@ -449,35 +514,88 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: RepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        *Note*: Some upstream resources can be slow to create, so if creating a project at
-        the same time as the repository, it's recommended to use the `depends_on` meta argument.
+        This resource allows you to manage connections to git repositories in dbt Cloud.
+
+        By itself, this resource won't show you the repository in the dbt Cloud UI.
+        You will need to also set up a `ProjectRepository` resource as well to link your dbt Cloud project and the git repository.
 
         In order to find the `github_installation_id`, you can log in to dbt Cloud, replace `<dbt_cloud_url>` by your dbt Cloud
         URL and run the following commands in the Google Chrome console:
 
         Alternatively, you can go to the page `https://<dbt_cloud_url>/api/v2/integrations/github/installations/` and read the
         value of `id`  or use the `http` provider to retrieve it automatically like in the example below.
 
         ## Example Usage
 
-        ## Import
-
-        Import using a project ID and repository ID found in the URL or via the API.
+        ### repo cloned via the GitHub integration, manually entering the `github_installation_id`
+        resource "Repository" "github_repo" {
+          project_id             = dbtcloud_project.dbt_project.id
+          remote_url             = "git@github.com:<github_org>/<github_repo>.git"
+          github_installation_id = 9876
+          git_clone_strategy     = "github_app"
+        }
+
+        ### repo cloned via the GitHub integration, with auto-retrieval of the `github_installation_id`
+        # here, we assume that `token` and `host_url` are respectively accessible via `var.dbt_token` and `var.dbt_host_url`
+        # NOTE: the following requires connecting via a user token and can't be retrieved with a service token
+        data "http" "github_installations_response" {
+          url = format("%s/v2/integrations/github/installations/", var.dbt_host_url)
+          request_headers = {
+            Authorization = format("Bearer %s", var.dbt_token)
+          }
+        }
+
+        locals {
+          github_installation_id = jsondecode(data.http.github_installations_response.response_body)[0].id
+        }
+
+        resource "Repository" "github_repo_other" {
+          project_id             = dbtcloud_project.dbt_project.id
+          remote_url             = "git@github.com:<github_org>/<github_repo>.git"
+          github_installation_id = local.github_installation_id
+          git_clone_strategy     = "github_app"
+        }
+
+        ### repo cloned via the GitLab integration
+        # as of 15 Sept 2023 this resource requires using a user token and can't be set with a service token - CC-791
+        resource "Repository" "gitlab_repo" {
+          project_id         = dbtcloud_project.dbt_project.id
+          remote_url         = "<gitlab-group>/<gitlab-project>"
+          gitlab_project_id  = 8765
+          git_clone_strategy = "deploy_token"
+        }
+
+        ### repo cloned via the deploy token strategy
+        resource "Repository" "deploy_repo" {
+          project_id         = dbtcloud_project.dbt_project.id
+          remote_url         = "git://github.com/<github_org>/<github_repo>.git"
+          git_clone_strategy = "deploy_key"
+        }
+
+        ### repo cloned via the Azure Dev Ops integration
+        resource "Repository" "ado_repo" {
+          project_id = dbtcloud_project.dbt_project.id
+        # the following values can be added manually (IDs can be retrieved from the ADO API) or via data sources
+        # remote_url                              = "https://abc@dev.azure.com/abc/def/_git/my_repo"
+        # azure_active_directory_project_id       = "12345678-1234-1234-1234-1234567890ab"
+        # azure_active_directory_repository_id    = "87654321-4321-abcd-abcd-464327678642"
+          remote_url                                = data.dbtcloud_azure_dev_ops_repository.my_devops_repo.remote_url
+          azure_active_directory_repository_id      = data.dbtcloud_azure_dev_ops_repository.my_devops_repo.id
+          azure_active_directory_project_id         = data.dbtcloud_azure_dev_ops_project.my_devops_project.id
+          azure_bypass_webhook_registration_failure = false
+          git_clone_strategy                        = "azure_active_directory_app"
+        }
 
         ```sh
-        $ pulumi import dbtcloud:index/repository:Repository test_repository "project_id:repository_id"
-        ```
-
-        ```sh
-        $ pulumi import dbtcloud:index/repository:Repository test_repository 12345:6789
+        $ pulumi import dbtcloud:index/repository:Repository my_repository 12345:6789
         ```
 
         :param str resource_name: The name of the resource.
         :param RepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -624,14 +742,17 @@
 
     @property
     @pulumi.getter(name="fetchDeployKey")
     def fetch_deploy_key(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether we should return the public deploy key - (for the `deploy_key` strategy)
         """
+        warnings.warn("""This field is deprecated and will be removed in a future version of the provider, please remove it from your configuration. The key is always fetched when the clone strategy is `deploy_key`""", DeprecationWarning)
+        pulumi.log.warn("""fetch_deploy_key is deprecated: This field is deprecated and will be removed in a future version of the provider, please remove it from your configuration. The key is always fetched when the clone strategy is `deploy_key`""")
+
         return pulumi.get(self, "fetch_deploy_key")
 
     @property
     @pulumi.getter(name="gitCloneStrategy")
     def git_clone_strategy(self) -> pulumi.Output[Optional[str]]:
         """
         Git clone strategy for the repository. Can be `deploy_key` (default) for cloning via SSH Deploy Key, `github_app` for GitHub native integration, `deploy_token` for the GitLab native integration and `azure_active_directory_app` for ADO native integration
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/service_token.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/service_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,14 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         test_service_token = dbtcloud.ServiceToken("test_service_token",
             name="Test Service Token",
             service_token_permissions=[
                 dbtcloud.ServiceTokenServiceTokenPermissionArgs(
                     permission_set="git_admin",
                     all_projects=True,
                 ),
@@ -187,22 +186,40 @@
                     project_id=dbt_project["id"],
                 ),
             ])
         ```
 
         ## Import
 
-        Import using a group ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_group.my_service_token
+
+          id = "service_token_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_group.my_service_token
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
-        $ pulumi import dbtcloud:index/serviceToken:ServiceToken test_service_token "service_token_id"
+        $ pulumi import dbtcloud:index/serviceToken:ServiceToken my_service_token "service_token_id"
         ```
 
         ```sh
-        $ pulumi import dbtcloud:index/serviceToken:ServiceToken test_service_token 12345
+        $ pulumi import dbtcloud:index/serviceToken:ServiceToken my_service_token 12345
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: Service token name
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceTokenServiceTokenPermissionArgs']]]] service_token_permissions: Permissions set for the service token
         :param pulumi.Input[int] state: Service token state (1 is active, 2 is inactive)
@@ -216,15 +233,14 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         test_service_token = dbtcloud.ServiceToken("test_service_token",
             name="Test Service Token",
             service_token_permissions=[
                 dbtcloud.ServiceTokenServiceTokenPermissionArgs(
                     permission_set="git_admin",
                     all_projects=True,
                 ),
@@ -234,22 +250,40 @@
                     project_id=dbt_project["id"],
                 ),
             ])
         ```
 
         ## Import
 
-        Import using a group ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_group.my_service_token
+
+          id = "service_token_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_group.my_service_token
+
+          id = "12345"
+
+        }
+
+        using the older import command
 
         ```sh
-        $ pulumi import dbtcloud:index/serviceToken:ServiceToken test_service_token "service_token_id"
+        $ pulumi import dbtcloud:index/serviceToken:ServiceToken my_service_token "service_token_id"
         ```
 
         ```sh
-        $ pulumi import dbtcloud:index/serviceToken:ServiceToken test_service_token 12345
+        $ pulumi import dbtcloud:index/serviceToken:ServiceToken my_service_token 12345
         ```
 
         :param str resource_name: The name of the resource.
         :param ServiceTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/snowflake_credential.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/snowflake_credential.py`

 * *Files 3% similar despite different names*

```diff
@@ -443,27 +443,44 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         prod_credential = dbtcloud.SnowflakeCredential("prod_credential",
             project_id=dbt_project["id"],
             auth_type="password",
             num_threads=16,
             schema="SCHEMA",
             user="user",
             password="password")
         ```
 
         ## Import
 
-        Import using a project ID and credential ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_snowflake_credential.prod_snowflake_credential
+
+          id = "project_id:credential_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_snowflake_credential.prod_snowflake_credential
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/snowflakeCredential:SnowflakeCredential prod_snowflake_credential "project_id:credential_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/snowflakeCredential:SnowflakeCredential prod_snowflake_credential 12345:6789
@@ -493,27 +510,44 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         prod_credential = dbtcloud.SnowflakeCredential("prod_credential",
             project_id=dbt_project["id"],
             auth_type="password",
             num_threads=16,
             schema="SCHEMA",
             user="user",
             password="password")
         ```
 
         ## Import
 
-        Import using a project ID and credential ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_snowflake_credential.prod_snowflake_credential
+
+          id = "project_id:credential_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_snowflake_credential.prod_snowflake_credential
+
+          id = "12345:6789"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/snowflakeCredential:SnowflakeCredential prod_snowflake_credential "project_id:credential_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/snowflakeCredential:SnowflakeCredential prod_snowflake_credential 12345:6789
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/user_groups.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/user_groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,15 +126,33 @@
             group_ids=[])
         ```
 
         ## Import
 
         Import using the User ID
 
-        The User ID can be retrieved from the dbt Cloud UI or with the data source dbtcloud_user
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_user_groups.my_user_groups
+
+          id = "user_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_user_groups.my_user_groups
+
+          id = "123456"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/userGroups:UserGroups my_user_groups "user_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/userGroups:UserGroups my_user_groups 123456
@@ -180,15 +198,33 @@
             group_ids=[])
         ```
 
         ## Import
 
         Import using the User ID
 
-        The User ID can be retrieved from the dbt Cloud UI or with the data source dbtcloud_user
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_user_groups.my_user_groups
+
+          id = "user_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_user_groups.my_user_groups
+
+          id = "123456"
+
+        }
+
+        using the older import command
 
         ```sh
         $ pulumi import dbtcloud:index/userGroups:UserGroups my_user_groups "user_id"
         ```
 
         ```sh
         $ pulumi import dbtcloud:index/userGroups:UserGroups my_user_groups 123456
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/webhook.py` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,15 +296,14 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         test_webhook = dbtcloud.Webhook("test_webhook",
             name="test-webhook",
             description="Test webhook",
             client_url="http://localhost/nothing",
             event_types=[
                 "job.run.started",
                 "job.run.completed",
@@ -313,22 +312,40 @@
                 1234,
                 5678,
             ])
         ```
 
         ## Import
 
-        Import using a job ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_webhook.my_webhook
+
+          id = "webhook_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_webhook.my_webhook
+
+          id = "wsu_abcdefg"
+
+        }
+
+        using the older import command
 
         ```sh
-        $ pulumi import dbtcloud:index/webhook:Webhook test_webhook "job_id"
+        $ pulumi import dbtcloud:index/webhook:Webhook my_webhook "webhook_id"
         ```
 
         ```sh
-        $ pulumi import dbtcloud:index/webhook:Webhook test_webhook wsu_abcdefg
+        $ pulumi import dbtcloud:index/webhook:Webhook my_webhook wsu_abcdefg
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: Webhooks active flag
         :param pulumi.Input[str] client_url: Webhooks Client URL
         :param pulumi.Input[str] description: Webhooks Description
@@ -345,15 +362,14 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_dbtcloud as dbtcloud
 
-        # NOTE for customers using the LEGACY dbt_cloud provider:
         test_webhook = dbtcloud.Webhook("test_webhook",
             name="test-webhook",
             description="Test webhook",
             client_url="http://localhost/nothing",
             event_types=[
                 "job.run.started",
                 "job.run.completed",
@@ -362,22 +378,40 @@
                 1234,
                 5678,
             ])
         ```
 
         ## Import
 
-        Import using a job ID found in the URL or via the API.
+        using  import blocks (requires Terraform >= 1.5)
+
+        import {
+
+          to = dbtcloud_webhook.my_webhook
+
+          id = "webhook_id"
+
+        }
+
+        import {
+
+          to = dbtcloud_webhook.my_webhook
+
+          id = "wsu_abcdefg"
+
+        }
+
+        using the older import command
 
         ```sh
-        $ pulumi import dbtcloud:index/webhook:Webhook test_webhook "job_id"
+        $ pulumi import dbtcloud:index/webhook:Webhook my_webhook "webhook_id"
         ```
 
         ```sh
-        $ pulumi import dbtcloud:index/webhook:Webhook test_webhook wsu_abcdefg
+        $ pulumi import dbtcloud:index/webhook:Webhook my_webhook wsu_abcdefg
         ```
 
         :param str resource_name: The name of the resource.
         :param WebhookArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/PKG-INFO` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_dbtcloud
-Version: 0.2.0a1716506595
+Version: 0.2.0a1716988489
 Summary: A Pulumi package for creating and managing dbt Cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-dbtcloud
 Keywords: pulumi,dbtcloud,dbt,cloud,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/SOURCES.txt` & `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 pulumi_dbtcloud/get_azure_dev_ops_repository.py
 pulumi_dbtcloud/get_big_query_connection.py
 pulumi_dbtcloud/get_big_query_credential.py
 pulumi_dbtcloud/get_connection.py
 pulumi_dbtcloud/get_databricks_credential.py
 pulumi_dbtcloud/get_environment.py
 pulumi_dbtcloud/get_environment_variable.py
+pulumi_dbtcloud/get_environments.py
 pulumi_dbtcloud/get_extended_attributes.py
 pulumi_dbtcloud/get_group.py
 pulumi_dbtcloud/get_group_users.py
 pulumi_dbtcloud/get_job.py
 pulumi_dbtcloud/get_notification.py
 pulumi_dbtcloud/get_postgres_credential.py
 pulumi_dbtcloud/get_privatelink_endpoint.py
@@ -32,18 +33,20 @@
 pulumi_dbtcloud/get_repository.py
 pulumi_dbtcloud/get_service_token.py
 pulumi_dbtcloud/get_snowflake_credential.py
 pulumi_dbtcloud/get_user.py
 pulumi_dbtcloud/get_user_groups.py
 pulumi_dbtcloud/get_webhook.py
 pulumi_dbtcloud/group.py
+pulumi_dbtcloud/group_partial_permissions.py
 pulumi_dbtcloud/job.py
 pulumi_dbtcloud/license_map.py
 pulumi_dbtcloud/notification.py
 pulumi_dbtcloud/outputs.py
+pulumi_dbtcloud/partial_notification.py
 pulumi_dbtcloud/postgres_credential.py
 pulumi_dbtcloud/project.py
 pulumi_dbtcloud/project_artefacts.py
 pulumi_dbtcloud/project_connection.py
 pulumi_dbtcloud/project_repository.py
 pulumi_dbtcloud/provider.py
 pulumi_dbtcloud/pulumi-plugin.json
```

### Comparing `pulumi_dbtcloud-0.2.0a1716506595/pyproject.toml` & `pulumi_dbtcloud-0.2.0a1716988489/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_dbtcloud"
   description = "A Pulumi package for creating and managing dbt Cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "dbtcloud", "dbt", "cloud", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.2.0a1716506595"
+  version = "0.2.0a1716988489"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-dbtcloud"
 
 [build-system]
```

