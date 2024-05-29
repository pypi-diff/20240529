# Comparing `tmp/ophyd_devices-1.1.0.tar.gz` & `tmp/ophyd_devices-1.2.0.tar.gz`

## Comparing `ophyd_devices-1.1.0.tar` & `ophyd_devices-1.2.0.tar`

### file list

```diff
@@ -1,402 +1,403 @@
--rw-r--r--   0        0        0     7769 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/README.md
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.git_hooks/pre-commit
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.gitlab/issue_templates/bug_report_template.md
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.gitlab/issue_templates/documentation_update_template.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.gitlab/issue_templates/feature_request_template.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.gitlab/merge_request_templates/default.md
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.gitignore
--rw-r--r--   0        0        0    19819 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.gitlab-ci.yml
--rw-r--r--   0        0        0    18519 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.pylintrc
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.readthedocs.yaml
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/CHANGELOG.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/LICENSE
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/README.md
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_config_template.yaml
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.git_hooks/post-commit
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.git_hooks/pre-commit
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.gitlab/issue_templates/bug_report_template.md
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.gitlab/issue_templates/documentation_update_template.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.gitlab/issue_templates/feature_request_template.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.gitlab/merge_request_templates/default.md
--rw-r--r--   0        0        0     6867 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/demo.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/pyproject.toml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/__init__.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/bec_magics.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/bec_startup.py
--rw-r--r--   0        0        0     8631 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/main.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/prettytable.py
--rw-r--r--   0        0        0    11090 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/progressbar.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/signals.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/__init__.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py
--rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py
--rw-r--r--   0        0        0    12166 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/__init__.py
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/conftest.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py
--rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_bec_client.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_device_progress.py
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_live_table.py
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_move_callback.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_pretty_table.py
--rw-r--r--   0        0        0    25202 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py
--rw-r--r--   0        0        0    11064 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/README.md
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/pyproject.toml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/__init__.py
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/alarm_handler.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/async_data.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bec_errors.py
--rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bec_service.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bec_yaml_loader.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bl_checks.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bl_conditions.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/callback_handler.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/channel_monitor.py
--rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/client.py
--rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/config_helper.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/connector.py
--rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/dap_plugin_objects.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/dap_plugins.py
--rw-r--r--   0        0        0    31017 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/device.py
--rw-r--r--   0        0        0    23466 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/devicemanager.py
--rw-r--r--   0        0        0    38756 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/endpoints.py
--rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/file_utils.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/lmfit_serializer.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/logbook_connector.py
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/logger.py
--rw-r--r--   0        0        0    24060 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/messages.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/numpy_encoder.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/observer.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/pdf_writer.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/plugin_helper.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/queue_items.py
--rw-r--r--   0        0        0    41753 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/redis_connector.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/request_items.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_data.py
--rw-r--r--   0        0        0    11042 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_items.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_manager.py
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_report.py
--rw-r--r--   0        0        0    16698 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scans.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scibec_validator.py
--rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/serialization.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/service_config.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/signature_serializer.py
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/user_scripts_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/configs/__init__.py
--rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/configs/demo_config.yaml
--rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/configs/openapi_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/__init__.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/fixtures.py
--rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/test_config.yaml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/test_service_config.yaml
--rw-r--r--   0        0        0    22495 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/__init__.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/import_utils.py
--rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/proxy.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/rpc_utils.py
--rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/scan_utils.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/threading_utils.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/conftest.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_async_data.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_beamline_checks.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_bec_logger.py
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_bec_messages.py
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_bec_service.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_bl_conditions.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_callback_handler.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_channel_monitor.py
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_config_helper.py
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_core_utils.py
--rw-r--r--   0        0        0    26550 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_dap_plugins.py
--rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_device_manager.py
--rw-r--r--   0        0        0    25863 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_devices.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_file_utils.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_import_utils.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_lmfit_serializer.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_observer.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_pdf_writer.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_plugin_helper.py
--rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_redis_connector.py
--rw-r--r--   0        0        0    22325 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_redis_connector_fakeredis.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_context.py
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_data.py
--rw-r--r--   0        0        0    16743 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_items.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_manager.py
--rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_object.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_report.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scibec_validator.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_serializer.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_signature_serializer.py
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_user_scripts_mixin.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_yaml_loader.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/create_plugin_structure.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/init_config.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/gitignore
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/setup_device_server.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/post-commit
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/pre-commit
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/README.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/pyproject.toml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/launch.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/service_handler.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/dap_server.py
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/dap_service.py
--rw-r--r--   0        0        0     9729 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/dap_service_manager.py
--rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/lmfit1d_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/cli/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/cli/launch.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/__init__.py
--rw-r--r--   0        0        0    19037 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/device_server.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/rpc_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/cli/__init__.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/cli/launch.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/__init__.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/config_update_handler.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/device_serializer.py
--rw-r--r--   0        0        0    22629 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/devicemanager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/tests/__init__.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/tests/utils.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/__init__.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/default_writer.py
--rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/file_writer.py
--rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/file_writer_manager.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/merged_dicts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/cli/__init__.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/cli/launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer_plugins/__init__.py
--rw-r--r--   0        0        0    22204 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/__init__.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/bec_emitter.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/emitter.py
--rw-r--r--   0        0        0    16121 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/scan_bundler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/cli/__init__.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/cli/launch.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/__init__.py
--rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/device_validation.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/errors.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/path_optimization.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_assembler.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_guard.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_manager.py
--rw-r--r--   0        0        0    35246 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_queue.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_server.py
--rw-r--r--   0        0        0    18915 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_stubs.py
--rw-r--r--   0        0        0    35721 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_worker.py
--rw-r--r--   0        0        0    51830 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/cli/__init__.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/cli/launch.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_plugins/__init__.py
--rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/tests/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/tests/fixtures.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/tests/utils.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/repeated_timer.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scihub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/cli/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/cli/launch.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/__init__.py
--rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/config_handler.py
--rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py
--rw-r--r--   0        0        0    10735 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scilog/__init__.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scilog/scilog.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_bec_server_utils/test_main.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/conftest.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_dap_server.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/conftest.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_config_handler.py
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_serializer.py
--rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_server.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py
--rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/conftest.py
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/test_file_writer.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py
--rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/conftest.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_emitter.py
--rw-r--r--   0        0        0    25417 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/conftest.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_path_optimization.py
--rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_guard.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py
--rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py
--rw-r--r--   0        0        0    53947 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_worker.py
--rw-r--r--   0        0        0    87794 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scans.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/conftest.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_repeated_timer.py
--rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py
--rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scibec_connector.py
--rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scilog_connector.py
--rwxr-xr-x   0        0        0     3629 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bin/install_bec_dev.sh
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/Dockerfile.run_pytest
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/Dockerfile.run_server
--rwxr-xr-x   0        0        0      347 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/build_python_services.sh
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/docker-compose.yaml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/functionalAccounts.json
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/semantic_release.toml
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/test_config.yaml
--rw-r--r--   0        0        0   307212 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/architecture/BEC.drawio
--rw-r--r--   0        0        0   124683 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/architecture/BEC_config_db.drawio
--rw-r--r--   0        0        0    11580 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/architecture/BEC_config_db.svg
--rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/architecture/bec_architecture.png
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/Makefile
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/conf.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/make.bat
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/requirements.txt
--rw-r--r--   0        0        0    41260 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/_static/bec.png
--rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/_static/custom.css
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/_static/switcher.json
--rw-r--r--   0        0        0  4672990 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/_static/gif/bec_plotter.gif
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/api_reference/api_reference.md
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/api_reference/modules.rst
--rw-r--r--   0        0        0   310535 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/BEC_context_user_centric.png
--rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/bec_architecture.png
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/bec_device_structure.drawio
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/bec_device_structure.png
--rw-r--r--   0        0        0   185658 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/bec_widgets_glance.png
--rw-r--r--   0        0        0    17460 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/gauss_scatter_plot.png
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/index_api.svg
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/index_contribute.svg
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/index_getting_started.svg
--rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/index_user_guide.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/portrait_48dp.svg
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/precision_manufacturing_48dp.svg
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/rocket_launch_48dp.svg
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/simulation_context_diagram.drawio
--rw-r--r--   0        0        0    69323 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/simulation_context_diagram.png
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/tab-complete-devices.png
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/timeline_48dp.svg
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/toc_48dp.svg
--rw-r--r--   0        0        0    37244 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/vscode_debug_button.png
--rw-r--r--   0        0        0   374770 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/vscode_with_annotations.drawio
--rw-r--r--   0        0        0   711275 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/vscode_with_annotations.png
--rw-r--r--   0        0        0    96330 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/wm-devices.png
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/developer.md
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/glossary.md
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/data_acess/data_access.md
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/data_acess/event_data.md
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/devices/bec_sim.md
--rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/devices/device_configuration.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/devices/devices.md
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/devices/external_sources.md
--rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/devices/ophyd.md
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/architecture.md
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/bec_config.md
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/bec_plugins.md
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/contributing.md
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/getting_started.md
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/install_developer_env.md
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/logs.md
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/tests.md
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/vscode.md
--rw-r--r--   0        0        0    16567 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/scans/scans.md
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/user_interfaces/bec_cli.md
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/user_interfaces/bec_gui.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/user_interfaces/user_interfaces.md
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/introduction/introduction.md
--rw-r--r--   0        0        0    15455 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/user/command_line_interface.md
--rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/user/data_access_and_plotting.md
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/user/devices.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/user/graphical_user_interface.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/user/installation.md
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/user/user.md
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/pytest_bec_e2e/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/pytest_bec_e2e/pytest_bec_e2e/__init__.py
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/ophyd_patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/configs/__init__.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/configs/ophyd_devices_simulation.yaml
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/configs/ophyd_simulation.yaml
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/configs/sls_devices.yaml
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/SpmBase.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/XbpmBase.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/__init__.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/device_list.md
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/epics_motor_ex.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/mono_dccm.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/slits.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/sls_detector.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/sls_devices.py
--rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/specMotors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/base_classes/__init__.py
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py
--rw-r--r--   0        0        0    18126 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py
--rw-r--r--   0        0        0    11151 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/base_classes/psi_detector_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/protocols/__init__.py
--rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/protocols/bec_protocols.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/__init__.py
--rw-r--r--   0        0        0    27788 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/sim.py
--rw-r--r--   0        0        0    28125 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/sim_data.py
--rw-r--r--   0        0        0    12071 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/sim_frameworks.py
--rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/sim_signals.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/sim_test_devices.py
--rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/sim_xtreme.py
--rw-r--r--   0        0        0   671622 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt
--rw-r--r--   0        0        0   669534 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt
--rw-r--r--   0        0        0   670586 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt
--rw-r--r--   0        0        0   668300 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/__init__.py
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/bec_device_base.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/bec_scaninfo_mixin.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/bec_utils.py
--rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/controller.py
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/dynamic_pseudo.py
--rw-r--r--   0        0        0     7309 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/socket.py
--rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/static_device_test.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_base_classes.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_controller.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_dynamic_pseudo.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_ophyd_status_obj.py
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_simulation.py
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_socket.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_static_device_test.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.gitignore
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/LICENSE
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/README.md
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/.git_hooks/pre-commit
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/.gitlab/issue_templates/bug_report_template.md
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/.gitlab/issue_templates/documentation_update_template.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/.gitlab/issue_templates/feature_request_template.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/.gitlab/merge_request_templates/default.md
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/.gitignore
+-rw-r--r--   0        0        0    19819 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/.gitlab-ci.yml
+-rw-r--r--   0        0        0    18519 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/.pylintrc
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/.readthedocs.yaml
+-rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/CHANGELOG.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/LICENSE
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/README.md
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_config_template.yaml
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/.git_hooks/post-commit
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/.git_hooks/pre-commit
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/.gitlab/issue_templates/bug_report_template.md
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/.gitlab/issue_templates/documentation_update_template.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/.gitlab/issue_templates/feature_request_template.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/.gitlab/merge_request_templates/default.md
+-rw-r--r--   0        0        0     6867 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/demo.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/pyproject.toml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/__init__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/bec_magics.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/bec_startup.py
+-rw-r--r--   0        0        0     8631 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/main.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/prettytable.py
+-rw-r--r--   0        0        0    11090 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/progressbar.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/signals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/callbacks/__init__.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py
+-rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py
+-rw-r--r--   0        0        0    12166 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/__init__.py
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/tests/conftest.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/tests/client_tests/test_bec_client.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/tests/client_tests/test_device_progress.py
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/tests/client_tests/test_live_table.py
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/tests/client_tests/test_move_callback.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/tests/client_tests/test_pretty_table.py
+-rw-r--r--   0        0        0    25202 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py
+-rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/README.md
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/pyproject.toml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/__init__.py
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/alarm_handler.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/async_data.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/bec_errors.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/bec_service.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/bec_yaml_loader.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/bl_checks.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/bl_conditions.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/callback_handler.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/channel_monitor.py
+-rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/client.py
+-rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/config_helper.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/connector.py
+-rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/dap_plugin_objects.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/dap_plugins.py
+-rw-r--r--   0        0        0    31017 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/device.py
+-rw-r--r--   0        0        0    23466 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/devicemanager.py
+-rw-r--r--   0        0        0    38756 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/endpoints.py
+-rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/file_utils.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/lmfit_serializer.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/logbook_connector.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/logger.py
+-rw-r--r--   0        0        0    24060 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/messages.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/numpy_encoder.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/observer.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/pdf_writer.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/plugin_helper.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/queue_items.py
+-rw-r--r--   0        0        0    41753 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/redis_connector.py
+-rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/request_items.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/scan_data.py
+-rw-r--r--   0        0        0    11042 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/scan_items.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/scan_manager.py
+-rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/scan_report.py
+-rw-r--r--   0        0        0    16698 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/scans.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/scibec_validator.py
+-rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/serialization.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/service_config.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/signature_serializer.py
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/user_scripts_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/configs/__init__.py
+-rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/configs/demo_config.yaml
+-rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/configs/openapi_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/tests/__init__.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/tests/fixtures.py
+-rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/tests/test_config.yaml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/tests/test_service_config.yaml
+-rw-r--r--   0        0        0    22495 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/tests/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/utils/__init__.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/utils/import_utils.py
+-rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/utils/proxy.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/utils/rpc_utils.py
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/utils/scan_utils.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/bec_lib/utils/threading_utils.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/conftest.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_async_data.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_beamline_checks.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_bec_logger.py
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_bec_messages.py
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_bec_service.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_bl_conditions.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_callback_handler.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_channel_monitor.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_config_helper.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_core_utils.py
+-rw-r--r--   0        0        0    26550 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_dap_plugins.py
+-rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_device_manager.py
+-rw-r--r--   0        0        0    25863 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_devices.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_file_utils.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_import_utils.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_lmfit_serializer.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_observer.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_pdf_writer.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_plugin_helper.py
+-rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_redis_connector.py
+-rw-r--r--   0        0        0    22325 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_redis_connector_fakeredis.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_scan_context.py
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_scan_data.py
+-rw-r--r--   0        0        0    16743 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_scan_items.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_scan_manager.py
+-rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_scan_object.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_scan_report.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_scibec_validator.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_serializer.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_signature_serializer.py
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_user_scripts_mixin.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/tests/test_yaml_loader.py
+-rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/util_scripts/create_plugin_structure.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/util_scripts/init_config.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/gitignore
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/setup_device_server.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/post-commit
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/pre-commit
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/README.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/pyproject.toml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/bec_server_utils/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/bec_server_utils/launch.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/bec_server_utils/service_handler.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/data_processing/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/data_processing/dap_server.py
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/data_processing/dap_service.py
+-rw-r--r--   0        0        0     9729 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/data_processing/dap_service_manager.py
+-rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/data_processing/lmfit1d_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/data_processing/cli/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/data_processing/cli/launch.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/__init__.py
+-rw-r--r--   0        0        0    19037 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/device_server.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/rpc_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/cli/__init__.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/cli/launch.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/devices/__init__.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/devices/config_update_handler.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/devices/device_serializer.py
+-rw-r--r--   0        0        0    22629 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/devices/devicemanager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/tests/__init__.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/tests/utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer/__init__.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer/default_writer.py
+-rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer/file_writer.py
+-rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer/file_writer_manager.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer/merged_dicts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer/cli/__init__.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer/cli/launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer_plugins/__init__.py
+-rw-r--r--   0        0        0    22204 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_bundler/__init__.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_bundler/bec_emitter.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_bundler/emitter.py
+-rw-r--r--   0        0        0    16121 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_bundler/scan_bundler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_bundler/cli/__init__.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_bundler/cli/launch.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/__init__.py
+-rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/device_validation.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/errors.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/path_optimization.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_assembler.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_guard.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_manager.py
+-rw-r--r--   0        0        0    35246 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_queue.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_server.py
+-rw-r--r--   0        0        0    18915 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_stubs.py
+-rw-r--r--   0        0        0    35721 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_worker.py
+-rw-r--r--   0        0        0    51830 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/cli/__init__.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/cli/launch.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_plugins/__init__.py
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/tests/__init__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/tests/fixtures.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/tests/utils.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/repeated_timer.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/scihub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/cli/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/cli/launch.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/scibec/__init__.py
+-rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/scibec/config_handler.py
+-rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py
+-rw-r--r--   0        0        0    10735 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/scilog/__init__.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/scilog/scilog.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_bec_server_utils/test_main.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_data_processing/conftest.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_data_processing/test_dap_server.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/conftest.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/test_config_handler.py
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/test_device_serializer.py
+-rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/test_device_server.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_file_writer/conftest.py
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_file_writer/test_file_writer.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py
+-rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_bundler/conftest.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_bundler/test_emitter.py
+-rw-r--r--   0        0        0    25417 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/conftest.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_path_optimization.py
+-rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_scan_guard.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py
+-rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py
+-rw-r--r--   0        0        0    53947 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_scan_worker.py
+-rw-r--r--   0        0        0    87794 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_scans.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/conftest.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/test_repeated_timer.py
+-rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py
+-rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/test_scibec_connector.py
+-rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/test_scilog_connector.py
+-rwxr-xr-x   0        0        0     3629 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/bin/install_bec_dev.sh
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/ci/Dockerfile.run_pytest
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/ci/Dockerfile.run_server
+-rwxr-xr-x   0        0        0      347 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/ci/build_python_services.sh
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/ci/docker-compose.yaml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/ci/functionalAccounts.json
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/ci/semantic_release.toml
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/ci/test_config.yaml
+-rw-r--r--   0        0        0   307212 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/architecture/BEC.drawio
+-rw-r--r--   0        0        0   124683 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/architecture/BEC_config_db.drawio
+-rw-r--r--   0        0        0    11580 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/architecture/BEC_config_db.svg
+-rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/architecture/bec_architecture.png
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/Makefile
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/conf.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/make.bat
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/requirements.txt
+-rw-r--r--   0        0        0    41260 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/_static/bec.png
+-rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/_static/custom.css
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/_static/switcher.json
+-rw-r--r--   0        0        0  4672990 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/_static/gif/bec_plotter.gif
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/api_reference/api_reference.md
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/api_reference/modules.rst
+-rw-r--r--   0        0        0   310535 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/BEC_context_user_centric.png
+-rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/bec_architecture.png
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/bec_device_structure.drawio
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/bec_device_structure.png
+-rw-r--r--   0        0        0   185658 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/bec_widgets_glance.png
+-rw-r--r--   0        0        0    17460 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/gauss_scatter_plot.png
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/index_api.svg
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/index_contribute.svg
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/index_getting_started.svg
+-rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/index_user_guide.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/portrait_48dp.svg
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/precision_manufacturing_48dp.svg
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/rocket_launch_48dp.svg
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/simulation_context_diagram.drawio
+-rw-r--r--   0        0        0    69323 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/simulation_context_diagram.png
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/tab-complete-devices.png
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/timeline_48dp.svg
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/toc_48dp.svg
+-rw-r--r--   0        0        0    37244 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/vscode_debug_button.png
+-rw-r--r--   0        0        0   374770 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/vscode_with_annotations.drawio
+-rw-r--r--   0        0        0   711275 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/vscode_with_annotations.png
+-rw-r--r--   0        0        0    96330 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/assets/wm-devices.png
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/developer.md
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/glossary.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/data_acess/data_access.md
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/data_acess/event_data.md
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/devices/bec_sim.md
+-rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/devices/device_configuration.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/devices/devices.md
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/devices/external_sources.md
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/devices/ophyd.md
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/architecture.md
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/bec_config.md
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/bec_plugins.md
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/contributing.md
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/getting_started.md
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/install_developer_env.md
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/logs.md
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/tests.md
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/vscode.md
+-rw-r--r--   0        0        0    16567 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/scans/scans.md
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/user_interfaces/bec_cli.md
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/user_interfaces/bec_gui.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/developer/user_interfaces/user_interfaces.md
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/introduction/introduction.md
+-rw-r--r--   0        0        0    15455 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/user/command_line_interface.md
+-rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/user/data_access_and_plotting.md
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/user/devices.md
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/user/graphical_user_interface.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/user/installation.md
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/docs/source/user/user.md
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/pytest_bec_e2e/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/pytest_bec_e2e/pytest_bec_e2e/__init__.py
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/__init__.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/ophyd_patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/configs/__init__.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/configs/ophyd_devices_simulation.yaml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/configs/ophyd_simulation.yaml
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/configs/sls_devices.yaml
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/devices/SpmBase.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/devices/XbpmBase.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/devices/__init__.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/devices/device_list.md
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/devices/epics_motor_ex.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/devices/mono_dccm.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/devices/slits.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/devices/sls_detector.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/devices/sls_devices.py
+-rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/devices/specMotors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/interfaces/base_classes/__init__.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py
+-rw-r--r--   0        0        0    18126 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/interfaces/base_classes/psi_detector_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/interfaces/protocols/bec_protocols.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/sim/__init__.py
+-rw-r--r--   0        0        0    27852 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/sim/sim.py
+-rw-r--r--   0        0        0    27990 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/sim/sim_data.py
+-rw-r--r--   0        0        0    12071 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/sim/sim_frameworks.py
+-rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/sim/sim_signals.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/sim/sim_test_devices.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/sim/sim_utils.py
+-rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/sim/sim_xtreme.py
+-rw-r--r--   0        0        0   671622 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt
+-rw-r--r--   0        0        0   669534 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt
+-rw-r--r--   0        0        0   670586 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt
+-rw-r--r--   0        0        0   668300 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/utils/__init__.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/utils/bec_device_base.py
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/utils/bec_scaninfo_mixin.py
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/utils/bec_utils.py
+-rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/utils/controller.py
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/utils/dynamic_pseudo.py
+-rw-r--r--   0        0        0     7309 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/utils/socket.py
+-rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/ophyd_devices/utils/static_device_test.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/tests/test_base_classes.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/tests/test_controller.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/tests/test_dynamic_pseudo.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/tests/test_ophyd_status_obj.py
+-rw-r--r--   0        0        0    12977 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/tests/test_simulation.py
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/tests/test_socket.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/tests/test_static_device_test.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ophyd_devices-1.2.0/PKG-INFO
```

