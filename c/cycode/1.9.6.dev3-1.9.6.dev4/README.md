# Comparing `tmp/cycode-1.9.6.dev3.tar.gz` & `tmp/cycode-1.9.6.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-1.9.6.dev3.tar", max compression
+gzip compressed data, was "cycode-1.9.6.dev4.tar", max compression
```

## Comparing `cycode-1.9.6.dev3.tar` & `cycode-1.9.6.dev4.tar`

### file list

```diff
@@ -1,109 +1,110 @@
--rw-r--r--   0        0        0    42867 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/README.md
--rw-r--r--   0        0        0      114 2024-05-28 10:47:48.925091 cycode-1.9.6.dev3/cycode/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/auth/__init__.py
--rw-r--r--   0        0        0     2897 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/auth/auth_command.py
--rw-r--r--   0        0        0     4726 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/auth/auth_manager.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/configure/__init__.py
--rw-r--r--   0        0        0     5423 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/configure/configure_command.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/ignore/__init__.py
--rw-r--r--   0        0        0     3873 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/ignore/ignore_command.py
--rw-r--r--   0        0        0     2497 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/main_cli.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/__init__.py
--rw-r--r--   0        0        0      563 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/report_command.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/__init__.py
--rw-r--r--   0        0        0     3435 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/common.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/path/__init__.py
--rw-r--r--   0        0        0     2821 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/path/path_command.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/repository_url/__init__.py
--rw-r--r--   0        0        0     2143 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py
--rw-r--r--   0        0        0     2358 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/sbom_command.py
--rw-r--r--   0        0        0     1533 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/sbom_report_file.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/__init__.py
--rw-r--r--   0        0        0    39829 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/code_scanner.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/commit_history/__init__.py
--rw-r--r--   0        0        0      975 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/commit_history/commit_history_command.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/path/__init__.py
--rw-r--r--   0        0        0      590 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/path/path_command.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/pre_commit/__init__.py
--rw-r--r--   0        0        0     1605 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/pre_commit/pre_commit_command.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/pre_receive/__init__.py
--rw-r--r--   0        0        0     2722 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/pre_receive/pre_receive_command.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/repository/__init__.py
--rw-r--r--   0        0        0     2710 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/repository/repository_command.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_ci/__init__.py
--rw-r--r--   0        0        0     1588 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_ci/ci_integrations.py
--rw-r--r--   0        0        0      552 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_ci/scan_ci_command.py
--rw-r--r--   0        0        0     5082 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_command.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/version/__init__.py
--rw-r--r--   0        0        0      509 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/version/version_command.py
--rw-r--r--   0        0        0      466 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/config.py
--rw-r--r--   0        0        0      463 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/config.yaml
--rw-r--r--   0        0        0     6194 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     2109 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0     1620 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/exceptions/handle_report_sbom_errors.py
--rw-r--r--   0        0        0     2785 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/exceptions/handle_scan_errors.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/__init__.py
--rw-r--r--   0        0        0     6243 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/excluder.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/iac/__init__.py
--rw-r--r--   0        0        0     2457 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/iac/tf_content_generator.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/models/__init__.py
--rw-r--r--   0        0        0     1247 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/models/in_memory_zip.py
--rw-r--r--   0        0        0     4394 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/path_documents.py
--rw-r--r--   0        0        0     4940 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/repository_documents.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/sca/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/__init__.py
--rw-r--r--   0        0        0     2412 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0     1136 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     3119 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     6400 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/sca/sca_code_scanner.py
--rw-r--r--   0        0        0     1873 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/zip_documents.py
--rw-r--r--   0        0        0      387 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/main.py
--rw-r--r--   0        0        0     2051 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0     2496 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     2490 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     1613 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/printer_base.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/tables/__init__.py
--rw-r--r--   0        0        0     7762 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/tables/sca_table_printer.py
--rw-r--r--   0        0        0     2281 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/tables/table.py
--rw-r--r--   0        0        0      480 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/tables/table_models.py
--rw-r--r--   0        0        0     5264 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/tables/table_printer.py
--rw-r--r--   0        0        0     2618 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/tables/table_printer_base.py
--rw-r--r--   0        0        0    10847 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      630 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4939 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     7591 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     2987 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0      745 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/user_settings/jwt_creator.py
--rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0      211 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/enum_utils.py
--rw-r--r--   0        0        0     1584 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/get_api_client.py
--rw-r--r--   0        0        0     1953 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0     9940 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/progress_bar.py
--rw-r--r--   0        0        0     2794 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/scan_batch.py
--rw-r--r--   0        0        0      334 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      967 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     2034 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2748 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      934 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0       71 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1777 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     1072 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/client_creator.py
--rw-r--r--   0        0        0     3349 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      120 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      257 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     3699 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      670 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     3600 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     1319 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/headers.py
--rw-r--r--   0        0        0    13226 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/models.py
--rw-r--r--   0        0        0     3971 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/report_client.py
--rw-r--r--   0        0        0    13213 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0     1658 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/scan_config_base.py
--rw-r--r--   0        0        0     3467 2024-05-28 10:47:48.921091 cycode-1.9.6.dev3/pyproject.toml
--rw-r--r--   0        0        0    44445 1970-01-01 00:00:00.000000 cycode-1.9.6.dev3/PKG-INFO
+-rw-r--r--   0        0        0    42867 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/README.md
+-rw-r--r--   0        0        0      114 2024-05-28 11:11:10.722034 cycode-1.9.6.dev4/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/auth/__init__.py
+-rw-r--r--   0        0        0     2897 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/auth/auth_command.py
+-rw-r--r--   0        0        0     4726 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/auth/auth_manager.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/configure/__init__.py
+-rw-r--r--   0        0        0     5423 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/configure/configure_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/ignore/__init__.py
+-rw-r--r--   0        0        0     3873 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/ignore/ignore_command.py
+-rw-r--r--   0        0        0     2497 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/main_cli.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/report/__init__.py
+-rw-r--r--   0        0        0      563 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/report/report_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/report/sbom/__init__.py
+-rw-r--r--   0        0        0     3435 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/report/sbom/common.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/report/sbom/path/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/report/sbom/path/path_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/report/sbom/repository_url/__init__.py
+-rw-r--r--   0        0        0     2143 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py
+-rw-r--r--   0        0        0     2358 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/report/sbom/sbom_command.py
+-rw-r--r--   0        0        0     1533 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/report/sbom/sbom_report_file.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/scan/__init__.py
+-rw-r--r--   0        0        0    39881 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/scan/code_scanner.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/scan/commit_history/__init__.py
+-rw-r--r--   0        0        0      975 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/scan/commit_history/commit_history_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/scan/path/__init__.py
+-rw-r--r--   0        0        0      590 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/scan/path/path_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/scan/pre_commit/__init__.py
+-rw-r--r--   0        0        0     1647 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/scan/pre_commit/pre_commit_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/scan/pre_receive/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-28 11:11:01.170107 cycode-1.9.6.dev4/cycode/cli/commands/scan/pre_receive/pre_receive_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/commands/scan/repository/__init__.py
+-rw-r--r--   0        0        0     2710 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/commands/scan/repository/repository_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/commands/scan/scan_ci/__init__.py
+-rw-r--r--   0        0        0     1588 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/commands/scan/scan_ci/ci_integrations.py
+-rw-r--r--   0        0        0      552 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/commands/scan/scan_ci/scan_ci_command.py
+-rw-r--r--   0        0        0     5082 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/commands/scan/scan_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/commands/version/__init__.py
+-rw-r--r--   0        0        0      509 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/commands/version/version_command.py
+-rw-r--r--   0        0        0      466 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/config.py
+-rw-r--r--   0        0        0      463 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     6194 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     2109 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/exceptions/handle_report_sbom_errors.py
+-rw-r--r--   0        0        0     2875 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/exceptions/handle_scan_errors.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/__init__.py
+-rw-r--r--   0        0        0     6243 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/excluder.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/iac/__init__.py
+-rw-r--r--   0        0        0     2457 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/iac/tf_content_generator.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/models/__init__.py
+-rw-r--r--   0        0        0     1247 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/models/in_memory_zip.py
+-rw-r--r--   0        0        0     4394 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/path_documents.py
+-rw-r--r--   0        0        0     5053 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/repository_documents.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/sca/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/sca/maven/__init__.py
+-rw-r--r--   0        0        0     2412 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0     1136 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     3119 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     6489 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/sca/sca_code_scanner.py
+-rw-r--r--   0        0        0     1873 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/files_collector/zip_documents.py
+-rw-r--r--   0        0        0      387 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/main.py
+-rw-r--r--   0        0        0     2051 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0     2496 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     2490 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     1636 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/printers/printer_base.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/printers/tables/__init__.py
+-rw-r--r--   0        0        0     7762 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/printers/tables/sca_table_printer.py
+-rw-r--r--   0        0        0     2281 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/printers/tables/table.py
+-rw-r--r--   0        0        0      480 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/printers/tables/table_models.py
+-rw-r--r--   0        0        0     5264 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/printers/tables/table_printer.py
+-rw-r--r--   0        0        0     2618 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/printers/tables/table_printer_base.py
+-rw-r--r--   0        0        0    10847 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      630 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4939 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     7591 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     2987 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0      745 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/user_settings/jwt_creator.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/utils/enum_utils.py
+-rw-r--r--   0        0        0     1584 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/utils/get_api_client.py
+-rw-r--r--   0        0        0     2083 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/utils/git_proxy.py
+-rw-r--r--   0        0        0     1953 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0     9940 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/utils/progress_bar.py
+-rw-r--r--   0        0        0     2794 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/utils/scan_batch.py
+-rw-r--r--   0        0        0      334 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      967 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     2034 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2748 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      934 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0       71 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1777 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     1072 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/client_creator.py
+-rw-r--r--   0        0        0     3349 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      120 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      257 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3699 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      670 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     3600 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     1319 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/headers.py
+-rw-r--r--   0        0        0    13226 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     3971 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/report_client.py
+-rw-r--r--   0        0        0    13213 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0     1658 2024-05-28 11:11:01.174107 cycode-1.9.6.dev4/cycode/cyclient/scan_config_base.py
+-rw-r--r--   0        0        0     3467 2024-05-28 11:11:10.718034 cycode-1.9.6.dev4/pyproject.toml
+-rw-r--r--   0        0        0    44445 1970-01-01 00:00:00.000000 cycode-1.9.6.dev4/PKG-INFO
```

### Comparing `cycode-1.9.6.dev3/README.md` & `cycode-1.9.6.dev4/README.md`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/auth/auth_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/auth/auth_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/auth/auth_manager.py` & `cycode-1.9.6.dev4/cycode/cli/commands/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/configure/configure_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/configure/configure_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/ignore/ignore_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/ignore/ignore_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/main_cli.py` & `cycode-1.9.6.dev4/cycode/cli/commands/main_cli.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/report/report_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/report/report_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/common.py` & `cycode-1.9.6.dev4/cycode/cli/commands/report/sbom/common.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/path/path_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/report/sbom/path/path_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/sbom_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/report/sbom/sbom_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/sbom_report_file.py` & `cycode-1.9.6.dev4/cycode/cli/commands/report/sbom/sbom_report_file.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/scan/code_scanner.py` & `cycode-1.9.6.dev4/cycode/cli/commands/scan/code_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import sys
 import time
 from platform import platform
 from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Tuple
 from uuid import UUID, uuid4
 
 import click
-from git import NULL_TREE, Repo
 
 from cycode.cli import consts
 from cycode.cli.config import configuration_manager
 from cycode.cli.exceptions import custom_exceptions
 from cycode.cli.exceptions.handle_scan_errors import handle_scan_exception
 from cycode.cli.files_collector.excluder import exclude_irrelevant_documents_to_scan
 from cycode.cli.files_collector.models.in_memory_zip import InMemoryZip
@@ -24,17 +23,16 @@
 )
 from cycode.cli.files_collector.sca import sca_code_scanner
 from cycode.cli.files_collector.sca.sca_code_scanner import perform_pre_scan_documents_actions
 from cycode.cli.files_collector.zip_documents import zip_documents
 from cycode.cli.models import CliError, Document, DocumentDetections, LocalScanResult, Severity
 from cycode.cli.printers import ConsolePrinter
 from cycode.cli.utils import scan_utils
-from cycode.cli.utils.path_utils import (
-    get_path_by_os,
-)
+from cycode.cli.utils.git_proxy import git_proxy
+from cycode.cli.utils.path_utils import get_path_by_os
 from cycode.cli.utils.progress_bar import ScanProgressBarSection
 from cycode.cli.utils.scan_batch import run_parallel_batched_scan
 from cycode.cli.utils.scan_utils import set_issue_detected
 from cycode.cyclient import logger
 from cycode.cyclient.config import set_logging_level
 from cycode.cyclient.models import Detection, DetectionSchema, DetectionsPerFile, ZippedFileScanResult
 
@@ -240,15 +238,15 @@
 
     if scan_type == consts.SCA_SCAN_TYPE:
         return scan_sca_commit_range(context, path, commit_range)
 
     documents_to_scan = []
     commit_ids_to_scan = []
 
-    repo = Repo(path)
+    repo = git_proxy.get_repo(path)
     total_commits_count = int(repo.git.rev_list('--count', commit_range))
     logger.debug('Calculating diffs for %s commits in the commit range %s', total_commits_count, commit_range)
 
     progress_bar.set_section_length(ScanProgressBarSection.PREPARE_LOCAL_FILES, total_commits_count)
 
     scanned_commits_count = 0
     for commit in repo.iter_commits(rev=commit_range):
@@ -257,15 +255,15 @@
             progress_bar.update(ScanProgressBarSection.PREPARE_LOCAL_FILES, total_commits_count - scanned_commits_count)
             break
 
         progress_bar.update(ScanProgressBarSection.PREPARE_LOCAL_FILES)
 
         commit_id = commit.hexsha
         commit_ids_to_scan.append(commit_id)
-        parent = commit.parents[0] if commit.parents else NULL_TREE
+        parent = commit.parents[0] if commit.parents else git_proxy.get_null_tree()
         diff = commit.diff(parent, create_patch=True, R=True)
         commit_documents_to_scan = []
         for blob in diff:
             blob_path = get_path_by_os(os.path.join(path, get_diff_file_path(blob)))
             commit_documents_to_scan.append(
                 Document(
                     path=blob_path,
@@ -684,15 +682,15 @@
         scan_parameters['remote_url'] = remote_url
 
     return scan_parameters
 
 
 def try_get_git_remote_url(path: str) -> Optional[str]:
     try:
-        remote_url = Repo(path).remotes[0].config_reader.get('url')
+        remote_url = git_proxy.get_repo(path).remotes[0].config_reader.get('url')
         logger.debug('Found Git remote URL, %s', {'remote_url': remote_url, 'path': path})
         return remote_url
     except Exception as e:
         logger.debug('Failed to get Git remote URL', exc_info=e)
         return None
```

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/scan/commit_history/commit_history_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/scan/commit_history/commit_history_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/scan/path/path_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/scan/path/path_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/scan/pre_commit/pre_commit_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/scan/pre_commit/pre_commit_command.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 from typing import List
 
 import click
