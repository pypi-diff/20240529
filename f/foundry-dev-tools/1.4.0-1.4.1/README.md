# Comparing `tmp/foundry-dev-tools-1.4.0.tar.gz` & `tmp/foundry_dev_tools-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundry-dev-tools-1.4.0.tar", last modified: Mon Feb  5 17:03:31 2024, max compression
+gzip compressed data, was "foundry_dev_tools-1.4.1.tar", last modified: Wed May 29 20:24:46 2024, max compression
```

## Comparing `foundry-dev-tools-1.4.0.tar` & `foundry_dev_tools-1.4.1.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.089458 foundry-dev-tools-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.069458 foundry-dev-tools-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.073458 foundry-dev-tools-1.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/.github/ISSUE_TEMPLATE/blank_issue.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.073458 foundry-dev-tools-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11361 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-02-05 17:03:31.089458 foundry-dev-tools-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.073458 foundry-dev-tools-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/Configuration_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/FoundryFileSystem_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/FoundryRestClient_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/SSO_usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.073458 foundry-dev-tools-1.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/architecture.md
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/contributors.md
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/develop.md
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.077458 foundry-dev-tools-1.4.0/docs/pictures/
--rw-r--r--   0 runner    (1001) docker     (127)    28579 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/pictures/mermaid-diagram-already-cached-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    33149 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/pictures/mermaid-diagram-already-cached-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)    35104 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/pictures/mermaid-diagram-new-transaction-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    41514 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/pictures/mermaid-diagram-new-transaction-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)    87463 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/pictures/tpa_config.png
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/s3.md
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/docs/usage_and_examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 17:03:31.089458 foundry-dev-tools-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.069458 foundry-dev-tools-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.077458 foundry-dev-tools-1.4.0/src/foundry_dev_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14644 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/cached_foundry_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.081458 foundry-dev-tools-1.4.0/src/foundry_dev_tools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12754 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/cli/info.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/cli/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    11548 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    95673 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/foundry_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20215 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/fsspec_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.081458 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/async_s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.081458 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/caches/metadata_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/caches/spark_caches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.081458 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/converter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/converter/foundry_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/token_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.089458 foundry-dev-tools-1.4.0/src/foundry_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-02-05 17:03:31.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-05 17:03:31.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 17:03:31.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-05 17:03:31.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 17:03:30.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-05 17:03:31.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-05 17:03:31.000000 foundry-dev-tools-1.4.0/src/foundry_dev_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.081458 foundry-dev-tools-1.4.0/src/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.085458 foundry-dev-tools-1.4.0/src/transforms/api/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/transforms/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/transforms/api/_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/transforms/api/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/transforms/api/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17933 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/src/transforms/api/_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.089458 foundry-dev-tools-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    23741 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/foundry_mock_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18409 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_cached_foundry_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_cached_foundry_client_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_cli_build.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_cli_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.069458 foundry-dev-tools-1.4.0/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.089458 foundry-dev-tools-1.4.0/tests/test_data/binary_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_data/binary_dataset/bin
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 17:03:31.089458 foundry-dev-tools-1.4.0/tests/test_data/iris/
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_data/iris/iris.csv
--rw-r--r--   0 runner    (1001) docker     (127)    30233 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_foundry_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_foundry_local_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_foundry_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    17648 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_foundry_spark_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14379 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_foundry_sql_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33976 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_fsspec_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_multipass_tpa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    14859 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_spark_caches.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_token_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_transforms_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/test_utils_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-02-05 17:02:40.000000 foundry-dev-tools-1.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.262050 foundry_dev_tools-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.242049 foundry_dev_tools-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.246050 foundry_dev_tools-1.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/.github/ISSUE_TEMPLATE/blank_issue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.246050 foundry_dev_tools-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11361 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-29 20:24:46.262050 foundry_dev_tools-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.246050 foundry_dev_tools-1.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/Configuration_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/FoundryFileSystem_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/FoundryRestClient_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/SSO_usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.246050 foundry_dev_tools-1.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/contributors.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/develop.md
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.250049 foundry_dev_tools-1.4.1/docs/pictures/
+-rw-r--r--   0 runner    (1001) docker     (127)    28579 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/pictures/mermaid-diagram-already-cached-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    33149 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/pictures/mermaid-diagram-already-cached-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    35104 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/pictures/mermaid-diagram-new-transaction-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    41514 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/pictures/mermaid-diagram-new-transaction-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    87463 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/pictures/tpa_config.png
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/s3.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/docs/usage_and_examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:24:46.262050 foundry_dev_tools-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.242049 foundry_dev_tools-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.250049 foundry_dev_tools-1.4.1/src/foundry_dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14644 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/cached_foundry_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.254049 foundry_dev_tools-1.4.1/src/foundry_dev_tools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12754 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/cli/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11548 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96192 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/foundry_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20215 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/fsspec_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.254049 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/async_s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.254049 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/caches/metadata_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/caches/spark_caches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.254049 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/converter/foundry_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/token_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.262050 foundry_dev_tools-1.4.1/src/foundry_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-29 20:24:46.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-29 20:24:46.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:24:46.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 20:24:46.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:24:45.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-29 20:24:46.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-29 20:24:46.000000 foundry_dev_tools-1.4.1/src/foundry_dev_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.254049 foundry_dev_tools-1.4.1/src/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.254049 foundry_dev_tools-1.4.1/src/transforms/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/transforms/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/transforms/api/_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/transforms/api/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/transforms/api/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17933 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/src/transforms/api/_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.262050 foundry_dev_tools-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23741 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/foundry_mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18409 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_cached_foundry_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_cached_foundry_client_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15871 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_cli_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_cli_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.242049 foundry_dev_tools-1.4.1/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.262050 foundry_dev_tools-1.4.1/tests/test_data/binary_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_data/binary_dataset/bin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:24:46.262050 foundry_dev_tools-1.4.1/tests/test_data/iris/
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_data/iris/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    30351 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_foundry_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_foundry_local_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_foundry_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17648 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_foundry_spark_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14379 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_foundry_sql_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33976 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_fsspec_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_multipass_tpa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14859 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_spark_caches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_transforms_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/test_utils_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-29 20:23:57.000000 foundry_dev_tools-1.4.1/tox.ini
```

### Comparing `foundry-dev-tools-1.4.0/.github/ISSUE_TEMPLATE/blank_issue.yml` & `foundry_dev_tools-1.4.1/.github/ISSUE_TEMPLATE/blank_issue.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `foundry_dev_tools-1.4.1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `foundry_dev_tools-1.4.1/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/.github/pull_request_template.md` & `foundry_dev_tools-1.4.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/.github/workflows/ci.yml` & `foundry_dev_tools-1.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/.github/workflows/docs.yml` & `foundry_dev_tools-1.4.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/.gitignore` & `foundry_dev_tools-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/.pre-commit-config.yaml` & `foundry_dev_tools-1.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/LICENSE` & `foundry_dev_tools-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/PKG-INFO` & `foundry_dev_tools-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry-dev-tools
-Version: 1.4.0
+Version: 1.4.1
 Summary: Seamlessly run your Palantir Foundry Repository transforms code on your local machine.
 Author-email: Nicolas Renkamp <nicolas.renkamp@merckgroup.com>, Jonas Wunderlich <jonas.wunderlich@merckgroup.com>
 License: Apache-2.0
 Project-URL: Homepage, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Documentation, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Source, https://github.com/emdgroup/foundry-dev-tools
 Project-URL: Tracker, https://github.com/emdgroup/foundry-dev-tools/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.4.0 Summary:
+Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.4.1 Summary:
 Seamlessly run your Palantir Foundry Repository transforms code on your local
 machine. Author-email: Nicolas Renkamp
 merckgroup.com>, Jonas Wunderlich
 merckgroup.com> License: Apache-2.0 Project-URL: Homepage, https://
 emdgroup.github.io/foundry-dev-tools Project-URL: Documentation, https://
 emdgroup.github.io/foundry-dev-tools Project-URL: Source, https://github.com/
 emdgroup/foundry-dev-tools Project-URL: Tracker, https://github.com/emdgroup/
```

### Comparing `foundry-dev-tools-1.4.0/README.md` & `foundry_dev_tools-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/FoundryFileSystem_usage.md` & `foundry_dev_tools-1.4.1/docs/FoundryFileSystem_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/FoundryRestClient_usage.md` & `foundry_dev_tools-1.4.1/docs/FoundryRestClient_usage.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,21 +30,21 @@
 
 Upload the complete content of a local folder to a dataset in Foundry
 
 ```python
 import os
 from foundry_dev_tools import FoundryRestClient
 
-upload_folder = "/path/to/folder-to-upload"
-target_dataset_path = "/paht/to/test_folder_upload"
+upload_folder = "/local-path/to/folder-to-upload"
+target_dataset_path = "/path/to/foundry-dataset"
+
+file_paths = [file for file in Path(upload_folder).rglob("*") if file.is_file() and not file.name.startswith(".")]
+dataset_paths_in_foundry = [str(file_path.relative_to(upload_folder)) for file_path in file_paths]
+path_file_dict = dict(zip(dataset_paths_in_foundry, file_paths))
 
-filenames = os.listdir(upload_folder)
-filepaths = list(map(lambda file: os.sep.join([upload_folder, file]), filenames))
-dataset_paths_in_foundry = list(map(lambda file: file, filenames))
-path_file_dict = dict(zip(dataset_paths_in_foundry, filepaths))
 rest_client = FoundryRestClient()
 dataset_rid = rest_client.get_dataset_rid(dataset_path=target_dataset_path)
 transaction_rid = rest_client.open_transaction(dataset_rid=dataset_rid,
                                                mode='UPDATE',
                                                branch='master')
 rest_client.upload_dataset_files(dataset_rid=dataset_rid,
                                  transaction_rid=transaction_rid,
```

