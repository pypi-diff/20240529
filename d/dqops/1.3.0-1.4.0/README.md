# Comparing `tmp/dqops-1.3.0.tar.gz` & `tmp/dqops-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqops-1.3.0.tar", last modified: Thu May  9 18:54:43 2024, max compression
+gzip compressed data, was "dqops-1.4.0.tar", last modified: Wed May 29 21:58:44 2024, max compression
```

## Comparing `dqops-1.3.0.tar` & `dqops-1.4.0.tar`

### file list

```diff
@@ -1,1265 +1,1268 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.475198 dqops-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-05-09 18:41:17.000000 dqops-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-09 18:54:43.475198 dqops-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-09 18:41:17.000000 dqops-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:42.963195 dqops-1.3.0/dqops/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:42.967195 dqops-1.3.0/dqops/client/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:42.967195 dqops-1.3.0/dqops/client/api/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:42.971195 dqops-1.3.0/dqops/client/api/check_results/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results/get_column_monitoring_checks_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results/get_column_partitioned_checks_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    11067 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results/get_column_profiling_checks_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    14194 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results/get_table_data_quality_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results/get_table_monitoring_checks_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results/get_table_partitioned_checks_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results/get_table_profiling_checks_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:42.975195 dqops-1.3.0/dqops/client/api/check_results_overview/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results_overview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results_overview/get_column_monitoring_checks_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results_overview/get_column_partitioned_checks_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results_overview/get_column_profiling_checks_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results_overview/get_table_monitoring_checks_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results_overview/get_table_partitioned_checks_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/check_results_overview/get_table_profiling_checks_overview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:42.979195 dqops-1.3.0/dqops/client/api/checks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/checks/create_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/checks/delete_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/checks/get_all_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/checks/get_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/checks/get_check_folder_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/checks/update_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:42.991196 dqops-1.3.0/dqops/client/api/columns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/create_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/delete_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_monitoring_checks_basic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_monitoring_checks_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_monitoring_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_monitoring_checks_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_monitoring_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_partitioned_checks_basic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_partitioned_checks_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_partitioned_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_partitioned_checks_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_partitioned_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_profiling_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_profiling_checks_basic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_profiling_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_profiling_checks_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_column_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/get_columns_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/update_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/update_column_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/update_column_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/update_column_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/update_column_monitoring_checks_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/update_column_monitoring_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/update_column_monitoring_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/update_column_partitioned_checks_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/update_column_partitioned_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/update_column_partitioned_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/update_column_profiling_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/columns/update_column_profiling_checks_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:42.999195 dqops-1.3.0/dqops/client/api/connections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/bulk_activate_connection_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/bulk_deactivate_connection_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/create_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/create_connection_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/delete_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/get_all_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/get_connection_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/get_connection_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/get_connection_common_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/get_connection_default_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/get_connection_incident_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/get_connection_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/get_connection_scheduling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/update_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/update_connection_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/update_connection_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/update_connection_default_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/update_connection_incident_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/update_connection_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/connections/update_connection_scheduling_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.003196 dqops-1.3.0/dqops/client/api/dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dashboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dashboards/get_all_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dashboards/get_dashboard_level_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dashboards/get_dashboard_level_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dashboards/get_dashboard_level_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dashboards/get_dashboard_level_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dashboards/get_dashboard_level_5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.007196 dqops-1.3.0/dqops/client/api/data_grouping_configurations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/data_grouping_configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/data_grouping_configurations/create_table_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/data_grouping_configurations/delete_table_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/data_grouping_configurations/set_table_default_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/data_grouping_configurations/update_table_grouping_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.007196 dqops-1.3.0/dqops/client/api/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/data_sources/get_remote_data_source_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/data_sources/get_remote_data_source_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/data_sources/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.015195 dqops-1.3.0/dqops/client/api/default_column_check_patterns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/delete_default_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_all_default_column_checks_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_daily_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_monthly_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_daily_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_monthly_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_profiling_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_daily_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_monthly_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_daily_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_monthly_column_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_profiling_column_checks_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.023196 dqops-1.3.0/dqops/client/api/default_table_check_patterns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/delete_default_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_all_default_table_checks_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_daily_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_monthly_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_daily_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_monthly_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_profiling_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_daily_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_monthly_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_daily_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_monthly_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_profiling_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern_target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.023196 dqops-1.3.0/dqops/client/api/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/defaults/get_default_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/defaults/get_default_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/defaults/update_default_schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/defaults/update_default_webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.027196 dqops-1.3.0/dqops/client/api/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dictionaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dictionaries/create_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dictionaries/delete_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dictionaries/download_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dictionaries/get_all_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dictionaries/get_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/dictionaries/update_dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.027196 dqops-1.3.0/dqops/client/api/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/environment/get_dqo_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/environment/get_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/environment/issue_api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.031196 dqops-1.3.0/dqops/client/api/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/errors/get_column_monitoring_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/errors/get_column_partitioned_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10967 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/errors/get_column_profiling_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/errors/get_table_monitoring_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/errors/get_table_partitioned_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/errors/get_table_profiling_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.031196 dqops-1.3.0/dqops/client/api/healthcheck/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/healthcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/healthcheck/is_healthy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.035196 dqops-1.3.0/dqops/client/api/incidents/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/incidents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/incidents/find_connection_incident_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/incidents/find_recent_incidents_on_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/incidents/get_incident.py
--rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/incidents/get_incident_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/incidents/get_incident_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/incidents/set_incident_issue_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/incidents/set_incident_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.039196 dqops-1.3.0/dqops/client/api/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/cancel_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/collect_statistics_on_data_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/collect_statistics_on_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/delete_stored_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/get_all_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/get_job_changes_since.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/import_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/is_cron_scheduler_running.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/run_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/start_cron_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/stop_cron_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/synchronize_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/wait_for_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/jobs/wait_for_run_checks_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.043196 dqops-1.3.0/dqops/client/api/labels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/labels/get_all_labels_for_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/labels/get_all_labels_for_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/labels/get_all_labels_for_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.043196 dqops-1.3.0/dqops/client/api/log_shipping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/log_shipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/log_shipping/log_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/log_shipping/log_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/log_shipping/log_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/log_shipping/log_warn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.047196 dqops-1.3.0/dqops/client/api/rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/rules/create_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/rules/delete_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/rules/get_all_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/rules/get_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/rules/get_rule_folder_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/rules/update_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.051196 dqops-1.3.0/dqops/client/api/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/schemas/get_schema_monitoring_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/schemas/get_schema_monitoring_checks_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/schemas/get_schema_partitioned_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/schemas/get_schema_partitioned_checks_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/schemas/get_schema_profiling_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/schemas/get_schema_profiling_checks_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/schemas/get_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.051196 dqops-1.3.0/dqops/client/api/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/search/find_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.051196 dqops-1.3.0/dqops/client/api/sensor_readouts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensor_readouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensor_readouts/get_column_monitoring_sensor_readouts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11674 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensor_readouts/get_column_partitioned_sensor_readouts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensor_readouts/get_column_profiling_sensor_readouts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensor_readouts/get_table_monitoring_sensor_readouts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensor_readouts/get_table_partitioned_sensor_readouts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensor_readouts/get_table_profiling_sensor_readouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.055196 dqops-1.3.0/dqops/client/api/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensors/create_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensors/delete_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensors/get_all_sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensors/get_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensors/get_sensor_folder_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/sensors/update_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.059196 dqops-1.3.0/dqops/client/api/shared_credentials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/shared_credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/shared_credentials/create_shared_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/shared_credentials/delete_shared_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/shared_credentials/download_shared_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/shared_credentials/get_all_shared_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/shared_credentials/get_shared_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/shared_credentials/update_shared_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.059196 dqops-1.3.0/dqops/client/api/table_comparison_results/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparison_results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparison_results/get_table_comparison_monitoring_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparison_results/get_table_comparison_partitioned_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparison_results/get_table_comparison_profiling_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.067196 dqops-1.3.0/dqops/client/api/table_comparisons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/create_table_comparison_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/create_table_comparison_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/delete_table_comparison_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/update_table_comparison_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/table_comparisons/update_table_comparison_profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.087196 dqops-1.3.0/dqops/client/api/tables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/create_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/delete_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_columns_monitoring_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_columns_partitioned_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_columns_profiling_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_daily_monitoring_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_daily_partitioned_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_default_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_incident_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_monitoring_checks_basic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_monitoring_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_monitoring_checks_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_monitoring_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_monitoring_checks_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_partitioned_checks_basic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_partitioned_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_partitioned_checks_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_partitioned_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_partitioned_checks_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_partitioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_profiling_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_profiling_checks_basic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_profiling_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_profiling_checks_model_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_profiling_checks_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_scheduling_group_override.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_table_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/get_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_daily_monitoring_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_default_grouping_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_incident_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_monitoring_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_monitoring_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_partitioned_checks_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     6611 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_partitioned_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_partitioned_checks_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_partitioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_profiling_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_profiling_checks_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/tables/update_table_scheduling_group_override.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.087196 dqops-1.3.0/dqops/client/api/timezones/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/timezones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/timezones/get_available_zone_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.091196 dqops-1.3.0/dqops/client/api/users/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/users/change_caller_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/users/change_user_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/users/create_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/users/delete_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/users/get_all_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/users/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/api/users/update_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.475198 dqops-1.3.0/dqops/client/models/
--rw-r--r--   0 runner    (1001) docker     (127)   128822 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/all_checks_patch_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/all_checks_patch_parameters_selected_tables_to_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_error_05_pct_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_warning_1_pct_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_error_05_pct_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_warning_1_pct_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/authenticated_dashboard_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/aws_authentication_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/azure_authentication_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/between_floats_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/between_ints_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/between_percent_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/big_query_authentication_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/big_query_jobs_create_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/big_query_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/bulk_check_deactivate_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/bulk_check_deactivate_parameters_selected_tables_to_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/change_percent_1_day_rule_10_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/change_percent_1_day_rule_20_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/change_percent_1_day_rule_50_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/change_percent_30_days_rule_10_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/change_percent_30_days_rule_20_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/change_percent_30_days_rule_50_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/change_percent_7_days_rule_10_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/change_percent_7_days_rule_20_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/change_percent_7_days_rule_50_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/change_percent_rule_10_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/change_percent_rule_20_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/change_percent_rule_50_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_container_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_container_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_container_type_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_current_data_quality_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_definition_folder_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_definition_folder_model_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_definition_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_definition_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22351 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_result_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_result_sort_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_result_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_results_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_results_overview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_run_schedule_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_search_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_target.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_target_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_time_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/check_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/cloud_synchronization_folders_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/collect_statistics_on_table_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/collect_statistics_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/collect_statistics_queue_job_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/collect_statistics_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    14850 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15128 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16655 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14997 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accepted_values_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accepted_values_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accepted_values_text_found_in_set_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11425 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_total_average_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_total_average_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_total_max_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_total_max_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_total_min_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_total_min_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_total_sum_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_accuracy_total_sum_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    22723 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    27374 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    23256 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_anomaly_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_anomaly_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_bool_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_bool_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_bool_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_bool_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_bool_false_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_bool_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_bool_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_bool_true_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_column_exists_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_column_type_hash_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_max_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_mean_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_min_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_not_null_count_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10535 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_null_count_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_comparison_sum_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10648 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_conversions_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_conversions_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_current_data_quality_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_current_data_quality_status_model_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_current_data_quality_status_model_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9980 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_custom_sql_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_custom_sql_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20452 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_daily_monitoring_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_daily_monitoring_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_daily_monitoring_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    18781 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_daily_partitioned_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_daily_partitioned_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_daily_partitioned_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datatype_detected_datatype_in_text_changed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datatype_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datatype_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datatype_string_datatype_detect_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_date_in_range_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_date_in_range_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_date_values_in_future_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8372 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datetime_date_values_in_future_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datetime_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_datetime_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_default_checks_pattern_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_detected_datatype_in_text_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_distinct_count_anomaly_differencing_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_distinct_count_anomaly_stationary_partition_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_distinct_count_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_distinct_count_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_distinct_count_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_distinct_count_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_distinct_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_distinct_percent_anomaly_stationary_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_distinct_percent_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_distinct_percent_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_distinct_percent_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_distinct_percent_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_distinct_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_duplicate_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_duplicate_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_expected_numbers_in_use_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10803 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_expected_text_values_in_use_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_expected_texts_in_top_values_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_false_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integer_in_range_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10819 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_foreign_key_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_foreign_key_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_foreign_key_not_match_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_lookup_key_not_found_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_integrity_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_invalid_email_format_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_invalid_email_format_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_invalid_ip_4_address_format_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_invalid_ip_6_address_format_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_invalid_latitude_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_invalid_longitude_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_invalid_uuid_format_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    17399 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_max_anomaly_differencing_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_max_anomaly_stationary_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_max_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_mean_anomaly_stationary_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_mean_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_mean_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_mean_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_mean_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_mean_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_median_anomaly_stationary_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_median_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_median_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10578 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_median_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_median_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_median_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_min_anomaly_differencing_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_min_anomaly_stationary_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_min_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_monitoring_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    19879 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_monthly_monitoring_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_monthly_partitioned_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_negative_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_negative_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_non_negative_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_non_negative_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_not_nulls_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_not_nulls_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_null_percent_anomaly_stationary_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_null_percent_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10699 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_null_percent_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_null_percent_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_null_percent_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    14733 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_not_nulls_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_not_nulls_count_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_not_nulls_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_not_nulls_percent_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_nulls_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_nulls_count_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_nulls_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_nulls_percent_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    15004 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_nulls_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_number_above_max_value_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_number_above_max_value_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_number_below_min_value_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_number_below_min_value_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_number_found_in_set_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_number_in_range_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    40287 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    47758 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_expected_numbers_in_use_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_integer_in_range_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_invalid_latitude_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_invalid_longitude_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_max_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_mean_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_median_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_min_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    42487 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    49106 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_negative_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_negative_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_non_negative_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_non_negative_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_number_above_max_value_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_number_above_max_value_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_number_below_min_value_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_number_below_min_value_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_number_found_in_set_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_number_in_range_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_percentile_10_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_percentile_25_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_percentile_75_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_percentile_90_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_percentile_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_population_stddev_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_population_variance_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    42302 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_sample_stddev_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_sample_variance_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_sum_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_valid_latitude_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_numeric_valid_longitude_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_partitioned_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    23750 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_invalid_email_format_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_invalid_email_format_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_invalid_ip_4_address_format_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_invalid_ip_6_address_format_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_invalid_uuid_format_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    21923 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    24282 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    21738 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_text_matching_date_pattern_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_text_matching_name_pattern_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_text_not_matching_date_pattern_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_text_not_matching_regex_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_texts_matching_regex_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_patterns_valid_uuid_format_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_percentile_10_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_percentile_25_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_percentile_75_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_percentile_90_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_percentile_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_contains_email_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_contains_email_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_contains_ip_4_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_contains_ip_4_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_contains_ip_6_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_contains_ip_6_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_contains_usa_phone_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_contains_usa_phone_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11725 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_pii_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_population_stddev_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_population_variance_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    19300 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_profiling_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_profiling_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_profiling_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_range_max_value_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_range_max_value_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_range_median_value_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_range_min_value_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_range_min_value_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_range_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_range_sum_value_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sample_stddev_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sample_variance_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sampling_column_samples_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sampling_column_samples_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sampling_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_schema_column_exists_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_schema_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_schema_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_schema_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_schema_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_schema_type_changed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sql_aggregate_expression_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sql_aggregated_expression_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10548 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sql_condition_failed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sql_condition_failed_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sql_condition_passed_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sql_condition_passed_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sql_import_custom_result_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sql_import_custom_result_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_statistics_collectors_root_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_strings_expected_text_values_in_use_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_strings_expected_texts_in_top_values_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sum_anomaly_differencing_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sum_anomaly_stationary_partition_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sum_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sum_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sum_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sum_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_sum_in_range_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16767 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10805 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_found_in_set_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_length_above_max_length_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_length_above_max_length_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_length_below_min_length_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_length_below_min_length_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_length_in_range_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_match_date_format_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_match_date_format_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_matching_date_pattern_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_matching_name_pattern_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_max_length_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_mean_length_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_min_length_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_not_matching_date_pattern_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_not_matching_regex_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_parsable_to_boolean_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_parsable_to_date_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_parsable_to_float_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_parsable_to_integer_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_datatype_detect_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_length_above_max_length_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_length_above_max_length_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_length_below_min_length_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_length_below_min_length_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_length_in_range_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_max_length_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_max_length_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_mean_length_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_mean_length_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_min_length_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_min_length_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_parsable_to_boolean_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_parsable_to_date_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_parsable_to_float_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_parsable_to_integer_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_valid_country_code_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_text_valid_currency_code_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_valid_country_code_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_text_valid_currency_code_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10802 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_texts_matching_regex_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_true_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_type_snapshot_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    23392 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    26847 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_distinct_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_distinct_count_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_distinct_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_distinct_percent_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_duplicate_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_duplicate_count_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_duplicate_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_duplicate_percent_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    23959 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_uniqueness_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_valid_latitude_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_valid_longitude_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_valid_uuid_format_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    15940 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17913 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_empty_text_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_empty_text_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_empty_text_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_empty_text_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    18227 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_null_placeholder_text_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10870 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_null_placeholder_text_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_whitespace_text_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_whitespace_text_found_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10774 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_whitespace_text_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/column_whitespace_whitespace_text_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/comment_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/common_column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/compare_thresholds_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/comparison_check_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/compression_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/connection_incident_grouping_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    22688 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/connection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/connection_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/connection_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/connection_test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/connection_test_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/count_between_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/credential_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/csv_file_format_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/custom_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/custom_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/custom_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dashboard_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dashboard_spec_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dashboards_folder_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/data_delete_result_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/data_dictionary_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/data_dictionary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/data_grouping_configuration_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/data_grouping_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/data_grouping_configuration_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/data_grouping_configuration_trimmed_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/data_grouping_dimension_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/data_grouping_dimension_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/data_type_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/databricks_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/databricks_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/datetime_built_in_date_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/default_column_checks_pattern_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/default_column_checks_pattern_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/default_schedules_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/default_table_checks_pattern_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/default_table_checks_pattern_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11837 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/delete_stored_data_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/delete_stored_data_queue_job_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/delete_stored_data_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/delete_stored_data_result_partition_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/detected_datatype_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/detected_datatype_equals_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dimension_current_data_quality_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/display_hint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_cloud_user_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_job_change_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16949 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_job_entry_parameters_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_job_history_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_job_queue_incremental_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_job_queue_initial_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_job_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_queue_job_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_root.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_settings_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_settings_model_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_settings_model_properties_additional_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_user_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/dqo_user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/duckdb_files_format_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13076 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/duckdb_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/duckdb_parameters_spec_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/duckdb_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/duckdb_read_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/duckdb_storage_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/effective_schedule_level_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/effective_schedule_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/equals_1_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/equals_integer_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/error_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/errors_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/external_log_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/field_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/file_format_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/file_synchronization_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/folder_synchronization_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/hierarchy_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/hierarchy_id_model_path_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/historic_data_points_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/import_schema_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/import_severity_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/import_tables_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/import_tables_queue_job_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/import_tables_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/incident_daily_issues_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/incident_grouping_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/incident_issue_histogram_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/incident_issue_histogram_model_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/incident_issue_histogram_model_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/incident_issue_histogram_model_days.py
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/incident_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/incident_sort_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/incident_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/incident_webhook_notifications_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/incidents_per_connection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/json_file_format_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/json_format_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/json_records_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/label_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_count_rule_0_error_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_count_rule_0_warning_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_count_rule_100_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_days_rule_1_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_days_rule_2_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_days_rule_7_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_diff_percent_rule_0_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_diff_percent_rule_1_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_diff_percent_rule_5_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_failures_rule_0_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_failures_rule_1_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_failures_rule_5_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_missing_rule_0_error_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_missing_rule_0_warning_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_missing_rule_2_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_percent_rule_0_error_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_percent_rule_0_warning_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/max_percent_rule_5_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/min_count_rule_1_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/min_percent_rule_100_error_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/min_percent_rule_100_warning_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/min_percent_rule_95_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/minimum_grouping_severity_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/monitoring_schedule_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/mono.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/mono_dqo_queue_job_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/mono_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/mono_void.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/my_sql_ssl_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/mysql_engine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/mysql_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/mysql_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/new_line_character_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/optional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/optional_incident_webhook_notifications_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/optional_monitoring_schedule_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/oracle_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/oracle_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/parameter_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/parameter_definition_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/parquet_file_format_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/partition_incremental_time_window_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/physical_table_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/postgresql_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/postgresql_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/postgresql_ssl_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/presto_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/presto_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/profiling_time_period_truncation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/provider_sensor_definition_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/provider_sensor_definition_spec_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/provider_sensor_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/provider_sensor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/provider_sensor_runner_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/provider_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/quality_category_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/redshift_authentication_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/redshift_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/redshift_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/remote_table_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/repair_stored_data_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/rule_folder_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/rule_folder_model_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/rule_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/rule_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/rule_model_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/rule_parameters_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/rule_runner_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/rule_severity_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/rule_thresholds_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/rule_time_window_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/rule_time_window_settings_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/run_checks_on_table_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/run_checks_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/run_checks_queue_job_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/run_checks_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/schedule_enabled_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13462 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/schema_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/schema_remote_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/sensor_definition_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/sensor_definition_spec_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/sensor_folder_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/sensor_folder_model_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/sensor_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/sensor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/sensor_readout_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/sensor_readouts_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/shared_credential_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/shared_credential_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/similar_check_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/single_store_db_load_balancing_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/single_store_db_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/snowflake_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/snowflake_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/spark_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/spark_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/spring_error_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/sql_server_authentication_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/sql_server_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/sql_server_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/statistics_collector_search_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/statistics_collector_target.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/statistics_data_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/statistics_metric_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/statistics_metric_model_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/statistics_result_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/synchronize_multiple_folders_dqo_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/synchronize_multiple_folders_queue_job_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/synchronize_root_folder_dqo_queue_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/synchronize_root_folder_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_accuracy_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_accuracy_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_accuracy_total_row_count_match_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_accuracy_total_row_count_match_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_availability_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_availability_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_availability_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_availability_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_availability_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_availability_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_column_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_column_list_ordered_hash_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_column_list_unordered_hash_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_column_types_hash_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_columns_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_column_count_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_column_results_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_column_results_model_column_comparison_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_configuration_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_grouping_column_pair_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_grouping_columns_pair_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_results_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_results_model_column_comparison_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_results_model_table_comparison_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_comparison_row_count_match_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    12081 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_current_data_quality_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_current_data_quality_status_model_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_current_data_quality_status_model_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_current_data_quality_status_model_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_custom_sql_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_custom_sql_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_daily_monitoring_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_daily_monitoring_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_daily_monitoring_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_daily_partitioned_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_daily_partitioned_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_daily_partitioned_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_data_freshness_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_data_ingestion_delay_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_data_staleness_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_default_checks_pattern_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_incident_grouping_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    22643 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_monitoring_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_monthly_monitoring_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_monthly_partitioned_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_owner_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_partition_reload_lag_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_partitioned_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_partitioning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_profiling_check_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_profiling_check_categories_spec_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_profiling_check_categories_spec_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_row_count_anomaly_differencing_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_row_count_anomaly_stationary_partition_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_row_count_change_1_day_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_row_count_change_30_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_row_count_change_7_days_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_row_count_change_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_row_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_schema_column_count_changed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_schema_column_count_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_schema_column_count_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_schema_column_list_changed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_schema_column_list_or_order_changed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_schema_column_types_changed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_schema_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_schema_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_schema_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_schema_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_schema_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    19622 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_spec_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_spec_groupings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_spec_table_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_sql_aggregate_expression_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_sql_aggregated_expression_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_sql_condition_failed_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_sql_condition_failed_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_sql_condition_passed_percent_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_sql_condition_passed_percent_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_sql_import_custom_result_check_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_sql_import_custom_result_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_statistics_collectors_root_categories_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_data_freshness_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_data_ingestion_delay_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_data_staleness_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_partition_reload_lag_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_timeliness_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_volume_daily_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_volume_daily_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_volume_daily_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_volume_daily_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_volume_profiling_checks_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_volume_profiling_checks_spec_custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_volume_row_count_sensor_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_volume_row_count_statistics_collector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/table_volume_statistics_collectors_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/target_column_pattern_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/target_table_pattern_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/temporal_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/text_built_in_date_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/time_period_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/time_window_filter_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/timestamp_columns_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/trino_engine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/trino_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/trino_parameters_spec_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/models/value_changed_rule_parameters_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/install.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/startdqo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-09 18:41:17.000000 dqops-1.3.0/dqops/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:54:43.475198 dqops-1.3.0/dqops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-09 18:54:42.000000 dqops-1.3.0/dqops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    78773 2024-05-09 18:54:42.000000 dqops-1.3.0/dqops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:54:42.000000 dqops-1.3.0/dqops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 18:54:42.000000 dqops-1.3.0/dqops.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-09 18:54:42.000000 dqops-1.3.0/dqops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 18:54:42.000000 dqops-1.3.0/dqops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-09 18:41:17.000000 dqops-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-09 18:54:43.475198 dqops-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-09 18:41:17.000000 dqops-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:44.212341 dqops-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-05-29 21:45:31.000000 dqops-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-29 21:58:44.212341 dqops-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-29 21:45:31.000000 dqops-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.796348 dqops-1.4.0/dqops/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.800348 dqops-1.4.0/dqops/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.800348 dqops-1.4.0/dqops/client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.804348 dqops-1.4.0/dqops/client/api/check_results/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results/get_column_monitoring_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results/get_column_partitioned_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11067 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results/get_column_profiling_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14194 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results/get_table_data_quality_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results/get_table_monitoring_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results/get_table_partitioned_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results/get_table_profiling_checks_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.804348 dqops-1.4.0/dqops/client/api/check_results_overview/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results_overview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results_overview/get_column_monitoring_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results_overview/get_column_partitioned_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results_overview/get_column_profiling_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results_overview/get_table_monitoring_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results_overview/get_table_partitioned_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/check_results_overview/get_table_profiling_checks_overview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.808348 dqops-1.4.0/dqops/client/api/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/checks/create_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/checks/delete_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/checks/get_all_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/checks/get_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/checks/get_check_folder_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/checks/update_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.820348 dqops-1.4.0/dqops/client/api/columns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/create_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/delete_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_monitoring_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_monitoring_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_monitoring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_monitoring_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_monitoring_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_partitioned_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_partitioned_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_partitioned_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_partitioned_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_profiling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_profiling_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_profiling_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_column_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/get_columns_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/update_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/update_column_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/update_column_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/update_column_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/update_column_monitoring_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/update_column_monitoring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/update_column_monitoring_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/update_column_partitioned_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/update_column_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/update_column_partitioned_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/update_column_profiling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/columns/update_column_profiling_checks_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.824348 dqops-1.4.0/dqops/client/api/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/bulk_activate_connection_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/bulk_deactivate_connection_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/create_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/create_connection_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/delete_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/get_all_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/get_connection_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/get_connection_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/get_connection_common_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/get_connection_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/get_connection_incident_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/get_connection_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/get_connection_scheduling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/update_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/update_connection_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/update_connection_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/update_connection_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/update_connection_incident_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/update_connection_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/connections/update_connection_scheduling_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.828348 dqops-1.4.0/dqops/client/api/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dashboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dashboards/get_all_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dashboards/get_dashboard_level_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dashboards/get_dashboard_level_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dashboards/get_dashboard_level_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dashboards/get_dashboard_level_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dashboards/get_dashboard_level_5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.828348 dqops-1.4.0/dqops/client/api/data_grouping_configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/data_grouping_configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/data_grouping_configurations/create_table_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/data_grouping_configurations/delete_table_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/data_grouping_configurations/set_table_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/data_grouping_configurations/update_table_grouping_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.832348 dqops-1.4.0/dqops/client/api/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/data_sources/get_remote_data_source_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/data_sources/get_remote_data_source_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/data_sources/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.836348 dqops-1.4.0/dqops/client/api/default_column_check_patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/delete_default_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_all_default_column_checks_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_daily_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_monthly_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_daily_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_monthly_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_profiling_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_daily_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_monthly_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_daily_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_monthly_column_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_profiling_column_checks_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.844348 dqops-1.4.0/dqops/client/api/default_table_check_patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/delete_default_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_all_default_table_checks_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_daily_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_monthly_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_daily_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_monthly_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_profiling_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_daily_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_monthly_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_daily_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_monthly_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_profiling_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern_target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.844348 dqops-1.4.0/dqops/client/api/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/defaults/get_default_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/defaults/get_default_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/defaults/update_default_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/defaults/update_default_webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.848348 dqops-1.4.0/dqops/client/api/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dictionaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dictionaries/create_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dictionaries/delete_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dictionaries/download_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dictionaries/get_all_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dictionaries/get_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/dictionaries/update_dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.848348 dqops-1.4.0/dqops/client/api/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/environment/get_dqo_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/environment/get_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/environment/issue_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.852347 dqops-1.4.0/dqops/client/api/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/errors/get_column_monitoring_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/errors/get_column_partitioned_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10967 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/errors/get_column_profiling_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/errors/get_table_monitoring_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/errors/get_table_partitioned_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/errors/get_table_profiling_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.852347 dqops-1.4.0/dqops/client/api/healthcheck/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/healthcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/healthcheck/is_healthy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.852347 dqops-1.4.0/dqops/client/api/incidents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/incidents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/incidents/disable_checks_for_incident.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/incidents/find_connection_incident_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/incidents/find_recent_incidents_on_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/incidents/get_incident.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/incidents/get_incident_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/incidents/get_incident_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/incidents/recalibrate_checks_for_incident.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/incidents/set_incident_issue_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/incidents/set_incident_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.860347 dqops-1.4.0/dqops/client/api/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/cancel_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/collect_statistics_on_data_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/collect_statistics_on_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/delete_stored_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/get_all_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/get_job_changes_since.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/import_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/is_cron_scheduler_running.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/run_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/start_cron_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/stop_cron_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/synchronize_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/wait_for_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/jobs/wait_for_run_checks_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.860347 dqops-1.4.0/dqops/client/api/labels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/labels/get_all_labels_for_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/labels/get_all_labels_for_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/labels/get_all_labels_for_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.860347 dqops-1.4.0/dqops/client/api/log_shipping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/log_shipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/log_shipping/log_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/log_shipping/log_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/log_shipping/log_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/log_shipping/log_warn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.864347 dqops-1.4.0/dqops/client/api/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/rules/create_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/rules/delete_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/rules/get_all_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/rules/get_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/rules/get_rule_folder_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/rules/update_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.864347 dqops-1.4.0/dqops/client/api/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/schemas/get_schema_monitoring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/schemas/get_schema_monitoring_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/schemas/get_schema_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/schemas/get_schema_partitioned_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/schemas/get_schema_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/schemas/get_schema_profiling_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/schemas/get_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.868347 dqops-1.4.0/dqops/client/api/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/search/find_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/search/find_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.868347 dqops-1.4.0/dqops/client/api/sensor_readouts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensor_readouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensor_readouts/get_column_monitoring_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11674 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensor_readouts/get_column_partitioned_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensor_readouts/get_column_profiling_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensor_readouts/get_table_monitoring_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensor_readouts/get_table_partitioned_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensor_readouts/get_table_profiling_sensor_readouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.872347 dqops-1.4.0/dqops/client/api/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensors/create_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensors/delete_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensors/get_all_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensors/get_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensors/get_sensor_folder_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/sensors/update_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.872347 dqops-1.4.0/dqops/client/api/shared_credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/shared_credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/shared_credentials/create_shared_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/shared_credentials/delete_shared_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/shared_credentials/download_shared_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/shared_credentials/get_all_shared_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/shared_credentials/get_shared_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/shared_credentials/update_shared_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.876347 dqops-1.4.0/dqops/client/api/table_comparison_results/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparison_results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparison_results/get_table_comparison_monitoring_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparison_results/get_table_comparison_partitioned_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparison_results/get_table_comparison_profiling_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.880347 dqops-1.4.0/dqops/client/api/table_comparisons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/create_table_comparison_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/create_table_comparison_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/delete_table_comparison_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/update_table_comparison_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/table_comparisons/update_table_comparison_profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.896347 dqops-1.4.0/dqops/client/api/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/create_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/delete_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_columns_monitoring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_columns_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_columns_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_daily_monitoring_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_daily_partitioned_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_incident_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_monitoring_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_monitoring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_monitoring_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_monitoring_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_monitoring_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_partitioned_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_partitioned_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_partitioned_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_partitioned_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_partitioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_profiling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_profiling_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_profiling_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_profiling_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_scheduling_group_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_table_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/get_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_daily_monitoring_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_incident_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_monitoring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_monitoring_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_partitioned_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6611 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_partitioned_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_partitioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_profiling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/tables/update_table_scheduling_group_override.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.896347 dqops-1.4.0/dqops/client/api/timezones/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/timezones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/timezones/get_available_zone_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:43.900346 dqops-1.4.0/dqops/client/api/users/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/users/change_caller_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/users/change_user_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/users/create_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/users/delete_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/users/get_all_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/users/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/api/users/update_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:44.208341 dqops-1.4.0/dqops/client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)   128822 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/all_checks_patch_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/all_checks_patch_parameters_selected_tables_to_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_error_05_pct_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_warning_1_pct_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_error_05_pct_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_warning_1_pct_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/authenticated_dashboard_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/aws_authentication_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/azure_authentication_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/between_floats_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/between_ints_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/between_percent_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/big_query_authentication_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/big_query_jobs_create_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/big_query_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/bulk_check_deactivate_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/bulk_check_deactivate_parameters_selected_tables_to_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/change_percent_1_day_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/change_percent_1_day_rule_20_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/change_percent_1_day_rule_50_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/change_percent_30_days_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/change_percent_30_days_rule_20_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/change_percent_30_days_rule_50_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/change_percent_7_days_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/change_percent_7_days_rule_20_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/change_percent_7_days_rule_50_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/change_percent_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/change_percent_rule_20_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/change_percent_rule_50_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_container_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_container_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_container_type_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_current_data_quality_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_definition_folder_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_definition_folder_model_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_definition_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_definition_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22351 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_result_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_result_sort_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_result_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_results_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_results_overview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_run_schedule_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_search_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/check_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/cloud_synchronization_folders_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/collect_statistics_on_table_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/collect_statistics_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/collect_statistics_queue_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/collect_statistics_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14850 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15128 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16655 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14997 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accepted_values_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accepted_values_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accepted_values_text_found_in_set_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11425 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_total_average_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_total_average_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_total_max_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_total_max_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_total_min_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_total_min_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_total_sum_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_accuracy_total_sum_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22723 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27374 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23256 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_anomaly_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_anomaly_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_bool_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_bool_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_bool_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_bool_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_bool_false_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_bool_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_bool_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_bool_true_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_column_exists_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_column_type_hash_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_max_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_mean_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_min_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_not_null_count_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10535 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_null_count_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_comparison_sum_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10648 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_conversions_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_conversions_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_current_data_quality_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_current_data_quality_status_model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_current_data_quality_status_model_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9980 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_custom_sql_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_custom_sql_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20452 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_daily_monitoring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_daily_monitoring_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_daily_monitoring_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18781 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_daily_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_daily_partitioned_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_daily_partitioned_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datatype_detected_datatype_in_text_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datatype_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datatype_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datatype_string_datatype_detect_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_date_in_range_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_date_in_range_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_date_values_in_future_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8372 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datetime_date_values_in_future_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datetime_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_datetime_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_default_checks_pattern_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_detected_datatype_in_text_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_distinct_count_anomaly_differencing_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_distinct_count_anomaly_stationary_partition_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_distinct_count_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_distinct_count_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_distinct_count_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_distinct_count_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_distinct_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_distinct_percent_anomaly_stationary_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_distinct_percent_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_distinct_percent_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_distinct_percent_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_distinct_percent_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_distinct_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_duplicate_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_duplicate_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_expected_numbers_in_use_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10803 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_expected_text_values_in_use_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_expected_texts_in_top_values_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_false_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integer_in_range_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10819 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_foreign_key_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_foreign_key_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_foreign_key_not_match_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_lookup_key_not_found_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_integrity_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_invalid_email_format_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_invalid_email_format_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_invalid_ip_4_address_format_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_invalid_ip_6_address_format_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_invalid_latitude_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_invalid_longitude_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_invalid_uuid_format_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18840 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_max_anomaly_differencing_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_max_anomaly_stationary_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_max_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_mean_anomaly_stationary_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_mean_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_mean_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_mean_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_mean_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_mean_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_median_anomaly_stationary_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_median_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_median_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10578 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_median_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_median_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_median_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_min_anomaly_differencing_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_min_anomaly_stationary_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_min_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_monitoring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19879 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_monthly_monitoring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_monthly_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_negative_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_negative_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_non_negative_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_non_negative_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_not_nulls_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_not_nulls_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_null_percent_anomaly_stationary_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_null_percent_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10699 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_null_percent_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_null_percent_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_null_percent_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14733 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_not_nulls_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_not_nulls_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_not_nulls_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_not_nulls_percent_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_nulls_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_nulls_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_nulls_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_nulls_percent_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15004 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_nulls_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_number_above_max_value_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_number_above_max_value_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_number_below_min_value_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_number_below_min_value_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_number_found_in_set_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_number_in_range_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40287 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47758 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_expected_numbers_in_use_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_integer_in_range_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_invalid_latitude_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_invalid_longitude_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_max_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_mean_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_median_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_min_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42487 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49106 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_negative_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_negative_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_non_negative_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_non_negative_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_number_above_max_value_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_number_above_max_value_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_number_below_min_value_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_number_below_min_value_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_number_found_in_set_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_number_in_range_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_percentile_10_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_percentile_25_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_percentile_75_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_percentile_90_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_percentile_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_population_stddev_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_population_variance_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42302 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_sample_stddev_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_sample_variance_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_sum_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_valid_latitude_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_numeric_valid_longitude_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23750 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_invalid_email_format_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_invalid_email_format_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_invalid_ip_4_address_format_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_invalid_ip_6_address_format_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_invalid_uuid_format_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21923 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24282 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21738 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_text_matching_date_pattern_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_text_matching_name_pattern_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_text_not_matching_date_pattern_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_text_not_matching_regex_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_texts_matching_regex_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_patterns_valid_uuid_format_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_percentile_10_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_percentile_25_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_percentile_75_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_percentile_90_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_percentile_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_contains_email_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_contains_email_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_contains_ip_4_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_contains_ip_4_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_contains_ip_6_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_contains_ip_6_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_contains_usa_phone_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_contains_usa_phone_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11725 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_pii_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_population_stddev_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_population_variance_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19300 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_profiling_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_profiling_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_profiling_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_range_max_value_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_range_max_value_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_range_median_value_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_range_min_value_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_range_min_value_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_range_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_range_sum_value_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sample_stddev_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sample_variance_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sampling_column_samples_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sampling_column_samples_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sampling_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_schema_column_exists_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_schema_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_schema_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_schema_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_schema_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_schema_type_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sql_aggregate_expression_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sql_aggregated_expression_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10548 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sql_condition_failed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sql_condition_failed_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sql_condition_passed_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sql_condition_passed_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sql_import_custom_result_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sql_import_custom_result_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_statistics_collectors_root_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_strings_expected_text_values_in_use_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_strings_expected_texts_in_top_values_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sum_anomaly_differencing_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sum_anomaly_stationary_partition_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sum_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sum_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sum_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sum_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_sum_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16767 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10805 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_found_in_set_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_length_above_max_length_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_length_above_max_length_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_length_below_min_length_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_length_below_min_length_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_length_in_range_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_match_date_format_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_match_date_format_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_matching_date_pattern_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_matching_name_pattern_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_max_length_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_mean_length_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_min_length_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_not_matching_date_pattern_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_not_matching_regex_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_parsable_to_boolean_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_parsable_to_date_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_parsable_to_float_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_parsable_to_integer_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_datatype_detect_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_length_above_max_length_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_length_above_max_length_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_length_below_min_length_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_length_below_min_length_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_length_in_range_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_max_length_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_max_length_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_mean_length_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_mean_length_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_min_length_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_min_length_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_parsable_to_boolean_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_parsable_to_date_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_parsable_to_float_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_parsable_to_integer_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_valid_country_code_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_text_valid_currency_code_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_valid_country_code_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_text_valid_currency_code_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10802 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_texts_matching_regex_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_true_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_type_snapshot_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23392 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26847 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_distinct_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_distinct_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_distinct_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_distinct_percent_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_duplicate_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_duplicate_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_duplicate_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_duplicate_percent_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23959 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_uniqueness_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_valid_latitude_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_valid_longitude_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_valid_uuid_format_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15940 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17913 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_empty_text_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_empty_text_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_empty_text_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_empty_text_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18227 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_null_placeholder_text_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10870 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_null_placeholder_text_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_whitespace_text_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_whitespace_text_found_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10774 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_whitespace_text_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/column_whitespace_whitespace_text_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/comment_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/common_column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/compare_thresholds_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/comparison_check_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/compression_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/connection_incident_grouping_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22688 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/connection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/connection_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/connection_specification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/connection_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/connection_test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/count_between_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/credential_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/csv_file_format_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/custom_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/custom_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/custom_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dashboard_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dashboard_spec_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dashboards_folder_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/data_delete_result_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/data_dictionary_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/data_dictionary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/data_grouping_configuration_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/data_grouping_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/data_grouping_configuration_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/data_grouping_configuration_trimmed_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/data_grouping_dimension_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/data_grouping_dimension_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/data_type_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/databricks_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/databricks_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/datetime_built_in_date_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/default_column_checks_pattern_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/default_column_checks_pattern_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/default_schedules_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/default_table_checks_pattern_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/default_table_checks_pattern_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11837 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/delete_stored_data_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/delete_stored_data_queue_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/delete_stored_data_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/delete_stored_data_result_partition_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/detected_datatype_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/detected_datatype_equals_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dimension_current_data_quality_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/display_hint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_cloud_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_job_change_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16949 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_job_entry_parameters_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_job_history_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_job_queue_incremental_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_job_queue_initial_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_queue_job_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_settings_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_settings_model_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_settings_model_properties_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_user_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/dqo_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/duckdb_files_format_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13076 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/duckdb_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/duckdb_parameters_spec_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/duckdb_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/duckdb_read_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/duckdb_storage_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/effective_schedule_level_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/effective_schedule_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/equals_1_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/equals_integer_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/error_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/errors_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/external_log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/field_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/file_format_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/file_synchronization_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/folder_synchronization_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/hierarchy_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/hierarchy_id_model_path_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/historic_data_points_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/import_schema_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/import_severity_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/import_tables_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/import_tables_queue_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/import_tables_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/incident_daily_issues_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/incident_grouping_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/incident_issue_histogram_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/incident_issue_histogram_model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/incident_issue_histogram_model_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/incident_issue_histogram_model_days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/incident_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/incident_sort_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/incident_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/incident_webhook_notifications_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/incidents_per_connection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/json_file_format_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/json_format_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/json_records_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/label_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_count_rule_0_error_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_count_rule_0_warning_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_count_rule_100_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_days_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_days_rule_2_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_days_rule_7_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_diff_percent_rule_0_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_diff_percent_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_diff_percent_rule_5_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_failures_rule_0_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_failures_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_failures_rule_5_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_missing_rule_0_error_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_missing_rule_0_warning_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_missing_rule_2_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_percent_rule_0_error_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_percent_rule_0_warning_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/max_percent_rule_5_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/min_count_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/min_percent_rule_100_error_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/min_percent_rule_100_warning_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/min_percent_rule_95_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/minimum_grouping_severity_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/monitoring_schedule_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/mono.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/mono_dqo_queue_job_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/mono_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/mono_void.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/my_sql_ssl_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/mysql_engine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/mysql_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/mysql_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/new_line_character_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/optional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/optional_incident_webhook_notifications_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/optional_monitoring_schedule_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/oracle_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/oracle_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/parameter_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/parameter_definition_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/parquet_file_format_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/partition_incremental_time_window_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/physical_table_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/postgresql_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/postgresql_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/postgresql_ssl_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/presto_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/presto_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/profiling_time_period_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/provider_sensor_definition_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/provider_sensor_definition_spec_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/provider_sensor_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/provider_sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/provider_sensor_runner_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/provider_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/quality_category_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/redshift_authentication_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/redshift_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/redshift_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/remote_table_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/repair_stored_data_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/rule_folder_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/rule_folder_model_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/rule_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/rule_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/rule_model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/rule_parameters_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/rule_runner_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/rule_severity_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/rule_thresholds_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/rule_time_window_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/rule_time_window_settings_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/run_checks_on_table_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/run_checks_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/run_checks_queue_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/run_checks_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/schedule_enabled_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13462 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/schema_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/schema_remote_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/sensor_definition_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/sensor_definition_spec_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/sensor_folder_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/sensor_folder_model_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/sensor_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/sensor_readout_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/sensor_readouts_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/shared_credential_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/shared_credential_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/similar_check_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/single_store_db_load_balancing_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/single_store_db_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/snowflake_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/snowflake_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/spark_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/spark_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/spring_error_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/sql_server_authentication_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/sql_server_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/sql_server_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/statistics_collector_search_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/statistics_collector_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/statistics_data_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/statistics_metric_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/statistics_metric_model_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/statistics_result_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/synchronize_multiple_folders_dqo_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/synchronize_multiple_folders_queue_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/synchronize_root_folder_dqo_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/synchronize_root_folder_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_accuracy_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_accuracy_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_accuracy_total_row_count_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_accuracy_total_row_count_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_availability_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_availability_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_availability_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_availability_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_availability_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_availability_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_column_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_column_list_ordered_hash_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_column_list_unordered_hash_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_column_types_hash_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_columns_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_column_count_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_column_results_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_column_results_model_column_comparison_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_configuration_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_grouping_column_pair_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_grouping_columns_pair_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_results_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_results_model_column_comparison_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_results_model_table_comparison_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_comparison_row_count_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12081 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_current_data_quality_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_current_data_quality_status_model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_current_data_quality_status_model_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_current_data_quality_status_model_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_custom_sql_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_custom_sql_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_daily_monitoring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_daily_monitoring_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_daily_monitoring_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_daily_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_daily_partitioned_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_daily_partitioned_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_data_freshness_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_data_ingestion_delay_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_data_staleness_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_default_checks_pattern_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_incident_grouping_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22643 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_monitoring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_monthly_monitoring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_monthly_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_owner_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_partition_reload_lag_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_partitioning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_profiling_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_profiling_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_profiling_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_row_count_anomaly_differencing_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_row_count_anomaly_stationary_partition_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_row_count_change_1_day_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_row_count_change_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_row_count_change_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_row_count_change_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_row_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_schema_column_count_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_schema_column_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_schema_column_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_schema_column_list_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_schema_column_list_or_order_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_schema_column_types_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_schema_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_schema_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_schema_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_schema_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_schema_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19622 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_spec_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_spec_groupings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_spec_table_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_sql_aggregate_expression_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_sql_aggregated_expression_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_sql_condition_failed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_sql_condition_failed_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_sql_condition_passed_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_sql_condition_passed_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_sql_import_custom_result_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_sql_import_custom_result_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_statistics_collectors_root_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_data_freshness_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_data_ingestion_delay_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_data_staleness_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_partition_reload_lag_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_timeliness_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_volume_daily_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_volume_daily_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_volume_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_volume_daily_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_volume_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_volume_profiling_checks_spec_custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_volume_row_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_volume_row_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/table_volume_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/target_column_pattern_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/target_table_pattern_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/temporal_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/text_built_in_date_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/time_period_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/time_window_filter_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/timestamp_columns_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/trino_engine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/trino_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/trino_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/models/value_changed_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/startdqo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-29 21:45:31.000000 dqops-1.4.0/dqops/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:58:44.208341 dqops-1.4.0/dqops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-29 21:58:43.000000 dqops-1.4.0/dqops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    78933 2024-05-29 21:58:43.000000 dqops-1.4.0/dqops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:58:43.000000 dqops-1.4.0/dqops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 21:58:43.000000 dqops-1.4.0/dqops.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-29 21:58:43.000000 dqops-1.4.0/dqops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 21:58:43.000000 dqops-1.4.0/dqops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-29 21:45:31.000000 dqops-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 21:58:44.212341 dqops-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-29 21:45:31.000000 dqops-1.4.0/setup.py
```

### Comparing `dqops-1.3.0/LICENSE` & `dqops-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/PKG-INFO` & `dqops-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqops
-Version: 1.3.0
+Version: 1.4.0
 Summary: DQOps Data Quality Operations Center
 Home-page: https://github.com/dqops/dqo/tree/master/distribution/python
 Author: DQOps Developers
 Author-email: support@dqops.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dqops-1.3.0/README.md` & `dqops-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/__init__.py` & `dqops-1.4.0/dqops/__init__.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/__main__.py` & `dqops-1.4.0/dqops/__main__.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/check_results/get_column_monitoring_checks_results.py` & `dqops-1.4.0/dqops/client/api/check_results/get_column_monitoring_checks_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/check_results/get_column_partitioned_checks_results.py` & `dqops-1.4.0/dqops/client/api/check_results/get_column_partitioned_checks_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/check_results/get_column_profiling_checks_results.py` & `dqops-1.4.0/dqops/client/api/check_results/get_column_profiling_checks_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/check_results/get_table_data_quality_status.py` & `dqops-1.4.0/dqops/client/api/check_results/get_table_data_quality_status.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/check_results/get_table_monitoring_checks_results.py` & `dqops-1.4.0/dqops/client/api/check_results/get_table_monitoring_checks_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/check_results/get_table_partitioned_checks_results.py` & `dqops-1.4.0/dqops/client/api/check_results/get_table_partitioned_checks_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/check_results/get_table_profiling_checks_results.py` & `dqops-1.4.0/dqops/client/api/check_results/get_table_profiling_checks_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/check_results_overview/get_column_monitoring_checks_overview.py` & `dqops-1.4.0/dqops/client/api/check_results_overview/get_column_monitoring_checks_overview.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/check_results_overview/get_column_partitioned_checks_overview.py` & `dqops-1.4.0/dqops/client/api/check_results_overview/get_column_partitioned_checks_overview.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/check_results_overview/get_column_profiling_checks_overview.py` & `dqops-1.4.0/dqops/client/api/check_results_overview/get_column_profiling_checks_overview.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/check_results_overview/get_table_monitoring_checks_overview.py` & `dqops-1.4.0/dqops/client/api/check_results_overview/get_table_monitoring_checks_overview.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/check_results_overview/get_table_partitioned_checks_overview.py` & `dqops-1.4.0/dqops/client/api/check_results_overview/get_table_partitioned_checks_overview.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/check_results_overview/get_table_profiling_checks_overview.py` & `dqops-1.4.0/dqops/client/api/check_results_overview/get_table_profiling_checks_overview.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/checks/create_check.py` & `dqops-1.4.0/dqops/client/api/checks/create_check.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/checks/delete_check.py` & `dqops-1.4.0/dqops/client/api/checks/delete_check.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/checks/get_all_checks.py` & `dqops-1.4.0/dqops/client/api/checks/get_all_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/checks/get_check.py` & `dqops-1.4.0/dqops/client/api/checks/get_check.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/checks/get_check_folder_tree.py` & `dqops-1.4.0/dqops/client/api/checks/get_check_folder_tree.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/checks/update_check.py` & `dqops-1.4.0/dqops/client/api/checks/update_check.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/create_column.py` & `dqops-1.4.0/dqops/client/api/columns/create_column.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/delete_column.py` & `dqops-1.4.0/dqops/client/api/columns/delete_column.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column.py` & `dqops-1.4.0/dqops/client/api/columns/get_column.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_basic.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_comments.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_comments.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_labels.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_labels.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_monitoring_checks_basic_model.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_monitoring_checks_basic_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_monitoring_checks_daily.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_monitoring_checks_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_monitoring_checks_model.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_monitoring_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_monitoring_checks_model_filter.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_monitoring_checks_model_filter.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_monitoring_checks_monthly.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_monitoring_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_partitioned_checks_basic_model.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_partitioned_checks_basic_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_partitioned_checks_daily.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_partitioned_checks_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_partitioned_checks_model.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_partitioned_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_partitioned_checks_model_filter.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_partitioned_checks_model_filter.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_partitioned_checks_monthly.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_partitioned_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_profiling_checks.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_profiling_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_profiling_checks_basic_model.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_profiling_checks_basic_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_profiling_checks_model.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_profiling_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_profiling_checks_model_filter.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_profiling_checks_model_filter.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_column_statistics.py` & `dqops-1.4.0/dqops/client/api/columns/get_column_statistics.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_columns.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_labels.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,86 +1,80 @@
 from http import HTTPStatus
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union, cast
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.column_list_model import ColumnListModel
 from ...types import Response
 
 
 def _get_kwargs(
     connection_name: str,
     schema_name: str,
     table_name: str,
 ) -> Dict[str, Any]:
     pass
 
     return {
         "method": "get",
-        "url": "api/connections/{connectionName}/schemas/{schemaName}/tables/{tableName}/columns".format(
+        "url": "api/connections/{connectionName}/schemas/{schemaName}/tables/{tableName}/labels".format(
             connectionName=connection_name,
             schemaName=schema_name,
             tableName=table_name,
         ),
     }
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[List["ColumnListModel"]]:
+) -> Optional[List[str]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in _response_200:
-            response_200_item = ColumnListModel.from_dict(response_200_item_data)
-
-            response_200.append(response_200_item)
+        response_200 = cast(List[str], response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[List["ColumnListModel"]]:
+) -> Response[List[str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     connection_name: str,
     schema_name: str,
     table_name: str,
     *,
     client: AuthenticatedClient,
-) -> Response[List["ColumnListModel"]]:
-    """getColumns
+) -> Response[List[str]]:
+    """getTableLabels
 
-     Returns a list of columns inside a table
+     Return the list of labels assigned to a table
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['ColumnListModel']]
+        Response[List[str]]
     """
 
     kwargs = _get_kwargs(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
     )
@@ -94,30 +88,30 @@
 
 def sync(
     connection_name: str,
     schema_name: str,
     table_name: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[List["ColumnListModel"]]:
-    """getColumns
+) -> Optional[List[str]]:
+    """getTableLabels
 
-     Returns a list of columns inside a table
+     Return the list of labels assigned to a table
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['ColumnListModel']
+        List[str]
     """
 
     return sync_detailed(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
         client=client,
@@ -126,30 +120,30 @@
 
 async def asyncio_detailed(
     connection_name: str,
     schema_name: str,
     table_name: str,
     *,
     client: AuthenticatedClient,
-) -> Response[List["ColumnListModel"]]:
-    """getColumns
+) -> Response[List[str]]:
+    """getTableLabels
 
-     Returns a list of columns inside a table
+     Return the list of labels assigned to a table
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['ColumnListModel']]
+        Response[List[str]]
     """
 
     kwargs = _get_kwargs(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
     )
@@ -161,30 +155,30 @@
 
 async def asyncio(
     connection_name: str,
     schema_name: str,
     table_name: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[List["ColumnListModel"]]:
-    """getColumns
+) -> Optional[List[str]]:
+    """getTableLabels
 
-     Returns a list of columns inside a table
+     Return the list of labels assigned to a table
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['ColumnListModel']
+        List[str]
     """
 
     return (
         await asyncio_detailed(
             connection_name=connection_name,
             schema_name=schema_name,
             table_name=table_name,
```

### Comparing `dqops-1.3.0/dqops/client/api/columns/get_columns_statistics.py` & `dqops-1.4.0/dqops/client/api/columns/get_columns_statistics.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/update_column.py` & `dqops-1.4.0/dqops/client/api/columns/update_column.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/update_column_basic.py` & `dqops-1.4.0/dqops/client/api/columns/update_column_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/update_column_comments.py` & `dqops-1.4.0/dqops/client/api/columns/update_column_comments.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/update_column_labels.py` & `dqops-1.4.0/dqops/client/api/columns/update_column_labels.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/update_column_monitoring_checks_daily.py` & `dqops-1.4.0/dqops/client/api/columns/update_column_monitoring_checks_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/update_column_monitoring_checks_model.py` & `dqops-1.4.0/dqops/client/api/columns/update_column_monitoring_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/update_column_monitoring_checks_monthly.py` & `dqops-1.4.0/dqops/client/api/columns/update_column_monitoring_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/update_column_partitioned_checks_daily.py` & `dqops-1.4.0/dqops/client/api/columns/update_column_partitioned_checks_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/update_column_partitioned_checks_model.py` & `dqops-1.4.0/dqops/client/api/columns/update_column_partitioned_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/update_column_partitioned_checks_monthly.py` & `dqops-1.4.0/dqops/client/api/columns/update_column_partitioned_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/update_column_profiling_checks.py` & `dqops-1.4.0/dqops/client/api/columns/update_column_profiling_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/columns/update_column_profiling_checks_model.py` & `dqops-1.4.0/dqops/client/api/columns/update_column_profiling_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/bulk_activate_connection_checks.py` & `dqops-1.4.0/dqops/client/api/connections/bulk_activate_connection_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/bulk_deactivate_connection_checks.py` & `dqops-1.4.0/dqops/client/api/connections/bulk_deactivate_connection_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/create_connection.py` & `dqops-1.4.0/dqops/client/api/connections/create_connection.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/create_connection_basic.py` & `dqops-1.4.0/dqops/client/api/connections/create_connection_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/delete_connection.py` & `dqops-1.4.0/dqops/client/api/connections/delete_connection.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/get_all_connections.py` & `dqops-1.4.0/dqops/client/api/connections/get_all_connections.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/get_connection.py` & `dqops-1.4.0/dqops/client/api/connections/get_connection.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/get_connection_basic.py` & `dqops-1.4.0/dqops/client/api/connections/get_connection_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/get_connection_comments.py` & `dqops-1.4.0/dqops/client/api/connections/get_connection_comments.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/get_connection_common_columns.py` & `dqops-1.4.0/dqops/client/api/connections/get_connection_common_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/get_connection_default_grouping_configuration.py` & `dqops-1.4.0/dqops/client/api/connections/get_connection_default_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/get_connection_incident_grouping.py` & `dqops-1.4.0/dqops/client/api/connections/get_connection_incident_grouping.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/get_connection_labels.py` & `dqops-1.4.0/dqops/client/api/connections/get_connection_labels.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/get_connection_scheduling_group.py` & `dqops-1.4.0/dqops/client/api/connections/get_connection_scheduling_group.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/update_connection.py` & `dqops-1.4.0/dqops/client/api/connections/update_connection.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/update_connection_basic.py` & `dqops-1.4.0/dqops/client/api/connections/update_connection_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/update_connection_comments.py` & `dqops-1.4.0/dqops/client/api/connections/update_connection_comments.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/update_connection_default_grouping_configuration.py` & `dqops-1.4.0/dqops/client/api/connections/update_connection_default_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/update_connection_incident_grouping.py` & `dqops-1.4.0/dqops/client/api/connections/update_connection_incident_grouping.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/update_connection_labels.py` & `dqops-1.4.0/dqops/client/api/connections/update_connection_labels.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/connections/update_connection_scheduling_group.py` & `dqops-1.4.0/dqops/client/api/connections/update_connection_scheduling_group.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/dashboards/get_all_dashboards.py` & `dqops-1.4.0/dqops/client/api/dashboards/get_all_dashboards.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/dashboards/get_dashboard_level_1.py` & `dqops-1.4.0/dqops/client/api/dashboards/get_dashboard_level_1.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/dashboards/get_dashboard_level_2.py` & `dqops-1.4.0/dqops/client/api/dashboards/get_dashboard_level_2.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/dashboards/get_dashboard_level_3.py` & `dqops-1.4.0/dqops/client/api/dashboards/get_dashboard_level_3.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/dashboards/get_dashboard_level_4.py` & `dqops-1.4.0/dqops/client/api/dashboards/get_dashboard_level_4.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/dashboards/get_dashboard_level_5.py` & `dqops-1.4.0/dqops/client/api/dashboards/get_dashboard_level_5.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/data_grouping_configurations/create_table_grouping_configuration.py` & `dqops-1.4.0/dqops/client/api/data_grouping_configurations/create_table_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/data_grouping_configurations/delete_table_grouping_configuration.py` & `dqops-1.4.0/dqops/client/api/data_grouping_configurations/delete_table_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configuration.py` & `dqops-1.4.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configurations.py` & `dqops-1.4.0/dqops/client/api/data_grouping_configurations/get_table_grouping_configurations.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/data_grouping_configurations/set_table_default_grouping_configuration.py` & `dqops-1.4.0/dqops/client/api/data_grouping_configurations/set_table_default_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/data_grouping_configurations/update_table_grouping_configuration.py` & `dqops-1.4.0/dqops/client/api/data_grouping_configurations/update_table_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/data_sources/get_remote_data_source_schemas.py` & `dqops-1.4.0/dqops/client/api/data_sources/get_remote_data_source_schemas.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/data_sources/get_remote_data_source_tables.py` & `dqops-1.4.0/dqops/client/api/data_sources/get_remote_data_source_tables.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/data_sources/test_connection.py` & `dqops-1.4.0/dqops/client/api/data_sources/test_connection.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern_target.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/create_default_column_checks_pattern_target.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/delete_default_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/delete_default_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_all_default_column_checks_patterns.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_all_default_column_checks_patterns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern_target.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_column_checks_pattern_target.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_daily_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_daily_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_monthly_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_monitoring_monthly_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_daily_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_daily_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_monthly_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_partitioned_monthly_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/get_default_profiling_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/get_default_profiling_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern_target.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_column_checks_pattern_target.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_daily_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_daily_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_monthly_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_monitoring_monthly_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_daily_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_daily_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_monthly_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_partitioned_monthly_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_column_check_patterns/update_default_profiling_column_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_column_check_patterns/update_default_profiling_column_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern_target.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/create_default_table_checks_pattern_target.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/delete_default_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/delete_default_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_all_default_table_checks_patterns.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_all_default_table_checks_patterns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_daily_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_daily_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_monthly_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_monitoring_monthly_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_daily_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_daily_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_monthly_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_partitioned_monthly_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_profiling_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_profiling_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern_target.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/get_default_table_checks_pattern_target.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_daily_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_daily_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_monthly_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_monitoring_monthly_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_daily_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_daily_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_monthly_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_partitioned_monthly_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_profiling_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_profiling_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern_target.py` & `dqops-1.4.0/dqops/client/api/default_table_check_patterns/update_default_table_checks_pattern_target.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/defaults/get_default_schedule.py` & `dqops-1.4.0/dqops/client/api/defaults/get_default_schedule.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/defaults/get_default_webhooks.py` & `dqops-1.4.0/dqops/client/api/defaults/get_default_webhooks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/defaults/update_default_schedules.py` & `dqops-1.4.0/dqops/client/api/defaults/update_default_schedules.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/defaults/update_default_webhooks.py` & `dqops-1.4.0/dqops/client/api/defaults/update_default_webhooks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/dictionaries/create_dictionary.py` & `dqops-1.4.0/dqops/client/api/dictionaries/create_dictionary.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/dictionaries/delete_dictionary.py` & `dqops-1.4.0/dqops/client/api/dictionaries/delete_dictionary.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/dictionaries/download_dictionary.py` & `dqops-1.4.0/dqops/client/api/dictionaries/download_dictionary.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/dictionaries/get_all_dictionaries.py` & `dqops-1.4.0/dqops/client/api/dictionaries/get_all_dictionaries.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/dictionaries/get_dictionary.py` & `dqops-1.4.0/dqops/client/api/dictionaries/get_dictionary.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/dictionaries/update_dictionary.py` & `dqops-1.4.0/dqops/client/api/dictionaries/update_dictionary.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/environment/get_dqo_settings.py` & `dqops-1.4.0/dqops/client/api/environment/get_dqo_settings.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/environment/get_user_profile.py` & `dqops-1.4.0/dqops/client/api/environment/get_user_profile.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/environment/issue_api_key.py` & `dqops-1.4.0/dqops/client/api/environment/issue_api_key.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/errors/get_column_monitoring_errors.py` & `dqops-1.4.0/dqops/client/api/errors/get_column_monitoring_errors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/errors/get_column_partitioned_errors.py` & `dqops-1.4.0/dqops/client/api/errors/get_column_partitioned_errors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/errors/get_column_profiling_errors.py` & `dqops-1.4.0/dqops/client/api/errors/get_column_profiling_errors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/errors/get_table_monitoring_errors.py` & `dqops-1.4.0/dqops/client/api/errors/get_table_monitoring_errors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/errors/get_table_partitioned_errors.py` & `dqops-1.4.0/dqops/client/api/errors/get_table_partitioned_errors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/errors/get_table_profiling_errors.py` & `dqops-1.4.0/dqops/client/api/errors/get_table_profiling_errors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/healthcheck/is_healthy.py` & `dqops-1.4.0/dqops/client/api/healthcheck/is_healthy.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/incidents/find_connection_incident_stats.py` & `dqops-1.4.0/dqops/client/api/incidents/find_connection_incident_stats.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/incidents/find_recent_incidents_on_connection.py` & `dqops-1.4.0/dqops/client/api/incidents/find_recent_incidents_on_connection.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/incidents/get_incident.py` & `dqops-1.4.0/dqops/client/api/incidents/get_incident.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/incidents/get_incident_histogram.py` & `dqops-1.4.0/dqops/client/api/incidents/get_incident_histogram.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/incidents/get_incident_issues.py` & `dqops-1.4.0/dqops/client/api/incidents/get_incident_issues.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/incidents/set_incident_issue_url.py` & `dqops-1.4.0/dqops/client/api/incidents/set_incident_issue_url.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/incidents/set_incident_status.py` & `dqops-1.4.0/dqops/client/api/incidents/set_incident_status.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/cancel_job.py` & `dqops-1.4.0/dqops/client/api/jobs/cancel_job.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/collect_statistics_on_data_groups.py` & `dqops-1.4.0/dqops/client/api/jobs/collect_statistics_on_data_groups.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/collect_statistics_on_table.py` & `dqops-1.4.0/dqops/client/api/jobs/collect_statistics_on_table.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/delete_stored_data.py` & `dqops-1.4.0/dqops/client/api/jobs/delete_stored_data.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/get_all_jobs.py` & `dqops-1.4.0/dqops/client/api/jobs/get_all_jobs.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/get_job.py` & `dqops-1.4.0/dqops/client/api/jobs/get_job.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/get_job_changes_since.py` & `dqops-1.4.0/dqops/client/api/jobs/get_job_changes_since.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/import_tables.py` & `dqops-1.4.0/dqops/client/api/jobs/import_tables.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/is_cron_scheduler_running.py` & `dqops-1.4.0/dqops/client/api/jobs/is_cron_scheduler_running.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/run_checks.py` & `dqops-1.4.0/dqops/client/api/jobs/run_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/start_cron_scheduler.py` & `dqops-1.4.0/dqops/client/api/jobs/start_cron_scheduler.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/stop_cron_scheduler.py` & `dqops-1.4.0/dqops/client/api/jobs/stop_cron_scheduler.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/synchronize_folders.py` & `dqops-1.4.0/dqops/client/api/jobs/synchronize_folders.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/wait_for_job.py` & `dqops-1.4.0/dqops/client/api/jobs/wait_for_job.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/jobs/wait_for_run_checks_job.py` & `dqops-1.4.0/dqops/client/api/jobs/wait_for_run_checks_job.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/labels/get_all_labels_for_columns.py` & `dqops-1.4.0/dqops/client/api/labels/get_all_labels_for_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/labels/get_all_labels_for_connections.py` & `dqops-1.4.0/dqops/client/api/labels/get_all_labels_for_connections.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/labels/get_all_labels_for_tables.py` & `dqops-1.4.0/dqops/client/api/labels/get_all_labels_for_tables.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/log_shipping/log_debug.py` & `dqops-1.4.0/dqops/client/api/log_shipping/log_debug.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/log_shipping/log_error.py` & `dqops-1.4.0/dqops/client/api/log_shipping/log_error.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/log_shipping/log_info.py` & `dqops-1.4.0/dqops/client/api/log_shipping/log_info.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/log_shipping/log_warn.py` & `dqops-1.4.0/dqops/client/api/log_shipping/log_warn.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/rules/create_rule.py` & `dqops-1.4.0/dqops/client/api/rules/create_rule.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/rules/delete_rule.py` & `dqops-1.4.0/dqops/client/api/rules/delete_rule.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/rules/get_all_rules.py` & `dqops-1.4.0/dqops/client/api/rules/get_all_rules.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/rules/get_rule.py` & `dqops-1.4.0/dqops/client/api/rules/get_rule.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/rules/get_rule_folder_tree.py` & `dqops-1.4.0/dqops/client/api/rules/get_rule_folder_tree.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/rules/update_rule.py` & `dqops-1.4.0/dqops/client/api/rules/update_rule.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/schemas/get_schema_monitoring_checks_model.py` & `dqops-1.4.0/dqops/client/api/schemas/get_schema_monitoring_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/schemas/get_schema_monitoring_checks_templates.py` & `dqops-1.4.0/dqops/client/api/schemas/get_schema_monitoring_checks_templates.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/schemas/get_schema_partitioned_checks_model.py` & `dqops-1.4.0/dqops/client/api/schemas/get_schema_partitioned_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/schemas/get_schema_partitioned_checks_templates.py` & `dqops-1.4.0/dqops/client/api/schemas/get_schema_partitioned_checks_templates.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/schemas/get_schema_profiling_checks_model.py` & `dqops-1.4.0/dqops/client/api/schemas/get_schema_profiling_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/schemas/get_schema_profiling_checks_templates.py` & `dqops-1.4.0/dqops/client/api/schemas/get_schema_profiling_checks_templates.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/schemas/get_schemas.py` & `dqops-1.4.0/dqops/client/api/schemas/get_schemas.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/search/find_tables.py` & `dqops-1.4.0/dqops/client/api/search/find_tables.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/sensor_readouts/get_column_monitoring_sensor_readouts.py` & `dqops-1.4.0/dqops/client/api/sensor_readouts/get_column_monitoring_sensor_readouts.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/sensor_readouts/get_column_partitioned_sensor_readouts.py` & `dqops-1.4.0/dqops/client/api/sensor_readouts/get_column_partitioned_sensor_readouts.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/sensor_readouts/get_column_profiling_sensor_readouts.py` & `dqops-1.4.0/dqops/client/api/sensor_readouts/get_column_profiling_sensor_readouts.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/sensor_readouts/get_table_monitoring_sensor_readouts.py` & `dqops-1.4.0/dqops/client/api/sensor_readouts/get_table_monitoring_sensor_readouts.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/sensor_readouts/get_table_partitioned_sensor_readouts.py` & `dqops-1.4.0/dqops/client/api/sensor_readouts/get_table_partitioned_sensor_readouts.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/sensor_readouts/get_table_profiling_sensor_readouts.py` & `dqops-1.4.0/dqops/client/api/sensor_readouts/get_table_profiling_sensor_readouts.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/sensors/create_sensor.py` & `dqops-1.4.0/dqops/client/api/sensors/create_sensor.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/sensors/delete_sensor.py` & `dqops-1.4.0/dqops/client/api/sensors/delete_sensor.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/sensors/get_all_sensors.py` & `dqops-1.4.0/dqops/client/api/sensors/get_all_sensors.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/sensors/get_sensor.py` & `dqops-1.4.0/dqops/client/api/sensors/get_sensor.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/sensors/get_sensor_folder_tree.py` & `dqops-1.4.0/dqops/client/api/sensors/get_sensor_folder_tree.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/sensors/update_sensor.py` & `dqops-1.4.0/dqops/client/api/sensors/update_sensor.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/shared_credentials/create_shared_credential.py` & `dqops-1.4.0/dqops/client/api/shared_credentials/create_shared_credential.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/shared_credentials/delete_shared_credential.py` & `dqops-1.4.0/dqops/client/api/shared_credentials/delete_shared_credential.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/shared_credentials/download_shared_credential.py` & `dqops-1.4.0/dqops/client/api/shared_credentials/download_shared_credential.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/shared_credentials/get_all_shared_credentials.py` & `dqops-1.4.0/dqops/client/api/shared_credentials/get_all_shared_credentials.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/shared_credentials/get_shared_credential.py` & `dqops-1.4.0/dqops/client/api/shared_credentials/get_shared_credential.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/shared_credentials/update_shared_credential.py` & `dqops-1.4.0/dqops/client/api/shared_credentials/update_shared_credential.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparison_results/get_table_comparison_monitoring_results.py` & `dqops-1.4.0/dqops/client/api/table_comparison_results/get_table_comparison_monitoring_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparison_results/get_table_comparison_partitioned_results.py` & `dqops-1.4.0/dqops/client/api/table_comparison_results/get_table_comparison_partitioned_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparison_results/get_table_comparison_profiling_results.py` & `dqops-1.4.0/dqops/client/api/table_comparison_results/get_table_comparison_profiling_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/create_table_comparison_configuration.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/create_table_comparison_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_daily.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_monthly.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/create_table_comparison_monitoring_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_daily.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_monthly.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/create_table_comparison_partitioned_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/create_table_comparison_profiling.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/create_table_comparison_profiling.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/delete_table_comparison_configuration.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/delete_table_comparison_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_configuration.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_configurations.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_configurations.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_daily.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_monthly.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_monitoring_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_daily.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_monthly.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_partitioned_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/get_table_comparison_profiling.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/get_table_comparison_profiling.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/update_table_comparison_configuration.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/update_table_comparison_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_daily.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_monthly.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/update_table_comparison_monitoring_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_daily.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_monthly.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/update_table_comparison_partitioned_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/table_comparisons/update_table_comparison_profiling.py` & `dqops-1.4.0/dqops/client/api/table_comparisons/update_table_comparison_profiling.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/create_table.py` & `dqops-1.4.0/dqops/client/api/tables/create_table.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/delete_table.py` & `dqops-1.4.0/dqops/client/api/tables/delete_table.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table.py` & `dqops-1.4.0/dqops/client/api/tables/get_table.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_basic.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_columns_monitoring_checks_model.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_columns_monitoring_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_columns_partitioned_checks_model.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_columns_partitioned_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_columns_profiling_checks_model.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_columns_profiling_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_comments.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_comments.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_daily_monitoring_checks.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_daily_monitoring_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_daily_partitioned_checks.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_daily_partitioned_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_default_grouping_configuration.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_default_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_incident_grouping.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_incident_grouping.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_labels.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_profiling_checks_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,82 @@
 from http import HTTPStatus
-from typing import Any, Dict, List, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
+from ...models.check_container_model import CheckContainerModel
 from ...types import Response
 
 
 def _get_kwargs(
     connection_name: str,
     schema_name: str,
     table_name: str,
 ) -> Dict[str, Any]:
     pass
 
     return {
         "method": "get",
-        "url": "api/connections/{connectionName}/schemas/{schemaName}/tables/{tableName}/labels".format(
+        "url": "api/connections/{connectionName}/schemas/{schemaName}/tables/{tableName}/profiling/model".format(
             connectionName=connection_name,
             schemaName=schema_name,
             tableName=table_name,
         ),
     }
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[List[str]]:
+) -> Optional[CheckContainerModel]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = cast(List[str], response.json())
+        response_200 = CheckContainerModel.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[List[str]]:
+) -> Response[CheckContainerModel]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     connection_name: str,
     schema_name: str,
     table_name: str,
     *,
     client: AuthenticatedClient,
-) -> Response[List[str]]:
-    """getTableLabels
+) -> Response[CheckContainerModel]:
+    """getTableProfilingChecksModel
 