-from git import Repo
 
 from cycode.cli import consts
 from cycode.cli.commands.scan.code_scanner import scan_documents, scan_sca_pre_commit
 from cycode.cli.files_collector.excluder import exclude_irrelevant_documents_to_scan
 from cycode.cli.files_collector.repository_documents import (
     get_diff_file_content,
     get_diff_file_path,
 )
 from cycode.cli.models import Document
+from cycode.cli.utils.git_proxy import git_proxy
 from cycode.cli.utils.path_utils import (
     get_path_by_os,
 )
 from cycode.cli.utils.progress_bar import ScanProgressBarSection
 
 
 @click.command(short_help='Use this command to scan any content that was not committed yet.')
@@ -27,15 +27,15 @@
     progress_bar = context.obj['progress_bar']
     progress_bar.start()
 
     if scan_type == consts.SCA_SCAN_TYPE:
         scan_sca_pre_commit(context)
         return
 
-    diff_files = Repo(os.getcwd()).index.diff('HEAD', create_patch=True, R=True)
+    diff_files = git_proxy.get_repo(os.getcwd()).index.diff('HEAD', create_patch=True, R=True)
 
     progress_bar.set_section_length(ScanProgressBarSection.PREPARE_LOCAL_FILES, len(diff_files))
 
     documents_to_scan = []
     for file in diff_files:
         progress_bar.update(ScanProgressBarSection.PREPARE_LOCAL_FILES)
         documents_to_scan.append(Document(get_path_by_os(get_diff_file_path(file)), get_diff_file_content(file)))