### Comparing `foundry-dev-tools-1.4.0/docs/SSO_usage.md` & `foundry_dev_tools-1.4.1/docs/SSO_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/architecture.md` & `foundry_dev_tools-1.4.1/docs/architecture.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/changelog.md` & `foundry_dev_tools-1.4.1/docs/changelog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog],
 and this project adheres to [Semantic Versioning].
 
+## [1.4.1] - 2024-05-29
+
+## Added
+  - Support for git submodules (#56)
+
 ## [1.4.0] - 2024-02-05
 
 ## Added
 
 - support for lightweight transforms (#47)
 
 ## Fixed
@@ -195,15 +200,17 @@
 ## [1.0] - 2023-02-28 [YANKED]
 
 - First public Open Source Release of Foundry DevTools.
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/spec/v2.0.0.html
 
-[1.3.4]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.3.4...v1.3.5
+[1.4.1]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.4.0...v1.4.1
+[1.4.0]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.3.5...v1.4.0
+[1.3.5]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.3.4...v1.3.5
 [1.3.4]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.3.3...v1.3.4
 [1.3.3]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.3.2...v1.3.3
 [1.3.2]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.3.1...v1.3.2
 [1.3.1]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.3...v1.3.1
 [1.3]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.2...v1.3
 [1.2]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.1...v1.2
 [1.1]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.12...v1.1
```

### Comparing `foundry-dev-tools-1.4.0/docs/cli.md` & `foundry_dev_tools-1.4.1/docs/cli.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/conf.py` & `foundry_dev_tools-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/develop.md` & `foundry_dev_tools-1.4.1/docs/develop.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/index.md` & `foundry_dev_tools-1.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/installation.md` & `foundry_dev_tools-1.4.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/pictures/mermaid-diagram-already-cached-dark.svg` & `foundry_dev_tools-1.4.1/docs/pictures/mermaid-diagram-already-cached-dark.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/pictures/mermaid-diagram-already-cached-light.svg` & `foundry_dev_tools-1.4.1/docs/pictures/mermaid-diagram-already-cached-light.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/pictures/mermaid-diagram-new-transaction-dark.svg` & `foundry_dev_tools-1.4.1/docs/pictures/mermaid-diagram-new-transaction-dark.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/pictures/mermaid-diagram-new-transaction-light.svg` & `foundry_dev_tools-1.4.1/docs/pictures/mermaid-diagram-new-transaction-light.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/pictures/tpa_config.png` & `foundry_dev_tools-1.4.1/docs/pictures/tpa_config.png`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/s3.md` & `foundry_dev_tools-1.4.1/docs/s3.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/docs/usage_and_examples.md` & `foundry_dev_tools-1.4.1/docs/usage_and_examples.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/pyproject.toml` & `foundry_dev_tools-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/setup.py` & `foundry_dev_tools-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/cached_foundry_client.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/cached_foundry_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/cli/build.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/cli/build.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/cli/info.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/cli/info.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/cli/s3.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/cli/s3.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/config.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/config.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/foundry_api_client.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/foundry_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,14 +319,32 @@
             "POST",
             f"{self.catalog}/catalog/datasets/{dataset_rid}/branchesUpdate2/{quote_plus(branch)}",
             data=f'"{parent_branch}"',
         )
         _raise_for_status_verbose(response)
         return response.json()
 
+    def get_branches(self, dataset_rid: str) -> list[str]:
+        """Returns a list of branches available a dataset.
+
+        Args:
+            dataset_rid (str): Unique identifier of the dataset
+
+        Returns:
+            list[str]:
+                with keys id (name) the dataset branches
+
+        """
+        response = self._request(
+            "GET",
+            f"{self.catalog}/catalog/datasets/{dataset_rid}/branches2",
+        )
+        _raise_for_status_verbose(response)
+        return response.json()
+
     def get_branch(self, dataset_rid: str, branch: str) -> dict:
         """Returns branch information.
 
         Args:
             dataset_rid (str): Unique identifier of the dataset
             branch (str): Branch name
```

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/fsspec_impl.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/fsspec_impl.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/async_s3.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/async_s3.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/caches/metadata_store.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/caches/metadata_store.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/caches/spark_caches.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/caches/spark_caches.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/converter/foundry_spark.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/converter/foundry_spark.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/importer.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/importer.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/misc.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/repo.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,18 +109,18 @@
                 ["git", "rev-parse", "--show-toplevel"], cwd=git_dir
             )
             .decode("utf-8")
             .strip()
         )
     if git_dir is None:
         git_dir = Path.cwd()