-     Return the list of labels assigned to a table
+     Return a UI friendly model of configurations for all table level data quality profiling checks on a
+    table
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List[str]]
+        Response[CheckContainerModel]
     """
 
     kwargs = _get_kwargs(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
     )
@@ -88,30 +90,31 @@
 
 def sync(
     connection_name: str,
     schema_name: str,
     table_name: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[List[str]]:
-    """getTableLabels
+) -> Optional[CheckContainerModel]:
+    """getTableProfilingChecksModel
 
-     Return the list of labels assigned to a table
+     Return a UI friendly model of configurations for all table level data quality profiling checks on a
+    table
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List[str]
+        CheckContainerModel
     """
 
     return sync_detailed(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
         client=client,
@@ -120,30 +123,31 @@
 
 async def asyncio_detailed(
     connection_name: str,
     schema_name: str,
     table_name: str,
     *,
     client: AuthenticatedClient,
-) -> Response[List[str]]:
-    """getTableLabels
+) -> Response[CheckContainerModel]:
+    """getTableProfilingChecksModel
 
-     Return the list of labels assigned to a table
+     Return a UI friendly model of configurations for all table level data quality profiling checks on a
+    table
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List[str]]
+        Response[CheckContainerModel]
     """
 
     kwargs = _get_kwargs(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
     )
@@ -155,30 +159,31 @@
 
 async def asyncio(
     connection_name: str,
     schema_name: str,
     table_name: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[List[str]]:
-    """getTableLabels
+) -> Optional[CheckContainerModel]:
+    """getTableProfilingChecksModel
 
-     Return the list of labels assigned to a table
+     Return a UI friendly model of configurations for all table level data quality profiling checks on a
+    table
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List[str]
+        CheckContainerModel
     """
 
     return (
         await asyncio_detailed(
             connection_name=connection_name,
             schema_name=schema_name,
             table_name=table_name,
```

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_monitoring_checks_basic_model.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_monitoring_checks_basic_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_monitoring_checks_model.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_monitoring_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_monitoring_checks_model_filter.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_monitoring_checks_model_filter.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_monitoring_checks_monthly.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_monitoring_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_monitoring_checks_templates.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_monitoring_checks_templates.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_partitioned_checks_basic_model.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_partitioned_checks_basic_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_partitioned_checks_model.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_partitioned_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_partitioned_checks_model_filter.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_partitioned_checks_model_filter.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_partitioned_checks_monthly.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_partitioned_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_partitioned_checks_templates.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_partitioned_checks_templates.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_partitioning.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_partitioning.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_profiling_checks.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_profiling_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_profiling_checks_basic_model.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_profiling_checks_basic_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_profiling_checks_model.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_profiling_checks_model_filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 from ...types import Response
 
 
 def _get_kwargs(
     connection_name: str,
     schema_name: str,
     table_name: str,
+    check_category: str,
+    check_name: str,
 ) -> Dict[str, Any]:
     pass
 
     return {
         "method": "get",
-        "url": "api/connections/{connectionName}/schemas/{schemaName}/tables/{tableName}/profiling/model".format(
+        "url": "api/connections/{connectionName}/schemas/{schemaName}/tables/{tableName}/profiling/model/filter/{checkCategory}/{checkName}".format(
             connectionName=connection_name,
             schemaName=schema_name,
             tableName=table_name,
+            checkCategory=check_category,
+            checkName=check_name,
         ),
     }
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
 ) -> Optional[CheckContainerModel]:
@@ -50,143 +54,167 @@
     )
 
 
 def sync_detailed(
     connection_name: str,
     schema_name: str,
     table_name: str,
+    check_category: str,
+    check_name: str,
     *,
     client: AuthenticatedClient,
 ) -> Response[CheckContainerModel]:
-    """getTableProfilingChecksModel
+    """getTableProfilingChecksModelFilter
 
      Return a UI friendly model of configurations for all table level data quality profiling checks on a
-    table
+    table passing a filter
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
+        check_category (str):
+        check_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[CheckContainerModel]
     """
 
     kwargs = _get_kwargs(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
+        check_category=check_category,
+        check_name=check_name,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     connection_name: str,
     schema_name: str,
     table_name: str,
+    check_category: str,
+    check_name: str,
     *,
     client: AuthenticatedClient,
 ) -> Optional[CheckContainerModel]:
-    """getTableProfilingChecksModel
+    """getTableProfilingChecksModelFilter
 
      Return a UI friendly model of configurations for all table level data quality profiling checks on a
-    table
+    table passing a filter
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
+        check_category (str):
+        check_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         CheckContainerModel
     """
 
     return sync_detailed(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
+        check_category=check_category,
+        check_name=check_name,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     connection_name: str,
     schema_name: str,
     table_name: str,
+    check_category: str,
+    check_name: str,
     *,
     client: AuthenticatedClient,
 ) -> Response[CheckContainerModel]:
-    """getTableProfilingChecksModel
+    """getTableProfilingChecksModelFilter
 
      Return a UI friendly model of configurations for all table level data quality profiling checks on a
-    table
+    table passing a filter
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
+        check_category (str):
+        check_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[CheckContainerModel]
     """
 
     kwargs = _get_kwargs(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
+        check_category=check_category,
+        check_name=check_name,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     connection_name: str,
     schema_name: str,
     table_name: str,
+    check_category: str,
+    check_name: str,
     *,
     client: AuthenticatedClient,
 ) -> Optional[CheckContainerModel]:
-    """getTableProfilingChecksModel
+    """getTableProfilingChecksModelFilter
 
      Return a UI friendly model of configurations for all table level data quality profiling checks on a
-    table
+    table passing a filter
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
+        check_category (str):
+        check_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         CheckContainerModel
     """
 
     return (
         await asyncio_detailed(
             connection_name=connection_name,
             schema_name=schema_name,
             table_name=table_name,
+            check_category=check_category,
+            check_name=check_name,
             client=client,
         )
     ).parsed
```

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_profiling_checks_model_filter.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_profiling_checks_templates.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,101 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.check_container_model import CheckContainerModel
-from ...types import Response
+from ...models.check_template import CheckTemplate
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     connection_name: str,
     schema_name: str,
     table_name: str,
-    check_category: str,
-    check_name: str,
+    *,
+    check_category: Union[Unset, None, str] = UNSET,
+    check_name: Union[Unset, None, str] = UNSET,
 ) -> Dict[str, Any]:
     pass
 
+    params: Dict[str, Any] = {}
+    params["checkCategory"] = check_category
+
+    params["checkName"] = check_name
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
     return {
         "method": "get",
-        "url": "api/connections/{connectionName}/schemas/{schemaName}/tables/{tableName}/profiling/model/filter/{checkCategory}/{checkName}".format(
+        "url": "api/connections/{connectionName}/schemas/{schemaName}/tables/{tableName}/bulkenable/profiling".format(
             connectionName=connection_name,
             schemaName=schema_name,
             tableName=table_name,
-            checkCategory=check_category,
-            checkName=check_name,
         ),
+        "params": params,
     }
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[CheckContainerModel]:
+) -> Optional[List["CheckTemplate"]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = CheckContainerModel.from_dict(response.json())
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = CheckTemplate.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[CheckContainerModel]:
+) -> Response[List["CheckTemplate"]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     connection_name: str,
     schema_name: str,
     table_name: str,
-    check_category: str,
-    check_name: str,
     *,
     client: AuthenticatedClient,
-) -> Response[CheckContainerModel]:
-    """getTableProfilingChecksModelFilter
+    check_category: Union[Unset, None, str] = UNSET,
+    check_name: Union[Unset, None, str] = UNSET,
+) -> Response[List["CheckTemplate"]]:
+    """getTableProfilingChecksTemplates
 
-     Return a UI friendly model of configurations for all table level data quality profiling checks on a
-    table passing a filter
+     Return available data quality checks on a requested table.
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
-        check_category (str):
-        check_name (str):
+        check_category (Union[Unset, None, str]):
+        check_name (Union[Unset, None, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CheckContainerModel]
+        Response[List['CheckTemplate']]
     """
 
     kwargs = _get_kwargs(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
         check_category=check_category,
@@ -98,76 +109,74 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     connection_name: str,
     schema_name: str,
     table_name: str,
-    check_category: str,
-    check_name: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[CheckContainerModel]:
-    """getTableProfilingChecksModelFilter
+    check_category: Union[Unset, None, str] = UNSET,
+    check_name: Union[Unset, None, str] = UNSET,
+) -> Optional[List["CheckTemplate"]]:
+    """getTableProfilingChecksTemplates
 
-     Return a UI friendly model of configurations for all table level data quality profiling checks on a
-    table passing a filter
+     Return available data quality checks on a requested table.
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
-        check_category (str):
-        check_name (str):
+        check_category (Union[Unset, None, str]):
+        check_name (Union[Unset, None, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        CheckContainerModel
+        List['CheckTemplate']
     """
 
     return sync_detailed(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
+        client=client,
         check_category=check_category,
         check_name=check_name,
-        client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     connection_name: str,
     schema_name: str,
     table_name: str,
-    check_category: str,
-    check_name: str,
     *,
     client: AuthenticatedClient,
-) -> Response[CheckContainerModel]:
-    """getTableProfilingChecksModelFilter
+    check_category: Union[Unset, None, str] = UNSET,
+    check_name: Union[Unset, None, str] = UNSET,
+) -> Response[List["CheckTemplate"]]:
+    """getTableProfilingChecksTemplates
 
-     Return a UI friendly model of configurations for all table level data quality profiling checks on a
-    table passing a filter
+     Return available data quality checks on a requested table.
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
-        check_category (str):
-        check_name (str):
+        check_category (Union[Unset, None, str]):
+        check_name (Union[Unset, None, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CheckContainerModel]
+        Response[List['CheckTemplate']]
     """
 
     kwargs = _get_kwargs(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
         check_category=check_category,
@@ -179,42 +188,41 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     connection_name: str,
     schema_name: str,
     table_name: str,
-    check_category: str,
-    check_name: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[CheckContainerModel]:
-    """getTableProfilingChecksModelFilter
+    check_category: Union[Unset, None, str] = UNSET,
+    check_name: Union[Unset, None, str] = UNSET,
+) -> Optional[List["CheckTemplate"]]:
+    """getTableProfilingChecksTemplates
 
-     Return a UI friendly model of configurations for all table level data quality profiling checks on a
-    table passing a filter
+     Return available data quality checks on a requested table.
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
-        check_category (str):
-        check_name (str):
+        check_category (Union[Unset, None, str]):
+        check_name (Union[Unset, None, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        CheckContainerModel
+        List['CheckTemplate']
     """
 
     return (
         await asyncio_detailed(
             connection_name=connection_name,
             schema_name=schema_name,
             table_name=table_name,
+            client=client,
             check_category=check_category,
             check_name=check_name,
-            client=client,
         )
     ).parsed
```

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_profiling_checks_templates.py` & `dqops-1.4.0/dqops/client/api/columns/get_columns.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,114 @@
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.check_template import CheckTemplate
+from ...models.check_type import CheckType
+from ...models.column_list_model import ColumnListModel
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     connection_name: str,
     schema_name: str,
     table_name: str,
     *,
-    check_category: Union[Unset, None, str] = UNSET,
-    check_name: Union[Unset, None, str] = UNSET,
+    data_quality_status: Union[Unset, None, bool] = UNSET,
+    check_type: Union[Unset, None, CheckType] = UNSET,
 ) -> Dict[str, Any]:
     pass
 
     params: Dict[str, Any] = {}
-    params["checkCategory"] = check_category
+    params["dataQualityStatus"] = data_quality_status
 
-    params["checkName"] = check_name
+    json_check_type: Union[Unset, None, str] = UNSET
+    if not isinstance(check_type, Unset):
+        json_check_type = check_type.value if check_type else None
+
+    params["checkType"] = json_check_type
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
-        "url": "api/connections/{connectionName}/schemas/{schemaName}/tables/{tableName}/bulkenable/profiling".format(
+        "url": "api/connections/{connectionName}/schemas/{schemaName}/tables/{tableName}/columns".format(
             connectionName=connection_name,
             schemaName=schema_name,
             tableName=table_name,
         ),
         "params": params,
     }
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[List["CheckTemplate"]]:
+) -> Optional[List["ColumnListModel"]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = []
         _response_200 = response.json()
         for response_200_item_data in _response_200:
-            response_200_item = CheckTemplate.from_dict(response_200_item_data)
+            response_200_item = ColumnListModel.from_dict(response_200_item_data)
 
             response_200.append(response_200_item)
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[List["CheckTemplate"]]:
+) -> Response[List["ColumnListModel"]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     connection_name: str,
     schema_name: str,
     table_name: str,
     *,
     client: AuthenticatedClient,
-    check_category: Union[Unset, None, str] = UNSET,
-    check_name: Union[Unset, None, str] = UNSET,
-) -> Response[List["CheckTemplate"]]:
-    """getTableProfilingChecksTemplates
+    data_quality_status: Union[Unset, None, bool] = UNSET,
+    check_type: Union[Unset, None, CheckType] = UNSET,
+) -> Response[List["ColumnListModel"]]:
+    """getColumns
 
-     Return available data quality checks on a requested table.
+     Returns a list of columns inside a table
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
-        check_category (Union[Unset, None, str]):
-        check_name (Union[Unset, None, str]):
+        data_quality_status (Union[Unset, None, bool]):
+        check_type (Union[Unset, None, CheckType]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['CheckTemplate']]
+        Response[List['ColumnListModel']]
     """
 
     kwargs = _get_kwargs(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
-        check_category=check_category,
-        check_name=check_name,
+        data_quality_status=data_quality_status,
+        check_type=check_type,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
@@ -111,118 +116,118 @@
 
 def sync(
     connection_name: str,
     schema_name: str,
     table_name: str,
     *,
     client: AuthenticatedClient,
-    check_category: Union[Unset, None, str] = UNSET,
-    check_name: Union[Unset, None, str] = UNSET,
-) -> Optional[List["CheckTemplate"]]:
-    """getTableProfilingChecksTemplates
+    data_quality_status: Union[Unset, None, bool] = UNSET,
+    check_type: Union[Unset, None, CheckType] = UNSET,
+) -> Optional[List["ColumnListModel"]]:
+    """getColumns
 
-     Return available data quality checks on a requested table.
+     Returns a list of columns inside a table
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
-        check_category (Union[Unset, None, str]):
-        check_name (Union[Unset, None, str]):
+        data_quality_status (Union[Unset, None, bool]):
+        check_type (Union[Unset, None, CheckType]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['CheckTemplate']
+        List['ColumnListModel']
     """
 
     return sync_detailed(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
         client=client,
-        check_category=check_category,
-        check_name=check_name,
+        data_quality_status=data_quality_status,
+        check_type=check_type,
     ).parsed
 
 
 async def asyncio_detailed(
     connection_name: str,
     schema_name: str,
     table_name: str,
     *,
     client: AuthenticatedClient,
-    check_category: Union[Unset, None, str] = UNSET,
-    check_name: Union[Unset, None, str] = UNSET,
-) -> Response[List["CheckTemplate"]]:
-    """getTableProfilingChecksTemplates
+    data_quality_status: Union[Unset, None, bool] = UNSET,
+    check_type: Union[Unset, None, CheckType] = UNSET,
+) -> Response[List["ColumnListModel"]]:
+    """getColumns
 
-     Return available data quality checks on a requested table.
+     Returns a list of columns inside a table
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
-        check_category (Union[Unset, None, str]):
-        check_name (Union[Unset, None, str]):
+        data_quality_status (Union[Unset, None, bool]):
+        check_type (Union[Unset, None, CheckType]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['CheckTemplate']]
+        Response[List['ColumnListModel']]
     """
 
     kwargs = _get_kwargs(
         connection_name=connection_name,
         schema_name=schema_name,
         table_name=table_name,
-        check_category=check_category,
-        check_name=check_name,
+        data_quality_status=data_quality_status,
+        check_type=check_type,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     connection_name: str,
     schema_name: str,
     table_name: str,
     *,
     client: AuthenticatedClient,
-    check_category: Union[Unset, None, str] = UNSET,
-    check_name: Union[Unset, None, str] = UNSET,
-) -> Optional[List["CheckTemplate"]]:
-    """getTableProfilingChecksTemplates
+    data_quality_status: Union[Unset, None, bool] = UNSET,
+    check_type: Union[Unset, None, CheckType] = UNSET,
+) -> Optional[List["ColumnListModel"]]:
+    """getColumns
 
-     Return available data quality checks on a requested table.
+     Returns a list of columns inside a table
 
     Args:
         connection_name (str):
         schema_name (str):
         table_name (str):
-        check_category (Union[Unset, None, str]):
-        check_name (Union[Unset, None, str]):
+        data_quality_status (Union[Unset, None, bool]):
+        check_type (Union[Unset, None, CheckType]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['CheckTemplate']
+        List['ColumnListModel']
     """
 
     return (
         await asyncio_detailed(
             connection_name=connection_name,
             schema_name=schema_name,
             table_name=table_name,
             client=client,
-            check_category=check_category,
-            check_name=check_name,
+            data_quality_status=data_quality_status,
+            check_type=check_type,
         )
     ).parsed
```

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_scheduling_group_override.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_scheduling_group_override.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_table_statistics.py` & `dqops-1.4.0/dqops/client/api/tables/get_table_statistics.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/get_tables.py` & `dqops-1.4.0/dqops/client/api/tables/get_tables.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table.py` & `dqops-1.4.0/dqops/client/api/tables/update_table.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_basic.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_basic.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_comments.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_comments.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_daily_monitoring_checks.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_daily_monitoring_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_default_grouping_configuration.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_default_grouping_configuration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_incident_grouping.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_incident_grouping.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_labels.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_labels.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_monitoring_checks_model.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_monitoring_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_monitoring_checks_monthly.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_monitoring_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_partitioned_checks_daily.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_partitioned_checks_daily.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_partitioned_checks_model.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_partitioned_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_partitioned_checks_monthly.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_partitioned_checks_monthly.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_partitioning.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_partitioning.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_profiling_checks.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_profiling_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_profiling_checks_model.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_profiling_checks_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/tables/update_table_scheduling_group_override.py` & `dqops-1.4.0/dqops/client/api/tables/update_table_scheduling_group_override.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/timezones/get_available_zone_ids.py` & `dqops-1.4.0/dqops/client/api/timezones/get_available_zone_ids.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/users/change_caller_password.py` & `dqops-1.4.0/dqops/client/api/users/change_caller_password.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/users/change_user_password.py` & `dqops-1.4.0/dqops/client/api/users/change_user_password.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/users/create_user.py` & `dqops-1.4.0/dqops/client/api/users/create_user.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/users/delete_user.py` & `dqops-1.4.0/dqops/client/api/users/delete_user.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/users/get_all_users.py` & `dqops-1.4.0/dqops/client/api/users/get_all_users.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/users/get_user.py` & `dqops-1.4.0/dqops/client/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/api/users/update_user.py` & `dqops-1.4.0/dqops/client/api/users/update_user.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/client.py` & `dqops-1.4.0/dqops/client/client.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/__init__.py` & `dqops-1.4.0/dqops/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/all_checks_patch_parameters.py` & `dqops-1.4.0/dqops/client/models/all_checks_patch_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/all_checks_patch_parameters_selected_tables_to_columns.py` & `dqops-1.4.0/dqops/client/models/all_checks_patch_parameters_selected_tables_to_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_error_05_pct_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_error_05_pct_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_warning_1_pct_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_warning_1_pct_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_error_05_pct_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_error_05_pct_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_fatal_01_pct_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_warning_1_pct_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_warning_1_pct_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/authenticated_dashboard_model.py` & `dqops-1.4.0/dqops/client/models/authenticated_dashboard_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/between_floats_rule_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/between_floats_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/between_ints_rule_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/between_ints_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/between_percent_rule_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/between_percent_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/big_query_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/big_query_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/bulk_check_deactivate_parameters.py` & `dqops-1.4.0/dqops/client/models/bulk_check_deactivate_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/bulk_check_deactivate_parameters_selected_tables_to_columns.py` & `dqops-1.4.0/dqops/client/models/bulk_check_deactivate_parameters_selected_tables_to_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/change_percent_1_day_rule_10_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/change_percent_1_day_rule_10_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/change_percent_1_day_rule_20_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/change_percent_1_day_rule_20_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/change_percent_1_day_rule_50_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/change_percent_1_day_rule_50_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/change_percent_30_days_rule_10_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/change_percent_30_days_rule_10_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/change_percent_30_days_rule_20_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/change_percent_30_days_rule_20_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/change_percent_30_days_rule_50_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/change_percent_30_days_rule_50_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/change_percent_7_days_rule_10_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/change_percent_7_days_rule_10_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/change_percent_7_days_rule_20_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/change_percent_7_days_rule_20_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/change_percent_7_days_rule_50_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/change_percent_7_days_rule_50_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/change_percent_rule_10_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/change_percent_rule_10_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/change_percent_rule_20_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/change_percent_rule_20_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/change_percent_rule_50_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/change_percent_rule_50_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_configuration_model.py` & `dqops-1.4.0/dqops/client/models/check_configuration_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_container_list_model.py` & `dqops-1.4.0/dqops/client/models/check_container_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_container_model.py` & `dqops-1.4.0/dqops/client/models/check_container_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_container_type_model.py` & `dqops-1.4.0/dqops/client/models/check_container_type_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_current_data_quality_status_model.py` & `dqops-1.4.0/dqops/client/models/check_current_data_quality_status_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_definition_folder_model.py` & `dqops-1.4.0/dqops/client/models/check_definition_folder_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_definition_folder_model_folders.py` & `dqops-1.4.0/dqops/client/models/check_definition_folder_model_folders.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_definition_list_model.py` & `dqops-1.4.0/dqops/client/models/check_definition_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_definition_model.py` & `dqops-1.4.0/dqops/client/models/check_definition_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_list_model.py` & `dqops-1.4.0/dqops/client/models/check_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_model.py` & `dqops-1.4.0/dqops/client/models/check_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_result_entry_model.py` & `dqops-1.4.0/dqops/client/models/check_result_entry_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_result_sort_order.py` & `dqops-1.4.0/dqops/client/models/check_result_sort_order.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_results_list_model.py` & `dqops-1.4.0/dqops/client/models/check_results_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_results_overview_data_model.py` & `dqops-1.4.0/dqops/client/models/check_results_overview_data_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_search_filters.py` & `dqops-1.4.0/dqops/client/models/check_search_filters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/check_template.py` & `dqops-1.4.0/dqops/client/models/check_template.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/cloud_synchronization_folders_status_model.py` & `dqops-1.4.0/dqops/client/models/cloud_synchronization_folders_status_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/collect_statistics_on_table_queue_job_parameters.py` & `dqops-1.4.0/dqops/client/models/collect_statistics_on_table_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/collect_statistics_queue_job_parameters.py` & `dqops-1.4.0/dqops/client/models/collect_statistics_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/collect_statistics_queue_job_result.py` & `dqops-1.4.0/dqops/client/models/collect_statistics_queue_job_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/collect_statistics_result.py` & `dqops-1.4.0/dqops/client/models/collect_statistics_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_accepted_values_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_accepted_values_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_accepted_values_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_accepted_values_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accepted_values_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_accepted_values_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accepted_values_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_accepted_values_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accepted_values_text_found_in_set_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_accepted_values_text_found_in_set_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_total_average_match_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_total_average_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_total_average_match_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_total_average_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_total_max_match_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_total_max_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_total_max_match_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_total_max_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_total_min_match_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_total_min_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_total_min_match_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_total_min_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_total_not_null_count_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_total_sum_match_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_total_sum_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_accuracy_total_sum_match_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_accuracy_total_sum_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_anomaly_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_anomaly_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_anomaly_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_anomaly_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_anomaly_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_anomaly_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_bool_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_bool_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_bool_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_bool_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_bool_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_bool_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_bool_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_bool_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_bool_false_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_bool_false_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_bool_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_bool_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_bool_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_bool_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_bool_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_bool_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_bool_true_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_bool_true_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_column_exists_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_column_exists_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_column_type_hash_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_column_type_hash_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_comparison_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_comparison_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_max_match_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_comparison_max_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_mean_match_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_comparison_mean_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_min_match_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_comparison_min_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_model.py` & `dqops-1.4.0/dqops/client/models/column_comparison_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_comparison_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_comparison_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_not_null_count_match_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_comparison_not_null_count_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_null_count_match_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_comparison_null_count_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_comparison_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_comparison_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_comparison_sum_match_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_comparison_sum_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_conversions_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_conversions_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_conversions_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_conversions_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_conversions_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_conversions_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_conversions_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_conversions_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_current_data_quality_status_model.py` & `dqops-1.4.0/dqops/client/models/column_current_data_quality_status_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,14 +39,17 @@
                 severity data quality issue.
             fatals (Union[Unset, int]): The number of most recent data quality checks that failed by raising a fatal
                 severity data quality issue.
             execution_errors (Union[Unset, int]): The number of data quality check execution errors that were reported due
                 to access issues to the data source, invalid mapping in DQOps, invalid queries in data quality sensors or
                 invalid python rules. When an execution error is reported, the configuration of a data quality check on a column
                 must be updated.
+            data_quality_kpi (Union[Unset, float]): Data quality KPI score for the column, measured as a percentage of
+                passed data quality checks. DQOps counts data quality issues at a warning severity level as passed checks. The
+                data quality KPI score is a value in the range 0..100.
             checks (Union[Unset, ColumnCurrentDataQualityStatusModelChecks]): The dictionary of statuses for data quality
                 checks. The keys are data quality check names, the values are the current data quality check statuses that
                 describe the most current status.
             dimensions (Union[Unset, ColumnCurrentDataQualityStatusModelDimensions]): Dictionary of the current data quality
                 statues for each data quality dimension.
     """
 
@@ -55,14 +58,15 @@
     last_check_executed_at: Union[Unset, int] = UNSET
     executed_checks: Union[Unset, int] = UNSET
     valid_results: Union[Unset, int] = UNSET
     warnings: Union[Unset, int] = UNSET
     errors: Union[Unset, int] = UNSET
     fatals: Union[Unset, int] = UNSET
     execution_errors: Union[Unset, int] = UNSET
+    data_quality_kpi: Union[Unset, float] = UNSET
     checks: Union[Unset, "ColumnCurrentDataQualityStatusModelChecks"] = UNSET
     dimensions: Union[Unset, "ColumnCurrentDataQualityStatusModelDimensions"] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         current_severity: Union[Unset, str] = UNSET
         if not isinstance(self.current_severity, Unset):
@@ -75,14 +79,15 @@
         last_check_executed_at = self.last_check_executed_at
         executed_checks = self.executed_checks
         valid_results = self.valid_results
         warnings = self.warnings
         errors = self.errors
         fatals = self.fatals
         execution_errors = self.execution_errors
+        data_quality_kpi = self.data_quality_kpi
         checks: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.checks, Unset):
             checks = self.checks.to_dict()
 
         dimensions: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.dimensions, Unset):
             dimensions = self.dimensions.to_dict()
@@ -104,14 +109,16 @@
             field_dict["warnings"] = warnings
         if errors is not UNSET:
             field_dict["errors"] = errors
         if fatals is not UNSET:
             field_dict["fatals"] = fatals
         if execution_errors is not UNSET:
             field_dict["execution_errors"] = execution_errors
+        if data_quality_kpi is not UNSET:
+            field_dict["data_quality_kpi"] = data_quality_kpi
         if checks is not UNSET:
             field_dict["checks"] = checks
         if dimensions is not UNSET:
             field_dict["dimensions"] = dimensions
 
         return field_dict
 
@@ -151,14 +158,16 @@
 
         errors = d.pop("errors", UNSET)
 
         fatals = d.pop("fatals", UNSET)
 
         execution_errors = d.pop("execution_errors", UNSET)
 
+        data_quality_kpi = d.pop("data_quality_kpi", UNSET)
+
         _checks = d.pop("checks", UNSET)
         checks: Union[Unset, ColumnCurrentDataQualityStatusModelChecks]
         if isinstance(_checks, Unset):
             checks = UNSET
         else:
             checks = ColumnCurrentDataQualityStatusModelChecks.from_dict(_checks)
 
@@ -177,14 +186,15 @@
             last_check_executed_at=last_check_executed_at,
             executed_checks=executed_checks,
             valid_results=valid_results,
             warnings=warnings,
             errors=errors,
             fatals=fatals,
             execution_errors=execution_errors,
+            data_quality_kpi=data_quality_kpi,
             checks=checks,
             dimensions=dimensions,
         )
 
         column_current_data_quality_status_model.additional_properties = d
         return column_current_data_quality_status_model
```

### Comparing `dqops-1.3.0/dqops/client/models/column_current_data_quality_status_model_checks.py` & `dqops-1.4.0/dqops/client/models/column_current_data_quality_status_model_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_current_data_quality_status_model_dimensions.py` & `dqops-1.4.0/dqops/client/models/column_current_data_quality_status_model_dimensions.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_custom_sql_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_custom_sql_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_custom_sql_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_custom_sql_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_custom_sql_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_custom_sql_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_custom_sql_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_custom_sql_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_daily_monitoring_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/column_daily_monitoring_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_daily_monitoring_check_categories_spec_comparisons.py` & `dqops-1.4.0/dqops/client/models/column_daily_monitoring_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_daily_monitoring_check_categories_spec_custom.py` & `dqops-1.4.0/dqops/client/models/column_daily_monitoring_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_daily_partitioned_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/column_daily_partitioned_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_daily_partitioned_check_categories_spec_comparisons.py` & `dqops-1.4.0/dqops/client/models/column_daily_partitioned_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_daily_partitioned_check_categories_spec_custom.py` & `dqops-1.4.0/dqops/client/models/column_daily_partitioned_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_datatype_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_datatype_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datatype_detected_datatype_in_text_changed_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_datatype_detected_datatype_in_text_changed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_datatype_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_datatype_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datatype_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_datatype_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datatype_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_datatype_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datatype_string_datatype_detect_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_datatype_string_datatype_detect_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_date_in_range_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_date_in_range_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_date_in_range_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_date_in_range_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_date_values_in_future_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_date_values_in_future_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_datetime_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_datetime_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datetime_date_values_in_future_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_datetime_date_values_in_future_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_datetime_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_datetime_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datetime_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_datetime_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_datetime_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_datetime_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_default_checks_pattern_spec.py` & `dqops-1.4.0/dqops/client/models/column_default_checks_pattern_spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,29 +23,35 @@
 
 @_attrs_define
 class ColumnDefaultChecksPatternSpec:
     """
     Attributes:
         priority (Union[Unset, int]): The priority of the pattern. Patterns with lower values are applied before
             patterns with higher priority values.
+        disabled (Union[Unset, bool]): Disables this data quality check configuration. The checks will not be activated.
+        description (Union[Unset, str]): The description (documentation) of this data quality check configuration.
         target (Union[Unset, TargetColumnPatternSpec]):
         profiling_checks (Union[Unset, ColumnProfilingCheckCategoriesSpec]):
         monitoring_checks (Union[Unset, ColumnMonitoringCheckCategoriesSpec]):
         partitioned_checks (Union[Unset, ColumnPartitionedCheckCategoriesSpec]):
     """
 
     priority: Union[Unset, int] = UNSET
+    disabled: Union[Unset, bool] = UNSET
+    description: Union[Unset, str] = UNSET
     target: Union[Unset, "TargetColumnPatternSpec"] = UNSET
     profiling_checks: Union[Unset, "ColumnProfilingCheckCategoriesSpec"] = UNSET
     monitoring_checks: Union[Unset, "ColumnMonitoringCheckCategoriesSpec"] = UNSET
     partitioned_checks: Union[Unset, "ColumnPartitionedCheckCategoriesSpec"] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         priority = self.priority
+        disabled = self.disabled
+        description = self.description
         target: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.target, Unset):
             target = self.target.to_dict()
 
         profiling_checks: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.profiling_checks, Unset):
             profiling_checks = self.profiling_checks.to_dict()
@@ -59,14 +65,18 @@
             partitioned_checks = self.partitioned_checks.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if priority is not UNSET:
             field_dict["priority"] = priority
+        if disabled is not UNSET:
+            field_dict["disabled"] = disabled
+        if description is not UNSET:
+            field_dict["description"] = description
         if target is not UNSET:
             field_dict["target"] = target
         if profiling_checks is not UNSET:
             field_dict["profiling_checks"] = profiling_checks
         if monitoring_checks is not UNSET:
             field_dict["monitoring_checks"] = monitoring_checks
         if partitioned_checks is not UNSET:
@@ -86,14 +96,18 @@
             ColumnProfilingCheckCategoriesSpec,
         )
         from ..models.target_column_pattern_spec import TargetColumnPatternSpec
 
         d = src_dict.copy()
         priority = d.pop("priority", UNSET)
 
+        disabled = d.pop("disabled", UNSET)
+
+        description = d.pop("description", UNSET)
+
         _target = d.pop("target", UNSET)
         target: Union[Unset, TargetColumnPatternSpec]
         if isinstance(_target, Unset):
             target = UNSET
         else:
             target = TargetColumnPatternSpec.from_dict(_target)
 
@@ -122,14 +136,16 @@
         else:
             partitioned_checks = ColumnPartitionedCheckCategoriesSpec.from_dict(
                 _partitioned_checks
             )
 
         column_default_checks_pattern_spec = cls(
             priority=priority,
+            disabled=disabled,
+            description=description,
             target=target,
             profiling_checks=profiling_checks,
             monitoring_checks=monitoring_checks,
             partitioned_checks=partitioned_checks,
         )
 
         column_default_checks_pattern_spec.additional_properties = d
```

### Comparing `dqops-1.3.0/dqops/client/models/column_detected_datatype_in_text_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_detected_datatype_in_text_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_distinct_count_anomaly_differencing_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_distinct_count_anomaly_differencing_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_distinct_count_anomaly_stationary_partition_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_distinct_count_anomaly_stationary_partition_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_distinct_count_change_1_day_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_distinct_count_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_distinct_count_change_30_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_distinct_count_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_distinct_count_change_7_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_distinct_count_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_distinct_count_change_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_distinct_count_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_distinct_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_distinct_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_distinct_percent_anomaly_stationary_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_distinct_percent_anomaly_stationary_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_distinct_percent_change_1_day_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_distinct_percent_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_distinct_percent_change_30_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_distinct_percent_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_distinct_percent_change_7_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_distinct_percent_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_distinct_percent_change_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_distinct_percent_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_distinct_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_distinct_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_duplicate_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_duplicate_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_duplicate_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_duplicate_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_expected_numbers_in_use_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_expected_numbers_in_use_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_expected_text_values_in_use_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_expected_text_values_in_use_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_expected_texts_in_top_values_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_expected_texts_in_top_values_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_false_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_false_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integer_in_range_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_integer_in_range_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_integrity_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_integrity_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_foreign_key_match_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_integrity_foreign_key_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_foreign_key_match_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_integrity_foreign_key_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_foreign_key_not_match_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_integrity_foreign_key_not_match_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_lookup_key_not_found_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_integrity_lookup_key_not_found_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_integrity_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_integrity_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_integrity_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_integrity_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_integrity_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_invalid_email_format_found_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_invalid_email_format_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_invalid_email_format_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_invalid_email_format_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_invalid_ip_4_address_format_found_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_invalid_ip_4_address_format_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_invalid_ip_6_address_format_found_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_invalid_ip_6_address_format_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_invalid_latitude_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_invalid_latitude_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_invalid_longitude_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_invalid_longitude_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_invalid_uuid_format_found_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_invalid_uuid_format_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_list_model.py` & `dqops-1.4.0/dqops/client/models/column_list_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.check_search_filters import CheckSearchFilters
+    from ..models.column_current_data_quality_status_model import (
+        ColumnCurrentDataQualityStatusModel,
+    )
     from ..models.column_type_snapshot_spec import ColumnTypeSnapshotSpec
     from ..models.delete_stored_data_queue_job_parameters import (
         DeleteStoredDataQueueJobParameters,
     )
     from ..models.physical_table_name import PhysicalTableName
     from ..models.statistics_collector_search_filters import (
         StatisticsCollectorSearchFilters,
@@ -38,14 +41,17 @@
             has_any_configured_profiling_checks (Union[Unset, bool]): True when the column has any profiling checks
                 configured.
             has_any_configured_monitoring_checks (Union[Unset, bool]): True when the column has any monitoring checks
                 configured.
             has_any_configured_partition_checks (Union[Unset, bool]): True when the column has any partition checks
                 configured.
             type_snapshot (Union[Unset, ColumnTypeSnapshotSpec]):
+            data_quality_status (Union[Unset, ColumnCurrentDataQualityStatusModel]): The column's most recent data quality
+                status. It is a summary of the results of the most recently executed data quality checks on the column. Verify
+                the value of the current_severity to see if there are any data quality issues on the column.
             run_checks_job_template (Union[Unset, CheckSearchFilters]): Target data quality checks filter, identifies which
                 checks on which tables and columns should be executed.
             run_profiling_checks_job_template (Union[Unset, CheckSearchFilters]): Target data quality checks filter,
                 identifies which checks on which tables and columns should be executed.
             run_monitoring_checks_job_template (Union[Unset, CheckSearchFilters]): Target data quality checks filter,
                 identifies which checks on which tables and columns should be executed.
             run_partition_checks_job_template (Union[Unset, CheckSearchFilters]): Target data quality checks filter,
@@ -67,14 +73,15 @@
     column_hash: Union[Unset, int] = UNSET
     disabled: Union[Unset, bool] = UNSET
     has_any_configured_checks: Union[Unset, bool] = UNSET
     has_any_configured_profiling_checks: Union[Unset, bool] = UNSET
     has_any_configured_monitoring_checks: Union[Unset, bool] = UNSET
     has_any_configured_partition_checks: Union[Unset, bool] = UNSET
     type_snapshot: Union[Unset, "ColumnTypeSnapshotSpec"] = UNSET
+    data_quality_status: Union[Unset, "ColumnCurrentDataQualityStatusModel"] = UNSET
     run_checks_job_template: Union[Unset, "CheckSearchFilters"] = UNSET
     run_profiling_checks_job_template: Union[Unset, "CheckSearchFilters"] = UNSET
     run_monitoring_checks_job_template: Union[Unset, "CheckSearchFilters"] = UNSET
     run_partition_checks_job_template: Union[Unset, "CheckSearchFilters"] = UNSET
     collect_statistics_job_template: Union[
         Unset, "StatisticsCollectorSearchFilters"
     ] = UNSET
@@ -103,14 +110,18 @@
         has_any_configured_profiling_checks = self.has_any_configured_profiling_checks
         has_any_configured_monitoring_checks = self.has_any_configured_monitoring_checks
         has_any_configured_partition_checks = self.has_any_configured_partition_checks
         type_snapshot: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.type_snapshot, Unset):
             type_snapshot = self.type_snapshot.to_dict()
 
+        data_quality_status: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.data_quality_status, Unset):
+            data_quality_status = self.data_quality_status.to_dict()
+
         run_checks_job_template: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.run_checks_job_template, Unset):
             run_checks_job_template = self.run_checks_job_template.to_dict()
 
         run_profiling_checks_job_template: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.run_profiling_checks_job_template, Unset):
             run_profiling_checks_job_template = (
@@ -173,14 +184,16 @@
             ] = has_any_configured_monitoring_checks
         if has_any_configured_partition_checks is not UNSET:
             field_dict[
                 "has_any_configured_partition_checks"
             ] = has_any_configured_partition_checks
         if type_snapshot is not UNSET:
             field_dict["type_snapshot"] = type_snapshot
+        if data_quality_status is not UNSET:
+            field_dict["data_quality_status"] = data_quality_status
         if run_checks_job_template is not UNSET:
             field_dict["run_checks_job_template"] = run_checks_job_template
         if run_profiling_checks_job_template is not UNSET:
             field_dict[
                 "run_profiling_checks_job_template"
             ] = run_profiling_checks_job_template
         if run_monitoring_checks_job_template is not UNSET:
@@ -207,14 +220,17 @@
             field_dict["can_delete_data"] = can_delete_data
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.check_search_filters import CheckSearchFilters
+        from ..models.column_current_data_quality_status_model import (
+            ColumnCurrentDataQualityStatusModel,
+        )
         from ..models.column_type_snapshot_spec import ColumnTypeSnapshotSpec
         from ..models.delete_stored_data_queue_job_parameters import (
             DeleteStoredDataQueueJobParameters,
         )
         from ..models.physical_table_name import PhysicalTableName
         from ..models.statistics_collector_search_filters import (
             StatisticsCollectorSearchFilters,
@@ -257,14 +273,23 @@
         _type_snapshot = d.pop("type_snapshot", UNSET)
         type_snapshot: Union[Unset, ColumnTypeSnapshotSpec]
         if isinstance(_type_snapshot, Unset):
             type_snapshot = UNSET
         else:
             type_snapshot = ColumnTypeSnapshotSpec.from_dict(_type_snapshot)
 
+        _data_quality_status = d.pop("data_quality_status", UNSET)
+        data_quality_status: Union[Unset, ColumnCurrentDataQualityStatusModel]
+        if isinstance(_data_quality_status, Unset):
+            data_quality_status = UNSET
+        else:
+            data_quality_status = ColumnCurrentDataQualityStatusModel.from_dict(
+                _data_quality_status
+            )
+
         _run_checks_job_template = d.pop("run_checks_job_template", UNSET)
         run_checks_job_template: Union[Unset, CheckSearchFilters]
         if isinstance(_run_checks_job_template, Unset):
             run_checks_job_template = UNSET
         else:
             run_checks_job_template = CheckSearchFilters.from_dict(
                 _run_checks_job_template
@@ -342,14 +367,15 @@
             column_hash=column_hash,
             disabled=disabled,
             has_any_configured_checks=has_any_configured_checks,
             has_any_configured_profiling_checks=has_any_configured_profiling_checks,
             has_any_configured_monitoring_checks=has_any_configured_monitoring_checks,
             has_any_configured_partition_checks=has_any_configured_partition_checks,
             type_snapshot=type_snapshot,
+            data_quality_status=data_quality_status,
             run_checks_job_template=run_checks_job_template,
             run_profiling_checks_job_template=run_profiling_checks_job_template,
             run_monitoring_checks_job_template=run_monitoring_checks_job_template,
             run_partition_checks_job_template=run_partition_checks_job_template,
             collect_statistics_job_template=collect_statistics_job_template,
             data_clean_job_template=data_clean_job_template,
             can_edit=can_edit,
```

### Comparing `dqops-1.3.0/dqops/client/models/column_max_anomaly_differencing_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_max_anomaly_differencing_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_max_anomaly_stationary_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_max_anomaly_stationary_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_max_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_max_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_mean_anomaly_stationary_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_mean_anomaly_stationary_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_mean_change_1_day_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_mean_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_mean_change_30_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_mean_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_mean_change_7_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_mean_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_mean_change_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_mean_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_mean_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_mean_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_median_anomaly_stationary_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_median_anomaly_stationary_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_median_change_1_day_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_median_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_median_change_30_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_median_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_median_change_7_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_median_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_median_change_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_median_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_median_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_median_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_min_anomaly_differencing_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_min_anomaly_differencing_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_min_anomaly_stationary_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_min_anomaly_stationary_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_min_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_min_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_model.py` & `dqops-1.4.0/dqops/client/models/column_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_monitoring_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/column_monitoring_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_monthly_monitoring_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/column_monthly_monitoring_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_comparisons.py` & `dqops-1.4.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_custom.py` & `dqops-1.4.0/dqops/client/models/column_monthly_monitoring_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_monthly_partitioned_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/column_monthly_partitioned_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_comparisons.py` & `dqops-1.4.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_custom.py` & `dqops-1.4.0/dqops/client/models/column_monthly_partitioned_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_negative_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_negative_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_negative_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_negative_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_non_negative_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_non_negative_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_non_negative_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_non_negative_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_not_nulls_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_not_nulls_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_not_nulls_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_not_nulls_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_null_percent_anomaly_stationary_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_null_percent_anomaly_stationary_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_null_percent_change_1_day_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_null_percent_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_null_percent_change_30_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_null_percent_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_null_percent_change_7_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_null_percent_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_null_percent_change_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_null_percent_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_nulls_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_nulls_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_nulls_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_nulls_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_not_nulls_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_not_nulls_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_not_nulls_count_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_not_nulls_count_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_not_nulls_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_not_nulls_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_not_nulls_percent_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_not_nulls_percent_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_nulls_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_nulls_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_nulls_count_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_nulls_count_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_nulls_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_nulls_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_nulls_percent_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_nulls_percent_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_nulls_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_nulls_statistics_collectors_spec.py` & `dqops-1.4.0/dqops/client/models/column_nulls_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_number_above_max_value_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_number_above_max_value_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_number_above_max_value_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_number_above_max_value_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_number_below_min_value_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_number_below_min_value_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_number_below_min_value_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_number_below_min_value_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_number_found_in_set_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_number_found_in_set_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_number_in_range_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_number_in_range_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_numeric_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_numeric_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_expected_numbers_in_use_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_expected_numbers_in_use_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_integer_in_range_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_integer_in_range_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_invalid_latitude_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_invalid_latitude_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_invalid_longitude_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_invalid_longitude_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_max_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_max_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_mean_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_mean_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_median_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_median_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_min_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_min_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_numeric_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_numeric_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_negative_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_negative_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_negative_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_negative_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_non_negative_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_non_negative_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_non_negative_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_non_negative_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_number_above_max_value_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_number_above_max_value_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_number_above_max_value_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_number_above_max_value_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_number_below_min_value_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_number_below_min_value_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_number_below_min_value_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_number_below_min_value_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_number_found_in_set_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_number_found_in_set_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_number_in_range_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_number_in_range_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_percentile_10_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_percentile_10_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_percentile_25_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_percentile_25_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_percentile_75_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_percentile_75_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_percentile_90_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_percentile_90_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_percentile_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_percentile_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_population_stddev_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_population_stddev_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_population_variance_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_population_variance_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_numeric_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_sample_stddev_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_sample_stddev_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_sample_variance_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_sample_variance_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_sum_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_sum_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_valid_latitude_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_valid_latitude_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_numeric_valid_longitude_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_numeric_valid_longitude_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_partitioned_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/column_partitioned_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_patterns_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_patterns_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_invalid_email_format_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_invalid_email_format_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_invalid_email_format_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_invalid_email_format_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_invalid_ip_4_address_format_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_invalid_ip_4_address_format_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_invalid_ip_6_address_format_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_invalid_ip_6_address_format_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_invalid_uuid_format_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_invalid_uuid_format_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_patterns_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_patterns_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_patterns_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_text_matching_date_pattern_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_text_matching_date_pattern_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_text_matching_name_pattern_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_text_matching_name_pattern_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_text_not_matching_date_pattern_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_text_not_matching_date_pattern_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_text_not_matching_regex_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_text_not_matching_regex_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_texts_matching_regex_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_texts_matching_regex_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_patterns_valid_uuid_format_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_patterns_valid_uuid_format_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_percentile_10_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_percentile_10_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_percentile_25_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_percentile_25_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_percentile_75_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_percentile_75_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_percentile_90_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_percentile_90_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_percentile_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_percentile_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_contains_email_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_contains_email_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_contains_email_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_contains_email_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_contains_ip_4_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_contains_ip_4_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_contains_ip_4_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_contains_ip_4_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_contains_ip_6_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_contains_ip_6_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_contains_ip_6_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_contains_ip_6_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_contains_usa_phone_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_contains_usa_phone_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_contains_usa_phone_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_contains_usa_phone_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_contains_usa_zipcode_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_pii_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_pii_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_pii_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_pii_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_pii_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_pii_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_pii_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_population_stddev_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_population_stddev_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_population_variance_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_population_variance_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_profiling_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/column_profiling_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_profiling_check_categories_spec_comparisons.py` & `dqops-1.4.0/dqops/client/models/column_profiling_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_profiling_check_categories_spec_custom.py` & `dqops-1.4.0/dqops/client/models/column_profiling_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_range_max_value_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_range_max_value_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_range_max_value_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_range_max_value_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_range_median_value_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_range_median_value_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_range_min_value_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_range_min_value_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_range_min_value_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_range_min_value_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_range_statistics_collectors_spec.py` & `dqops-1.4.0/dqops/client/models/column_range_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_range_sum_value_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_range_sum_value_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sample_stddev_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_sample_stddev_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sample_variance_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_sample_variance_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sampling_column_samples_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_sampling_column_samples_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sampling_column_samples_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_sampling_column_samples_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sampling_statistics_collectors_spec.py` & `dqops-1.4.0/dqops/client/models/column_sampling_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_schema_column_exists_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_schema_column_exists_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_schema_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_schema_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_schema_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_schema_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_schema_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_schema_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_schema_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_schema_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_schema_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_schema_type_changed_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_schema_type_changed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_spec.py` & `dqops-1.4.0/dqops/client/models/column_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sql_aggregate_expression_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_sql_aggregate_expression_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sql_aggregated_expression_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_sql_aggregated_expression_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sql_condition_failed_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_sql_condition_failed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sql_condition_failed_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_sql_condition_failed_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sql_condition_passed_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_sql_condition_passed_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sql_condition_passed_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_sql_condition_passed_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sql_import_custom_result_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_sql_import_custom_result_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sql_import_custom_result_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_sql_import_custom_result_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_statistics_collectors_root_categories_spec.py` & `dqops-1.4.0/dqops/client/models/column_statistics_collectors_root_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_statistics_model.py` & `dqops-1.4.0/dqops/client/models/column_statistics_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_strings_expected_text_values_in_use_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_strings_expected_text_values_in_use_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_strings_expected_texts_in_top_values_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_strings_expected_texts_in_top_values_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sum_anomaly_differencing_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_sum_anomaly_differencing_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sum_anomaly_stationary_partition_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_sum_anomaly_stationary_partition_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sum_change_1_day_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_sum_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sum_change_30_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_sum_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sum_change_7_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_sum_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sum_change_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_sum_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_sum_in_range_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_sum_in_range_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_text_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_text_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_found_in_set_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_found_in_set_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_length_above_max_length_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_length_above_max_length_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_length_above_max_length_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_length_above_max_length_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_length_below_min_length_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_length_below_min_length_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_length_below_min_length_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_length_below_min_length_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_length_in_range_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_length_in_range_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_match_date_format_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_match_date_format_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_match_date_format_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_match_date_format_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_matching_date_pattern_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_matching_date_pattern_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_matching_name_pattern_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_matching_name_pattern_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_max_length_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_max_length_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_mean_length_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_mean_length_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_min_length_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_min_length_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_text_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_text_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_not_matching_date_pattern_found_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_not_matching_date_pattern_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_not_matching_regex_found_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_not_matching_regex_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_parsable_to_boolean_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_parsable_to_boolean_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_parsable_to_date_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_parsable_to_date_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_parsable_to_float_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_parsable_to_float_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_parsable_to_integer_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_parsable_to_integer_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_text_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_statistics_collectors_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_datatype_detect_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_datatype_detect_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_length_above_max_length_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_length_above_max_length_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_length_above_max_length_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_length_above_max_length_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_length_below_min_length_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_length_below_min_length_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_length_below_min_length_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_length_below_min_length_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_length_in_range_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_length_in_range_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_max_length_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_max_length_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_max_length_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_max_length_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_mean_length_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_mean_length_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_mean_length_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_mean_length_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_min_length_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_min_length_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_min_length_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_min_length_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_parsable_to_boolean_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_parsable_to_boolean_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_parsable_to_date_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_parsable_to_date_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_parsable_to_float_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_parsable_to_float_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_parsable_to_integer_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_parsable_to_integer_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_valid_country_code_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_valid_country_code_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_text_valid_currency_code_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_text_valid_currency_code_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_valid_country_code_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_valid_country_code_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_text_valid_currency_code_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_text_valid_currency_code_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_texts_matching_regex_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_texts_matching_regex_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_true_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_true_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_type_snapshot_spec.py` & `dqops-1.4.0/dqops/client/models/column_type_snapshot_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_distinct_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_distinct_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_distinct_count_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_distinct_count_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_distinct_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_distinct_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_distinct_percent_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_distinct_percent_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_duplicate_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_duplicate_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_duplicate_count_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_duplicate_count_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_duplicate_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_duplicate_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_duplicate_percent_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_duplicate_percent_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_uniqueness_statistics_collectors_spec.py` & `dqops-1.4.0/dqops/client/models/column_uniqueness_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_valid_latitude_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_valid_latitude_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_valid_longitude_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_valid_longitude_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_valid_uuid_format_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_valid_uuid_format_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_blank_null_placeholder_text_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_empty_text_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_empty_text_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_empty_text_found_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_empty_text_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_empty_text_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_empty_text_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_empty_text_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_empty_text_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_null_placeholder_text_found_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_null_placeholder_text_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_null_placeholder_text_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_null_placeholder_text_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_found_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_text_surrounded_by_whitespace_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_whitespace_text_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_whitespace_text_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_whitespace_text_found_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_whitespace_text_found_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_whitespace_text_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_whitespace_text_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/column_whitespace_whitespace_text_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/column_whitespace_whitespace_text_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/comment_spec.py` & `dqops-1.4.0/dqops/client/models/comment_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/common_column_model.py` & `dqops-1.4.0/dqops/client/models/common_column_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/compare_thresholds_model.py` & `dqops-1.4.0/dqops/client/models/compare_thresholds_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/comparison_check_result_model.py` & `dqops-1.4.0/dqops/client/models/comparison_check_result_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/connection_incident_grouping_spec.py` & `dqops-1.4.0/dqops/client/models/connection_incident_grouping_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/connection_model.py` & `dqops-1.4.0/dqops/client/models/connection_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/connection_spec.py` & `dqops-1.4.0/dqops/client/models/connection_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/connection_specification_model.py` & `dqops-1.4.0/dqops/client/models/connection_specification_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/connection_test_model.py` & `dqops-1.4.0/dqops/client/models/connection_test_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/count_between_rule_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/count_between_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/csv_file_format_spec.py` & `dqops-1.4.0/dqops/client/models/csv_file_format_spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     """
     Attributes:
         all_varchar (Union[Unset, bool]): Option to skip type detection for CSV parsing and assume all columns to be of
             type VARCHAR.
         allow_quoted_nulls (Union[Unset, bool]): Option to allow the conversion of quoted values to NULL values.
         auto_detect (Union[Unset, bool]): Enables auto detection of CSV parameters.
         compression (Union[Unset, CompressionType]):
+        no_compression_extension (Union[Unset, bool]): Whether the compression extension is present at the end of the
+            file name.
         dateformat (Union[Unset, str]): Specifies the date format to use when parsing dates.
         decimal_separator (Union[Unset, str]): The decimal separator of numbers.
         delim (Union[Unset, str]): Specifies the string that separates columns within each row (line) of the file.
         escape (Union[Unset, str]): Specifies the string that should appear before a data character sequence that
             matches the quote value.
         filename (Union[Unset, bool]): Whether or not an extra filename column should be included in the result.
         header (Union[Unset, bool]): Specifies that the file contains a header line with the names of each column in the
@@ -37,14 +39,15 @@
         timestampformat (Union[Unset, str]): Specifies the date format to use when parsing timestamps.
     """
 
     all_varchar: Union[Unset, bool] = UNSET
     allow_quoted_nulls: Union[Unset, bool] = UNSET
     auto_detect: Union[Unset, bool] = UNSET
     compression: Union[Unset, CompressionType] = UNSET
+    no_compression_extension: Union[Unset, bool] = UNSET
     dateformat: Union[Unset, str] = UNSET
     decimal_separator: Union[Unset, str] = UNSET
     delim: Union[Unset, str] = UNSET
     escape: Union[Unset, str] = UNSET
     filename: Union[Unset, bool] = UNSET
     header: Union[Unset, bool] = UNSET
     hive_partitioning: Union[Unset, bool] = UNSET
@@ -60,14 +63,15 @@
         all_varchar = self.all_varchar
         allow_quoted_nulls = self.allow_quoted_nulls
         auto_detect = self.auto_detect
         compression: Union[Unset, str] = UNSET
         if not isinstance(self.compression, Unset):
             compression = self.compression.value
 
+        no_compression_extension = self.no_compression_extension
         dateformat = self.dateformat
         decimal_separator = self.decimal_separator
         delim = self.delim
         escape = self.escape
         filename = self.filename
         header = self.header
         hive_partitioning = self.hive_partitioning
@@ -88,14 +92,16 @@
             field_dict["all_varchar"] = all_varchar
         if allow_quoted_nulls is not UNSET:
             field_dict["allow_quoted_nulls"] = allow_quoted_nulls
         if auto_detect is not UNSET:
             field_dict["auto_detect"] = auto_detect
         if compression is not UNSET:
             field_dict["compression"] = compression
+        if no_compression_extension is not UNSET:
+            field_dict["no_compression_extension"] = no_compression_extension
         if dateformat is not UNSET:
             field_dict["dateformat"] = dateformat
         if decimal_separator is not UNSET:
             field_dict["decimal_separator"] = decimal_separator
         if delim is not UNSET:
             field_dict["delim"] = delim
         if escape is not UNSET:
@@ -133,14 +139,16 @@
         _compression = d.pop("compression", UNSET)
         compression: Union[Unset, CompressionType]
         if isinstance(_compression, Unset):
             compression = UNSET
         else:
             compression = CompressionType(_compression)
 
+        no_compression_extension = d.pop("no_compression_extension", UNSET)
+
         dateformat = d.pop("dateformat", UNSET)
 
         decimal_separator = d.pop("decimal_separator", UNSET)
 
         delim = d.pop("delim", UNSET)
 
         escape = d.pop("escape", UNSET)
@@ -169,14 +177,15 @@
         timestampformat = d.pop("timestampformat", UNSET)
 
         csv_file_format_spec = cls(
             all_varchar=all_varchar,
             allow_quoted_nulls=allow_quoted_nulls,
             auto_detect=auto_detect,
             compression=compression,
+            no_compression_extension=no_compression_extension,
             dateformat=dateformat,
             decimal_separator=decimal_separator,
             delim=delim,
             escape=escape,
             filename=filename,
             header=header,
             hive_partitioning=hive_partitioning,
```

### Comparing `dqops-1.3.0/dqops/client/models/custom_check_spec.py` & `dqops-1.4.0/dqops/client/models/custom_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/custom_rule_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/custom_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/custom_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/custom_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dashboard_spec.py` & `dqops-1.4.0/dqops/client/models/dashboard_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dashboard_spec_parameters.py` & `dqops-1.4.0/dqops/client/models/dashboard_spec_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dashboards_folder_spec.py` & `dqops-1.4.0/dqops/client/models/dashboards_folder_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/data_delete_result_partition.py` & `dqops-1.4.0/dqops/client/models/data_delete_result_partition.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/data_dictionary_list_model.py` & `dqops-1.4.0/dqops/client/models/data_dictionary_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/data_dictionary_model.py` & `dqops-1.4.0/dqops/client/models/data_dictionary_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/data_grouping_configuration_list_model.py` & `dqops-1.4.0/dqops/client/models/data_grouping_configuration_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/data_grouping_configuration_model.py` & `dqops-1.4.0/dqops/client/models/data_grouping_configuration_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/data_grouping_configuration_spec.py` & `dqops-1.4.0/dqops/client/models/data_grouping_configuration_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/data_grouping_configuration_trimmed_model.py` & `dqops-1.4.0/dqops/client/models/data_grouping_configuration_trimmed_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/data_grouping_dimension_spec.py` & `dqops-1.4.0/dqops/client/models/data_grouping_dimension_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/data_type_category.py` & `dqops-1.4.0/dqops/client/models/data_type_category.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/databricks_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/databricks_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/databricks_parameters_spec_properties.py` & `dqops-1.4.0/dqops/client/models/databricks_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/default_column_checks_pattern_list_model.py` & `dqops-1.4.0/dqops/client/models/default_column_checks_pattern_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,98 +2,93 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.target_column_pattern_spec import TargetColumnPatternSpec
+    from ..models.column_default_checks_pattern_spec import (
+        ColumnDefaultChecksPatternSpec,
+    )
 
 
-T = TypeVar("T", bound="DefaultColumnChecksPatternListModel")
+T = TypeVar("T", bound="DefaultColumnChecksPatternModel")
 
 
 @_attrs_define
-class DefaultColumnChecksPatternListModel:
-    """Default column-level checks pattern list model
+class DefaultColumnChecksPatternModel:
+    """Default column-level checks pattern model
 
     Attributes:
-        pattern_name (Union[Unset, str]): Pattern name.
-        priority (Union[Unset, int]): The priority of the pattern. Patterns with lower values are applied before
-            patterns with higher priority values.
-        target_column (Union[Unset, TargetColumnPatternSpec]):
+        pattern_name (Union[Unset, str]): Pattern name
+        pattern_spec (Union[Unset, ColumnDefaultChecksPatternSpec]):
         can_edit (Union[Unset, bool]): Boolean flag that decides if the current user can update or delete this object.
         yaml_parsing_error (Union[Unset, str]): Optional parsing error that was captured when parsing the YAML file.
             This field is null when the YAML file is valid. If an error was captured, this field returns the file parsing
             error message and the file location.
     """
 
     pattern_name: Union[Unset, str] = UNSET
-    priority: Union[Unset, int] = UNSET
-    target_column: Union[Unset, "TargetColumnPatternSpec"] = UNSET
+    pattern_spec: Union[Unset, "ColumnDefaultChecksPatternSpec"] = UNSET
     can_edit: Union[Unset, bool] = UNSET
     yaml_parsing_error: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         pattern_name = self.pattern_name
-        priority = self.priority
-        target_column: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.target_column, Unset):
-            target_column = self.target_column.to_dict()
+        pattern_spec: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.pattern_spec, Unset):
+            pattern_spec = self.pattern_spec.to_dict()
 
         can_edit = self.can_edit
         yaml_parsing_error = self.yaml_parsing_error
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if pattern_name is not UNSET:
             field_dict["pattern_name"] = pattern_name