### Comparing `ophyd_devices-1.1.0/.gitlab-ci.yml` & `ophyd_devices-1.2.0/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     - if: $CI_PIPELINE_SOURCE == "parent_pipeline"
     - if: $CI_COMMIT_BRANCH && $CI_OPEN_MERGE_REQUESTS
       when: never
     - if: $CI_COMMIT_BRANCH
   auto_cancel:
     on_new_commit: interruptible
 
-
 include:
   - template: Security/Secret-Detection.gitlab-ci.yml
   - project: "bec/awi_utils"
     file: "/templates/check-packages-job.yml"
     inputs:
       stage: test
       path: "."
@@ -40,15 +39,15 @@
     inputs:
       target: $CI_PROJECT_NAME
       token: $CI_UPDATES
 
 #commands to run in the Docker container before starting each job.
 before_script:
   - if [[ "$CI_PROJECT_PATH" != "bec/ophyd_devices" ]]; then
-    echo -e "\033[35;1m Using branch $CHILD_PIPELINE_BRANCH of Ophyd Devices \033[0;m"; 
+    echo -e "\033[35;1m Using branch $CHILD_PIPELINE_BRANCH of Ophyd Devices \033[0;m";
     test -d ophyd_devices || git clone --branch $CHILD_PIPELINE_BRANCH https://gitlab.psi.ch/bec/ophyd_devices.git; cd ophyd_devices;
     fi
   - pip install -e .[dev]
   - git clone --branch $BEC_CORE_BRANCH https://gitlab.psi.ch/bec/bec.git
   - pip install -e ./bec/bec_lib[dev]
   - pip install -e ./bec/bec_server[dev]
 