-    if git_dir.joinpath(".git").is_dir():
+    if git_dir.joinpath(".git").exists():
         return git_dir
     for p in git_dir.resolve().parents:
-        if p.joinpath(".git").is_dir():
+        if p.joinpath(".git").exists():
             return p
     return None
 
 
 def find_project_config_file(
     project_directory: "Path | None" = None, use_git: bool = False
 ) -> "Path | None":
```

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/s3.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/s3.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/spark.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/spark.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools/utils/token_provider.py` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools/utils/token_provider.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools.egg-info/PKG-INFO` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry-dev-tools
-Version: 1.4.0
+Version: 1.4.1
 Summary: Seamlessly run your Palantir Foundry Repository transforms code on your local machine.
 Author-email: Nicolas Renkamp <nicolas.renkamp@merckgroup.com>, Jonas Wunderlich <jonas.wunderlich@merckgroup.com>
 License: Apache-2.0
 Project-URL: Homepage, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Documentation, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Source, https://github.com/emdgroup/foundry-dev-tools
 Project-URL: Tracker, https://github.com/emdgroup/foundry-dev-tools/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.4.0 Summary:
+Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.4.1 Summary:
 Seamlessly run your Palantir Foundry Repository transforms code on your local
 machine. Author-email: Nicolas Renkamp
 merckgroup.com>, Jonas Wunderlich
 merckgroup.com> License: Apache-2.0 Project-URL: Homepage, https://
 emdgroup.github.io/foundry-dev-tools Project-URL: Documentation, https://
 emdgroup.github.io/foundry-dev-tools Project-URL: Source, https://github.com/
 emdgroup/foundry-dev-tools Project-URL: Tracker, https://github.com/emdgroup/
```

