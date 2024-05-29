# Comparing `tmp/entity_management-1.2.46.tar.gz` & `tmp/entity_management-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entity_management-1.2.46.tar", last modified: Wed May  8 09:24:05 2024, max compression
+gzip compressed data, was "entity_management-1.3.0.tar", last modified: Wed May 29 12:58:39 2024, max compression
```

## Comparing `entity_management-1.2.46.tar` & `entity_management-1.3.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:05.776922 entity_management-1.2.46/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:05.760922 entity_management-1.2.46/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:05.764922 entity_management-1.2.46/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-08 09:24:02.000000 entity_management-1.2.46/.github/workflows/sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 09:24:02.000000 entity_management-1.2.46/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-08 09:24:02.000000 entity_management-1.2.46/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-08 09:24:02.000000 entity_management-1.2.46/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-08 09:24:02.000000 entity_management-1.2.46/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 09:24:02.000000 entity_management-1.2.46/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-08 09:24:02.000000 entity_management-1.2.46/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14763 2024-05-08 09:24:05.776922 entity_management-1.2.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-08 09:24:02.000000 entity_management-1.2.46/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:05.764922 entity_management-1.2.46/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-08 09:24:02.000000 entity_management-1.2.46/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:05.764922 entity_management-1.2.46/doc/source/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-08 09:24:02.000000 entity_management-1.2.46/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-05-08 09:24:02.000000 entity_management-1.2.46/doc/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-08 09:24:02.000000 entity_management-1.2.46/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-08 09:24:02.000000 entity_management-1.2.46/doc/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-08 09:24:02.000000 entity_management-1.2.46/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-05-08 09:24:02.000000 entity_management-1.2.46/doc/source/prov_patterns.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:05.768922 entity_management-1.2.46/entity_management/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/atlas.py
--rw-r--r--   0 runner    (1001) docker     (127)    29511 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:05.768922 entity_management-1.2.46/entity_management/circuit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/circuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:05.768922 entity_management-1.2.46/entity_management/circuit/building/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/circuit/building/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/circuit/building/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:05.768922 entity_management-1.2.46/entity_management/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/cli/model_building_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    21912 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/electrophysiology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/emodel.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)    17732 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16956 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/typecheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-08 09:24:02.000000 entity_management-1.2.46/entity_management/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:05.776922 entity_management-1.2.46/entity_management.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14763 2024-05-08 09:24:05.000000 entity_management-1.2.46/entity_management.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-08 09:24:05.000000 entity_management-1.2.46/entity_management.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:24:05.000000 entity_management-1.2.46/entity_management.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 09:24:05.000000 entity_management-1.2.46/entity_management.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-08 09:24:05.000000 entity_management-1.2.46/entity_management.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 09:24:05.000000 entity_management-1.2.46/entity_management.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-08 09:24:02.000000 entity_management-1.2.46/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:24:05.776922 entity_management-1.2.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:24:02.000000 entity_management-1.2.46/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:05.772922 entity_management-1.2.46/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:24:05.776922 entity_management-1.2.46/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/atlas_release_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/cells_page1_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/cells_page2_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/detailed_circuit_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/emodel_configuration_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/emodel_data_catalog_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/emodel_pipeline_settings_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/emodel_release_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/emodel_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/emodel_script_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/emodel_workflow_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/entity_data_download_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/extraction_targets_configuration_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/file_link_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/file_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/fitness_calculator_configuration_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/sparql_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/sub_cellular_model_script_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/trace_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/unconstrained_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/data/workflow_resp.json
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/test_atlas.py
--rw-r--r--   0 runner    (1001) docker     (127)    17390 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/test_emodel.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/test_model_building_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/test_morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/test_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)    29566 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/test_typecheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-08 09:24:02.000000 entity_management-1.2.46/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-08 09:24:02.000000 entity_management-1.2.46/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:39.030239 entity_management-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:39.014239 entity_management-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:39.018239 entity_management-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-29 12:58:34.000000 entity_management-1.3.0/.github/workflows/sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-29 12:58:34.000000 entity_management-1.3.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-29 12:58:34.000000 entity_management-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-29 12:58:34.000000 entity_management-1.3.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-29 12:58:34.000000 entity_management-1.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-29 12:58:34.000000 entity_management-1.3.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 12:58:34.000000 entity_management-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-05-29 12:58:39.026239 entity_management-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-29 12:58:34.000000 entity_management-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:39.018239 entity_management-1.3.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-29 12:58:34.000000 entity_management-1.3.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:39.018239 entity_management-1.3.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-29 12:58:34.000000 entity_management-1.3.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-05-29 12:58:34.000000 entity_management-1.3.0/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-29 12:58:34.000000 entity_management-1.3.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-29 12:58:34.000000 entity_management-1.3.0/doc/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-29 12:58:34.000000 entity_management-1.3.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-05-29 12:58:34.000000 entity_management-1.3.0/doc/source/prov_patterns.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:39.022239 entity_management-1.3.0/entity_management/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29580 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:39.022239 entity_management-1.3.0/entity_management/circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/circuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:39.022239 entity_management-1.3.0/entity_management/circuit/building/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/circuit/building/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/circuit/building/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:39.022239 entity_management-1.3.0/entity_management/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/cli/model_building_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/electrophysiology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/emodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17790 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17001 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-29 12:58:34.000000 entity_management-1.3.0/entity_management/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:39.026239 entity_management-1.3.0/entity_management.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-05-29 12:58:38.000000 entity_management-1.3.0/entity_management.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-29 12:58:39.000000 entity_management-1.3.0/entity_management.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:58:38.000000 entity_management-1.3.0/entity_management.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 12:58:38.000000 entity_management-1.3.0/entity_management.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-29 12:58:38.000000 entity_management-1.3.0/entity_management.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 12:58:38.000000 entity_management-1.3.0/entity_management.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-29 12:58:34.000000 entity_management-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:58:39.030239 entity_management-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:58:34.000000 entity_management-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:39.026239 entity_management-1.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:39.026239 entity_management-1.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/atlas_release_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/cells_page1_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/cells_page2_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/detailed_circuit_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/emodel_configuration_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/emodel_data_catalog_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/emodel_pipeline_settings_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/emodel_release_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/emodel_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/emodel_script_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/emodel_workflow_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/entity_data_download_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/extraction_targets_configuration_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/file_link_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/file_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/fitness_calculator_configuration_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/sparql_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/sub_cellular_model_script_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/trace_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/unconstrained_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/data/workflow_resp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/test_atlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/test_emodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/test_model_building_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/test_morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/test_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29566 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/test_typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-29 12:58:34.000000 entity_management-1.3.0/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-29 12:58:34.000000 entity_management-1.3.0/tox.ini
```

### Comparing `entity_management-1.2.46/.github/workflows/sdist.yml` & `entity_management-1.3.0/.github/workflows/sdist.yml`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/.github/workflows/tox.yml` & `entity_management-1.3.0/.github/workflows/tox.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,37 +12,37 @@
 
 jobs:
   checks:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        tox-env: ['py3', 'check-packaging', 'lint', 'coverage', 'docs']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
 
     steps:
 
     - uses: actions/checkout@v4
 
     - name: Install graphviz if docs tox-env
       if: matrix.tox-env == 'docs'
       run: |
         sudo apt-get update
         sudo apt-get -y install graphviz
 
-    - name: Set up Python 3.10
+    - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
-        python-version: '3.10'
+        python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools
-        pip install tox-gh-actions
+        python -m pip install tox-gh-actions
 
     - name: Run tox
-      run: tox -e ${{ matrix.tox-env }}
+      run: tox
 
     - name: Upload coverage reports to Codecov
       uses: codecov/codecov-action@v4.0.1
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         slug: BlueBrain/entity-management
```

