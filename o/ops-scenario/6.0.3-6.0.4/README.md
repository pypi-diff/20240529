# Comparing `tmp/ops-scenario-6.0.3.tar.gz` & `tmp/ops_scenario-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-scenario-6.0.3.tar", last modified: Tue Mar 19 10:40:22 2024, max compression
+gzip compressed data, was "ops_scenario-6.0.4.tar", last modified: Wed May 29 07:31:10 2024, max compression
```

## Comparing `ops-scenario-6.0.3.tar` & `ops_scenario-6.0.4.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 10:40:22.601220 ops-scenario-6.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 10:40:22.589220 ops-scenario-6.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 10:40:22.593220 ops-scenario-6.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/.github/workflows/build_wheels.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/.github/workflows/quality_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    50684 2024-03-19 10:40:22.601220 ops-scenario-6.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 10:40:22.601220 ops-scenario-6.0.3/ops_scenario.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50684 2024-03-19 10:40:22.000000 ops-scenario-6.0.3/ops_scenario.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-19 10:40:22.000000 ops-scenario-6.0.3/ops_scenario.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 10:40:22.000000 ops-scenario-6.0.3/ops_scenario.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-19 10:40:22.000000 ops-scenario-6.0.3/ops_scenario.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-19 10:40:22.000000 ops-scenario-6.0.3/ops_scenario.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 10:40:22.593220 ops-scenario-6.0.3/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    50386 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/resources/state-transition-model.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 10:40:22.597220 ops-scenario-6.0.3/scenario/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/scenario/capture_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    18208 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/scenario/consistency_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    21173 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/scenario/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/scenario/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    24384 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/scenario/mocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/scenario/ops_main_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/scenario/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/scenario/sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)    51869 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/scenario/state.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/scenario/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 10:40:22.601220 ops-scenario-6.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 10:40:22.597220 ops-scenario-6.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_charm_spec_autoload.py
--rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_consistency_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_dcbase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 10:40:22.601220 ops-scenario-6.0.3/tests/test_e2e/
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_builtin_scenes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_custom_event_triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_event_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_juju_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_pebble.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_play_assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_rubbish_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    17410 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_stored_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_e2e/test_vroot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_emitted_events_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-19 10:40:17.000000 ops-scenario-6.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:10.353174 ops_scenario-6.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:10.341174 ops_scenario-6.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:10.345174 ops_scenario-6.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/.github/workflows/build_wheels.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/.github/workflows/quality_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    51221 2024-05-29 07:31:10.353174 ops_scenario-6.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    50356 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:10.353174 ops_scenario-6.0.4/ops_scenario.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    51221 2024-05-29 07:31:10.000000 ops_scenario-6.0.4/ops_scenario.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-29 07:31:10.000000 ops_scenario-6.0.4/ops_scenario.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 07:31:10.000000 ops_scenario-6.0.4/ops_scenario.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 07:31:10.000000 ops_scenario-6.0.4/ops_scenario.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 07:31:10.000000 ops_scenario-6.0.4/ops_scenario.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:10.345174 ops_scenario-6.0.4/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    50386 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/resources/state-transition-model.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:10.349174 ops_scenario-6.0.4/scenario/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/scenario/capture_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/scenario/consistency_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21173 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/scenario/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/scenario/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24646 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/scenario/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/scenario/ops_main_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/scenario/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/scenario/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54197 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/scenario/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/scenario/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 07:31:10.353174 ops_scenario-6.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:10.349174 ops_scenario-6.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_charm_spec_autoload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16195 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_consistency_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_dcbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:10.353174 ops_scenario-6.0.4/tests/test_e2e/
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_builtin_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_cloud_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_custom_event_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_event_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_juju_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_pebble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_play_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_rubbish_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17371 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_stored_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_e2e/test_vroot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_emitted_events_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-29 07:31:00.000000 ops_scenario-6.0.4/tox.ini
```

### Comparing `ops-scenario-6.0.3/.github/workflows/build_wheels.yaml` & `ops_scenario-6.0.4/.github/workflows/build_wheels.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/.github/workflows/quality_checks.yaml` & `ops_scenario-6.0.4/.github/workflows/quality_checks.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/.pre-commit-config.yaml` & `ops_scenario-6.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/CONTRIBUTING.md` & `ops_scenario-6.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/LICENSE.txt` & `ops_scenario-6.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/PKG-INFO` & `ops_scenario-6.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-scenario
-Version: 6.0.3
+Version: 6.0.4
 Summary: Python library providing a state-transition testing API for Operator Framework charms.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/canonical/ops-scenario
 Project-URL: Bug Tracker, https://github.com/canonical/ops-scenario/issues
 Keywords: juju,test
 Classifier: Development Status :: 3 - Alpha
@@ -36,54 +36,54 @@
 event on the charm and execute its logic.
 
 This puts scenario tests somewhere in between unit and integration tests: some say 'functional', some say 'contract', I prefer 'state-transition'.
 
 Scenario tests nudge you into thinking of a charm as an input->output function. The input is the
 union of an `Event` (why am I, charm, being executed), a `State` (am I leader? what is my relation data? what is my
 config?...) and the charm's execution `Context` (what relations can I have? what containers can I have?...). The output is another `State`: the state after the charm has had a chance to interact with the
-mocked juju model and affect the initial state back.
+mocked Juju model and affect the initial state back.
 
 ![state transition model depiction](resources/state-transition-model.png)
 
 For example: a charm currently in `unknown` status is executed with a `start` event, and based on whether it has leadership or not (according to its input state), it will decide to set `active` or `blocked` status (which will be reflected in the output state).
 
 Scenario-testing a charm, then, means verifying that:
 
 - the charm does not raise uncaught exceptions while handling the event
 - the output state (or the diff with the input state) is as expected.
 
-# Core concepts as a metaphor
+## Core concepts as a metaphor
 
 I like metaphors, so here we go:
 
 - There is a theatre stage.
 - You pick an actor (a Charm) to put on the stage. Not just any actor: an improv one.
 - You arrange the stage with content that the actor will have to interact with. This consists of selecting:
     - An initial situation (`State`) in which the actor is, e.g. is the actor the main role or an NPC (`is_leader`), or what
       other actors are there around it, what is written in those pebble-shaped books on the table?
     - Something that has just happened (an `Event`) and to which the actor has to react (e.g. one of the NPCs leaves the
       stage (`relation-departed`), or the content of one of the books changes).
 - How the actor will react to the event will have an impact on the context: e.g. the actor might knock over a table (a
   container), or write something down into one of the books.
 
-# Core concepts not as a metaphor
+## Core concepts not as a metaphor
 
 Scenario tests are about running assertions on atomic state transitions treating the charm being tested like a black
 box. An initial state goes in, an event occurs (say, `'start'`) and a new state comes out. Scenario tests are about
 validating the transition, that is, consistency-checking the delta between the two states, and verifying the charm
 author's expectations.
 
 Comparing scenario tests with `Harness` tests:
 
 - Harness exposes an imperative API: the user is expected to call methods on the Harness driving it to the desired
   state, then verify its validity by calling charm methods or inspecting the raw data. In contrast, Scenario is declarative. You fully specify an initial state, an execution context and an event, then you run the charm and inspect the results.
 - Harness instantiates the charm once, then allows you to fire multiple events on the charm, which is breeding ground
   for subtle bugs. Scenario tests are centered around testing single state transitions, that is, one event at a time.
   This ensures that the execution environment is as clean as possible (for a unit test).
-- Harness maintains a model of the juju Model, which is a maintenance burden and adds complexity. Scenario mocks at the
+- Harness maintains a model of the Juju Model, which is a maintenance burden and adds complexity. Scenario mocks at the
   level of hook tools and stores all mocking data in a monolithic data structure (the State), which makes it more
   lightweight and portable.
 
 # Writing scenario tests
 
 A scenario test consists of three broad steps:
 
@@ -100,430 +100,422 @@
 
 The most basic scenario is one in which all is defaulted and barely any data is
 available. The charm has no config, no relations, no leadership, and its status is `unknown`.
 
 With that, we can write the simplest possible scenario test:
 
 ```python
-from scenario import State, Context, Event
-from ops.charm import CharmBase
-from ops.model import UnknownStatus
+import ops
+import scenario
 
 
-class MyCharm(CharmBase):
+class MyCharm(ops.CharmBase):
     pass
 
 
 def test_scenario_base():
-    ctx = Context(MyCharm, meta={"name": "foo"})
-    out = ctx.run(Event("start"), State())
-    assert out.unit_status == UnknownStatus()
+    ctx = scenario.Context(MyCharm, meta={"name": "foo"})
+    out = ctx.run(scenario.Event("start"), scenario.State())
+    assert out.unit_status == ops.UnknownStatus()
 ```
 
 Now let's start making it more complicated. Our charm sets a special state if it has leadership on 'start':
 
 ```python
+import ops
 import pytest
-from scenario import State, Context
-from ops.charm import CharmBase
-from ops.model import ActiveStatus
+import scenario
 
 
-class MyCharm(CharmBase):
-    def __init__(self, ...):
-        self.framework.observe(self.on.start, self._on_start)
+class MyCharm(ops.CharmBase):
+    def __init__(self, framework):
+        super().__init__(framework)
+        framework.observe(self.on.start, self._on_start)
 
     def _on_start(self, _):
         if self.unit.is_leader():
-            self.unit.status = ActiveStatus('I rule')
+            self.unit.status = ops.ActiveStatus('I rule')
         else:
-            self.unit.status = ActiveStatus('I am ruled')
+            self.unit.status = ops.ActiveStatus('I am ruled')
 
 
 @pytest.mark.parametrize('leader', (True, False))
 def test_status_leader(leader):
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-    out = ctx.run('start', State(leader=leader))
-    assert out.unit_status == ActiveStatus('I rule' if leader else 'I am ruled')
+    ctx = scenario.Context(MyCharm, meta={"name": "foo"})
+    out = ctx.run('start', scenario.State(leader=leader))
+    assert out.unit_status == ops.ActiveStatus('I rule' if leader else 'I am ruled')
 ```
 
 By defining the right state we can programmatically define what answers will the charm get to all the questions it can
-ask the juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
+ask the Juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
 
 ## Statuses
 
 One of the simplest types of black-box testing available to charmers is to execute the charm and verify that the charm
 sets the expected unit/application status. We have seen a simple example above including leadership. But what if the
 charm transitions through a sequence of statuses?
 
 ```python
-from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, BlockedStatus
+import ops
 
 
 # charm code:
 def _on_event(self, _event):
-    self.unit.status = MaintenanceStatus('determining who the ruler is...')
+    self.unit.status = ops.MaintenanceStatus('determining who the ruler is...')
     try:
-        if self._call_that_takes_a_few_seconds_and_only_passes_on_leadership:
-            self.unit.status = ActiveStatus('I rule')
+        if self._call_that_takes_a_few_seconds_and_only_passes_on_leadership():
+            self.unit.status = ops.ActiveStatus('I rule')
         else:
-            self.unit.status = WaitingStatus('checking this is right...')
+            self.unit.status = ops.WaitingStatus('checking this is right...')
             self._check_that_takes_some_more_time()
-            self.unit.status = ActiveStatus('I am ruled')
+            self.unit.status = ops.ActiveStatus('I am ruled')
     except:
-        self.unit.status = BlockedStatus('something went wrong')
+        self.unit.status = ops.BlockedStatus('something went wrong')
 ```
 
 More broadly, often we want to test 'side effects' of executing a charm, such as what events have been emitted, what
 statuses it went through, etc... Before we get there, we have to explain what the `Context` represents, and its
 relationship with the `State`.
 
-# Context and State
+## Context and State
 
-Consider the following tests. Suppose we want to verify that while handling a given toplevel juju event:
+Consider the following tests. Suppose we want to verify that while handling a given top-level Juju event:
 
 - a specific chain of (custom) events was emitted on the charm
 - the charm `juju-log`ged these specific strings
 - the charm went through this sequence of app/unit statuses (e.g. `maintenance`, then `waiting`, then `active`)
 
-These types of test have a place in Scenario, but that is not State: the contents of the juju log or the status history
+These types of test have a place in Scenario, but that is not State: the contents of the Juju log or the status history
 are side effects of executing a charm, but are not persisted in a charm-accessible "state" in any meaningful way.
 In other words: those data streams are, from the charm's perspective, write-only.
 
 As such, they do not belong in `scenario.State` but in `scenario.Context`: the object representing the charm's execution
 context.
 
 ## Status history
 
 You can verify that the charm has followed the expected path by checking the unit/app status history like so:
 
 ```python
+import ops
+import scenario
 from charm import MyCharm
-from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, UnknownStatus
-from scenario import State, Context
 
 
 def test_statuses():
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-    ctx.run('start', State(leader=False))
+    ctx = scenario.Context(MyCharm, meta={"name": "foo"})
+    out = ctx.run('start', scenario.State(leader=False))
     assert ctx.unit_status_history == [
-        UnknownStatus(),
-        MaintenanceStatus('determining who the ruler is...'),
-        WaitingStatus('checking this is right...'),
-        ActiveStatus("I am ruled"),
+        ops.UnknownStatus(),
+        ops.MaintenanceStatus('determining who the ruler is...'),
+        ops.WaitingStatus('checking this is right...'),
     ]
+    assert out.unit_status == ops.ActiveStatus("I am ruled"),
     
     # similarly you can check the app status history:
     assert ctx.app_status_history == [
-        UnknownStatus(),
+        ops.UnknownStatus(),
         ...
     ]
 ```
 
-Note that the current status is not in the **unit status history**.
+Note that the *current* status is **not** in the unit status history.
 
 Also note that, unless you initialize the State with a preexisting status, the first status in the history will always
-be `unknown`. That is because, so far as scenario is concerned, each event is "the first event this charm has ever
+be `unknown`. That is because, so far as Scenario is concerned, each event is "the first event this charm has ever
 seen".
 
 If you want to simulate a situation in which the charm already has seen some event, and is in a status other than
 Unknown (the default status every charm is born with), you will have to pass the 'initial status' to State.
 
 ```python
-from ops.model import ActiveStatus
-from scenario import State, Status
+import ops
+import scenario
 
 # ...
-ctx.run('start', State(unit_status=ActiveStatus('foo')))
+ctx.run('start', scenario.State(unit_status=ops.ActiveStatus('foo')))
 assert ctx.unit_status_history == [
-    ActiveStatus('foo'),  # now the first status is active: 'foo'!
+    ops.ActiveStatus('foo'),  # now the first status is active: 'foo'!
     # ...
 ]
-
 ```
 
 ## Workload version history
 
 Using a similar api to `*_status_history`, you can assert that the charm has set one or more workload versions during a
 hook execution:
 
 ```python
-from scenario import Context
+import scenario
 
 # ...
-ctx: Context
+ctx: scenario.Context
 assert ctx.workload_version_history == ['1', '1.2', '1.5']
 # ...
 ```
 
+Note that the *current* version is not in the version history, as with the status history.
+
 ## Emitted events
 
 If your charm deals with deferred events, custom events, and charm libs that in turn emit their own custom events, it
 can be hard to examine the resulting control flow. In these situations it can be useful to verify that, as a result of a
 given Juju event triggering (say, 'start'), a specific chain of events is emitted on the charm. The
 resulting state, black-box as it is, gives little insight into how exactly it was obtained.
 
 ```python
-from scenario import Context
-from ops.charm import StartEvent
+import ops
+import scenario
 
 
 def test_foo():
-    ctx = Context(...)
+    ctx = scenario.Context(...)
     ctx.run('start', ...)
 
     assert len(ctx.emitted_events) == 1
-    assert isinstance(ctx.emitted_events[0], StartEvent)
+    assert isinstance(ctx.emitted_events[0], ops.StartEvent)
 ```
 
 You can configure what events will be captured by passing the following arguments to `Context`:
 -  `capture_deferred_events`: If you want to include re-emitted deferred events.
 -  `capture_framework_events`: If you want to include framework events (`pre-commit`, `commit`, and `collect-status`). 
 
 For example:
 ```python
-from scenario import Context, Event, State
+import scenario
 
 def test_emitted_full():
-    ctx = Context(
+    ctx = scenario.Context(
         MyCharm,
         capture_deferred_events=True,
         capture_framework_events=True,
     )
-    ctx.run("start", State(deferred=[Event("update-status").deferred(MyCharm._foo)]))
+    ctx.run("start", scenario.State(deferred=[scenario.Event("update-status").deferred(MyCharm._foo)]))
 
     assert len(ctx.emitted_events) == 5
     assert [e.handle.kind for e in ctx.emitted_events] == [
         "update_status",
         "start",
         "collect_unit_status",
         "pre_commit",
         "commit",
     ]
 ```
 