```

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/scan/pre_receive/pre_receive_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/scan/pre_receive/pre_receive_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/scan/repository/repository_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/scan/repository/repository_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_ci/ci_integrations.py` & `cycode-1.9.6.dev4/cycode/cli/commands/scan/scan_ci/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_ci/scan_ci_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/scan/scan_ci/scan_ci_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_command.py` & `cycode-1.9.6.dev4/cycode/cli/commands/scan/scan_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/consts.py` & `cycode-1.9.6.dev4/cycode/cli/consts.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/exceptions/custom_exceptions.py` & `cycode-1.9.6.dev4/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/exceptions/handle_report_sbom_errors.py` & `cycode-1.9.6.dev4/cycode/cli/exceptions/handle_report_sbom_errors.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/exceptions/handle_scan_errors.py` & `cycode-1.9.6.dev4/cycode/cli/exceptions/handle_scan_errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Optional
 
 import click
-from git import InvalidGitRepositoryError
 
 from cycode.cli.exceptions import custom_exceptions
 from cycode.cli.models import CliError, CliErrors
 from cycode.cli.printers import ConsolePrinter
+from cycode.cli.utils.git_proxy import git_proxy
 
 
 def handle_scan_exception(
     context: click.Context, e: Exception, *, return_exception: bool = False
 ) -> Optional[CliError]:
     context.obj['did_fail'] = True
 
-    ConsolePrinter(context).print_exception()
+    ConsolePrinter(context).print_exception(e)
 
     errors: CliErrors = {
         custom_exceptions.NetworkError: CliError(
             soft_fail=True,
             code='cycode_error',
             message='Cycode was unable to complete this scan. '
             'Please try again by executing the `cycode scan` command',
@@ -45,15 +45,15 @@
             soft_fail=True,
             code='key_error',
             message=f'\n{e!s}\n'
             'A crucial field is missing in your terraform plan file. '
             'Please make sure that your file is well formed '
             'and execute the scan again',
         ),
-        InvalidGitRepositoryError: CliError(
+        git_proxy.get_invalid_git_repository_error(): CliError(
             soft_fail=False,
             code='invalid_git_error',
             message='The path you supplied does not correlate to a git repository. '
             'If you still wish to scan this path, use: `cycode scan path <path>`',
         ),
     }
 
@@ -65,14 +65,17 @@
 
         if return_exception:
             return error
 
         ConsolePrinter(context).print_error(error)
         return None
 
+    unknown_error = CliError(code='unknown_error', message=str(e))
+
     if return_exception:
-        return CliError(code='unknown_error', message=str(e))
+        return unknown_error
 
     if isinstance(e, click.ClickException):
         raise e
 
-    raise click.ClickException(str(e))
+    ConsolePrinter(context).print_error(unknown_error)
+    exit(1)
```