@@ -155,15 +154,15 @@
       - ./config_tests
     when: on_failure
     expire_in: "30 days"
   interruptible: true
 
 tests-3.11:
   stage: AdditionalTests
-  needs: 
+  needs:
     - job: "formatter"
       optional: true
     - job: "pylint"
       optional: true
   image: $CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX/python:3.11
   script:
     - pytest -v --random-order ./tests
@@ -176,33 +175,34 @@
   image: $CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX/python:3.12
   allow_failure: true
 
 trigger_bec:
   trigger:
     project: bec/bec
     strategy: depend
+    branch: $BEC_CORE_BRANCH
   variables:
     OPHYD_DEVICES_BRANCH: $CI_COMMIT_REF_NAME
   rules:
     - if: '$CI_MERGE_REQUEST_TARGET_BRANCH_NAME == "main" && $CI_PROJECT_PATH == "bec/ophyd_devices"'
   interruptible: true
 
 trigger:
   parallel:
     matrix:
       - CHILD_PROJECT: csaxs_bec
-        CHILD_PIPELINE_BRANCH: $CSAXS_BEC_BRANCH     
+        CHILD_PIPELINE_BRANCH: $CSAXS_BEC_BRANCH
       - CHILD_PROJECT: debye_bec
-        CHILD_PIPELINE_BRANCH: $DEBYE_BEC_BRANCH           
+        CHILD_PIPELINE_BRANCH: $DEBYE_BEC_BRANCH
       - CHILD_PROJECT: pxiii_bec
         CHILD_PIPELINE_BRANCH: $PXIII_BEC_BRANCH
       - CHILD_PROJECT: tomcat_bec
         CHILD_PIPELINE_BRANCH: $TOMCAT_BEC_BRANCH
       - CHILD_PROJECT: xtreme_bec
-        CHILD_PIPELINE_BRANCH: $XTREME_BEC_BRANCH             
+        CHILD_PIPELINE_BRANCH: $XTREME_BEC_BRANCH
 
   needs: []
   trigger:
     strategy: depend
     include:
       - project: bec/$CHILD_PROJECT
         ref: $CHILD_PIPELINE_BRANCH
@@ -232,15 +232,15 @@
     - git fetch --tags
     - git tag
 
     # build and publish package
     - pip install python-semantic-release==9.* wheel build twine
     - export GL_TOKEN=$CI_UPDATES
     - semantic-release -vv version