### Comparing `entity_management-1.2.46/.pylintrc` & `entity_management-1.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/LICENSE.txt` & `entity_management-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/PKG-INFO` & `entity_management-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entity-management
-Version: 1.2.46
+Version: 1.3.0
 Summary: Access to production entity management
 Author: Blue Brain Project, EPFL
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -203,23 +203,24 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/BlueBrain/entity-management
-Project-URL: Repository, https://github.com/BlueBrain/NeuroM.git
-Project-URL: Tracker, https://github.com/BlueBrain/entity-management/issues
+Project-URL: Documentation, https://entity-management.readthedocs.io/en/stable/
+Project-URL: Repository, https://github.com/BlueBrain/entity-management
+Project-URL: Issues, https://github.com/BlueBrain/entity-management/issues
 Keywords: computational neuroscience,simulation,analysis,nexus,parameters,BlueBrainProject
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 Requires-Dist: requests
 Requires-Dist: attrs
 Requires-Dist: python-dateutil
 Requires-Dist: sparqlwrapper
@@ -232,14 +233,20 @@
 Requires-Dist: sphinx-bluebrain-theme; extra == "docs"
 
 entity-management
 =================
 
 Library for handling NEXUS entity dataclass definitions.
 
+Documentation
+=============
+
+* `latest release <https://entity-management.readthedocs.io/en/stable/>`_
+* `latest snapshot <https://entity-management.readthedocs.io/en/latest/>`_
+
 Installation
 ============
 
 entity-management can be pip installed with the following command:
 
 .. code-block:: bash
```

### Comparing `entity_management-1.2.46/README.rst` & `entity_management-1.3.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 entity-management
 =================
 
 Library for handling NEXUS entity dataclass definitions.
 
+Documentation
+=============
+
+* `latest release <https://entity-management.readthedocs.io/en/stable/>`_
+* `latest snapshot <https://entity-management.readthedocs.io/en/latest/>`_
+
 Installation
 ============
 
 entity-management can be pip installed with the following command:
 
 .. code-block:: bash
```

### Comparing `entity_management-1.2.46/doc/Makefile` & `entity_management-1.3.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/doc/source/cli.rst` & `entity_management-1.3.0/doc/source/cli.rst`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/doc/source/conf.py` & `entity_management-1.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/doc/source/examples.rst` & `entity_management-1.3.0/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/doc/source/index.rst` & `entity_management-1.3.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/doc/source/prov_patterns.rst` & `entity_management-1.3.0/doc/source/prov_patterns.rst`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/entity_management/atlas.py` & `entity_management-1.3.0/entity_management/atlas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """Atlas related entities."""
 