-        if priority is not UNSET:
-            field_dict["priority"] = priority
-        if target_column is not UNSET:
-            field_dict["target_column"] = target_column
+        if pattern_spec is not UNSET:
+            field_dict["pattern_spec"] = pattern_spec
         if can_edit is not UNSET:
             field_dict["can_edit"] = can_edit
         if yaml_parsing_error is not UNSET:
             field_dict["yaml_parsing_error"] = yaml_parsing_error
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.target_column_pattern_spec import TargetColumnPatternSpec
+        from ..models.column_default_checks_pattern_spec import (
+            ColumnDefaultChecksPatternSpec,
+        )
 
         d = src_dict.copy()
         pattern_name = d.pop("pattern_name", UNSET)
 
-        priority = d.pop("priority", UNSET)
-
-        _target_column = d.pop("target_column", UNSET)
-        target_column: Union[Unset, TargetColumnPatternSpec]
-        if isinstance(_target_column, Unset):
-            target_column = UNSET
+        _pattern_spec = d.pop("pattern_spec", UNSET)
+        pattern_spec: Union[Unset, ColumnDefaultChecksPatternSpec]
+        if isinstance(_pattern_spec, Unset):
+            pattern_spec = UNSET
         else:
-            target_column = TargetColumnPatternSpec.from_dict(_target_column)
+            pattern_spec = ColumnDefaultChecksPatternSpec.from_dict(_pattern_spec)
 
         can_edit = d.pop("can_edit", UNSET)
 
         yaml_parsing_error = d.pop("yaml_parsing_error", UNSET)
 