### Comparing `foundry-dev-tools-1.4.0/src/foundry_dev_tools.egg-info/SOURCES.txt` & `foundry_dev_tools-1.4.1/src/foundry_dev_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/transforms/api/__init__.py` & `foundry_dev_tools-1.4.1/src/transforms/api/__init__.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/transforms/api/_configure.py` & `foundry_dev_tools-1.4.1/src/transforms/api/_configure.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/transforms/api/_dataset.py` & `foundry_dev_tools-1.4.1/src/transforms/api/_dataset.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/transforms/api/_decorators.py` & `foundry_dev_tools-1.4.1/src/transforms/api/_decorators.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/src/transforms/api/_transform.py` & `foundry_dev_tools-1.4.1/src/transforms/api/_transform.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/conftest.py` & `foundry_dev_tools-1.4.1/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -202,7 +202,18 @@
         ) = generic_upload_dataset_if_not_exists(
             client,
             name=DATASET_NAME,
             upload_folder=tmpdir,
             foundry_schema=FOUNDRY_SCHEMA_COMPLEX_DATASET,
         )
         yield ds_rid
+
+
+@pytest.fixture()
+def git_env():
+    return {
+        "GIT_CONFIG_NOSYSTEM": "1",
+        "GIT_COMMITTER_NAME": "Jon Doe",
+        "GIT_COMMITTER_EMAIL": "john@doe",
+        "GIT_AUTHOR_NAME": "Jon Doe",
+        "GIT_AUTHOR_EMAIL": "john@doe",
+    }
```

### Comparing `foundry-dev-tools-1.4.0/tests/foundry_mock_client.py` & `foundry_dev_tools-1.4.1/tests/foundry_mock_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_cached_foundry_client.py` & `foundry_dev_tools-1.4.1/tests/test_cached_foundry_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_cached_foundry_client_integration.py` & `foundry_dev_tools-1.4.1/tests/test_cached_foundry_client_integration.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_cli_build.py` & `foundry_dev_tools-1.4.1/tests/test_cli_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,50 +450,42 @@
             "Build status: SUCCEEDEDLink to the foundry build: https://test_build.url/workspace/data-integration/job-tr"
             "acker/builds/ri.foundry.main.build.0e7ca16b-49f1-4b2d-953e-21b18bc7c560The resulting dataset(s):https://te"
             "st_build.url/workspace/data-integration/dataset/preview/ri.foundry.main.dataset.81d943dd-8b84-46ba-b720-5e227de8bb6a/dev%2Fbranch"
         )
         assert result.exit_code == 0
 
 
-def test_get_transform_files(tmpdir: "py.path.LocalPath"):
-    GIT_ENV = {
-        "HOME": str(tmpdir),
-        "GIT_CONFIG_NOSYSTEM": "1",
-        "GIT_COMMITTER_NAME": "pytest get_transform_files test",
-        "GIT_COMMITTER_EMAIL": "pytest@get_transform_files.py",
-        "GIT_AUTHOR_NAME": "pytest get_transform_files test",
-        "GIT_AUTHOR_EMAIL": "pytest@get_transform_files.py",
-    }  # should use default configs
+def test_get_transform_files(tmpdir: "py.path.LocalPath", git_env: dict):
     with tmpdir.as_cwd():
         from foundry_dev_tools.cli.build import (
             TRANSFORM_DECORATORS,
             get_transform_files,
             is_transform_file,
         )
 