-
 ### Low-level access: using directly `capture_events`
 
 If you need more control over what events are captured (or you're not into pytest), you can use directly the context
 manager that powers the `emitted_events` fixture: `scenario.capture_events`.
 This context manager allows you to intercept any events emitted by the framework.
 
 Usage:
 
 ```python
-from ops.charm import StartEvent, UpdateStatusEvent
-from scenario import State, Context, DeferredEvent, capture_events
+import ops
+import scenario
 
 with capture_events() as emitted:
-    ctx = Context(...)
+    ctx = scenario.Context(...)
     state_out = ctx.run(
         "update-status",
-        State(deferred=[DeferredEvent("start", ...)])
+        scenario.State(deferred=[scenario.DeferredEvent("start", ...)])
     )
 
 # deferred events get reemitted first
-assert isinstance(emitted[0], StartEvent)
-# the main juju event gets emitted next
-assert isinstance(emitted[1], UpdateStatusEvent)
-# possibly followed by a tail of all custom events that the main juju event triggered in turn
+assert isinstance(emitted[0], ops.StartEvent)
+# the main Juju event gets emitted next
+assert isinstance(emitted[1], ops.UpdateStatusEvent)
+# possibly followed by a tail of all custom events that the main Juju event triggered in turn
 # assert isinstance(emitted[2], MyFooEvent)
 # ...
 ```
 
 You can filter events by type like so:
 
 ```python
-from ops.charm import StartEvent, RelationEvent
-from scenario import capture_events
+import ops
 
-with capture_events(StartEvent, RelationEvent) as emitted:
+with capture_events(ops.StartEvent, ops.RelationEvent) as emitted:
     # capture all `start` and `*-relation-*` events.
     pass
 ```
 
 Configuration:
 
-- Passing no event types, like: `capture_events()`, is equivalent to `capture_events(EventBase)`.
+- Passing no event types, like: `capture_events()`, is equivalent to `capture_events(ops.EventBase)`.
 - By default, **framework events** (`PreCommit`, `Commit`) are not considered for inclusion in the output list even if
   they match the instance check. You can toggle that by passing: `capture_events(include_framework=True)`.
 - By default, **deferred events** are included in the listing if they match the instance check. You can toggle that by
   passing: `capture_events(include_deferred=False)`.
 
 ## Relations
 
 You can write scenario tests to verify the shape of relation data:
 
 ```python
-from ops.charm import CharmBase
-
-from scenario import Relation, State, Context
+import ops
+import scenario
 
 
 # This charm copies over remote app data to local unit data
-class MyCharm(CharmBase):
+class MyCharm(ops.CharmBase):
     ...
 
-    def _on_event(self, e):
-        rel = e.relation
+    def _on_event(self, event):
+        rel = event.relation
         assert rel.app.name == 'remote'
         assert rel.data[self.unit]['abc'] == 'foo'
-        rel.data[self.unit]['abc'] = rel.data[e.app]['cde']
+        rel.data[self.unit]['abc'] = rel.data[event.app]['cde']
 
 
 def test_relation_data():
-    state_in = State(relations=[
-        Relation(
+    state_in = scenario.State(relations=[
+        scenario.Relation(
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "foo"},
             remote_app_data={"cde": "baz!"},
         ),
     ])
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
+    ctx = scenario.Context(MyCharm, meta={"name": "foo"})
 
     state_out = ctx.run('start', state_in)
 
     assert state_out.relations[0].local_unit_data == {"abc": "baz!"}
     # you can do this to check that there are no other differences:
     assert state_out.relations == [
-        Relation(
+        scenario.Relation(
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "baz!"},
             remote_app_data={"cde": "baz!"},
         ),
     ]
 
 # which is very idiomatic and superbly explicit. Noice.
 ```
 
 The only mandatory argument to `Relation` (and other relation types, see below) is `endpoint`. The `interface` will be
-derived from the charm's `metadata.yaml`. When fully defaulted, a relation is 'empty'. There are no remote units, the
+derived from the charm's metadata. When fully defaulted, a relation is 'empty'. There are no remote units, the
 remote application is called `'remote'` and only has a single unit `remote/0`, and nobody has written any data to the
 databags yet.
 
 That is typically the state of a relation when the first unit joins it.
 
 When you use `Relation`, you are specifying a regular (conventional) relation. But that is not the only type of
 relation. There are also peer relations and subordinate relations. While in the background the data model is the same,
 the data access rules and the consistency constraints on them are very different. For example, it does not make sense
 for a peer relation to have a different 'remote app' than its 'local app', because it's the same application.
 
 ### PeerRelation
 
-To declare a peer relation, you should use `scenario.state.PeerRelation`. The core difference with regular relations is
+To declare a peer relation, you should use `scenario.PeerRelation`. The core difference with regular relations is
 that peer relations do not have a "remote app" (it's this app, in fact). So unlike `Relation`, a `PeerRelation` does not
 have `remote_app_name` or `remote_app_data` arguments. Also, it talks in terms of `peers`:
 
 - `Relation.remote_units_data` maps to `PeerRelation.peers_data`
 
 ```python
-from scenario.state import PeerRelation
+import scenario
 
-relation = PeerRelation(
+relation = scenario.PeerRelation(
     endpoint="peers",
     peers_data={1: {}, 2: {}, 42: {'foo': 'bar'}},
 )
 ```
 
 be mindful when using `PeerRelation` not to include **"this unit"**'s ID in `peers_data` or `peers_ids`, as that would
 be flagged by the Consistency Checker:
 
 ```python
-from scenario import State, PeerRelation, Context
+import scenario
 
-state_in = State(relations=[
-    PeerRelation(
+state_in = scenario.State(relations=[
+    scenario.PeerRelation(
         endpoint="peers",
         peers_data={1: {}, 2: {}, 42: {'foo': 'bar'}},
     )])
 
-Context(..., unit_id=1).run("start", state_in)  # invalid: this unit's id cannot be the ID of a peer.
+scenario.Context(..., unit_id=1).run("start", state_in)  # invalid: this unit's id cannot be the ID of a peer.
 
 
 ```
 
 ### SubordinateRelation
 
-To declare a subordinate relation, you should use `scenario.state.SubordinateRelation`. The core difference with regular
+To declare a subordinate relation, you should use `scenario.SubordinateRelation`. The core difference with regular
 relations is that subordinate relations always have exactly one remote unit (there is always exactly one remote unit
 that this unit can see). 
 Because of that, `SubordinateRelation`, compared to `Relation`, always talks in terms of `remote`:
 
 - `Relation.remote_units_data` becomes `SubordinateRelation.remote_unit_data` taking a single `Dict[str:str]`. The remote unit ID can be provided as a separate argument. 
 - `Relation.remote_unit_ids` becomes `SubordinateRelation.remote_unit_id` (a single ID instead of a list of IDs)
 - `Relation.remote_units_data` becomes `SubordinateRelation.remote_unit_data` (a single databag instead of a mapping from unit IDs to databags)
 
 ```python
-from scenario.state import SubordinateRelation
+import scenario
 
-relation = SubordinateRelation(
+relation = scenario.SubordinateRelation(
     endpoint="peers",
     remote_unit_data={"foo": "bar"},
     remote_app_name="zookeeper",
     remote_unit_id=42
 )
 relation.remote_unit_name  # "zookeeper/42"
 ```
 
 ### Triggering Relation Events
 
 If you want to trigger relation events, the easiest way to do so is get a hold of the Relation instance and grab the
 event from one of its aptly-named properties:
 
 ```python
-from scenario import Relation
+import scenario
 
-relation = Relation(endpoint="foo", interface="bar")
+relation = scenario.Relation(endpoint="foo", interface="bar")
 changed_event = relation.changed_event
 joined_event = relation.joined_event
 # ...
 ```
 
 This is in fact syntactic sugar for:
 
 ```python
-from scenario import Relation, Event
+import scenario
 
-relation = Relation(endpoint="foo", interface="bar")
-changed_event = Event('foo-relation-changed', relation=relation)
+relation = scenario.Relation(endpoint="foo", interface="bar")
+changed_event = scenario.Event('foo-relation-changed', relation=relation)
 ```
 
 The reason for this construction is that the event is associated with some relation-specific metadata, that Scenario
 needs to set up the process that will run `ops.main` with the right environment variables.
 
 ### Working with relation IDs
 
-Every time you instantiate `Relation` (or peer, or subordinate), the new instance will be given a unique `relation_id`.
-To inspect the ID the next relation instance will have, you can call `state.next_relation_id`.
+Every time you instantiate `Relation` (or peer, or subordinate), the new instance will be given a unique `id`.
+To inspect the ID the next relation instance will have, you can call `scenario.state.next_relation_id`.
 
 ```python
-from scenario import Relation
-from scenario.state import next_relation_id
+import scenario.state
 
-next_id = next_relation_id(update=False)
-rel = Relation('foo')
-assert rel.relation_id == next_id
+next_id = scenario.state.next_relation_id(update=False)
+rel = scenario.Relation('foo')
+assert rel.id == next_id
 ``` 
 
 This can be handy when using `replace` to create new relations, to avoid relation ID conflicts:
 
 ```python
-from scenario import Relation
-from scenario.state import next_relation_id
+import scenario.state
 
-rel = Relation('foo')
-rel2 = rel.replace(local_app_data={"foo": "bar"}, relation_id=next_relation_id())
-assert rel2.relation_id == rel.relation_id + 1 
+rel = scenario.Relation('foo')
+rel2 = rel.replace(local_app_data={"foo": "bar"}, id=scenario.state.next_relation_id())
+assert rel2.id == rel.id + 1 
 ``` 
 
 If you don't do this, and pass both relations into a `State`, you will trigger a consistency checker error.
 
 ### Additional event parameters
 
 All relation events have some additional metadata that does not belong in the Relation object, such as, for a
@@ -535,230 +527,236 @@
 events, is that the relation already ties 'this app' to some 'remote app' (cfr. the `Relation.remote_app_name` attr),
 but not to a specific unit. What remote unit this event is about is not a `State` concern but an `Event` one.
 
 The `remote_unit_id` will default to the first ID found in the relation's `remote_units_data`, but if the test you are
 writing is close to that domain, you should probably override it and pass it manually.
 
 ```python
-from scenario import Relation, Event
+import scenario
 
-relation = Relation(endpoint="foo", interface="bar")
+relation = scenario.Relation(endpoint="foo", interface="bar")
 remote_unit_2_is_joining_event = relation.joined_event(remote_unit_id=2)
 
 # which is syntactic sugar for:
-remote_unit_2_is_joining_event = Event('foo-relation-changed', relation=relation, relation_remote_unit_id=2)
+remote_unit_2_is_joining_event = scenario.Event('foo-relation-changed', relation=relation, relation_remote_unit_id=2)
 ```
 
-### Networks
+## Networks
 
 Simplifying a bit the Juju "spaces" model, each integration endpoint a charm defines in its metadata is associated with a network. Regardless of whether there is a living relation over that endpoint, that is.  
 
-If your charm has a relation `"foo"` (defined in metadata.yaml), then the charm will be able at runtime to do `self.model.get_binding("foo").network`.
+If your charm has a relation `"foo"` (defined in its metadata), then the charm will be able at runtime to do `self.model.get_binding("foo").network`.
 The network you'll get by doing so is heavily defaulted (see `state.Network.default`) and good for most use-cases because the charm should typically not be concerned about what IP it gets. 
 
-On top of the relation-provided network bindings, a charm can also define some `extra-bindings` in its metadata.yaml and access them at runtime. Note that this is a deprecated feature that should not be relied upon. For completeness, we support it in Scenario.
+On top of the relation-provided network bindings, a charm can also define some `extra-bindings` in its metadata and access them at runtime. Note that this is a deprecated feature that should not be relied upon. For completeness, we support it in Scenario.
 
 If you want to, you can override any of these relation or extra-binding associated networks with a custom one by passing it to `State.networks`.
 
 ```python
-from scenario import State, Network
-state = State(networks={
-  'foo': Network.default(private_address='4.4.4.4')
+import scenario
+
+state = scenario.State(networks={
+  'foo': scenario.Network.default(private_address='192.0.2.1')
 })
 ```
 
 Where `foo` can either be the name of an `extra-bindings`-defined binding, or a relation endpoint.
 
-# Containers
+## Containers
 
-When testing a kubernetes charm, you can mock container interactions. When using the null state (`State()`), there will
+When testing a Kubernetes charm, you can mock container interactions. When using the null state (`State()`), there will
 be no containers. So if the charm were to `self.unit.containers`, it would get back an empty dict.
 
 To give the charm access to some containers, you need to pass them to the input state, like so:
 `State(containers=[...])`
 
 An example of a state including some containers:
 
 ```python
-from scenario.state import Container, State
+import scenario
 
-state = State(containers=[
-    Container(name="foo", can_connect=True),
-    Container(name="bar", can_connect=False)
+state = scenario.State(containers=[
+    scenario.Container(name="foo", can_connect=True),
+    scenario.Container(name="bar", can_connect=False)
 ])
 ```
 
 In this case, `self.unit.get_container('foo').can_connect()` would return `True`, while for 'bar' it would give `False`.
 
 ### Container filesystem setup
+
 You can configure a container to have some files in it:
 
 ```python
-from pathlib import Path
+import pathlib
 
-from scenario.state import Container, State, Mount
+import scenario
 
-local_file = Path('/path/to/local/real/file.txt')
+local_file = pathlib.Path('/path/to/local/real/file.txt')
 
-container = Container(name="foo", can_connect=True, mounts={'local': Mount('/local/share/config.yaml', local_file)})
-state = State(containers=[container])
+container = scenario.Container(
+    name="foo",
+    can_connect=True,
+    mounts={'local': Mount('/local/share/config.yaml', local_file)}
+    )
+state = scenario.State(containers=[container])
 ```
 
 In this case, if the charm were to:
 
 ```python
 def _on_start(self, _):
     foo = self.unit.get_container('foo')
     content = foo.pull('/local/share/config.yaml').read()
 ```
 
-then `content` would be the contents of our locally-supplied `file.txt`. You can use `tempdir` for nicely wrapping
+then `content` would be the contents of our locally-supplied `file.txt`. You can use `tempfile` for nicely wrapping
 data and passing it to the charm via the container.
 
 `container.push` works similarly, so you can write a test like:
 
 ```python
 import tempfile
-from ops.charm import CharmBase
-from scenario import State, Container, Mount, Context
+
+import ops
+import scenario
 
 
-class MyCharm(CharmBase):
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
+class MyCharm(ops.CharmBase):
+    def __init__(self, framework):
+        super().__init__(framework)
+        framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
 
     def _on_pebble_ready(self, _):
         foo = self.unit.get_container('foo')
         foo.push('/local/share/config.yaml', "TEST", make_dirs=True)
 
 
 def test_pebble_push():
     with tempfile.NamedTemporaryFile() as local_file:
-        container = Container(name='foo',
-                              can_connect=True,
-                              mounts={'local': Mount('/local/share/config.yaml', local_file.name)})
-        state_in = State(
-            containers=[container]
+        container = scenario,Container(
+            name='foo',
+            can_connect=True,
+            mounts={'local': Mount('/local/share/config.yaml', local_file.name)}
         )
-        Context(
+        state_in = State(containers=[container])
+        ctx = Context(
             MyCharm,
             meta={"name": "foo", "containers": {"foo": {}}}
-        ).run(
+        )
+        ctx.run(
             container.pebble_ready_event(),
             state_in,
         )
         assert local_file.read().decode() == "TEST"
 ```
 
 `container.pebble_ready_event` is syntactic sugar for: `Event("foo-pebble-ready", container=container)`. The reason we
 need to associate the container with the event is that the Framework uses an envvar to determine which container the
 pebble-ready event is about (it does not use the event name). Scenario needs that information, similarly, for injecting
 that envvar into the charm's runtime.
 
-## Container filesystem post-mortem
+### Container filesystem post-mortem
+
 If the charm writes files to a container (to a location you didn't Mount as a temporary folder you have access to), you will be able to inspect them using the `get_filesystem` api.
 
 ```python
-from ops.charm import CharmBase
-from scenario import State, Container, Mount, Context
+import ops
+import scenario
 
 
-class MyCharm(CharmBase):
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
+class MyCharm(ops.CharmBase):
+    def __init__(self, framework):
+        super().__init__(framework)
+        framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
 
     def _on_pebble_ready(self, _):
         foo = self.unit.get_container('foo')
         foo.push('/local/share/config.yaml', "TEST", make_dirs=True)
 
 
 def test_pebble_push():
-    container = Container(name='foo',
-                          can_connect=True)
-    state_in = State(
-        containers=[container]
-    )
-    ctx = Context(
+    container = scenario.Container(name='foo', can_connect=True)
+    state_in = scenario.State(containers=[container])
+    ctx = scenario.Context(
         MyCharm,
         meta={"name": "foo", "containers": {"foo": {}}}
     )
     
     ctx.run("start", state_in)
 
-    # this is the root of the simulated container filesystem. Any mounts will be symlinks in it.
+    # This is the root of the simulated container filesystem. Any mounts will be symlinks in it.
     container_root_fs = container.get_filesystem(ctx)
     cfg_file = container_root_fs / 'local' / 'share' / 'config.yaml'
     assert cfg_file.read_text() == "TEST"
 ```
 
-## `Container.exec` mocks
+### `Container.exec` mocks
 
 `container.exec` is a tad more complicated, but if you get to this low a level of simulation, you probably will have far
 worse issues to deal with. You need to specify, for each possible command the charm might run on the container, what the
 result of that would be: its return code, what will be written to stdout/stderr.
 
 ```python
-from ops.charm import CharmBase
-
-from scenario import State, Container, ExecOutput, Context
+import ops
+import scenario
 
 LS_LL = """
 .rw-rw-r--  228 ubuntu ubuntu 18 jan 12:05 -- charmcraft.yaml
 .rw-rw-r--  497 ubuntu ubuntu 18 jan 12:05 -- config.yaml
 .rw-rw-r--  900 ubuntu ubuntu 18 jan 12:05 -- CONTRIBUTING.md
 drwxrwxr-x    - ubuntu ubuntu 18 jan 12:06 -- lib
 """
 
 
-class MyCharm(CharmBase):
+class MyCharm(ops.CharmBase):
     def _on_start(self, _):
         foo = self.unit.get_container('foo')
         proc = foo.exec(['ls', '-ll'])
         stdout, _ = proc.wait_output()
         assert stdout == LS_LL
 
 
 def test_pebble_exec():
-    container = Container(
+    container = scenario.Container(
         name='foo',
         exec_mock={
             ('ls', '-ll'):  # this is the command we're mocking
-                ExecOutput(return_code=0,  # this data structure contains all we need to mock the call.
-                           stdout=LS_LL)
+                scenario.ExecOutput(return_code=0,  # this data structure contains all we need to mock the call.
+                                    stdout=LS_LL)
         }
     )
-    state_in = State(
-        containers=[container]
-    )
-    state_out = Context(
+    state_in = scenario.State(containers=[container])
+    ctx = scenario.Context(
         MyCharm,
         meta={"name": "foo", "containers": {"foo": {}}},
-    ).run(
+    )
+    state_out = ctx.run(
         container.pebble_ready_event,
         state_in,
     )
 ```
 
-# Storage
+## Storage
 
-If your charm defines `storage` in its metadata, you can use `scenario.state.Storage` to instruct Scenario to make (mocked) filesystem storage available to the charm at runtime.
+If your charm defines `storage` in its metadata, you can use `scenario.Storage` to instruct Scenario to make (mocked) filesystem storage available to the charm at runtime.
 
-Using the same `get_filesystem` API as `Container`, you can access the tempdir used by Scenario to mock the filesystem root before and after the scenario runs.
+Using the same `get_filesystem` API as `Container`, you can access the temporary directory used by Scenario to mock the filesystem root before and after the scenario runs.
 
 ```python
-from scenario import Storage, Context, State
-# some charm with a 'foo' filesystem-type storage defined in metadata.yaml 
-ctx = Context(MyCharm)
-storage = Storage("foo")
-# setup storage with some content
+import scenario
+
+# Some charm with a 'foo' filesystem-type storage defined in its metadata:
+ctx = scenario.Context(MyCharm)
+storage = scenario.Storage("foo")
+
+# Setup storage with some content:
 (storage.get_filesystem(ctx) / "myfile.txt").write_text("helloworld")
 
-with ctx.manager("update-status", State(storage=[storage])) as mgr:
+with ctx.manager("update-status", scenario.State(storage=[storage])) as mgr:
     foo = mgr.charm.model.storages["foo"][0]
     loc = foo.location
     path = loc / "myfile.txt"
     assert path.exists()
     assert path.read_text() == "helloworld"
 
     myfile = loc / "path.py"
@@ -768,87 +766,85 @@
 assert (
     storage.get_filesystem(ctx) / "path.py"
 ).read_text() == "helloworlds"
 ```
 
 Note that State only wants to know about **attached** storages. A storage which is not attached to the charm can simply be omitted from State and the charm will be none the wiser.
 
-## Storage-add
+### Storage-add
 
 If a charm requests adding more storage instances while handling some event, you can inspect that from the `Context.requested_storage` API.
 
 ```python
-# in MyCharm._on_foo:
-# the charm requests two new "foo" storage instances to be provisioned 
+# In MyCharm._on_foo:
+# The charm requests two new "foo" storage instances to be provisioned:
 self.model.storages.request("foo", 2)
 ```
 
 From test code, you can inspect that:
 
 ```python
-from scenario import Context, State
+import scenario
 
-ctx = Context(MyCharm)
-ctx.run('some-event-that-will-cause_on_foo-to-be-called', State())
+ctx = scenario.Context(MyCharm)
+ctx.run('some-event-that-will-cause_on_foo-to-be-called', scenario.State())
 
-# the charm has requested two 'foo' storages to be provisioned
+# the charm has requested two 'foo' storages to be provisioned:
 assert ctx.requested_storages['foo'] == 2
 ```
 
 Requesting storages has no other consequence in Scenario. In real life, this request will trigger Juju to provision the storage and execute the charm again with `foo-storage-attached`.
 So a natural follow-up Scenario test suite for this case would be:
 
 ```python
-from scenario import Context, State, Storage
+import scenario
 
-ctx = Context(MyCharm)
-foo_0 = Storage('foo')
-# the charm is notified that one of the storages it has requested is ready
+ctx = scenario.Context(MyCharm)
+foo_0 = scenario.Storage('foo')
+# The charm is notified that one of the storages it has requested is ready:
 ctx.run(foo_0.attached_event, State(storage=[foo_0]))
 
-foo_1 = Storage('foo')
-# the charm is notified that the other storage is also ready
+foo_1 = scenario.Storage('foo')
+# The charm is notified that the other storage is also ready:
 ctx.run(foo_1.attached_event, State(storage=[foo_0, foo_1]))
 ```
 
+## Ports
 
-# Ports
-
-Since `ops 2.6.0`, charms can invoke the `open-port`, `close-port`, and `opened-ports` hook tools to manage the ports opened on the host vm/container. Using the `State.opened_ports` api, you can: 
+Since `ops 2.6.0`, charms can invoke the `open-port`, `close-port`, and `opened-ports` hook tools to manage the ports opened on the host VM/container. Using the `State.opened_ports` API, you can: 
 
 - simulate a charm run with a port opened by some previous execution
 ```python
-from scenario import State, Port, Context
+import scenario
 
-ctx = Context(MyCharm)
-ctx.run("start", State(opened_ports=[Port("tcp", 42)]))
+ctx = scenario.Context(MyCharm)
+ctx.run("start", scenario.State(opened_ports=[scenario.Port("tcp", 42)]))
 ```
 - assert that a charm has called `open-port` or `close-port`:
 ```python
-from scenario import State, Port, Context
+import scenario
 
-ctx = Context(MyCharm)
-state1 = ctx.run("start", State())
-assert state1.opened_ports == [Port("tcp", 42)]
+ctx = scenario.Context(MyCharm)
+state1 = ctx.run("start", scenario.State())
+assert state1.opened_ports == [scenario.Port("tcp", 42)]
 
 state2 = ctx.run("stop", state1)
 assert state2.opened_ports == []
 ```
 
-
-# Secrets
+## Secrets
 
 Scenario has secrets. Here's how you use them.
 
 ```python
-from scenario import State, Secret
+import scenario
 
-state = State(
+state = scenario.State(
     secrets=[
-        Secret(
+        scenario.Secret(
             id='foo',
             contents={0: {'key': 'public'}}
         )
     ]
 )
 ```
 
@@ -858,327 +854,381 @@
 There are three cases:
 - the secret is owned by this app but not this unit, in which case this charm can only manage it if we are the leader
 - the secret is owned by this unit, in which case this charm can always manage it (leader or not)
 - (default) the secret is not owned by this app nor unit, which means we can't manage it but only view it
 
 Thus by default, the secret is not owned by **this charm**, but, implicitly, by some unknown 'other charm', and that other charm has granted us view rights.
 
-
 The presence of the secret in `State.secrets` entails that we have access to it, either as owners or as grantees. Therefore, if we're not owners, we must be grantees. Absence of a Secret from the known secrets list means we are not entitled to obtaining it in any way. The charm, indeed, shouldn't even know it exists.
 
 [note]
 If this charm does not own the secret, but also it was not granted view rights by the (remote) owner, you model this in Scenario by _not adding it to State.secrets_! The presence of a `Secret` in `State.secrets` means, in other words, that the charm has view rights (otherwise, why would we put it there?). If the charm owns the secret, or is leader, it will _also_ have manage rights on top of view ones.
 [/note]
 
 To specify a secret owned by this unit (or app):
 
 ```python
-from scenario import State, Secret
+import scenario
 
-state = State(
+state = scenario.State(
     secrets=[
-        Secret(
+        scenario.Secret(
             id='foo',
             contents={0: {'key': 'private'}},
             owner='unit',  # or 'app'
             remote_grants={0: {"remote"}}
             # the secret owner has granted access to the "remote" app over some relation with ID 0
         )
     ]
 )
 ```
 
 To specify a secret owned by some other application and give this unit (or app) access to it:
 
 ```python
-from scenario import State, Secret
+import scenario
 
-state = State(
+state = scenario.State(
     secrets=[
-        Secret(
+        scenario.Secret(
             id='foo',
             contents={0: {'key': 'public'}},
             # owner=None, which is the default
             revision=0,  # the revision that this unit (or app) is currently tracking
         )
     ]
 )
 ```
 
+## StoredState
+
+Scenario can simulate StoredState. You can define it on the input side as:
+
+```python
+import ops
+import scenario
+
+from ops.charm import CharmBase
+
+
+class MyCharmType(ops.CharmBase):
+    my_stored_state = ops.StoredState()
+
+    def __init__(self, framework):
+        super().__init__(framework)
+        assert self.my_stored_state.foo == 'bar'  # this will pass!
+
+
+state = scenario.State(stored_state=[
+    scenario.StoredState(
+        owner_path="MyCharmType",
+        name="my_stored_state",
+        content={
+            'foo': 'bar',
+            'baz': {42: 42},
+        })
+])
+```
+
+And the charm's runtime will see `self.my_stored_state.foo` and `.baz` as expected. Also, you can run assertions on it on
+the output side the same as any other bit of state.
+
+## Resources
+
+If your charm requires access to resources, you can make them available to it through `State.resources`.
+From the perspective of a 'real' deployed charm, if your charm _has_ resources defined in its metadata, they _must_ be made available to the charm. That is a Juju-enforced constraint: you can't deploy a charm without attaching all resources it needs to it.
+However, when testing, this constraint is unnecessarily strict (and it would also mean the great majority of all existing tests would break) since a charm will only notice that a resource is not available when it explicitly asks for it, which not many charms do.
+
+So, the only consistency-level check we enforce in Scenario when it comes to resource is that if a resource is provided in State, it needs to have been declared in the metadata.
+
+```python
+import scenario
+
+ctx = scenario.Context(MyCharm, meta={'name': 'juliette', "resources": {"foo": {"type": "oci-image"}}})
+with ctx.manager("start", scenario.State(resources={'foo': '/path/to/resource.tar'})) as mgr:
+    # If the charm, at runtime, were to call self.model.resources.fetch("foo"), it would get '/path/to/resource.tar' back.
+    path = mgr.charm.model.resources.fetch('foo')
+    assert path == '/path/to/resource.tar'
+```
+
+## Model
+
+Charms don't usually need to be aware of the model in which they are deployed,
+but if you need to set the model name or UUID, you can provide a `scenario.Model`
+to the state:
+
+```python
+import ops
+import scenario
+
+class MyCharm(ops.CharmBase):
+    pass
+
+ctx = scenario.Context(MyCharm, meta={"name": "foo"})
+state_in = scenario.State(model=scenario.Model(name="my-model"))
+out = ctx.run("start", state_in)
+assert out.model.name == "my-model"
+assert out.model.uuid == state_in.model.uuid
+```
+
+## CloudSpec
+
+You can set CloudSpec information in the state (only `type` and `name` are required).
+
+Example:
+
+```python
+import scenario
+
+state = scenario.State(
+    cloud_spec=scenario.CloudSpec(
+        type="lxd",
+        name="localhost",
+        endpoint="https://127.0.0.1:8443",
+        credential=scenario.CloudCredential(
+            auth_type="clientcertificate",
+            attributes={
+                "client-cert": "foo",
+                "client-key": "bar",
+                "server-cert": "baz",
+            },
+        ),
+    ),
+    model=scenario.Model(name="my-vm-model", type="lxd"),
+)
+```
+
+Then you can access it by `Model.get_cloud_spec()`:
+
+```python
+# charm.py
+class MyVMCharm(ops.CharmBase):
+    def __init__(self, framework: ops.Framework):
+        super().__init__(framework)
+        framework.observe(self.on.start, self._on_start)
+
+    def _on_start(self, event: ops.StartEvent):
+        self.cloud_spec = self.model.get_cloud_spec()
+```
+
 # Actions
 
 An action is a special sort of event, even though `ops` handles them almost identically.
 In most cases, you'll want to inspect the 'results' of an action, or whether it has failed or
 logged something while executing. Many actions don't have a direct effect on the output state.
 For this reason, the output state is less prominent in the return type of `Context.run_action`.
 
 How to test actions with scenario:
 
 ## Actions without parameters
 
 ```python
-from scenario import Context, State, ActionOutput
+import scenario
+
 from charm import MyCharm
 
 
 def test_backup_action():
-    ctx = Context(MyCharm)
+    ctx = scenario.Context(MyCharm)
 
-    # If you didn't declare do_backup in the charm's `actions.yaml`, 
+    # If you didn't declare do_backup in the charm's metadata, 
     # the `ConsistencyChecker` will slap you on the wrist and refuse to proceed.
-    out: ActionOutput = ctx.run_action("do_backup_action", State())
+    out: scenario.ActionOutput = ctx.run_action("do_backup_action", scenario.State())
 
-    # you can assert action results, logs, failure using the ActionOutput interface
+    # You can assert action results, logs, failure using the ActionOutput interface:
     assert out.logs == ['baz', 'qux']
     
     if out.success:
-      # if the action did not fail, we can read the results:
+      # If the action did not fail, we can read the results:
       assert out.results == {'foo': 'bar'}
 
     else:
-      # if the action fails, we can read a failure message
+      # If the action fails, we can read a failure message:
       assert out.failure == 'boo-hoo'
 ```
 
 ## Parametrized Actions
 
 If the action takes parameters, you'll need to instantiate an `Action`.
 
 ```python
-from scenario import Action, Context, State, ActionOutput
+import scenario
+
 from charm import MyCharm
 
 
 def test_backup_action():
-    # define an action
-    action = Action('do_backup', params={'a': 'b'})
-    ctx = Context(MyCharm)
-
-    # if the parameters (or their type) don't match what declared in actions.yaml, 
-    # the `ConsistencyChecker` will slap you on the other wrist. 
-    out: ActionOutput = ctx.run_action(action, State())
+    # Define an action:
+    action = scenario.Action('do_backup', params={'a': 'b'})
+    ctx = scenario.Context(MyCharm)
+
+    # If the parameters (or their type) don't match what is declared in the metadata, 
+    # the `ConsistencyChecker` will slap you on the other wrist.
+    out: scenario.ActionOutput = ctx.run_action(action, scenario.State())
 
     # ...
 ```
 
 # Deferred events
 
 Scenario allows you to accurately simulate the Operator Framework's event queue. The event queue is responsible for
 keeping track of the deferred events. On the input side, you can verify that if the charm triggers with this and that
 event in its queue (they would be there because they had been deferred in the previous run), then the output state is
 valid.
 
 ```python
-from scenario import State, deferred, Context
+import scenario
 
 
 class MyCharm(...):
     ...
 
-    def _on_update_status(self, e):
-        e.defer()
+    def _on_update_status(self, event):
+        event.defer()
 
-    def _on_start(self, e):
-        e.defer()
+    def _on_start(self, event):
+        event.defer()
 
 
 def test_start_on_deferred_update_status(MyCharm):
     """Test charm execution if a 'start' is dispatched when in the previous run an update-status had been deferred."""
-    state_in = State(
+    state_in = scenario.State(
         deferred=[
-            deferred('update_status',
-                     handler=MyCharm._on_update_status)
+            scenario.deferred('update_status', handler=MyCharm._on_update_status)
         ]
     )
-    state_out = Context(MyCharm).run('start', state_in)
+    state_out = scenario.Context(MyCharm).run('start', state_in)
     assert len(state_out.deferred) == 1
     assert state_out.deferred[0].name == 'start'
 ```
 
 You can also generate the 'deferred' data structure (called a DeferredEvent) from the corresponding Event (and the
 handler):
 
 ```python
-from scenario import Event, Relation
+import scenario
 
 
 class MyCharm(...):
     ...
 
 
-deferred_start = Event('start').deferred(MyCharm._on_start)
-deferred_install = Event('install').deferred(MyCharm._on_start)
-```
-
-## relation events:
-
-```python
-foo_relation = Relation('foo')
-deferred_relation_changed_evt = foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
+deferred_start = scenario.Event('start').deferred(MyCharm._on_start)
+deferred_install = scenario.Event('install').deferred(MyCharm._on_start)
 ```
 
 On the output side, you can verify that an event that you expect to have been deferred during this trigger, has indeed
 been deferred.
 
 ```python
-from scenario import State, Context
+import scenario
 
 
 class MyCharm(...):
     ...
 
-    def _on_start(self, e):
-        e.defer()
+    def _on_start(self, event):
+        event.defer()
 
 
 def test_defer(MyCharm):
-    out = Context(MyCharm).run('start', State())
+    out = scenario.Context(MyCharm).run('start', scenario.State())
     assert len(out.deferred) == 1
     assert out.deferred[0].name == 'start'
 ```
 
 ## Deferring relation events
 
 If you want to test relation event deferrals, some extra care needs to be taken. RelationEvents hold references to the
 Relation instance they are about. So do they in Scenario. You can use the deferred helper to generate the data
 structure:
 
 ```python
-from scenario import State, Relation, deferred
+import scenario
 
 
 class MyCharm(...):
     ...
 
-    def _on_foo_relation_changed(self, e):
-        e.defer()
+    def _on_foo_relation_changed(self, event):
+        event.defer()
 
 
 def test_start_on_deferred_update_status(MyCharm):
-    foo_relation = Relation('foo')
-    State(
+    foo_relation = scenario.Relation('foo')
+    scenario.State(
         relations=[foo_relation],
         deferred=[
-            deferred('foo_relation_changed',
-                     handler=MyCharm._on_foo_relation_changed,
-                     relation=foo_relation)
+            scenario.deferred('foo_relation_changed',
+                              handler=MyCharm._on_foo_relation_changed,
+                              relation=foo_relation)
         ]
     )
 ```
 
-but you can also use a shortcut from the relation event itself, as mentioned above:
+but you can also use a shortcut from the relation event itself:
 
 ```python
-
-from scenario import Relation
+import scenario
 
 
 class MyCharm(...):
     ...
 
 
-foo_relation = Relation('foo')
+foo_relation = scenario.Relation('foo')
 foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
 ```
 
-### Fine-tuning
+## Fine-tuning
 
 The deferred helper Scenario provides will not support out of the box all custom event subclasses, or events emitted by
 charm libraries or objects other than the main charm class.
 
 For general-purpose usage, you will need to instantiate DeferredEvent directly.
 
 ```python
-from scenario import DeferredEvent
+import scenario
 
-my_deferred_event = DeferredEvent(
+my_deferred_event = scenario.DeferredEvent(
     handle_path='MyCharm/MyCharmLib/on/database_ready[1]',
     owner='MyCharmLib',  # the object observing the event. Could also be MyCharm.
     observer='_on_database_ready'
 )
 ```
 
-# StoredState
-
-Scenario can simulate StoredState. You can define it on the input side as:
-
-```python
-from ops.charm import CharmBase
-from ops.framework import StoredState as Ops_StoredState, Framework
-from scenario import State, StoredState
-
-
-class MyCharmType(CharmBase):
-    my_stored_state = Ops_StoredState()
-
-    def __init__(self, framework: Framework):
-        super().__init__(framework)
-        assert self.my_stored_state.foo == 'bar'  # this will pass!
-
-
-state = State(stored_state=[
-    StoredState(
-        owner_path="MyCharmType",
-        name="my_stored_state",
-        content={
-            'foo': 'bar',
-            'baz': {42: 42},
-        })
-])
-```
-
-And the charm's runtime will see `self.stored_State.foo` and `.baz` as expected. Also, you can run assertions on it on
-the output side the same as any other bit of state.
-
-# Resources
-
-If your charm requires access to resources, you can make them available to it through `State.resources`.
-From the perspective of a 'real' deployed charm, if your charm _has_ resources defined in `metadata.yaml`, they _must_ be made available to the charm. That is a Juju-enforced constraint: you can't deploy a charm without attaching all resources it needs to it.
-However, when testing, this constraint is unnecessarily strict (and it would also mean the great majority of all existing tests would break) since a charm will only notice that a resource is not available when it explicitly asks for it, which not many charms do.
-
-So, the only consistency-level check we enforce in Scenario when it comes to resource is that if a resource is provided in State, it needs to have been declared in metadata.
-
-```python
-from scenario import State, Context
-ctx = Context(MyCharm, meta={'name': 'juliette', "resources": {"foo": {"type": "oci-image"}}})
-with ctx.manager("start", State(resources={'foo': '/path/to/resource.tar'})) as mgr:
-    # if the charm, at runtime, were to call self.model.resources.fetch("foo"), it would get '/path/to/resource.tar' back.
-    path = mgr.charm.model.resources.fetch('foo')
-    assert path == '/path/to/resource.tar' 
-```
-
 # Emitting custom events
 
-While the main use case of Scenario is to emit juju events, i.e. the built-in `start`, `install`, `*-relation-changed`,
+While the main use case of Scenario is to emit Juju events, i.e. the built-in `start`, `install`, `*-relation-changed`,
 etc..., it can be sometimes handy to directly trigger custom events defined on arbitrary Objects in your hierarchy.
 
 Suppose your charm uses a charm library providing an `ingress_provided` event.
 The 'proper' way to emit it is to run the event that causes that custom event to be emitted by the library, whatever
 that may be, for example a `foo-relation-changed`.
 
 However, that may mean that you have to set up all sorts of State and mocks so that the right preconditions are met and
 the event is emitted at all.
 
 If for whatever reason you don't want to do that and you attempt to run that event directly you will get an error:
 
 ```python
-from scenario import Context, State
+import scenario
 
-Context(...).run("ingress_provided", State())  # raises scenario.ops_main_mock.NoObserverError
+scenario.Context(...).run("ingress_provided", scenario.State())  # raises scenario.ops_main_mock.NoObserverError
 ```
 
 This happens because the framework, by default, searches for an event source named `ingress_provided` in `charm.on`, but
 since the event is defined on another Object, it will fail to find it.
 
 You can prefix the event name with the path leading to its owner to tell Scenario where to find the event source:
 
 ```python
-from scenario import Context, State
+import scenario
 
-Context(...).run("my_charm_lib.on.foo", State())
+scenario.Context(...).run("my_charm_lib.on.foo", scenario.State())
 ```
 
 This will instruct Scenario to emit `my_charm.my_charm_lib.on.foo`.
 
 (always omit the 'root', i.e. the charm framework key, from the path)
 
 # Live charm introspection
@@ -1186,158 +1236,155 @@
 Scenario is a black-box, state-transition testing framework. It makes it trivial to assert that a status went from A to
 B, but not to assert that, in the context of this charm execution, with this state, a certain charm-internal method was called and returned a
 given piece of data, or would return this and that _if_ it had been called.
 
 Scenario offers a cheekily-named context manager for this use case specifically:
 
 ```python
-from ops import CharmBase, StoredState
+import ops
+import scenario
 
 from charms.bar.lib_name.v1.charm_lib import CharmLib
-from scenario import Context, State
 
 
-class MyCharm(CharmBase):
+class MyCharm(ops.CharmBase):
     META = {"name": "mycharm"}
-    _stored = StoredState()
+    _stored = ops.StoredState()
     
     def __init__(self, framework):
         super().__init__(framework)
         self._stored.set_default(a="a")
         self.my_charm_lib = CharmLib()
         framework.observe(self.on.start, self._on_start)
 
     def _on_start(self, event):
         self._stored.a = "b"
 
 
 def test_live_charm_introspection(mycharm):
-    ctx = Context(mycharm, meta=mycharm.META)
+    ctx = scenario.Context(mycharm, meta=mycharm.META)
     # If you want to do this with actions, you can use `Context.action_manager` instead.
-    with ctx.manager("start", State()) as manager:
-        # this is your charm instance, after ops has set it up
+    with ctx.manager("start", scenario.State()) as manager:
+        # This is your charm instance, after ops has set it up:
         charm: MyCharm = manager.charm
         
-        # we can check attributes on nested Objects or the charm itself 
+        # We can check attributes on nested Objects or the charm itself:
         assert charm.my_charm_lib.foo == "foo"
-        # such as stored state
+        # such as stored state:
         assert charm._stored.a == "a"
 
-        # this will tell ops.main to proceed with normal execution and emit the "start" event on the charm
+        # This will tell ops.main to proceed with normal execution and emit the "start" event on the charm:
         state_out = manager.run()
     
-        # after that is done, we are handed back control, and we can again do some introspection
+        # After that is done, we are handed back control, and we can again do some introspection:
         assert charm.my_charm_lib.foo == "bar"
-        # and check that the charm's internal state is as we expect
+        # and check that the charm's internal state is as we expect:
         assert charm._stored.a == "b"
 
     # state_out is, as in regular scenario tests, a State object you can assert on:
     assert state_out.unit_status == ...
 ```
 
 Note that you can't call `manager.run()` multiple times: the manager is a context that ensures that `ops.main` 'pauses' right
 before emitting the event to hand you some introspection hooks, but for the rest this is a regular scenario test: you
 can't emit multiple events in a single charm execution.
 
 # The virtual charm root
 
 Before executing the charm, Scenario copies the charm's `/src`, any libs, the metadata, config, and actions `yaml`s to a temporary directory. The
-charm will see that tempdir as its 'root'. This allows us to keep things simple when dealing with metadata that can be
+charm will see that temporary directory as its 'root'. This allows us to keep things simple when dealing with metadata that can be
 either inferred from the charm type being passed to `Context` or be passed to it as an argument, thereby overriding
 the inferred one. This also allows you to test charms defined on the fly, as in:
 
 ```python
-from ops.charm import CharmBase
-from scenario import State, Context
+import ops
+import scenario
 
 
-class MyCharmType(CharmBase):
+class MyCharmType(ops.CharmBase):
     pass
 
 
-ctx = Context(charm_type=MyCharmType,
-              meta={'name': 'my-charm-name'})
+ctx = scenario.Context(charm_type=MyCharmType, meta={'name': 'my-charm-name'})
 ctx.run('start', State())
 ```
 
-A consequence of this fact is that you have no direct control over the tempdir that we are creating to put the metadata
+A consequence of this fact is that you have no direct control over the temporary directory that we are creating to put the metadata
 you are passing to `.run()` (because `ops` expects it to be a file...). That is, unless you pass your own:
 
 ```python
-from ops.charm import CharmBase
-from scenario import State, Context
 import tempfile
 
+import ops
+import scenario
+
 
-class MyCharmType(CharmBase):
+class MyCharmType(ops.CharmBase):
     pass
 
 
 td = tempfile.TemporaryDirectory()
-state = Context(
+state = scenario.Context(
     charm_type=MyCharmType,
     meta={'name': 'my-charm-name'},
     charm_root=td.name
-).run('start', State())
+).run('start', scenario.State())
 ```
 
 Do this, and you will be able to set up said directory as you like before the charm is run, as well as verify its
 contents after the charm has run. Do keep in mind that any metadata files you create in it will be overwritten by Scenario, and therefore
 ignored, if you pass any metadata keys to `Context`. Omit `meta` in the call
-above, and Scenario will instead attempt to read `metadata.yaml` from the
+above, and Scenario will instead attempt to read metadata from the
 temporary directory.
 
-
 # Immutability
 
-All of the data structures in `state`, e.g. `State, Relation, Container`, etc... are immutable (implemented as frozen
-dataclasses).
+All of the data structures in `state`, e.g. `State, Relation, Container`, etc... are implemented as frozen dataclasses.
 
 This means that all components of the state that goes into a `context.run()` call are not mutated by the call, and the
 state that you obtain in return is a different instance, and all parts of it have been (deep)copied.
-This ensures that you can do delta-based comparison of states without worrying about them being mutated by scenario.
+This ensures that you can do delta-based comparison of states without worrying about them being mutated by Scenario.
 
 If you want to modify any of these data structures, you will need to either reinstantiate it from scratch, or use
 the `replace` api.
 
 ```python
-from scenario import Relation
+import scenario
 
-relation = Relation('foo', remote_app_data={"1": "2"})
+relation = scenario.Relation('foo', remote_app_data={"1": "2"})
 # make a copy of relation, but with remote_app_data set to {"3", "4"} 
 relation2 = relation.replace(remote_app_data={"3", "4"})
 ```
 
 # Consistency checks
 
 A Scenario, that is, the combination of an event, a state, and a charm, is consistent if it's plausible in JujuLand. For
 example, Juju can't emit a `foo-relation-changed` event on your charm unless your charm has declared a `foo` relation
-endpoint in its `metadata.yaml`. If that happens, that's a juju bug. Scenario however assumes that Juju is bug-free,
+endpoint in its metadata. If that happens, that's a Juju bug. Scenario however assumes that Juju is bug-free,
 therefore, so far as we're concerned, that can't happen, and therefore we help you verify that the scenarios you create
 are consistent and raise an exception if that isn't so.
 
 That happens automatically behind the scenes whenever you trigger an event;
 `scenario.consistency_checker.check_consistency` is called and verifies that the scenario makes sense.
 
 ## Caveats:
 
 - False positives: not all checks are implemented yet; more will come.
 - False negatives: it is possible that a scenario you know to be consistent is seen as inconsistent. That is probably a
-  bug in the consistency checker itself, please report it.
+  bug in the consistency checker itself; please report it.
 - Inherent limitations: if you have a custom event whose name conflicts with a builtin one, the consistency constraints
   of the builtin one will apply. For example: if you decide to name your custom event `bar-pebble-ready`, but you are
   working on a machine charm or don't have either way a `bar` container in your `metadata.yaml`, Scenario will flag that
   as inconsistent.
 
 ## Bypassing the checker
 
 If you have a clear false negative, are explicitly testing 'edge', inconsistent situations, or for whatever reason the
 checker is in your way, you can set the `SCENARIO_SKIP_CONSISTENCY_CHECKS` envvar and skip it altogether. Hopefully you
 don't need that.
 
 # Jhack integrations
 
-Up until `v5.6.0`, `scenario` shipped with a cli tool called `snapshot`, used to interact with a live charm's state.
+Up until `v5.6.0`, Scenario shipped with a cli tool called `snapshot`, used to interact with a live charm's state.
 The functionality [has been moved over to `jhack`](https://github.com/PietroPasotti/jhack/pull/111), 
 to allow us to keep working on it independently, and to streamline 
-the profile of `scenario` itself as it becomes more broadly adopted and ready for widespread usage.
-
+the profile of Scenario itself as it becomes more broadly adopted and ready for widespread usage.
```

### Comparing `ops-scenario-6.0.3/README.md` & `ops_scenario-6.0.4/ops_scenario.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: ops-scenario
+Version: 6.0.4
+Summary: Python library providing a state-transition testing API for Operator Framework charms.
+Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/canonical/ops-scenario
+Project-URL: Bug Tracker, https://github.com/canonical/ops-scenario/issues
+Keywords: juju,test
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: ops>=2.6
+Requires-Dist: PyYAML>=6.0.1
+
 # Scenario
 
 [![Build](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml)
 [![QC](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml/badge.svg?event=pull_request)](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml?event=pull_request)
 [![Discourse Status](https://img.shields.io/discourse/status?server=https%3A%2F%2Fdiscourse.charmhub.io&style=flat&label=CharmHub%20Discourse)](https://discourse.charmhub.io)
 [![foo](https://img.shields.io/badge/everything-charming-blueviolet)](https://github.com/PietroPasotti/jhack)
 [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://discourse.charmhub.io/t/rethinking-charm-testing-with-ops-scenario/8649)
@@ -14,54 +36,54 @@
 event on the charm and execute its logic.
 
 This puts scenario tests somewhere in between unit and integration tests: some say 'functional', some say 'contract', I prefer 'state-transition'.
 
 Scenario tests nudge you into thinking of a charm as an input->output function. The input is the
 union of an `Event` (why am I, charm, being executed), a `State` (am I leader? what is my relation data? what is my
 config?...) and the charm's execution `Context` (what relations can I have? what containers can I have?...). The output is another `State`: the state after the charm has had a chance to interact with the
-mocked juju model and affect the initial state back.
+mocked Juju model and affect the initial state back.
 
 ![state transition model depiction](resources/state-transition-model.png)
 
 For example: a charm currently in `unknown` status is executed with a `start` event, and based on whether it has leadership or not (according to its input state), it will decide to set `active` or `blocked` status (which will be reflected in the output state).
 
 Scenario-testing a charm, then, means verifying that:
 
 - the charm does not raise uncaught exceptions while handling the event
 - the output state (or the diff with the input state) is as expected.
 
-# Core concepts as a metaphor
+## Core concepts as a metaphor
 
 I like metaphors, so here we go:
 
 - There is a theatre stage.
 - You pick an actor (a Charm) to put on the stage. Not just any actor: an improv one.
 - You arrange the stage with content that the actor will have to interact with. This consists of selecting:
     - An initial situation (`State`) in which the actor is, e.g. is the actor the main role or an NPC (`is_leader`), or what
       other actors are there around it, what is written in those pebble-shaped books on the table?
     - Something that has just happened (an `Event`) and to which the actor has to react (e.g. one of the NPCs leaves the
       stage (`relation-departed`), or the content of one of the books changes).
 - How the actor will react to the event will have an impact on the context: e.g. the actor might knock over a table (a
   container), or write something down into one of the books.
 
-# Core concepts not as a metaphor
+## Core concepts not as a metaphor
 
 Scenario tests are about running assertions on atomic state transitions treating the charm being tested like a black
 box. An initial state goes in, an event occurs (say, `'start'`) and a new state comes out. Scenario tests are about
 validating the transition, that is, consistency-checking the delta between the two states, and verifying the charm
 author's expectations.
 
 Comparing scenario tests with `Harness` tests:
 
 - Harness exposes an imperative API: the user is expected to call methods on the Harness driving it to the desired
   state, then verify its validity by calling charm methods or inspecting the raw data. In contrast, Scenario is declarative. You fully specify an initial state, an execution context and an event, then you run the charm and inspect the results.
 - Harness instantiates the charm once, then allows you to fire multiple events on the charm, which is breeding ground
   for subtle bugs. Scenario tests are centered around testing single state transitions, that is, one event at a time.
   This ensures that the execution environment is as clean as possible (for a unit test).
-- Harness maintains a model of the juju Model, which is a maintenance burden and adds complexity. Scenario mocks at the
+- Harness maintains a model of the Juju Model, which is a maintenance burden and adds complexity. Scenario mocks at the
   level of hook tools and stores all mocking data in a monolithic data structure (the State), which makes it more
   lightweight and portable.
 
 # Writing scenario tests
 
 A scenario test consists of three broad steps:
 
@@ -78,430 +100,422 @@
 
 The most basic scenario is one in which all is defaulted and barely any data is
 available. The charm has no config, no relations, no leadership, and its status is `unknown`.
 
 With that, we can write the simplest possible scenario test:
 
 ```python
-from scenario import State, Context, Event
-from ops.charm import CharmBase
-from ops.model import UnknownStatus
+import ops
+import scenario
 
 
-class MyCharm(CharmBase):
+class MyCharm(ops.CharmBase):
     pass
 
 
 def test_scenario_base():
-    ctx = Context(MyCharm, meta={"name": "foo"})
-    out = ctx.run(Event("start"), State())
-    assert out.unit_status == UnknownStatus()
+    ctx = scenario.Context(MyCharm, meta={"name": "foo"})
+    out = ctx.run(scenario.Event("start"), scenario.State())
+    assert out.unit_status == ops.UnknownStatus()
 ```
 
 Now let's start making it more complicated. Our charm sets a special state if it has leadership on 'start':
 
 ```python
+import ops
 import pytest
-from scenario import State, Context
-from ops.charm import CharmBase
-from ops.model import ActiveStatus
+import scenario
 
 
-class MyCharm(CharmBase):
-    def __init__(self, ...):
-        self.framework.observe(self.on.start, self._on_start)
+class MyCharm(ops.CharmBase):
+    def __init__(self, framework):
+        super().__init__(framework)
+        framework.observe(self.on.start, self._on_start)
 
     def _on_start(self, _):
         if self.unit.is_leader():
-            self.unit.status = ActiveStatus('I rule')
+            self.unit.status = ops.ActiveStatus('I rule')
         else:
-            self.unit.status = ActiveStatus('I am ruled')
+            self.unit.status = ops.ActiveStatus('I am ruled')
 
 
 @pytest.mark.parametrize('leader', (True, False))
 def test_status_leader(leader):
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-    out = ctx.run('start', State(leader=leader))
-    assert out.unit_status == ActiveStatus('I rule' if leader else 'I am ruled')
+    ctx = scenario.Context(MyCharm, meta={"name": "foo"})
+    out = ctx.run('start', scenario.State(leader=leader))
+    assert out.unit_status == ops.ActiveStatus('I rule' if leader else 'I am ruled')
 ```
 
 By defining the right state we can programmatically define what answers will the charm get to all the questions it can
-ask the juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
+ask the Juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
 
 ## Statuses
 
 One of the simplest types of black-box testing available to charmers is to execute the charm and verify that the charm
 sets the expected unit/application status. We have seen a simple example above including leadership. But what if the
 charm transitions through a sequence of statuses?
 
 ```python
-from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, BlockedStatus
+import ops
 
 
 # charm code:
 def _on_event(self, _event):
-    self.unit.status = MaintenanceStatus('determining who the ruler is...')
+    self.unit.status = ops.MaintenanceStatus('determining who the ruler is...')
     try:
-        if self._call_that_takes_a_few_seconds_and_only_passes_on_leadership:
-            self.unit.status = ActiveStatus('I rule')
+        if self._call_that_takes_a_few_seconds_and_only_passes_on_leadership():
+            self.unit.status = ops.ActiveStatus('I rule')
         else:
-            self.unit.status = WaitingStatus('checking this is right...')
+            self.unit.status = ops.WaitingStatus('checking this is right...')
             self._check_that_takes_some_more_time()
-            self.unit.status = ActiveStatus('I am ruled')
+            self.unit.status = ops.ActiveStatus('I am ruled')
     except:
-        self.unit.status = BlockedStatus('something went wrong')
+        self.unit.status = ops.BlockedStatus('something went wrong')
 ```
 
 More broadly, often we want to test 'side effects' of executing a charm, such as what events have been emitted, what
 statuses it went through, etc... Before we get there, we have to explain what the `Context` represents, and its
 relationship with the `State`.
 
-# Context and State
+## Context and State
 
-Consider the following tests. Suppose we want to verify that while handling a given toplevel juju event:
+Consider the following tests. Suppose we want to verify that while handling a given top-level Juju event:
 
 - a specific chain of (custom) events was emitted on the charm
 - the charm `juju-log`ged these specific strings
 - the charm went through this sequence of app/unit statuses (e.g. `maintenance`, then `waiting`, then `active`)
 
-These types of test have a place in Scenario, but that is not State: the contents of the juju log or the status history
+These types of test have a place in Scenario, but that is not State: the contents of the Juju log or the status history
 are side effects of executing a charm, but are not persisted in a charm-accessible "state" in any meaningful way.
 In other words: those data streams are, from the charm's perspective, write-only.
 
 As such, they do not belong in `scenario.State` but in `scenario.Context`: the object representing the charm's execution
 context.
 
 ## Status history
 
 You can verify that the charm has followed the expected path by checking the unit/app status history like so:
 
 ```python
+import ops
+import scenario
 from charm import MyCharm
-from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, UnknownStatus
-from scenario import State, Context
 
 
 def test_statuses():
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-    ctx.run('start', State(leader=False))
+    ctx = scenario.Context(MyCharm, meta={"name": "foo"})
+    out = ctx.run('start', scenario.State(leader=False))
     assert ctx.unit_status_history == [
-        UnknownStatus(),
-        MaintenanceStatus('determining who the ruler is...'),
-        WaitingStatus('checking this is right...'),
-        ActiveStatus("I am ruled"),
+        ops.UnknownStatus(),
+        ops.MaintenanceStatus('determining who the ruler is...'),
+        ops.WaitingStatus('checking this is right...'),
     ]
+    assert out.unit_status == ops.ActiveStatus("I am ruled"),
     
     # similarly you can check the app status history:
     assert ctx.app_status_history == [
-        UnknownStatus(),
+        ops.UnknownStatus(),
         ...
     ]
 ```
 
-Note that the current status is not in the **unit status history**.
+Note that the *current* status is **not** in the unit status history.
 
 Also note that, unless you initialize the State with a preexisting status, the first status in the history will always
-be `unknown`. That is because, so far as scenario is concerned, each event is "the first event this charm has ever
+be `unknown`. That is because, so far as Scenario is concerned, each event is "the first event this charm has ever
 seen".
 
 If you want to simulate a situation in which the charm already has seen some event, and is in a status other than
 Unknown (the default status every charm is born with), you will have to pass the 'initial status' to State.
 
 ```python
-from ops.model import ActiveStatus
-from scenario import State, Status
+import ops
+import scenario
 
 # ...
-ctx.run('start', State(unit_status=ActiveStatus('foo')))
+ctx.run('start', scenario.State(unit_status=ops.ActiveStatus('foo')))
 assert ctx.unit_status_history == [
-    ActiveStatus('foo'),  # now the first status is active: 'foo'!
+    ops.ActiveStatus('foo'),  # now the first status is active: 'foo'!
     # ...
 ]
-
 ```
 
 ## Workload version history
 
 Using a similar api to `*_status_history`, you can assert that the charm has set one or more workload versions during a
 hook execution:
 
 ```python
-from scenario import Context
+import scenario
 
 # ...
-ctx: Context
+ctx: scenario.Context
 assert ctx.workload_version_history == ['1', '1.2', '1.5']
 # ...
 ```
 
+Note that the *current* version is not in the version history, as with the status history.
+
 ## Emitted events
 
 If your charm deals with deferred events, custom events, and charm libs that in turn emit their own custom events, it
 can be hard to examine the resulting control flow. In these situations it can be useful to verify that, as a result of a
 given Juju event triggering (say, 'start'), a specific chain of events is emitted on the charm. The
 resulting state, black-box as it is, gives little insight into how exactly it was obtained.
 
 ```python
-from scenario import Context
-from ops.charm import StartEvent
+import ops
+import scenario
 
 
 def test_foo():
-    ctx = Context(...)
+    ctx = scenario.Context(...)
     ctx.run('start', ...)
 
     assert len(ctx.emitted_events) == 1
-    assert isinstance(ctx.emitted_events[0], StartEvent)
+    assert isinstance(ctx.emitted_events[0], ops.StartEvent)
 ```
 
 You can configure what events will be captured by passing the following arguments to `Context`:
 -  `capture_deferred_events`: If you want to include re-emitted deferred events.
 -  `capture_framework_events`: If you want to include framework events (`pre-commit`, `commit`, and `collect-status`). 
 
 For example:
 ```python
-from scenario import Context, Event, State
+import scenario
 
 def test_emitted_full():
-    ctx = Context(
+    ctx = scenario.Context(
         MyCharm,
         capture_deferred_events=True,
         capture_framework_events=True,
     )
-    ctx.run("start", State(deferred=[Event("update-status").deferred(MyCharm._foo)]))
+    ctx.run("start", scenario.State(deferred=[scenario.Event("update-status").deferred(MyCharm._foo)]))
 
     assert len(ctx.emitted_events) == 5
     assert [e.handle.kind for e in ctx.emitted_events] == [
         "update_status",
         "start",
         "collect_unit_status",
         "pre_commit",
         "commit",
     ]
 ```
 
-
 ### Low-level access: using directly `capture_events`
 
 If you need more control over what events are captured (or you're not into pytest), you can use directly the context
 manager that powers the `emitted_events` fixture: `scenario.capture_events`.
 This context manager allows you to intercept any events emitted by the framework.
 
 Usage:
 
 ```python
-from ops.charm import StartEvent, UpdateStatusEvent
-from scenario import State, Context, DeferredEvent, capture_events
+import ops
+import scenario
 
 with capture_events() as emitted:
-    ctx = Context(...)
+    ctx = scenario.Context(...)
     state_out = ctx.run(
         "update-status",
-        State(deferred=[DeferredEvent("start", ...)])
+        scenario.State(deferred=[scenario.DeferredEvent("start", ...)])
     )
 
 # deferred events get reemitted first
-assert isinstance(emitted[0], StartEvent)
-# the main juju event gets emitted next
-assert isinstance(emitted[1], UpdateStatusEvent)
-# possibly followed by a tail of all custom events that the main juju event triggered in turn
+assert isinstance(emitted[0], ops.StartEvent)
+# the main Juju event gets emitted next
+assert isinstance(emitted[1], ops.UpdateStatusEvent)
+# possibly followed by a tail of all custom events that the main Juju event triggered in turn
 # assert isinstance(emitted[2], MyFooEvent)
 # ...
 ```
 
 You can filter events by type like so:
 
 ```python
-from ops.charm import StartEvent, RelationEvent
-from scenario import capture_events
+import ops
 
-with capture_events(StartEvent, RelationEvent) as emitted:
+with capture_events(ops.StartEvent, ops.RelationEvent) as emitted:
     # capture all `start` and `*-relation-*` events.
     pass
 ```
 
 Configuration:
 
-- Passing no event types, like: `capture_events()`, is equivalent to `capture_events(EventBase)`.
+- Passing no event types, like: `capture_events()`, is equivalent to `capture_events(ops.EventBase)`.
 - By default, **framework events** (`PreCommit`, `Commit`) are not considered for inclusion in the output list even if
   they match the instance check. You can toggle that by passing: `capture_events(include_framework=True)`.
 - By default, **deferred events** are included in the listing if they match the instance check. You can toggle that by
   passing: `capture_events(include_deferred=False)`.
 
 ## Relations
 
 You can write scenario tests to verify the shape of relation data:
 
 ```python
-from ops.charm import CharmBase
-
-from scenario import Relation, State, Context
+import ops
+import scenario
 
 
 # This charm copies over remote app data to local unit data
-class MyCharm(CharmBase):
+class MyCharm(ops.CharmBase):
     ...
 
-    def _on_event(self, e):
-        rel = e.relation
+    def _on_event(self, event):
+        rel = event.relation
         assert rel.app.name == 'remote'
         assert rel.data[self.unit]['abc'] == 'foo'
-        rel.data[self.unit]['abc'] = rel.data[e.app]['cde']
+        rel.data[self.unit]['abc'] = rel.data[event.app]['cde']
 
 
 def test_relation_data():
-    state_in = State(relations=[
-        Relation(
+    state_in = scenario.State(relations=[
+        scenario.Relation(
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "foo"},
             remote_app_data={"cde": "baz!"},
         ),
     ])
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
+    ctx = scenario.Context(MyCharm, meta={"name": "foo"})
 
     state_out = ctx.run('start', state_in)
 
     assert state_out.relations[0].local_unit_data == {"abc": "baz!"}
     # you can do this to check that there are no other differences:
     assert state_out.relations == [
-        Relation(
+        scenario.Relation(
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "baz!"},
             remote_app_data={"cde": "baz!"},
         ),
     ]
 
 # which is very idiomatic and superbly explicit. Noice.
 ```
 
 The only mandatory argument to `Relation` (and other relation types, see below) is `endpoint`. The `interface` will be
-derived from the charm's `metadata.yaml`. When fully defaulted, a relation is 'empty'. There are no remote units, the
+derived from the charm's metadata. When fully defaulted, a relation is 'empty'. There are no remote units, the
 remote application is called `'remote'` and only has a single unit `remote/0`, and nobody has written any data to the
 databags yet.
 
 That is typically the state of a relation when the first unit joins it.
 
 When you use `Relation`, you are specifying a regular (conventional) relation. But that is not the only type of
 relation. There are also peer relations and subordinate relations. While in the background the data model is the same,
 the data access rules and the consistency constraints on them are very different. For example, it does not make sense
 for a peer relation to have a different 'remote app' than its 'local app', because it's the same application.
 
 ### PeerRelation
 
-To declare a peer relation, you should use `scenario.state.PeerRelation`. The core difference with regular relations is
+To declare a peer relation, you should use `scenario.PeerRelation`. The core difference with regular relations is
 that peer relations do not have a "remote app" (it's this app, in fact). So unlike `Relation`, a `PeerRelation` does not
 have `remote_app_name` or `remote_app_data` arguments. Also, it talks in terms of `peers`:
 
 - `Relation.remote_units_data` maps to `PeerRelation.peers_data`
 
 ```python
-from scenario.state import PeerRelation
+import scenario
 
-relation = PeerRelation(
+relation = scenario.PeerRelation(
     endpoint="peers",
     peers_data={1: {}, 2: {}, 42: {'foo': 'bar'}},
 )
 ```
 
 be mindful when using `PeerRelation` not to include **"this unit"**'s ID in `peers_data` or `peers_ids`, as that would
 be flagged by the Consistency Checker:
 
 ```python
-from scenario import State, PeerRelation, Context
+import scenario
 
-state_in = State(relations=[
-    PeerRelation(
+state_in = scenario.State(relations=[
+    scenario.PeerRelation(
         endpoint="peers",
         peers_data={1: {}, 2: {}, 42: {'foo': 'bar'}},
     )])
 
-Context(..., unit_id=1).run("start", state_in)  # invalid: this unit's id cannot be the ID of a peer.
+scenario.Context(..., unit_id=1).run("start", state_in)  # invalid: this unit's id cannot be the ID of a peer.
 
 
 ```
 
 ### SubordinateRelation
 
-To declare a subordinate relation, you should use `scenario.state.SubordinateRelation`. The core difference with regular
+To declare a subordinate relation, you should use `scenario.SubordinateRelation`. The core difference with regular
 relations is that subordinate relations always have exactly one remote unit (there is always exactly one remote unit
 that this unit can see). 
 Because of that, `SubordinateRelation`, compared to `Relation`, always talks in terms of `remote`:
 
 - `Relation.remote_units_data` becomes `SubordinateRelation.remote_unit_data` taking a single `Dict[str:str]`. The remote unit ID can be provided as a separate argument. 
 - `Relation.remote_unit_ids` becomes `SubordinateRelation.remote_unit_id` (a single ID instead of a list of IDs)
 - `Relation.remote_units_data` becomes `SubordinateRelation.remote_unit_data` (a single databag instead of a mapping from unit IDs to databags)
 
 ```python
-from scenario.state import SubordinateRelation
+import scenario
 
-relation = SubordinateRelation(
+relation = scenario.SubordinateRelation(
     endpoint="peers",
     remote_unit_data={"foo": "bar"},
     remote_app_name="zookeeper",
     remote_unit_id=42
 )
 relation.remote_unit_name  # "zookeeper/42"
 ```
 
 ### Triggering Relation Events
 
 If you want to trigger relation events, the easiest way to do so is get a hold of the Relation instance and grab the
 event from one of its aptly-named properties:
 
 ```python
-from scenario import Relation
+import scenario
 
-relation = Relation(endpoint="foo", interface="bar")
+relation = scenario.Relation(endpoint="foo", interface="bar")
 changed_event = relation.changed_event
 joined_event = relation.joined_event
 # ...
 ```
 
 This is in fact syntactic sugar for:
 
 ```python
-from scenario import Relation, Event
+import scenario
 
-relation = Relation(endpoint="foo", interface="bar")
-changed_event = Event('foo-relation-changed', relation=relation)
+relation = scenario.Relation(endpoint="foo", interface="bar")
+changed_event = scenario.Event('foo-relation-changed', relation=relation)
 ```
 
 The reason for this construction is that the event is associated with some relation-specific metadata, that Scenario
 needs to set up the process that will run `ops.main` with the right environment variables.
 
 ### Working with relation IDs
 
-Every time you instantiate `Relation` (or peer, or subordinate), the new instance will be given a unique `relation_id`.
-To inspect the ID the next relation instance will have, you can call `state.next_relation_id`.
+Every time you instantiate `Relation` (or peer, or subordinate), the new instance will be given a unique `id`.
+To inspect the ID the next relation instance will have, you can call `scenario.state.next_relation_id`.
 
 ```python
-from scenario import Relation
-from scenario.state import next_relation_id
+import scenario.state
 
-next_id = next_relation_id(update=False)
-rel = Relation('foo')
-assert rel.relation_id == next_id
+next_id = scenario.state.next_relation_id(update=False)
+rel = scenario.Relation('foo')
+assert rel.id == next_id
 ``` 
 
 This can be handy when using `replace` to create new relations, to avoid relation ID conflicts:
 
 ```python
-from scenario import Relation
-from scenario.state import next_relation_id
+import scenario.state
 
-rel = Relation('foo')
-rel2 = rel.replace(local_app_data={"foo": "bar"}, relation_id=next_relation_id())
-assert rel2.relation_id == rel.relation_id + 1 
+rel = scenario.Relation('foo')
+rel2 = rel.replace(local_app_data={"foo": "bar"}, id=scenario.state.next_relation_id())
+assert rel2.id == rel.id + 1 
 ``` 
 
 If you don't do this, and pass both relations into a `State`, you will trigger a consistency checker error.
 
 ### Additional event parameters
 
 All relation events have some additional metadata that does not belong in the Relation object, such as, for a
@@ -513,230 +527,236 @@
 events, is that the relation already ties 'this app' to some 'remote app' (cfr. the `Relation.remote_app_name` attr),
 but not to a specific unit. What remote unit this event is about is not a `State` concern but an `Event` one.
 
 The `remote_unit_id` will default to the first ID found in the relation's `remote_units_data`, but if the test you are
 writing is close to that domain, you should probably override it and pass it manually.
 
 ```python
-from scenario import Relation, Event
+import scenario
 
-relation = Relation(endpoint="foo", interface="bar")
+relation = scenario.Relation(endpoint="foo", interface="bar")
 remote_unit_2_is_joining_event = relation.joined_event(remote_unit_id=2)
 
 # which is syntactic sugar for:
-remote_unit_2_is_joining_event = Event('foo-relation-changed', relation=relation, relation_remote_unit_id=2)
+remote_unit_2_is_joining_event = scenario.Event('foo-relation-changed', relation=relation, relation_remote_unit_id=2)
 ```
 
-### Networks
+## Networks
 
 Simplifying a bit the Juju "spaces" model, each integration endpoint a charm defines in its metadata is associated with a network. Regardless of whether there is a living relation over that endpoint, that is.  
 
-If your charm has a relation `"foo"` (defined in metadata.yaml), then the charm will be able at runtime to do `self.model.get_binding("foo").network`.
+If your charm has a relation `"foo"` (defined in its metadata), then the charm will be able at runtime to do `self.model.get_binding("foo").network`.
 The network you'll get by doing so is heavily defaulted (see `state.Network.default`) and good for most use-cases because the charm should typically not be concerned about what IP it gets. 
 
-On top of the relation-provided network bindings, a charm can also define some `extra-bindings` in its metadata.yaml and access them at runtime. Note that this is a deprecated feature that should not be relied upon. For completeness, we support it in Scenario.
+On top of the relation-provided network bindings, a charm can also define some `extra-bindings` in its metadata and access them at runtime. Note that this is a deprecated feature that should not be relied upon. For completeness, we support it in Scenario.
 
 If you want to, you can override any of these relation or extra-binding associated networks with a custom one by passing it to `State.networks`.
 
 ```python
-from scenario import State, Network
-state = State(networks={
-  'foo': Network.default(private_address='4.4.4.4')
+import scenario
+
+state = scenario.State(networks={
+  'foo': scenario.Network.default(private_address='192.0.2.1')
 })
 ```
 
 Where `foo` can either be the name of an `extra-bindings`-defined binding, or a relation endpoint.
 
-# Containers
+## Containers
 
-When testing a kubernetes charm, you can mock container interactions. When using the null state (`State()`), there will
+When testing a Kubernetes charm, you can mock container interactions. When using the null state (`State()`), there will
 be no containers. So if the charm were to `self.unit.containers`, it would get back an empty dict.
 
 To give the charm access to some containers, you need to pass them to the input state, like so:
 `State(containers=[...])`
 
 An example of a state including some containers:
 
 ```python
-from scenario.state import Container, State
+import scenario
 
-state = State(containers=[
-    Container(name="foo", can_connect=True),
-    Container(name="bar", can_connect=False)
+state = scenario.State(containers=[
+    scenario.Container(name="foo", can_connect=True),
+    scenario.Container(name="bar", can_connect=False)
 ])
 ```
 
 In this case, `self.unit.get_container('foo').can_connect()` would return `True`, while for 'bar' it would give `False`.
 
 ### Container filesystem setup
+
 You can configure a container to have some files in it:
 
 ```python
-from pathlib import Path
+import pathlib
 
-from scenario.state import Container, State, Mount
+import scenario
 
-local_file = Path('/path/to/local/real/file.txt')
+local_file = pathlib.Path('/path/to/local/real/file.txt')
 
-container = Container(name="foo", can_connect=True, mounts={'local': Mount('/local/share/config.yaml', local_file)})
-state = State(containers=[container])
+container = scenario.Container(
+    name="foo",
+    can_connect=True,
+    mounts={'local': Mount('/local/share/config.yaml', local_file)}
+    )
+state = scenario.State(containers=[container])
 ```
 
 In this case, if the charm were to:
 
 ```python
 def _on_start(self, _):
     foo = self.unit.get_container('foo')
     content = foo.pull('/local/share/config.yaml').read()
 ```
 
-then `content` would be the contents of our locally-supplied `file.txt`. You can use `tempdir` for nicely wrapping
+then `content` would be the contents of our locally-supplied `file.txt`. You can use `tempfile` for nicely wrapping
 data and passing it to the charm via the container.
 
 `container.push` works similarly, so you can write a test like:
 
 ```python
 import tempfile
-from ops.charm import CharmBase
-from scenario import State, Container, Mount, Context
 
+import ops
+import scenario
 
-class MyCharm(CharmBase):
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
+
+class MyCharm(ops.CharmBase):
+    def __init__(self, framework):
+        super().__init__(framework)
+        framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
 
     def _on_pebble_ready(self, _):
         foo = self.unit.get_container('foo')
         foo.push('/local/share/config.yaml', "TEST", make_dirs=True)
 
 
 def test_pebble_push():
     with tempfile.NamedTemporaryFile() as local_file:
-        container = Container(name='foo',
-                              can_connect=True,
-                              mounts={'local': Mount('/local/share/config.yaml', local_file.name)})
-        state_in = State(
-            containers=[container]
+        container = scenario,Container(
+            name='foo',
+            can_connect=True,
+            mounts={'local': Mount('/local/share/config.yaml', local_file.name)}
         )
-        Context(
+        state_in = State(containers=[container])
+        ctx = Context(
             MyCharm,
             meta={"name": "foo", "containers": {"foo": {}}}
-        ).run(
+        )
+        ctx.run(
             container.pebble_ready_event(),
             state_in,
         )
         assert local_file.read().decode() == "TEST"
 ```
 
 `container.pebble_ready_event` is syntactic sugar for: `Event("foo-pebble-ready", container=container)`. The reason we
 need to associate the container with the event is that the Framework uses an envvar to determine which container the
 pebble-ready event is about (it does not use the event name). Scenario needs that information, similarly, for injecting
 that envvar into the charm's runtime.
 
-## Container filesystem post-mortem
+### Container filesystem post-mortem
+
 If the charm writes files to a container (to a location you didn't Mount as a temporary folder you have access to), you will be able to inspect them using the `get_filesystem` api.
 
 ```python
-from ops.charm import CharmBase
-from scenario import State, Container, Mount, Context
+import ops
+import scenario
 
 
-class MyCharm(CharmBase):
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
+class MyCharm(ops.CharmBase):
+    def __init__(self, framework):
+        super().__init__(framework)
+        framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
 
     def _on_pebble_ready(self, _):
         foo = self.unit.get_container('foo')
         foo.push('/local/share/config.yaml', "TEST", make_dirs=True)
 
 
 def test_pebble_push():
-    container = Container(name='foo',
-                          can_connect=True)
-    state_in = State(
-        containers=[container]
-    )
-    ctx = Context(
+    container = scenario.Container(name='foo', can_connect=True)
+    state_in = scenario.State(containers=[container])
+    ctx = scenario.Context(
         MyCharm,
         meta={"name": "foo", "containers": {"foo": {}}}
     )
     
     ctx.run("start", state_in)
 
-    # this is the root of the simulated container filesystem. Any mounts will be symlinks in it.
+    # This is the root of the simulated container filesystem. Any mounts will be symlinks in it.
     container_root_fs = container.get_filesystem(ctx)
     cfg_file = container_root_fs / 'local' / 'share' / 'config.yaml'
     assert cfg_file.read_text() == "TEST"
 ```
 
-## `Container.exec` mocks
+### `Container.exec` mocks
 
 `container.exec` is a tad more complicated, but if you get to this low a level of simulation, you probably will have far
 worse issues to deal with. You need to specify, for each possible command the charm might run on the container, what the
 result of that would be: its return code, what will be written to stdout/stderr.
 
 ```python
-from ops.charm import CharmBase
-
-from scenario import State, Container, ExecOutput, Context
+import ops
+import scenario
 
 LS_LL = """
 .rw-rw-r--  228 ubuntu ubuntu 18 jan 12:05 -- charmcraft.yaml
 .rw-rw-r--  497 ubuntu ubuntu 18 jan 12:05 -- config.yaml
 .rw-rw-r--  900 ubuntu ubuntu 18 jan 12:05 -- CONTRIBUTING.md
 drwxrwxr-x    - ubuntu ubuntu 18 jan 12:06 -- lib
 """
 
 
-class MyCharm(CharmBase):
+class MyCharm(ops.CharmBase):
     def _on_start(self, _):
         foo = self.unit.get_container('foo')
         proc = foo.exec(['ls', '-ll'])
         stdout, _ = proc.wait_output()
         assert stdout == LS_LL
 
 
 def test_pebble_exec():
-    container = Container(
+    container = scenario.Container(
         name='foo',
         exec_mock={
             ('ls', '-ll'):  # this is the command we're mocking
-                ExecOutput(return_code=0,  # this data structure contains all we need to mock the call.
-                           stdout=LS_LL)
+                scenario.ExecOutput(return_code=0,  # this data structure contains all we need to mock the call.
+                                    stdout=LS_LL)
         }
     )
-    state_in = State(
-        containers=[container]
-    )
-    state_out = Context(
+    state_in = scenario.State(containers=[container])
+    ctx = scenario.Context(
         MyCharm,
         meta={"name": "foo", "containers": {"foo": {}}},
-    ).run(
+    )
+    state_out = ctx.run(
         container.pebble_ready_event,
         state_in,
     )
 ```
 
-# Storage
+## Storage
 
-If your charm defines `storage` in its metadata, you can use `scenario.state.Storage` to instruct Scenario to make (mocked) filesystem storage available to the charm at runtime.
+If your charm defines `storage` in its metadata, you can use `scenario.Storage` to instruct Scenario to make (mocked) filesystem storage available to the charm at runtime.
 
-Using the same `get_filesystem` API as `Container`, you can access the tempdir used by Scenario to mock the filesystem root before and after the scenario runs.
+Using the same `get_filesystem` API as `Container`, you can access the temporary directory used by Scenario to mock the filesystem root before and after the scenario runs.
 
 ```python
-from scenario import Storage, Context, State
-# some charm with a 'foo' filesystem-type storage defined in metadata.yaml 
-ctx = Context(MyCharm)
-storage = Storage("foo")
-# setup storage with some content
+import scenario
+
+# Some charm with a 'foo' filesystem-type storage defined in its metadata:
+ctx = scenario.Context(MyCharm)
+storage = scenario.Storage("foo")
+
+# Setup storage with some content:
 (storage.get_filesystem(ctx) / "myfile.txt").write_text("helloworld")
 
-with ctx.manager("update-status", State(storage=[storage])) as mgr:
+with ctx.manager("update-status", scenario.State(storage=[storage])) as mgr:
     foo = mgr.charm.model.storages["foo"][0]
     loc = foo.location
     path = loc / "myfile.txt"
     assert path.exists()
     assert path.read_text() == "helloworld"
 
     myfile = loc / "path.py"
@@ -746,87 +766,85 @@
 assert (
     storage.get_filesystem(ctx) / "path.py"
 ).read_text() == "helloworlds"
 ```
 
 Note that State only wants to know about **attached** storages. A storage which is not attached to the charm can simply be omitted from State and the charm will be none the wiser.
 
-## Storage-add
+### Storage-add
 
 If a charm requests adding more storage instances while handling some event, you can inspect that from the `Context.requested_storage` API.
 
 ```python
-# in MyCharm._on_foo:
-# the charm requests two new "foo" storage instances to be provisioned 
+# In MyCharm._on_foo:
+# The charm requests two new "foo" storage instances to be provisioned:
 self.model.storages.request("foo", 2)
 ```
 
 From test code, you can inspect that:
 
 ```python
-from scenario import Context, State
+import scenario
 
-ctx = Context(MyCharm)
-ctx.run('some-event-that-will-cause_on_foo-to-be-called', State())
+ctx = scenario.Context(MyCharm)
+ctx.run('some-event-that-will-cause_on_foo-to-be-called', scenario.State())
 
-# the charm has requested two 'foo' storages to be provisioned
+# the charm has requested two 'foo' storages to be provisioned:
 assert ctx.requested_storages['foo'] == 2
 ```
 
 Requesting storages has no other consequence in Scenario. In real life, this request will trigger Juju to provision the storage and execute the charm again with `foo-storage-attached`.
 So a natural follow-up Scenario test suite for this case would be:
 
 ```python
-from scenario import Context, State, Storage
+import scenario
 
-ctx = Context(MyCharm)
-foo_0 = Storage('foo')
-# the charm is notified that one of the storages it has requested is ready
+ctx = scenario.Context(MyCharm)
+foo_0 = scenario.Storage('foo')
+# The charm is notified that one of the storages it has requested is ready:
 ctx.run(foo_0.attached_event, State(storage=[foo_0]))
 
-foo_1 = Storage('foo')
-# the charm is notified that the other storage is also ready
+foo_1 = scenario.Storage('foo')
+# The charm is notified that the other storage is also ready:
 ctx.run(foo_1.attached_event, State(storage=[foo_0, foo_1]))
 ```
 
+## Ports
 
-# Ports
-
-Since `ops 2.6.0`, charms can invoke the `open-port`, `close-port`, and `opened-ports` hook tools to manage the ports opened on the host vm/container. Using the `State.opened_ports` api, you can: 
+Since `ops 2.6.0`, charms can invoke the `open-port`, `close-port`, and `opened-ports` hook tools to manage the ports opened on the host VM/container. Using the `State.opened_ports` API, you can: 
 
 - simulate a charm run with a port opened by some previous execution
 ```python
-from scenario import State, Port, Context
+import scenario
 
-ctx = Context(MyCharm)
-ctx.run("start", State(opened_ports=[Port("tcp", 42)]))
+ctx = scenario.Context(MyCharm)
+ctx.run("start", scenario.State(opened_ports=[scenario.Port("tcp", 42)]))
 ```
 - assert that a charm has called `open-port` or `close-port`:
 ```python
-from scenario import State, Port, Context
+import scenario
 
-ctx = Context(MyCharm)
-state1 = ctx.run("start", State())
-assert state1.opened_ports == [Port("tcp", 42)]
+ctx = scenario.Context(MyCharm)
+state1 = ctx.run("start", scenario.State())
+assert state1.opened_ports == [scenario.Port("tcp", 42)]
 
 state2 = ctx.run("stop", state1)
 assert state2.opened_ports == []
 ```
 
-
-# Secrets
+## Secrets
 
 Scenario has secrets. Here's how you use them.
 
 ```python
-from scenario import State, Secret
+import scenario
 
-state = State(
+state = scenario.State(
     secrets=[
-        Secret(
+        scenario.Secret(
             id='foo',
             contents={0: {'key': 'public'}}
         )
     ]
 )
 ```
 
@@ -836,327 +854,381 @@
 There are three cases:
 - the secret is owned by this app but not this unit, in which case this charm can only manage it if we are the leader
 - the secret is owned by this unit, in which case this charm can always manage it (leader or not)
 - (default) the secret is not owned by this app nor unit, which means we can't manage it but only view it
 
 Thus by default, the secret is not owned by **this charm**, but, implicitly, by some unknown 'other charm', and that other charm has granted us view rights.
 
-
 The presence of the secret in `State.secrets` entails that we have access to it, either as owners or as grantees. Therefore, if we're not owners, we must be grantees. Absence of a Secret from the known secrets list means we are not entitled to obtaining it in any way. The charm, indeed, shouldn't even know it exists.
 
 [note]
 If this charm does not own the secret, but also it was not granted view rights by the (remote) owner, you model this in Scenario by _not adding it to State.secrets_! The presence of a `Secret` in `State.secrets` means, in other words, that the charm has view rights (otherwise, why would we put it there?). If the charm owns the secret, or is leader, it will _also_ have manage rights on top of view ones.
 [/note]
 
 To specify a secret owned by this unit (or app):
 
 ```python
-from scenario import State, Secret
+import scenario
 
-state = State(
+state = scenario.State(
     secrets=[
-        Secret(
+        scenario.Secret(
             id='foo',
             contents={0: {'key': 'private'}},
             owner='unit',  # or 'app'
             remote_grants={0: {"remote"}}
             # the secret owner has granted access to the "remote" app over some relation with ID 0
         )
     ]
 )
 ```
 
 To specify a secret owned by some other application and give this unit (or app) access to it:
 
 ```python
-from scenario import State, Secret
+import scenario
 
-state = State(
+state = scenario.State(
     secrets=[
-        Secret(
+        scenario.Secret(
             id='foo',
             contents={0: {'key': 'public'}},
             # owner=None, which is the default
             revision=0,  # the revision that this unit (or app) is currently tracking
         )
     ]
 )
 ```
 
+## StoredState
+
+Scenario can simulate StoredState. You can define it on the input side as:
+
+```python
+import ops
+import scenario
+
+from ops.charm import CharmBase
+
+
+class MyCharmType(ops.CharmBase):
+    my_stored_state = ops.StoredState()
+
+    def __init__(self, framework):
+        super().__init__(framework)
+        assert self.my_stored_state.foo == 'bar'  # this will pass!
+
+
+state = scenario.State(stored_state=[
+    scenario.StoredState(
+        owner_path="MyCharmType",
+        name="my_stored_state",
+        content={
+            'foo': 'bar',
+            'baz': {42: 42},
+        })
+])
+```
+
+And the charm's runtime will see `self.my_stored_state.foo` and `.baz` as expected. Also, you can run assertions on it on
+the output side the same as any other bit of state.
+
+## Resources
+
+If your charm requires access to resources, you can make them available to it through `State.resources`.
+From the perspective of a 'real' deployed charm, if your charm _has_ resources defined in its metadata, they _must_ be made available to the charm. That is a Juju-enforced constraint: you can't deploy a charm without attaching all resources it needs to it.
+However, when testing, this constraint is unnecessarily strict (and it would also mean the great majority of all existing tests would break) since a charm will only notice that a resource is not available when it explicitly asks for it, which not many charms do.
+
+So, the only consistency-level check we enforce in Scenario when it comes to resource is that if a resource is provided in State, it needs to have been declared in the metadata.
+
+```python
+import scenario
+
+ctx = scenario.Context(MyCharm, meta={'name': 'juliette', "resources": {"foo": {"type": "oci-image"}}})
+with ctx.manager("start", scenario.State(resources={'foo': '/path/to/resource.tar'})) as mgr:
+    # If the charm, at runtime, were to call self.model.resources.fetch("foo"), it would get '/path/to/resource.tar' back.
+    path = mgr.charm.model.resources.fetch('foo')
+    assert path == '/path/to/resource.tar'
+```
+
+## Model
+
+Charms don't usually need to be aware of the model in which they are deployed,
+but if you need to set the model name or UUID, you can provide a `scenario.Model`
+to the state:
+
+```python
+import ops
+import scenario
+
+class MyCharm(ops.CharmBase):
+    pass
+
+ctx = scenario.Context(MyCharm, meta={"name": "foo"})
+state_in = scenario.State(model=scenario.Model(name="my-model"))
+out = ctx.run("start", state_in)
+assert out.model.name == "my-model"
+assert out.model.uuid == state_in.model.uuid
+```
+
+## CloudSpec
+
+You can set CloudSpec information in the state (only `type` and `name` are required).
+
+Example:
+
+```python
+import scenario
+
+state = scenario.State(
+    cloud_spec=scenario.CloudSpec(
+        type="lxd",
+        name="localhost",
+        endpoint="https://127.0.0.1:8443",
+        credential=scenario.CloudCredential(
+            auth_type="clientcertificate",
+            attributes={
+                "client-cert": "foo",
+                "client-key": "bar",
+                "server-cert": "baz",
+            },
+        ),
+    ),
+    model=scenario.Model(name="my-vm-model", type="lxd"),
+)
+```
+
+Then you can access it by `Model.get_cloud_spec()`:
+
+```python
+# charm.py
+class MyVMCharm(ops.CharmBase):
+    def __init__(self, framework: ops.Framework):
+        super().__init__(framework)
+        framework.observe(self.on.start, self._on_start)
+
+    def _on_start(self, event: ops.StartEvent):
+        self.cloud_spec = self.model.get_cloud_spec()
+```
+
 # Actions
 
 An action is a special sort of event, even though `ops` handles them almost identically.
 In most cases, you'll want to inspect the 'results' of an action, or whether it has failed or
 logged something while executing. Many actions don't have a direct effect on the output state.
 For this reason, the output state is less prominent in the return type of `Context.run_action`.
 
 How to test actions with scenario:
 
 ## Actions without parameters
 
 ```python
-from scenario import Context, State, ActionOutput
+import scenario
+
 from charm import MyCharm
 
 
 def test_backup_action():
-    ctx = Context(MyCharm)
+    ctx = scenario.Context(MyCharm)
 
-    # If you didn't declare do_backup in the charm's `actions.yaml`, 
+    # If you didn't declare do_backup in the charm's metadata, 
     # the `ConsistencyChecker` will slap you on the wrist and refuse to proceed.
-    out: ActionOutput = ctx.run_action("do_backup_action", State())
+    out: scenario.ActionOutput = ctx.run_action("do_backup_action", scenario.State())
 
-    # you can assert action results, logs, failure using the ActionOutput interface
+    # You can assert action results, logs, failure using the ActionOutput interface:
     assert out.logs == ['baz', 'qux']
     
     if out.success:
-      # if the action did not fail, we can read the results:
+      # If the action did not fail, we can read the results:
       assert out.results == {'foo': 'bar'}
 
     else:
-      # if the action fails, we can read a failure message
+      # If the action fails, we can read a failure message:
       assert out.failure == 'boo-hoo'
 ```
 
 ## Parametrized Actions
 
 If the action takes parameters, you'll need to instantiate an `Action`.
 
 ```python
-from scenario import Action, Context, State, ActionOutput
+import scenario
+
 from charm import MyCharm
 
 
 def test_backup_action():
-    # define an action
-    action = Action('do_backup', params={'a': 'b'})
-    ctx = Context(MyCharm)
-
-    # if the parameters (or their type) don't match what declared in actions.yaml, 
-    # the `ConsistencyChecker` will slap you on the other wrist. 
-    out: ActionOutput = ctx.run_action(action, State())
+    # Define an action:
+    action = scenario.Action('do_backup', params={'a': 'b'})
+    ctx = scenario.Context(MyCharm)
+
+    # If the parameters (or their type) don't match what is declared in the metadata, 
+    # the `ConsistencyChecker` will slap you on the other wrist.
+    out: scenario.ActionOutput = ctx.run_action(action, scenario.State())
 
     # ...
 ```
 
 # Deferred events
 
 Scenario allows you to accurately simulate the Operator Framework's event queue. The event queue is responsible for
 keeping track of the deferred events. On the input side, you can verify that if the charm triggers with this and that
 event in its queue (they would be there because they had been deferred in the previous run), then the output state is
 valid.
 
 ```python
-from scenario import State, deferred, Context
+import scenario
 
 
 class MyCharm(...):
     ...
 
-    def _on_update_status(self, e):
-        e.defer()
+    def _on_update_status(self, event):
+        event.defer()
 
-    def _on_start(self, e):
-        e.defer()
+    def _on_start(self, event):
+        event.defer()
 
 
 def test_start_on_deferred_update_status(MyCharm):
     """Test charm execution if a 'start' is dispatched when in the previous run an update-status had been deferred."""
-    state_in = State(
+    state_in = scenario.State(
         deferred=[
-            deferred('update_status',
-                     handler=MyCharm._on_update_status)
+            scenario.deferred('update_status', handler=MyCharm._on_update_status)
         ]
     )
-    state_out = Context(MyCharm).run('start', state_in)
+    state_out = scenario.Context(MyCharm).run('start', state_in)
     assert len(state_out.deferred) == 1
     assert state_out.deferred[0].name == 'start'
 ```
 
 You can also generate the 'deferred' data structure (called a DeferredEvent) from the corresponding Event (and the
 handler):
 
 ```python
-from scenario import Event, Relation
+import scenario
 
 
 class MyCharm(...):
     ...
 
 
-deferred_start = Event('start').deferred(MyCharm._on_start)
-deferred_install = Event('install').deferred(MyCharm._on_start)
-```
-
-## relation events:
-
-```python
-foo_relation = Relation('foo')
-deferred_relation_changed_evt = foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
+deferred_start = scenario.Event('start').deferred(MyCharm._on_start)
+deferred_install = scenario.Event('install').deferred(MyCharm._on_start)
 ```
 
 On the output side, you can verify that an event that you expect to have been deferred during this trigger, has indeed
 been deferred.
 
 ```python
-from scenario import State, Context
+import scenario
 
 
 class MyCharm(...):
     ...
 
-    def _on_start(self, e):
-        e.defer()
+    def _on_start(self, event):
+        event.defer()
 
 
 def test_defer(MyCharm):
-    out = Context(MyCharm).run('start', State())
+    out = scenario.Context(MyCharm).run('start', scenario.State())
     assert len(out.deferred) == 1
     assert out.deferred[0].name == 'start'
 ```
 
 ## Deferring relation events
 
 If you want to test relation event deferrals, some extra care needs to be taken. RelationEvents hold references to the
 Relation instance they are about. So do they in Scenario. You can use the deferred helper to generate the data
 structure:
 
 ```python
-from scenario import State, Relation, deferred
+import scenario
 
 
 class MyCharm(...):
     ...
 
-    def _on_foo_relation_changed(self, e):
-        e.defer()
+    def _on_foo_relation_changed(self, event):
+        event.defer()
 
 
 def test_start_on_deferred_update_status(MyCharm):
-    foo_relation = Relation('foo')
-    State(
+    foo_relation = scenario.Relation('foo')
+    scenario.State(
         relations=[foo_relation],
         deferred=[
-            deferred('foo_relation_changed',
-                     handler=MyCharm._on_foo_relation_changed,
-                     relation=foo_relation)
+            scenario.deferred('foo_relation_changed',
+                              handler=MyCharm._on_foo_relation_changed,
+                              relation=foo_relation)
         ]
     )
 ```
 
-but you can also use a shortcut from the relation event itself, as mentioned above:
+but you can also use a shortcut from the relation event itself:
 
 ```python
-
-from scenario import Relation
+import scenario
 
 
 class MyCharm(...):
     ...
 
 
-foo_relation = Relation('foo')
+foo_relation = scenario.Relation('foo')
 foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
 ```
 
-### Fine-tuning
+## Fine-tuning
 
 The deferred helper Scenario provides will not support out of the box all custom event subclasses, or events emitted by
 charm libraries or objects other than the main charm class.
 
 For general-purpose usage, you will need to instantiate DeferredEvent directly.
 
 ```python
-from scenario import DeferredEvent
+import scenario
 
-my_deferred_event = DeferredEvent(
+my_deferred_event = scenario.DeferredEvent(
     handle_path='MyCharm/MyCharmLib/on/database_ready[1]',
     owner='MyCharmLib',  # the object observing the event. Could also be MyCharm.
     observer='_on_database_ready'
 )
 ```
 
-# StoredState
-
-Scenario can simulate StoredState. You can define it on the input side as:
-
-```python
-from ops.charm import CharmBase
-from ops.framework import StoredState as Ops_StoredState, Framework
-from scenario import State, StoredState
-
-
-class MyCharmType(CharmBase):
-    my_stored_state = Ops_StoredState()
-
-    def __init__(self, framework: Framework):
-        super().__init__(framework)
-        assert self.my_stored_state.foo == 'bar'  # this will pass!
-
-
-state = State(stored_state=[
-    StoredState(
-        owner_path="MyCharmType",
-        name="my_stored_state",
-        content={
-            'foo': 'bar',
-            'baz': {42: 42},
-        })
-])
-```
-
-And the charm's runtime will see `self.stored_State.foo` and `.baz` as expected. Also, you can run assertions on it on
-the output side the same as any other bit of state.
-
-# Resources
-
-If your charm requires access to resources, you can make them available to it through `State.resources`.
-From the perspective of a 'real' deployed charm, if your charm _has_ resources defined in `metadata.yaml`, they _must_ be made available to the charm. That is a Juju-enforced constraint: you can't deploy a charm without attaching all resources it needs to it.
-However, when testing, this constraint is unnecessarily strict (and it would also mean the great majority of all existing tests would break) since a charm will only notice that a resource is not available when it explicitly asks for it, which not many charms do.
-
-So, the only consistency-level check we enforce in Scenario when it comes to resource is that if a resource is provided in State, it needs to have been declared in metadata.
-
-```python
-from scenario import State, Context
-ctx = Context(MyCharm, meta={'name': 'juliette', "resources": {"foo": {"type": "oci-image"}}})
-with ctx.manager("start", State(resources={'foo': '/path/to/resource.tar'})) as mgr:
-    # if the charm, at runtime, were to call self.model.resources.fetch("foo"), it would get '/path/to/resource.tar' back.
-    path = mgr.charm.model.resources.fetch('foo')
-    assert path == '/path/to/resource.tar' 
-```
-
 # Emitting custom events
 
-While the main use case of Scenario is to emit juju events, i.e. the built-in `start`, `install`, `*-relation-changed`,
+While the main use case of Scenario is to emit Juju events, i.e. the built-in `start`, `install`, `*-relation-changed`,
 etc..., it can be sometimes handy to directly trigger custom events defined on arbitrary Objects in your hierarchy.
 
 Suppose your charm uses a charm library providing an `ingress_provided` event.
 The 'proper' way to emit it is to run the event that causes that custom event to be emitted by the library, whatever
 that may be, for example a `foo-relation-changed`.
 
 However, that may mean that you have to set up all sorts of State and mocks so that the right preconditions are met and
 the event is emitted at all.
 
 If for whatever reason you don't want to do that and you attempt to run that event directly you will get an error:
 
 ```python
-from scenario import Context, State
+import scenario
 
-Context(...).run("ingress_provided", State())  # raises scenario.ops_main_mock.NoObserverError
+scenario.Context(...).run("ingress_provided", scenario.State())  # raises scenario.ops_main_mock.NoObserverError
 ```
 
 This happens because the framework, by default, searches for an event source named `ingress_provided` in `charm.on`, but
 since the event is defined on another Object, it will fail to find it.
 
 You can prefix the event name with the path leading to its owner to tell Scenario where to find the event source:
 
 ```python
-from scenario import Context, State
+import scenario
 
-Context(...).run("my_charm_lib.on.foo", State())
+scenario.Context(...).run("my_charm_lib.on.foo", scenario.State())
 ```
 
 This will instruct Scenario to emit `my_charm.my_charm_lib.on.foo`.
 
 (always omit the 'root', i.e. the charm framework key, from the path)
 
 # Live charm introspection
@@ -1164,158 +1236,155 @@
 Scenario is a black-box, state-transition testing framework. It makes it trivial to assert that a status went from A to
 B, but not to assert that, in the context of this charm execution, with this state, a certain charm-internal method was called and returned a
 given piece of data, or would return this and that _if_ it had been called.
 
 Scenario offers a cheekily-named context manager for this use case specifically:
 
 ```python
-from ops import CharmBase, StoredState
+import ops
+import scenario
 
 from charms.bar.lib_name.v1.charm_lib import CharmLib
-from scenario import Context, State
 
 
-class MyCharm(CharmBase):
+class MyCharm(ops.CharmBase):
     META = {"name": "mycharm"}
-    _stored = StoredState()
+    _stored = ops.StoredState()
     
     def __init__(self, framework):
         super().__init__(framework)
         self._stored.set_default(a="a")
         self.my_charm_lib = CharmLib()
         framework.observe(self.on.start, self._on_start)
 
     def _on_start(self, event):
         self._stored.a = "b"
 
 
 def test_live_charm_introspection(mycharm):
-    ctx = Context(mycharm, meta=mycharm.META)
+    ctx = scenario.Context(mycharm, meta=mycharm.META)
     # If you want to do this with actions, you can use `Context.action_manager` instead.
-    with ctx.manager("start", State()) as manager:
-        # this is your charm instance, after ops has set it up
+    with ctx.manager("start", scenario.State()) as manager:
+        # This is your charm instance, after ops has set it up:
         charm: MyCharm = manager.charm
         
-        # we can check attributes on nested Objects or the charm itself 
+        # We can check attributes on nested Objects or the charm itself:
         assert charm.my_charm_lib.foo == "foo"
-        # such as stored state
+        # such as stored state:
         assert charm._stored.a == "a"
 
-        # this will tell ops.main to proceed with normal execution and emit the "start" event on the charm
+        # This will tell ops.main to proceed with normal execution and emit the "start" event on the charm:
         state_out = manager.run()
     
-        # after that is done, we are handed back control, and we can again do some introspection
+        # After that is done, we are handed back control, and we can again do some introspection:
         assert charm.my_charm_lib.foo == "bar"
-        # and check that the charm's internal state is as we expect
+        # and check that the charm's internal state is as we expect:
         assert charm._stored.a == "b"
 
     # state_out is, as in regular scenario tests, a State object you can assert on:
     assert state_out.unit_status == ...
 ```
 
 Note that you can't call `manager.run()` multiple times: the manager is a context that ensures that `ops.main` 'pauses' right
 before emitting the event to hand you some introspection hooks, but for the rest this is a regular scenario test: you
 can't emit multiple events in a single charm execution.
 
 # The virtual charm root
 
 Before executing the charm, Scenario copies the charm's `/src`, any libs, the metadata, config, and actions `yaml`s to a temporary directory. The
-charm will see that tempdir as its 'root'. This allows us to keep things simple when dealing with metadata that can be
+charm will see that temporary directory as its 'root'. This allows us to keep things simple when dealing with metadata that can be
 either inferred from the charm type being passed to `Context` or be passed to it as an argument, thereby overriding
 the inferred one. This also allows you to test charms defined on the fly, as in:
 
 ```python
-from ops.charm import CharmBase
-from scenario import State, Context
+import ops
+import scenario
 
 
-class MyCharmType(CharmBase):
+class MyCharmType(ops.CharmBase):
     pass
 
 
-ctx = Context(charm_type=MyCharmType,
-              meta={'name': 'my-charm-name'})
+ctx = scenario.Context(charm_type=MyCharmType, meta={'name': 'my-charm-name'})
 ctx.run('start', State())
 ```
 
-A consequence of this fact is that you have no direct control over the tempdir that we are creating to put the metadata
+A consequence of this fact is that you have no direct control over the temporary directory that we are creating to put the metadata
 you are passing to `.run()` (because `ops` expects it to be a file...). That is, unless you pass your own:
 
 ```python
-from ops.charm import CharmBase
-from scenario import State, Context
 import tempfile
 
+import ops
+import scenario
+
 
-class MyCharmType(CharmBase):
+class MyCharmType(ops.CharmBase):
     pass
 
 
 td = tempfile.TemporaryDirectory()
-state = Context(
+state = scenario.Context(
     charm_type=MyCharmType,
     meta={'name': 'my-charm-name'},
     charm_root=td.name
-).run('start', State())
+).run('start', scenario.State())
 ```
 
 Do this, and you will be able to set up said directory as you like before the charm is run, as well as verify its
 contents after the charm has run. Do keep in mind that any metadata files you create in it will be overwritten by Scenario, and therefore
 ignored, if you pass any metadata keys to `Context`. Omit `meta` in the call
-above, and Scenario will instead attempt to read `metadata.yaml` from the
+above, and Scenario will instead attempt to read metadata from the
 temporary directory.
 
-
 # Immutability
 
-All of the data structures in `state`, e.g. `State, Relation, Container`, etc... are immutable (implemented as frozen
-dataclasses).
+All of the data structures in `state`, e.g. `State, Relation, Container`, etc... are implemented as frozen dataclasses.
 
 This means that all components of the state that goes into a `context.run()` call are not mutated by the call, and the
 state that you obtain in return is a different instance, and all parts of it have been (deep)copied.
-This ensures that you can do delta-based comparison of states without worrying about them being mutated by scenario.
+This ensures that you can do delta-based comparison of states without worrying about them being mutated by Scenario.
 
 If you want to modify any of these data structures, you will need to either reinstantiate it from scratch, or use
 the `replace` api.
 
 ```python
-from scenario import Relation
+import scenario
 
-relation = Relation('foo', remote_app_data={"1": "2"})
+relation = scenario.Relation('foo', remote_app_data={"1": "2"})
 # make a copy of relation, but with remote_app_data set to {"3", "4"} 
 relation2 = relation.replace(remote_app_data={"3", "4"})
 ```
 
 # Consistency checks
 
 A Scenario, that is, the combination of an event, a state, and a charm, is consistent if it's plausible in JujuLand. For
 example, Juju can't emit a `foo-relation-changed` event on your charm unless your charm has declared a `foo` relation
-endpoint in its `metadata.yaml`. If that happens, that's a juju bug. Scenario however assumes that Juju is bug-free,
+endpoint in its metadata. If that happens, that's a Juju bug. Scenario however assumes that Juju is bug-free,
 therefore, so far as we're concerned, that can't happen, and therefore we help you verify that the scenarios you create
 are consistent and raise an exception if that isn't so.
 
 That happens automatically behind the scenes whenever you trigger an event;
 `scenario.consistency_checker.check_consistency` is called and verifies that the scenario makes sense.
 
 ## Caveats:
 
 - False positives: not all checks are implemented yet; more will come.
 - False negatives: it is possible that a scenario you know to be consistent is seen as inconsistent. That is probably a
-  bug in the consistency checker itself, please report it.
+  bug in the consistency checker itself; please report it.
 - Inherent limitations: if you have a custom event whose name conflicts with a builtin one, the consistency constraints
   of the builtin one will apply. For example: if you decide to name your custom event `bar-pebble-ready`, but you are
   working on a machine charm or don't have either way a `bar` container in your `metadata.yaml`, Scenario will flag that
   as inconsistent.
 
 ## Bypassing the checker
 
 If you have a clear false negative, are explicitly testing 'edge', inconsistent situations, or for whatever reason the
 checker is in your way, you can set the `SCENARIO_SKIP_CONSISTENCY_CHECKS` envvar and skip it altogether. Hopefully you
 don't need that.
 
 # Jhack integrations
 
-Up until `v5.6.0`, `scenario` shipped with a cli tool called `snapshot`, used to interact with a live charm's state.
+Up until `v5.6.0`, Scenario shipped with a cli tool called `snapshot`, used to interact with a live charm's state.
 The functionality [has been moved over to `jhack`](https://github.com/PietroPasotti/jhack/pull/111), 
 to allow us to keep working on it independently, and to streamline 
-the profile of `scenario` itself as it becomes more broadly adopted and ready for widespread usage.
-
+the profile of Scenario itself as it becomes more broadly adopted and ready for widespread usage.
```

### Comparing `ops-scenario-6.0.3/ops_scenario.egg-info/PKG-INFO` & `ops_scenario-6.0.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: ops-scenario
-Version: 6.0.3
-Summary: Python library providing a state-transition testing API for Operator Framework charms.
-Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/canonical/ops-scenario
-Project-URL: Bug Tracker, https://github.com/canonical/ops-scenario/issues
-Keywords: juju,test
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Framework :: Pytest
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: ops>=2.6
-Requires-Dist: PyYAML>=6.0.1
-
 # Scenario
 
 [![Build](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml)
 [![QC](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml/badge.svg?event=pull_request)](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml?event=pull_request)
 [![Discourse Status](https://img.shields.io/discourse/status?server=https%3A%2F%2Fdiscourse.charmhub.io&style=flat&label=CharmHub%20Discourse)](https://discourse.charmhub.io)
 [![foo](https://img.shields.io/badge/everything-charming-blueviolet)](https://github.com/PietroPasotti/jhack)
 [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://discourse.charmhub.io/t/rethinking-charm-testing-with-ops-scenario/8649)
@@ -36,54 +14,54 @@
 event on the charm and execute its logic.
 
 This puts scenario tests somewhere in between unit and integration tests: some say 'functional', some say 'contract', I prefer 'state-transition'.
 
 Scenario tests nudge you into thinking of a charm as an input->output function. The input is the
 union of an `Event` (why am I, charm, being executed), a `State` (am I leader? what is my relation data? what is my
 config?...) and the charm's execution `Context` (what relations can I have? what containers can I have?...). The output is another `State`: the state after the charm has had a chance to interact with the
-mocked juju model and affect the initial state back.
+mocked Juju model and affect the initial state back.
 
 ![state transition model depiction](resources/state-transition-model.png)
 
 For example: a charm currently in `unknown` status is executed with a `start` event, and based on whether it has leadership or not (according to its input state), it will decide to set `active` or `blocked` status (which will be reflected in the output state).
 
 Scenario-testing a charm, then, means verifying that:
 
 - the charm does not raise uncaught exceptions while handling the event
 - the output state (or the diff with the input state) is as expected.
 
-# Core concepts as a metaphor
+## Core concepts as a metaphor
 
 I like metaphors, so here we go:
 
 - There is a theatre stage.
 - You pick an actor (a Charm) to put on the stage. Not just any actor: an improv one.
 - You arrange the stage with content that the actor will have to interact with. This consists of selecting:
     - An initial situation (`State`) in which the actor is, e.g. is the actor the main role or an NPC (`is_leader`), or what
       other actors are there around it, what is written in those pebble-shaped books on the table?
     - Something that has just happened (an `Event`) and to which the actor has to react (e.g. one of the NPCs leaves the
       stage (`relation-departed`), or the content of one of the books changes).
 - How the actor will react to the event will have an impact on the context: e.g. the actor might knock over a table (a
   container), or write something down into one of the books.
 
-# Core concepts not as a metaphor
+## Core concepts not as a metaphor
 
 Scenario tests are about running assertions on atomic state transitions treating the charm being tested like a black
 box. An initial state goes in, an event occurs (say, `'start'`) and a new state comes out. Scenario tests are about
 validating the transition, that is, consistency-checking the delta between the two states, and verifying the charm
 author's expectations.
 
 Comparing scenario tests with `Harness` tests:
 
 - Harness exposes an imperative API: the user is expected to call methods on the Harness driving it to the desired
   state, then verify its validity by calling charm methods or inspecting the raw data. In contrast, Scenario is declarative. You fully specify an initial state, an execution context and an event, then you run the charm and inspect the results.
 - Harness instantiates the charm once, then allows you to fire multiple events on the charm, which is breeding ground
   for subtle bugs. Scenario tests are centered around testing single state transitions, that is, one event at a time.
   This ensures that the execution environment is as clean as possible (for a unit test).
-- Harness maintains a model of the juju Model, which is a maintenance burden and adds complexity. Scenario mocks at the
+- Harness maintains a model of the Juju Model, which is a maintenance burden and adds complexity. Scenario mocks at the
   level of hook tools and stores all mocking data in a monolithic data structure (the State), which makes it more
   lightweight and portable.
 
 # Writing scenario tests
 
 A scenario test consists of three broad steps:
 
@@ -100,430 +78,422 @@
 
 The most basic scenario is one in which all is defaulted and barely any data is
 available. The charm has no config, no relations, no leadership, and its status is `unknown`.
 
 With that, we can write the simplest possible scenario test:
 
 ```python
-from scenario import State, Context, Event
-from ops.charm import CharmBase
-from ops.model import UnknownStatus
+import ops
+import scenario
 
 
-class MyCharm(CharmBase):
+class MyCharm(ops.CharmBase):
     pass
 
 
 def test_scenario_base():
-    ctx = Context(MyCharm, meta={"name": "foo"})
-    out = ctx.run(Event("start"), State())
-    assert out.unit_status == UnknownStatus()
+    ctx = scenario.Context(MyCharm, meta={"name": "foo"})
+    out = ctx.run(scenario.Event("start"), scenario.State())
+    assert out.unit_status == ops.UnknownStatus()
 ```
 
 Now let's start making it more complicated. Our charm sets a special state if it has leadership on 'start':
 
 ```python
+import ops
 import pytest
-from scenario import State, Context
-from ops.charm import CharmBase
-from ops.model import ActiveStatus
+import scenario
 
 
-class MyCharm(CharmBase):
-    def __init__(self, ...):
-        self.framework.observe(self.on.start, self._on_start)
+class MyCharm(ops.CharmBase):
+    def __init__(self, framework):
+        super().__init__(framework)
+        framework.observe(self.on.start, self._on_start)
 
     def _on_start(self, _):
         if self.unit.is_leader():
-            self.unit.status = ActiveStatus('I rule')
+            self.unit.status = ops.ActiveStatus('I rule')
         else:
-            self.unit.status = ActiveStatus('I am ruled')
+            self.unit.status = ops.ActiveStatus('I am ruled')
 
 
 @pytest.mark.parametrize('leader', (True, False))
 def test_status_leader(leader):
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-    out = ctx.run('start', State(leader=leader))
-    assert out.unit_status == ActiveStatus('I rule' if leader else 'I am ruled')
+    ctx = scenario.Context(MyCharm, meta={"name": "foo"})
+    out = ctx.run('start', scenario.State(leader=leader))
+    assert out.unit_status == ops.ActiveStatus('I rule' if leader else 'I am ruled')
 ```
 
 By defining the right state we can programmatically define what answers will the charm get to all the questions it can
-ask the juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
+ask the Juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
 
 ## Statuses
 
 One of the simplest types of black-box testing available to charmers is to execute the charm and verify that the charm
 sets the expected unit/application status. We have seen a simple example above including leadership. But what if the
 charm transitions through a sequence of statuses?
 
 ```python
-from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, BlockedStatus
+import ops
 
 
 # charm code:
 def _on_event(self, _event):
-    self.unit.status = MaintenanceStatus('determining who the ruler is...')
+    self.unit.status = ops.MaintenanceStatus('determining who the ruler is...')
     try:
-        if self._call_that_takes_a_few_seconds_and_only_passes_on_leadership:
-            self.unit.status = ActiveStatus('I rule')
+        if self._call_that_takes_a_few_seconds_and_only_passes_on_leadership():
+            self.unit.status = ops.ActiveStatus('I rule')
         else:
-            self.unit.status = WaitingStatus('checking this is right...')
+            self.unit.status = ops.WaitingStatus('checking this is right...')
             self._check_that_takes_some_more_time()
-            self.unit.status = ActiveStatus('I am ruled')
+            self.unit.status = ops.ActiveStatus('I am ruled')
     except:
-        self.unit.status = BlockedStatus('something went wrong')
+        self.unit.status = ops.BlockedStatus('something went wrong')
 ```
 
 More broadly, often we want to test 'side effects' of executing a charm, such as what events have been emitted, what
 statuses it went through, etc... Before we get there, we have to explain what the `Context` represents, and its
 relationship with the `State`.
 
-# Context and State
+## Context and State
 
-Consider the following tests. Suppose we want to verify that while handling a given toplevel juju event:
+Consider the following tests. Suppose we want to verify that while handling a given top-level Juju event:
 
 - a specific chain of (custom) events was emitted on the charm
 - the charm `juju-log`ged these specific strings
 - the charm went through this sequence of app/unit statuses (e.g. `maintenance`, then `waiting`, then `active`)
 
-These types of test have a place in Scenario, but that is not State: the contents of the juju log or the status history
+These types of test have a place in Scenario, but that is not State: the contents of the Juju log or the status history
 are side effects of executing a charm, but are not persisted in a charm-accessible "state" in any meaningful way.
 In other words: those data streams are, from the charm's perspective, write-only.
 
 As such, they do not belong in `scenario.State` but in `scenario.Context`: the object representing the charm's execution
 context.
 
 ## Status history
 
 You can verify that the charm has followed the expected path by checking the unit/app status history like so:
 
 ```python
+import ops
+import scenario
 from charm import MyCharm
-from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, UnknownStatus
-from scenario import State, Context
 
 
 def test_statuses():
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-    ctx.run('start', State(leader=False))
+    ctx = scenario.Context(MyCharm, meta={"name": "foo"})
+    out = ctx.run('start', scenario.State(leader=False))
     assert ctx.unit_status_history == [
-        UnknownStatus(),
-        MaintenanceStatus('determining who the ruler is...'),
-        WaitingStatus('checking this is right...'),
-        ActiveStatus("I am ruled"),
+        ops.UnknownStatus(),
+        ops.MaintenanceStatus('determining who the ruler is...'),
+        ops.WaitingStatus('checking this is right...'),
     ]
+    assert out.unit_status == ops.ActiveStatus("I am ruled"),
     
     # similarly you can check the app status history:
     assert ctx.app_status_history == [
-        UnknownStatus(),
+        ops.UnknownStatus(),
         ...
     ]
 ```
 
-Note that the current status is not in the **unit status history**.
+Note that the *current* status is **not** in the unit status history.
 
 Also note that, unless you initialize the State with a preexisting status, the first status in the history will always
-be `unknown`. That is because, so far as scenario is concerned, each event is "the first event this charm has ever
+be `unknown`. That is because, so far as Scenario is concerned, each event is "the first event this charm has ever
 seen".
 
 If you want to simulate a situation in which the charm already has seen some event, and is in a status other than
 Unknown (the default status every charm is born with), you will have to pass the 'initial status' to State.
 
 ```python
-from ops.model import ActiveStatus
-from scenario import State, Status
+import ops
+import scenario
 
 # ...
-ctx.run('start', State(unit_status=ActiveStatus('foo')))
+ctx.run('start', scenario.State(unit_status=ops.ActiveStatus('foo')))
 assert ctx.unit_status_history == [
-    ActiveStatus('foo'),  # now the first status is active: 'foo'!
+    ops.ActiveStatus('foo'),  # now the first status is active: 'foo'!
     # ...
 ]
-
 ```
 
 ## Workload version history
 
 Using a similar api to `*_status_history`, you can assert that the charm has set one or more workload versions during a
 hook execution:
 
 ```python
-from scenario import Context
+import scenario
 
 # ...
-ctx: Context
+ctx: scenario.Context
 assert ctx.workload_version_history == ['1', '1.2', '1.5']
 # ...
 ```
 
+Note that the *current* version is not in the version history, as with the status history.
+
 ## Emitted events
 
 If your charm deals with deferred events, custom events, and charm libs that in turn emit their own custom events, it
 can be hard to examine the resulting control flow. In these situations it can be useful to verify that, as a result of a
 given Juju event triggering (say, 'start'), a specific chain of events is emitted on the charm. The
 resulting state, black-box as it is, gives little insight into how exactly it was obtained.
 
 ```python
-from scenario import Context
-from ops.charm import StartEvent
+import ops
+import scenario
 
 
 def test_foo():
-    ctx = Context(...)
+    ctx = scenario.Context(...)
     ctx.run('start', ...)
 
     assert len(ctx.emitted_events) == 1
-    assert isinstance(ctx.emitted_events[0], StartEvent)
+    assert isinstance(ctx.emitted_events[0], ops.StartEvent)
 ```
 
 You can configure what events will be captured by passing the following arguments to `Context`:
 -  `capture_deferred_events`: If you want to include re-emitted deferred events.
 -  `capture_framework_events`: If you want to include framework events (`pre-commit`, `commit`, and `collect-status`). 
 
 For example:
 ```python
-from scenario import Context, Event, State
+import scenario
 
 def test_emitted_full():
-    ctx = Context(
+    ctx = scenario.Context(
         MyCharm,
         capture_deferred_events=True,
         capture_framework_events=True,
     )
-    ctx.run("start", State(deferred=[Event("update-status").deferred(MyCharm._foo)]))
+    ctx.run("start", scenario.State(deferred=[scenario.Event("update-status").deferred(MyCharm._foo)]))
 
     assert len(ctx.emitted_events) == 5
     assert [e.handle.kind for e in ctx.emitted_events] == [
         "update_status",
         "start",
         "collect_unit_status",
         "pre_commit",
         "commit",
     ]
 ```
 
-
 ### Low-level access: using directly `capture_events`
 
 If you need more control over what events are captured (or you're not into pytest), you can use directly the context
 manager that powers the `emitted_events` fixture: `scenario.capture_events`.
 This context manager allows you to intercept any events emitted by the framework.
 
 Usage:
 
 ```python
-from ops.charm import StartEvent, UpdateStatusEvent
-from scenario import State, Context, DeferredEvent, capture_events
+import ops
+import scenario
 
 with capture_events() as emitted:
-    ctx = Context(...)
+    ctx = scenario.Context(...)
     state_out = ctx.run(
         "update-status",
-        State(deferred=[DeferredEvent("start", ...)])
+        scenario.State(deferred=[scenario.DeferredEvent("start", ...)])
     )
 
 # deferred events get reemitted first
-assert isinstance(emitted[0], StartEvent)
-# the main juju event gets emitted next
-assert isinstance(emitted[1], UpdateStatusEvent)
-# possibly followed by a tail of all custom events that the main juju event triggered in turn
+assert isinstance(emitted[0], ops.StartEvent)
+# the main Juju event gets emitted next
+assert isinstance(emitted[1], ops.UpdateStatusEvent)
+# possibly followed by a tail of all custom events that the main Juju event triggered in turn
 # assert isinstance(emitted[2], MyFooEvent)
 # ...
 ```
 
 You can filter events by type like so:
 
 ```python
-from ops.charm import StartEvent, RelationEvent
-from scenario import capture_events
+import ops
 
-with capture_events(StartEvent, RelationEvent) as emitted:
+with capture_events(ops.StartEvent, ops.RelationEvent) as emitted:
     # capture all `start` and `*-relation-*` events.
     pass
 ```
 
 Configuration:
 
-- Passing no event types, like: `capture_events()`, is equivalent to `capture_events(EventBase)`.
+- Passing no event types, like: `capture_events()`, is equivalent to `capture_events(ops.EventBase)`.
 - By default, **framework events** (`PreCommit`, `Commit`) are not considered for inclusion in the output list even if
   they match the instance check. You can toggle that by passing: `capture_events(include_framework=True)`.
 - By default, **deferred events** are included in the listing if they match the instance check. You can toggle that by
   passing: `capture_events(include_deferred=False)`.
 
 ## Relations
 
 You can write scenario tests to verify the shape of relation data:
 
 ```python
-from ops.charm import CharmBase
-
-from scenario import Relation, State, Context
+import ops
+import scenario
 
 
 # This charm copies over remote app data to local unit data
-class MyCharm(CharmBase):
+class MyCharm(ops.CharmBase):
     ...
 
-    def _on_event(self, e):
-        rel = e.relation
+    def _on_event(self, event):
+        rel = event.relation
         assert rel.app.name == 'remote'
         assert rel.data[self.unit]['abc'] == 'foo'
-        rel.data[self.unit]['abc'] = rel.data[e.app]['cde']
+        rel.data[self.unit]['abc'] = rel.data[event.app]['cde']
 
 
 def test_relation_data():
-    state_in = State(relations=[
-        Relation(
+    state_in = scenario.State(relations=[
+        scenario.Relation(
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "foo"},
             remote_app_data={"cde": "baz!"},
         ),
     ])
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
+    ctx = scenario.Context(MyCharm, meta={"name": "foo"})
 
     state_out = ctx.run('start', state_in)
 
     assert state_out.relations[0].local_unit_data == {"abc": "baz!"}
     # you can do this to check that there are no other differences:
     assert state_out.relations == [
-        Relation(
+        scenario.Relation(
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "baz!"},
             remote_app_data={"cde": "baz!"},
         ),
     ]
 
 # which is very idiomatic and superbly explicit. Noice.
 ```
 
 The only mandatory argument to `Relation` (and other relation types, see below) is `endpoint`. The `interface` will be
-derived from the charm's `metadata.yaml`. When fully defaulted, a relation is 'empty'. There are no remote units, the
+derived from the charm's metadata. When fully defaulted, a relation is 'empty'. There are no remote units, the
 remote application is called `'remote'` and only has a single unit `remote/0`, and nobody has written any data to the
 databags yet.
 
 That is typically the state of a relation when the first unit joins it.
 
 When you use `Relation`, you are specifying a regular (conventional) relation. But that is not the only type of
 relation. There are also peer relations and subordinate relations. While in the background the data model is the same,
 the data access rules and the consistency constraints on them are very different. For example, it does not make sense
 for a peer relation to have a different 'remote app' than its 'local app', because it's the same application.
 
 ### PeerRelation
 
-To declare a peer relation, you should use `scenario.state.PeerRelation`. The core difference with regular relations is
+To declare a peer relation, you should use `scenario.PeerRelation`. The core difference with regular relations is
 that peer relations do not have a "remote app" (it's this app, in fact). So unlike `Relation`, a `PeerRelation` does not
 have `remote_app_name` or `remote_app_data` arguments. Also, it talks in terms of `peers`:
 
 - `Relation.remote_units_data` maps to `PeerRelation.peers_data`
 
 ```python
-from scenario.state import PeerRelation
+import scenario
 
-relation = PeerRelation(
+relation = scenario.PeerRelation(
     endpoint="peers",
     peers_data={1: {}, 2: {}, 42: {'foo': 'bar'}},
 )
 ```
 
 be mindful when using `PeerRelation` not to include **"this unit"**'s ID in `peers_data` or `peers_ids`, as that would
 be flagged by the Consistency Checker:
 
 ```python
-from scenario import State, PeerRelation, Context
+import scenario
 
-state_in = State(relations=[
-    PeerRelation(
+state_in = scenario.State(relations=[
+    scenario.PeerRelation(
         endpoint="peers",
         peers_data={1: {}, 2: {}, 42: {'foo': 'bar'}},
     )])
 
-Context(..., unit_id=1).run("start", state_in)  # invalid: this unit's id cannot be the ID of a peer.
+scenario.Context(..., unit_id=1).run("start", state_in)  # invalid: this unit's id cannot be the ID of a peer.
 
 
 ```
 
 ### SubordinateRelation
 
-To declare a subordinate relation, you should use `scenario.state.SubordinateRelation`. The core difference with regular
+To declare a subordinate relation, you should use `scenario.SubordinateRelation`. The core difference with regular
 relations is that subordinate relations always have exactly one remote unit (there is always exactly one remote unit
 that this unit can see). 
 Because of that, `SubordinateRelation`, compared to `Relation`, always talks in terms of `remote`:
 
 - `Relation.remote_units_data` becomes `SubordinateRelation.remote_unit_data` taking a single `Dict[str:str]`. The remote unit ID can be provided as a separate argument. 
 - `Relation.remote_unit_ids` becomes `SubordinateRelation.remote_unit_id` (a single ID instead of a list of IDs)
 - `Relation.remote_units_data` becomes `SubordinateRelation.remote_unit_data` (a single databag instead of a mapping from unit IDs to databags)
 
 ```python
-from scenario.state import SubordinateRelation
+import scenario
 
-relation = SubordinateRelation(
+relation = scenario.SubordinateRelation(
     endpoint="peers",
     remote_unit_data={"foo": "bar"},
     remote_app_name="zookeeper",
     remote_unit_id=42
 )
 relation.remote_unit_name  # "zookeeper/42"
 ```
 
 ### Triggering Relation Events
 
 If you want to trigger relation events, the easiest way to do so is get a hold of the Relation instance and grab the
 event from one of its aptly-named properties:
 
 ```python
-from scenario import Relation
+import scenario
 
-relation = Relation(endpoint="foo", interface="bar")
+relation = scenario.Relation(endpoint="foo", interface="bar")
 changed_event = relation.changed_event
 joined_event = relation.joined_event
 # ...
 ```
 
 This is in fact syntactic sugar for:
 
 ```python
-from scenario import Relation, Event
+import scenario
 
-relation = Relation(endpoint="foo", interface="bar")
-changed_event = Event('foo-relation-changed', relation=relation)
+relation = scenario.Relation(endpoint="foo", interface="bar")
+changed_event = scenario.Event('foo-relation-changed', relation=relation)
 ```
 
 The reason for this construction is that the event is associated with some relation-specific metadata, that Scenario
 needs to set up the process that will run `ops.main` with the right environment variables.
 
 ### Working with relation IDs
 
-Every time you instantiate `Relation` (or peer, or subordinate), the new instance will be given a unique `relation_id`.
-To inspect the ID the next relation instance will have, you can call `state.next_relation_id`.
+Every time you instantiate `Relation` (or peer, or subordinate), the new instance will be given a unique `id`.
+To inspect the ID the next relation instance will have, you can call `scenario.state.next_relation_id`.
 
 ```python
-from scenario import Relation
-from scenario.state import next_relation_id
+import scenario.state
 
-next_id = next_relation_id(update=False)
-rel = Relation('foo')
-assert rel.relation_id == next_id
+next_id = scenario.state.next_relation_id(update=False)
+rel = scenario.Relation('foo')
+assert rel.id == next_id
 ``` 
 
 This can be handy when using `replace` to create new relations, to avoid relation ID conflicts:
 
 ```python
-from scenario import Relation
-from scenario.state import next_relation_id
+import scenario.state
 
-rel = Relation('foo')
-rel2 = rel.replace(local_app_data={"foo": "bar"}, relation_id=next_relation_id())
-assert rel2.relation_id == rel.relation_id + 1 
+rel = scenario.Relation('foo')
+rel2 = rel.replace(local_app_data={"foo": "bar"}, id=scenario.state.next_relation_id())
+assert rel2.id == rel.id + 1 
 ``` 
 
 If you don't do this, and pass both relations into a `State`, you will trigger a consistency checker error.
 
 ### Additional event parameters
 
 All relation events have some additional metadata that does not belong in the Relation object, such as, for a
@@ -535,230 +505,236 @@
 events, is that the relation already ties 'this app' to some 'remote app' (cfr. the `Relation.remote_app_name` attr),
 but not to a specific unit. What remote unit this event is about is not a `State` concern but an `Event` one.
 
 The `remote_unit_id` will default to the first ID found in the relation's `remote_units_data`, but if the test you are
 writing is close to that domain, you should probably override it and pass it manually.
 
 ```python
-from scenario import Relation, Event
+import scenario
 
-relation = Relation(endpoint="foo", interface="bar")
+relation = scenario.Relation(endpoint="foo", interface="bar")
 remote_unit_2_is_joining_event = relation.joined_event(remote_unit_id=2)
 
 # which is syntactic sugar for:
-remote_unit_2_is_joining_event = Event('foo-relation-changed', relation=relation, relation_remote_unit_id=2)
+remote_unit_2_is_joining_event = scenario.Event('foo-relation-changed', relation=relation, relation_remote_unit_id=2)
 ```
 
-### Networks
+## Networks
 
 Simplifying a bit the Juju "spaces" model, each integration endpoint a charm defines in its metadata is associated with a network. Regardless of whether there is a living relation over that endpoint, that is.  
 
-If your charm has a relation `"foo"` (defined in metadata.yaml), then the charm will be able at runtime to do `self.model.get_binding("foo").network`.
+If your charm has a relation `"foo"` (defined in its metadata), then the charm will be able at runtime to do `self.model.get_binding("foo").network`.
 The network you'll get by doing so is heavily defaulted (see `state.Network.default`) and good for most use-cases because the charm should typically not be concerned about what IP it gets. 
 
-On top of the relation-provided network bindings, a charm can also define some `extra-bindings` in its metadata.yaml and access them at runtime. Note that this is a deprecated feature that should not be relied upon. For completeness, we support it in Scenario.
+On top of the relation-provided network bindings, a charm can also define some `extra-bindings` in its metadata and access them at runtime. Note that this is a deprecated feature that should not be relied upon. For completeness, we support it in Scenario.
 
 If you want to, you can override any of these relation or extra-binding associated networks with a custom one by passing it to `State.networks`.
 
 ```python
-from scenario import State, Network
-state = State(networks={
-  'foo': Network.default(private_address='4.4.4.4')
+import scenario
+
+state = scenario.State(networks={
+  'foo': scenario.Network.default(private_address='192.0.2.1')
 })
 ```
 
 Where `foo` can either be the name of an `extra-bindings`-defined binding, or a relation endpoint.
 
-# Containers
+## Containers
 
-When testing a kubernetes charm, you can mock container interactions. When using the null state (`State()`), there will
+When testing a Kubernetes charm, you can mock container interactions. When using the null state (`State()`), there will
 be no containers. So if the charm were to `self.unit.containers`, it would get back an empty dict.
 
 To give the charm access to some containers, you need to pass them to the input state, like so:
 `State(containers=[...])`
 
 An example of a state including some containers:
 
 ```python
-from scenario.state import Container, State
+import scenario
 
-state = State(containers=[
-    Container(name="foo", can_connect=True),
-    Container(name="bar", can_connect=False)
+state = scenario.State(containers=[
+    scenario.Container(name="foo", can_connect=True),
+    scenario.Container(name="bar", can_connect=False)
 ])
 ```
 
 In this case, `self.unit.get_container('foo').can_connect()` would return `True`, while for 'bar' it would give `False`.
 
 ### Container filesystem setup
+
 You can configure a container to have some files in it:
 
 ```python
-from pathlib import Path
+import pathlib
 
-from scenario.state import Container, State, Mount
+import scenario
 
-local_file = Path('/path/to/local/real/file.txt')
+local_file = pathlib.Path('/path/to/local/real/file.txt')
 
-container = Container(name="foo", can_connect=True, mounts={'local': Mount('/local/share/config.yaml', local_file)})
-state = State(containers=[container])
+container = scenario.Container(
+    name="foo",
+    can_connect=True,
+    mounts={'local': Mount('/local/share/config.yaml', local_file)}
+    )
+state = scenario.State(containers=[container])
 ```
 
 In this case, if the charm were to:
 
 ```python
 def _on_start(self, _):
     foo = self.unit.get_container('foo')
     content = foo.pull('/local/share/config.yaml').read()
 ```
 
-then `content` would be the contents of our locally-supplied `file.txt`. You can use `tempdir` for nicely wrapping
+then `content` would be the contents of our locally-supplied `file.txt`. You can use `tempfile` for nicely wrapping
 data and passing it to the charm via the container.
 
 `container.push` works similarly, so you can write a test like:
 
 ```python
 import tempfile
-from ops.charm import CharmBase
-from scenario import State, Container, Mount, Context
 
+import ops
+import scenario
 
-class MyCharm(CharmBase):
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
+
+class MyCharm(ops.CharmBase):
+    def __init__(self, framework):
+        super().__init__(framework)
+        framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
 
     def _on_pebble_ready(self, _):
         foo = self.unit.get_container('foo')
         foo.push('/local/share/config.yaml', "TEST", make_dirs=True)
 
 
 def test_pebble_push():
     with tempfile.NamedTemporaryFile() as local_file:
-        container = Container(name='foo',
-                              can_connect=True,
-                              mounts={'local': Mount('/local/share/config.yaml', local_file.name)})
-        state_in = State(
-            containers=[container]
+        container = scenario,Container(
+            name='foo',
+            can_connect=True,
+            mounts={'local': Mount('/local/share/config.yaml', local_file.name)}
         )
-        Context(
+        state_in = State(containers=[container])
+        ctx = Context(
             MyCharm,
             meta={"name": "foo", "containers": {"foo": {}}}
-        ).run(
+        )
+        ctx.run(
             container.pebble_ready_event(),
             state_in,
         )
         assert local_file.read().decode() == "TEST"
 ```
 
 `container.pebble_ready_event` is syntactic sugar for: `Event("foo-pebble-ready", container=container)`. The reason we
 need to associate the container with the event is that the Framework uses an envvar to determine which container the
 pebble-ready event is about (it does not use the event name). Scenario needs that information, similarly, for injecting
 that envvar into the charm's runtime.
 
-## Container filesystem post-mortem
+### Container filesystem post-mortem
+
 If the charm writes files to a container (to a location you didn't Mount as a temporary folder you have access to), you will be able to inspect them using the `get_filesystem` api.
 
 ```python
-from ops.charm import CharmBase
-from scenario import State, Container, Mount, Context
+import ops
+import scenario
 
 
-class MyCharm(CharmBase):
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
+class MyCharm(ops.CharmBase):
+    def __init__(self, framework):
+        super().__init__(framework)
+        framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
 
     def _on_pebble_ready(self, _):
         foo = self.unit.get_container('foo')
         foo.push('/local/share/config.yaml', "TEST", make_dirs=True)
 
 
 def test_pebble_push():
-    container = Container(name='foo',
-                          can_connect=True)
-    state_in = State(
-        containers=[container]
-    )
-    ctx = Context(
+    container = scenario.Container(name='foo', can_connect=True)
+    state_in = scenario.State(containers=[container])
+    ctx = scenario.Context(
         MyCharm,
         meta={"name": "foo", "containers": {"foo": {}}}
     )
     
     ctx.run("start", state_in)
 
-    # this is the root of the simulated container filesystem. Any mounts will be symlinks in it.
+    # This is the root of the simulated container filesystem. Any mounts will be symlinks in it.
     container_root_fs = container.get_filesystem(ctx)
     cfg_file = container_root_fs / 'local' / 'share' / 'config.yaml'
     assert cfg_file.read_text() == "TEST"
 ```
 
-## `Container.exec` mocks
+### `Container.exec` mocks
 
 `container.exec` is a tad more complicated, but if you get to this low a level of simulation, you probably will have far
 worse issues to deal with. You need to specify, for each possible command the charm might run on the container, what the
 result of that would be: its return code, what will be written to stdout/stderr.
 
 ```python
-from ops.charm import CharmBase
-
-from scenario import State, Container, ExecOutput, Context
+import ops
+import scenario
 
 LS_LL = """
 .rw-rw-r--  228 ubuntu ubuntu 18 jan 12:05 -- charmcraft.yaml
 .rw-rw-r--  497 ubuntu ubuntu 18 jan 12:05 -- config.yaml
 .rw-rw-r--  900 ubuntu ubuntu 18 jan 12:05 -- CONTRIBUTING.md
 drwxrwxr-x    - ubuntu ubuntu 18 jan 12:06 -- lib
 """
 
 
-class MyCharm(CharmBase):
+class MyCharm(ops.CharmBase):
     def _on_start(self, _):
         foo = self.unit.get_container('foo')
         proc = foo.exec(['ls', '-ll'])
         stdout, _ = proc.wait_output()
         assert stdout == LS_LL
 
 
 def test_pebble_exec():
-    container = Container(
+    container = scenario.Container(
         name='foo',
         exec_mock={
             ('ls', '-ll'):  # this is the command we're mocking
-                ExecOutput(return_code=0,  # this data structure contains all we need to mock the call.
-                           stdout=LS_LL)
+                scenario.ExecOutput(return_code=0,  # this data structure contains all we need to mock the call.
+                                    stdout=LS_LL)
         }
     )
-    state_in = State(
-        containers=[container]
-    )
-    state_out = Context(
+    state_in = scenario.State(containers=[container])
+    ctx = scenario.Context(
         MyCharm,
         meta={"name": "foo", "containers": {"foo": {}}},
-    ).run(
+    )
+    state_out = ctx.run(
         container.pebble_ready_event,
         state_in,
     )
 ```
 
-# Storage
+## Storage
 
-If your charm defines `storage` in its metadata, you can use `scenario.state.Storage` to instruct Scenario to make (mocked) filesystem storage available to the charm at runtime.
+If your charm defines `storage` in its metadata, you can use `scenario.Storage` to instruct Scenario to make (mocked) filesystem storage available to the charm at runtime.
 
-Using the same `get_filesystem` API as `Container`, you can access the tempdir used by Scenario to mock the filesystem root before and after the scenario runs.
+Using the same `get_filesystem` API as `Container`, you can access the temporary directory used by Scenario to mock the filesystem root before and after the scenario runs.
 
 ```python
-from scenario import Storage, Context, State
-# some charm with a 'foo' filesystem-type storage defined in metadata.yaml 
-ctx = Context(MyCharm)
-storage = Storage("foo")
-# setup storage with some content
+import scenario
+
+# Some charm with a 'foo' filesystem-type storage defined in its metadata:
+ctx = scenario.Context(MyCharm)
+storage = scenario.Storage("foo")
+
+# Setup storage with some content:
 (storage.get_filesystem(ctx) / "myfile.txt").write_text("helloworld")
 
-with ctx.manager("update-status", State(storage=[storage])) as mgr:
+with ctx.manager("update-status", scenario.State(storage=[storage])) as mgr:
     foo = mgr.charm.model.storages["foo"][0]
     loc = foo.location
     path = loc / "myfile.txt"
     assert path.exists()
     assert path.read_text() == "helloworld"
 
     myfile = loc / "path.py"
@@ -768,87 +744,85 @@
 assert (
     storage.get_filesystem(ctx) / "path.py"
 ).read_text() == "helloworlds"
 ```
 
 Note that State only wants to know about **attached** storages. A storage which is not attached to the charm can simply be omitted from State and the charm will be none the wiser.
 
-## Storage-add
+### Storage-add
 
 If a charm requests adding more storage instances while handling some event, you can inspect that from the `Context.requested_storage` API.
 
 ```python
-# in MyCharm._on_foo:
-# the charm requests two new "foo" storage instances to be provisioned 
+# In MyCharm._on_foo:
+# The charm requests two new "foo" storage instances to be provisioned:
 self.model.storages.request("foo", 2)
 ```
 
 From test code, you can inspect that:
 
 ```python
-from scenario import Context, State
+import scenario
 
-ctx = Context(MyCharm)
-ctx.run('some-event-that-will-cause_on_foo-to-be-called', State())
+ctx = scenario.Context(MyCharm)
+ctx.run('some-event-that-will-cause_on_foo-to-be-called', scenario.State())
 
-# the charm has requested two 'foo' storages to be provisioned
+# the charm has requested two 'foo' storages to be provisioned:
 assert ctx.requested_storages['foo'] == 2
 ```
 
 Requesting storages has no other consequence in Scenario. In real life, this request will trigger Juju to provision the storage and execute the charm again with `foo-storage-attached`.
 So a natural follow-up Scenario test suite for this case would be:
 
 ```python
-from scenario import Context, State, Storage
+import scenario
 
-ctx = Context(MyCharm)
-foo_0 = Storage('foo')
-# the charm is notified that one of the storages it has requested is ready
+ctx = scenario.Context(MyCharm)
+foo_0 = scenario.Storage('foo')
+# The charm is notified that one of the storages it has requested is ready:
 ctx.run(foo_0.attached_event, State(storage=[foo_0]))
 
-foo_1 = Storage('foo')
-# the charm is notified that the other storage is also ready
+foo_1 = scenario.Storage('foo')
+# The charm is notified that the other storage is also ready:
 ctx.run(foo_1.attached_event, State(storage=[foo_0, foo_1]))
 ```
 
+## Ports
 
-# Ports
-
-Since `ops 2.6.0`, charms can invoke the `open-port`, `close-port`, and `opened-ports` hook tools to manage the ports opened on the host vm/container. Using the `State.opened_ports` api, you can: 
+Since `ops 2.6.0`, charms can invoke the `open-port`, `close-port`, and `opened-ports` hook tools to manage the ports opened on the host VM/container. Using the `State.opened_ports` API, you can: 
 
 - simulate a charm run with a port opened by some previous execution
 ```python
-from scenario import State, Port, Context
+import scenario
 
-ctx = Context(MyCharm)
-ctx.run("start", State(opened_ports=[Port("tcp", 42)]))
+ctx = scenario.Context(MyCharm)
+ctx.run("start", scenario.State(opened_ports=[scenario.Port("tcp", 42)]))
 ```
 - assert that a charm has called `open-port` or `close-port`:
 ```python
-from scenario import State, Port, Context
+import scenario
 
-ctx = Context(MyCharm)
-state1 = ctx.run("start", State())
-assert state1.opened_ports == [Port("tcp", 42)]
+ctx = scenario.Context(MyCharm)
+state1 = ctx.run("start", scenario.State())
+assert state1.opened_ports == [scenario.Port("tcp", 42)]
 
 state2 = ctx.run("stop", state1)
 assert state2.opened_ports == []
 ```
 
-
-# Secrets
+## Secrets
 
 Scenario has secrets. Here's how you use them.
 
 ```python
-from scenario import State, Secret
+import scenario
 
-state = State(
+state = scenario.State(
     secrets=[
-        Secret(
+        scenario.Secret(
             id='foo',
             contents={0: {'key': 'public'}}
         )
     ]
 )
 ```
 
@@ -858,327 +832,381 @@
 There are three cases:
 - the secret is owned by this app but not this unit, in which case this charm can only manage it if we are the leader
 - the secret is owned by this unit, in which case this charm can always manage it (leader or not)
 - (default) the secret is not owned by this app nor unit, which means we can't manage it but only view it
 
 Thus by default, the secret is not owned by **this charm**, but, implicitly, by some unknown 'other charm', and that other charm has granted us view rights.
 
-
 The presence of the secret in `State.secrets` entails that we have access to it, either as owners or as grantees. Therefore, if we're not owners, we must be grantees. Absence of a Secret from the known secrets list means we are not entitled to obtaining it in any way. The charm, indeed, shouldn't even know it exists.
 
 [note]
 If this charm does not own the secret, but also it was not granted view rights by the (remote) owner, you model this in Scenario by _not adding it to State.secrets_! The presence of a `Secret` in `State.secrets` means, in other words, that the charm has view rights (otherwise, why would we put it there?). If the charm owns the secret, or is leader, it will _also_ have manage rights on top of view ones.
 [/note]
 
 To specify a secret owned by this unit (or app):
 
 ```python
-from scenario import State, Secret
+import scenario
 
-state = State(
+state = scenario.State(
     secrets=[
-        Secret(
+        scenario.Secret(
             id='foo',
             contents={0: {'key': 'private'}},
             owner='unit',  # or 'app'
             remote_grants={0: {"remote"}}
             # the secret owner has granted access to the "remote" app over some relation with ID 0
         )
     ]
 )
 ```
 
 To specify a secret owned by some other application and give this unit (or app) access to it:
 
 ```python
-from scenario import State, Secret
+import scenario
 
-state = State(
+state = scenario.State(
     secrets=[
-        Secret(
+        scenario.Secret(
             id='foo',
             contents={0: {'key': 'public'}},
             # owner=None, which is the default
             revision=0,  # the revision that this unit (or app) is currently tracking
         )
     ]
 )
 ```
 
+## StoredState
+
+Scenario can simulate StoredState. You can define it on the input side as:
+
+```python
+import ops
+import scenario
+
+from ops.charm import CharmBase
+
+
+class MyCharmType(ops.CharmBase):
+    my_stored_state = ops.StoredState()
+
+    def __init__(self, framework):
+        super().__init__(framework)
+        assert self.my_stored_state.foo == 'bar'  # this will pass!
+
+
+state = scenario.State(stored_state=[
+    scenario.StoredState(
+        owner_path="MyCharmType",
+        name="my_stored_state",
+        content={
+            'foo': 'bar',
+            'baz': {42: 42},
+        })
+])
+```
+
+And the charm's runtime will see `self.my_stored_state.foo` and `.baz` as expected. Also, you can run assertions on it on
+the output side the same as any other bit of state.
+
+## Resources
+
+If your charm requires access to resources, you can make them available to it through `State.resources`.
+From the perspective of a 'real' deployed charm, if your charm _has_ resources defined in its metadata, they _must_ be made available to the charm. That is a Juju-enforced constraint: you can't deploy a charm without attaching all resources it needs to it.
+However, when testing, this constraint is unnecessarily strict (and it would also mean the great majority of all existing tests would break) since a charm will only notice that a resource is not available when it explicitly asks for it, which not many charms do.
+
+So, the only consistency-level check we enforce in Scenario when it comes to resource is that if a resource is provided in State, it needs to have been declared in the metadata.
+
+```python
+import scenario
+
+ctx = scenario.Context(MyCharm, meta={'name': 'juliette', "resources": {"foo": {"type": "oci-image"}}})
+with ctx.manager("start", scenario.State(resources={'foo': '/path/to/resource.tar'})) as mgr:
+    # If the charm, at runtime, were to call self.model.resources.fetch("foo"), it would get '/path/to/resource.tar' back.
+    path = mgr.charm.model.resources.fetch('foo')
+    assert path == '/path/to/resource.tar'
+```
+
+## Model
+
+Charms don't usually need to be aware of the model in which they are deployed,
+but if you need to set the model name or UUID, you can provide a `scenario.Model`
+to the state:
+
+```python
+import ops
+import scenario
+
+class MyCharm(ops.CharmBase):
+    pass
+
+ctx = scenario.Context(MyCharm, meta={"name": "foo"})
+state_in = scenario.State(model=scenario.Model(name="my-model"))
+out = ctx.run("start", state_in)
+assert out.model.name == "my-model"
+assert out.model.uuid == state_in.model.uuid
+```
+
+## CloudSpec
+
+You can set CloudSpec information in the state (only `type` and `name` are required).
+
+Example:
+
+```python
+import scenario
+
+state = scenario.State(
+    cloud_spec=scenario.CloudSpec(
+        type="lxd",
+        name="localhost",
+        endpoint="https://127.0.0.1:8443",
+        credential=scenario.CloudCredential(
+            auth_type="clientcertificate",
+            attributes={
+                "client-cert": "foo",
+                "client-key": "bar",
+                "server-cert": "baz",
+            },
+        ),
+    ),
+    model=scenario.Model(name="my-vm-model", type="lxd"),
+)
+```
+
+Then you can access it by `Model.get_cloud_spec()`:
+
+```python
+# charm.py
+class MyVMCharm(ops.CharmBase):
+    def __init__(self, framework: ops.Framework):
+        super().__init__(framework)
+        framework.observe(self.on.start, self._on_start)
+
+    def _on_start(self, event: ops.StartEvent):
+        self.cloud_spec = self.model.get_cloud_spec()
+```
+
 # Actions
 
 An action is a special sort of event, even though `ops` handles them almost identically.
 In most cases, you'll want to inspect the 'results' of an action, or whether it has failed or
 logged something while executing. Many actions don't have a direct effect on the output state.
 For this reason, the output state is less prominent in the return type of `Context.run_action`.
 
 How to test actions with scenario:
 
 ## Actions without parameters
 
 ```python
-from scenario import Context, State, ActionOutput
+import scenario
+
 from charm import MyCharm
 
 
 def test_backup_action():
-    ctx = Context(MyCharm)
+    ctx = scenario.Context(MyCharm)
 
-    # If you didn't declare do_backup in the charm's `actions.yaml`, 
+    # If you didn't declare do_backup in the charm's metadata, 
     # the `ConsistencyChecker` will slap you on the wrist and refuse to proceed.
-    out: ActionOutput = ctx.run_action("do_backup_action", State())
+    out: scenario.ActionOutput = ctx.run_action("do_backup_action", scenario.State())
 
-    # you can assert action results, logs, failure using the ActionOutput interface
+    # You can assert action results, logs, failure using the ActionOutput interface:
     assert out.logs == ['baz', 'qux']
     
     if out.success:
-      # if the action did not fail, we can read the results:
+      # If the action did not fail, we can read the results:
       assert out.results == {'foo': 'bar'}
 
     else:
-      # if the action fails, we can read a failure message
+      # If the action fails, we can read a failure message:
       assert out.failure == 'boo-hoo'
 ```
 
 ## Parametrized Actions
 
 If the action takes parameters, you'll need to instantiate an `Action`.
 
 ```python
-from scenario import Action, Context, State, ActionOutput
+import scenario
+
 from charm import MyCharm
 
 
 def test_backup_action():
-    # define an action
-    action = Action('do_backup', params={'a': 'b'})
-    ctx = Context(MyCharm)
-
-    # if the parameters (or their type) don't match what declared in actions.yaml, 
-    # the `ConsistencyChecker` will slap you on the other wrist. 
-    out: ActionOutput = ctx.run_action(action, State())
+    # Define an action:
+    action = scenario.Action('do_backup', params={'a': 'b'})
+    ctx = scenario.Context(MyCharm)
+
+    # If the parameters (or their type) don't match what is declared in the metadata, 
+    # the `ConsistencyChecker` will slap you on the other wrist.
+    out: scenario.ActionOutput = ctx.run_action(action, scenario.State())
 
     # ...
 ```
 
 # Deferred events
 
 Scenario allows you to accurately simulate the Operator Framework's event queue. The event queue is responsible for
 keeping track of the deferred events. On the input side, you can verify that if the charm triggers with this and that
 event in its queue (they would be there because they had been deferred in the previous run), then the output state is
 valid.
 
 ```python
-from scenario import State, deferred, Context
+import scenario
 
 
 class MyCharm(...):
     ...
 
-    def _on_update_status(self, e):
-        e.defer()
+    def _on_update_status(self, event):
+        event.defer()
 
-    def _on_start(self, e):
-        e.defer()
+    def _on_start(self, event):
+        event.defer()
 
 
 def test_start_on_deferred_update_status(MyCharm):
     """Test charm execution if a 'start' is dispatched when in the previous run an update-status had been deferred."""
-    state_in = State(
+    state_in = scenario.State(
         deferred=[
-            deferred('update_status',
-                     handler=MyCharm._on_update_status)
+            scenario.deferred('update_status', handler=MyCharm._on_update_status)
         ]
     )
-    state_out = Context(MyCharm).run('start', state_in)
+    state_out = scenario.Context(MyCharm).run('start', state_in)
     assert len(state_out.deferred) == 1
     assert state_out.deferred[0].name == 'start'
 ```
 
 You can also generate the 'deferred' data structure (called a DeferredEvent) from the corresponding Event (and the
 handler):
 
 ```python
-from scenario import Event, Relation
+import scenario
 
 
 class MyCharm(...):
     ...
 
 
-deferred_start = Event('start').deferred(MyCharm._on_start)
-deferred_install = Event('install').deferred(MyCharm._on_start)
-```
-
-## relation events:
-
-```python
-foo_relation = Relation('foo')
-deferred_relation_changed_evt = foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
+deferred_start = scenario.Event('start').deferred(MyCharm._on_start)
+deferred_install = scenario.Event('install').deferred(MyCharm._on_start)
 ```
 
 On the output side, you can verify that an event that you expect to have been deferred during this trigger, has indeed
 been deferred.
 
 ```python
-from scenario import State, Context
+import scenario
 
 
 class MyCharm(...):
     ...
 
-    def _on_start(self, e):
-        e.defer()
+    def _on_start(self, event):
+        event.defer()
 
 
 def test_defer(MyCharm):
-    out = Context(MyCharm).run('start', State())
+    out = scenario.Context(MyCharm).run('start', scenario.State())
     assert len(out.deferred) == 1
     assert out.deferred[0].name == 'start'
 ```
 
 ## Deferring relation events
 
 If you want to test relation event deferrals, some extra care needs to be taken. RelationEvents hold references to the
 Relation instance they are about. So do they in Scenario. You can use the deferred helper to generate the data
 structure:
 
 ```python
-from scenario import State, Relation, deferred
+import scenario
 
 
 class MyCharm(...):
     ...
 
-    def _on_foo_relation_changed(self, e):
-        e.defer()
+    def _on_foo_relation_changed(self, event):
+        event.defer()
 
 
 def test_start_on_deferred_update_status(MyCharm):
-    foo_relation = Relation('foo')
-    State(
+    foo_relation = scenario.Relation('foo')
+    scenario.State(
         relations=[foo_relation],
         deferred=[
-            deferred('foo_relation_changed',
-                     handler=MyCharm._on_foo_relation_changed,
-                     relation=foo_relation)
+            scenario.deferred('foo_relation_changed',
+                              handler=MyCharm._on_foo_relation_changed,
+                              relation=foo_relation)
         ]
     )
 ```
 
-but you can also use a shortcut from the relation event itself, as mentioned above:
+but you can also use a shortcut from the relation event itself:
 
 ```python
-
-from scenario import Relation
+import scenario
 
 
 class MyCharm(...):
     ...
 
 
-foo_relation = Relation('foo')
+foo_relation = scenario.Relation('foo')
 foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
 ```
 
-### Fine-tuning
+## Fine-tuning
 
 The deferred helper Scenario provides will not support out of the box all custom event subclasses, or events emitted by
 charm libraries or objects other than the main charm class.
 
 For general-purpose usage, you will need to instantiate DeferredEvent directly.
 
 ```python
-from scenario import DeferredEvent
+import scenario
 
-my_deferred_event = DeferredEvent(
+my_deferred_event = scenario.DeferredEvent(
     handle_path='MyCharm/MyCharmLib/on/database_ready[1]',
     owner='MyCharmLib',  # the object observing the event. Could also be MyCharm.
     observer='_on_database_ready'
 )
 ```
 
-# StoredState
-
-Scenario can simulate StoredState. You can define it on the input side as:
-
-```python
-from ops.charm import CharmBase
-from ops.framework import StoredState as Ops_StoredState, Framework
-from scenario import State, StoredState
-
-
-class MyCharmType(CharmBase):
-    my_stored_state = Ops_StoredState()
-
-    def __init__(self, framework: Framework):
-        super().__init__(framework)
-        assert self.my_stored_state.foo == 'bar'  # this will pass!
-
-
-state = State(stored_state=[
-    StoredState(
-        owner_path="MyCharmType",
-        name="my_stored_state",
-        content={
-            'foo': 'bar',
-            'baz': {42: 42},
-        })
-])
-```
-
-And the charm's runtime will see `self.stored_State.foo` and `.baz` as expected. Also, you can run assertions on it on
-the output side the same as any other bit of state.
-
-# Resources
-
-If your charm requires access to resources, you can make them available to it through `State.resources`.
-From the perspective of a 'real' deployed charm, if your charm _has_ resources defined in `metadata.yaml`, they _must_ be made available to the charm. That is a Juju-enforced constraint: you can't deploy a charm without attaching all resources it needs to it.
-However, when testing, this constraint is unnecessarily strict (and it would also mean the great majority of all existing tests would break) since a charm will only notice that a resource is not available when it explicitly asks for it, which not many charms do.
-
-So, the only consistency-level check we enforce in Scenario when it comes to resource is that if a resource is provided in State, it needs to have been declared in metadata.
-
-```python
-from scenario import State, Context
-ctx = Context(MyCharm, meta={'name': 'juliette', "resources": {"foo": {"type": "oci-image"}}})
-with ctx.manager("start", State(resources={'foo': '/path/to/resource.tar'})) as mgr:
-    # if the charm, at runtime, were to call self.model.resources.fetch("foo"), it would get '/path/to/resource.tar' back.
-    path = mgr.charm.model.resources.fetch('foo')
-    assert path == '/path/to/resource.tar' 
-```
-
 # Emitting custom events
 
-While the main use case of Scenario is to emit juju events, i.e. the built-in `start`, `install`, `*-relation-changed`,
+While the main use case of Scenario is to emit Juju events, i.e. the built-in `start`, `install`, `*-relation-changed`,
 etc..., it can be sometimes handy to directly trigger custom events defined on arbitrary Objects in your hierarchy.
 
 Suppose your charm uses a charm library providing an `ingress_provided` event.
 The 'proper' way to emit it is to run the event that causes that custom event to be emitted by the library, whatever
 that may be, for example a `foo-relation-changed`.
 
 However, that may mean that you have to set up all sorts of State and mocks so that the right preconditions are met and
 the event is emitted at all.
 
 If for whatever reason you don't want to do that and you attempt to run that event directly you will get an error:
 
 ```python
-from scenario import Context, State
+import scenario
 
-Context(...).run("ingress_provided", State())  # raises scenario.ops_main_mock.NoObserverError
+scenario.Context(...).run("ingress_provided", scenario.State())  # raises scenario.ops_main_mock.NoObserverError
 ```
 
 This happens because the framework, by default, searches for an event source named `ingress_provided` in `charm.on`, but
 since the event is defined on another Object, it will fail to find it.
 
 You can prefix the event name with the path leading to its owner to tell Scenario where to find the event source:
 
 ```python
-from scenario import Context, State
+import scenario
 
-Context(...).run("my_charm_lib.on.foo", State())
+scenario.Context(...).run("my_charm_lib.on.foo", scenario.State())
 ```
 
 This will instruct Scenario to emit `my_charm.my_charm_lib.on.foo`.
 
 (always omit the 'root', i.e. the charm framework key, from the path)
 
 # Live charm introspection
@@ -1186,158 +1214,155 @@
 Scenario is a black-box, state-transition testing framework. It makes it trivial to assert that a status went from A to
 B, but not to assert that, in the context of this charm execution, with this state, a certain charm-internal method was called and returned a
 given piece of data, or would return this and that _if_ it had been called.
 
 Scenario offers a cheekily-named context manager for this use case specifically:
 
 ```python
-from ops import CharmBase, StoredState
+import ops
+import scenario
 
 from charms.bar.lib_name.v1.charm_lib import CharmLib
-from scenario import Context, State
 
 
-class MyCharm(CharmBase):
+class MyCharm(ops.CharmBase):
     META = {"name": "mycharm"}
-    _stored = StoredState()
+    _stored = ops.StoredState()
     
     def __init__(self, framework):
         super().__init__(framework)
         self._stored.set_default(a="a")
         self.my_charm_lib = CharmLib()
         framework.observe(self.on.start, self._on_start)
 
     def _on_start(self, event):
         self._stored.a = "b"
 
 
 def test_live_charm_introspection(mycharm):
-    ctx = Context(mycharm, meta=mycharm.META)
+    ctx = scenario.Context(mycharm, meta=mycharm.META)
     # If you want to do this with actions, you can use `Context.action_manager` instead.
-    with ctx.manager("start", State()) as manager:
-        # this is your charm instance, after ops has set it up
+    with ctx.manager("start", scenario.State()) as manager:
+        # This is your charm instance, after ops has set it up:
         charm: MyCharm = manager.charm
         
-        # we can check attributes on nested Objects or the charm itself 
+        # We can check attributes on nested Objects or the charm itself:
         assert charm.my_charm_lib.foo == "foo"
-        # such as stored state
+        # such as stored state:
         assert charm._stored.a == "a"
 
-        # this will tell ops.main to proceed with normal execution and emit the "start" event on the charm
+        # This will tell ops.main to proceed with normal execution and emit the "start" event on the charm:
         state_out = manager.run()
     
-        # after that is done, we are handed back control, and we can again do some introspection
+        # After that is done, we are handed back control, and we can again do some introspection:
         assert charm.my_charm_lib.foo == "bar"
-        # and check that the charm's internal state is as we expect
+        # and check that the charm's internal state is as we expect:
         assert charm._stored.a == "b"
 
     # state_out is, as in regular scenario tests, a State object you can assert on:
     assert state_out.unit_status == ...
 ```
 
 Note that you can't call `manager.run()` multiple times: the manager is a context that ensures that `ops.main` 'pauses' right
 before emitting the event to hand you some introspection hooks, but for the rest this is a regular scenario test: you
 can't emit multiple events in a single charm execution.
 
 # The virtual charm root
 
 Before executing the charm, Scenario copies the charm's `/src`, any libs, the metadata, config, and actions `yaml`s to a temporary directory. The
-charm will see that tempdir as its 'root'. This allows us to keep things simple when dealing with metadata that can be
+charm will see that temporary directory as its 'root'. This allows us to keep things simple when dealing with metadata that can be
 either inferred from the charm type being passed to `Context` or be passed to it as an argument, thereby overriding
 the inferred one. This also allows you to test charms defined on the fly, as in:
 
 ```python
-from ops.charm import CharmBase
-from scenario import State, Context
+import ops
+import scenario
 
 
-class MyCharmType(CharmBase):
+class MyCharmType(ops.CharmBase):
     pass
 
 
-ctx = Context(charm_type=MyCharmType,
-              meta={'name': 'my-charm-name'})
+ctx = scenario.Context(charm_type=MyCharmType, meta={'name': 'my-charm-name'})
 ctx.run('start', State())
 ```
 
-A consequence of this fact is that you have no direct control over the tempdir that we are creating to put the metadata
+A consequence of this fact is that you have no direct control over the temporary directory that we are creating to put the metadata
 you are passing to `.run()` (because `ops` expects it to be a file...). That is, unless you pass your own:
 
 ```python
-from ops.charm import CharmBase
-from scenario import State, Context
 import tempfile
 
+import ops
+import scenario
+
 
-class MyCharmType(CharmBase):
+class MyCharmType(ops.CharmBase):
     pass
 
 
 td = tempfile.TemporaryDirectory()
-state = Context(
+state = scenario.Context(
     charm_type=MyCharmType,
     meta={'name': 'my-charm-name'},
     charm_root=td.name
-).run('start', State())
+).run('start', scenario.State())
 ```
 
 Do this, and you will be able to set up said directory as you like before the charm is run, as well as verify its
 contents after the charm has run. Do keep in mind that any metadata files you create in it will be overwritten by Scenario, and therefore
 ignored, if you pass any metadata keys to `Context`. Omit `meta` in the call
-above, and Scenario will instead attempt to read `metadata.yaml` from the
+above, and Scenario will instead attempt to read metadata from the
 temporary directory.
 
-
 # Immutability
 
-All of the data structures in `state`, e.g. `State, Relation, Container`, etc... are immutable (implemented as frozen
-dataclasses).
+All of the data structures in `state`, e.g. `State, Relation, Container`, etc... are implemented as frozen dataclasses.
 
 This means that all components of the state that goes into a `context.run()` call are not mutated by the call, and the
 state that you obtain in return is a different instance, and all parts of it have been (deep)copied.
-This ensures that you can do delta-based comparison of states without worrying about them being mutated by scenario.
+This ensures that you can do delta-based comparison of states without worrying about them being mutated by Scenario.
 
 If you want to modify any of these data structures, you will need to either reinstantiate it from scratch, or use
 the `replace` api.
 
 ```python
-from scenario import Relation
+import scenario
 
-relation = Relation('foo', remote_app_data={"1": "2"})
+relation = scenario.Relation('foo', remote_app_data={"1": "2"})
 # make a copy of relation, but with remote_app_data set to {"3", "4"} 
 relation2 = relation.replace(remote_app_data={"3", "4"})
 ```
 
 # Consistency checks
 
 A Scenario, that is, the combination of an event, a state, and a charm, is consistent if it's plausible in JujuLand. For
 example, Juju can't emit a `foo-relation-changed` event on your charm unless your charm has declared a `foo` relation
-endpoint in its `metadata.yaml`. If that happens, that's a juju bug. Scenario however assumes that Juju is bug-free,
+endpoint in its metadata. If that happens, that's a Juju bug. Scenario however assumes that Juju is bug-free,
 therefore, so far as we're concerned, that can't happen, and therefore we help you verify that the scenarios you create
 are consistent and raise an exception if that isn't so.
 
 That happens automatically behind the scenes whenever you trigger an event;
 `scenario.consistency_checker.check_consistency` is called and verifies that the scenario makes sense.
 
 ## Caveats:
 
 - False positives: not all checks are implemented yet; more will come.
 - False negatives: it is possible that a scenario you know to be consistent is seen as inconsistent. That is probably a
-  bug in the consistency checker itself, please report it.
+  bug in the consistency checker itself; please report it.
 - Inherent limitations: if you have a custom event whose name conflicts with a builtin one, the consistency constraints
   of the builtin one will apply. For example: if you decide to name your custom event `bar-pebble-ready`, but you are
   working on a machine charm or don't have either way a `bar` container in your `metadata.yaml`, Scenario will flag that
   as inconsistent.
 
 ## Bypassing the checker
 
 If you have a clear false negative, are explicitly testing 'edge', inconsistent situations, or for whatever reason the
 checker is in your way, you can set the `SCENARIO_SKIP_CONSISTENCY_CHECKS` envvar and skip it altogether. Hopefully you
 don't need that.
 
 # Jhack integrations
 
-Up until `v5.6.0`, `scenario` shipped with a cli tool called `snapshot`, used to interact with a live charm's state.
+Up until `v5.6.0`, Scenario shipped with a cli tool called `snapshot`, used to interact with a live charm's state.
 The functionality [has been moved over to `jhack`](https://github.com/PietroPasotti/jhack/pull/111), 
 to allow us to keep working on it independently, and to streamline 
-the profile of `scenario` itself as it becomes more broadly adopted and ready for widespread usage.
-
+the profile of Scenario itself as it becomes more broadly adopted and ready for widespread usage.
```

### Comparing `ops-scenario-6.0.3/ops_scenario.egg-info/SOURCES.txt` & `ops_scenario-6.0.4/ops_scenario.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 tests/test_dcbase.py
 tests/test_emitted_events_util.py
 tests/test_hypothesis.py
 tests/test_plugin.py
 tests/test_runtime.py
 tests/test_e2e/test_actions.py
 tests/test_e2e/test_builtin_scenes.py
+tests/test_e2e/test_cloud_spec.py
 tests/test_e2e/test_config.py
 tests/test_e2e/test_custom_event_triggers.py
 tests/test_e2e/test_deferred.py
 tests/test_e2e/test_event.py
 tests/test_e2e/test_event_bind.py
 tests/test_e2e/test_juju_log.py
 tests/test_e2e/test_manager.py
```

### Comparing `ops-scenario-6.0.3/pyproject.toml` & `ops_scenario-6.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools_scm >= 2.0.0, <3"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ops-scenario"
 
-version = "6.0.3"
+version = "6.0.4"
 
 authors = [
     { name = "Pietro Pasotti", email = "pietro.pasotti@canonical.com" }
 ]
 description = "Python library providing a state-transition testing API for Operator Framework charms."
 license.text = "Apache-2.0"
 keywords = ["juju", "test"]
```

### Comparing `ops-scenario-6.0.3/resources/state-transition-model.png` & `ops_scenario-6.0.4/resources/state-transition-model.png`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/scenario/capture_events.py` & `ops_scenario-6.0.4/scenario/capture_events.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/scenario/consistency_checker.py` & `ops_scenario-6.0.4/scenario/consistency_checker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 # Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 import os
+import re
 from collections import Counter
 from collections.abc import Sequence
 from numbers import Number
-from typing import TYPE_CHECKING, Iterable, List, NamedTuple, Tuple
+from typing import TYPE_CHECKING, Iterable, List, NamedTuple, Tuple, Union
 
 from scenario.runtime import InconsistentScenarioError
 from scenario.runtime import logger as scenario_logger
 from scenario.state import (
     Action,
     PeerRelation,
     SubordinateRelation,
@@ -65,14 +66,15 @@
         check_config_consistency,
         check_resource_consistency,
         check_event_consistency,
         check_secrets_consistency,
         check_storages_consistency,
         check_relation_consistency,
         check_network_consistency,
+        check_cloudspec_consistency,
     ):
         results = check(
             state=state,
             event=event,
             charm_spec=charm_spec,
             juju_version=juju_version_,
         )
@@ -322,18 +324,25 @@
                 f"occurs multiple times in State.storage.",
             )
         seen.append(tag)
 
     return Results(errors, [])
 
 
+def _is_secret_identifier(value: Union[str, int, float, bool]) -> bool:
+    """Return true iff the value is in the form `secret:{secret id}`."""
+    # cf. https://github.com/juju/juju/blob/13eb9df3df16a84fd471af8a3c95ddbd04389b71/core/secrets/secret.go#L48
+    return bool(re.match(r"secret:[0-9a-z]{20}$", str(value)))
+
+
 def check_config_consistency(
     *,
     state: "State",
     charm_spec: "_CharmSpec",
+    juju_version: Tuple[int, ...],
     **_kwargs,  # noqa: U101
 ) -> Results:
     """Check the consistency of the state.config with the charm_spec.config (config.yaml)."""
     state_config = state.config
     meta_config = (charm_spec.config or {}).get("options", {})
     errors = []
 
@@ -344,37 +353,47 @@
             )
             continue
 
         # todo unify with snapshot's when merged.
         converters = {
             "string": str,
             "int": int,
-            "integer": int,  # fixme: which one is it?
-            "number": float,
+            "float": float,
             "boolean": bool,
-            # "attrs": NotImplemented,  # fixme: wot?
+        }
+        if juju_version >= (3, 4):
+            converters["secret"] = str
+
+        validators = {
+            "secret": _is_secret_identifier,
         }
 
         expected_type_name = meta_config[key].get("type", None)
         if not expected_type_name:
             errors.append(f"config.yaml invalid; option {key!r} has no 'type'.")
             continue
+        validator = validators.get(expected_type_name)
 
         expected_type = converters.get(expected_type_name)
         if not expected_type:
             errors.append(
                 f"config invalid for option {key!r}: 'type' {expected_type_name} unknown",
             )
 
         elif not isinstance(value, expected_type):
             errors.append(
                 f"config invalid; option {key!r} should be of type {expected_type} "
                 f"but is of type {type(value)}.",
             )
 
+        elif validator and not validator(value):
+            errors.append(
+                f"config invalid: option {key!r} value {value!r} is not valid.",
+            )
+
     return Results(errors, [])
 
 
 def check_secrets_consistency(
     *,
     event: "Event",
     state: "State",
@@ -464,21 +483,21 @@
             errors.append(f"relation endpoint {ep} is not declared in metadata.")
 
     seen_ids = set()
     for endpoint, relation_meta in all_relations_meta:
         expected_sub = relation_meta.get("scope", "") == "container"
         relations = _get_relations(endpoint)
         for relation in relations:
-            if relation.relation_id in seen_ids:
+            if relation.id in seen_ids:
                 errors.append(
-                    f"duplicate relation ID: {relation.relation_id} is claimed "
+                    f"duplicate relation ID: {relation.id} is claimed "
                     f"by multiple Relation instances",
                 )
 
-            seen_ids.add(relation.relation_id)
+            seen_ids.add(relation.id)
             is_sub = isinstance(relation, SubordinateRelation)
             if is_sub and not expected_sub:
                 errors.append(
                     f"endpoint {endpoint} is not a subordinate relation; "
                     f"expecting relation to be of type Relation, "
                     f"got {type(relation)}",
                 )
@@ -543,7 +562,27 @@
 
     # guard against duplicate container names
     names = Counter(state_containers)
     if dupes := [n for n in names if names[n] > 1]:
         errors.append(f"Duplicate container name(s): {dupes}.")
 
     return Results(errors, [])
+
+
+def check_cloudspec_consistency(
+    *,
+    state: "State",
+    event: "Event",
+    charm_spec: "_CharmSpec",
+    **_kwargs,  # noqa: U101
+) -> Results:
+    """Check that Kubernetes charms/models don't have `state.cloud_spec`."""
+
+    errors = []
+    warnings = []
+
+    if state.model.type == "kubernetes" and state.cloud_spec:
+        errors.append(
+            "CloudSpec is only available for machine charms, not Kubernetes charms. Tell Scenario to simulate a machine substrate with: `scenario.State(..., model=scenario.Model(type='lxd'))`.",
+        )
+
+    return Results(errors, warnings)
```

### Comparing `ops-scenario-6.0.3/scenario/context.py` & `ops_scenario-6.0.4/scenario/context.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/scenario/mocking.py` & `ops_scenario-6.0.4/scenario/mocking.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Optional,
     Set,
     Tuple,
     Union,
     cast,
 )
 
-from ops import JujuVersion, pebble
+from ops import CloudSpec, JujuVersion, pebble
 from ops.model import ModelError, RelationNotFoundError
 from ops.model import Secret as Secret_Ops  # lol
 from ops.model import (
     SecretInfo,
     SecretNotFoundError,
     SecretRotate,
     _format_action_result_dict,
@@ -159,15 +159,15 @@
 
     def _get_relation_by_id(
         self,
         rel_id,
     ) -> Union["Relation", "SubordinateRelation", "PeerRelation"]:
         try:
             return next(
-                filter(lambda r: r.relation_id == rel_id, self._state.relations),
+                filter(lambda r: r.id == rel_id, self._state.relations),
             )
         except StopIteration:
             raise RelationNotFoundError()
 
     def _get_secret(self, id=None, label=None):
         # FIXME: what error would a charm get IRL?
         # ops 2.0 supports secrets, but juju only supports it from 3.0.2
@@ -241,17 +241,15 @@
 
     def status_get(self, *, is_app: bool = False):
         status = self._state.app_status if is_app else self._state.unit_status
         return {"status": status.name, "message": status.message}
 
     def relation_ids(self, relation_name):
         return [
-            rel.relation_id
-            for rel in self._state.relations
-            if rel.endpoint == relation_name
+            rel.id for rel in self._state.relations if rel.endpoint == relation_name
         ]
 
     def relation_list(self, relation_id: int) -> Tuple[str, ...]:
         relation = self._get_relation_by_id(relation_id)
 
         if isinstance(relation, PeerRelation):
             return tuple(
@@ -627,14 +625,21 @@
             # ops will not let us get there if the resource name is unknown from metadata.
             # but if the user forgot to add it in State, then we remind you of that.
             raise RuntimeError(
                 f"Inconsistent state: "
                 f"resource {resource_name} not found in State. please pass it.",
             )
 
+    def credential_get(self) -> CloudSpec:
+        if not self._state.cloud_spec:
+            raise ModelError(
+                "ERROR cloud spec is empty, initialise it with `scenario.State(cloud_spec=scenario.CloudSpec(...))`",
+            )
+        return self._state.cloud_spec._to_ops()
+
 
 class _MockPebbleClient(_TestingPebbleClient):
     def __init__(
         self,
         socket_path: str,
         container_root: Path,
         mounts: Dict[str, Mount],
```

### Comparing `ops-scenario-6.0.3/scenario/ops_main_mock.py` & `ops_scenario-6.0.4/scenario/ops_main_mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 # Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 import inspect
 import os
+import sys
 from typing import TYPE_CHECKING, Any, Optional, Sequence, cast
 
 import ops.charm
 import ops.framework
 import ops.model
 import ops.storage
 from ops import CharmBase
@@ -92,14 +93,17 @@
         state=state,
         event=event,
         context=context,
         charm_spec=charm_spec,
     )
     debug = "JUJU_DEBUG" in os.environ
     setup_root_logging(model_backend, debug=debug)
+    # ops sets sys.excepthook to go to Juju's debug-log, but that's not useful
+    # in a testing context, so reset it.
+    sys.excepthook = sys.__excepthook__
     ops_logger.debug(
         "Operator Framework %s up and running.",
         ops.__version__,
     )  # type:ignore
 
     metadata = (charm_dir / "metadata.yaml").read_text()
     actions_meta = charm_dir / "actions.yaml"
@@ -111,15 +115,15 @@
     meta = CharmMeta.from_yaml(metadata, actions_metadata)
 
     # ops >= 2.10
     if inspect.signature(ops.model.Model).parameters.get("broken_relation_id"):
         # If we are in a RelationBroken event, we want to know which relation is
         # broken within the model, not only in the event's `.relation` attribute.
         broken_relation_id = (
-            event.relation.relation_id  # type: ignore
+            event.relation.id  # type: ignore
             if event.name.endswith("_relation_broken")
             else None
         )
 
         model = ops.model.Model(
             meta,
             model_backend,
```

### Comparing `ops-scenario-6.0.3/scenario/runtime.py` & `ops_scenario-6.0.4/scenario/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
             if isinstance(relation, PeerRelation):
                 remote_app_name = self._app_name
             else:
                 remote_app_name = relation.remote_app_name
             env.update(
                 {
                     "JUJU_RELATION": relation.endpoint,
-                    "JUJU_RELATION_ID": str(relation.relation_id),
+                    "JUJU_RELATION_ID": str(relation.id),
                     "JUJU_REMOTE_APP": remote_app_name,
                 },
             )
 
             remote_unit_id = event.relation_remote_unit_id
 
             # don't check truthiness because remote_unit_id could be 0
```

### Comparing `ops-scenario-6.0.3/scenario/sequences.py` & `ops_scenario-6.0.4/scenario/sequences.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/scenario/state.py` & `ops_scenario-6.0.4/scenario/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     Type,
     TypeVar,
     Union,
     cast,
 )
 from uuid import uuid4
 
+import ops
 import yaml
 from ops import pebble
 from ops.charm import CharmBase, CharmEvents
 from ops.model import SecretRotate, StatusBase
 
 from scenario.logger import logger as scenario_logger
 
@@ -137,14 +138,85 @@
 
     def copy(self) -> "Self":
         """Produce a deep copy of this object."""
         return copy.deepcopy(self)
 
 
 @dataclasses.dataclass(frozen=True)
+class CloudCredential:
+    auth_type: str
+    """Authentication type."""
+
+    attributes: Dict[str, str] = dataclasses.field(default_factory=dict)
+    """A dictionary containing cloud credentials.
+
+    For example, for AWS, it contains `access-key` and `secret-key`;
+    for Azure, `application-id`, `application-password` and `subscription-id`
+    can be found here.
+    """
+
+    redacted: List[str] = dataclasses.field(default_factory=list)
+    """A list of redacted generic cloud API secrets."""
+
+    def _to_ops(self) -> ops.CloudCredential:
+        return ops.CloudCredential(
+            auth_type=self.auth_type,
+            attributes=self.attributes,
+            redacted=self.redacted,
+        )
+
+
+@dataclasses.dataclass(frozen=True)
+class CloudSpec:
+    type: str
+    """Type of the cloud."""
+
+    name: str = "localhost"
+    """Juju cloud name."""
+
+    region: Optional[str] = None
+    """Region of the cloud."""
+
+    endpoint: Optional[str] = None
+    """Endpoint of the cloud."""
+
+    identity_endpoint: Optional[str] = None
+    """Identity endpoint of the cloud."""
+
+    storage_endpoint: Optional[str] = None
+    """Storage endpoint of the cloud."""
+
+    credential: Optional[CloudCredential] = None
+    """Cloud credentials with key-value attributes."""
+
+    ca_certificates: List[str] = dataclasses.field(default_factory=list)
+    """A list of CA certificates."""
+
+    skip_tls_verify: bool = False
+    """Whether to skip TLS verfication."""
+
+    is_controller_cloud: bool = False
+    """If this is the cloud used by the controller."""
+
+    def _to_ops(self) -> ops.CloudSpec:
+        return ops.CloudSpec(
+            type=self.type,
+            name=self.name,
+            region=self.region,
+            endpoint=self.endpoint,
+            identity_endpoint=self.identity_endpoint,
+            storage_endpoint=self.storage_endpoint,
+            credential=self.credential._to_ops() if self.credential else None,
+            ca_certificates=self.ca_certificates,
+            skip_tls_verify=self.skip_tls_verify,
+            is_controller_cloud=self.is_controller_cloud,
+        )
+
+
+@dataclasses.dataclass(frozen=True)
 class Secret(_DCBase):
     id: str
     # CAUTION: ops-created Secrets (via .add_secret()) will have a canonicalized
     #  secret id (`secret:` prefix)
     #  but user-created ones will not. Using post-init to patch it in feels bad, but requiring the user to
     #  add the prefix manually every time seems painful as well.
 
@@ -349,15 +421,15 @@
     endpoint: str
     """Relation endpoint name. Must match some endpoint name defined in metadata.yaml."""
 
     interface: Optional[str] = None
     """Interface name. Must match the interface name attached to this endpoint in metadata.yaml.
     If left empty, it will be automatically derived from metadata.yaml."""
 
-    relation_id: int = dataclasses.field(default_factory=next_relation_id)
+    id: int = dataclasses.field(default_factory=next_relation_id)
     """Juju relation ID. Every new Relation instance gets a unique one,
     if there's trouble, override."""
 
     local_app_data: "RawDataBagContents" = dataclasses.field(default_factory=dict)
     """This application's databag for this relation."""
 
     local_unit_data: "RawDataBagContents" = dataclasses.field(
@@ -558,16 +630,16 @@
 
     space = string.ascii_letters + string.digits
     return "".join(random.choice(space) for _ in range(20))
 
 
 @dataclasses.dataclass(frozen=True)
 class Model(_DCBase):
-    name: str = _random_model_name()
-    uuid: str = str(uuid4())
+    name: str = dataclasses.field(default_factory=_random_model_name)
+    uuid: str = dataclasses.field(default_factory=lambda: str(uuid4()))
 
     # whatever juju models --format=json | jq '.models[<current-model-index>].type' gives back.
     # TODO: make this exhaustive.
     type: Literal["kubernetes", "lxd"] = "kubernetes"
 
 
 # for now, proc mock allows you to map one command to one mocked output.
@@ -915,14 +987,16 @@
     # the current statuses. Will be cast to _EntitiyStatus in __post_init__
     app_status: Union[StatusBase, _EntityStatus] = _EntityStatus("unknown")
     """Status of the application."""
     unit_status: Union[StatusBase, _EntityStatus] = _EntityStatus("unknown")
     """Status of the unit."""
     workload_version: str = ""
     """Workload version."""
+    cloud_spec: Optional[CloudSpec] = None
+    """Cloud specification information (metadata) including credentials."""
 
     def __post_init__(self):
         for name in ["app_status", "unit_status"]:
             val = getattr(self, name)
             if isinstance(val, _EntityStatus):
                 pass
             elif isinstance(val, StatusBase):
@@ -1406,15 +1480,15 @@
                 #  don't have access to the local app name in this context.
                 remote_app = "local"
             else:
                 remote_app = relation.remote_app_name
 
             snapshot_data = {
                 "relation_name": relation.endpoint,
-                "relation_id": relation.relation_id,
+                "relation_id": relation.id,
                 "app_name": remote_app,
                 "unit_name": f"{remote_app}/{self.relation_remote_unit_id}",
             }
 
         return DeferredEvent(
             handle_path,
             owner_name,
```

### Comparing `ops-scenario-6.0.3/tests/helpers.py` & `ops_scenario-6.0.4/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_charm_spec_autoload.py` & `ops_scenario-6.0.4/tests/test_charm_spec_autoload.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_consistency_checker.py` & `ops_scenario-6.0.4/tests/test_consistency_checker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import pytest
 from ops.charm import CharmBase
 
+from scenario import Model
 from scenario.consistency_checker import check_consistency
 from scenario.runtime import InconsistentScenarioError
 from scenario.state import (
     RELATION_EVENTS_SUFFIX,
     Action,
+    CloudCredential,
+    CloudSpec,
     Container,
     Event,
     Network,
     PeerRelation,
     Relation,
     Secret,
     State,
@@ -152,14 +155,77 @@
     assert_consistent(
         State(config={"foo": True}),
         Event("bar"),
         _CharmSpec(MyCharm, {}, config={"options": {"foo": {"type": "boolean"}}}),
     )
 
 
+@pytest.mark.parametrize(
+    "config_type",
+    (
+        ("string", "foo", 1),
+        ("int", 1, "1"),
+        ("float", 1.0, 1),
+        ("boolean", False, "foo"),
+    ),
+)
+def test_config_types(config_type):
+    type_name, valid_value, invalid_value = config_type
+    assert_consistent(
+        State(config={"foo": valid_value}),
+        Event("bar"),
+        _CharmSpec(MyCharm, {}, config={"options": {"foo": {"type": type_name}}}),
+    )
+    assert_inconsistent(
+        State(config={"foo": invalid_value}),
+        Event("bar"),
+        _CharmSpec(MyCharm, {}, config={"options": {"foo": {"type": type_name}}}),
+    )
+
+
+@pytest.mark.parametrize("juju_version", ("3.4", "3.5", "4.0"))
+def test_config_secret(juju_version):
+    assert_consistent(
+        State(config={"foo": "secret:co28kefmp25c77utl3n0"}),
+        Event("bar"),
+        _CharmSpec(MyCharm, {}, config={"options": {"foo": {"type": "secret"}}}),
+        juju_version=juju_version,
+    )
+    assert_inconsistent(
+        State(config={"foo": 1}),
+        Event("bar"),
+        _CharmSpec(MyCharm, {}, config={"options": {"foo": {"type": "secret"}}}),
+    )
+    assert_inconsistent(
+        State(config={"foo": "co28kefmp25c77utl3n0"}),
+        Event("bar"),
+        _CharmSpec(MyCharm, {}, config={"options": {"foo": {"type": "secret"}}}),
+    )
+    assert_inconsistent(
+        State(config={"foo": "secret:secret"}),
+        Event("bar"),
+        _CharmSpec(MyCharm, {}, config={"options": {"foo": {"type": "secret"}}}),
+    )
+    assert_inconsistent(
+        State(config={"foo": "secret:co28kefmp25c77utl3n!"}),
+        Event("bar"),
+        _CharmSpec(MyCharm, {}, config={"options": {"foo": {"type": "secret"}}}),
+    )
+
+
+@pytest.mark.parametrize("juju_version", ("2.9", "3.3"))
+def test_config_secret_old_juju(juju_version):
+    assert_inconsistent(
+        State(config={"foo": "secret:co28kefmp25c77utl3n0"}),
+        Event("bar"),
+        _CharmSpec(MyCharm, {}, config={"options": {"foo": {"type": "secret"}}}),
+        juju_version=juju_version,
+    )
+
+
 @pytest.mark.parametrize("bad_v", ("1.0", "0", "1.2", "2.35.42", "2.99.99", "2.99"))
 def test_secrets_jujuv_bad(bad_v):
     secret = Secret("secret:foo", {0: {"a": "b"}})
     assert_inconsistent(
         State(secrets=[secret]),
         Event("bar"),
         _CharmSpec(MyCharm, {}),
@@ -334,40 +400,34 @@
                 MyCharm, meta={}, actions={"foo": {"params": {"bar": {"type": ptype}}}}
             ),
         )
 
 
 def test_duplicate_relation_ids():
     assert_inconsistent(
-        State(
-            relations=[Relation("foo", relation_id=1), Relation("bar", relation_id=1)]
-        ),
+        State(relations=[Relation("foo", id=1), Relation("bar", id=1)]),
         Event("start"),
         _CharmSpec(
             MyCharm,
             meta={
                 "requires": {"foo": {"interface": "foo"}, "bar": {"interface": "bar"}}
             },
         ),
     )
 
 
 def test_relation_without_endpoint():
     assert_inconsistent(
-        State(
-            relations=[Relation("foo", relation_id=1), Relation("bar", relation_id=1)]
-        ),
+        State(relations=[Relation("foo", id=1), Relation("bar", id=1)]),
         Event("start"),
         _CharmSpec(MyCharm, meta={"name": "charlemagne"}),
     )
 
     assert_consistent(
-        State(
-            relations=[Relation("foo", relation_id=1), Relation("bar", relation_id=2)]
-        ),
+        State(relations=[Relation("foo", id=1), Relation("bar", id=2)]),
         Event("start"),
         _CharmSpec(
             MyCharm,
             meta={
                 "requires": {"foo": {"interface": "foo"}, "bar": {"interface": "bar"}}
             },
         ),
@@ -501,7 +561,40 @@
             meta={
                 "name": "pinky",
                 "extra-bindings": {"foo": {}},
                 "requires": {"bar": {"interface": "bar"}},
             },
         ),
     )
+
+
+def test_cloudspec_consistency():
+    cloud_spec = CloudSpec(
+        type="lxd",
+        endpoint="https://127.0.0.1:8443",
+        credential=CloudCredential(
+            auth_type="clientcertificate",
+            attributes={
+                "client-cert": "foo",
+                "client-key": "bar",
+                "server-cert": "baz",
+            },
+        ),
+    )
+
+    assert_consistent(
+        State(cloud_spec=cloud_spec, model=Model(name="lxd-model", type="lxd")),
+        Event("start"),
+        _CharmSpec(
+            MyCharm,
+            meta={"name": "MyVMCharm"},
+        ),
+    )
+
+    assert_inconsistent(
+        State(cloud_spec=cloud_spec, model=Model(name="k8s-model", type="kubernetes")),
+        Event("start"),
+        _CharmSpec(
+            MyCharm,
+            meta={"name": "MyK8sCharm"},
+        ),
+    )
```

### Comparing `ops-scenario-6.0.3/tests/test_context.py` & `ops_scenario-6.0.4/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_dcbase.py` & `ops_scenario-6.0.4/tests/test_dcbase.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_actions.py` & `ops_scenario-6.0.4/tests/test_e2e/test_actions.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_builtin_scenes.py` & `ops_scenario-6.0.4/tests/test_e2e/test_builtin_scenes.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_config.py` & `ops_scenario-6.0.4/tests/test_e2e/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     trigger(
         State(
             config={"foo": "bar", "baz": 1},
         ),
         "update_status",
         mycharm,
         meta={"name": "foo"},
-        config={"options": {"foo": {"type": "string"}, "baz": {"type": "integer"}}},
+        config={"options": {"foo": {"type": "string"}, "baz": {"type": "int"}}},
         post_event=check_cfg,
     )
 
 
 def test_config_get_default_from_meta(mycharm):
     def check_cfg(charm: CharmBase):
         assert charm.config["foo"] == "bar"
```

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_custom_event_triggers.py` & `ops_scenario-6.0.4/tests/test_e2e/test_custom_event_triggers.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_deferred.py` & `ops_scenario-6.0.4/tests/test_e2e/test_deferred.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     )
 
     # we deferred the first 2 events we saw: foo_relation_changed, start.
     assert len(out.deferred) == 2
     assert out.deferred[0].name == "foo_relation_changed"
     assert out.deferred[0].snapshot_data == {
         "relation_name": rel.endpoint,
-        "relation_id": rel.relation_id,
+        "relation_id": rel.id,
         "app_name": "remote",
         "unit_name": "remote/1",
     }
     assert out.deferred[1].name == "start"
 
     # we saw start and foo_relation_changed.
     assert len(mycharm.captured) == 3
```

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_event.py` & `ops_scenario-6.0.4/tests/test_e2e/test_event.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_event_bind.py` & `ops_scenario-6.0.4/tests/test_e2e/test_event_bind.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_juju_log.py` & `ops_scenario-6.0.4/tests/test_e2e/test_juju_log.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_manager.py` & `ops_scenario-6.0.4/tests/test_e2e/test_manager.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_network.py` & `ops_scenario-6.0.4/tests/test_e2e/test_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         "update_status",
         State(
             relations=[
                 Relation(
                     interface="foo",
                     remote_app_name="remote",
                     endpoint="metrics-endpoint",
-                    relation_id=1,
+                    id=1,
                 ),
             ],
             networks={"foo": Network.default(private_address="4.4.4.4")},
         ),
     ) as mgr:
         # we have a network for the relation
         rel = mgr.charm.model.get_relation("metrics-endpoint")
@@ -106,15 +106,15 @@
         "update_status",
         State(
             relations=[
                 Relation(
                     interface="foo",
                     remote_app_name="remote",
                     endpoint="metrics-endpoint",
-                    relation_id=1,
+                    id=1,
                 ),
             ],
             networks={"bar": Network.default()},
         ),
     ) as mgr:
         with pytest.raises(RelationNotFoundError):
             net = mgr.charm.model.get_binding("foo").network
```

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_pebble.py` & `ops_scenario-6.0.4/tests/test_e2e/test_pebble.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_play_assertions.py` & `ops_scenario-6.0.4/tests/test_e2e/test_play_assertions.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         assert remote_app_data == {"yaba": "doodle"}
 
     state_in = State(
         relations=[
             Relation(
                 endpoint="relation_test",
                 interface="azdrubales",
-                relation_id=1,
+                id=1,
                 remote_app_name="karlos",
                 remote_app_data={"yaba": "doodle"},
                 remote_units_data={0: {"foo": "bar"}, 1: {"baz": "qux"}},
             )
         ]
     )
     trigger(
```

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_ports.py` & `ops_scenario-6.0.4/tests/test_e2e/test_ports.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_relations.py` & `ops_scenario-6.0.4/tests/test_e2e/test_relations.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,15 +384,15 @@
 
 def test_relation_ids():
     from scenario.state import _next_relation_id_counter
 
     initial_id = _next_relation_id_counter
     for i in range(10):
         rel = Relation("foo")
-        assert rel.relation_id == initial_id + i
+        assert rel.id == initial_id + i
 
 
 def test_broken_relation_not_in_model_relations(mycharm):
     rel = Relation("foo")
 
     with Context(
         mycharm, meta={"name": "local", "requires": {"foo": {"interface": "foo"}}}
```

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_rubbish_events.py` & `ops_scenario-6.0.4/tests/test_e2e/test_rubbish_events.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_secrets.py` & `ops_scenario-6.0.4/tests/test_e2e/test_secrets.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,17 +517,15 @@
     )
     relation_remote_app = "remote_secret_desirerer"
     relation_id = 42
 
     state = State(
         leader=True,
         relations=[
-            Relation(
-                "bar", remote_app_name=relation_remote_app, relation_id=relation_id
-            )
+            Relation("bar", remote_app_name=relation_remote_app, id=relation_id)
         ],
     )
 
     with context.manager("start", state) as mgr:
         charm = mgr.charm
         secret = charm.app.add_secret({"foo": "bar"}, label="mylabel")
         bar_relation = charm.model.relations["bar"][0]
```

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_state.py` & `ops_scenario-6.0.4/tests/test_e2e/test_state.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_status.py` & `ops_scenario-6.0.4/tests/test_e2e/test_status.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_storage.py` & `ops_scenario-6.0.4/tests/test_e2e/test_storage.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_stored_state.py` & `ops_scenario-6.0.4/tests/test_e2e/test_stored_state.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_e2e/test_vroot.py` & `ops_scenario-6.0.4/tests/test_e2e/test_vroot.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_emitted_events_util.py` & `ops_scenario-6.0.4/tests/test_emitted_events_util.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_plugin.py` & `ops_scenario-6.0.4/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tests/test_runtime.py` & `ops_scenario-6.0.4/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-6.0.3/tox.ini` & `ops_scenario-6.0.4/tox.ini`

 * *Files identical despite different names*