### Comparing `cycode-1.9.6.dev3/cycode/cli/files_collector/excluder.py` & `cycode-1.9.6.dev4/cycode/cli/files_collector/excluder.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/files_collector/iac/tf_content_generator.py` & `cycode-1.9.6.dev4/cycode/cli/files_collector/iac/tf_content_generator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/files_collector/models/in_memory_zip.py` & `cycode-1.9.6.dev4/cycode/cli/files_collector/models/in_memory_zip.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/files_collector/path_documents.py` & `cycode-1.9.6.dev4/cycode/cli/files_collector/path_documents.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/files_collector/repository_documents.py` & `cycode-1.9.6.dev4/cycode/cli/files_collector/repository_documents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import os
 from typing import TYPE_CHECKING, Iterator, List, Optional, Tuple, Union
 
 from cycode.cli import consts
 from cycode.cli.files_collector.sca import sca_code_scanner
 from cycode.cli.models import Document
+from cycode.cli.utils.git_proxy import git_proxy
 from cycode.cli.utils.path_utils import get_file_content, get_path_by_os
 
 if TYPE_CHECKING:
     from git import Blob, Diff
     from git.objects.base import IndexObjUnion
     from git.objects.tree import TraversedTreeTup
 
     from cycode.cli.utils.progress_bar import BaseProgressBar, ProgressBarSection
 