-        subprocess.check_call(["git", "init"], env=GIT_ENV)
+        subprocess.check_call(["git", "init"], env=git_env)
         t = Path("transforms-python", "examples")
         t.mkdir(parents=True)
         tfiles = []
         for decorator in TRANSFORM_DECORATORS:
             transform_file = t.joinpath(f"{decorator}.py")
             with transform_file.open("w+") as tfile:
                 tfile.write(
                     f"from transforms.api import {decorator},Output\n\n@transform_df()\ndef test_transform():\n    pass"
                 )
             tfiles.append(transform_file.as_posix())  # git returns with forward slash
-        subprocess.check_call(["git", "add", "-A"], env=GIT_ENV)
-        subprocess.check_call(["git", "commit", "-m", "transform commit"], env=GIT_ENV)
+        subprocess.check_call(["git", "add", "-A"], env=git_env)
+        subprocess.check_call(["git", "commit", "-m", "transform commit"], env=git_env)
 
         for f in tfiles:
             assert is_transform_file(Path(f))
 
         assert not is_transform_file(Path("does not exist"))
         assert get_transform_files(Path.cwd()) == tfiles
         with tmpdir.join("get_transform.txt").open("w+") as gttxt:
             gttxt.write("something something")
-        subprocess.check_call(["git", "add", "-A"], env=GIT_ENV)
+        subprocess.check_call(["git", "add", "-A"], env=git_env)
         subprocess.check_call(
-            ["git", "commit", "-m", "no transform in last commit"], env=GIT_ENV
+            ["git", "commit", "-m", "no transform in last commit"], env=git_env
         )
         with pytest.raises(UsageError, match="No transform files in the last commit."):
             get_transform_files(Path.cwd())
```

### Comparing `foundry-dev-tools-1.4.0/tests/test_config.py` & `foundry_dev_tools-1.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_data/binary_dataset/bin` & `foundry_dev_tools-1.4.1/tests/test_data/binary_dataset/bin`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_data/iris/iris.csv` & `foundry_dev_tools-1.4.1/tests/test_data/iris/iris.csv`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_foundry_api.py` & `foundry_dev_tools-1.4.1/tests/test_foundry_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,17 @@
         client.get_branch(ds["rid"], BRANCH)
 
     branch = client.create_branch(ds["rid"], BRANCH)
     with pytest.raises(BranchesAlreadyExistError):
         _ = client.create_branch(ds["rid"], BRANCH)
     branch_returned = client.get_branch(ds["rid"], BRANCH)
     assert branch == branch_returned
+    branch_list = client.get_branches(ds["rid"])
+    assert len(branch_list) == 1
+    assert branch_list[0] == BRANCH
 
     assert client.get_dataset_identity(ds["rid"], BRANCH) == {
         "dataset_path": dataset_path,
         "dataset_rid": ds["rid"],
         "last_transaction_rid": None,
         "last_transaction": None,
     }
```

### Comparing `foundry-dev-tools-1.4.0/tests/test_foundry_local_deprecation.py` & `foundry_dev_tools-1.4.1/tests/test_foundry_local_deprecation.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_foundry_mock.py` & `foundry_dev_tools-1.4.1/tests/test_foundry_mock.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_foundry_spark_converters.py` & `foundry_dev_tools-1.4.1/tests/test_foundry_spark_converters.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_foundry_sql_client.py` & `foundry_dev_tools-1.4.1/tests/test_foundry_sql_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_fsspec_impl.py` & `foundry_dev_tools-1.4.1/tests/test_fsspec_impl.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_multipass_tpa.py` & `foundry_dev_tools-1.4.1/tests/test_multipass_tpa.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_s3.py` & `foundry_dev_tools-1.4.1/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_spark_caches.py` & `foundry_dev_tools-1.4.1/tests/test_spark_caches.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_token_provider.py` & `foundry_dev_tools-1.4.1/tests/test_token_provider.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_transforms.py` & `foundry_dev_tools-1.4.1/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/test_transforms_integration.py` & `foundry_dev_tools-1.4.1/tests/test_transforms_integration.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tests/utils.py` & `foundry_dev_tools-1.4.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.4.0/tox.ini` & `foundry_dev_tools-1.4.1/tox.ini`

 * *Files identical despite different names*