-        default_column_checks_pattern_list_model = cls(
+        default_column_checks_pattern_model = cls(
             pattern_name=pattern_name,
-            priority=priority,
-            target_column=target_column,
+            pattern_spec=pattern_spec,
             can_edit=can_edit,
             yaml_parsing_error=yaml_parsing_error,
         )
 
-        default_column_checks_pattern_list_model.additional_properties = d
-        return default_column_checks_pattern_list_model
+        default_column_checks_pattern_model.additional_properties = d
+        return default_column_checks_pattern_model
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dqops-1.3.0/dqops/client/models/default_column_checks_pattern_model.py` & `dqops-1.4.0/dqops/client/models/default_table_checks_pattern_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,37 +2,35 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.column_default_checks_pattern_spec import (
-        ColumnDefaultChecksPatternSpec,
-    )
+    from ..models.table_default_checks_pattern_spec import TableDefaultChecksPatternSpec
 
 
-T = TypeVar("T", bound="DefaultColumnChecksPatternModel")
+T = TypeVar("T", bound="DefaultTableChecksPatternModel")
 
 
 @_attrs_define
-class DefaultColumnChecksPatternModel:
-    """Default column-level checks pattern model
+class DefaultTableChecksPatternModel:
+    """Default table-level checks pattern model
 
     Attributes:
         pattern_name (Union[Unset, str]): Pattern name
-        pattern_spec (Union[Unset, ColumnDefaultChecksPatternSpec]):
+        pattern_spec (Union[Unset, TableDefaultChecksPatternSpec]):
         can_edit (Union[Unset, bool]): Boolean flag that decides if the current user can update or delete this object.
         yaml_parsing_error (Union[Unset, str]): Optional parsing error that was captured when parsing the YAML file.
             This field is null when the YAML file is valid. If an error was captured, this field returns the file parsing
             error message and the file location.
     """
 
     pattern_name: Union[Unset, str] = UNSET
-    pattern_spec: Union[Unset, "ColumnDefaultChecksPatternSpec"] = UNSET
+    pattern_spec: Union[Unset, "TableDefaultChecksPatternSpec"] = UNSET
     can_edit: Union[Unset, bool] = UNSET
     yaml_parsing_error: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         pattern_name = self.pattern_name
         pattern_spec: Union[Unset, Dict[str, Any]] = UNSET
@@ -54,41 +52,41 @@
         if yaml_parsing_error is not UNSET:
             field_dict["yaml_parsing_error"] = yaml_parsing_error
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.column_default_checks_pattern_spec import (
-            ColumnDefaultChecksPatternSpec,
+        from ..models.table_default_checks_pattern_spec import (
+            TableDefaultChecksPatternSpec,
         )
 
         d = src_dict.copy()
         pattern_name = d.pop("pattern_name", UNSET)
 
         _pattern_spec = d.pop("pattern_spec", UNSET)
-        pattern_spec: Union[Unset, ColumnDefaultChecksPatternSpec]
+        pattern_spec: Union[Unset, TableDefaultChecksPatternSpec]
         if isinstance(_pattern_spec, Unset):
             pattern_spec = UNSET
         else:
-            pattern_spec = ColumnDefaultChecksPatternSpec.from_dict(_pattern_spec)
+            pattern_spec = TableDefaultChecksPatternSpec.from_dict(_pattern_spec)
 
         can_edit = d.pop("can_edit", UNSET)
 
         yaml_parsing_error = d.pop("yaml_parsing_error", UNSET)
 
-        default_column_checks_pattern_model = cls(
+        default_table_checks_pattern_model = cls(
             pattern_name=pattern_name,
             pattern_spec=pattern_spec,
             can_edit=can_edit,
             yaml_parsing_error=yaml_parsing_error,
         )
 
-        default_column_checks_pattern_model.additional_properties = d
-        return default_column_checks_pattern_model
+        default_table_checks_pattern_model.additional_properties = d
+        return default_table_checks_pattern_model
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dqops-1.3.0/dqops/client/models/default_schedules_spec.py` & `dqops-1.4.0/dqops/client/models/default_schedules_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/default_table_checks_pattern_list_model.py` & `dqops-1.4.0/dqops/client/models/default_table_checks_pattern_list_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,45 +16,55 @@
 class DefaultTableChecksPatternListModel:
     """Default table-level checks pattern list model
 
     Attributes:
         pattern_name (Union[Unset, str]): Pattern name.
         priority (Union[Unset, int]): The priority of the pattern. Patterns with lower values are applied before
             patterns with higher priority values.
+        disabled (Union[Unset, bool]): Disables this data quality check configuration. The checks will not be activated.
+        description (Union[Unset, str]): The description (documentation) of this data quality check configuration.
         target_table (Union[Unset, TargetTablePatternSpec]):
         can_edit (Union[Unset, bool]): Boolean flag that decides if the current user can update or delete this object.
         yaml_parsing_error (Union[Unset, str]): Optional parsing error that was captured when parsing the YAML file.
             This field is null when the YAML file is valid. If an error was captured, this field returns the file parsing
             error message and the file location.
     """
 
     pattern_name: Union[Unset, str] = UNSET
     priority: Union[Unset, int] = UNSET
+    disabled: Union[Unset, bool] = UNSET
+    description: Union[Unset, str] = UNSET
     target_table: Union[Unset, "TargetTablePatternSpec"] = UNSET
     can_edit: Union[Unset, bool] = UNSET
     yaml_parsing_error: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         pattern_name = self.pattern_name
         priority = self.priority
+        disabled = self.disabled
+        description = self.description
         target_table: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.target_table, Unset):
             target_table = self.target_table.to_dict()
 
         can_edit = self.can_edit
         yaml_parsing_error = self.yaml_parsing_error
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if pattern_name is not UNSET:
             field_dict["pattern_name"] = pattern_name
         if priority is not UNSET:
             field_dict["priority"] = priority
+        if disabled is not UNSET:
+            field_dict["disabled"] = disabled
+        if description is not UNSET:
+            field_dict["description"] = description
         if target_table is not UNSET:
             field_dict["target_table"] = target_table
         if can_edit is not UNSET:
             field_dict["can_edit"] = can_edit
         if yaml_parsing_error is not UNSET:
             field_dict["yaml_parsing_error"] = yaml_parsing_error
 
@@ -65,28 +75,34 @@
         from ..models.target_table_pattern_spec import TargetTablePatternSpec
 
         d = src_dict.copy()
         pattern_name = d.pop("pattern_name", UNSET)
 
         priority = d.pop("priority", UNSET)
 
+        disabled = d.pop("disabled", UNSET)
+
+        description = d.pop("description", UNSET)
+
         _target_table = d.pop("target_table", UNSET)
         target_table: Union[Unset, TargetTablePatternSpec]
         if isinstance(_target_table, Unset):
             target_table = UNSET
         else:
             target_table = TargetTablePatternSpec.from_dict(_target_table)
 
         can_edit = d.pop("can_edit", UNSET)
 
         yaml_parsing_error = d.pop("yaml_parsing_error", UNSET)
 
         default_table_checks_pattern_list_model = cls(
             pattern_name=pattern_name,
             priority=priority,
+            disabled=disabled,
+            description=description,
             target_table=target_table,
             can_edit=can_edit,
             yaml_parsing_error=yaml_parsing_error,
         )
 
         default_table_checks_pattern_list_model.additional_properties = d
         return default_table_checks_pattern_list_model
```

### Comparing `dqops-1.3.0/dqops/client/models/default_table_checks_pattern_model.py` & `dqops-1.4.0/dqops/client/models/rule_list_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,93 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.table_default_checks_pattern_spec import TableDefaultChecksPatternSpec
-
-
-T = TypeVar("T", bound="DefaultTableChecksPatternModel")
+T = TypeVar("T", bound="RuleListModel")
 
 
 @_attrs_define
-class DefaultTableChecksPatternModel:
-    """Default table-level checks pattern model
+class RuleListModel:
+    """Rule list model
 
     Attributes:
-        pattern_name (Union[Unset, str]): Pattern name
-        pattern_spec (Union[Unset, TableDefaultChecksPatternSpec]):
+        rule_name (Union[Unset, str]): Rule name without the folder.
+        full_rule_name (Union[Unset, str]): Full rule name, including the folder within the "rules" rule folder.
+        custom (Union[Unset, bool]): This rule has is a custom rule or was customized by the user. This is a read-only
+            value.
+        built_in (Union[Unset, bool]): This rule is provided with DQOps as a built-in rule. This is a read-only value.
         can_edit (Union[Unset, bool]): Boolean flag that decides if the current user can update or delete this object.
         yaml_parsing_error (Union[Unset, str]): Optional parsing error that was captured when parsing the YAML file.
             This field is null when the YAML file is valid. If an error was captured, this field returns the file parsing
             error message and the file location.
     """
 
-    pattern_name: Union[Unset, str] = UNSET
-    pattern_spec: Union[Unset, "TableDefaultChecksPatternSpec"] = UNSET
+    rule_name: Union[Unset, str] = UNSET
+    full_rule_name: Union[Unset, str] = UNSET
+    custom: Union[Unset, bool] = UNSET
+    built_in: Union[Unset, bool] = UNSET
     can_edit: Union[Unset, bool] = UNSET
     yaml_parsing_error: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        pattern_name = self.pattern_name
-        pattern_spec: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.pattern_spec, Unset):
-            pattern_spec = self.pattern_spec.to_dict()
-
+        rule_name = self.rule_name
+        full_rule_name = self.full_rule_name
+        custom = self.custom
+        built_in = self.built_in
         can_edit = self.can_edit
         yaml_parsing_error = self.yaml_parsing_error
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if pattern_name is not UNSET:
-            field_dict["pattern_name"] = pattern_name
-        if pattern_spec is not UNSET:
-            field_dict["pattern_spec"] = pattern_spec
+        if rule_name is not UNSET:
+            field_dict["rule_name"] = rule_name
+        if full_rule_name is not UNSET:
+            field_dict["full_rule_name"] = full_rule_name
+        if custom is not UNSET:
+            field_dict["custom"] = custom
+        if built_in is not UNSET:
+            field_dict["built_in"] = built_in
         if can_edit is not UNSET:
             field_dict["can_edit"] = can_edit
         if yaml_parsing_error is not UNSET:
             field_dict["yaml_parsing_error"] = yaml_parsing_error
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.table_default_checks_pattern_spec import (
-            TableDefaultChecksPatternSpec,
-        )
-
         d = src_dict.copy()