-from git import Repo
-
 
 def should_process_git_object(obj: 'Blob', _: int) -> bool:
     return obj.type == 'blob' and obj.size > 0
 
 
 def get_git_repository_tree_file_entries(
     path: str, branch: str
 ) -> Union[Iterator['IndexObjUnion'], Iterator['TraversedTreeTup']]:
-    return Repo(path).tree(branch).traverse(predicate=should_process_git_object)
+    return git_proxy.get_repo(path).tree(branch).traverse(predicate=should_process_git_object)
 
 
 def parse_commit_range(commit_range: str, path: str) -> Tuple[str, str]:
     from_commit_rev = None
     to_commit_rev = None
 
-    for commit in Repo(path).iter_commits(rev=commit_range):
+    for commit in git_proxy.get_repo(path).iter_commits(rev=commit_range):
         if not to_commit_rev:
             to_commit_rev = commit.hexsha
         from_commit_rev = commit.hexsha
 
     return from_commit_rev, to_commit_rev
 
 
@@ -48,15 +47,15 @@
 
 def get_pre_commit_modified_documents(
     progress_bar: 'BaseProgressBar', progress_bar_section: 'ProgressBarSection'
 ) -> Tuple[List[Document], List[Document]]:
     git_head_documents = []
     pre_committed_documents = []
 