+from typing import List
+
 from entity_management.base import BrainLocation, Derivation, Identifiable, Subject, attributes
 from entity_management.core import Contribution, DataDownload, Entity
 from entity_management.util import AttrOf
 
 
 @attributes(
     {
@@ -104,15 +108,15 @@
 )
 class HemisphereAnnotationDataLayer(Entity):
     """Hemisphere annotation from Allen ccfv3 volume at 25 microns."""
 
 
 @attributes(
     {
-        "distribution": AttrOf(list[DataDownload]),
+        "distribution": AttrOf(List[DataDownload]),
     }
 )
 class ParcellationOntology(Entity):
     """Raster volume of the brain template. This originaly comes from AIBS CCF (25µm)"""
 
 
 @attributes(
@@ -169,47 +173,47 @@
 class AtlasRelease(Entity):
     """AtlasRelease resource representation."""
 
 
 @attributes(
     {
         "atlasRelease": AttrOf(AtlasRelease, default=None),
-        "about": AttrOf(list[str], default=None),
+        "about": AttrOf(List[str], default=None),
         "brainLocation": AttrOf(BrainLocation, default=None),
-        "contribution": AttrOf(list[Contribution], default=None),
+        "contribution": AttrOf(List[Contribution], default=None),
         "derivation": AttrOf(Derivation, default=None),
         "distribution": AttrOf(DataDownload),
         "subject": AttrOf(Subject, default=None),
     }
 )
 class CellCompositionSummary(Entity):
     """CellCompositionSummary"""
 
 
 @attributes(
     {
-        "about": AttrOf(list[str], default=None),
+        "about": AttrOf(List[str], default=None),
         "atlasRelease": AttrOf(AtlasRelease, default=None),
         "brainLocation": AttrOf(BrainLocation, default=None),
-        "contribution": AttrOf(list[Contribution], default=None),
+        "contribution": AttrOf(List[Contribution], default=None),
         "derivation": AttrOf(Derivation, default=None),
         "distribution": AttrOf(DataDownload),
         "subject": AttrOf(Subject, default=None),
     }
 )
 class CellCompositionVolume(Entity):
     """CellCompositionVolume"""
 
 
 @attributes(
     {
-        "about": AttrOf(list[str], default=None),
+        "about": AttrOf(List[str], default=None),
         "atlasRelease": AttrOf(AtlasRelease),
         "atlasSpatialReferenceSystem": AttrOf(AtlasSpatialReferenceSystem, default=None),
         "brainLocation": AttrOf(BrainLocation, default=None),
         "cellCompositionSummary": AttrOf(CellCompositionSummary),
         "cellCompositionVolume": AttrOf(CellCompositionVolume),
-        "contribution": AttrOf(list[Contribution], default=None),
+        "contribution": AttrOf(List[Contribution], default=None),
     }
 )
 class CellComposition(Entity):
     """CellComposition"""
```

### Comparing `entity_management-1.2.46/entity_management/base.py` & `entity_management-1.3.0/entity_management/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """
 Base simulation entities
 
 .. inheritance-diagram:: entity_management.base
    :parts: 2
 """
 
@@ -395,15 +397,15 @@
     if typecheck.is_data_mapping(data_raw) and JSLD_TYPE in data_raw:
         data_type = nexus.get_type_from_name(data_raw[JSLD_TYPE])
         return _deserialize_json_to_datatype(
             data_type, data_raw, context=context, base=base, org=org, token=token
         )
 
     # e.g. int | float | dict
-    if type(data_raw) in type_args:
+    if type(data_raw) in typecheck.get_type_root_args(data_type):
         return data_raw
 
     raise NotImplementedError(
         "Unknown type/data combination:\n" f"data_type: {data_type}\n" f"data_raw : {data_raw}"
     )
```

### Comparing `entity_management-1.2.46/entity_management/circuit/building/functional.py` & `entity_management-1.3.0/entity_management/circuit/building/functional.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """Entities for s2f recipe generation."""
 
 import re
 from pathlib import Path
+from typing import List, Optional, Union
 
 import attr
 
 
 def _cls_name_to_snake_case(cls):
     name = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", cls.__name__)
     return re.sub("([a-z0-9])([A-Z])", r"\1_\2", name).lower()
@@ -29,46 +32,46 @@
 
 
 @attr.frozen
 class Sample:
     """Parameters for sampling bouton density."""
 
     size: int = 100  #: Sample size
-    target: str | None = None  #: Sample target
+    target: Optional[str] = None  #: Sample target
     #: Region of interest. If provided, only axonal segments within this region would be considered.
-    mask: str | None = None
+    mask: Optional[str] = None
     assume_nsyn_bouton: float = 1.0  #: FIMXE
     assume_syns_bouton: float = 1.0  #: Assumed synapse count per bouton
 
 
 @attr.frozen
 class EstimateSynsCon(Strategy):
     """Estimate the functional mean number of synapses per connection from the structural number \
     of appositions per connection. For the prediction, an algebraic expression using ‘n’ \
     (mean number of appositions) should be specified."""
 
     formula: str  #: Synapse number prediction formula.
     #: Synapse number prediction formula for EXC->EXC pathways.
     #: If omitted, general formula would be used
-    formula_ee: str | None = None
+    formula_ee: Optional[str] = None
     #: Synapse number prediction formula for EXC->INH pathways.
     #: If omitted, general formula would be used
-    formula_ei: str | None = None
+    formula_ei: Optional[str] = None
     #: Synapse number prediction formula for INH->EXC pathways.
     #: If omitted, general formula would be used
-    formula_ie: str | None = None
+    formula_ie: Optional[str] = None
     #: Synapse number prediction formula for INH->INH pathways.
     #: If omitted, general formula would be used
-    formula_ii: str | None = None
+    formula_ii: Optional[str] = None
     #: Max value for predicted synapse number.
     #: If omitted, the predicted synapse number is not clipped above NB: predicted synapse value
     #: would be always min-clipped to 1.0 to avoid invalid synapse count values.
-    max_value: float | None = None
+    max_value: Optional[float] = None
     #: Parameters for sampling bouton density OR path to bouton-density dataset already sampled
-    sample: Sample | Path | None = None
+    sample: Union[Sample, Path, None] = None
 
 
 @attr.frozen
 class ExperimentalSynsCon(Strategy):
     """Use the biological mean number of synapses per connection for a number of pathways where \
     experimental data is available."""
 
@@ -78,17 +81,17 @@
 
 @attr.frozen
 class EstimateBoutonReduction(Strategy):
     """Estimate an overall reduction factor based on an estimated mean bouton density over all \
     mtypes."""
 
     #: Path to bouton-density dataset representing reference biological data (OR single float value)
-    bio_data: Path | float
+    bio_data: Union[Path, float]
     #: Parameters for sampling bouton density OR path to bouton-density dataset already sampled
-    sample: Sample | Path | None = None
+    sample: Union[Sample, Path, None] = None
 
 
 @attr.frozen
 class EstimateIndividualBoutonReduction(EstimateBoutonReduction):
     """Estimate a reduction factor for each individual mtype, where experimental data is available.\
     """
 
@@ -100,22 +103,22 @@
     cv: float  #: cv_syns_connection value to use
 
 
 @attr.frozen
 class Recipe:
     """Synapse pruning functionalizer recipe."""
 
-    strategies: list[
-        (
-            EstimateSynsCon
-            | ExperimentalSynsCon
-            | EstimateBoutonReduction
-            | EstimateIndividualBoutonReduction
-            | GeneralizedCv
-        )
+    strategies: List[
+        Union[
+            EstimateSynsCon,
+            ExperimentalSynsCon,
+            EstimateBoutonReduction,
+            EstimateIndividualBoutonReduction,
+            GeneralizedCv,
+        ]
     ] = []  #:
 
     def asdict(self):
         """Recipe dictionary representation."""
         return [
             {
                 _cls_name_to_snake_case(type(strategy)): attr.asdict(
```

### Comparing `entity_management-1.2.46/entity_management/cli/base.py` & `entity_management-1.3.0/entity_management/cli/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """Command line interface."""
 
 import logging
 import os
 from pprint import pprint
 
 import click
```

### Comparing `entity_management-1.2.46/entity_management/cli/model_building_config.py` & `entity_management-1.3.0/entity_management/cli/model_building_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """Command line interface for Model Building Config."""
 
 import json
 import logging
 import os
 import re
 
@@ -80,20 +82,21 @@
 
 def _get_ids_from_dict(config):
     ids = set()
     if isinstance(config, dict):
         id_ = _get_key(config, "id")
         type_ = _get_key(config, "type")
         if id_ and type_:
-            if rev := (_get_key(config, "_rev") or _get_key(config, "rev")):
+            rev = _get_key(config, "_rev") or _get_key(config, "rev")
+            if rev:
                 id_ = f"{id_}?rev={rev}"
             ids.add(id_)
         for key, item in config.items():
             if key not in UNALLOWED_ID_KEYS:
-                ids |= _get_ids_from_dict(item)
+                ids.update(_get_ids_from_dict(item))
 
     return ids
 
 
 def _get_timestamp(entity):
     return re.sub(":", "-", entity.get("_createdAt", ""))
 
@@ -122,22 +125,23 @@
     ids = set()
     distribution = entity.get("distribution", [])
 
     if not isinstance(distribution, list):
         distribution = [distribution]
 
     for d_item in distribution:
-        if url := d_item.get("contentUrl"):
+        url = d_item.get("contentUrl")
+        if url:
             filename = _get_distribution_filename(entity, d_item)
             print(f"    {filename}")
             download_file(url, path, file_name=filename)
             mapping[url] = filename
             if d_item.get("encodingFormat", "") == "application/json":
                 content = file_as_dict(url)
-                ids |= _get_ids_from_dict(content)
+                ids.update(_get_ids_from_dict(content))
 
     return ids
 
 
 def _download_entity_get_ids(id_, path, mapping):
     def _err_exit():
         print(f"\nERROR: Can't fetch: {id_}\n")
@@ -154,15 +158,15 @@
 
     filename = _get_entity_filename(entity)
     _write_json(entity, path, filename)
     mapping[id_] = filename
 
     entity.pop("@id", None)
     ids = _get_ids_from_dict(entity)
-    ids |= download_and_get_ids_from_distribution(entity, path, mapping)
+    ids.update(download_and_get_ids_from_distribution(entity, path, mapping))
 
     return ids
 
 
 def _download_entity_recursive(id_, path, depth, mapping=None):
     mapping = mapping or {}
```

### Comparing `entity_management-1.2.46/entity_management/config.py` & `entity_management-1.3.0/entity_management/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """Entities for Model building config
 
     see entity_management/cli/model_building_config.py for an example
     on how to use the objects
 
 """
```

### Comparing `entity_management-1.2.46/entity_management/context.py` & `entity_management-1.3.0/entity_management/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """Context related functions."""
 
+from __future__ import annotations
+
 from typing import Any
 
 from rdflib.plugins.shared.jsonld.context import Context
 
 from entity_management import nexus
 
 _CONTEXT_CACHE = {}
```

### Comparing `entity_management-1.2.46/entity_management/core.py` & `entity_management-1.3.0/entity_management/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """
 Provenance entities
 
 .. inheritance-diagram:: entity_management.core
    :top-classes: entity_management.base.BlankNode,
     entity_management.base.Identifiable
    :parts: 1
 """
 
 import os
 import uuid
 from datetime import datetime
 from io import IOBase, StringIO
 from pathlib import Path
+from typing import List
 
 from attr.validators import in_
 
 from entity_management import nexus
 
 # Subject used to be in this module. It is imported for backward compatibility
 from entity_management.base import Subject  # noqa pylint: disable=unused-import
@@ -439,20 +442,20 @@
     """Contribution"""
 
 
 @attributes(
     {
         "name": AttrOf(str, default=None),
         "description": AttrOf(str, default=None),
-        "wasAttributedTo": AttrOf(list[Agent], default=None),
+        "wasAttributedTo": AttrOf(List[Agent], default=None),
         "wasGeneratedBy": AttrOf(Identifiable, default=None),
-        "wasDerivedFrom": AttrOf(list[Identifiable], default=None),
+        "wasDerivedFrom": AttrOf(List[Identifiable], default=None),
         "dateCreated": AttrOf(datetime, default=None),
         "distribution": AttrOf(MaybeList[DataDownload], default=None),
-        "contribution": AttrOf(list[Contribution], default=None),
+        "contribution": AttrOf(List[Contribution], default=None),
     }
 )
 class Entity(Identifiable):
     """Enables provenance metadata when publishing/deprecating entities."""
 
     @classmethod
     def was_generated_by(cls, generated_by, **kwargs):
@@ -543,15 +546,15 @@
             use_auth=use_auth,
             include_rev=include_rev,
         )
 
 
 @attributes(
     {
-        "distribution": AttrOf(list[DataDownload], default=None),
+        "distribution": AttrOf(List[DataDownload], default=None),
     }
 )
 class MultiDistributionEntity(Entity):
     """Entity with one or more distributions."""
 
 
 @attributes(
```

### Comparing `entity_management-1.2.46/entity_management/electrophysiology.py` & `entity_management-1.3.0/entity_management/electrophysiology.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """
 Experimental morphologies entities
 
 .. inheritance-diagram:: entity_management.electrophysiology
    :top-classes: entity_management.electrophysiology._Entity,
     entity_management.electrophysiology.StimulusType, entity_management.core.Activity
    :parts: 1
```

### Comparing `entity_management-1.2.46/entity_management/emodel.py` & `entity_management-1.3.0/entity_management/emodel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """
 EModel related entities.
 See https://bbpgitlab.epfl.ch/dke/apps/brain-modeling-ontology/-/tree/develop/shapes/
 """
-
 from datetime import datetime
+from typing import List, Union
 
 from entity_management.atlas import AtlasRelease
 from entity_management.base import (
     BlankNode,
     BrainLocation,
     Frozen,
     Identifiable,
@@ -68,70 +70,72 @@
         "iteration": AttrOf(str, default=None),
         "score": AttrOf(float, default=None),
         "seed": AttrOf(int, default=None),
         "objectOfStudy": AttrOf(OntologyTerm, default=None),
         "brainLocation": AttrOf(BrainLocation, default=None),
         "atlasRelease": AttrOf(AtlasRelease, default=None),
         "subject": AttrOf(Subject, default=None),
-        "annotation": AttrOf(list[MTypeAnnotation | ETypeAnnotation], default=None),
+        "annotation": AttrOf(List[Union[MTypeAnnotation, ETypeAnnotation]], default=None),
     }
 )
 class EModelEntity(MultiDistributionEntity):
     """EModel entity with common EModel properties."""
 
 
 @attributes(
     {
-        "uses": AttrOf(list[Trace]),
+        "uses": AttrOf(List[Trace]),
     }
 )
 class ExtractionTargetsConfiguration(EModelEntity):
     """ExtractionTargetsConfiguration."""
 
 
 class EModelPipelineSettings(EModelEntity):
     """EModelPipelineSettings."""
 
 
 @attributes(
     {
-        "distribution": AttrOf(list[DataDownload]),
-        "exposesParameter": AttrOf(list[dict], default=None),
+        "distribution": AttrOf(List[DataDownload]),
+        "exposesParameter": AttrOf(List[dict], default=None),
         "modelId": AttrOf(str, default=None),
         "nmodlParameters": AttrOf(dict, default=None),
         "origin": AttrOf(str, default=None),
         "suffix": AttrOf(str, default=None),
-        "temperature": AttrOf(int | dict, default=None),
+        "temperature": AttrOf(Union[int, dict], default=None),
         "subject": AttrOf(Subject, default=None),
         "identifier": AttrOf(str, default=None),
         "mod": AttrOf(dict, default=None),
-        "ion": AttrOf(list[OntologyTerm], default=None),
+        "ion": AttrOf(List[OntologyTerm], default=None),
         "isLjpCorrected": AttrOf(bool, default=None),
         "objectOfStudy": AttrOf(OntologyTerm, default=None),
         "isTemperatureDependent": AttrOf(bool, default=None),
     }
 )
 class SubCellularModelScript(Entity):
     """SubCellularModelScript,"""
 
 
 @attributes(
     {
-        "uses": AttrOf(list[NeuronMorphology | SubCellularModelScript], default=None),
+        "uses": AttrOf(List[Union[NeuronMorphology, SubCellularModelScript]], default=None),
     }
 )
 class EModelConfiguration(EModelEntity):
     """EModelConfiguration."""
 
 
 @attributes(
     {
-        "generates": AttrOf(list[Identifiable], default=None),
+        "generates": AttrOf(List[Identifiable], default=None),
         "hasPart": AttrOf(
-            list[ExtractionTargetsConfiguration | EModelPipelineSettings | EModelConfiguration],
+            List[
+                Union[ExtractionTargetsConfiguration, EModelPipelineSettings, EModelConfiguration]
+            ],
             default=None,
         ),
         "state": AttrOf(str, default=None),
     }
 )
 class EModelWorkflow(EModelEntity):
     """EModelWorkflow."""
@@ -173,15 +177,15 @@
 )
 class EModel(EModelEntity):
     """EModel definition."""
 
 
 @attributes(
     {
-        "hasPart": AttrOf(list[EModel]),
+        "hasPart": AttrOf(List[EModel]),
         "brainLocation": AttrOf(BrainLocation),
         "distribution": AttrOf(DataDownload),
         "subject": AttrOf(Subject, default=None),
     }
 )
 class EModelDataCatalog(Entity):
     """EModel Data Catalog."""
```

### Comparing `entity_management-1.2.46/entity_management/morphology.py` & `entity_management-1.3.0/entity_management/morphology.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """
 Experimental morphologies entities
 
 .. inheritance-diagram:: entity_management.morphology
    :top-classes: entity_management.morphology.ReconstructedCell
    :parts: 1
 """
```

### Comparing `entity_management-1.2.46/entity_management/nexus.py` & `entity_management-1.3.0/entity_management/nexus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """New nexus access layer"""
 
 import json as js
 import logging
 import os
 import re
 import sys
@@ -70,15 +72,15 @@
         no_hash = re.sub(r",? *(Constraint|Node)(:|\() ?_:\w{32}\)?", "", error)
         no_hash = re.sub(r"^Error: Violation Error\((.*?)\). ", r"Violation(\g<1>):\n", no_hash)
         if no_hash.startswith("Violation"):
             color = "\033[92m"
             end_color = "\033[0m"
             color_url = re.sub(r"<(.*?)>", color + r"<\g<1>>" + end_color, no_hash)
 
-        print(color_url + "\n", file=sys.stderr)
+            print(color_url + "\n", file=sys.stderr)
 
 
 def _print_nexus_error(http_error):
     """Helper function to log nexus error response."""
     request = http_error.response.request
     response = http_error.response
     try:
@@ -211,30 +213,30 @@
     Returns:
         Json response.
     """
     assert id_url is not None
     assert rev > 0
     params = {"rev": rev}
     if sync_index:
-        params |= {"indexing": "sync"}
+        params.update({"indexing": "sync"})
     response = requests.put(
         id_url, headers=_get_headers(token), params=params, json=payload, timeout=10
     )
     response.raise_for_status()
     return _to_json(response, payload)
 
 
 @_nexus_wrapper
 def deprecate(id_url, rev, sync_index=False, token=None):
     """Mark entity as deprecated, return json response"""
     assert id_url is not None
     assert rev > 0
     params = {"rev": rev}
     if sync_index:
-        params |= {"indexing": "sync"}
+        params.update({"indexing": "sync"})
     response = requests.delete(id_url, headers=_get_headers(token), params=params, timeout=10)
     response.raise_for_status()
     return _to_json(response)
 
 
 @_nexus_wrapper
 def load_by_url(url, params=None, stream=False, token=None):
@@ -291,15 +293,15 @@
     """
     base_url = get_base_url(base=base, org=org, proj=proj, cross_bucket=cross_bucket)
 
     resource_id, revision_query = split_url_from_revision_query(resource_id)
 
     if params is None:
         params = {}
-    params |= revision_query
+    params.update(revision_query)
 
     url = f"{base_url}/{quote(resource_id)}"
     return load_by_url(url=url, params=params, stream=stream, token=token)
 
 
 @_nexus_wrapper
 def get_current_agent(token=None):
```

### Comparing `entity_management-1.2.46/entity_management/settings.py` & `entity_management-1.3.0/entity_management/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """Settings module"""
 
 import os
 
 from rdflib import Namespace
 
 JSLD_ID = "@id"
```

### Comparing `entity_management-1.2.46/entity_management/simulation.py` & `entity_management-1.3.0/entity_management/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """Simulation domain entities."""
 
 from datetime import datetime
-from typing import Union
+from typing import List, Union
 
 from attr.validators import in_
 
 from entity_management import morphology
 from entity_management.atlas import AtlasRelease
 from entity_management.base import (
     BrainLocation,
@@ -145,24 +147,24 @@
 
 
 @attributes()
 class SingleCellSimulationTrace(Entity):
     """Single cell simulation trace file"""
 
 
-@attributes({"hadMember": AttrOf(list[Trace], default=None)})
+@attributes({"hadMember": AttrOf(List[Trace], default=None)})
 class TraceCollection(Entity):
     """Collection of traces
 
     Args:
         hadMember(List[Trace]): List of traces.
     """
 
 
-@attributes({"hadMember": AttrOf(list[Trace], default=None)})
+@attributes({"hadMember": AttrOf(List[Trace], default=None)})
 class CoreTraceCollection(Entity):
     """Collection of traces
 
     Args:
         hadMember(List[Trace]): List of traces.
     """
 
@@ -198,15 +200,15 @@
 
 @attributes(
     {
         "brainLocation": AttrOf(BrainLocation),
         "subject": AttrOf(Subject, default=None),
         "mType": AttrOf(OntologyTerm),
         "eType": AttrOf(OntologyTerm),
-        "experimentalCell": AttrOf(list[ExperimentalCell]),
+        "experimentalCell": AttrOf(List[ExperimentalCell]),
         "featureExtractionConfiguration": AttrOf(dict),
         "stimuliToExperimentMap": AttrOf(dict, default=None),
     }
 )
 class BluePyEfeConfiguration(Entity):
     """BluePyEfe configuration entity"""
 
@@ -320,15 +322,15 @@
 @attributes({"activity": AttrOf(Activity)})
 class EModelGenerationShape(Entity):
     """EModel generation."""
 
 
 @attributes(
     {
-        "used": AttrOf(list[Union[CoreTraceCollection, BluePyEfeConfiguration]]),
+        "used": AttrOf(List[Union[CoreTraceCollection, BluePyEfeConfiguration]]),
         "generated": AttrOf(BluePyEfeFeatures, default=None),
     }
 )
 class TraceFeatureExtraction(Activity):
     """Trace feature extraction activity.
 
     Args:
@@ -472,15 +474,15 @@
         )
 
         return _NexusBySparqlIterator(cls, query, **kwargs)
 
 
 @attributes(
     {
-        "hadMember": AttrOf(list[Report], default=None),
+        "hadMember": AttrOf(List[Report], default=None),
     }
 )
 class SimulationCampaignReportCollection(Entity):
     """Simulation campaign.
 
     Groups multiple simulations when same circuit is tested under different conditions.
 
@@ -530,28 +532,28 @@
     Args:
         distribution (DataDownload): Json representation of the configuration.
     """
 
 
 @attributes(
     {
-        "used": AttrOf(list[Identifiable], default=None),
+        "used": AttrOf(List[Identifiable], default=None),
     }
 )
 class Analysis(Activity):
     """Simulation analysis activity.
 
     Args:
         used (Identifiable): Used variable report/analysis configuration.
     """
 
 
 @attributes(
     {
-        "used": AttrOf(list[VariableReport], default=None),
+        "used": AttrOf(List[VariableReport], default=None),
         "generated": AttrOf(AnalysisReport, default=None),
         # 'wasInformedBy': AttrOf(SimulationCampaign, default=None),
     }
 )
 class CampaignAnalysis(Activity):
     """Simulation campaign analysis activity.
```

### Comparing `entity_management-1.2.46/entity_management/state.py` & `entity_management-1.3.0/entity_management/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """State of the interaction with nexus. For example current project to use.
 
 Nexus organization, project and access token are initialized from the corresponding
 environment variables. They can be updated using setter functions from this module.
 """
 
 import os
```

### Comparing `entity_management-1.2.46/entity_management/typecheck.py` & `entity_management-1.3.0/entity_management/typecheck.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,70 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """Type checking related utils."""
 
 import collections.abc
+import inspect
+import sys
 import types
 import typing
 
 
 def get_type_root_class(data_type):
     """Get type class. First try if it's `typing` type class then fallback to regular type."""
     root_type = typing.get_origin(data_type) or data_type
 
-    # Return types.UnionType instead of typing.Union because it works with issubclass
-    if root_type is typing.Union:
-        return types.UnionType
+    # types.UnionType for A | B is added in python3.10
+    if sys.version_info >= (3, 10) and root_type is types.UnionType:  # pylint: disable=no-member
+        return typing.Union
 
     return root_type
 
 
+def get_type_root_args(data_type):
+    """Return the type's args as type classes.
+
+    For example list | Dict returns (list, dict).
+    """
+    return tuple(get_type_root_class(arg) for arg in typing.get_args(data_type))
+
+
 def is_type_sequence(data_type):
     """Return True if the data_type is a sequence."""
-    return data_type is not str and issubclass(
+    return data_type is not str and _issubclass(
         get_type_root_class(data_type), collections.abc.Sequence
     )
 
 
+def _issubclass(x, y):
+    """Return True if x is a class that is a subclass of y."""
+    return inspect.isclass(x) and issubclass(x, y)
+
+
 def is_data_sequence(data_raw):
     """Return True if the data_raw is a sequence."""
     return not isinstance(data_raw, str) and isinstance(data_raw, collections.abc.Sequence)
 
 
 def is_type_mapping(data_type):
     """Return True if the data_type is a mapping."""
-    return issubclass(get_type_root_class(data_type), collections.abc.Mapping)
+    return _issubclass(get_type_root_class(data_type), collections.abc.Mapping)
 
 
 def is_data_mapping(data_raw):
     """Return True if the data_raw is a mapping."""
     return isinstance(data_raw, collections.abc.Mapping)
 
 
 def is_type_union(data_type):
     """Return True if the data_type is a union."""
-    return get_type_root_class(data_type) in {typing.Union, types.UnionType}
+    if sys.version_info.minor >= 10:
+        # pylint: disable=no-member
+        return get_type_root_class(data_type) in {typing.Union, types.UnionType}
+    return get_type_root_class(data_type) is typing.Union
 
 
 def is_type_single_or_list_union(data_type):
     """Return True for unions of the form T | list[T]"""
     type_args = typing.get_args(data_type)
 
     if len(type_args) != 2:
@@ -52,10 +72,10 @@
 
     arg1, arg2 = type_args
     # check that arg2 is a list generic e.g. list[int]
     # and that arg1 has the same type as arg2's element
     arg2_origin = typing.get_origin(arg2)
     return (
         arg2_origin is not None
-        and issubclass(arg2_origin, list)
+        and _issubclass(arg2_origin, list)
         and arg1 is typing.get_args(arg2)[0]
     )
```

### Comparing `entity_management-1.2.46/entity_management/util.py` & `entity_management-1.3.0/entity_management/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """Utilities"""
 
 import typing
+from typing import Optional
 from urllib.parse import parse_qs
 from urllib.parse import quote as parse_quote
 from urllib.parse import unquote, urlparse
 
 import attr
 from attr.validators import instance_of as instance_of_validator
 from attr.validators import optional as optional_validator
@@ -153,19 +156,22 @@
         # like typing.List[Distribution]
         list_element_type = _get_list_params(type_)[0]
         if typecheck.is_type_union(list_element_type):
             types = _get_union_params(list_element_type)
             validator = _list_of(types, default)
         else:
             validator = _list_of(list_element_type, default)
-
     # e.g. A | list[A]
     elif typecheck.is_type_single_or_list_union(type_):
         element_type = typing.get_args(type_)[0]
         validator = _one_or_list_of(element_type, default)
+    # e.g A | B
+    elif typecheck.is_type_union(type_):
+        types = _get_union_params(type_)
+        validator = instance_of(types)
     else:
         if default is None:  # default explicitly provided as None
             validator = optional_of(type_)
         else:  # default either not provided -> mandatory, or initialized with value
             validator = instance_of(type_)
 
     validators = [validator]
@@ -218,18 +224,18 @@
 
 def get_entity(
     resource_id: str,
     *,
     cls,
     cross_bucket: bool = True,
     resolve_context: bool = False,
-    base: str | None = None,
-    org: str | None = None,
-    proj: str | None = None,
-    token: str | None = None,
+    base: Optional[str] = None,
+    org: Optional[str] = None,
+    proj: Optional[str] = None,
+    token: Optional[str] = None,
 ):
     """Instantiate an entity from a resource id.
 
     Args:
         resource_id: The string id of the KG resource.
         cls: entity-management class to instantiate.
         cross_bucket: Whether to use the resolvers to get the resource. Default is True.
```

### Comparing `entity_management-1.2.46/entity_management/workflow.py` & `entity_management-1.3.0/entity_management/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-License-Identifier: Apache-2.0
+
 """Bbp-workflow entities."""
 
 from entity_management.base import Identifiable, _NexusBySparqlIterator, attributes
 from entity_management.core import Activity, Entity
 from entity_management.util import AttrOf
```

### Comparing `entity_management-1.2.46/entity_management.egg-info/PKG-INFO` & `entity_management-1.3.0/entity_management.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entity-management
-Version: 1.2.46
+Version: 1.3.0
 Summary: Access to production entity management
 Author: Blue Brain Project, EPFL
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -203,23 +203,24 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/BlueBrain/entity-management
-Project-URL: Repository, https://github.com/BlueBrain/NeuroM.git
-Project-URL: Tracker, https://github.com/BlueBrain/entity-management/issues
+Project-URL: Documentation, https://entity-management.readthedocs.io/en/stable/
+Project-URL: Repository, https://github.com/BlueBrain/entity-management
+Project-URL: Issues, https://github.com/BlueBrain/entity-management/issues
 Keywords: computational neuroscience,simulation,analysis,nexus,parameters,BlueBrainProject
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 Requires-Dist: requests
 Requires-Dist: attrs
 Requires-Dist: python-dateutil
 Requires-Dist: sparqlwrapper
@@ -232,14 +233,20 @@
 Requires-Dist: sphinx-bluebrain-theme; extra == "docs"
 
 entity-management
 =================
 
 Library for handling NEXUS entity dataclass definitions.
 
+Documentation
+=============
+
+* `latest release <https://entity-management.readthedocs.io/en/stable/>`_
+* `latest snapshot <https://entity-management.readthedocs.io/en/latest/>`_
+
 Installation
 ============
 
 entity-management can be pip installed with the following command:
 
 .. code-block:: bash
```

### Comparing `entity_management-1.2.46/entity_management.egg-info/SOURCES.txt` & `entity_management-1.3.0/entity_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/pyproject.toml` & `entity_management-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "entity-management"
 description = "Access to production entity management"
 readme = { file = "README.rst", content-type = "text/x-rst" }
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 license = { file = "LICENSE.txt" }
 authors = [
   { name = "Blue Brain Project, EPFL" },
 ]
 keywords = [
   "computational neuroscience",
   "simulation",
@@ -45,30 +45,35 @@
 [project.optional-dependencies]
 docs = [
   "sphinx-bluebrain-theme",
 ]
 
 [project.urls]
 Homepage = "https://github.com/BlueBrain/entity-management"
-Repository = "https://github.com/BlueBrain/NeuroM.git"
-Tracker = "https://github.com/BlueBrain/entity-management/issues"
+Documentation = "https://entity-management.readthedocs.io/en/stable/"
+Repository = "https://github.com/BlueBrain/entity-management"
+Issues = "https://github.com/BlueBrain/entity-management/issues"
 
 [project.scripts]
 entity-management = "entity_management.cli.base:cli"
 
 [tool.setuptools.packages.find]
 include = ["entity_management"]
 namespaces = false
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
 
 [tool.black]
 line-length = 100
 target-version = [
+    'py38',
+    'py39',
     'py310',
+    'py311',
+    'py312',
 ]
 include = 'entity_management\/.*\.py$|tests\/.*\.py$|doc\/source\/conf\.py$|setup\.py$'
 
 [tool.isort]
 profile = "black"
 line_length = 100
```

### Comparing `entity_management-1.2.46/tests/data/atlas_release_resp.json` & `entity_management-1.3.0/tests/data/atlas_release_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/cells_page1_resp.json` & `entity_management-1.3.0/tests/data/cells_page1_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/cells_page2_resp.json` & `entity_management-1.3.0/tests/data/cells_page2_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/detailed_circuit_resp.json` & `entity_management-1.3.0/tests/data/detailed_circuit_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/emodel_configuration_resp.json` & `entity_management-1.3.0/tests/data/emodel_configuration_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/emodel_data_catalog_resp.json` & `entity_management-1.3.0/tests/data/emodel_data_catalog_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/emodel_pipeline_settings_resp.json` & `entity_management-1.3.0/tests/data/emodel_pipeline_settings_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/emodel_release_resp.json` & `entity_management-1.3.0/tests/data/emodel_release_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/emodel_resp.json` & `entity_management-1.3.0/tests/data/emodel_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/emodel_script_resp.json` & `entity_management-1.3.0/tests/data/emodel_script_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/emodel_workflow_resp.json` & `entity_management-1.3.0/tests/data/emodel_workflow_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/entity_data_download_resp.json` & `entity_management-1.3.0/tests/data/entity_data_download_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/extraction_targets_configuration_resp.json` & `entity_management-1.3.0/tests/data/extraction_targets_configuration_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/file_link_resp.json` & `entity_management-1.3.0/tests/data/file_link_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/file_resp.json` & `entity_management-1.3.0/tests/data/file_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/fitness_calculator_configuration_resp.json` & `entity_management-1.3.0/tests/data/fitness_calculator_configuration_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/sub_cellular_model_script_resp.json` & `entity_management-1.3.0/tests/data/sub_cellular_model_script_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/trace_resp.json` & `entity_management-1.3.0/tests/data/trace_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/unconstrained_resp.json` & `entity_management-1.3.0/tests/data/unconstrained_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/data/workflow_resp.json` & `entity_management-1.3.0/tests/data/workflow_resp.json`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/test_atlas.py` & `entity_management-1.3.0/tests/test_atlas.py`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/test_base.py` & `entity_management-1.3.0/tests/test_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # pylint: disable=missing-docstring,no-member
 import io
+import sys
 import json
 from datetime import datetime
 from typing import List, Dict
 from dateutil.parser import parse
 from unittest.mock import patch
 
+from typing import Dict, List, Union
+
 import pytest
 
 import attr
 import requests
 from SPARQLWrapper import Wrapper
 
 from entity_management.settings import JSLD_ID, JSLD_REV, JSLD_TYPE, JSLD_LINK_REV
@@ -148,108 +151,167 @@
         "d": AttrOf(float),
     }
 )
 class BlankNode2(BlankNode):
     pass
 
 
+def _skip(*args, min_version):
+    return pytest.param(
+        *args,
+        marks=pytest.mark.skipif(
+            sys.version_info < min_version,
+            reason=f"Test requres {min_version} or higher.",
+        ),
+    )
+
+
+def _eval(string_or_type):
+    if isinstance(string_or_type, str):
+        return eval(string_or_type)
+    return string_or_type
+
+
 @pytest.mark.parametrize(
     "data_type, data_raw, expected",
     [
         (str, None, None),
         (list, [], None),
+        (List, [], None),
         (dict, {}, None),
+        (Dict, {}, None),
         (datetime, {"@value": "2024-01-22T10:07:16.052123Z"}, parse("2024-01-22T10:07:16.052123Z")),
         (dict, {"a": "b"}, {"a": "b"}),
         (Dict, {"a": "b"}, {"a": "b"}),
         (dict, [{"a": "b"}], {"a": "b"}),
         (Dict, [{"a": "b"}], {"a": "b"}),
         (list, [{"a": "b"}], [{"a": "b"}]),
         (List, [{"a": "b"}], [{"a": "b"}]),
-        (list[dict], [{"a": "b"}], [{"a": "b"}]),
-        (list[dict], [], None),
+        _skip("list[dict]", [{"a": "b"}], [{"a": "b"}], min_version=(3, 9)),
+        _skip("list[dict]", [], None, min_version=(3, 9)),
         (List[dict], [{"a": "b"}], [{"a": "b"}]),
-        (list[dict], {"a": "b"}, [{"a": "b"}]),
+        (List[Dict], [{"a": "b"}], [{"a": "b"}]),
+        _skip("list[Dict]", [{"a": "b"}], [{"a": "b"}], min_version=(3, 9)),
+        _skip("list[dict]", {"a": "b"}, [{"a": "b"}], min_version=(3, 9)),
         (List[str], "Ringo", ["Ringo"]),
-        (list[str], "Ringo", ["Ringo"]),
-        (list[str], [], None),
-        (list[str], ["a", "b"], ["a", "b"]),
+        _skip("list[str]", "Ringo", ["Ringo"], min_version=(3, 9)),
+        _skip("list[str]", [], None, min_version=(3, 9)),
+        _skip("list[str]", ["a", "b"], ["a", "b"], min_version=(3, 9)),
         (List[int], 2, [2]),
-        (list[int], 2, [2]),
+        _skip("list[int]", 2, [2], min_version=(3, 9)),
         (List[float], 2.0, [2.0]),
-        (list[float], 2.0, [2.0]),
+        _skip("list[float]", 2.0, [2.0], min_version=(3, 9)),
         (List[bool], True, [True]),
-        (list[bool], False, [False]),
+        _skip("list[bool]", False, [False], min_version=(3, 9)),
         (Dummy, {"a": 1, "b": 2}, Dummy(a=1, b=2)),
         (List[Dummy], [{"a": 1, "b": 2}], [Dummy(a=1, b=2)]),
-        (list[Dummy], [{"a": 1, "b": 2}], [Dummy(a=1, b=2)]),
-        (list[Dummy], [], None),
+        _skip("list[Dummy]", [{"a": 1, "b": 2}], [Dummy(a=1, b=2)], min_version=(3, 9)),
+        _skip("list[Dummy]", [], None, min_version=(3, 9)),
         (List[Dummy], {"a": 1, "b": 2}, [Dummy(a=1, b=2)]),
-        (list[Dummy], {"a": 1, "b": 2}, [Dummy(a=1, b=2)]),
-        (list[Dummy], [{"a": 1, "b": 2}, {"a": 2, "b": 3}], [Dummy(a=1, b=2), Dummy(a=2, b=3)]),
+        _skip("list[Dummy]", {"a": 1, "b": 2}, [Dummy(a=1, b=2)], min_version=(3, 9)),
+        _skip(
+            "list[Dummy]",
+            [{"a": 1, "b": 2}, {"a": 2, "b": 3}],
+            [Dummy(a=1, b=2), Dummy(a=2, b=3)],
+            min_version=(3, 9),
+        ),
         (FrozenDummy, {"a": 1, "b": "2"}, FrozenDummy(a=1, b="2")),
         (List[FrozenDummy], {"a": 1, "b": "2"}, [FrozenDummy(a=1, b="2")]),
-        (list[FrozenDummy], {"a": 1, "b": "2"}, [FrozenDummy(a=1, b="2")]),
-        (list[FrozenDummy], [], None),
-        (dict[str, str], {"foo": "bar"}, {"foo": "bar"}),
-        (dict[str, Dummy], {"foo": {"a": 1, "b": "2"}}, {"foo": Dummy(a=1, b="2")}),
-        (dict[str, FrozenDummy], {"foo": {"a": 1, "b": "2"}}, {"foo": FrozenDummy(a=1, b="2")}),
-        (dict[str, list[Dummy]], {"foo": {"a": 1, "b": "2"}}, {"foo": [Dummy(a=1, b="2")]}),
+        _skip(
+            "list[FrozenDummy]", {"a": 1, "b": "2"}, [FrozenDummy(a=1, b="2")], min_version=(3, 9)
+        ),
+        _skip("list[FrozenDummy]", [], None, min_version=(3, 9)),
+        _skip("dict[str, str]", {"foo": "bar"}, {"foo": "bar"}, min_version=(3, 9)),
+        _skip(
+            "dict[str, Dummy]",
+            {"foo": {"a": 1, "b": "2"}},
+            {"foo": Dummy(a=1, b="2")},
+            min_version=(3, 9),
+        ),
+        _skip(
+            "dict[str, FrozenDummy]",
+            {"foo": {"a": 1, "b": "2"}},
+            {"foo": FrozenDummy(a=1, b="2")},
+            min_version=(3, 9),
+        ),
+        _skip(
+            "dict[str, list[Dummy]]",
+            {"foo": {"a": 1, "b": "2"}},
+            {"foo": [Dummy(a=1, b="2")]},
+            min_version=(3, 9),
+        ),
         (
             OntologyTerm,
             {"@id": "foo", "label": "bar", "@type": "zee"},
             OntologyTerm(url="foo", label="bar"),
         ),
         (datetime, "2024-02-21T18:03:18.804172", datetime(2024, 2, 21, 18, 3, 18, 804172)),
         (datetime, {"@type": "xsd:date", "@value": "2024-02-14"}, datetime(2024, 2, 14, 0, 0)),
-        (int | float, 2, 2),
-        (int | float, 1.0, 1.0),
-        (int | dict, {"a": 1, "b": 2}, {"a": 1, "b": 2}),
-        (int | dict, 2, 2),
+        (Union[int, float], 2, 2),
+        _skip("int | float", 2, 2, min_version=(3, 10)),
+        (Union[int, float], 1.0, 1.0),
+        _skip("int | float", 1.0, 1.0, min_version=(3, 10)),
+        (Union[int, dict], {"a": 1, "b": 2}, {"a": 1, "b": 2}),
+        _skip("int | dict", {"a": 1, "b": 2}, {"a": 1, "b": 2}, min_version=(3, 10)),
+        (Union[int, dict], 2, 2),
+        _skip("int | dict", 2, 2, min_version=(3, 10)),
         (
-            BlankNode1 | BlankNode2,
+            Union[BlankNode1, BlankNode2],
             {"@type": "BlankNode1", "a": 2, "b": 3.0},
             BlankNode1(a=2, b=3.0),
         ),
+        _skip(
+            "BlankNode1 | BlankNode2",
+            {"@type": "BlankNode1", "a": 2, "b": 3.0},
+            BlankNode1(a=2, b=3.0),
+            min_version=(3, 10),
+        ),
         (
-            BlankNode1 | BlankNode2,
+            Union[BlankNode1, BlankNode2],
+            {"@type": "BlankNode2", "c": 2, "d": 3.0},
+            BlankNode2(c=2, d=3.0),
+        ),
+        _skip(
+            "BlankNode1 | BlankNode2",
             {"@type": "BlankNode2", "c": 2, "d": 3.0},
             BlankNode2(c=2, d=3.0),
+            min_version=(3, 10),
         ),
         (MaybeList[int], 1, 1),
         (MaybeList[int], [1, 2], [1, 2]),
         (MaybeList[Dummy], {"a": 1, "b": "2"}, Dummy(a=1, b="2")),
         (
             MaybeList[Dummy],
             [{"a": 1, "b": "2"}, {"a": 2, "b": "3"}],
             [Dummy(a=1, b="2"), Dummy(a=2, b="3")],
         ),
     ],
 )
 def test_deserialize_json_to_datatype(data_type, data_raw, expected):
-    assert _deserialize_json_to_datatype(data_type, data_raw) == expected
+    assert _deserialize_json_to_datatype(_eval(data_type), data_raw) == expected
 
 
 def _make_valid_resp(data):
-    essentials = {
+    res = {
         "@context": [
             "https://bluebrain.github.io/nexus/contexts/metadata.json",
             "https://bbp.neuroshapes.org",
         ],
         "_rev": 1,
         "_project": "my-project",
         "_self": "my-self",
         "_constrainedBy": "https://bluebrain.github.io/nexus/schemas/unconstrained.json",
         "_createdAt": "2024-01-22T10:07:16.052123Z",
         "_createdBy": "https://bbp.epfl.ch/nexus/v1/realms/bbp/users/zisis",
         "_deprecated": False,
         "_updatedAt": "2024-01-22T10:07:16.052123Z",
         "_updatedBy": "https://bbp.epfl.ch/nexus/v1/realms/bbp/users/zisis",
     }
-    return essentials | data
+    res.update(data)
+    return res
 
 
 def test_deserialize_json_to_datatype__union(monkeypatch):
 
     @attributes(
         {
             "a": AttrOf(int, default=42),
@@ -275,29 +337,29 @@
             "a": 1,
             "b": "2",
         }
     )
 
     monkeypatch.setattr(nexus, "load_by_id", lambda *args, **kwargs: data_raw_t1)
 
-    res = _deserialize_json_to_datatype(T1 | T2, data_raw_t1)
+    res = _deserialize_json_to_datatype(Union[T1, T2], data_raw_t1)
     assert res == T1(a=1, b="2")
 
     data_raw_t2 = _make_valid_resp(
         {
             "@id": "t2-id",
             "@type": "T2",
             "c": 1,
             "d": "2",
         }
     )
 
     monkeypatch.setattr(nexus, "load_by_id", lambda *args, **kwargs: data_raw_t2)
 
-    res = _deserialize_json_to_datatype(T1 | T2, data_raw_t2)
+    res = _deserialize_json_to_datatype(Union[T1, T2], data_raw_t2)
     assert res == T2(c=1, d="2")
 
 
 def test_deserialize_json_to_datatype__list_union(monkeypatch):
 
     @attributes(
         {
@@ -347,15 +409,15 @@
         if resource_id == "t1-id?rev=1":
             return data_raw_t1
         if resource_id == "t3-id?rev=1":
             return data_raw_t3
         raise
 
     monkeypatch.setattr(nexus, "load_by_id", mock_load_by_id)
-    res = _deserialize_json_to_datatype(list[T1 | T2 | T3], [data_raw_t3, data_raw_t1])
+    res = _deserialize_json_to_datatype(List[Union[T1, T2, T3]], [data_raw_t3, data_raw_t1])
     assert res == [T3(e=4, f="5"), T1(a=2, b="3")]
 
 
 @pytest.fixture(name="unconstrained_resp", scope="session")
 def fixture_unconstrained():
     with open("tests/data/unconstrained_resp.json") as f:
         return json.load(f)
```

### Comparing `entity_management-1.2.46/tests/test_context.py` & `entity_management-1.3.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/test_core.py` & `entity_management-1.3.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/test_emodel.py` & `entity_management-1.3.0/tests/test_emodel.py`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/test_model_building_config.py` & `entity_management-1.3.0/tests/test_model_building_config.py`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/test_morphology.py` & `entity_management-1.3.0/tests/test_morphology.py`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/test_nexus.py` & `entity_management-1.3.0/tests/test_nexus.py`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/test_simulation.py` & `entity_management-1.3.0/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tests/test_state.py` & `entity_management-1.3.0/tests/test_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 from unittest.mock import patch
 from entity_management import state as test_module
 
 
 def test_refresh_token__no_offline_token():
     """Test that refreshing is not attempted if no OFFLINE_TOKEN"""
-    with (
-        patch("entity_management.state.ACCESS_TOKEN", "my-token"),
-        patch("entity_management.state.OFFLINE_TOKEN", None),
-    ):
-        token = test_module.refresh_token()
-        assert token == "my-token"
+    with patch("entity_management.state.ACCESS_TOKEN", "my-token"):
+        with patch("entity_management.state.OFFLINE_TOKEN", None):
+            token = test_module.refresh_token()
+            assert token == "my-token"
 
 
 def test_get_base_resolvers():
     res = test_module.get_base_resolvers(base="my-base")
     assert res == "my-base/resolvers"
 
 
 def test_get_base_resolvers__None():
     with patch("entity_management.state.BASE", "my-base"):
         res = test_module.get_base_resolvers()
         assert res == "my-base/resolvers"
 
 
 def test_base_url__cross_bucket():
-    with (
-        patch("entity_management.state.BASE", "my-base"),
-        patch("entity_management.state.PROJ", "my-proj"),
-        patch("entity_management.state.ORG", "my-org"),
-    ):
-        res = test_module.get_base_url()
-        assert res == "my-base/resources/my-org/my-proj/_"
+    with patch("entity_management.state.BASE", "my-base"):
+        with patch("entity_management.state.PROJ", "my-proj"):
+            with patch("entity_management.state.ORG", "my-org"):
+                res = test_module.get_base_url()
+                assert res == "my-base/resources/my-org/my-proj/_"
 
-        res = test_module.get_base_url(cross_bucket=True)
-        assert res == "my-base/resolvers/my-org/my-proj/_"
+                res = test_module.get_base_url(cross_bucket=True)
+                assert res == "my-base/resolvers/my-org/my-proj/_"
```

### Comparing `entity_management-1.2.46/tests/util.py` & `entity_management-1.3.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `entity_management-1.2.46/tox.ini` & `entity_management-1.3.0/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 testdeps =
     pytest
     responses
     certifi
 
 [tox]
 envlist =
-    check-packaging
     lint
-    py3
+    coverage
+    check-packaging
+    py{38,39,310,311,312}
 
 [testenv]
 deps = {[base]testdeps}
 commands = pytest tests {posargs}
 
 [testenv:check-packaging]
 skip_install = true
@@ -44,15 +45,14 @@
 [testenv:format]
 deps =
     pyupgrade
     autoflake
     isort
     black
 commands =
-    find {[base]name} -type f -name '*.py' -exec pyupgrade --py310-plus {} ;
     autoflake -ir --remove-all-unused-imports --ignore-init-module-imports {[base]name}
     isort {[base]name}
     black .
 allowlist_externals=find
 
 [testenv:coverage]
 deps =
@@ -71,7 +71,15 @@
 
 # E731: do not assign a lambda expression, use a def
 # W503: line break after binary operator
 # W504: line break before binary operator
 [pycodestyle]
 ignore = E731,W503,W504
 max-line-length = 100
+
+[gh-actions]
+python =
+    3.8: py38, lint
+    3.9: py39
+    3.10: py310, docs, check-packaging
+    3.11: py311, coverage
+    3.12: py312, check-packaging
```