-        pattern_name = d.pop("pattern_name", UNSET)
+        rule_name = d.pop("rule_name", UNSET)
+
+        full_rule_name = d.pop("full_rule_name", UNSET)
+
+        custom = d.pop("custom", UNSET)
 
-        _pattern_spec = d.pop("pattern_spec", UNSET)
-        pattern_spec: Union[Unset, TableDefaultChecksPatternSpec]
-        if isinstance(_pattern_spec, Unset):
-            pattern_spec = UNSET
-        else:
-            pattern_spec = TableDefaultChecksPatternSpec.from_dict(_pattern_spec)
+        built_in = d.pop("built_in", UNSET)
 
         can_edit = d.pop("can_edit", UNSET)
 
         yaml_parsing_error = d.pop("yaml_parsing_error", UNSET)
 
-        default_table_checks_pattern_model = cls(
-            pattern_name=pattern_name,
-            pattern_spec=pattern_spec,
+        rule_list_model = cls(
+            rule_name=rule_name,
+            full_rule_name=full_rule_name,
+            custom=custom,
+            built_in=built_in,
             can_edit=can_edit,
             yaml_parsing_error=yaml_parsing_error,
         )
 
-        default_table_checks_pattern_model.additional_properties = d
-        return default_table_checks_pattern_model
+        rule_list_model.additional_properties = d
+        return rule_list_model
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dqops-1.3.0/dqops/client/models/delete_stored_data_queue_job_parameters.py` & `dqops-1.4.0/dqops/client/models/delete_stored_data_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/delete_stored_data_queue_job_result.py` & `dqops-1.4.0/dqops/client/models/delete_stored_data_queue_job_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/delete_stored_data_result.py` & `dqops-1.4.0/dqops/client/models/delete_stored_data_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/delete_stored_data_result_partition_results.py` & `dqops-1.4.0/dqops/client/models/delete_stored_data_result_partition_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/detected_datatype_equals_rule_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/detected_datatype_equals_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dimension_current_data_quality_status_model.py` & `dqops-1.4.0/dqops/client/models/dimension_current_data_quality_status_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dqo_cloud_user_model.py` & `dqops-1.4.0/dqops/client/models/dqo_cloud_user_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dqo_job_change_model.py` & `dqops-1.4.0/dqops/client/models/dqo_job_change_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dqo_job_entry_parameters_model.py` & `dqops-1.4.0/dqops/client/models/dqo_job_entry_parameters_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dqo_job_history_entry_model.py` & `dqops-1.4.0/dqops/client/models/dqo_job_history_entry_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dqo_job_queue_incremental_snapshot_model.py` & `dqops-1.4.0/dqops/client/models/dqo_job_queue_incremental_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dqo_job_queue_initial_snapshot_model.py` & `dqops-1.4.0/dqops/client/models/dqo_job_queue_initial_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dqo_job_type.py` & `dqops-1.4.0/dqops/client/models/dqo_job_type.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dqo_queue_job_id.py` & `dqops-1.4.0/dqops/client/models/dqo_queue_job_id.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dqo_root.py` & `dqops-1.4.0/dqops/client/models/dqo_root.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dqo_settings_model.py` & `dqops-1.4.0/dqops/client/models/dqo_settings_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dqo_settings_model_properties.py` & `dqops-1.4.0/dqops/client/models/dqo_settings_model_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dqo_settings_model_properties_additional_property.py` & `dqops-1.4.0/dqops/client/models/dqo_settings_model_properties_additional_property.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/dqo_user_profile_model.py` & `dqops-1.4.0/dqops/client/models/dqo_user_profile_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/duckdb_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/duckdb_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/duckdb_parameters_spec_directories.py` & `dqops-1.4.0/dqops/client/models/duckdb_parameters_spec_directories.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/duckdb_parameters_spec_properties.py` & `dqops-1.4.0/dqops/client/models/duckdb_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/duration.py` & `dqops-1.4.0/dqops/client/models/duration.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/effective_schedule_model.py` & `dqops-1.4.0/dqops/client/models/effective_schedule_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/equals_1_rule_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/equals_1_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/equals_integer_rule_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/equals_integer_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/error_entry_model.py` & `dqops-1.4.0/dqops/client/models/error_entry_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/errors_list_model.py` & `dqops-1.4.0/dqops/client/models/errors_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/external_log_entry.py` & `dqops-1.4.0/dqops/client/models/external_log_entry.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/field_model.py` & `dqops-1.4.0/dqops/client/models/field_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/file_format_spec.py` & `dqops-1.4.0/dqops/client/models/file_format_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/hierarchy_id_model.py` & `dqops-1.4.0/dqops/client/models/hierarchy_id_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/hierarchy_id_model_path_item.py` & `dqops-1.4.0/dqops/client/models/hierarchy_id_model_path_item.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/import_schema_queue_job_parameters.py` & `dqops-1.4.0/dqops/client/models/import_schema_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/import_severity_rule_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/import_severity_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/import_tables_queue_job_parameters.py` & `dqops-1.4.0/dqops/client/models/import_tables_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/import_tables_queue_job_result.py` & `dqops-1.4.0/dqops/client/models/import_tables_queue_job_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/import_tables_result.py` & `dqops-1.4.0/dqops/client/models/import_tables_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/incident_daily_issues_count.py` & `dqops-1.4.0/dqops/client/models/incident_daily_issues_count.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/incident_issue_histogram_model.py` & `dqops-1.4.0/dqops/client/models/incident_issue_histogram_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/incident_issue_histogram_model_checks.py` & `dqops-1.4.0/dqops/client/models/incident_issue_histogram_model_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/incident_issue_histogram_model_columns.py` & `dqops-1.4.0/dqops/client/models/incident_issue_histogram_model_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/incident_issue_histogram_model_days.py` & `dqops-1.4.0/dqops/client/models/incident_issue_histogram_model_days.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/incident_model.py` & `dqops-1.4.0/dqops/client/models/incident_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/incident_webhook_notifications_spec.py` & `dqops-1.4.0/dqops/client/models/incident_webhook_notifications_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/incidents_per_connection_model.py` & `dqops-1.4.0/dqops/client/models/incidents_per_connection_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,44 +10,53 @@
 
 @_attrs_define
 class IncidentsPerConnectionModel:
     """
     Attributes:
         connection (Union[Unset, str]): Connection (data source) name.
         open_incidents (Union[Unset, int]): Count of open (new) data quality incidents.
+        most_recent_first_seen (Union[Unset, int]): The UTC timestamp when the most recent data quality incident was
+            first seen.
     """
 
     connection: Union[Unset, str] = UNSET
     open_incidents: Union[Unset, int] = UNSET
+    most_recent_first_seen: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         connection = self.connection
         open_incidents = self.open_incidents
+        most_recent_first_seen = self.most_recent_first_seen
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if connection is not UNSET:
             field_dict["connection"] = connection
         if open_incidents is not UNSET:
             field_dict["openIncidents"] = open_incidents
+        if most_recent_first_seen is not UNSET:
+            field_dict["mostRecentFirstSeen"] = most_recent_first_seen
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         connection = d.pop("connection", UNSET)
 
         open_incidents = d.pop("openIncidents", UNSET)
 
+        most_recent_first_seen = d.pop("mostRecentFirstSeen", UNSET)
+
         incidents_per_connection_model = cls(
             connection=connection,
             open_incidents=open_incidents,
+            most_recent_first_seen=most_recent_first_seen,
         )
 
         incidents_per_connection_model.additional_properties = d
         return incidents_per_connection_model
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `dqops-1.3.0/dqops/client/models/json_file_format_spec.py` & `dqops-1.4.0/dqops/client/models/json_file_format_spec.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 @_attrs_define
 class JsonFileFormatSpec:
     """
     Attributes:
         auto_detect (Union[Unset, bool]): Whether to auto-detect detect the names of the keys and data types of the
             values automatically.
         compression (Union[Unset, CompressionType]):
+        no_compression_extension (Union[Unset, bool]): Whether the compression extension is present at the end of the
+            file name.
         convert_strings_to_integers (Union[Unset, bool]): Whether strings representing integer values should be
             converted to a numerical type.
         dateformat (Union[Unset, str]): Specifies the date format to use when parsing dates.
         filename (Union[Unset, bool]): Whether or not an extra filename column should be included in the result.
         format_ (Union[Unset, JsonFormatType]):
         hive_partitioning (Union[Unset, bool]): Whether or not to interpret the path as a hive partitioned path.
         ignore_errors (Union[Unset, bool]): Whether to ignore parse errors (only possible when format is
@@ -32,14 +34,15 @@
         records (Union[Unset, JsonRecordsType]):
         sample_size (Union[Unset, int]): The number of sample rows for auto detection of parameters.
         timestampformat (Union[Unset, str]): Specifies the date format to use when parsing timestamps.
     """
 
     auto_detect: Union[Unset, bool] = UNSET
     compression: Union[Unset, CompressionType] = UNSET
+    no_compression_extension: Union[Unset, bool] = UNSET
     convert_strings_to_integers: Union[Unset, bool] = UNSET
     dateformat: Union[Unset, str] = UNSET
     filename: Union[Unset, bool] = UNSET
     format_: Union[Unset, JsonFormatType] = UNSET
     hive_partitioning: Union[Unset, bool] = UNSET
     ignore_errors: Union[Unset, bool] = UNSET
     maximum_depth: Union[Unset, int] = UNSET
@@ -51,14 +54,15 @@
 
     def to_dict(self) -> Dict[str, Any]:
         auto_detect = self.auto_detect
         compression: Union[Unset, str] = UNSET
         if not isinstance(self.compression, Unset):
             compression = self.compression.value
 
+        no_compression_extension = self.no_compression_extension
         convert_strings_to_integers = self.convert_strings_to_integers
         dateformat = self.dateformat
         filename = self.filename
         format_: Union[Unset, str] = UNSET
         if not isinstance(self.format_, Unset):
             format_ = self.format_.value
 
@@ -76,14 +80,16 @@
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if auto_detect is not UNSET:
             field_dict["auto_detect"] = auto_detect
         if compression is not UNSET:
             field_dict["compression"] = compression
+        if no_compression_extension is not UNSET:
+            field_dict["no_compression_extension"] = no_compression_extension
         if convert_strings_to_integers is not UNSET:
             field_dict["convert_strings_to_integers"] = convert_strings_to_integers
         if dateformat is not UNSET:
             field_dict["dateformat"] = dateformat
         if filename is not UNSET:
             field_dict["filename"] = filename
         if format_ is not UNSET:
@@ -113,14 +119,16 @@
         _compression = d.pop("compression", UNSET)
         compression: Union[Unset, CompressionType]
         if isinstance(_compression, Unset):
             compression = UNSET
         else:
             compression = CompressionType(_compression)
 
+        no_compression_extension = d.pop("no_compression_extension", UNSET)
+
         convert_strings_to_integers = d.pop("convert_strings_to_integers", UNSET)
 
         dateformat = d.pop("dateformat", UNSET)
 
         filename = d.pop("filename", UNSET)
 
         _format_ = d.pop("format", UNSET)
@@ -148,14 +156,15 @@
         sample_size = d.pop("sample_size", UNSET)
 
         timestampformat = d.pop("timestampformat", UNSET)
 
         json_file_format_spec = cls(
             auto_detect=auto_detect,
             compression=compression,
+            no_compression_extension=no_compression_extension,
             convert_strings_to_integers=convert_strings_to_integers,
             dateformat=dateformat,
             filename=filename,
             format_=format_,
             hive_partitioning=hive_partitioning,
             ignore_errors=ignore_errors,
             maximum_depth=maximum_depth,
```

### Comparing `dqops-1.3.0/dqops/client/models/label_model.py` & `dqops-1.4.0/dqops/client/models/label_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_count_rule_0_error_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_count_rule_0_error_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_count_rule_0_warning_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_count_rule_0_warning_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_count_rule_100_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_count_rule_100_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_days_rule_1_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_days_rule_1_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_days_rule_2_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_days_rule_2_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_days_rule_7_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_days_rule_7_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_diff_percent_rule_0_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_diff_percent_rule_0_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_diff_percent_rule_1_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_diff_percent_rule_1_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_diff_percent_rule_5_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_diff_percent_rule_5_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_failures_rule_0_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_failures_rule_0_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_failures_rule_1_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_failures_rule_1_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_failures_rule_5_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_failures_rule_5_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_missing_rule_0_error_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_missing_rule_0_error_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_missing_rule_0_warning_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_missing_rule_0_warning_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_missing_rule_2_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_missing_rule_2_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_percent_rule_0_error_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_percent_rule_0_error_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_percent_rule_0_warning_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_percent_rule_0_warning_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/max_percent_rule_5_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/max_percent_rule_5_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/min_count_rule_1_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/min_count_rule_1_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/min_percent_rule_100_error_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/min_percent_rule_100_error_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/min_percent_rule_100_warning_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/min_percent_rule_100_warning_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/min_percent_rule_95_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/min_percent_rule_95_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/monitoring_schedule_spec.py` & `dqops-1.4.0/dqops/client/models/monitoring_schedule_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/mono.py` & `dqops-1.4.0/dqops/client/models/mono.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/mono_dqo_queue_job_id.py` & `dqops-1.4.0/dqops/client/models/mono_dqo_queue_job_id.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/mono_object.py` & `dqops-1.4.0/dqops/client/models/mono_object.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/mono_void.py` & `dqops-1.4.0/dqops/client/models/mono_void.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/mysql_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/mysql_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/mysql_parameters_spec_properties.py` & `dqops-1.4.0/dqops/client/models/mysql_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/optional.py` & `dqops-1.4.0/dqops/client/models/optional.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/optional_incident_webhook_notifications_spec.py` & `dqops-1.4.0/dqops/client/models/optional_incident_webhook_notifications_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/optional_monitoring_schedule_spec.py` & `dqops-1.4.0/dqops/client/models/optional_monitoring_schedule_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/oracle_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/oracle_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/oracle_parameters_spec_properties.py` & `dqops-1.4.0/dqops/client/models/oracle_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/parameter_definition_spec.py` & `dqops-1.4.0/dqops/client/models/parameter_definition_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/parquet_file_format_spec.py` & `dqops-1.4.0/dqops/client/models/parquet_file_format_spec.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
+from ..models.compression_type import CompressionType
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="ParquetFileFormatSpec")
 
 
 @_attrs_define
 class ParquetFileFormatSpec:
@@ -16,43 +17,57 @@
             flag for strings, causing string columns to be loaded as BLOB instead. Set this to true to load binary columns
             as strings.
         filename (Union[Unset, bool]): Whether or not an extra filename column should be included in the result.
         file_row_number (Union[Unset, bool]): Whether or not to include the file_row_number column.
         hive_partitioning (Union[Unset, bool]): Whether or not to interpret the path as a hive partitioned path.
         union_by_name (Union[Unset, bool]): Whether the columns of multiple schemas should be unified by name, rather
             than by position.
+        compression (Union[Unset, CompressionType]):
+        no_compression_extension (Union[Unset, bool]): Whether the compression extension is present at the end of the
+            file name.
     """
 
     binary_as_string: Union[Unset, bool] = UNSET
     filename: Union[Unset, bool] = UNSET
     file_row_number: Union[Unset, bool] = UNSET
     hive_partitioning: Union[Unset, bool] = UNSET
     union_by_name: Union[Unset, bool] = UNSET
+    compression: Union[Unset, CompressionType] = UNSET
+    no_compression_extension: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         binary_as_string = self.binary_as_string
         filename = self.filename
         file_row_number = self.file_row_number
         hive_partitioning = self.hive_partitioning
         union_by_name = self.union_by_name
+        compression: Union[Unset, str] = UNSET
+        if not isinstance(self.compression, Unset):
+            compression = self.compression.value
+
+        no_compression_extension = self.no_compression_extension
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if binary_as_string is not UNSET:
             field_dict["binary_as_string"] = binary_as_string
         if filename is not UNSET:
             field_dict["filename"] = filename
         if file_row_number is not UNSET:
             field_dict["file_row_number"] = file_row_number
         if hive_partitioning is not UNSET:
             field_dict["hive_partitioning"] = hive_partitioning
         if union_by_name is not UNSET:
             field_dict["union_by_name"] = union_by_name
+        if compression is not UNSET:
+            field_dict["compression"] = compression
+        if no_compression_extension is not UNSET:
+            field_dict["no_compression_extension"] = no_compression_extension
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         binary_as_string = d.pop("binary_as_string", UNSET)
@@ -61,20 +76,31 @@
 
         file_row_number = d.pop("file_row_number", UNSET)
 
         hive_partitioning = d.pop("hive_partitioning", UNSET)
 
         union_by_name = d.pop("union_by_name", UNSET)
 
+        _compression = d.pop("compression", UNSET)
+        compression: Union[Unset, CompressionType]
+        if isinstance(_compression, Unset):
+            compression = UNSET
+        else:
+            compression = CompressionType(_compression)
+
+        no_compression_extension = d.pop("no_compression_extension", UNSET)
+
         parquet_file_format_spec = cls(
             binary_as_string=binary_as_string,
             filename=filename,
             file_row_number=file_row_number,
             hive_partitioning=hive_partitioning,
             union_by_name=union_by_name,
+            compression=compression,
+            no_compression_extension=no_compression_extension,
         )
 
         parquet_file_format_spec.additional_properties = d
         return parquet_file_format_spec
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `dqops-1.3.0/dqops/client/models/partition_incremental_time_window_spec.py` & `dqops-1.4.0/dqops/client/models/partition_incremental_time_window_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/physical_table_name.py` & `dqops-1.4.0/dqops/client/models/physical_table_name.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/postgresql_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/postgresql_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/postgresql_parameters_spec_properties.py` & `dqops-1.4.0/dqops/client/models/postgresql_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/presto_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/presto_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/presto_parameters_spec_properties.py` & `dqops-1.4.0/dqops/client/models/presto_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/profiling_time_period_truncation.py` & `dqops-1.4.0/dqops/client/models/profiling_time_period_truncation.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/provider_sensor_definition_spec.py` & `dqops-1.4.0/dqops/client/models/provider_sensor_definition_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/provider_sensor_definition_spec_parameters.py` & `dqops-1.4.0/dqops/client/models/provider_sensor_definition_spec_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/provider_sensor_list_model.py` & `dqops-1.4.0/dqops/client/models/provider_sensor_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/provider_sensor_model.py` & `dqops-1.4.0/dqops/client/models/provider_sensor_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/quality_category_model.py` & `dqops-1.4.0/dqops/client/models/quality_category_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/redshift_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/redshift_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/redshift_parameters_spec_properties.py` & `dqops-1.4.0/dqops/client/models/redshift_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/remote_table_list_model.py` & `dqops-1.4.0/dqops/client/models/remote_table_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/repair_stored_data_queue_job_parameters.py` & `dqops-1.4.0/dqops/client/models/repair_stored_data_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/rule_folder_model.py` & `dqops-1.4.0/dqops/client/models/rule_folder_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/rule_folder_model_folders.py` & `dqops-1.4.0/dqops/client/models/rule_folder_model_folders.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/rule_list_model.py` & `dqops-1.4.0/dqops/client/models/table_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,98 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RuleListModel")
+if TYPE_CHECKING:
+    from ..models.table_spec import TableSpec
+
+
+T = TypeVar("T", bound="TableModel")
 
 
 @_attrs_define
-class RuleListModel:
-    """Rule list model
+class TableModel:
+    """Full table model, including all nested objects like columns or checks.
 
     Attributes:
-        rule_name (Union[Unset, str]): Rule name without the folder.
-        full_rule_name (Union[Unset, str]): Full rule name, including the folder within the "rules" rule folder.
-        custom (Union[Unset, bool]): This rule has is a custom rule or was customized by the user. This is a read-only
-            value.
-        built_in (Union[Unset, bool]): This rule is provided with DQOps as a built-in rule. This is a read-only value.
+        connection_name (Union[Unset, str]): Connection name.
+        table_hash (Union[Unset, int]): Table hash that identifies the table using a unique hash code.
+        spec (Union[Unset, TableSpec]):
         can_edit (Union[Unset, bool]): Boolean flag that decides if the current user can update or delete this object.
         yaml_parsing_error (Union[Unset, str]): Optional parsing error that was captured when parsing the YAML file.
             This field is null when the YAML file is valid. If an error was captured, this field returns the file parsing
             error message and the file location.
     """
 