-    
+
     # check if any artifacts were created
     - if [ ! -d dist ]; then echo No release will be made; exit 0; fi
     - twine upload dist/* -u __token__ -p $CI_PYPI_TOKEN --skip-existing
     - semantic-release publish
 
   allow_failure: false
   rules:
```

### Comparing `ophyd_devices-1.1.0/CHANGELOG.md` & `ophyd_devices-1.2.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,36 @@
 # CHANGELOG
 
 
 
+## v1.2.0 (2024-05-29)
+
+### Ci
+
+* ci: fix bec_core_branch triggering in ci file ([`3cab569`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/3cab5690db3fbabffecc179cbaadf6878f0ab2f1))
+
+### Documentation
+
+* docs: Update device list ([`08dfc9e`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/08dfc9e314a1b498ec2fc1f9056234fe732d6428))
+
+* docs: Update device list ([`106233f`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/106233f8d951794e261b08a11b20db6cbf4ef63a))
+
+* docs: Update device list ([`9c93916`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/9c9391610845bc1b21e342e7c3b34b8db978a038))
+
+* docs: Update device list ([`018fdac`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/018fdaced4120557ea64501c107c027e362c93fb))
+
+### Feature
+
+* feat: add option to save Camera data to disk, closes #66 ([`60b2e75`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/60b2e756550196fb5c07bb91abb4c1ae5b815c6c))
+
+### Test
+
+* test: add tests ([`af908fa`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/af908fa210914519de9a713ed2ef3e2e0c743742))
+
+
 ## v1.1.0 (2024-05-27)
 
 ### Feature
 
 * feat: refactor psi_detector_base class, add tests ([`a0ac8c9`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/a0ac8c9ad701f52429f393a134fd0705583eddb1))
 
 ### Refactor
@@ -126,35 +151,7 @@
 
 
 ## v0.33.3 (2024-04-24)
 
 ### Ci
 
 * ci: removed allow_failure from config check ([`d34b396`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/d34b39669c4faf2d1c5518a632239303a48c2fd6))
-
-### Fix
-
-* fix: updated device configs to new import schema ([`5725fc3`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/5725fc36c7aff052fc704782a99bd04cfb13c112))
-
-
-## v0.33.2 (2024-04-22)
-
-### Fix
-
-* fix(pyproject.toml): add bec-server to dev dependencies; closes #62 ([`9353b46`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/9353b46be804de967810f0d9370d230dfae5c92b))
-
-
-## v0.33.1 (2024-04-20)
-
-### Fix
-
-* fix: fix pyproject.toml ([`6081eb4`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/6081eb4ba54b2a6a2072f638af06c6f1cf264b69))
-
-
-## v0.33.0 (2024-04-19)
-
-### Feature
-
-* feat: move csaxs devices to plugin structure, fix imports and tests ([`74f6fa7`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/74f6fa7ffdf339399504e15f27564e3f0e43db56))
-
-
-## v0.32.0 (2024-04-19)
```

### Comparing `ophyd_devices-1.1.0/README.md` & `ophyd_devices-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/.gitlab/issue_templates/documentation_update_template.md` & `ophyd_devices-1.2.0/.gitlab/issue_templates/documentation_update_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/.gitlab/issue_templates/feature_request_template.md` & `ophyd_devices-1.2.0/.gitlab/issue_templates/feature_request_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/.gitlab/merge_request_templates/default.md` & `ophyd_devices-1.2.0/.gitlab/merge_request_templates/default.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/.gitignore` & `ophyd_devices-1.2.0/bec/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/.gitlab-ci.yml` & `ophyd_devices-1.2.0/bec/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/.pylintrc` & `ophyd_devices-1.2.0/bec/.pylintrc`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/.readthedocs.yaml` & `ophyd_devices-1.2.0/bec/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/CHANGELOG.md` & `ophyd_devices-1.2.0/bec/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,59 @@
 # CHANGELOG
 
 
 
+## v2.12.5 (2024-05-28)
+
+### Fix
+
+* fix: remove deprecated arg speed from deviceconfig ([`67f0bea`](https://gitlab.psi.ch/bec/bec/-/commit/67f0beac75bbeecf69768662e373b96a0839f122))
+
+
+## v2.12.4 (2024-05-28)
+
+### Ci
+
+* ci: added development pages ([`4a9f4f8`](https://gitlab.psi.ch/bec/bec/-/commit/4a9f4f83fae16f40df679cddc5bf816e3b77deff))
+
+### Documentation
+
+* docs: fixed broken links ([`5dfcbe6`](https://gitlab.psi.ch/bec/bec/-/commit/5dfcbe6d132dd199be9f42980ed254efb2dc0e82))
+
+* docs: added reference to gitlab issues ([`7277ac3`](https://gitlab.psi.ch/bec/bec/-/commit/7277ac3c40f86ff465f7af69a060fb9d5f2d4acc))
+
+* docs: fixed api reference; added reference to scanbase ([`121e592`](https://gitlab.psi.ch/bec/bec/-/commit/121e5922eb3806eff88f49b5378b1f12056be132))
+
+* docs: cleanup ([`7254755`](https://gitlab.psi.ch/bec/bec/-/commit/7254755aacda0f9c50b09237a59cd3584fb48e74))
+
+* docs: added reference to user docs for loading new device configs ([`fd29dfb`](https://gitlab.psi.ch/bec/bec/-/commit/fd29dfb5f7d63d864e08adae1b5128f0f0fed14a))
+
+* docs: added linkify ([`3a363f5`](https://gitlab.psi.ch/bec/bec/-/commit/3a363f5f52b644bc2542913cf4e9acf224ef69f9))
+
+* docs: improvements for the dev docs ([`e5a98d7`](https://gitlab.psi.ch/bec/bec/-/commit/e5a98d718d06004819b32db1fabf77e634bdefd0))
+
+* docs: restructured developer docs ([`7fd66f8`](https://gitlab.psi.ch/bec/bec/-/commit/7fd66f895905cb3e46ee90b98bfac8985837d6ca))
+
+* docs: added docs for developing scans ([`5f44521`](https://gitlab.psi.ch/bec/bec/-/commit/5f4452110519404573484d2c6a95d8a46c325a1f))
+
+* docs: fixed dependency for building sphinx ([`9cbde72`](https://gitlab.psi.ch/bec/bec/-/commit/9cbde72505723b5e4da94eeab4c8313e29c295c5))
+
+* docs: fixed api reference ([`29862dc`](https://gitlab.psi.ch/bec/bec/-/commit/29862dca51873d4c22db6a693014ecf7addb4447))
+
+### Fix
+
+* fix: create readme for tests_dap_services ([`104c847`](https://gitlab.psi.ch/bec/bec/-/commit/104c847b55427c3ac78afb3af9e71154deff7d9e))
+
+### Refactor
+
+* refactor: renamed move_and_wait to move_scan_motors_and_wait ([`eaa8bd8`](https://gitlab.psi.ch/bec/bec/-/commit/eaa8bd8e67aa75a00d6a5b3e2494ed9828e7d6cf))
+
+* refactor: deprecated scan report hint ([`0382ac5`](https://gitlab.psi.ch/bec/bec/-/commit/0382ac52dd9d68e6871866311416632ee39ed232))
+
+
 ## v2.12.3 (2024-05-21)
 
 ### Fix
 
 * fix: renamed table_wait to scan_progress ([`855f9a8`](https://gitlab.psi.ch/bec/bec/-/commit/855f9a8412e9c0d8b02d131ece533b4d85882b36))
 
 * fix: renamed scan_progress to device_progress ([`d344e85`](https://gitlab.psi.ch/bec/bec/-/commit/d344e8513781f29a1390adc92826f23d1702964b))
@@ -102,71 +150,10 @@
 ### Fix
 
 * fix: upgraded to ophyd_devices v1 ([`3077dbe`](https://gitlab.psi.ch/bec/bec/-/commit/3077dbe22ae50e6aae317c72022df6ea88b14cce))
 
 
 ## v2.10.2 (2024-05-08)
 
-### Ci
-
-* ci: added ds pipeline for tomcat ([`55d210c`](https://gitlab.psi.ch/bec/bec/-/commit/55d210c7ae06ea509328510e6aec636caf009cfd))
-
 ### Fix
 
 * fix(RedisConnector): add &#39;from_start&#39; support in &#39;register&#39; for streams ([`f059bf9`](https://gitlab.psi.ch/bec/bec/-/commit/f059bf9318038404ebbcc82b5abf5cd148486021))
-
-### Refactor
-
-* refactor(bec_startup): default gui is BECDockArea (gui variable) with fig in first dock ([`7dc2426`](https://gitlab.psi.ch/bec/bec/-/commit/7dc242689f0966d692d3aeb77ca7689ea8709680))
-
-
-## v2.10.1 (2024-05-07)
-
-### Build
-
-* build: fixed dependency range ([`c10ac5e`](https://gitlab.psi.ch/bec/bec/-/commit/c10ac5e78887844e46b965a707351d663ac4bcf8))
-
-### Ci
-
-* ci: moved from multi-project pipelines to parent-child pipelines ([`9eff5ca`](https://gitlab.psi.ch/bec/bec/-/commit/9eff5ca3580c3536e1edff5ade264dc6fc3f6f6e))
-
-* ci: changed repo name to bec_widgets in downstream tests ([`698029b`](https://gitlab.psi.ch/bec/bec/-/commit/698029b637b1c84c5b1e836d8c6fbc8c8c7e3e0e))
-
-### Fix
-
-* fix: upgraded plugin setup tools ([`ea38501`](https://gitlab.psi.ch/bec/bec/-/commit/ea38501ea7ae4a62d6525b00608484ff1be540a1))
-
-
-## v2.10.0 (2024-05-03)
-
-### Feature
-
-* feat: add client message handler to send info messages from services to clients; closes 258 ([`c0a0e3e`](https://gitlab.psi.ch/bec/bec/-/commit/c0a0e3e44299b350790687db436771c6b456567a))
-
-
-## v2.9.6 (2024-05-02)
-
-### Fix
-
-* fix(scihub): fixed scibec connector for new api ([`fc94c82`](https://gitlab.psi.ch/bec/bec/-/commit/fc94c827e40f12293c59b139ccd455df8b8b4d70))
-
-
-## v2.9.5 (2024-05-02)
-
-### Fix
-
-* fix: use the right redis fixture in &#34;bec_servers&#34; fixture to prevent multiple redis processes to be started ([`51d65e2`](https://gitlab.psi.ch/bec/bec/-/commit/51d65e2e9547765c34cc4a0a43f1adca90e7e5c3))
-
-* fix: do not try to populate `user_global_ns` if IPython interpreter is not there ([`cf07feb`](https://gitlab.psi.ch/bec/bec/-/commit/cf07febc5cf0fdadec0e9658c2469ce1adb1a369))
-
-### Test
-
-* test: added more tests for scan queue ([`b664b92`](https://gitlab.psi.ch/bec/bec/-/commit/b664b92aae917d2067bfca48a60eeaf44ced0c98))
-
-
-## v2.9.4 (2024-05-01)
-
-### Refactor
-
-* refactor: added isort params to pyproject ([`0a1beae`](https://gitlab.psi.ch/bec/bec/-/commit/0a1beae06ae128d9817272644d2f38ca761756ab))
-
-* refactor(bec_lib): cleanup ([`6bf0998`](https://gitlab.psi.ch/bec/bec/-/commit/6bf0998c71387307ad8d842931488ec2aea566a8))
```

### Comparing `ophyd_devices-1.1.0/bec/LICENSE` & `ophyd_devices-1.2.0/bec/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/README.md` & `ophyd_devices-1.2.0/bec/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/.gitlab/issue_templates/documentation_update_template.md` & `ophyd_devices-1.2.0/bec/.gitlab/issue_templates/documentation_update_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/.gitlab/issue_templates/feature_request_template.md` & `ophyd_devices-1.2.0/bec/.gitlab/issue_templates/feature_request_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/.gitlab/merge_request_templates/default.md` & `ophyd_devices-1.2.0/bec/.gitlab/merge_request_templates/default.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/demo.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/demo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/pyproject.toml` & `ophyd_devices-1.2.0/bec/bec_ipython_client/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec_ipython_client"
-version = "2.12.3"
+version = "2.12.5"
 description = "BEC IPython client"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/bec_magics.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/bec_startup.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/bec_startup.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/main.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/main.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/prettytable.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/progressbar.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/progressbar.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/signals.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/signals.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml` & `ophyd_devices-1.2.0/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_bec_client.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/tests/client_tests/test_bec_client.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_device_progress.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/tests/client_tests/test_device_progress.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_live_table.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/tests/client_tests/test_live_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_move_callback.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/tests/client_tests/test_move_callback.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py` & `ophyd_devices-1.2.0/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,14 @@
                     "readOnly": False,
                 },
                 "eyefoc": {
                     "deviceClass": "ophyd_devices.SimPositioner",
                     "deviceConfig": {
                         "delay": 1,
                         "limits": [-50, 50],
-                        "speed": 100,
                         "tolerance": 0.01,
                         "update_frequency": 400,
                     },
                     "deviceTags": ["user motors"],
                     "enabled": True,
                     "readOnly": False,
                 },
@@ -177,15 +176,14 @@
                     "readOnly": False,
                 },
                 "eyefoc": {
                     "deviceClass": "ophyd_devices.SimPositioner",
                     "deviceConfig": {
                         "delay": 1,
                         "limits": [-50, 50],
-                        "speed": 100,
                         "tolerance": 0.01,
                         "update_frequency": 400,
                     },
                     "readoutPriority": "baseline",
                     "deviceTags": ["user motors"],
                     "enabled": True,
                     "readOnly": False,
```

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/README.md` & `ophyd_devices-1.2.0/bec/bec_lib/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/pyproject.toml` & `ophyd_devices-1.2.0/bec/bec_lib/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec_lib"
-version = "2.12.3"
+version = "2.12.5"
 description = "BEC library"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/alarm_handler.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/async_data.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/async_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bec_service.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/bec_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bec_yaml_loader.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/bec_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bl_checks.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/bl_checks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bl_conditions.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/bl_conditions.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/callback_handler.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/channel_monitor.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/channel_monitor.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/client.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/client.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/config_helper.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/config_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/connector.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/dap_plugin_objects.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/dap_plugin_objects.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/dap_plugins.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/dap_plugins.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/device.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/device.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/devicemanager.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/devicemanager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/endpoints.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/endpoints.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/file_utils.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/file_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/lmfit_serializer.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/logbook_connector.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/logger.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/logger.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/messages.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/messages.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/numpy_encoder.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/observer.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/observer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/pdf_writer.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/plugin_helper.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/plugin_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/queue_items.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/redis_connector.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/redis_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/request_items.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/request_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_data.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/scan_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_items.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/scan_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_manager.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_report.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/scan_report.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scans.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scibec_validator.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/serialization.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/serialization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/service_config.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/service_config.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/signature_serializer.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/signature_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/user_scripts_mixin.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/configs/demo_config.yaml` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/configs/demo_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/configs/openapi_schema.json` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/fixtures.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/test_config.yaml` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/tests/test_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/utils.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/import_utils.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/proxy.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/rpc_utils.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/utils/rpc_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/scan_utils.py` & `ophyd_devices-1.2.0/bec/bec_lib/bec_lib/utils/scan_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_async_data.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_async_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_beamline_checks.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_beamline_checks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_bec_logger.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_bec_logger.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_bec_messages.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_bec_messages.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_bec_service.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_bec_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_bl_conditions.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_bl_conditions.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_callback_handler.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_callback_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_channel_monitor.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_channel_monitor.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_config_helper.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_config_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_core_utils.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_core_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_dap_plugins.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_dap_plugins.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_device_manager.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_devices.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_file_utils.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_lmfit_serializer.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_observer.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_plugin_helper.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_plugin_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_redis_connector.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_redis_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_redis_connector_fakeredis.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_redis_connector_fakeredis.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_context.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_scan_context.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_data.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_scan_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_items.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_scan_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_manager.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_scan_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_object.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_scan_object.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_report.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_scan_report.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_serializer.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_signature_serializer.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_signature_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_user_scripts_mixin.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/tests/test_yaml_loader.py` & `ophyd_devices-1.2.0/bec/bec_lib/tests/test_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/create_plugin_structure.py` & `ophyd_devices-1.2.0/bec/bec_lib/util_scripts/create_plugin_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         with open(os.path.join(self.target_dir, ".gitlab-ci.yml"), "w", encoding="utf-8") as f:
             yaml.dump(out, f)
 
     def add_tests(self):
         self.create_dir("tests/tests_bec_ipython_client")
         self.copy_tests_readme("tests/tests_bec_ipython_client")
         self.create_dir("tests/tests_dap_services")
-        self.copy_tests_readme("tests/tests_services")
+        self.copy_tests_readme("tests/tests_dap_services")
         self.create_dir("tests/tests_bec_widgets")
         self.copy_tests_readme("tests/tests_bec_widgets")
         self.create_dir("tests/tests_devices")
         self.copy_tests_readme("tests/tests_devices")
         self.create_dir("tests/tests_scans")
         self.copy_tests_readme("tests/tests_scans")
         self.create_dir("tests/tests_file_writer")
```

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/init_config.py` & `ophyd_devices-1.2.0/bec/bec_lib/util_scripts/init_config.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md` & `ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/gitignore` & `ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py` & `ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py` & `ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml` & `ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py` & `ophyd_devices-1.2.0/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/pyproject.toml` & `ophyd_devices-1.2.0/bec/bec_server/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec-server"
-version = "2.12.3"
+version = "2.12.5"
 description = "BEC server"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/launch.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/bec_server_utils/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/service_handler.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/bec_server_utils/service_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/dap_server.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/data_processing/dap_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/dap_service.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/data_processing/dap_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/dap_service_manager.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/data_processing/dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/lmfit1d_service.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/data_processing/lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/cli/launch.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/data_processing/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/device_server.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/device_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/rpc_mixin.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/cli/launch.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/config_update_handler.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/devices/config_update_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/device_serializer.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/devicemanager.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/devices/devicemanager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/tests/utils.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/device_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/default_writer.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer/default_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/file_writer.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer/file_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/file_writer_manager.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer/file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/merged_dicts.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer/merged_dicts.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/cli/launch.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/bec_emitter.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_bundler/bec_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/emitter.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_bundler/emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/scan_bundler.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_bundler/scan_bundler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/cli/launch.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_bundler/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/device_validation.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/device_validation.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/path_optimization.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_assembler.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_assembler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_guard.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_guard.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_manager.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_queue.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_queue.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_server.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_stubs.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_stubs.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_worker.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_worker.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scans.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/cli/launch.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/tests/utils.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scan_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/repeated_timer.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/repeated_timer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scihub.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/cli/launch.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/config_handler.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scilog/scilog.py` & `ophyd_devices-1.2.0/bec/bec_server/bec_server/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_bec_server_utils/test_main.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_bec_server_utils/test_main.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/conftest.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_config_handler.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/test_config_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_serializer.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/test_device_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_server.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/test_device_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/test_file_writer.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_file_writer/test_file_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/conftest.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_bundler/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_emitter.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_bundler/test_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_path_optimization.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_path_optimization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_guard.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_scan_guard.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_worker.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_scan_worker.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scans.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scan_server/test_scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/conftest.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_repeated_timer.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/test_repeated_timer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scibec_connector.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/test_scibec_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scilog_connector.py` & `ophyd_devices-1.2.0/bec/bec_server/tests/tests_scihub/test_scilog_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/bin/install_bec_dev.sh` & `ophyd_devices-1.2.0/bec/bin/install_bec_dev.sh`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/ci/Dockerfile.run_pytest` & `ophyd_devices-1.2.0/bec/ci/Dockerfile.run_pytest`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/ci/Dockerfile.run_server` & `ophyd_devices-1.2.0/bec/ci/Dockerfile.run_server`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/ci/docker-compose.yaml` & `ophyd_devices-1.2.0/bec/ci/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/ci/semantic_release.toml` & `ophyd_devices-1.2.0/bec/ci/semantic_release.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/architecture/BEC.drawio` & `ophyd_devices-1.2.0/bec/docs/architecture/BEC.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/architecture/BEC_config_db.drawio` & `ophyd_devices-1.2.0/bec/docs/architecture/BEC_config_db.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/architecture/BEC_config_db.svg` & `ophyd_devices-1.2.0/bec/docs/architecture/BEC_config_db.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/architecture/bec_architecture.png` & `ophyd_devices-1.2.0/bec/docs/architecture/bec_architecture.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/Makefile` & `ophyd_devices-1.2.0/bec/docs/source/Makefile`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/conf.py` & `ophyd_devices-1.2.0/bec/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/index.md` & `ophyd_devices-1.2.0/bec/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/make.bat` & `ophyd_devices-1.2.0/bec/docs/source/make.bat`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/_static/bec.png` & `ophyd_devices-1.2.0/bec/docs/source/_static/bec.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/_static/custom.css` & `ophyd_devices-1.2.0/bec/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/_static/gif/bec_plotter.gif` & `ophyd_devices-1.2.0/bec/docs/source/_static/gif/bec_plotter.gif`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/_templates/custom-class-template.rst` & `ophyd_devices-1.2.0/bec/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/_templates/custom-module-template.rst` & `ophyd_devices-1.2.0/bec/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/BEC_context_user_centric.png` & `ophyd_devices-1.2.0/bec/docs/source/assets/BEC_context_user_centric.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/bec_architecture.png` & `ophyd_devices-1.2.0/bec/docs/source/assets/bec_architecture.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/bec_device_structure.drawio` & `ophyd_devices-1.2.0/bec/docs/source/assets/bec_device_structure.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/bec_device_structure.png` & `ophyd_devices-1.2.0/bec/docs/source/assets/bec_device_structure.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/bec_widgets_glance.png` & `ophyd_devices-1.2.0/bec/docs/source/assets/bec_widgets_glance.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/gauss_scatter_plot.png` & `ophyd_devices-1.2.0/bec/docs/source/assets/gauss_scatter_plot.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/index_api.svg` & `ophyd_devices-1.2.0/bec/docs/source/assets/index_api.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/index_contribute.svg` & `ophyd_devices-1.2.0/bec/docs/source/assets/index_contribute.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/index_getting_started.svg` & `ophyd_devices-1.2.0/bec/docs/source/assets/index_getting_started.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/index_user_guide.svg` & `ophyd_devices-1.2.0/bec/docs/source/assets/index_user_guide.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/precision_manufacturing_48dp.svg` & `ophyd_devices-1.2.0/bec/docs/source/assets/precision_manufacturing_48dp.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/rocket_launch_48dp.svg` & `ophyd_devices-1.2.0/bec/docs/source/assets/rocket_launch_48dp.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/simulation_context_diagram.drawio` & `ophyd_devices-1.2.0/bec/docs/source/assets/simulation_context_diagram.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/simulation_context_diagram.png` & `ophyd_devices-1.2.0/bec/docs/source/assets/simulation_context_diagram.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/tab-complete-devices.png` & `ophyd_devices-1.2.0/bec/docs/source/assets/tab-complete-devices.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/timeline_48dp.svg` & `ophyd_devices-1.2.0/bec/docs/source/assets/timeline_48dp.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/vscode_debug_button.png` & `ophyd_devices-1.2.0/bec/docs/source/assets/vscode_debug_button.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/vscode_with_annotations.drawio` & `ophyd_devices-1.2.0/bec/docs/source/assets/vscode_with_annotations.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/vscode_with_annotations.png` & `ophyd_devices-1.2.0/bec/docs/source/assets/vscode_with_annotations.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/assets/wm-devices.png` & `ophyd_devices-1.2.0/bec/docs/source/assets/wm-devices.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/developer.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/developer.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/glossary.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/glossary.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/devices/bec_sim.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/devices/bec_sim.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/devices/device_configuration.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/devices/device_configuration.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/devices/devices.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/devices/devices.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/devices/external_sources.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/devices/external_sources.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/devices/ophyd.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/devices/ophyd.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/architecture.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/architecture.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/bec_plugins.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/bec_plugins.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/contributing.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/contributing.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/install_developer_env.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/install_developer_env.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/logs.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/logs.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/tests.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/tests.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/vscode.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/getting_started/vscode.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/scans/scans.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/scans/scans.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/developer/user_interfaces/bec_gui.md` & `ophyd_devices-1.2.0/bec/docs/source/developer/user_interfaces/bec_gui.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/introduction/introduction.md` & `ophyd_devices-1.2.0/bec/docs/source/introduction/introduction.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/user/command_line_interface.md` & `ophyd_devices-1.2.0/bec/docs/source/user/command_line_interface.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/user/data_access_and_plotting.md` & `ophyd_devices-1.2.0/bec/docs/source/user/data_access_and_plotting.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/user/devices.md` & `ophyd_devices-1.2.0/bec/docs/source/user/devices.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/user/graphical_user_interface.md` & `ophyd_devices-1.2.0/bec/docs/source/user/graphical_user_interface.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/user/installation.md` & `ophyd_devices-1.2.0/bec/docs/source/user/installation.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/docs/source/user/user.md` & `ophyd_devices-1.2.0/bec/docs/source/user/user.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/bec/pytest_bec_e2e/pyproject.toml` & `ophyd_devices-1.2.0/bec/pytest_bec_e2e/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytest-bec-e2e"
-version = "2.12.3"
+version = "2.12.5"
 description = "BEC pytest plugin for end-to-end tests"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.1.0/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py` & `ophyd_devices-1.2.0/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/__init__.py` & `ophyd_devices-1.2.0/ophyd_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/ophyd_patch.py` & `ophyd_devices-1.2.0/ophyd_devices/ophyd_patch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/configs/ophyd_devices_simulation.yaml` & `ophyd_devices-1.2.0/ophyd_devices/configs/ophyd_devices_simulation.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/configs/ophyd_simulation.yaml` & `ophyd_devices-1.2.0/ophyd_devices/configs/ophyd_simulation.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/devices/SpmBase.py` & `ophyd_devices-1.2.0/ophyd_devices/devices/SpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/devices/XbpmBase.py` & `ophyd_devices-1.2.0/ophyd_devices/devices/XbpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/devices/__init__.py` & `ophyd_devices-1.2.0/ophyd_devices/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/devices/device_list.md` & `ophyd_devices-1.2.0/ophyd_devices/devices/device_list.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/devices/epics_motor_ex.py` & `ophyd_devices-1.2.0/ophyd_devices/devices/epics_motor_ex.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/devices/mono_dccm.py` & `ophyd_devices-1.2.0/ophyd_devices/devices/mono_dccm.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/devices/slits.py` & `ophyd_devices-1.2.0/ophyd_devices/devices/slits.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/devices/sls_detector.py` & `ophyd_devices-1.2.0/ophyd_devices/devices/sls_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/devices/sls_devices.py` & `ophyd_devices-1.2.0/ophyd_devices/devices/sls_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/devices/specMotors.py` & `ophyd_devices-1.2.0/ophyd_devices/devices/specMotors.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py` & `ophyd_devices-1.2.0/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py` & `ophyd_devices-1.2.0/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/interfaces/base_classes/psi_detector_base.py` & `ophyd_devices-1.2.0/ophyd_devices/interfaces/base_classes/psi_detector_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,24 +73,26 @@
         This must also set self.parent.stopped to True.
 
         This step should include stopping the detector and backend service.
         """
 
     def on_trigger(self) -> None:
         """
-        Specify actions to be executed upon receiving trigger signal
+        Specify actions to be executed upon receiving trigger signal.
+        Return a DeviceStatus object or None
         """
 
     def on_pre_scan(self) -> None:
         """
         Specify actions to be executed right before a scan starts.
 
         Only use if needed, and it is recommended to keep this function as short/fast as possible.
         """
 
+    # TODO add configurable file_path instead of hardcoding self.parent.filepath
     def publish_file_location(
         self, done: bool = False, successful: bool = None, metadata: dict = {}
     ) -> None:
         """
         Publish the filepath to REDIS.
 
         We publish two events here:
```

### Comparing `ophyd_devices-1.1.0/ophyd_devices/interfaces/protocols/bec_protocols.py` & `ophyd_devices-1.2.0/ophyd_devices/interfaces/protocols/bec_protocols.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/sim/sim.py` & `ophyd_devices-1.2.0/ophyd_devices/sim/sim.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,27 @@
 from ophyd import DynamicDeviceComponent as Dcpt
 from ophyd import Kind, PositionerBase
 from ophyd.flyers import FlyerInterface
 from ophyd.sim import SynSignal
 from ophyd.status import StatusBase
 from ophyd.utils import LimitError
 
+from ophyd_devices.interfaces.base_classes.psi_detector_base import (
+    CustomDetectorMixin,
+    PSIDetectorBase,
+)
 from ophyd_devices.sim.sim_data import (
     SimulatedDataCamera,
     SimulatedDataMonitor,
     SimulatedDataWaveform,
     SimulatedPositioner,
 )
 from ophyd_devices.sim.sim_signals import ReadOnlySignal, SetableSignal
 from ophyd_devices.sim.sim_test_devices import DummyController
+from ophyd_devices.sim.sim_utils import H5Writer
 from ophyd_devices.utils.bec_scaninfo_mixin import BecScaninfoMixin
 
 logger = bec_logger.logger
 
 
 class DeviceStop(Exception):
     pass
@@ -71,28 +76,87 @@
         parent=None,
         kind=None,
         device_manager=None,
         **kwargs,
     ):
         self.precision = precision
         self.init_sim_params = sim_init
-        self.sim = self.sim_cls(parent=self, device_manager=device_manager, **kwargs)
+        self.device_manager = device_manager
+        self.sim = self.sim_cls(parent=self, **kwargs)
         self._registered_proxies = {}
 
         super().__init__(name=name, parent=parent, kind=kind, **kwargs)
         self.sim.sim_state[self.name] = self.sim.sim_state.pop(self.readback.name, None)
         self.readback.name = self.name
 
     @property
     def registered_proxies(self) -> None:
         """Dictionary of registered signal_names and proxies."""
         return self._registered_proxies
 
 
-class SimCamera(Device):
+class SimCameraSetup(CustomDetectorMixin):
+    """Mixin class for the SimCamera device."""
+
+    def on_trigger(self) -> None:
+        """Trigger the camera to acquire images.
+
+        This method can be called from BEC during a scan. It will acquire images and send them to BEC.
+        Whether the trigger is send from BEC is determined by the softwareTrigger argument in the device config.
+
+        Here, we also run a callback on SUB_MONITOR to send the image data the device_monitor endpoint in BEC.
+        """
+        try:
+            for _ in range(self.parent.burst.get()):
+                data = self.parent.image.get()
+                self.parent._run_subs(sub_type=self.parent.SUB_MONITOR, value=data)
+                if self.parent.stopped:
+                    raise DeviceStop
+                if self.parent.write_to_disk.get():
+                    self.parent.h5_writer.receive_data(data)
+        except DeviceStop:
+            pass
+        finally:
+            self.parent.stopped = False
+
+    def on_stage(self) -> None:
+        """Stage the camera for upcoming scan
+
+        This method is called from BEC in preparation of a scan.
+        It receives metadata about the scan from BEC,
+        compiles it and prepares the camera for the scan.
+
+        FYI: No data is written to disk in the simulation, but upon each trigger it
+        is published to the device_monitor endpoint in REDIS.
+        """
+        self.parent.filepath = self.parent.filewriter.compile_full_filename(f"{self.parent.name}")
+
+        self.parent.file_path.set(self.parent.filepath)
+        self.parent.frames.set(
+            self.parent.scaninfo.num_points * self.parent.scaninfo.frames_per_trigger
+        )
+        self.parent.exp_time.set(self.parent.scaninfo.exp_time)
+        self.parent.burst.set(self.parent.scaninfo.frames_per_trigger)
+        if self.parent.write_to_disk.get():
+            self.parent.h5_writer.prepare(
+                file_path=self.parent.filepath, h5_entry="/entry/data/data"
+            )
+            self.publish_file_location(done=False)
+        self.parent.stopped = False
+
+    def on_unstage(self) -> None:
+        """Unstage the device
+
+        Send reads from all config signals to redis
+        """
+        if self.parent.write_to_disk.get():
+            self.publish_file_location(done=True, successful=True)
+
+
+class SimCamera(PSIDetectorBase):
     """A simulated device mimic any 2D camera.
 
     It's image is a computed signal, which is configurable by the user and from the command line.
     The corresponding simulation class is sim_cls=SimulatedDataCamera, more details on defaults within the simulation class.
 
     >>> camera = SimCamera(name="camera")
 
@@ -105,14 +169,15 @@
     kind                    : A member the Kind IntEnum (or equivalent integer), optional. Default is Kind.normal. See Kind for options.
     device_manager          : DeviceManager from BEC, optional . Within startup of simulation, device_manager is passed on automatically.
 
     """
 
     USER_ACCESS = ["sim", "registered_proxies"]
 
+    custom_prepare_cls = SimCameraSetup
     sim_cls = SimulatedDataCamera
     SHAPE = (100, 100)
     BIT_DEPTH = np.uint16
 
     SUB_MONITOR = "monitor"
     _default_sub = SUB_MONITOR
 
@@ -126,106 +191,41 @@
     image = Cpt(
         ReadOnlySignal,
         name="image",
         value=np.empty(SHAPE, dtype=BIT_DEPTH),
         compute_readback=True,
         kind=Kind.omitted,
     )
+    write_to_disk = Cpt(SetableSignal, name="write_to_disk", value=False, kind=Kind.config)
 
     def __init__(
         self, name, *, kind=None, parent=None, sim_init: dict = None, device_manager=None, **kwargs
     ):
-        self.device_manager = device_manager
         self.init_sim_params = sim_init
         self._registered_proxies = {}
-        self.sim = self.sim_cls(parent=self, device_manager=device_manager, **kwargs)
-
-        super().__init__(name=name, parent=parent, kind=kind, **kwargs)
-        self._stopped = False
-        self._staged = False
-        self.scaninfo = None
-        self._update_scaninfo()
+        self.sim = self.sim_cls(parent=self, **kwargs)
+        self.h5_writer = H5Writer()
+        self.filepath = None
+        super().__init__(
+            name=name, parent=parent, kind=kind, device_manager=device_manager, **kwargs
+        )
 
     @property
     def registered_proxies(self) -> None:
         """Dictionary of registered signal_names and proxies."""
         return self._registered_proxies
 
-    def trigger(self) -> DeviceStatus:
-        """Trigger the camera to acquire images.
-
-        This method can be called from BEC during a scan. It will acquire images and send them to BEC.
-        Whether the trigger is send from BEC is determined by the softwareTrigger argument in the device config.
-
-        Here, we also run a callback on SUB_MONITOR to send the image data the device_monitor endpoint in BEC.
-        """
+    def complete(self) -> StatusBase:
+        """Complete the motion of the simulated device."""
         status = DeviceStatus(self)
-
-        self.subscribe(status._finished, event_type=self.SUB_ACQ_DONE, run=False)
-
-        def acquire():
-            try:
-                for _ in range(self.burst.get()):
-                    self._run_subs(sub_type=self.SUB_MONITOR, value=self.image.get())
-                    if self._stopped:
-                        raise DeviceStop
-            except DeviceStop:
-                pass
-            finally:
-                self._stopped = False
-                self._done_acquiring()
-
-        threading.Thread(target=acquire, daemon=True).start()
+        if self.write_to_disk.get():
+            self.h5_writer.write_data()
+        status.set_finished()
         return status
 
-    def _update_scaninfo(self) -> None:
-        """Update scaninfo from BecScaninfoMixing
-        This depends on device manager and operation/sim_mode
-        """
-        self.scaninfo = BecScaninfoMixin(self.device_manager)
-
-    def stage(self) -> list[object]:
-        """Stage the camera for upcoming scan
-
-        This method is called from BEC in preparation of a scan.
-        It receives metadata about the scan from BEC,
-        compiles it and prepares the camera for the scan.
-
-        FYI: No data is written to disk in the simulation, but upon each trigger it
-        is published to the device_monitor endpoint in REDIS.
-        """
-        if self._staged:
-            return super().stage()
-        self.scaninfo.load_scan_metadata()
-        self.file_path.set(
-            os.path.join(
-                self.file_path.get(), self.file_pattern.get().format(self.scaninfo.scan_number)
-            )
-        )
-        self.frames.set(self.scaninfo.num_points * self.scaninfo.frames_per_trigger)
-        self.exp_time.set(self.scaninfo.exp_time)
-        self.burst.set(self.scaninfo.frames_per_trigger)
-        self._stopped = False
-        return super().stage()
-
-    def unstage(self) -> list[object]:
-        """Unstage the device
-
-        Send reads from all config signals to redis
-        """
-        if self._stopped is True or not self._staged:
-            return super().unstage()
-
-        return super().unstage()
-
-    def stop(self, *, success=False):
-        """Stop the device"""
-        self._stopped = True
-        super().stop(success=success)
-
 
 class SimWaveform(Device):
     """A simulated device mimic any 1D Waveform detector.
 
     It's waveform is a computed signal, which is configurable by the user and from the command line.
     The corresponding simulation class is sim_cls=SimulatedDataWaveform, more details on defaults within the simulation class.
 
@@ -268,15 +268,15 @@
 
     def __init__(
         self, name, *, kind=None, parent=None, sim_init: dict = None, device_manager=None, **kwargs
     ):
         self.device_manager = device_manager
         self.init_sim_params = sim_init
         self._registered_proxies = {}
-        self.sim = self.sim_cls(parent=self, device_manager=device_manager, **kwargs)
+        self.sim = self.sim_cls(parent=self, **kwargs)
 
         super().__init__(name=name, parent=parent, kind=kind, **kwargs)
         self._stopped = False
         self._staged = False
         self.scaninfo = None
         self._update_scaninfo()
 
@@ -378,15 +378,15 @@
     kind                    : A member the Kind IntEnum (or equivalent integer), optional. Default is Kind.normal. See Kind for options.
     device_manager          : DeviceManager from BEC, optional . Within startup of simulation, device_manager is passed on automatically.
     sim_init (dict)         : Dictionary to initiate parameters of the simulation, check simulation type defaults for more details.
 
     """
 
     # Specify which attributes are accessible via BEC client
-    USER_ACCESS = ["sim", "readback", "speed", "dummy_controller", "registered_proxies"]
+    USER_ACCESS = ["sim", "readback", "dummy_controller", "registered_proxies"]
 
     sim_cls = SimulatedPositioner
 
     # Define the signals as class attributes
     readback = Cpt(ReadOnlySignal, name="readback", value=0, kind=Kind.hinted)
     setpoint = Cpt(SetableSignal, value=0, kind=Kind.normal)
     motor_is_moving = Cpt(SetableSignal, value=0, kind=Kind.normal)
@@ -413,16 +413,14 @@
         precision=3,
         tolerance: float = 0.5,
         limits=None,
         parent=None,
         kind=None,
         device_manager=None,
         sim_init: dict = None,
-        # TODO remove after refactoring config
-        speed: float = 100,
         **kwargs,
     ):
         self.delay = delay
         self.device_manager = device_manager
         self.precision = precision
         self.tolerance = tolerance
         self.init_sim_params = sim_init
@@ -595,21 +593,20 @@
         name: str,
         *,
         precision: int = 3,
         parent=None,
         kind=None,
         device_manager=None,
         # TODO remove after refactoring config
-        speed: float = 100,
         delay: int = 1,
         update_frequency: int = 100,
         **kwargs,
     ):
 
-        self.sim = self.sim_cls(parent=self, device_manager=device_manager, **kwargs)
+        self.sim = self.sim_cls(parent=self, **kwargs)
         self.precision = precision
         self.device_manager = device_manager
         self._registered_proxies = {}
 
         super().__init__(name=name, parent=parent, kind=kind, **kwargs)
         self.sim.sim_state[self.name] = self.sim.sim_state.pop(self.readback.name, None)
         self.readback.name = self.name
```

### Comparing `ophyd_devices-1.1.0/ophyd_devices/sim/sim_data.py` & `ophyd_devices-1.2.0/ophyd_devices/sim/sim_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,37 +86,36 @@
     - sim_params:                   get the parameters for the active simulation mdoel
     - sim_models:                   get the available simulation models
     - update_sim_state:             update the simulated state of the device
     """
 
     USER_ACCESS = ["sim_params", "sim_select_model", "sim_get_models", "sim_show_all"]
 
-    def __init__(self, *args, parent=None, device_manager=None, **kwargs) -> None:
+    def __init__(self, *args, parent=None, **kwargs) -> None:
         """
         Note:
         self._model_params duplicates parameters from _params that are solely relevant for the model used.
         This facilitates easier and faster access for computing the simulated state using the lmfit package.
         """
         self.parent = parent
-        self.device_manager = device_manager
         self.sim_state = defaultdict(dict)
         self.registered_proxies = getattr(self.parent, "registered_proxies", {})
         self._model = {}
         self._model_params = None
         self._params = {}
 
     def execute_simulation_method(self, *args, method=None, signal_name: str = "", **kwargs) -> any:
         """
         Execute either the provided method or reroutes the method execution
         to a device proxy in case it is registered in self.parentregistered_proxies.
         """
-        if self.registered_proxies and self.device_manager:
+        if self.registered_proxies and self.parent.device_manager:
             for proxy_name, signal in self.registered_proxies.items():
                 if signal == signal_name or f"{self.parent.name}_{signal}" == signal_name:
-                    sim_proxy = self.device_manager.devices.get(proxy_name, None)
+                    sim_proxy = self.parent.device_manager.devices.get(proxy_name, None)
                     if sim_proxy and sim_proxy.enabled is True:
                         method = sim_proxy.obj.lookup[self.parent.name]["method"]
                         args = sim_proxy.obj.lookup[self.parent.name]["args"]
                         kwargs = sim_proxy.obj.lookup[self.parent.name]["kwargs"]
                     break
 
         if method is not None:
@@ -300,17 +299,17 @@
             value = self.execute_simulation_method(method=method, signal_name=signal_name)
             self.update_sim_state(signal_name, value)
 
 
 class SimulatedDataMonitor(SimulatedDataBase):
     """Simulated data class for a monitor."""
 
-    def __init__(self, *args, parent=None, device_manager=None, **kwargs) -> None:
+    def __init__(self, *args, parent=None, **kwargs) -> None:
         self._model_lookup = self.init_lmfit_models()
-        super().__init__(*args, parent=parent, device_manager=device_manager, **kwargs)
+        super().__init__(*args, parent=parent, **kwargs)
         self.bit_depth = self.parent.BIT_DEPTH
         self._init_default()
 
     def _get_additional_params(self) -> None:
         params = deepcopy(DEFAULT_PARAMS_NOISE)
         params.update(deepcopy(DEFAULT_PARAMS_MOTOR))
         return params
@@ -408,16 +407,16 @@
         """
         Compute the return value for given motor position and active model.
 
         Returns:
             float: Value computed by the active model.
         """
         mot_name = self.sim_params["ref_motor"]
-        if self.device_manager and mot_name in self.device_manager.devices:
-            motor_pos = self.device_manager.devices[mot_name].obj.read()[mot_name]["value"]
+        if self.parent.device_manager and mot_name in self.parent.device_manager.devices:
+            motor_pos = self.parent.device_manager.devices[mot_name].obj.read()[mot_name]["value"]
         else:
             motor_pos = 0
         method = self._model
         value = int(method.eval(params=self._model_params, x=motor_pos))
         return self._add_noise(value, self.sim_params["noise"], self.sim_params["noise_multiplier"])
 
     def _add_noise(self, v: int, noise: NoiseType, noise_multiplier: float) -> int:
@@ -498,19 +497,19 @@
         if noise == NoiseType.NONE:
             return v
 
 
 class SimulatedDataCamera(SimulatedDataBase):
     """Simulated class to compute data for a 2D camera."""
 
-    def __init__(self, *args, parent=None, device_manager=None, **kwargs) -> None:
+    def __init__(self, *args, parent=None, **kwargs) -> None:
         self._model_lookup = self.init_2D_models()
         self._all_default_model_params = defaultdict(dict)
         self._init_default_camera_params()
-        super().__init__(*args, parent=parent, device_manager=device_manager, **kwargs)
+        super().__init__(*args, parent=parent, **kwargs)
         self.bit_depth = self.parent.BIT_DEPTH
         self._init_default()
 
     def _init_default(self) -> None:
         """Initialize the default model for a simulated camera
 
         Use the default model "Gaussian".
```

### Comparing `ophyd_devices-1.1.0/ophyd_devices/sim/sim_frameworks.py` & `ophyd_devices-1.2.0/ophyd_devices/sim/sim_frameworks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/sim/sim_signals.py` & `ophyd_devices-1.2.0/ophyd_devices/sim/sim_signals.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/sim/sim_test_devices.py` & `ophyd_devices-1.2.0/ophyd_devices/sim/sim_test_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/sim/sim_xtreme.py` & `ophyd_devices-1.2.0/ophyd_devices/sim/sim_xtreme.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt` & `ophyd_devices-1.2.0/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt` & `ophyd_devices-1.2.0/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt` & `ophyd_devices-1.2.0/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt` & `ophyd_devices-1.2.0/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/tests/utils.py` & `ophyd_devices-1.2.0/ophyd_devices/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/utils/bec_device_base.py` & `ophyd_devices-1.2.0/ophyd_devices/utils/bec_device_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/utils/bec_scaninfo_mixin.py` & `ophyd_devices-1.2.0/ophyd_devices/utils/bec_scaninfo_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,22 @@
         self.scan_id = None
         if bec_info_msg is None:
             infomsgmock = BECInfoMsgMock()
             self.bec_info_msg = infomsgmock.get_bec_info_msg()
         else:
             self.bec_info_msg = bec_info_msg
 
+        self.metadata = None
+        self.scan_id = None
+        self.scan_number = None
+        self.exp_time = None
+        self.frames_per_trigger = None
+        self.num_points = None
+        self.scan_type = None
+
     def get_bec_info_msg(self) -> None:
         """Get BECInfoMsg object"""
         return self.bec_info_msg
 
     def change_config(self, bec_info_msg: dict) -> None:
         """Change BECInfoMsg object"""
         self.bec_info_msg = bec_info_msg
```

### Comparing `ophyd_devices-1.1.0/ophyd_devices/utils/bec_utils.py` & `ophyd_devices-1.2.0/ophyd_devices/utils/bec_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/utils/controller.py` & `ophyd_devices-1.2.0/ophyd_devices/utils/controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/utils/dynamic_pseudo.py` & `ophyd_devices-1.2.0/ophyd_devices/utils/dynamic_pseudo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/utils/socket.py` & `ophyd_devices-1.2.0/ophyd_devices/utils/socket.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/ophyd_devices/utils/static_device_test.py` & `ophyd_devices-1.2.0/ophyd_devices/utils/static_device_test.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/tests/test_base_classes.py` & `ophyd_devices-1.2.0/tests/test_base_classes.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/tests/test_controller.py` & `ophyd_devices-1.2.0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/tests/test_dynamic_pseudo.py` & `ophyd_devices-1.2.0/tests/test_dynamic_pseudo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/tests/test_ophyd_status_obj.py` & `ophyd_devices-1.2.0/tests/test_ophyd_status_obj.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/tests/test_simulation.py` & `ophyd_devices-1.2.0/tests/test_simulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     BECPositionerProtocol,
     BECScanProtocol,
     BECSignalProtocol,
 )
 from ophyd_devices.sim.sim import SimCamera, SimFlyer, SimMonitor, SimPositioner
 from ophyd_devices.sim.sim_frameworks import H5ImageReplayProxy, SlitProxy
 from ophyd_devices.sim.sim_signals import ReadOnlySignal
+from ophyd_devices.sim.sim_utils import H5Writer
 from ophyd_devices.utils.bec_device_base import BECDevice, BECDeviceBase
 
 
 @pytest.fixture(scope="function")
 def signal(name="signal"):
     """Fixture for Signal."""
     sig = ReadOnlySignal(name=name, value=0)
@@ -38,41 +39,51 @@
     yield mon
 
 
 @pytest.fixture(scope="function")
 def camera(name="camera"):
     """Fixture for SimCamera."""
     dm = DMMock()
-    cam = SimCamera(name=name, device_manager=dm)
-    yield cam
+    with (
+        mock.patch(
+            "ophyd_devices.interfaces.base_classes.psi_detector_base.PSIDetectorBase._update_service_config",
+            mock.MagicMock(),
+        ) as mock_update_service_config,
+        mock.patch(
+            "ophyd_devices.interfaces.base_classes.psi_detector_base.PSIDetectorBase._update_filewriter",
+            mock.MagicMock(),
+        ) as mock_update_filewriter,
+    ):
+        cam = SimCamera(name=name, device_manager=dm)
+        cam.filewriter = mock.MagicMock()
+        cam.filewriter.compile_full_filename.return_value = ""
+        yield cam
 
 
 @pytest.fixture(scope="function")
 def positioner(name="positioner"):
     """Fixture for SimPositioner."""
     dm = DMMock()
     pos = SimPositioner(name=name, device_manager=dm)
     yield pos
 
 
 @pytest.fixture(scope="function")
-def h5proxy_fixture(name="h5proxy"):
+def h5proxy_fixture(camera, name="h5proxy"):
     """Fixture for SimCamera."""
-    dm = DMMock()
+    dm = camera.device_manager
     proxy = H5ImageReplayProxy(name=name, device_manager=dm)
-    camera = SimCamera(name="eiger", device_manager=dm)
     yield proxy, camera
 
 
 @pytest.fixture(scope="function")
-def slitproxy_fixture(name="slit_proxy"):
+def slitproxy_fixture(camera, name="slit_proxy"):
     """Fixture for SimCamera."""
-    dm = DMMock()
+    dm = camera.device_manager
     proxy = SlitProxy(name=name, device_manager=dm)
-    camera = SimCamera(name="eiger", device_manager=dm)
     samx = SimPositioner(name="samx", device_manager=dm)
     yield proxy, camera, samx
 
 
 @pytest.fixture(scope="function")
 def flyer(name="flyer"):
     """Fixture for SimFlyer."""
@@ -117,15 +128,15 @@
     assert isinstance(flyer, BECFlyerProtocol)
 
 
 @pytest.mark.parametrize("center", [-10, 0, 10])
 def test_monitor_readback(monitor, center):
     """Test the readback method of SimMonitor."""
     motor_pos = 0
-    monitor.sim.device_manager.add_device("samx", value=motor_pos)
+    monitor.device_manager.add_device("samx", value=motor_pos)
     for model_name in monitor.sim.sim_get_models():
         monitor.sim.sim_select_model(model_name)
         monitor.sim.sim_params["noise_multipler"] = 10
         monitor.sim.sim_params["ref_motor"] = "samx"
         if "c" in monitor.sim.sim_params:
             monitor.sim.sim_params["c"] = center
         elif "center" in monitor.sim.sim_params:
@@ -197,15 +208,15 @@
     assert bec_device_base.connected is True
     signal = Signal(name="signal")
     assert isinstance(signal, BECDevice)
     device = Device(name="device")
     assert isinstance(device, BECDevice)
 
 
-def test_h5proxy(h5proxy_fixture):
+def test_h5proxy(h5proxy_fixture, camera):
     """Test h5 camera proxy read from h5 file"""
     h5proxy, camera = h5proxy_fixture
     mock_proxy = mock.MagicMock()
     camera.device_manager.devices.update({h5proxy.name: mock_proxy})
     mock_proxy.enabled = True
     mock_proxy.obj = h5proxy
     fname = os.path.expanduser("tests/test_data/h5_test_file.h5")
@@ -215,23 +226,28 @@
     # pylint: disable=protected-access
     h5proxy._update_device_config(
         {camera.name: {"signal_name": "image", "file_source": fname, "h5_entry": h5entry}}
     )
     camera._registered_proxies.update({h5proxy.name: camera.image.name})
     camera.sim.sim_params = {"noise": "none", "noise_multiplier": 0}
     camera.scaninfo.sim_mode = True
+    camera.image_shape.set(data.shape[1:])
     camera.stage()
     img = camera.image.get()
     assert (img == data[0, ...]).all()
     camera.unstage()
 
 
 def test_slitproxy(slitproxy_fixture):
     """Test slit proxy to compute readback from readback of positioner samx"""
     proxy, camera, samx = slitproxy_fixture
+    for dev_name, dev in proxy.device_manager.devices.items():
+        camera.device_manager.devices.update({dev_name: mock.MagicMock()})
+        camera.device_manager.devices.get(dev_name).obj = dev
+        camera.device_manager.devices.get(dev_name).enabled = True
     px_size = 0.5
     slitwidth = 2
     proxy._update_device_config(
         {
             camera.name: {
                 "signal_name": "image",
                 "center_offset": [0, 0],
@@ -274,7 +290,70 @@
     img = camera.image.get()
     edges = (
         int(img.shape[0] // 2 + samx_pos / px_size - slitwidth / (2 * px_size)),
         int(img.shape[0] // 2 + samx_pos / px_size + slitwidth / (2 * px_size)),
     )
     assert (img[:, : edges[0]] == 0).all()
     assert (img[:, edges[1] :] == 0).all()
+
+
+def test_cam_stage_h5writer(camera):
+    """Test the H5Writer class"""
+    with (
+        mock.patch.object(camera, "h5_writer") as mock_h5_writer,
+        mock.patch.object(
+            camera.custom_prepare, "publish_file_location"
+        ) as mock_publish_file_location,
+    ):
+        camera.scaninfo.num_points = 10
+        camera.scaninfo.frames_per_trigger = 1
+        camera.scaninfo.exp_time = 1
+        camera.stage()
+        assert mock_h5_writer.prepare.call_count == 0
+        camera.unstage()
+        camera.write_to_disk.put(True)
+        camera.stage()
+        calls = [mock.call(file_path="", h5_entry="/entry/data/data")]
+        assert mock_h5_writer.prepare.mock_calls == calls
+        # mock_h5_writer.prepare
+
+
+def test_cam_complete(camera):
+    """Test the complete method of SimCamera."""
+    with mock.patch.object(camera, "h5_writer") as mock_h5_writer:
+        camera.complete()
+        assert mock_h5_writer.write_data.call_count == 0
+        camera.write_to_disk.put(True)
+        camera.complete()
+        assert mock_h5_writer.write_data.call_count == 1
+
+
+def test_cam_trigger(camera):
+    """Test the trigger method of SimCamera."""
+    with mock.patch.object(camera, "h5_writer") as mock_h5_writer:
+        data = []
+        camera.trigger()
+        assert mock_h5_writer.receive_data.call_count == 0
+        camera.write_to_disk.put(True)
+        camera.trigger()
+        assert mock_h5_writer.receive_data.call_count == 1
+        camera.trigger()
+        assert mock_h5_writer.receive_data.call_count == 2
+
+
+def test_h5writer():
+    """Test the H5Writer class"""
+
+    h5_writer = H5Writer()
+    with mock.patch.object(h5_writer, "create_dir") as mock_create_dir:
+        h5_writer.data_container = [0, 1, 2]
+        h5_writer.prepare(file_path="test.h5", h5_entry="entry/data/data")
+        assert mock_create_dir.call_count == 1
+        assert h5_writer.data_container == []
+        assert h5_writer.file_path == "test.h5"
+        assert h5_writer.h5_entry == "entry/data/data"
+
+        data = [0, 1, 2, 3]
+        h5_writer.receive_data(data)
+        assert h5_writer.data_container == [data]
+        h5_writer.receive_data(0)
+        assert h5_writer.data_container == [data, 0]
```

### Comparing `ophyd_devices-1.1.0/tests/test_socket.py` & `ophyd_devices-1.2.0/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/.gitignore` & `ophyd_devices-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/LICENSE` & `ophyd_devices-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.1.0/pyproject.toml` & `ophyd_devices-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ophyd_devices"
-version = "1.1.0"
+version = "1.2.0"
 description = "Custom device implementations based on the ophyd hardware abstraction layer"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.1.0/PKG-INFO` & `ophyd_devices-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ophyd_devices
-Version: 1.1.0
+Version: 1.2.0
 Summary: Custom device implementations based on the ophyd hardware abstraction layer
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/ophyd_devices/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/ophyd_devices
 Project-URL: documentation, https://bec.readthedocs.org
 Project-URL: changelog, https://gitlab.psi.ch/bec/ophyd_devices/blob/main/CHANGELOG.md
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