-    repo = Repo(os.getcwd())
+    repo = git_proxy.get_repo(os.getcwd())
     diff_files = repo.index.diff(consts.GIT_HEAD_COMMIT_REV, create_patch=True, R=True)
     progress_bar.set_section_length(progress_bar_section, len(diff_files))
     for file in diff_files:
         progress_bar.update(progress_bar_section)
 
         diff_file_path = get_diff_file_path(file)
         file_path = get_path_by_os(diff_file_path)
@@ -78,15 +77,15 @@
     path: str,
     from_commit_rev: str,
     to_commit_rev: str,
 ) -> Tuple[List[Document], List[Document]]:
     from_commit_documents = []
     to_commit_documents = []
 
-    repo = Repo(path)
+    repo = git_proxy.get_repo(path)
     diff = repo.commit(from_commit_rev).diff(to_commit_rev)
 
     modified_files_diff = [
         change for change in diff if change.change_type != consts.COMMIT_DIFF_DELETED_FILE_CHANGE_TYPE
     ]
     progress_bar.set_section_length(progress_bar_section, len(modified_files_diff))
     for blob in modified_files_diff:
@@ -127,14 +126,15 @@
     _, end_commit, _ = update_details.split()
     return end_commit
 
 
 def _get_oldest_unupdated_commit_for_branch(commit: str) -> Optional[str]:
     # get a list of commits by chronological order that are not in the remote repository yet
     # more info about rev-list command: https://git-scm.com/docs/git-rev-list
-    not_updated_commits = Repo(os.getcwd()).git.rev_list(commit, '--topo-order', '--reverse', '--not', '--all')
+    repo = git_proxy.get_repo(os.getcwd())
+    not_updated_commits = repo.git.rev_list(commit, '--topo-order', '--reverse', '--not', '--all')
 
     commits = not_updated_commits.splitlines()
     if not commits:
         return None
 
     return commits[0]
```

### Comparing `cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py` & `cycode-1.9.6.dev4/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py` & `cycode-1.9.6.dev4/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py` & `cycode-1.9.6.dev4/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/files_collector/sca/sca_code_scanner.py` & `cycode-1.9.6.dev4/cycode/cli/files_collector/sca/sca_code_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 import click
-from git import GitCommandError, Repo
 
 from cycode.cli import consts
 from cycode.cli.files_collector.sca.maven.restore_gradle_dependencies import RestoreGradleDependencies
 from cycode.cli.files_collector.sca.maven.restore_maven_dependencies import RestoreMavenDependencies
 from cycode.cli.models import Document
+from cycode.cli.utils.git_proxy import git_proxy
 from cycode.cli.utils.path_utils import get_file_content, get_file_dir, join_paths
 from cycode.cyclient import logger
 
 if TYPE_CHECKING:
+    from git import Repo
+
     from cycode.cli.files_collector.sca.maven.base_restore_maven_dependencies import BaseRestoreMavenDependencies
 
 BUILD_GRADLE_FILE_NAME = 'build.gradle'
 BUILD_GRADLE_KTS_FILE_NAME = 'build.gradle.kts'
 BUILD_GRADLE_DEP_TREE_FILE_NAME = 'gradle-dependencies-generated.txt'
 BUILD_GRADLE_DEP_TREE_TIMEOUT = 180
 
@@ -23,44 +25,44 @@
 def perform_pre_commit_range_scan_actions(
     path: str,
     from_commit_documents: List[Document],
     from_commit_rev: str,
     to_commit_documents: List[Document],
     to_commit_rev: str,
 ) -> None:
-    repo = Repo(path)
+    repo = git_proxy.get_repo(path)
     add_ecosystem_related_files_if_exists(from_commit_documents, repo, from_commit_rev)
     add_ecosystem_related_files_if_exists(to_commit_documents, repo, to_commit_rev)
 
 
 def perform_pre_hook_range_scan_actions(
     git_head_documents: List[Document], pre_committed_documents: List[Document]
 ) -> None:
-    repo = Repo(os.getcwd())
+    repo = git_proxy.get_repo(os.getcwd())
     add_ecosystem_related_files_if_exists(git_head_documents, repo, consts.GIT_HEAD_COMMIT_REV)
     add_ecosystem_related_files_if_exists(pre_committed_documents)
 
 
 def add_ecosystem_related_files_if_exists(
-    documents: List[Document], repo: Optional[Repo] = None, commit_rev: Optional[str] = None
+    documents: List[Document], repo: Optional['Repo'] = None, commit_rev: Optional[str] = None
 ) -> None:
     documents_to_add: List[Document] = []
     for doc in documents:
         ecosystem = get_project_file_ecosystem(doc)
         if ecosystem is None:
             logger.debug('Failed to resolve project file ecosystem: %s', doc.path)
             continue
 
         documents_to_add.extend(get_doc_ecosystem_related_project_files(doc, documents, ecosystem, commit_rev, repo))
 
     documents.extend(documents_to_add)
 
 
 def get_doc_ecosystem_related_project_files(
-    doc: Document, documents: List[Document], ecosystem: str, commit_rev: Optional[str], repo: Optional[Repo]
+    doc: Document, documents: List[Document], ecosystem: str, commit_rev: Optional[str], repo: Optional['Repo']
 ) -> List[Document]:
     documents_to_add: List[Document] = []
     for ecosystem_project_file in consts.PROJECT_FILES_BY_ECOSYSTEM_MAP.get(ecosystem):
         file_to_search = join_paths(get_file_dir(doc.path), ecosystem_project_file)
         if not is_project_file_exists_in_documents(documents, file_to_search):
             if repo:
                 file_content = get_file_content_from_commit(repo, commit_rev, file_to_search)
@@ -132,18 +134,18 @@
     ]
 
 
 def get_manifest_file_path(document: Document, is_monitor_action: bool, project_path: str) -> str:
     return join_paths(project_path, document.path) if is_monitor_action else document.path
 
 
-def get_file_content_from_commit(repo: Repo, commit: str, file_path: str) -> Optional[str]:
+def get_file_content_from_commit(repo: 'Repo', commit: str, file_path: str) -> Optional[str]:
     try:
         return repo.git.show(f'{commit}:{file_path}')
-    except GitCommandError:
+    except git_proxy.get_git_command_error():
         return None
 
 
 def perform_pre_scan_documents_actions(
     context: click.Context, scan_type: str, documents_to_scan: List[Document], is_git_diff: bool = False
 ) -> None:
     if scan_type == consts.SCA_SCAN_TYPE and not context.obj.get(consts.SCA_SKIP_RESTORE_DEPENDENCIES_FLAG):