-    rule_name: Union[Unset, str] = UNSET
-    full_rule_name: Union[Unset, str] = UNSET
-    custom: Union[Unset, bool] = UNSET
-    built_in: Union[Unset, bool] = UNSET
+    connection_name: Union[Unset, str] = UNSET
+    table_hash: Union[Unset, int] = UNSET
+    spec: Union[Unset, "TableSpec"] = UNSET
     can_edit: Union[Unset, bool] = UNSET
     yaml_parsing_error: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        rule_name = self.rule_name
-        full_rule_name = self.full_rule_name
-        custom = self.custom
-        built_in = self.built_in
+        connection_name = self.connection_name
+        table_hash = self.table_hash
+        spec: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.spec, Unset):
+            spec = self.spec.to_dict()
+
         can_edit = self.can_edit
         yaml_parsing_error = self.yaml_parsing_error
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if rule_name is not UNSET:
-            field_dict["rule_name"] = rule_name
-        if full_rule_name is not UNSET:
-            field_dict["full_rule_name"] = full_rule_name
-        if custom is not UNSET:
-            field_dict["custom"] = custom
-        if built_in is not UNSET:
-            field_dict["built_in"] = built_in
+        if connection_name is not UNSET:
+            field_dict["connection_name"] = connection_name
+        if table_hash is not UNSET:
+            field_dict["table_hash"] = table_hash
+        if spec is not UNSET:
+            field_dict["spec"] = spec
         if can_edit is not UNSET:
             field_dict["can_edit"] = can_edit
         if yaml_parsing_error is not UNSET:
             field_dict["yaml_parsing_error"] = yaml_parsing_error
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        rule_name = d.pop("rule_name", UNSET)
+        from ..models.table_spec import TableSpec
 
-        full_rule_name = d.pop("full_rule_name", UNSET)
+        d = src_dict.copy()
+        connection_name = d.pop("connection_name", UNSET)
 
-        custom = d.pop("custom", UNSET)
+        table_hash = d.pop("table_hash", UNSET)
 
-        built_in = d.pop("built_in", UNSET)
+        _spec = d.pop("spec", UNSET)
+        spec: Union[Unset, TableSpec]
+        if isinstance(_spec, Unset):
+            spec = UNSET
+        else:
+            spec = TableSpec.from_dict(_spec)
 
         can_edit = d.pop("can_edit", UNSET)
 
         yaml_parsing_error = d.pop("yaml_parsing_error", UNSET)
 
-        rule_list_model = cls(
-            rule_name=rule_name,
-            full_rule_name=full_rule_name,
-            custom=custom,
-            built_in=built_in,
+        table_model = cls(
+            connection_name=connection_name,
+            table_hash=table_hash,
+            spec=spec,
             can_edit=can_edit,
             yaml_parsing_error=yaml_parsing_error,
         )
 
-        rule_list_model.additional_properties = d
-        return rule_list_model
+        table_model.additional_properties = d
+        return table_model
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dqops-1.3.0/dqops/client/models/rule_model.py` & `dqops-1.4.0/dqops/client/models/rule_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/rule_model_parameters.py` & `dqops-1.4.0/dqops/client/models/rule_model_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/rule_parameters_model.py` & `dqops-1.4.0/dqops/client/models/rule_parameters_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/rule_thresholds_model.py` & `dqops-1.4.0/dqops/client/models/rule_thresholds_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/rule_time_window_settings_spec.py` & `dqops-1.4.0/dqops/client/models/rule_time_window_settings_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/run_checks_on_table_parameters.py` & `dqops-1.4.0/dqops/client/models/run_checks_on_table_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/run_checks_parameters.py` & `dqops-1.4.0/dqops/client/models/run_checks_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/run_checks_queue_job_result.py` & `dqops-1.4.0/dqops/client/models/run_checks_queue_job_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/run_checks_result.py` & `dqops-1.4.0/dqops/client/models/run_checks_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/schema_model.py` & `dqops-1.4.0/dqops/client/models/schema_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/schema_remote_model.py` & `dqops-1.4.0/dqops/client/models/schema_remote_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/sensor_definition_spec.py` & `dqops-1.4.0/dqops/client/models/sensor_definition_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/sensor_definition_spec_parameters.py` & `dqops-1.4.0/dqops/client/models/sensor_definition_spec_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/sensor_folder_model.py` & `dqops-1.4.0/dqops/client/models/sensor_folder_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/sensor_folder_model_folders.py` & `dqops-1.4.0/dqops/client/models/sensor_folder_model_folders.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/sensor_list_model.py` & `dqops-1.4.0/dqops/client/models/sensor_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/sensor_model.py` & `dqops-1.4.0/dqops/client/models/sensor_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/sensor_readout_entry_model.py` & `dqops-1.4.0/dqops/client/models/sensor_readout_entry_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/sensor_readouts_list_model.py` & `dqops-1.4.0/dqops/client/models/sensor_readouts_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/shared_credential_list_model.py` & `dqops-1.4.0/dqops/client/models/shared_credential_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/shared_credential_model.py` & `dqops-1.4.0/dqops/client/models/shared_credential_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/similar_check_model.py` & `dqops-1.4.0/dqops/client/models/similar_check_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/single_store_db_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/single_store_db_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/snowflake_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/snowflake_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/snowflake_parameters_spec_properties.py` & `dqops-1.4.0/dqops/client/models/snowflake_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/spark_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/spark_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/spark_parameters_spec_properties.py` & `dqops-1.4.0/dqops/client/models/spark_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/spring_error_payload.py` & `dqops-1.4.0/dqops/client/models/spring_error_payload.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/sql_server_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/sql_server_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/sql_server_parameters_spec_properties.py` & `dqops-1.4.0/dqops/client/models/sql_server_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/statistics_collector_search_filters.py` & `dqops-1.4.0/dqops/client/models/statistics_collector_search_filters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/statistics_metric_model.py` & `dqops-1.4.0/dqops/client/models/statistics_metric_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/statistics_metric_model_result.py` & `dqops-1.4.0/dqops/client/models/statistics_metric_model_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/synchronize_multiple_folders_dqo_queue_job_parameters.py` & `dqops-1.4.0/dqops/client/models/synchronize_multiple_folders_dqo_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/synchronize_multiple_folders_queue_job_result.py` & `dqops-1.4.0/dqops/client/models/synchronize_multiple_folders_queue_job_result.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/synchronize_root_folder_dqo_queue_job_parameters.py` & `dqops-1.4.0/dqops/client/models/synchronize_root_folder_dqo_queue_job_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/synchronize_root_folder_parameters.py` & `dqops-1.4.0/dqops/client/models/synchronize_root_folder_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_accuracy_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_accuracy_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_accuracy_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_accuracy_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_accuracy_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_accuracy_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_accuracy_total_row_count_match_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_accuracy_total_row_count_match_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_accuracy_total_row_count_match_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_accuracy_total_row_count_match_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_availability_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_availability_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_availability_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_availability_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_availability_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_availability_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_availability_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_availability_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_availability_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_availability_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_availability_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_availability_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_availability_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_column_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_column_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_column_list_ordered_hash_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_column_list_ordered_hash_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_column_list_unordered_hash_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_column_list_unordered_hash_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_column_types_hash_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_column_types_hash_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_columns_statistics_model.py` & `dqops-1.4.0/dqops/client/models/table_columns_statistics_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_column_count_match_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_comparison_column_count_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_column_results_model.py` & `dqops-1.4.0/dqops/client/models/table_comparison_column_results_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_column_results_model_column_comparison_results.py` & `dqops-1.4.0/dqops/client/models/table_comparison_column_results_model_column_comparison_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_configuration_model.py` & `dqops-1.4.0/dqops/client/models/table_comparison_configuration_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_configuration_spec.py` & `dqops-1.4.0/dqops/client/models/table_comparison_configuration_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_comparison_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_comparison_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_grouping_column_pair_model.py` & `dqops-1.4.0/dqops/client/models/table_comparison_grouping_column_pair_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_grouping_columns_pair_spec.py` & `dqops-1.4.0/dqops/client/models/table_comparison_grouping_columns_pair_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_model.py` & `dqops-1.4.0/dqops/client/models/table_comparison_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_comparison_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_comparison_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_comparison_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_comparison_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_results_model.py` & `dqops-1.4.0/dqops/client/models/table_comparison_results_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_results_model_column_comparison_results.py` & `dqops-1.4.0/dqops/client/models/table_comparison_results_model_column_comparison_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_results_model_table_comparison_results.py` & `dqops-1.4.0/dqops/client/models/table_comparison_results_model_table_comparison_results.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_comparison_row_count_match_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_comparison_row_count_match_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_current_data_quality_status_model.py` & `dqops-1.4.0/dqops/client/models/table_current_data_quality_status_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_current_data_quality_status_model_checks.py` & `dqops-1.4.0/dqops/client/models/table_current_data_quality_status_model_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_current_data_quality_status_model_columns.py` & `dqops-1.4.0/dqops/client/models/table_current_data_quality_status_model_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_current_data_quality_status_model_dimensions.py` & `dqops-1.4.0/dqops/client/models/table_current_data_quality_status_model_dimensions.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_custom_sql_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_custom_sql_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_custom_sql_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_custom_sql_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_custom_sql_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_custom_sql_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_custom_sql_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_custom_sql_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_daily_monitoring_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/table_daily_monitoring_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_daily_monitoring_check_categories_spec_comparisons.py` & `dqops-1.4.0/dqops/client/models/table_daily_monitoring_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_daily_monitoring_check_categories_spec_custom.py` & `dqops-1.4.0/dqops/client/models/table_daily_monitoring_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_daily_partitioned_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/table_daily_partitioned_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_daily_partitioned_check_categories_spec_comparisons.py` & `dqops-1.4.0/dqops/client/models/table_daily_partitioned_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_daily_partitioned_check_categories_spec_custom.py` & `dqops-1.4.0/dqops/client/models/table_daily_partitioned_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_data_freshness_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_data_freshness_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_data_ingestion_delay_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_data_ingestion_delay_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_data_staleness_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_data_staleness_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_default_checks_pattern_spec.py` & `dqops-1.4.0/dqops/client/models/table_default_checks_pattern_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,29 +23,35 @@
 
 @_attrs_define
 class TableDefaultChecksPatternSpec:
     """
     Attributes:
         priority (Union[Unset, int]): The priority of the pattern. Patterns with lower values are applied before
             patterns with higher priority values.
+        disabled (Union[Unset, bool]): Disables this data quality check configuration. The checks will not be activated.
+        description (Union[Unset, str]): The description (documentation) of this data quality check configuration.
         target (Union[Unset, TargetTablePatternSpec]):
         profiling_checks (Union[Unset, TableProfilingCheckCategoriesSpec]):
         monitoring_checks (Union[Unset, TableMonitoringCheckCategoriesSpec]):
         partitioned_checks (Union[Unset, TablePartitionedCheckCategoriesSpec]):
     """
 
     priority: Union[Unset, int] = UNSET
+    disabled: Union[Unset, bool] = UNSET
+    description: Union[Unset, str] = UNSET
     target: Union[Unset, "TargetTablePatternSpec"] = UNSET
     profiling_checks: Union[Unset, "TableProfilingCheckCategoriesSpec"] = UNSET
     monitoring_checks: Union[Unset, "TableMonitoringCheckCategoriesSpec"] = UNSET
     partitioned_checks: Union[Unset, "TablePartitionedCheckCategoriesSpec"] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         priority = self.priority
+        disabled = self.disabled
+        description = self.description
         target: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.target, Unset):
             target = self.target.to_dict()
 
         profiling_checks: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.profiling_checks, Unset):
             profiling_checks = self.profiling_checks.to_dict()
@@ -59,14 +65,18 @@
             partitioned_checks = self.partitioned_checks.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if priority is not UNSET:
             field_dict["priority"] = priority
+        if disabled is not UNSET:
+            field_dict["disabled"] = disabled
+        if description is not UNSET:
+            field_dict["description"] = description
         if target is not UNSET:
             field_dict["target"] = target
         if profiling_checks is not UNSET:
             field_dict["profiling_checks"] = profiling_checks
         if monitoring_checks is not UNSET:
             field_dict["monitoring_checks"] = monitoring_checks
         if partitioned_checks is not UNSET:
@@ -86,14 +96,18 @@
             TableProfilingCheckCategoriesSpec,
         )
         from ..models.target_table_pattern_spec import TargetTablePatternSpec
 
         d = src_dict.copy()
         priority = d.pop("priority", UNSET)
 
+        disabled = d.pop("disabled", UNSET)
+
+        description = d.pop("description", UNSET)
+
         _target = d.pop("target", UNSET)
         target: Union[Unset, TargetTablePatternSpec]
         if isinstance(_target, Unset):
             target = UNSET
         else:
             target = TargetTablePatternSpec.from_dict(_target)
 
@@ -122,14 +136,16 @@
         else:
             partitioned_checks = TablePartitionedCheckCategoriesSpec.from_dict(
                 _partitioned_checks
             )
 
         table_default_checks_pattern_spec = cls(
             priority=priority,
+            disabled=disabled,
+            description=description,
             target=target,
             profiling_checks=profiling_checks,
             monitoring_checks=monitoring_checks,
             partitioned_checks=partitioned_checks,
         )
 
         table_default_checks_pattern_spec.additional_properties = d
```

### Comparing `dqops-1.3.0/dqops/client/models/table_incident_grouping_spec.py` & `dqops-1.4.0/dqops/client/models/table_incident_grouping_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_list_model.py` & `dqops-1.4.0/dqops/client/models/table_list_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_monitoring_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/table_monitoring_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_monthly_monitoring_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/table_monthly_monitoring_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_comparisons.py` & `dqops-1.4.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_custom.py` & `dqops-1.4.0/dqops/client/models/table_monthly_monitoring_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_monthly_partitioned_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/table_monthly_partitioned_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_comparisons.py` & `dqops-1.4.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_custom.py` & `dqops-1.4.0/dqops/client/models/table_monthly_partitioned_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_owner_spec.py` & `dqops-1.4.0/dqops/client/models/table_owner_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_partition_reload_lag_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_partition_reload_lag_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_partitioned_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/table_partitioned_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_partitioning_model.py` & `dqops-1.4.0/dqops/client/models/table_partitioning_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_profiling_check_categories_spec.py` & `dqops-1.4.0/dqops/client/models/table_profiling_check_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_profiling_check_categories_spec_comparisons.py` & `dqops-1.4.0/dqops/client/models/table_profiling_check_categories_spec_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_profiling_check_categories_spec_custom.py` & `dqops-1.4.0/dqops/client/models/table_profiling_check_categories_spec_custom.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_row_count_anomaly_differencing_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_row_count_anomaly_differencing_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_row_count_anomaly_stationary_partition_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_row_count_anomaly_stationary_partition_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_row_count_change_1_day_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_row_count_change_1_day_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_row_count_change_30_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_row_count_change_30_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_row_count_change_7_days_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_row_count_change_7_days_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_row_count_change_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_row_count_change_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_row_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_row_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_schema_column_count_changed_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_schema_column_count_changed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_schema_column_count_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_schema_column_count_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_schema_column_count_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/table_schema_column_count_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_schema_column_list_changed_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_schema_column_list_changed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_schema_column_list_or_order_changed_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_schema_column_list_or_order_changed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_schema_column_types_changed_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_schema_column_types_changed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_schema_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_schema_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_schema_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_schema_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_schema_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_schema_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_schema_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_schema_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_schema_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_schema_statistics_collectors_spec.py` & `dqops-1.4.0/dqops/client/models/table_schema_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_spec.py` & `dqops-1.4.0/dqops/client/models/table_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_spec_columns.py` & `dqops-1.4.0/dqops/client/models/table_spec_columns.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_spec_groupings.py` & `dqops-1.4.0/dqops/client/models/table_spec_groupings.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_spec_table_comparisons.py` & `dqops-1.4.0/dqops/client/models/table_spec_table_comparisons.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_sql_aggregate_expression_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_sql_aggregate_expression_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_sql_aggregated_expression_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_sql_aggregated_expression_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_sql_condition_failed_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_sql_condition_failed_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_sql_condition_failed_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_sql_condition_failed_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_sql_condition_passed_percent_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_sql_condition_passed_percent_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_sql_condition_passed_percent_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_sql_condition_passed_percent_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_sql_import_custom_result_check_spec.py` & `dqops-1.4.0/dqops/client/models/table_sql_import_custom_result_check_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_sql_import_custom_result_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_sql_import_custom_result_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_statistics_collectors_root_categories_spec.py` & `dqops-1.4.0/dqops/client/models/table_statistics_collectors_root_categories_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_statistics_model.py` & `dqops-1.4.0/dqops/client/models/table_statistics_model.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_data_freshness_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_data_freshness_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_data_ingestion_delay_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_data_ingestion_delay_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_data_staleness_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_data_staleness_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_partition_reload_lag_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_partition_reload_lag_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_timeliness_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_timeliness_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_volume_daily_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_volume_daily_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_volume_daily_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_volume_daily_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_volume_daily_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_volume_daily_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_volume_daily_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_volume_daily_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_volume_monthly_monitoring_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_volume_monthly_partitioned_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_volume_profiling_checks_spec.py` & `dqops-1.4.0/dqops/client/models/table_volume_profiling_checks_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_volume_profiling_checks_spec_custom_checks.py` & `dqops-1.4.0/dqops/client/models/table_volume_profiling_checks_spec_custom_checks.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_volume_row_count_sensor_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/table_volume_row_count_sensor_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_volume_row_count_statistics_collector_spec.py` & `dqops-1.4.0/dqops/client/models/table_volume_row_count_statistics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/table_volume_statistics_collectors_spec.py` & `dqops-1.4.0/dqops/client/models/table_volume_statistics_collectors_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/target_column_pattern_spec.py` & `dqops-1.4.0/dqops/client/models/target_column_pattern_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/target_table_pattern_spec.py` & `dqops-1.4.0/dqops/client/models/target_table_pattern_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/temporal_unit.py` & `dqops-1.4.0/dqops/client/models/temporal_unit.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/time_window_filter_parameters.py` & `dqops-1.4.0/dqops/client/models/time_window_filter_parameters.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/timestamp_columns_spec.py` & `dqops-1.4.0/dqops/client/models/timestamp_columns_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/trino_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/trino_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/trino_parameters_spec_properties.py` & `dqops-1.4.0/dqops/client/models/trino_parameters_spec_properties.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/models/value_changed_rule_parameters_spec.py` & `dqops-1.4.0/dqops/client/models/value_changed_rule_parameters_spec.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/client/types.py` & `dqops-1.4.0/dqops/client/types.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/install.py` & `dqops-1.4.0/dqops/install.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/startdqo.py` & `dqops-1.4.0/dqops/startdqo.py`

 * *Files identical despite different names*

### Comparing `dqops-1.3.0/dqops/version.py` & `dqops-1.4.0/dqops/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limit
 
 # WARNING: the next two lines with the version numbers (VERSION =, PIP_VERSION =) should not be modified manually. They are changed by a maven profile at compile time.
-VERSION = "1.3.0"
-PIP_VERSION = "1.3.0"
+VERSION = "1.4.0"
+PIP_VERSION = "1.4.0"
 GITHUB_RELEASE = "v" + VERSION + ""
 JAVA_VERSION = "17"
 
 
 def get_dqo_version():
     return VERSION, PIP_VERSION, GITHUB_RELEASE, JAVA_VERSION
```

### Comparing `dqops-1.3.0/dqops.egg-info/PKG-INFO` & `dqops-1.4.0/dqops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqops
-Version: 1.3.0
+Version: 1.4.0
 Summary: DQOps Data Quality Operations Center
 Home-page: https://github.com/dqops/dqo/tree/master/distribution/python
 Author: DQOps Developers
 Author-email: support@dqops.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dqops-1.3.0/dqops.egg-info/SOURCES.txt` & `dqops-1.4.0/dqops.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -179,19 +179,21 @@
 dqops/client/api/errors/get_column_profiling_errors.py
 dqops/client/api/errors/get_table_monitoring_errors.py
 dqops/client/api/errors/get_table_partitioned_errors.py
 dqops/client/api/errors/get_table_profiling_errors.py
 dqops/client/api/healthcheck/__init__.py
 dqops/client/api/healthcheck/is_healthy.py
 dqops/client/api/incidents/__init__.py
+dqops/client/api/incidents/disable_checks_for_incident.py
 dqops/client/api/incidents/find_connection_incident_stats.py
 dqops/client/api/incidents/find_recent_incidents_on_connection.py
 dqops/client/api/incidents/get_incident.py
 dqops/client/api/incidents/get_incident_histogram.py
 dqops/client/api/incidents/get_incident_issues.py
+dqops/client/api/incidents/recalibrate_checks_for_incident.py
 dqops/client/api/incidents/set_incident_issue_url.py
 dqops/client/api/incidents/set_incident_status.py
 dqops/client/api/jobs/__init__.py
 dqops/client/api/jobs/cancel_job.py
 dqops/client/api/jobs/collect_statistics_on_data_groups.py
 dqops/client/api/jobs/collect_statistics_on_table.py
 dqops/client/api/jobs/delete_stored_data.py
@@ -227,14 +229,15 @@
 dqops/client/api/schemas/get_schema_monitoring_checks_templates.py
 dqops/client/api/schemas/get_schema_partitioned_checks_model.py
 dqops/client/api/schemas/get_schema_partitioned_checks_templates.py
 dqops/client/api/schemas/get_schema_profiling_checks_model.py
 dqops/client/api/schemas/get_schema_profiling_checks_templates.py
 dqops/client/api/schemas/get_schemas.py
 dqops/client/api/search/__init__.py
+dqops/client/api/search/find_columns.py
 dqops/client/api/search/find_tables.py
 dqops/client/api/sensor_readouts/__init__.py
 dqops/client/api/sensor_readouts/get_column_monitoring_sensor_readouts.py
 dqops/client/api/sensor_readouts/get_column_partitioned_sensor_readouts.py
 dqops/client/api/sensor_readouts/get_column_profiling_sensor_readouts.py
 dqops/client/api/sensor_readouts/get_table_monitoring_sensor_readouts.py
 dqops/client/api/sensor_readouts/get_table_partitioned_sensor_readouts.py
```

### Comparing `dqops-1.3.0/setup.py` & `dqops-1.4.0/setup.py`

 * *Files identical despite different names*