```

### Comparing `cycode-1.9.6.dev3/cycode/cli/files_collector/zip_documents.py` & `cycode-1.9.6.dev4/cycode/cli/files_collector/zip_documents.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/models.py` & `cycode-1.9.6.dev4/cycode/cli/models.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/printers/console_printer.py` & `cycode-1.9.6.dev4/cycode/cli/printers/console_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/printers/json_printer.py` & `cycode-1.9.6.dev4/cycode/cli/printers/json_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/printers/printer_base.py` & `cycode-1.9.6.dev4/cycode/cli/printers/printer_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,14 @@
         Note:
             Called only when the verbose flag is set.
         """
         if e is None:
             # gets the most recent exception caught by an except clause
             message = f'Error: {traceback.format_exc()}'
         else:
-            traceback_message = ''.join(traceback.format_exception(e))
+            traceback_message = ''.join(traceback.format_exception(None, e, e.__traceback__))
             message = f'Error: {traceback_message}'
 
         click.secho(message, err=True, fg=self.RED_COLOR_NAME)
 
         correlation_message = f'Correlation ID: {get_correlation_id()}'
         click.secho(correlation_message, err=True, fg=self.RED_COLOR_NAME)
```

### Comparing `cycode-1.9.6.dev3/cycode/cli/printers/tables/sca_table_printer.py` & `cycode-1.9.6.dev4/cycode/cli/printers/tables/sca_table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/printers/tables/table.py` & `cycode-1.9.6.dev4/cycode/cli/printers/tables/table.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/printers/tables/table_printer.py` & `cycode-1.9.6.dev4/cycode/cli/printers/tables/table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/printers/tables/table_printer_base.py` & `cycode-1.9.6.dev4/cycode/cli/printers/tables/table_printer_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/printers/text_printer.py` & `cycode-1.9.6.dev4/cycode/cli/printers/text_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/user_settings/base_file_manager.py` & `cycode-1.9.6.dev4/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/user_settings/config_file_manager.py` & `cycode-1.9.6.dev4/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/user_settings/configuration_manager.py` & `cycode-1.9.6.dev4/cycode/cli/user_settings/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/user_settings/credentials_manager.py` & `cycode-1.9.6.dev4/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/user_settings/jwt_creator.py` & `cycode-1.9.6.dev4/cycode/cli/user_settings/jwt_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/utils/get_api_client.py` & `cycode-1.9.6.dev4/cycode/cli/utils/get_api_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/utils/path_utils.py` & `cycode-1.9.6.dev4/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/utils/progress_bar.py` & `cycode-1.9.6.dev4/cycode/cli/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/utils/scan_batch.py` & `cycode-1.9.6.dev4/cycode/cli/utils/scan_batch.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/utils/shell_executor.py` & `cycode-1.9.6.dev4/cycode/cli/utils/shell_executor.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/utils/string_utils.py` & `cycode-1.9.6.dev4/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/utils/task_timer.py` & `cycode-1.9.6.dev4/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cli/utils/yaml_utils.py` & `cycode-1.9.6.dev4/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cyclient/auth_client.py` & `cycode-1.9.6.dev4/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cyclient/client_creator.py` & `cycode-1.9.6.dev4/cycode/cyclient/client_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cyclient/config.py` & `cycode-1.9.6.dev4/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cyclient/cycode_client_base.py` & `cycode-1.9.6.dev4/cycode/cyclient/cycode_client_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cyclient/cycode_dev_based_client.py` & `cycode-1.9.6.dev4/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cyclient/cycode_token_based_client.py` & `cycode-1.9.6.dev4/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cyclient/headers.py` & `cycode-1.9.6.dev4/cycode/cyclient/headers.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cyclient/models.py` & `cycode-1.9.6.dev4/cycode/cyclient/models.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cyclient/report_client.py` & `cycode-1.9.6.dev4/cycode/cyclient/report_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cyclient/scan_client.py` & `cycode-1.9.6.dev4/cycode/cyclient/scan_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/cycode/cyclient/scan_config_base.py` & `cycode-1.9.6.dev4/cycode/cyclient/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev3/pyproject.toml` & `cycode-1.9.6.dev4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "1.9.6.dev3" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "1.9.6.dev4" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Boost security in your dev lifecycle via SAST, SCA, Secrets & IaC scanning."
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq/cycode-cli"
 readme = "README.md"
 classifiers = [
```

### Comparing `cycode-1.9.6.dev3/PKG-INFO` & `cycode-1.9.6.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 1.9.6.dev3
+Version: 1.9.6.dev4
 Summary: Boost security in your dev lifecycle via SAST, SCA, Secrets & IaC scanning.
 Home-page: https://github.com/cycodehq/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.13
```

