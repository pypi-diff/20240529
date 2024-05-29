# Comparing `tmp/neomodel-5.2.1.tar.gz` & `tmp/neomodel-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neomodel-5.2.1.tar", last modified: Mon Dec 11 16:07:36 2023, max compression
+gzip compressed data, was "neomodel-5.3.0.tar", last modified: Mon Apr 22 10:22:40 2024, max compression
```

## Comparing `neomodel-5.2.1.tar` & `neomodel-5.3.0.tar`

### file list

```diff
@@ -1,84 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:36.646540 neomodel-5.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-12-11 16:07:24.000000 neomodel-5.2.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-11 16:07:24.000000 neomodel-5.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2023-12-11 16:07:36.646540 neomodel-5.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2023-12-11 16:07:24.000000 neomodel-5.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:36.630540 neomodel-5.2.1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:36.630540 neomodel-5.2.1/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:36.630540 neomodel-5.2.1/doc/source/_themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:36.630540 neomodel-5.2.1/doc/source/_themes/alabaster/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-11 16:07:24.000000 neomodel-5.2.1/doc/source/_themes/alabaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-11 16:07:24.000000 neomodel-5.2.1/doc/source/_themes/alabaster/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2023-12-11 16:07:24.000000 neomodel-5.2.1/doc/source/_themes/alabaster/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2023-12-11 16:07:24.000000 neomodel-5.2.1/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:36.634540 neomodel-5.2.1/neomodel/
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/cardinality.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:36.634540 neomodel-5.2.1/neomodel/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/contrib/semi_structured.py
--rw-r--r--   0 runner    (1001) docker     (127)    26472 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/contrib/spatial_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    26675 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:36.634540 neomodel-5.2.1/neomodel/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/integration/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/integration/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    36213 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/match.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/match_q.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    18579 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)    17478 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/relationship_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:36.638540 neomodel-5.2.1/neomodel/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15048 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/scripts/neomodel_inspect_database.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3559 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/scripts/neomodel_install_labels.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2139 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/scripts/neomodel_remove_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    23378 2023-12-11 16:07:24.000000 neomodel-5.2.1/neomodel/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:36.642540 neomodel-5.2.1/neomodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2023-12-11 16:07:36.000000 neomodel-5.2.1/neomodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-12-11 16:07:36.000000 neomodel-5.2.1/neomodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 16:07:36.000000 neomodel-5.2.1/neomodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-12-11 16:07:36.000000 neomodel-5.2.1/neomodel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-12-11 16:07:36.000000 neomodel-5.2.1/neomodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 16:07:36.000000 neomodel-5.2.1/neomodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2023-12-11 16:07:24.000000 neomodel-5.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 16:07:36.646540 neomodel-5.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:36.642540 neomodel-5.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_cardinality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:36.642540 neomodel-5.2.1/test/test_contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_contrib/test_semi_structured.py
--rw-r--r--   0 runner    (1001) docker     (127)    14354 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_contrib/test_spatial_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9702 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_contrib/test_spatial_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_cypher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_database_management.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_dbms_awareness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_driver_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_issue112.py
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_issue283.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_issue600.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_label_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_label_install.py
--rw-r--r--   0 runner    (1001) docker     (127)    15666 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_match_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_migration_neo4j_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     9181 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    12251 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_relationship_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_relative_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2023-12-11 16:07:24.000000 neomodel-5.2.1/test/test_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.479402 neomodel-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-22 10:22:36.000000 neomodel-5.3.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-22 10:22:36.000000 neomodel-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-22 10:22:40.479402 neomodel-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-22 10:22:36.000000 neomodel-5.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.455402 neomodel-5.3.0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.459402 neomodel-5.3.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.455402 neomodel-5.3.0/doc/source/_themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.459402 neomodel-5.3.0/doc/source/_themes/alabaster/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-22 10:22:36.000000 neomodel-5.3.0/doc/source/_themes/alabaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 10:22:36.000000 neomodel-5.3.0/doc/source/_themes/alabaster/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-22 10:22:36.000000 neomodel-5.3.0/doc/source/_themes/alabaster/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-04-22 10:22:36.000000 neomodel-5.3.0/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.463402 neomodel-5.3.0/neomodel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.463402 neomodel-5.3.0/neomodel/_async_compat/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/_async_compat/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.463402 neomodel-5.3.0/neomodel/async_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/async_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/async_/cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54084 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/async_/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39676 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/async_/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/async_/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/async_/property_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/async_/relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18570 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/async_/relationship_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.463402 neomodel-5.3.0/neomodel/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.463402 neomodel-5.3.0/neomodel/contrib/async_/
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/contrib/async_/semi_structured.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27130 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/contrib/spatial_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.467402 neomodel-5.3.0/neomodel/contrib/sync_/
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/contrib/sync_/semi_structured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.467402 neomodel-5.3.0/neomodel/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/integration/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/integration/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7800 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/match_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15237 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.467402 neomodel-5.3.0/neomodel/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15111 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/scripts/neomodel_inspect_database.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3612 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/scripts/neomodel_install_labels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2193 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/scripts/neomodel_remove_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.467402 neomodel-5.3.0/neomodel/sync_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/sync_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/sync_/cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53004 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/sync_/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39194 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/sync_/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/sync_/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/sync_/property_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/sync_/relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/sync_/relationship_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-22 10:22:36.000000 neomodel-5.3.0/neomodel/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.479402 neomodel-5.3.0/neomodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-22 10:22:40.000000 neomodel-5.3.0/neomodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-22 10:22:40.000000 neomodel-5.3.0/neomodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 10:22:40.000000 neomodel-5.3.0/neomodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-22 10:22:40.000000 neomodel-5.3.0/neomodel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 10:22:40.000000 neomodel-5.3.0/neomodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-22 10:22:40.000000 neomodel-5.3.0/neomodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-22 10:22:36.000000 neomodel-5.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 10:22:40.479402 neomodel-5.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.467402 neomodel-5.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.467402 neomodel-5.3.0/test/_async_compat/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/_async_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/_async_compat/mark_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.471403 neomodel-5.3.0/test/async_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.475402 neomodel-5.3.0/test/async_/test_contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_contrib/test_semi_structured.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14354 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_contrib/test_spatial_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_contrib/test_spatial_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_cypher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_database_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_dbms_awareness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_driver_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_issue112.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15606 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_issue283.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_issue600.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_label_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_label_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19353 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_match_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_migration_neo4j_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_relationship_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_relative_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/async_/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.479402 neomodel-5.3.0/test/sync_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:40.479402 neomodel-5.3.0/test/sync_/test_contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_contrib/test_semi_structured.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14354 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_contrib/test_spatial_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_contrib/test_spatial_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_cypher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_database_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_dbms_awareness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_driver_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_issue112.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14582 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_issue283.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_issue600.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_label_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_label_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18023 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_match_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_migration_neo4j_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_relationship_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_relative_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/sync_/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-04-22 10:22:36.000000 neomodel-5.3.0/test/test_scripts.py
```

### Comparing `neomodel-5.2.1/AUTHORS.txt` & `neomodel-5.3.0/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `neomodel-5.2.1/LICENSE` & `neomodel-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neomodel-5.2.1/PKG-INFO` & `neomodel-5.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,7 @@
-Metadata-Version: 2.1
-Name: neomodel
-Version: 5.2.1
-Summary: An object mapper for the neo4j graph database.
-Author-email: Robin Edwards <robin.ge@gmail.com>
-Maintainer: Cristina Escalante
-Maintainer-email: Marius Conjeaud <marius.conjeaud@outlook.com>, Athanasios Anastasiou <athanastasiou@gmail.com>
-License: MIT
-Project-URL: documentation, https://neomodel.readthedocs.io/en/latest/
-Project-URL: repository, http://github.com/neo4j-contrib/neomodel
-Project-URL: changelog, https://github.com/neo4j-contrib/neomodel/releases
-Keywords: graph,neo4j,ORM,OGM,mapper
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Database
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.txt
-Requires-Dist: neo4j~=5.15.0
-Provides-Extra: dev
-Requires-Dist: pytest>=7.1; extra == "dev"
-Requires-Dist: pytest-cov>=4.0; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: Shapely>=2.0.0; extra == "dev"
-Provides-Extra: pandas
-Requires-Dist: pandas; extra == "pandas"
-Provides-Extra: numpy
-Requires-Dist: numpy; extra == "numpy"
-
 ![neomodel](https://raw.githubusercontent.com/neo4j-contrib/neomodel/master/doc/source/_static/neomodel-300.png)
 
 An Object Graph Mapper (OGM) for the [neo4j](https://neo4j.com/) graph
 database, built on the awesome
 [neo4j_driver](https://github.com/neo4j/neo4j-python-driver)
 
 If you need assistance with neomodel, please create an issue on the
@@ -67,32 +30,29 @@
 **For neomodel releases 4.x :**
 
 -   Python 3.7 -\> 3.10
 -   Neo4j 4.x (including 4.4 LTS for neomodel version 4.0.10)
 
 # Documentation
 
-(Needs an update, but) Available on
+Available on
 [readthedocs](http://neomodel.readthedocs.org).
 
-# Upcoming breaking changes notice - \>=5.3
+# New in 5.3.0
+
+neomodel now supports asynchronous programming, thanks to the [Neo4j driver async API](https://neo4j.com/docs/api/python-driver/current/async_api.html). The [documentation](http://neomodel.readthedocs.org) has been updated accordingly, with an updated getting started section, and some specific documentation for the async API.
 
-Based on Python version [status](https://devguide.python.org/versions/),
-neomodel will be dropping support for Python 3.7 in the next release
-(5.3). This does not mean neomodel will stop working on Python 3.7, but
-it will no longer be tested against it. Instead, we will try to add
-support for Python 3.12.
-
-Another potential breaking change coming up is adding async support to
-neomodel. But we do not know when this will happen yet, or if it will
-actually be a breaking change. We will definitely push this in a major
-release though. More to come on that later.
+# Breaking change in 5.3.0
 
-Finally, we are looking at refactoring some standalone methods into the
-Database() class. More to come on that later.
+- config.AUTO_INSTALL_LABELS has been removed. Please use the `neomodel_install_labels` script instead. _Note : this is because of the addition of async, but also because it might lead to uncontrolled creation of indexes/constraints. The script makes you more in control of said creation._
+- Based on Python version [status](https://devguide.python.org/versions/),
+neomodel will be dropping support for Python 3.7 in an upcoming release
+(5.3 or later). _This does not mean neomodel will stop working on Python 3.7, but
+it will no longer be tested against it_
+- Some standalone methods have been refactored into the Database() class. Check the [documentation](http://neomodel.readthedocs.org) for a full list.
 
 # Installation
 
 Install from pypi (recommended):
 
     $ pip install neomodel ($ source dev # To install all things needed in a Python3 venv)
 
@@ -100,14 +60,23 @@
 
     $ pip install neomodel['extras']
 
 To install from github:
 
     $ pip install git+git://github.com/neo4j-contrib/neomodel.git@HEAD#egg=neomodel-dev
 
+# Performance comparison
+
+You can find some performance tests made using Locust [in this repo](https://github.com/mariusconjeaud/neomodel-locust).
+
+Two learnings from this :
+
+* The wrapping of the driver made by neomodel is very thin performance-wise : it does not add a lot of overhead ;
+* When used in a concurrent fashion, async neomodel is faster than concurrent sync neomodel, and a lot of faster than serial queries.
+
 # Contributing
 
 Ideas, bugs, tests and pull requests always welcome. Please use
 GitHub\'s Issues page to track these.
 
 If you are interested in developing `neomodel` further, pick a subject
 from the Issues page and open a Pull Request (PR) for it. If you are
@@ -145,7 +114,46 @@
 `debug.db` database.
 
 If you have `docker-compose` installed, you can run the test suite
 against all supported Python interpreters and neo4j versions: :
 
     # in the project's root folder:
     $ sh ./tests-with-docker-compose.sh
+
+## Developing with async
+
+### Transpiling async -> sync
+
+We use [this great library](https://github.com/python-trio/unasync) to automatically transpile async code into its sync version.
+
+In other words, when contributing to neomodel, only update the `async` code in `neomodel/async_`, then run : :
+
+    bin/make-unasync
+    isort .
+    black .
+
+Note that you can also use the pre-commit hooks for this.
+
+### Specific async/sync code
+This transpiling script mainly does two things :
+
+- It removes the await keywords, and the Async prefixes in class names
+- It does some specific replacements, like `adb`->`db`, `mark_async_test`->`mark_sync_test`
+
+It might be that your code should only be run for `async`, or `sync` ; or you want different stubs to be run for `async` vs `sync`.
+You can use the following utility function for this - taken from the official [Neo4j python driver code](https://github.com/neo4j/neo4j-python-driver) :
+
+    # neomodel/async_/core.py
+    from neomodel._async_compat.util import AsyncUtil
+
+    # AsyncUtil.is_async_code is always True
+    if AsyncUtil.is_async_code:
+        # Specific async code
+        # This one gets run when in async mode
+        assert await Coffee.nodes.check_contains(2)
+    else:
+        # Specific sync code
+        # This one gest run when in sync mode
+        assert 2 in Coffee.nodes
+
+You can check [test_match_api](test/async_/test_match_api.py) for some good examples, and how it's transpiled into sync.
+
```

### Comparing `neomodel-5.2.1/doc/source/_themes/alabaster/support.py` & `neomodel-5.3.0/doc/source/_themes/alabaster/support.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.2.1/doc/source/conf.py` & `neomodel-5.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.2.1/neomodel/__init__.py` & `neomodel-5.3.0/neomodel/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # pep8: noqa
-
+from neomodel.async_.cardinality import (
+    AsyncOne,
+    AsyncOneOrMore,
+    AsyncZeroOrMore,
+    AsyncZeroOrOne,
+)
+from neomodel.async_.core import AsyncStructuredNode, adb
+from neomodel.async_.match import AsyncNodeSet, AsyncTraversal
+from neomodel.async_.path import AsyncNeomodelPath
+from neomodel.async_.property_manager import AsyncPropertyManager
+from neomodel.async_.relationship import AsyncStructuredRel
+from neomodel.async_.relationship_manager import (
+    AsyncRelationship,
+    AsyncRelationshipDefinition,
+    AsyncRelationshipFrom,
+    AsyncRelationshipManager,
+    AsyncRelationshipTo,
+)
 from neomodel.exceptions import *
-from neomodel.match import EITHER, INCOMING, OUTGOING, NodeSet, Traversal
 from neomodel.match_q import Q  # noqa
-from neomodel.relationship_manager import (
-    NotConnected,
-    Relationship,
-    RelationshipDefinition,
-    RelationshipFrom,
-    RelationshipManager,
-    RelationshipTo,
-)
-
-from .cardinality import One, OneOrMore, ZeroOrMore, ZeroOrOne
-from .core import *
-from .properties import (
+from neomodel.properties import (
     AliasProperty,
     ArrayProperty,
     BooleanProperty,
     DateProperty,
     DateTimeFormatProperty,
     DateTimeProperty,
     EmailProperty,
@@ -26,15 +31,36 @@
     IntegerProperty,
     JSONProperty,
     NormalizedProperty,
     RegexProperty,
     StringProperty,
     UniqueIdProperty,
 )
-from .relationship import StructuredRel
-from .util import change_neo4j_password, clear_neo4j_database
-from .path import NeomodelPath
+from neomodel.sync_.cardinality import One, OneOrMore, ZeroOrMore, ZeroOrOne
+from neomodel.sync_.core import (
+    StructuredNode,
+    change_neo4j_password,
+    clear_neo4j_database,
+    db,
+    drop_constraints,
+    drop_indexes,
+    install_all_labels,
+    install_labels,
+    remove_all_labels,
+)
+from neomodel.sync_.match import NodeSet, Traversal
+from neomodel.sync_.path import NeomodelPath
+from neomodel.sync_.property_manager import PropertyManager
+from neomodel.sync_.relationship import StructuredRel
+from neomodel.sync_.relationship_manager import (
+    Relationship,
+    RelationshipDefinition,
+    RelationshipFrom,
+    RelationshipManager,
+    RelationshipTo,
+)
+from neomodel.util import EITHER, INCOMING, OUTGOING
 
 __author__ = "Robin Edwards"
 __email__ = "robin.ge@gmail.com"
 __license__ = "MIT"
 __package__ = "neomodel"
```

### Comparing `neomodel-5.2.1/neomodel/cardinality.py` & `neomodel-5.3.0/neomodel/sync_/cardinality.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from neomodel.exceptions import AttemptedCardinalityViolation, CardinalityViolation
-from neomodel.relationship_manager import (  # pylint:disable=unused-import
+from neomodel.sync_.relationship_manager import (  # pylint:disable=unused-import
     RelationshipManager,
     ZeroOrMore,
 )
 
 
 class ZeroOrOne(RelationshipManager):
     """A relationship to zero or one node."""
@@ -33,15 +33,15 @@
 
         :param node:
         :type: StructuredNode
         :param properties: relationship properties
         :type: dict
         :return: True / rel instance
         """
-        if len(self):
+        if super().__len__():
             raise AttemptedCardinalityViolation(
                 f"Node already has {self} can't connect more"
             )
         return super().connect(node, properties)
 
 
 class OneOrMore(RelationshipManager):
@@ -126,10 +126,10 @@
 
         :param node:
         :param properties: relationship properties
         :return: True / rel instance
         """
         if not hasattr(self.source, "element_id") or self.source.element_id is None:
             raise ValueError("Node has not been saved cannot connect!")
-        if len(self):
+        if super().__len__():
             raise AttemptedCardinalityViolation("Node already has one relationship")
         return super().connect(node, properties)
```

### Comparing `neomodel-5.2.1/neomodel/config.py` & `neomodel-5.3.0/neomodel/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import neo4j
 
-from ._version import __version__
-
-AUTO_INSTALL_LABELS = False
+from neomodel._version import __version__
 
 # Use this to connect with automatically created driver
 # The following options are the default ones that will be used as driver config
 DATABASE_URL = "bolt://neo4j:foobarbaz@localhost:7687"
 FORCE_TIMEZONE = False
 
 CONNECTION_ACQUISITION_TIMEOUT = 60.0
@@ -20,7 +18,10 @@
 TRUSTED_CERTIFICATES = neo4j.TrustSystemCAs()
 USER_AGENT = f"neomodel/v{__version__}"
 
 # Use this to connect with your self-managed driver instead
 # DRIVER = neo4j.GraphDatabase().driver(
 #     "bolt://localhost:7687", auth=("neo4j", "foobarbaz")
 # )
+DRIVER = None
+# Use this to connect to a specific database when using the self-managed driver
+DATABASE_NAME = None
```

### Comparing `neomodel-5.2.1/neomodel/contrib/spatial_properties.py` & `neomodel-5.3.0/neomodel/contrib/spatial_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 __author__ = "Athanasios Anastasiou"
 
 import neo4j.spatial
 
 # If shapely is not installed, its import will fail and the spatial properties will not be available
 try:
-    from shapely.geometry import Point as ShapelyPoint
     from shapely import __version__ as shapely_version
-    from shapely.coords import CoordinateSequence 
+    from shapely.coords import CoordinateSequence
+    from shapely.geometry import Point as ShapelyPoint
 except ImportError as exc:
     raise ImportError(
         "NEOMODEL ERROR: Shapely not found. If required, you can install Shapely via "
         "`pip install shapely`."
     ) from exc
 
 from neomodel.properties import Property, validator
@@ -49,32 +49,33 @@
     9157: "cartesian-3d",
     4326: "wgs-84",
     4979: "wgs-84-3d",
 }
 
 # Taking into account the Shapely 2.0.0 changes in the way POINT objects are initialisd.
 if int("".join(shapely_version.split(".")[0:3])) < 200:
+
     class NeomodelPoint(ShapelyPoint):
         """
         Abstracts the Point spatial data type of Neo4j.
-    
+
         Note:
         At the time of writing, Neo4j supports 2 main variants of Point:
             1. A generic point defined over a Cartesian plane
                 * The minimum data to define a point is x, y [,z] when crs is either "cartesian" or "cartesian-3d"
             2. A generic point defined over the WGS84 ellipsoid
                 * The minimum data to define a point is longitude, latitude [,Height] and the crs is then assumed
                   to be "wgs-84".
         """
-    
+
         # def __init__(self, *args, crs=None, x=None, y=None, z=None, latitude=None, longitude=None, height=None, **kwargs):
         def __init__(self, *args, **kwargs):
             """
             Creates a NeomodelPoint.
-    
+
             :param args: Positional arguments to emulate the behaviour of Shapely's Point (and specifically the copy
             constructor)
             :type args: list
             :param crs: Coordinate Reference System, must be one of ['cartesian', 'cartesian-3d', 'wgs-84', 'wgs-84-3d']
             :type crs: str
             :param x: x coordinate of point
             :type x: float
@@ -87,39 +88,43 @@
             :param longitude: Longitude of point
             :type longitude: float
             :param height: Height of point if the crs is wgs-84-3d
             :type height: float
             :param kwargs: Dictionary of keyword arguments
             :type kwargs: dict
             """
-    
+
             # Python2.7 Workaround for the order that the arguments get passed to the functions
             crs = kwargs.pop("crs", None)
             x = kwargs.pop("x", None)
             y = kwargs.pop("y", None)
             z = kwargs.pop("z", None)
             longitude = kwargs.pop("longitude", None)
             latitude = kwargs.pop("latitude", None)
             height = kwargs.pop("height", None)
-    
+
             _x, _y, _z = None, None, None
-    
+
             # CRS validity check is common to both types of constructors that follow
             if crs is not None and crs not in ACCEPTABLE_CRS:
-                raise ValueError(f"Invalid CRS({crs}). Expected one of {','.join(ACCEPTABLE_CRS)}")
+                raise ValueError(
+                    f"Invalid CRS({crs}). Expected one of {','.join(ACCEPTABLE_CRS)}"
+                )
             self._crs = crs
-    
+
             # If positional arguments have been supplied, then this is a possible call to the copy constructor or
             # initialisation by a coordinate iterable as per ShapelyPoint constructor.
             if len(args) > 0:
                 # If a coordinate iterable was passed, emulate a call with x,y[,z] parameters
                 if isinstance(args[0], (tuple, list)):
                     # Check dimensionality of tuple
                     if len(args[0]) < 2 or len(args[0]) > 3:
-                        raise ValueError(f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0])}")
+                        raise ValueError(
+                            f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0])}"
+                        )
                     x = args[0][0]
                     y = args[0][1]
                     if len(args[0]) == 3:
                         z = args[0][2]
                 # If another "Point" was passed, then this is a call to the copy constructor
                 elif isinstance(args[0], ShapelyPoint):
                     super().__init__(args[0])
@@ -139,151 +144,160 @@
                         if len(args[0].coords[0]) == 2:
                             if crs is None:
                                 self._crs = "cartesian"
                         elif len(args[0].coords[0]) == 3:
                             if crs is None:
                                 self._crs = "cartesian-3d"
                         else:
-                            raise ValueError(f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0].coords[0])}")
+                            raise ValueError(
+                                f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0].coords[0])}"
+                            )
                     return
                 else:
-                    raise TypeError(f"Invalid object passed to copy constructor. Expected NeomodelPoint or shapely Point, received {type(args[0])}")
-    
+                    raise TypeError(
+                        f"Invalid object passed to copy constructor. Expected NeomodelPoint or shapely Point, received {type(args[0])}"
+                    )
+
             # Initialisation is either via x,y[,z] XOR longitude,latitude[,height]. Specifying both leads to an error.
             if any(i is not None for i in [x, y, z]) and any(
                 i is not None for i in [latitude, longitude, height]
             ):
                 raise ValueError(
                     "Invalid instantiation via arguments. "
                     "A Point can be defined either by x,y,z coordinates OR latitude,longitude,height but not "
                     "a combination of these terms"
                 )
-    
+
             # Specifying no initialisation argument at this point in the constructor is flagged as an error
             if all(i is None for i in [x, y, z, latitude, longitude, height]):
                 raise ValueError(
                     "Invalid instantiation via no arguments. "
                     "A Point needs default values either in x,y,z or longitude, latitude, height coordinates"
                 )
-    
+
             # Geographical Point Initialisation
             if latitude is not None and longitude is not None:
                 if height is not None:
                     if self._crs is None:
                         self._crs = "wgs-84-3d"
                     _z = height
                 else:
                     if self._crs is None:
                         self._crs = "wgs-84"
                 _x = longitude
                 _y = latitude
-    
+
             # Geometrical Point Initialisation
             if x is not None and y is not None:
                 if z is not None:
                     if self._crs is None:
                         self._crs = "cartesian-3d"
                     _z = z
                 else:
                     if self._crs is None:
                         self._crs = "cartesian"
                 _x = x
                 _y = y
-    
+
             if _z is None:
                 if "-3d" not in self._crs:
                     super().__init__((float(_x), float(_y)), **kwargs)
                 else:
-                    raise ValueError(f"Invalid vector dimensions(2) for given CRS({self._crs}).")
+                    raise ValueError(
+                        f"Invalid vector dimensions(2) for given CRS({self._crs})."
+                    )
             else:
                 if "-3d" in self._crs:
                     super().__init__((float(_x), float(_y), float(_z)), **kwargs)
                 else:
-                    raise ValueError(f"Invalid vector dimensions(3) for given CRS({self._crs}).")
-    
+                    raise ValueError(
+                        f"Invalid vector dimensions(3) for given CRS({self._crs})."
+                    )
+
         @property
         def crs(self):
             return self._crs
-    
+
         @property
         def x(self):
             if not self._crs.startswith("cartesian"):
                 raise AttributeError(
                     f'Invalid coordinate ("x") for points defined over {self.crs}'
                 )
             return super().x
-    
+
         @property
         def y(self):
             if not self._crs.startswith("cartesian"):
                 raise AttributeError(
                     f'Invalid coordinate ("y") for points defined over {self.crs}'
                 )
             return super().y
-    
+
         @property
         def z(self):
             if self._crs != "cartesian-3d":
                 raise AttributeError(
                     f'Invalid coordinate ("z") for points defined over {self.crs}'
                 )
             return super().z
-    
+
         @property
         def latitude(self):
             if not self._crs.startswith("wgs-84"):
                 raise AttributeError(
                     f'Invalid coordinate ("latitude") for points defined over {self.crs}'
                 )
             return super().y
-    
+
         @property
         def longitude(self):
             if not self._crs.startswith("wgs-84"):
                 raise AttributeError(
                     f'Invalid coordinate ("longitude") for points defined over {self.crs}'
                 )
             return super().x
-    
+
         @property
         def height(self):
             if self._crs != "wgs-84-3d":
                 raise AttributeError(
                     f'Invalid coordinate ("height") for points defined over {self.crs}'
                 )
             return super().z
-    
+
         # The following operations are necessary here due to the way queries (and more importantly their parameters) get
         # combined and evaluated in neomodel. Specifically, query expressions get duplicated with deep copies and any valid
         # datatype values should also implement these operations.
         def __copy__(self):
             return NeomodelPoint(self)
-    
+
         def __deepcopy__(self, memo):
             return NeomodelPoint(self)
 
 else:
+
     class NeomodelPoint:
         """
         Abstracts the Point spatial data type of Neo4j.
-    
+
         Note:
         At the time of writing, Neo4j supports 2 main variants of Point:
             1. A generic point defined over a Cartesian plane
                 * The minimum data to define a point is x, y [,z] when crs is either "cartesian" or "cartesian-3d"
             2. A generic point defined over the WGS84 ellipsoid
                 * The minimum data to define a point is longitude, latitude [,Height] and the crs is then assumed
                   to be "wgs-84".
         """
-    
+
         # def __init__(self, *args, crs=None, x=None, y=None, z=None, latitude=None, longitude=None, height=None, **kwargs):
         def __init__(self, *args, **kwargs):
             """
             Creates a NeomodelPoint.
-    
+
             :param args: Positional arguments to emulate the behaviour of Shapely's Point (and specifically the copy
             constructor)
             :type args: list
             :param crs: Coordinate Reference System, must be one of ['cartesian', 'cartesian-3d', 'wgs-84', 'wgs-84-3d']
             :type crs: str
             :param x: x coordinate of point
             :type x: float
@@ -296,39 +310,43 @@
             :param longitude: Longitude of point
             :type longitude: float
             :param height: Height of point if the crs is wgs-84-3d
             :type height: float
             :param kwargs: Dictionary of keyword arguments
             :type kwargs: dict
             """
-    
+
             # Python2.7 Workaround for the order that the arguments get passed to the functions
             crs = kwargs.pop("crs", None)
             x = kwargs.pop("x", None)
             y = kwargs.pop("y", None)
             z = kwargs.pop("z", None)
             longitude = kwargs.pop("longitude", None)
             latitude = kwargs.pop("latitude", None)
             height = kwargs.pop("height", None)
-    
+
             _x, _y, _z = None, None, None
-    
+
             # CRS validity check is common to both types of constructors that follow
             if crs is not None and crs not in ACCEPTABLE_CRS:
-                raise ValueError(f"Invalid CRS({crs}). Expected one of {','.join(ACCEPTABLE_CRS)}")
+                raise ValueError(
+                    f"Invalid CRS({crs}). Expected one of {','.join(ACCEPTABLE_CRS)}"
+                )
             self._crs = crs
-    
+
             # If positional arguments have been supplied, then this is a possible call to the copy constructor or
             # initialisation by a coordinate iterable as per ShapelyPoint constructor.
             if len(args) > 0:
                 # If a coordinate iterable was passed, emulate a call with x,y[,z] parameters
                 if isinstance(args[0], (tuple, list)):
                     # Check dimensionality of tuple
                     if len(args[0]) < 2 or len(args[0]) > 3:
-                        raise ValueError(f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0])}")
+                        raise ValueError(
+                            f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0])}"
+                        )
                     x = args[0][0]
                     y = args[0][1]
                     if len(args[0]) == 3:
                         z = args[0][2]
                 # If another "Point" was passed, then this is a call to the copy constructor
                 elif isinstance(args[0], (ShapelyPoint, NeomodelPoint)):
                     if isinstance(args[0], ShapelyPoint):
@@ -350,145 +368,156 @@
                         if len(args[0].coords[0]) == 2:
                             if crs is None:
                                 self._crs = "cartesian"
                         elif len(args[0].coords[0]) == 3:
                             if crs is None:
                                 self._crs = "cartesian-3d"
                         else:
-                            raise ValueError(f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0].coords[0])}")
+                            raise ValueError(
+                                f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0].coords[0])}"
+                            )
                     return
                 else:
-                    raise TypeError(f"Invalid object passed to copy constructor. Expected NeomodelPoint or shapely Point, received {type(args[0])}")
-    
+                    raise TypeError(
+                        f"Invalid object passed to copy constructor. Expected NeomodelPoint or shapely Point, received {type(args[0])}"
+                    )
+
             # Initialisation is either via x,y[,z] XOR longitude,latitude[,height]. Specifying both leads to an error.
             if any(i is not None for i in [x, y, z]) and any(
                 i is not None for i in [latitude, longitude, height]
             ):
                 raise ValueError(
                     "Invalid instantiation via arguments. "
                     "A Point can be defined either by x,y,z coordinates OR latitude,longitude,height but not "
                     "a combination of these terms"
                 )
-    
+
             # Specifying no initialisation argument at this point in the constructor is flagged as an error
             if all(i is None for i in [x, y, z, latitude, longitude, height]):
                 raise ValueError(
                     "Invalid instantiation via no arguments. "
                     "A Point needs default values either in x,y,z or longitude, latitude, height coordinates"
                 )
-    
+
             # Geographical Point Initialisation
             if latitude is not None and longitude is not None:
                 if height is not None:
                     if self._crs is None:
                         self._crs = "wgs-84-3d"
                     _z = height
                 else:
                     if self._crs is None:
                         self._crs = "wgs-84"
                 _x = longitude
                 _y = latitude
-    
+
             # Geometrical Point Initialisation
             if x is not None and y is not None:
                 if z is not None:
                     if self._crs is None:
                         self._crs = "cartesian-3d"
                     _z = z
                 else:
                     if self._crs is None:
                         self._crs = "cartesian"
                 _x = x
                 _y = y
-    
+
             if _z is None:
                 if "-3d" not in self._crs:
                     self._shapely_point = ShapelyPoint((float(_x), float(_y)))
                 else:
-                    raise ValueError(f"Invalid vector dimensions(2) for given CRS({self._crs}).")
+                    raise ValueError(
+                        f"Invalid vector dimensions(2) for given CRS({self._crs})."
+                    )
             else:
                 if "-3d" in self._crs:
-                    self._shapely_point = ShapelyPoint((float(_x), float(_y), float(_z)))
+                    self._shapely_point = ShapelyPoint(
+                        (float(_x), float(_y), float(_z))
+                    )
                 else:
-                    raise ValueError(f"Invalid vector dimensions(3) for given CRS({self._crs}).")
+                    raise ValueError(
+                        f"Invalid vector dimensions(3) for given CRS({self._crs})."
+                    )
 
-               
         @property
         def crs(self):
             return self._crs
-    
+
         @property
         def x(self):
             if not self._crs.startswith("cartesian"):
                 raise TypeError(
                     f'Invalid coordinate ("x") for points defined over {self.crs}'
                 )
             return self._shapely_point.x
-    
+
         @property
         def y(self):
             if not self._crs.startswith("cartesian"):
                 raise TypeError(
                     f'Invalid coordinate ("y") for points defined over {self.crs}'
                 )
             return self._shapely_point.y
-    
+
         @property
         def z(self):
             if self._crs != "cartesian-3d":
                 raise TypeError(
                     f'Invalid coordinate ("z") for points defined over {self.crs}'
                 )
             return self._shapely_point.z
-    
+
         @property
         def latitude(self):
             if not self._crs.startswith("wgs-84"):
                 raise TypeError(
                     f'Invalid coordinate ("latitude") for points defined over {self.crs}'
                 )
             return self._shapely_point.y
-    
+
         @property
         def longitude(self):
             if not self._crs.startswith("wgs-84"):
                 raise TypeError(
                     f'Invalid coordinate ("longitude") for points defined over {self.crs}'
                 )
             return self._shapely_point.x
-    
+
         @property
         def height(self):
             if self._crs != "wgs-84-3d":
                 raise TypeError(
                     f'Invalid coordinate ("height") for points defined over {self.crs}'
                 )
             return self._shapely_point.z
-    
+
         # The following operations are necessary here due to the way queries (and more importantly their parameters) get
         # combined and evaluated in neomodel. Specifically, query expressions get duplicated with deep copies and any valid
         # datatype values should also implement these operations.
         def __copy__(self):
             return NeomodelPoint(self)
-    
+
         def __deepcopy__(self, memo):
             return NeomodelPoint(self)
 
         def __getattr__(self, attr):
             """
             Route messages to the right underlying object.
             """
             return getattr(self._shapely_point, attr)
 
         def __eq__(self, other):
             """
             Compare objects by value
             """
             if not isinstance(other, (ShapelyPoint, NeomodelPoint)):
-                raise ValueException(f"NeomodelPoint equality comparison expected NeomodelPoint or Shapely Point, received {type(other)}")
+                raise ValueException(
+                    f"NeomodelPoint equality comparison expected NeomodelPoint or Shapely Point, received {type(other)}"
+                )
             else:
                 if isinstance(other, ShapelyPoint):
                     return self.coords[0] == other.coords[0]
                 else:
                     return self.coords[0] == other.coords[0] and self.crs == other.crs
 
 
@@ -513,20 +542,27 @@
         if "crs" in kwargs:
             crs = kwargs["crs"]
             del kwargs["crs"]
         else:
             crs = None
 
         if crs is None or (crs not in ACCEPTABLE_CRS):
-            raise ValueError(f"Invalid CRS({crs}). Point properties require CRS to be one of {','.join(ACCEPTABLE_CRS)}")
+            raise ValueError(
+                f"Invalid CRS({crs}). Point properties require CRS to be one of {','.join(ACCEPTABLE_CRS)}"
+            )
 
         # If a default value is passed and it is not a callable, then make sure it is in the right type
-        if "default" in kwargs and not hasattr(kwargs["default"], "__call__") and not isinstance(kwargs["default"], NeomodelPoint):
-                    raise TypeError(f"Invalid default value. Expected NeomodelPoint, received {type(kwargs['default'])}"
-                    )
+        if (
+            "default" in kwargs
+            and not hasattr(kwargs["default"], "__call__")
+            and not isinstance(kwargs["default"], NeomodelPoint)
+        ):
+            raise TypeError(
+                f"Invalid default value. Expected NeomodelPoint, received {type(kwargs['default'])}"
+            )
 
         super().__init__(*args, **kwargs)
         self._crs = crs
 
     @validator
     def inflate(self, value):
         """
@@ -540,18 +576,22 @@
             raise TypeError(
                 f"Invalid datatype to inflate. Expected POINT datatype, received {type(value)}"
             )
 
         try:
             value_point_crs = SRID_TO_CRS[value.srid]
         except KeyError as e:
-            raise ValueError(f"Invalid SRID to inflate. Expected one of {SRID_TO_CRS.keys()}, received {value.srid}") from e
+            raise ValueError(
+                f"Invalid SRID to inflate. Expected one of {SRID_TO_CRS.keys()}, received {value.srid}"
+            ) from e
 
         if self._crs != value_point_crs:
-            raise ValueError(f"Invalid CRS. Expected POINT defined over {self._crs}, received {value_point_crs}")
+            raise ValueError(
+                f"Invalid CRS. Expected POINT defined over {self._crs}, received {value_point_crs}"
+            )
         # cartesian
         if value.srid == 7203:
             return NeomodelPoint(x=value.x, y=value.y)
         # cartesian-3d
         if value.srid == 9157:
             return NeomodelPoint(x=value.x, y=value.y, z=value.z)
         # wgs-84
@@ -577,15 +617,17 @@
         """
         if not isinstance(value, NeomodelPoint):
             raise TypeError(
                 f"Invalid datatype to deflate. Expected NeomodelPoint, received {type(value)}"
             )
 
         if value.crs != self._crs:
-            raise ValueError(f"Invalid CRS. Expected NeomodelPoint defined over {self._crs}, received NeomodelPoint defined over {value.crs}")
+            raise ValueError(
+                f"Invalid CRS. Expected NeomodelPoint defined over {self._crs}, received NeomodelPoint defined over {value.crs}"
+            )
 
         if value.crs == "cartesian-3d":
             return neo4j.spatial.CartesianPoint((value.x, value.y, value.z))
         if value.crs == "cartesian":
             return neo4j.spatial.CartesianPoint((value.x, value.y))
         if value.crs == "wgs-84":
             return neo4j.spatial.WGS84Point((value.longitude, value.latitude))
```

### Comparing `neomodel-5.2.1/neomodel/exceptions.py` & `neomodel-5.3.0/neomodel/exceptions.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.2.1/neomodel/integration/numpy.py` & `neomodel-5.3.0/neomodel/integration/numpy.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 .. note::
    This module requires numpy to be installed, and will raise a
    warning if this is not available.
 
 Example:
 
-    >>> from neomodel import db
+    >>> from neomodel.async_ import db
     >>> from neomodel.integration.numpy import to_nparray
     >>> db.set_connection('bolt://neo4j:secret@localhost:7687')
     >>> df = to_nparray(db.cypher_query("MATCH (u:User) RETURN u.email AS email, u.name AS name"))
     >>> df
     array([['jimla@test.com', 'jimla'], ['jimlo@test.com', 'jimlo']])
 """
```

### Comparing `neomodel-5.2.1/neomodel/integration/pandas.py` & `neomodel-5.3.0/neomodel/integration/pandas.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 .. note::
    This module requires pandas to be installed, and will raise a
    warning if this is not available.
 
 Example:
 
-    >>> from neomodel import db
+    >>> from neomodel.async_ import db
     >>> from neomodel.integration.pandas import to_dataframe
     >>> db.set_connection('bolt://neo4j:secret@localhost:7687')
     >>> df = to_dataframe(db.cypher_query("MATCH (u:User) RETURN u.email AS email, u.name AS name"))
     >>> df
                        email    name
     0         jimla@test.com   jimla
     1         jimlo@test.com   jimlo
```

### Comparing `neomodel-5.2.1/neomodel/match.py` & `neomodel-5.3.0/neomodel/sync_/match.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import inspect
 import re
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import Optional
 
-from .core import StructuredNode, db
-from .exceptions import MultipleNodesReturned
-from .match_q import Q, QBase
-from .properties import AliasProperty
-
-OUTGOING, INCOMING, EITHER = 1, -1, 0
+from neomodel.exceptions import MultipleNodesReturned
+from neomodel.match_q import Q, QBase
+from neomodel.properties import AliasProperty, ArrayProperty
+from neomodel.sync_.core import StructuredNode, db
+from neomodel.util import INCOMING, OUTGOING
 
 
 def _rel_helper(
     lhs,
     rhs,
     ident=None,
     relation_type=None,
@@ -146,14 +145,15 @@
         stmt = stmt.format(f"[{ident}:`{relation_type}`{rel_props}]")
 
     return f"({lhs}){stmt}({rhs}){rel_none_props}"
 
 
 # special operators
 _SPECIAL_OPERATOR_IN = "IN"
+_SPECIAL_OPERATOR_ARRAY_IN = "any(x IN {ident}.{prop} WHERE x IN {val})"
 _SPECIAL_OPERATOR_INSENSITIVE = "(?i)"
 _SPECIAL_OPERATOR_ISNULL = "IS NULL"
 _SPECIAL_OPERATOR_ISNOTNULL = "IS NOT NULL"
 _SPECIAL_OPERATOR_REGEX = "=~"
 
 _UNARY_OPERATORS = (_SPECIAL_OPERATOR_ISNULL, _SPECIAL_OPERATOR_ISNOTNULL)
 
@@ -243,44 +243,106 @@
                 operator=operator,
                 filter_key=key,
                 filter_value=value,
                 property_obj=property_obj,
             )
 
         # map property to correct property name in the database
-        db_property = cls.defined_properties(rels=False)[prop].db_property or prop
+        db_property = cls.defined_properties(rels=False)[prop].get_db_property_name(
+            prop
+        )
 
         output[db_property] = (operator, deflated_value)
 
     return output
 
 
+def transform_in_operator_to_filter(operator, filter_key, filter_value, property_obj):
+    """
+    Transform in operator to a cypher filter
+    Args:
+        operator (str): operator to transform
+        filter_key (str): filter key
+        filter_value (str): filter value
+        property_obj (object): property object
+    Returns:
+        tuple: operator, deflated_value
+    """
+    if not isinstance(filter_value, tuple) and not isinstance(filter_value, list):
+        raise ValueError(
+            f"Value must be a tuple or list for IN operation {filter_key}={filter_value}"
+        )
+    if isinstance(property_obj, ArrayProperty):
+        deflated_value = property_obj.deflate(filter_value)
+        operator = _SPECIAL_OPERATOR_ARRAY_IN
+    else:
+        deflated_value = [property_obj.deflate(v) for v in filter_value]
+
+    return operator, deflated_value
+
+
+def transform_null_operator_to_filter(filter_key, filter_value):
+    """
+    Transform null operator to a cypher filter
+    Args:
+        filter_key (str): filter key
+        filter_value (str): filter value
+    Returns:
+        tuple: operator, deflated_value
+    """
+    if not isinstance(filter_value, bool):
+        raise ValueError(f"Value must be a bool for isnull operation on {filter_key}")
+    operator = "IS NULL" if filter_value else "IS NOT NULL"
+    deflated_value = None
+    return operator, deflated_value
+
+
+def transform_regex_operator_to_filter(
+    operator, filter_key, filter_value, property_obj
+):
+    """
+    Transform regex operator to a cypher filter
+    Args:
+        operator (str): operator to transform
+        filter_key (str): filter key
+        filter_value (str): filter value
+        property_obj (object): property object
+    Returns:
+        tuple: operator, deflated_value
+    """
+
+    deflated_value = property_obj.deflate(filter_value)
+    if not isinstance(deflated_value, str):
+        raise ValueError(f"Must be a string value for {filter_key}")
+    if operator in _STRING_REGEX_OPERATOR_TABLE.values():
+        deflated_value = re.escape(deflated_value)
+    deflated_value = operator.format(deflated_value)
+    operator = _SPECIAL_OPERATOR_REGEX
+    return operator, deflated_value
+
+
 def transform_operator_to_filter(operator, filter_key, filter_value, property_obj):
-    # handle special operators
     if operator == _SPECIAL_OPERATOR_IN:
-        if not isinstance(filter_value, tuple) and not isinstance(filter_value, list):
-            raise ValueError(
-                f"Value must be a tuple or list for IN operation {filter_key}={filter_value}"
-            )
-        deflated_value = [property_obj.deflate(v) for v in filter_value]
+        operator, deflated_value = transform_in_operator_to_filter(
+            operator=operator,
+            filter_key=filter_key,
+            filter_value=filter_value,
+            property_obj=property_obj,
+        )
     elif operator == _SPECIAL_OPERATOR_ISNULL:
-        if not isinstance(filter_value, bool):
-            raise ValueError(
-                f"Value must be a bool for isnull operation on {filter_key}"
-            )
-        operator = "IS NULL" if filter_value else "IS NOT NULL"
-        deflated_value = None
+        operator, deflated_value = transform_null_operator_to_filter(
+            filter_key=filter_key, filter_value=filter_value
+        )
     elif operator in _REGEX_OPERATOR_TABLE.values():
-        deflated_value = property_obj.deflate(filter_value)
-        if not isinstance(deflated_value, str):
-            raise ValueError(f"Must be a string value for {filter_key}")
-        if operator in _STRING_REGEX_OPERATOR_TABLE.values():
-            deflated_value = re.escape(deflated_value)
-        deflated_value = operator.format(deflated_value)
-        operator = _SPECIAL_OPERATOR_REGEX
+        operator, deflated_value = transform_regex_operator_to_filter(
+            operator=operator,
+            filter_key=filter_key,
+            filter_value=filter_value,
+            property_obj=property_obj,
+        )
     else:
         deflated_value = property_obj.deflate(filter_value)
 
     return operator, deflated_value
 
 
 def process_has_args(cls, kwargs):
@@ -501,15 +563,15 @@
         ident = node.__class__.__name__.lower()
         place_holder = self._register_place_holder(ident)
 
         # Hack to emulate START to lookup a node by id
         _node_lookup = f"MATCH ({ident}) WHERE {db.get_id_method()}({ident})=${place_holder} WITH {ident}"
         self._ast.lookup = _node_lookup
 
-        self._query_params[place_holder] = node.element_id
+        self._query_params[place_holder] = db.parse_element_id(node.element_id)
 
         self._ast.return_clause = ident
         self._ast.result_class = node.__class__
         return ident
 
     def build_label(self, ident, cls):
         """
@@ -568,15 +630,22 @@
                 for prop, op_and_val in filters.items():
                     operator, val = op_and_val
                     if operator in _UNARY_OPERATORS:
                         # unary operators do not have a parameter
                         statement = f"{ident}.{prop} {operator}"
                     else:
                         place_holder = self._register_place_holder(ident + "_" + prop)
-                        statement = f"{ident}.{prop} {operator} ${place_holder}"
+                        if operator == _SPECIAL_OPERATOR_ARRAY_IN:
+                            statement = operator.format(
+                                ident=ident,
+                                prop=prop,
+                                val=f"${place_holder}",
+                            )
+                        else:
+                            statement = f"{ident}.{prop} {operator} ${place_holder}"
                         self._query_params[place_holder] = val
                     target.append(statement)
         ret = f" {q.connector} ".join(target)
         if q.negated:
             ret = f"NOT ({ret})"
         return ret
 
@@ -728,32 +797,50 @@
     def all(self, lazy=False):
         """
         Return all nodes belonging to the set
         :param lazy: False by default, specify True to get nodes with id only without the parameters.
         :return: list of nodes
         :rtype: list
         """
-        return self.query_cls(self).build_ast()._execute(lazy)
+        ast = self.query_cls(self).build_ast()
+        return ast._execute(lazy)
 
     def __iter__(self):
-        return (i for i in self.query_cls(self).build_ast()._execute())
+        ast = self.query_cls(self).build_ast()
+        for i in ast._execute():
+            yield i
 
     def __len__(self):
-        return self.query_cls(self).build_ast()._count()
+        ast = self.query_cls(self).build_ast()
+        return ast._count()
 
     def __bool__(self):
-        return self.query_cls(self).build_ast()._count() > 0
+        """
+        Override for __bool__ dunder method.
+        :return: True if the set contains any nodes, False otherwise
+        :rtype: bool
+        """
+        ast = self.query_cls(self).build_ast()
+        _count = ast._count()
+        return _count > 0
 
     def __nonzero__(self):
-        return self.query_cls(self).build_ast()._count() > 0
+        """
+        Override for __bool__ dunder method.
+        :return: True if the set contains any node, False otherwise
+        :rtype: bool
+        """
+        return self.__bool__()
 
     def __contains__(self, obj):
         if isinstance(obj, StructuredNode):
             if hasattr(obj, "element_id") and obj.element_id is not None:
-                return self.query_cls(self).build_ast()._contains(obj.element_id)
+                ast = self.query_cls(self).build_ast()
+                obj_element_id = db.parse_element_id(obj.element_id)
+                return ast._contains(obj_element_id)
             raise ValueError("Unsaved node: " + repr(obj))
 
         raise ValueError("Expecting StructuredNode instance")
 
     def __getitem__(self, key):
         if isinstance(key, slice):
             if key.stop and key.start:
@@ -766,15 +853,17 @@
 
             return self
 
         if isinstance(key, int):
             self.skip = key
             self.limit = 1
 
-            return self.query_cls(self).build_ast()._execute()[0]
+            ast = self.query_cls(self).build_ast()
+            _items = ast._execute()
+            return _items[0]
 
         return None
 
 
 @dataclass
 class Optional:
     """Simple relation qualifier."""
@@ -806,19 +895,23 @@
 
         # used by has()
         self.must_match = {}
         self.dont_match = {}
 
         self.relations_to_fetch: list = []
 
+    def __await__(self):
+        return self.all().__await__()
+
     def _get(self, limit=None, lazy=False, **kwargs):
         self.filter(**kwargs)
         if limit:
             self.limit = limit
-        return self.query_cls(self).build_ast()._execute(lazy)
+        ast = self.query_cls(self).build_ast()
+        return ast._execute(lazy)
 
     def get(self, lazy=False, **kwargs):
         """
         Retrieve one node from the set matching supplied parameters
         :param lazy: False by default, specify True to get nodes with id only without the parameters.
         :param kwargs: same syntax as `filter()`
         :return: node
@@ -845,15 +938,15 @@
     def first(self, **kwargs):
         """
         Retrieve the first node from the set matching supplied parameters
 
         :param kwargs: same syntax as `filter()`
         :return: node
         """
-        result = result = self._get(limit=1, **kwargs)
+        result = self._get(limit=1, **kwargs)
         if result:
             return result[0]
         else:
             raise self.source_class.DoesNotExist(repr(kwargs))
 
     def first_or_none(self, **kwargs):
         """
@@ -982,14 +1075,17 @@
     :param name: A name for the traversal.
     :type name: :class:`str`
     :param definition: A relationship definition that most certainly deserves
                        a documentation here.
     :type defintion: :class:`dict`
     """
 
+    def __await__(self):
+        return self.all().__await__()
+
     def __init__(self, source, name, definition):
         """
         Create a traversal
 
         """
         self.source = source
```

### Comparing `neomodel-5.2.1/neomodel/match_q.py` & `neomodel-5.3.0/neomodel/match_q.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,19 @@
         setting up to do).
         """
         obj = QBase(children, connector, negated)
         obj.__class__ = cls
         return obj
 
     def __str__(self):
-        return f"(NOT ({self.connector}: {', '.join(str(c) for c in self.children)}))" if self.negated else f"({self.connector}: {', '.join(str(c) for c in self.children)})"
+        return (
+            f"(NOT ({self.connector}: {', '.join(str(c) for c in self.children)}))"
+            if self.negated
+            else f"({self.connector}: {', '.join(str(c) for c in self.children)})"
+        )
 
     def __repr__(self):
         return f"<{self.__class__.__name__}: {self}>"
 
     def __deepcopy__(self, memodict):
         obj = QBase(connector=self.connector, negated=self.negated)
         obj.__class__ = self.__class__
```

### Comparing `neomodel-5.2.1/neomodel/path.py` & `neomodel-5.3.0/neomodel/sync_/path.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from neo4j.graph import Path
-from .core import db
-from .relationship import StructuredRel
-from .exceptions import RelationshipClassNotDefined
+
+from neomodel.sync_.core import db
+from neomodel.sync_.relationship import StructuredRel
 
 
 class NeomodelPath(Path):
     """
     Represents paths within neomodel.
 
-    This object is instantiated when you include whole paths in your ``cypher_query()`` 
+    This object is instantiated when you include whole paths in your ``cypher_query()``
     result sets and turn ``resolve_objects`` to True.
 
     That is, any query of the form:
     ::
 
         MATCH p=(:SOME_NODE_LABELS)-[:SOME_REL_LABELS]-(:SOME_OTHER_NODE_LABELS) return p
 
-    ``NeomodelPath`` are simple objects that reference their nodes and relationships, each of which is already 
+    ``NeomodelPath`` are simple objects that reference their nodes and relationships, each of which is already
     resolved to their neomodel objects if such mapping is possible.
 
 
     :param nodes: Neomodel nodes appearing in the path in order of appearance.
     :param relationships: Neomodel relationships appearing in the path in order of appearance.
     :type nodes: List[StructuredNode]
     :type relationships: List[StructuredRel]
     """
+
     def __init__(self, a_neopath):
-        self._nodes=[]
+        self._nodes = []
         self._relationships = []
 
         for a_node in a_neopath.nodes:
             self._nodes.append(db._object_resolution(a_node))
 
         for a_relationship in a_neopath.relationships:
             # This check is required here because if the relationship does not bear data
@@ -38,16 +39,15 @@
             # an "unspecified" StructuredRel.
             rel_type = frozenset([a_relationship.type])
             if rel_type in db._NODE_CLASS_REGISTRY:
                 new_rel = db._object_resolution(a_relationship)
             else:
                 new_rel = StructuredRel.inflate(a_relationship)
             self._relationships.append(new_rel)
+
     @property
     def nodes(self):
         return self._nodes
 
     @property
     def relationships(self):
         return self._relationships
-
-
```

### Comparing `neomodel-5.2.1/neomodel/properties.py` & `neomodel-5.3.0/neomodel/properties.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,130 +1,24 @@
 import functools
 import json
 import re
 import sys
-import types
 import uuid
 from datetime import date, datetime
 
 import neo4j.time
 import pytz
 
 from neomodel import config
-from neomodel.exceptions import DeflateError, InflateError, RequiredProperty
+from neomodel.exceptions import DeflateError, InflateError
 
 if sys.version_info >= (3, 0):
     Unicode = str
 
 
-def display_for(key):
-    def display_choice(self):
-        return getattr(self.__class__, key).choices[getattr(self, key)]
-
-    return display_choice
-
-
-class PropertyManager:
-    """
-    Common methods for handling properties on node and relationship objects.
-    """
-
-    def __init__(self, **kwargs):
-        properties = getattr(self, "__all_properties__", None)
-        if properties is None:
-            properties = self.defined_properties(rels=False, aliases=False).items()
-        for name, property in properties:
-            if kwargs.get(name) is None:
-                if getattr(property, "has_default", False):
-                    setattr(self, name, property.default_value())
-                else:
-                    setattr(self, name, None)
-            else:
-                setattr(self, name, kwargs[name])
-
-            if getattr(property, "choices", None):
-                setattr(
-                    self,
-                    f"get_{name}_display",
-                    types.MethodType(display_for(name), self),
-                )
-
-            if name in kwargs:
-                del kwargs[name]
-
-        aliases = getattr(self, "__all_aliases__", None)
-        if aliases is None:
-            aliases = self.defined_properties(
-                aliases=True, rels=False, properties=False
-            ).items()
-        for name, property in aliases:
-            if name in kwargs:
-                setattr(self, name, kwargs[name])
-                del kwargs[name]
-
-        # undefined properties (for magic @prop.setters etc)
-        for name, property in kwargs.items():
-            setattr(self, name, property)
-
-    @property
-    def __properties__(self):
-        from .relationship_manager import RelationshipManager
-
-        return dict(
-            (name, value)
-            for name, value in vars(self).items()
-            if not name.startswith("_")
-            and not callable(value)
-            and not isinstance(
-                value,
-                (
-                    RelationshipManager,
-                    AliasProperty,
-                ),
-            )
-        )
-
-    @classmethod
-    def deflate(cls, properties, obj=None, skip_empty=False):
-        # deflate dict ready to be stored
-        deflated = {}
-        for name, property in cls.defined_properties(aliases=False, rels=False).items():
-            db_property = property.db_property or name
-            if properties.get(name) is not None:
-                deflated[db_property] = property.deflate(properties[name], obj)
-            elif property.has_default:
-                deflated[db_property] = property.deflate(property.default_value(), obj)
-            elif property.required:
-                raise RequiredProperty(name, cls)
-            elif not skip_empty:
-                deflated[db_property] = None
-        return deflated
-
-    @classmethod
-    def defined_properties(cls, aliases=True, properties=True, rels=True):
-        from .relationship_manager import RelationshipDefinition
-
-        props = {}
-        for baseclass in reversed(cls.__mro__):
-            props.update(
-                dict(
-                    (name, property)
-                    for name, property in vars(baseclass).items()
-                    if (aliases and isinstance(property, AliasProperty))
-                    or (
-                        properties
-                        and isinstance(property, Property)
-                        and not isinstance(property, AliasProperty)
-                    )
-                    or (rels and isinstance(property, RelationshipDefinition))
-                )
-            )
-        return props
-
-
 def validator(fn):
     fn_name = fn.func_name if hasattr(fn, "func_name") else fn.__name__
     if fn_name == "inflate":
         exc_class = InflateError
     elif fn_name == "deflate":
         exc_class = DeflateError
     else:
@@ -206,14 +100,21 @@
         """
         if self.has_default:
             if hasattr(self.default, "__call__"):
                 return self.default()
             return self.default
         raise ValueError("No default value specified")
 
+    def get_db_property_name(self, attribute_name):
+        """
+        Returns the name that should be used for the property in the database. This is db_property if supplied upon
+        construction, otherwise the given attribute_name from the model is used.
+        """
+        return self.db_property or attribute_name
+
     @property
     def is_indexed(self):
         return self.unique_index or self.index
 
 
 class NormalizedProperty(Property):
     """
@@ -463,15 +364,15 @@
             msg = f"datetime.date object expected, got {repr(value)}"
             raise ValueError(msg)
         return value.isoformat()
 
 
 class DateTimeFormatProperty(Property):
     """
-    Store a datetime by custome format
+    Store a datetime by custom format
     :param default_now: If ``True``, the creation time (Local) will be used as default.
                         Defaults to ``False``.
     :param format:      Date format string, default is %Y-%m-%d
 
     :type default_now:  :class:`bool`
     :type format:       :class:`str`
     """
```

### Comparing `neomodel-5.2.1/neomodel/relationship.py` & `neomodel-5.3.0/neomodel/sync_/relationship.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import warnings
+from neomodel.hooks import hooks
+from neomodel.properties import Property
+from neomodel.sync_.core import db
+from neomodel.sync_.property_manager import PropertyManager
 
-from .core import db
-from .hooks import hooks
-from .properties import Property, PropertyManager
+ELEMENT_ID_MIGRATION_NOTICE = "id is deprecated in Neo4j version 5, please migrate to element_id. If you use the id in a Cypher query, replace id() by elementId()."
 
 
 class RelationshipMeta(type):
     def __new__(mcs, name, bases, dct):
         inst = super().__new__(mcs, name, bases, dct)
         for key, value in dct.items():
             if issubclass(value.__class__, Property):
@@ -46,128 +47,106 @@
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @property
     def element_id(self):
-        return (
-            int(self.element_id_property)
-            if db.database_version.startswith("4")
-            else self.element_id_property
-        )
+        if hasattr(self, "element_id_property"):
+            return self.element_id_property
 
     @property
     def _start_node_element_id(self):
-        return (
-            int(self._start_node_element_id_property)
-            if db.database_version.startswith("4")
-            else self._start_node_element_id_property
-        )
+        if hasattr(self, "_start_node_element_id_property"):
+            return self._start_node_element_id_property
 
     @property
     def _end_node_element_id(self):
-        return (
-            int(self._end_node_element_id_property)
-            if db.database_version.startswith("4")
-            else self._end_node_element_id_property
-        )
+        if hasattr(self, "_end_node_element_id_property"):
+            return self._end_node_element_id_property
 
     # Version 4.4 support - id is deprecated in version 5.x
     @property
     def id(self):
         try:
             return int(self.element_id_property)
-        except (TypeError, ValueError):
-            raise ValueError(
-                "id is deprecated in Neo4j version 5, please migrate to element_id. If you use the id in a Cypher query, replace id() by elementId()."
-            )
+        except (TypeError, ValueError) as exc:
+            raise ValueError(ELEMENT_ID_MIGRATION_NOTICE) from exc
 
     # Version 4.4 support - id is deprecated in version 5.x
     @property
     def _start_node_id(self):
         try:
             return int(self._start_node_element_id_property)
-        except (TypeError, ValueError):
-            raise ValueError(
-                "id is deprecated in Neo4j version 5, please migrate to element_id. If you use the id in a Cypher query, replace id() by elementId()."
-            )
+        except (TypeError, ValueError) as exc:
+            raise ValueError(ELEMENT_ID_MIGRATION_NOTICE) from exc
 
     # Version 4.4 support - id is deprecated in version 5.x
     @property
     def _end_node_id(self):
         try:
             return int(self._end_node_element_id_property)
-        except (TypeError, ValueError):
-            raise ValueError(
-                "id is deprecated in Neo4j version 5, please migrate to element_id. If you use the id in a Cypher query, replace id() by elementId()."
-            )
+        except (TypeError, ValueError) as exc:
+            raise ValueError(ELEMENT_ID_MIGRATION_NOTICE) from exc
 
     @hooks
     def save(self):
         """
         Save the relationship
 
         :return: self
         """
         props = self.deflate(self.__properties__)
         query = f"MATCH ()-[r]->() WHERE {db.get_id_method()}(r)=$self "
         query += "".join([f" SET r.{key} = ${key}" for key in props])
-        props["self"] = self.element_id
+        props["self"] = db.parse_element_id(self.element_id)
 
         db.cypher_query(query, props)
 
         return self
 
     def start_node(self):
         """
         Get start node
 
         :return: StructuredNode
         """
-        test = db.cypher_query(
+        results = db.cypher_query(
             f"""
             MATCH (aNode)
             WHERE {db.get_id_method()}(aNode)=$start_node_element_id
             RETURN aNode
             """,
-            {"start_node_element_id": self._start_node_element_id},
+            {"start_node_element_id": db.parse_element_id(self._start_node_element_id)},
             resolve_objects=True,
         )
-        return test[0][0][0]
+        return results[0][0][0]
 
     def end_node(self):
         """
         Get end node
 
         :return: StructuredNode
         """
-        return db.cypher_query(
+        results = db.cypher_query(
             f"""
             MATCH (aNode)
             WHERE {db.get_id_method()}(aNode)=$end_node_element_id
             RETURN aNode
             """,
-            {"end_node_element_id": self._end_node_element_id},
+            {"end_node_element_id": db.parse_element_id(self._end_node_element_id)},
             resolve_objects=True,
-        )[0][0][0]
+        )
+        return results[0][0][0]
 
     @classmethod
     def inflate(cls, rel):
         """
         Inflate a neo4j_driver relationship object to a neomodel object
         :param rel:
         :return: StructuredRel
         """
-        props = {}
-        for key, prop in cls.defined_properties(aliases=False, rels=False).items():
-            if key in rel:
-                props[key] = prop.inflate(rel[key], obj=rel)
-            elif prop.has_default:
-                props[key] = prop.default_value()
-            else:
-                props[key] = None
-        srel = cls(**props)
+        srel = super().inflate(rel)
         srel._start_node_element_id_property = rel.start_node.element_id
         srel._end_node_element_id_property = rel.end_node.element_id
         srel.element_id_property = rel.element_id
         return srel
```

### Comparing `neomodel-5.2.1/neomodel/relationship_manager.py` & `neomodel-5.3.0/neomodel/sync_/relationship_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import functools
 import inspect
 import sys
 from importlib import import_module
 
-from .core import db
-from .exceptions import NotConnected, RelationshipClassRedefined
-from .match import (
+from neomodel.exceptions import NotConnected, RelationshipClassRedefined
+from neomodel.sync_.core import db
+from neomodel.sync_.match import NodeSet, Traversal, _rel_helper, _rel_merge_helper
+from neomodel.sync_.relationship import StructuredRel
+from neomodel.util import (
     EITHER,
     INCOMING,
     OUTGOING,
-    NodeSet,
-    Traversal,
-    _rel_helper,
-    _rel_merge_helper,
+    enumerate_traceback,
+    get_graph_entity_properties,
 )
-from .relationship import StructuredRel
-from .util import _get_node_properties, enumerate_traceback
 
 # basestring python 3.x fallback
 try:
     basestring
 except NameError:
     basestring = str
 
@@ -62,14 +60,17 @@
         if self.definition["direction"] == OUTGOING:
             direction = "a outgoing"
         elif self.definition["direction"] == INCOMING:
             direction = "a incoming"
 
         return f"{self.description} in {direction} direction of type {self.definition['relation_type']} on node ({self.source.element_id}) of class '{self.source_class.__name__}'"
 
+    def __await__(self):
+        return self.all().__await__()
+
     def _check_node(self, obj):
         """check for valid node i.e correct class and is saved"""
         if not issubclass(type(obj), self.definition["node_class"]):
             raise ValueError(
                 "Expected node of class " + self.definition["node_class"].__name__
             )
         if not hasattr(obj, "element_id"):
@@ -120,21 +121,22 @@
             **self.definition,
         )
         q = (
             f"MATCH (them), (us) WHERE {db.get_id_method()}(them)=$them and {db.get_id_method()}(us)=$self "
             "MERGE" + new_rel
         )
 
-        params["them"] = node.element_id
+        params["them"] = db.parse_element_id(node.element_id)
 
         if not rel_model:
             self.source.cypher(q, params)
             return True
 
-        rel_ = self.source.cypher(q + " RETURN r", params)[0][0][0]
+        results = self.source.cypher(q + " RETURN r", params)
+        rel_ = results[0][0][0]
         rel_instance = self._set_start_end_cls(rel_model.inflate(rel_), node)
 
         if hasattr(rel_instance, "post_save"):
             rel_instance.post_save()
 
         return rel_instance
 
@@ -162,15 +164,16 @@
         self._check_node(node)
         my_rel = _rel_helper(lhs="us", rhs="them", ident="r", **self.definition)
         q = (
             "MATCH "
             + my_rel
             + f" WHERE {db.get_id_method()}(them)=$them and {db.get_id_method()}(us)=$self RETURN r LIMIT 1"
         )
-        rels = self.source.cypher(q, {"them": node.element_id})[0]
+        results = self.source.cypher(q, {"them": db.parse_element_id(node.element_id)})
+        rels = results[0]
         if not rels:
             return
 
         rel_model = self.definition.get("model") or StructuredRel
 
         return self._set_start_end_cls(rel_model.inflate(rels[0][0]), node)
 
@@ -182,15 +185,16 @@
         :param node:
         :return: [StructuredRel]
         """
         self._check_node(node)
 
         my_rel = _rel_helper(lhs="us", rhs="them", ident="r", **self.definition)
         q = f"MATCH {my_rel} WHERE {db.get_id_method()}(them)=$them and {db.get_id_method()}(us)=$self RETURN r "
-        rels = self.source.cypher(q, {"them": node.element_id})[0]
+        results = self.source.cypher(q, {"them": db.parse_element_id(node.element_id)})
+        rels = results[0]
         if not rels:
             return []
 
         rel_model = self.definition.get("model") or StructuredRel
         return [
             self._set_start_end_cls(rel_model.inflate(rel[0]), node) for rel in rels
         ]
@@ -219,23 +223,25 @@
         self._check_node(old_node)
         self._check_node(new_node)
         if old_node.element_id == new_node.element_id:
             return
         old_rel = _rel_helper(lhs="us", rhs="old", ident="r", **self.definition)
 
         # get list of properties on the existing rel
+        old_node_element_id = db.parse_element_id(old_node.element_id)
+        new_node_element_id = db.parse_element_id(new_node.element_id)
         result, _ = self.source.cypher(
             f"""
                 MATCH (us), (old) WHERE {db.get_id_method()}(us)=$self and {db.get_id_method()}(old)=$old
                 MATCH {old_rel} RETURN r
             """,
-            {"old": old_node.element_id},
+            {"old": old_node_element_id},
         )
         if result:
-            node_properties = _get_node_properties(result[0][0])
+            node_properties = get_graph_entity_properties(result[0][0])
             existing_properties = node_properties.keys()
         else:
             raise NotConnected("reconnect", self.source, old_node)
 
         # remove old relationship and create new one
         new_rel = _rel_merge_helper(lhs="us", rhs="new", ident="r2", **self.definition)
         q = (
@@ -245,30 +251,30 @@
         )
         q += " MERGE" + new_rel
 
         # copy over properties if we have
         q += "".join([f" SET r2.{prop} = r.{prop}" for prop in existing_properties])
         q += " WITH r DELETE r"
 
-        self.source.cypher(q, {"old": old_node.element_id, "new": new_node.element_id})
+        self.source.cypher(q, {"old": old_node_element_id, "new": new_node_element_id})
 
     @check_source
     def disconnect(self, node):
         """
         Disconnect a node
 
         :param node:
         :return:
         """
         rel = _rel_helper(lhs="a", rhs="b", ident="r", **self.definition)
         q = f"""
                 MATCH (a), (b) WHERE {db.get_id_method()}(a)=$self and {db.get_id_method()}(b)=$them
                 MATCH {rel} DELETE r
             """
-        self.source.cypher(q, {"them": node.element_id})
+        self.source.cypher(q, {"them": db.parse_element_id(node.element_id)})
 
     @check_source
     def disconnect_all(self):
         """
         Disconnect all nodes
 
         :return:
@@ -341,15 +347,16 @@
     def single(self):
         """
         Get a single related node or none.
 
         :return: StructuredNode
         """
         try:
-            return self[0]
+            rels = self
+            return rels[0]
         except IndexError:
             pass
 
     def match(self, **kwargs):
         """
         Return set of nodes who's relationship properties match supplied args
```

### Comparing `neomodel-5.2.1/neomodel/scripts/neomodel_inspect_database.py` & `neomodel-5.3.0/neomodel/scripts/neomodel_inspect_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 .. _neomodel_inspect_database:
 
-``_neomodel_inspect_database``
+``neomodel_inspect_database``
 ---------------------------
 
 ::
 
     usage: _neomodel_inspect_database [-h] [--db bolt://neo4j:neo4j@localhost:7687] [--write-to <someapp/models.py> ...]
     
     Connects to a Neo4j database and inspects existing nodes and relationships.
@@ -13,14 +13,16 @@
 
     If a connection URL is not specified, the tool will look up the environment 
     variable NEO4J_BOLT_URL. If that environment variable is not set, the tool
     will attempt to connect to the default URL bolt://neo4j:neo4j@localhost:7687
 
     If a file is specified, the tool will write the class definitions to that file.
     If no file is specified, the tool will print the class definitions to stdout.
+
+    Note : this script only has a synchronous mode.
     
     options:
         -h, --help            show this help message and exit
         --db bolt://neo4j:neo4j@localhost:7687
                             Neo4j Server URL
         -T, --write-to someapp/models.py
                             File where to write output.
@@ -29,15 +31,15 @@
 """
 
 import argparse
 import string
 import textwrap
 from os import environ
 
-from neomodel import db
+from neomodel.sync_.core import db
 
 IMPORTS = []
 
 
 def parse_prop_class(prop_type):
     _import = ""
     prop_class = ""
```

### Comparing `neomodel-5.2.1/neomodel/scripts/neomodel_install_labels.py` & `neomodel-5.3.0/neomodel/scripts/neomodel_install_labels.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     usage: neomodel_install_labels [-h] [--db bolt://neo4j:neo4j@localhost:7687] <someapp.models/app.py> [<someapp.models/app.py> ...]
     
     Setup indexes and constraints on labels in Neo4j for your neomodel schema.
     
     If a connection URL is not specified, the tool will look up the environment 
     variable NEO4J_BOLT_URL. If that environment variable is not set, the tool
     will attempt to connect to the default URL bolt://neo4j:neo4j@localhost:7687
+
+    Note : this script only has a synchronous mode.
     
     positional arguments:
       <someapp.models/app.py>
                             python modules or files with neomodel schema declarations.
     
     options:
       -h, --help            show this help message and exit
@@ -28,15 +30,15 @@
 
 import sys
 import textwrap
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from importlib import import_module
 from os import environ, path
 
-from .. import db, install_all_labels
+from neomodel.sync_.core import db
 
 
 def load_python_module_or_file(name):
     """
     Imports an existing python module or file into the current workspace.
 
     In both cases, *the resource must exist*.
@@ -107,12 +109,12 @@
     for app in args.apps:
         load_python_module_or_file(app)
 
     # Connect after to override any code in the module that may set the connection
     print(f"Connecting to {bolt_url}")
     db.set_connection(url=bolt_url)
 
-    install_all_labels()
+    db.install_all_labels()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `neomodel-5.2.1/neomodel/scripts/neomodel_remove_labels.py` & `neomodel-5.3.0/neomodel/scripts/neomodel_remove_labels.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,28 +10,30 @@
     usage: neomodel_remove_labels [-h] [--db bolt://neo4j:neo4j@localhost:7687]
     
     Drop all indexes and constraints on labels from schema in Neo4j database.
     
     If a connection URL is not specified, the tool will look up the environment 
     variable NEO4J_BOLT_URL. If that environment variable is not set, the tool
     will attempt to connect to the default URL bolt://neo4j:neo4j@localhost:7687
+
+    Note : this script only has a synchronous mode.
     
     options:
       -h, --help            show this help message and exit
       --db bolt://neo4j:neo4j@localhost:7687
                             Neo4j Server URL
 
 """
 from __future__ import print_function
 
 import textwrap
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from os import environ
 
-from .. import db, remove_all_labels
+from neomodel.sync_.core import db
 
 
 def main():
     parser = ArgumentParser(
         formatter_class=RawDescriptionHelpFormatter,
         description=textwrap.dedent(
             """
@@ -59,12 +61,12 @@
     if len(bolt_url) == 0:
         bolt_url = environ.get("NEO4J_BOLT_URL", "bolt://neo4j:neo4j@localhost:7687")
 
     # Connect after to override any code in the module that may set the connection
     print(f"Connecting to {bolt_url}")
     db.set_connection(url=bolt_url)
 
-    remove_all_labels()
+    db.remove_all_labels()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `neomodel-5.2.1/neomodel.egg-info/PKG-INFO` & `neomodel-5.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: neomodel
-Version: 5.2.1
+Version: 5.3.0
 Summary: An object mapper for the neo4j graph database.
 Author-email: Robin Edwards <robin.ge@gmail.com>
-Maintainer: Cristina Escalante
 Maintainer-email: Marius Conjeaud <marius.conjeaud@outlook.com>, Athanasios Anastasiou <athanastasiou@gmail.com>
 License: MIT
 Project-URL: documentation, https://neomodel.readthedocs.io/en/latest/
 Project-URL: repository, http://github.com/neo4j-contrib/neomodel
 Project-URL: changelog, https://github.com/neo4j-contrib/neomodel/releases
 Keywords: graph,neo4j,ORM,OGM,mapper
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,17 +17,19 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
-Requires-Dist: neo4j~=5.15.0
+Requires-Dist: neo4j~=5.19.0
 Provides-Extra: dev
+Requires-Dist: unasync; extra == "dev"
 Requires-Dist: pytest>=7.1; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov>=4.0; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: Shapely>=2.0.0; extra == "dev"
 Provides-Extra: pandas
 Requires-Dist: pandas; extra == "pandas"
@@ -67,32 +68,29 @@
 **For neomodel releases 4.x :**
 
 -   Python 3.7 -\> 3.10
 -   Neo4j 4.x (including 4.4 LTS for neomodel version 4.0.10)
 
 # Documentation
 
-(Needs an update, but) Available on
+Available on
 [readthedocs](http://neomodel.readthedocs.org).
 
-# Upcoming breaking changes notice - \>=5.3
+# New in 5.3.0
 
-Based on Python version [status](https://devguide.python.org/versions/),
-neomodel will be dropping support for Python 3.7 in the next release
-(5.3). This does not mean neomodel will stop working on Python 3.7, but
-it will no longer be tested against it. Instead, we will try to add
-support for Python 3.12.
-
-Another potential breaking change coming up is adding async support to
-neomodel. But we do not know when this will happen yet, or if it will
-actually be a breaking change. We will definitely push this in a major
-release though. More to come on that later.
+neomodel now supports asynchronous programming, thanks to the [Neo4j driver async API](https://neo4j.com/docs/api/python-driver/current/async_api.html). The [documentation](http://neomodel.readthedocs.org) has been updated accordingly, with an updated getting started section, and some specific documentation for the async API.
 
-Finally, we are looking at refactoring some standalone methods into the
-Database() class. More to come on that later.
+# Breaking change in 5.3.0
+
+- config.AUTO_INSTALL_LABELS has been removed. Please use the `neomodel_install_labels` script instead. _Note : this is because of the addition of async, but also because it might lead to uncontrolled creation of indexes/constraints. The script makes you more in control of said creation._
+- Based on Python version [status](https://devguide.python.org/versions/),
+neomodel will be dropping support for Python 3.7 in an upcoming release
+(5.3 or later). _This does not mean neomodel will stop working on Python 3.7, but
+it will no longer be tested against it_
+- Some standalone methods have been refactored into the Database() class. Check the [documentation](http://neomodel.readthedocs.org) for a full list.
 
 # Installation
 
 Install from pypi (recommended):
 
     $ pip install neomodel ($ source dev # To install all things needed in a Python3 venv)
 
@@ -100,14 +98,23 @@
 
     $ pip install neomodel['extras']
 
 To install from github:
 
     $ pip install git+git://github.com/neo4j-contrib/neomodel.git@HEAD#egg=neomodel-dev
 
+# Performance comparison
+
+You can find some performance tests made using Locust [in this repo](https://github.com/mariusconjeaud/neomodel-locust).
+
+Two learnings from this :
+
+* The wrapping of the driver made by neomodel is very thin performance-wise : it does not add a lot of overhead ;
+* When used in a concurrent fashion, async neomodel is faster than concurrent sync neomodel, and a lot of faster than serial queries.
+
 # Contributing
 
 Ideas, bugs, tests and pull requests always welcome. Please use
 GitHub\'s Issues page to track these.
 
 If you are interested in developing `neomodel` further, pick a subject
 from the Issues page and open a Pull Request (PR) for it. If you are
@@ -145,7 +152,46 @@
 `debug.db` database.
 
 If you have `docker-compose` installed, you can run the test suite
 against all supported Python interpreters and neo4j versions: :
 
     # in the project's root folder:
     $ sh ./tests-with-docker-compose.sh
+
+## Developing with async
+
+### Transpiling async -> sync
+
+We use [this great library](https://github.com/python-trio/unasync) to automatically transpile async code into its sync version.
+
+In other words, when contributing to neomodel, only update the `async` code in `neomodel/async_`, then run : :
+
+    bin/make-unasync
+    isort .
+    black .
+
+Note that you can also use the pre-commit hooks for this.
+
+### Specific async/sync code
+This transpiling script mainly does two things :
+
+- It removes the await keywords, and the Async prefixes in class names
+- It does some specific replacements, like `adb`->`db`, `mark_async_test`->`mark_sync_test`
+
+It might be that your code should only be run for `async`, or `sync` ; or you want different stubs to be run for `async` vs `sync`.
+You can use the following utility function for this - taken from the official [Neo4j python driver code](https://github.com/neo4j/neo4j-python-driver) :
+
+    # neomodel/async_/core.py
+    from neomodel._async_compat.util import AsyncUtil
+
+    # AsyncUtil.is_async_code is always True
+    if AsyncUtil.is_async_code:
+        # Specific async code
+        # This one gets run when in async mode
+        assert await Coffee.nodes.check_contains(2)
+    else:
+        # Specific sync code
+        # This one gest run when in sync mode
+        assert 2 in Coffee.nodes
+
+You can check [test_match_api](test/async_/test_match_api.py) for some good examples, and how it's transpiled into sync.
+
```

### Comparing `neomodel-5.2.1/neomodel.egg-info/SOURCES.txt` & `neomodel-5.3.0/neomodel.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -4,67 +4,115 @@
 pyproject.toml
 doc/source/conf.py
 doc/source/_themes/alabaster/__init__.py
 doc/source/_themes/alabaster/_version.py
 doc/source/_themes/alabaster/support.py
 neomodel/__init__.py
 neomodel/_version.py
-neomodel/cardinality.py
 neomodel/config.py
-neomodel/core.py
 neomodel/exceptions.py
 neomodel/hooks.py
-neomodel/match.py
 neomodel/match_q.py
-neomodel/path.py
 neomodel/properties.py
-neomodel/relationship.py
-neomodel/relationship_manager.py
 neomodel/util.py
 neomodel.egg-info/PKG-INFO
 neomodel.egg-info/SOURCES.txt
 neomodel.egg-info/dependency_links.txt
 neomodel.egg-info/entry_points.txt
 neomodel.egg-info/requires.txt
 neomodel.egg-info/top_level.txt
+neomodel/_async_compat/util.py
+neomodel/async_/__init__.py
+neomodel/async_/cardinality.py
+neomodel/async_/core.py
+neomodel/async_/match.py
+neomodel/async_/path.py
+neomodel/async_/property_manager.py
+neomodel/async_/relationship.py
+neomodel/async_/relationship_manager.py
 neomodel/contrib/__init__.py
-neomodel/contrib/semi_structured.py
 neomodel/contrib/spatial_properties.py
+neomodel/contrib/async_/semi_structured.py
+neomodel/contrib/sync_/semi_structured.py
 neomodel/integration/numpy.py
 neomodel/integration/pandas.py
 neomodel/scripts/__init__.py
 neomodel/scripts/neomodel_inspect_database.py
 neomodel/scripts/neomodel_install_labels.py
 neomodel/scripts/neomodel_remove_labels.py
+neomodel/sync_/__init__.py
+neomodel/sync_/cardinality.py
+neomodel/sync_/core.py
+neomodel/sync_/match.py
+neomodel/sync_/path.py
+neomodel/sync_/property_manager.py
+neomodel/sync_/relationship.py
+neomodel/sync_/relationship_manager.py
 test/__init__.py
 test/conftest.py
-test/test_alias.py
-test/test_batch.py
-test/test_cardinality.py
-test/test_connection.py
-test/test_cypher.py
-test/test_database_management.py
-test/test_dbms_awareness.py
-test/test_driver_options.py
-test/test_exceptions.py
-test/test_hooks.py
-test/test_indexing.py
-test/test_issue112.py
-test/test_issue283.py
-test/test_issue600.py
-test/test_label_drop.py
-test/test_label_install.py
-test/test_match_api.py
-test/test_migration_neo4j_5.py
-test/test_models.py
-test/test_multiprocessing.py
-test/test_paths.py
-test/test_properties.py
-test/test_relationship_models.py
-test/test_relationships.py
-test/test_relative_relationships.py
 test/test_scripts.py
-test/test_transactions.py
-test/test_contrib/__init__.py
-test/test_contrib/test_semi_structured.py
-test/test_contrib/test_spatial_datatypes.py
-test/test_contrib/test_spatial_properties.py
+test/_async_compat/__init__.py
+test/_async_compat/mark_decorator.py
+test/async_/__init__.py
+test/async_/conftest.py
+test/async_/test_alias.py
+test/async_/test_batch.py
+test/async_/test_cardinality.py
+test/async_/test_connection.py
+test/async_/test_cypher.py
+test/async_/test_database_management.py
+test/async_/test_dbms_awareness.py
+test/async_/test_driver_options.py
+test/async_/test_exceptions.py
+test/async_/test_hooks.py
+test/async_/test_indexing.py
+test/async_/test_issue112.py
+test/async_/test_issue283.py
+test/async_/test_issue600.py
+test/async_/test_label_drop.py
+test/async_/test_label_install.py
+test/async_/test_match_api.py
+test/async_/test_migration_neo4j_5.py
+test/async_/test_models.py
+test/async_/test_multiprocessing.py
+test/async_/test_paths.py
+test/async_/test_properties.py
+test/async_/test_relationship_models.py
+test/async_/test_relationships.py
+test/async_/test_relative_relationships.py
+test/async_/test_transactions.py
+test/async_/test_contrib/__init__.py
+test/async_/test_contrib/test_semi_structured.py
+test/async_/test_contrib/test_spatial_datatypes.py
+test/async_/test_contrib/test_spatial_properties.py
+test/sync_/__init__.py
+test/sync_/conftest.py
+test/sync_/test_alias.py
+test/sync_/test_batch.py
+test/sync_/test_cardinality.py
+test/sync_/test_connection.py
+test/sync_/test_cypher.py
+test/sync_/test_database_management.py
+test/sync_/test_dbms_awareness.py
+test/sync_/test_driver_options.py
+test/sync_/test_exceptions.py
+test/sync_/test_hooks.py
+test/sync_/test_indexing.py
+test/sync_/test_issue112.py
+test/sync_/test_issue283.py
+test/sync_/test_issue600.py
+test/sync_/test_label_drop.py
+test/sync_/test_label_install.py
+test/sync_/test_match_api.py
+test/sync_/test_migration_neo4j_5.py
+test/sync_/test_models.py
+test/sync_/test_multiprocessing.py
+test/sync_/test_paths.py
+test/sync_/test_properties.py
+test/sync_/test_relationship_models.py
+test/sync_/test_relationships.py
+test/sync_/test_relative_relationships.py
+test/sync_/test_transactions.py
+test/sync_/test_contrib/__init__.py
+test/sync_/test_contrib/test_semi_structured.py
+test/sync_/test_contrib/test_spatial_datatypes.py
+test/sync_/test_contrib/test_spatial_properties.py
```

### Comparing `neomodel-5.2.1/pyproject.toml` & `neomodel-5.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 name = "neomodel"
 authors = [
     {name = "Robin Edwards", email = "robin.ge@gmail.com"},
 ]
 maintainers = [
     {name = "Marius Conjeaud", email = "marius.conjeaud@outlook.com"},
     {name = "Athanasios Anastasiou", email = "athanastasiou@gmail.com"},
-    {name = "Cristina Escalante"},
 ]
 description = "An object mapper for the neo4j graph database."
 readme = "README.md"
 keywords = ["graph", "neo4j", "ORM", "OGM", "mapper"]
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -19,27 +18,29 @@
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     'Topic :: Software Development :: Libraries :: Python Modules',
     "Programming Language :: Python :: 3",
     "Topic :: Database",
 ]
 dependencies = [
-    "neo4j~=5.15.0",
+    "neo4j~=5.19.0",
 ]
 requires-python = ">=3.7"
 dynamic = ["version"]
 
 [project.urls]
 documentation = "https://neomodel.readthedocs.io/en/latest/"
 repository = "http://github.com/neo4j-contrib/neomodel"
 changelog = "https://github.com/neo4j-contrib/neomodel/releases"
 
 [project.optional-dependencies]
 dev = [
+    "unasync",
     "pytest>=7.1",
+    "pytest-asyncio",
     "pytest-cov>=4.0",
     "pre-commit",
     "black",
     "isort",
     "Shapely>=2.0.0"
 ]
 pandas = ["pandas"]
@@ -57,15 +58,15 @@
 
 [tool.pytest.ini_options]
 addopts = "--resetdb"
 testpaths = "test"
 
 [tool.isort]
 profile = 'black'
-src_paths = ['neomodel']
+src_paths = ['neomodel','test']
 
 [tool.pylint.'MESSAGES CONTROL']
 disable = 'missing-module-docstring,redefined-builtin,missing-class-docstring,missing-function-docstring,consider-using-f-string,line-too-long'
 
 [tool.pylint.'BASIC']
 good-names = 'i,j,k,ex,_,e,fn,x,y,z,id,db,q'
```

### Comparing `neomodel-5.2.1/test/conftest.py` & `neomodel-5.3.0/test/async_/test_connection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,119 +1,148 @@
-from __future__ import print_function
-
 import os
-import warnings
+from test._async_compat import mark_async_test
+from test.conftest import NEO4J_PASSWORD, NEO4J_URL, NEO4J_USERNAME
 
 import pytest
+from neo4j import AsyncDriver, AsyncGraphDatabase
+from neo4j.debug import watch
+
+from neomodel import AsyncStructuredNode, StringProperty, adb, config
+
+
+@mark_async_test
+@pytest.fixture(autouse=True)
+async def setup_teardown():
+    yield
+    # Teardown actions after tests have run
+    # Reconnect to initial URL for potential subsequent tests
+    await adb.close_connection()
+    await adb.set_connection(url=config.DATABASE_URL)
 
-from neomodel import clear_neo4j_database, config, db
-from neomodel.util import version_tag_to_integer
 
-NEO4J_URL = os.environ.get("NEO4J_URL", "bolt://localhost:7687")
-NEO4J_USERNAME = os.environ.get("NEO4J_USERNAME", "neo4j")
-NEO4J_PASSWORD = os.environ.get("NEO4J_PASSWORD", "foobarbaz")
+@pytest.fixture(autouse=True, scope="session")
+def neo4j_logging():
+    with watch("neo4j"):
+        yield
 
 
-def pytest_addoption(parser):
+@mark_async_test
+async def get_current_database_name() -> str:
     """
-    Adds the command line option --resetdb.
+    Fetches the name of the currently active database from the Neo4j database.
 
-    :param parser: The parser object. Please see <https://docs.pytest.org/en/latest/reference.html#_pytest.hookspec.pytest_addoption>`_
-    :type Parser object: For more information please see <https://docs.pytest.org/en/latest/reference.html#_pytest.config.Parser>`_
+    Returns:
+    - str: The name of the current database.
     """
-    parser.addoption(
-        "--resetdb",
-        action="store_true",
-        help="Ensures that the database is clear prior to running tests for neomodel",
-        default=False,
-    )
+    results, meta = await adb.cypher_query("CALL db.info")
+    results_as_dict = [dict(zip(meta, row)) for row in results]
 
+    return results_as_dict[0]["name"]
 
-@pytest.hookimpl
-def pytest_collection_modifyitems(items):
-    connect_to_aura_items = []
-    normal_items = []
-
-    # Separate all tests into two groups: those with "connect_to_aura" in their name, and all others
-    for item in items:
-        if "connect_to_aura" in item.name:
-            connect_to_aura_items.append(item)
-        else:
-            normal_items.append(item)
-
-    # Add all normal tests back to the front of the list
-    new_order = normal_items
-
-    # Add all connect_to_aura tests to the end of the list
-    new_order.extend(connect_to_aura_items)
 
-    # Replace the original items list with the new order
-    items[:] = new_order
+class Pastry(AsyncStructuredNode):
+    name = StringProperty(unique_index=True)
 
 
-@pytest.hookimpl
-def pytest_sessionstart(session):
-    """
-    Provides initial connection to the database and sets up the rest of the test suite
+@mark_async_test
+async def test_set_connection_driver_works():
+    # Verify that current connection is up
+    assert await Pastry(name="Chocolatine").save()
+    await adb.close_connection()
 
-    :param session: The session object. Please see <https://docs.pytest.org/en/latest/reference.html#_pytest.hookspec.pytest_sessionstart>`_
-    :type Session object: For more information please see <https://docs.pytest.org/en/latest/reference.html#session>`_
-    """
+    # Test connection using a driver
+    await adb.set_connection(
+        driver=AsyncGraphDatabase().driver(
+            NEO4J_URL, auth=(NEO4J_USERNAME, NEO4J_PASSWORD)
+        )
+    )
+    assert await Pastry(name="Croissant").save()
 
-    warnings.simplefilter("default")
 
-    config.DATABASE_URL = os.environ.get(
-        "NEO4J_BOLT_URL", "bolt://neo4j:foobarbaz@localhost:7687"
+@mark_async_test
+async def test_config_driver_works():
+    # Verify that current connection is up
+    assert await Pastry(name="Chausson aux pommes").save()
+    await adb.close_connection()
+
+    # Test connection using a driver defined in config
+    driver: AsyncDriver = AsyncGraphDatabase().driver(
+        NEO4J_URL, auth=(NEO4J_USERNAME, NEO4J_PASSWORD)
     )
-    config.AUTO_INSTALL_LABELS = True
 
-    # Clear the database if required
-    database_is_populated, _ = db.cypher_query(
-        "MATCH (a) return count(a)>0 as database_is_populated"
-    )
-    if database_is_populated[0][0] and not session.config.getoption("resetdb"):
-        raise SystemError(
-            "Please note: The database seems to be populated.\n\tEither delete all nodes and edges manually, or set the --resetdb parameter when calling pytest\n\n\tpytest --resetdb."
-        )
-    else:
-        clear_neo4j_database(db, clear_constraints=True, clear_indexes=True)
+    config.DRIVER = driver
+    assert await Pastry(name="Grignette").save()
 
-    db.cypher_query(
-        "CREATE OR REPLACE USER troygreene SET PASSWORD 'foobarbaz' CHANGE NOT REQUIRED"
-    )
-    if db.database_edition == "enterprise":
-        db.cypher_query("GRANT ROLE publisher TO troygreene")
-        db.cypher_query("GRANT IMPERSONATE (troygreene) ON DBMS TO admin")
+    # Clear config
+    # No need to close connection - pytest teardown will do it
+    config.DRIVER = None
 
 
-@pytest.hookimpl
-def pytest_unconfigure():
-    db.close_connection()
+@mark_async_test
+async def test_connect_to_non_default_database():
+    if not await adb.edition_is_enterprise():
+        pytest.skip("Skipping test for community edition - no multi database in CE")
+    database_name = "pastries"
+    await adb.cypher_query(f"CREATE DATABASE {database_name} IF NOT EXISTS")
+    await adb.close_connection()
 
+    # Set database name in url - for url init only
+    await adb.set_connection(url=f"{config.DATABASE_URL}/{database_name}")
+    assert await get_current_database_name() == "pastries"
 
-def check_and_skip_neo4j_least_version(required_least_neo4j_version, message):
-    """
-    Checks if the NEO4J_VERSION is at least `required_least_neo4j_version` and skips a test if not.
+    await adb.close_connection()
 
-    WARNING: If the NEO4J_VERSION variable is not set, this function returns True, allowing the test to go ahead.
+    # Set database name in config - for both url and driver init
+    config.DATABASE_NAME = database_name
 
-    :param required_least_neo4j_version: The least version to check. This must be the numberic representation of the
-    version. That is: '3.4.0' would be passed as 340.
-    :type required_least_neo4j_version: int
-    :param message: An informative message as to why the calling test had to be skipped.
-    :type message: str
-    :return: A boolean value of True if the version reported is at least `required_least_neo4j_version`
-    """
-    if (
-        "NEO4J_VERSION" in os.environ
-        and version_tag_to_integer(os.environ["NEO4J_VERSION"])
-        < required_least_neo4j_version
-    ):
-        pytest.skip(
-            "Neo4j version: {}. {}."
-            "Skipping test.".format(os.environ["NEO4J_VERSION"], message)
+    # url init
+    await adb.set_connection(url=config.DATABASE_URL)
+    assert await get_current_database_name() == "pastries"
+
+    await adb.close_connection()
+
+    # driver init
+    await adb.set_connection(
+        driver=AsyncGraphDatabase().driver(
+            NEO4J_URL, auth=(NEO4J_USERNAME, NEO4J_PASSWORD)
         )
+    )
+    assert await get_current_database_name() == "pastries"
+
+    # Clear config
+    # No need to close connection - pytest teardown will do it
+    config.DATABASE_NAME = None
+
+
+@mark_async_test
+@pytest.mark.parametrize(
+    "url", ["bolt://user:password", "http://user:password@localhost:7687"]
+)
+async def test_wrong_url_format(url):
+    with pytest.raises(
+        ValueError,
+        match=rf"Expecting url format: bolt://user:password@localhost:7687 got {url}",
+    ):
+        await adb.set_connection(url=url)
+
+
+@mark_async_test
+@pytest.mark.parametrize("protocol", ["neo4j+s", "neo4j+ssc", "bolt+s", "bolt+ssc"])
+async def test_connect_to_aura(protocol):
+    cypher_return = "hello world"
+    default_cypher_query = f"RETURN '{cypher_return}'"
+    await adb.close_connection()
+
+    await _set_connection(protocol=protocol)
+    result, _ = await adb.cypher_query(default_cypher_query)
+
+    assert len(result) > 0
+    assert result[0][0] == cypher_return
+
 
+async def _set_connection(protocol):
+    AURA_TEST_DB_USER = os.environ["AURA_TEST_DB_USER"]
+    AURA_TEST_DB_PASSWORD = os.environ["AURA_TEST_DB_PASSWORD"]
+    AURA_TEST_DB_HOSTNAME = os.environ["AURA_TEST_DB_HOSTNAME"]
 
-@pytest.fixture
-def skip_neo4j_before_330():
-    check_and_skip_neo4j_least_version(330, "Neo4J version does not support this test")
+    database_url = f"{protocol}://{AURA_TEST_DB_USER}:{AURA_TEST_DB_PASSWORD}@{AURA_TEST_DB_HOSTNAME}"
+    await adb.set_connection(url=database_url)
```

### Comparing `neomodel-5.2.1/test/test_alias.py` & `neomodel-5.3.0/test/sync_/test_alias.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,31 @@
+from test._async_compat import mark_sync_test
+
 from neomodel import AliasProperty, StringProperty, StructuredNode
 
 
 class MagicProperty(AliasProperty):
     def setup(self):
         self.owner.setup_hook_called = True
 
 
 class AliasTestNode(StructuredNode):
     name = StringProperty(unique_index=True)
     full_name = AliasProperty(to="name")
     long_name = MagicProperty(to="name")
 
 
+@mark_sync_test
 def test_property_setup_hook():
-    tim = AliasTestNode(long_name="tim").save()
+    timmy = AliasTestNode(long_name="timmy").save()
     assert AliasTestNode.setup_hook_called
-    assert tim.name == "tim"
+    assert timmy.name == "timmy"
 
 
+@mark_sync_test
 def test_alias():
     jim = AliasTestNode(full_name="Jim").save()
     assert jim.name == "Jim"
     assert jim.full_name == "Jim"
     assert "full_name" not in AliasTestNode.deflate(jim.__properties__)
     jim = AliasTestNode.nodes.get(full_name="Jim")
     assert jim
```

### Comparing `neomodel-5.2.1/test/test_batch.py` & `neomodel-5.3.0/test/sync_/test_batch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+from test._async_compat import mark_sync_test
+
 from pytest import raises
 
 from neomodel import (
     IntegerProperty,
     RelationshipFrom,
     RelationshipTo,
     StringProperty,
     StructuredNode,
     UniqueIdProperty,
     config,
 )
+from neomodel._async_compat.util import Util
 from neomodel.exceptions import DeflateError, UniqueProperty
 
 config.AUTO_INSTALL_LABELS = True
 
 
 class UniqueUser(StructuredNode):
     uid = UniqueIdProperty()
     name = StringProperty()
     age = IntegerProperty()
 
 
+@mark_sync_test
 def test_unique_id_property_batch():
     users = UniqueUser.create({"name": "bob", "age": 2}, {"name": "ben", "age": 3})
 
     assert users[0].uid != users[1].uid
 
     users = UniqueUser.get_or_create({"uid": users[0].uid}, {"name": "bill", "age": 4})
 
@@ -32,14 +36,15 @@
 
 
 class Customer(StructuredNode):
     email = StringProperty(unique_index=True, required=True)
     age = IntegerProperty(index=True)
 
 
+@mark_sync_test
 def test_batch_create():
     users = Customer.create(
         {"email": "jim1@aol.com", "age": 11},
         {"email": "jim2@aol.com", "age": 7},
         {"email": "jim3@aol.com", "age": 9},
         {"email": "jim4@aol.com", "age": 7},
         {"email": "jim5@aol.com", "age": 99},
@@ -47,72 +52,83 @@
     assert len(users) == 5
     assert users[0].age == 11
     assert users[1].age == 7
     assert users[1].email == "jim2@aol.com"
     assert Customer.nodes.get(email="jim1@aol.com")
 
 
+@mark_sync_test
 def test_batch_create_or_update():
     users = Customer.create_or_update(
         {"email": "merge1@aol.com", "age": 11},
         {"email": "merge2@aol.com"},
         {"email": "merge3@aol.com", "age": 1},
         {"email": "merge2@aol.com", "age": 2},
     )
     assert len(users) == 4
     assert users[1] == users[3]
-    assert Customer.nodes.get(email="merge1@aol.com").age == 11
+    merge_1: Customer = Customer.nodes.get(email="merge1@aol.com")
+    assert merge_1.age == 11
 
     more_users = Customer.create_or_update(
         {"email": "merge1@aol.com", "age": 22},
         {"email": "merge4@aol.com", "age": None},
     )
     assert len(more_users) == 2
     assert users[0] == more_users[0]
-    assert Customer.nodes.get(email="merge1@aol.com").age == 22
+    merge_1 = Customer.nodes.get(email="merge1@aol.com")
+    assert merge_1.age == 22
 
 
+@mark_sync_test
 def test_batch_validation():
     # test validation in batch create
     with raises(DeflateError):
         Customer.create(
             {"email": "jim1@aol.com", "age": "x"},
         )
 
 
+@mark_sync_test
 def test_batch_index_violation():
-    for u in Customer.nodes.all():
+    for u in Customer.nodes:
         u.delete()
 
     users = Customer.create(
         {"email": "jim6@aol.com", "age": 3},
     )
     assert users
     with raises(UniqueProperty):
         Customer.create(
             {"email": "jim6@aol.com", "age": 3},
             {"email": "jim7@aol.com", "age": 5},
         )
 
     # not found
-    assert not Customer.nodes.filter(email="jim7@aol.com")
+    if Util.is_async_code:
+        assert not Customer.nodes.filter(email="jim7@aol.com").__bool__()
+    else:
+        assert not Customer.nodes.filter(email="jim7@aol.com")
 
 
 class Dog(StructuredNode):
     name = StringProperty(required=True)
     owner = RelationshipTo("Person", "owner")
 
 
 class Person(StructuredNode):
     name = StringProperty(unique_index=True)
     pets = RelationshipFrom("Dog", "owner")
 
 
+@mark_sync_test
 def test_get_or_create_with_rel():
-    bob = Person.get_or_create({"name": "Bob"})[0]
+    create_bob = Person.get_or_create({"name": "Bob"})
+    bob = create_bob[0]
     bobs_gizmo = Dog.get_or_create({"name": "Gizmo"}, relationship=bob.pets)
 
-    tim = Person.get_or_create({"name": "Tim"})[0]
+    create_tim = Person.get_or_create({"name": "Tim"})
+    tim = create_tim[0]
     tims_gizmo = Dog.get_or_create({"name": "Gizmo"}, relationship=tim.pets)
 
     # not the same gizmo
     assert bobs_gizmo[0] != tims_gizmo[0]
```

### Comparing `neomodel-5.2.1/test/test_cardinality.py` & `neomodel-5.3.0/test/sync_/test_cardinality.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from test._async_compat import mark_sync_test
+
 from pytest import raises
 
 from neomodel import (
     AttemptedCardinalityViolation,
     CardinalityViolation,
     IntegerProperty,
     One,
@@ -35,52 +37,61 @@
     toothbrush = RelationshipTo("ToothBrush", "HAS_TOOTHBRUSH", cardinality=One)
 
 
 class ToothBrush(StructuredNode):
     name = StringProperty()
 
 
+@mark_sync_test
 def test_cardinality_zero_or_more():
     m = Monkey(name="tim").save()
     assert m.dryers.all() == []
-    assert m.dryers.single() is None
+    single_dryer = m.driver.single()
+    assert single_dryer is None
     h = HairDryer(version=1).save()
 
     m.dryers.connect(h)
     assert len(m.dryers.all()) == 1
-    assert m.dryers.single().version == 1
+    single_dryer = m.dryers.single()
+    assert single_dryer.version == 1
 
     m.dryers.disconnect(h)
     assert m.dryers.all() == []
-    assert m.dryers.single() is None
+    single_dryer = m.driver.single()
+    assert single_dryer is None
 
     h2 = HairDryer(version=2).save()
     m.dryers.connect(h)
     m.dryers.connect(h2)
     m.dryers.disconnect_all()
     assert m.dryers.all() == []
-    assert m.dryers.single() is None
+    single_dryer = m.driver.single()
+    assert single_dryer is None
 
 
+@mark_sync_test
 def test_cardinality_zero_or_one():
     m = Monkey(name="bob").save()
     assert m.driver.all() == []
+    single_driver = m.driver.single()
     assert m.driver.single() is None
     h = ScrewDriver(version=1).save()
 
     m.driver.connect(h)
     assert len(m.driver.all()) == 1
-    assert m.driver.single().version == 1
+    single_driver = m.driver.single()
+    assert single_driver.version == 1
 
     j = ScrewDriver(version=2).save()
     with raises(AttemptedCardinalityViolation):
         m.driver.connect(j)
 
     m.driver.reconnect(h, j)
-    assert m.driver.single().version == 2
+    single_driver = m.driver.single()
+    assert single_driver.version == 2
 
     # Forcing creation of a second ToothBrush to go around
     # AttemptedCardinalityViolation
     db.cypher_query(
         """
         MATCH (m:Monkey WHERE m.name="bob")
         CREATE (s:ScrewDriver {version:3})
@@ -90,26 +101,28 @@
     )
     with raises(
         CardinalityViolation, match=r"CardinalityViolation: Expected: .*, got: 2."
     ):
         m.driver.all()
 
 
+@mark_sync_test
 def test_cardinality_one_or_more():
     m = Monkey(name="jerry").save()
 
     with raises(CardinalityViolation):
         m.car.all()
 
     with raises(CardinalityViolation):
         m.car.single()
 
     c = Car(version=2).save()
     m.car.connect(c)
-    assert m.car.single().version == 2
+    single_car = m.car.single()
+    assert single_car.version == 2
 
     cars = m.car.all()
     assert len(cars) == 1
 
     with raises(AttemptedCardinalityViolation):
         m.car.disconnect(c)
 
@@ -119,30 +132,32 @@
     assert len(cars) == 2
 
     m.car.disconnect(d)
     cars = m.car.all()
     assert len(cars) == 1
 
 
+@mark_sync_test
 def test_cardinality_one():
     m = Monkey(name="jerry").save()
 
     with raises(
         CardinalityViolation, match=r"CardinalityViolation: Expected: .*, got: none."
     ):
         m.toothbrush.all()
 
     with raises(CardinalityViolation):
         m.toothbrush.single()
 
     b = ToothBrush(name="Jim").save()
     m.toothbrush.connect(b)
-    assert m.toothbrush.single().name == "Jim"
+    single_toothbrush = m.toothbrush.single()
+    assert single_toothbrush.name == "Jim"
 
-    x = ToothBrush(name="Jim").save
+    x = ToothBrush(name="Jim").save()
     with raises(AttemptedCardinalityViolation):
         m.toothbrush.connect(x)
 
     with raises(AttemptedCardinalityViolation):
         m.toothbrush.disconnect(b)
 
     with raises(AttemptedCardinalityViolation):
```

### Comparing `neomodel-5.2.1/test/test_connection.py` & `neomodel-5.3.0/test/sync_/test_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
-import time
+from test._async_compat import mark_sync_test
+from test.conftest import NEO4J_PASSWORD, NEO4J_URL, NEO4J_USERNAME
 
 import pytest
-from neo4j import GraphDatabase
+from neo4j import Driver, GraphDatabase
 from neo4j.debug import watch
 
 from neomodel import StringProperty, StructuredNode, config, db
 
-from .conftest import NEO4J_PASSWORD, NEO4J_URL, NEO4J_USERNAME
-
 
+@mark_sync_test
 @pytest.fixture(autouse=True)
 def setup_teardown():
     yield
     # Teardown actions after tests have run
     # Reconnect to initial URL for potential subsequent tests
     db.close_connection()
     db.set_connection(url=config.DATABASE_URL)
@@ -21,14 +21,15 @@
 
 @pytest.fixture(autouse=True, scope="session")
 def neo4j_logging():
     with watch("neo4j"):
         yield
 
 
+@mark_sync_test
 def get_current_database_name() -> str:
     """
     Fetches the name of the currently active database from the Neo4j database.
 
     Returns:
     - str: The name of the current database.
     """
@@ -38,47 +39,50 @@
     return results_as_dict[0]["name"]
 
 
 class Pastry(StructuredNode):
     name = StringProperty(unique_index=True)
 
 
+@mark_sync_test
 def test_set_connection_driver_works():
     # Verify that current connection is up
     assert Pastry(name="Chocolatine").save()
     db.close_connection()
 
     # Test connection using a driver
     db.set_connection(
         driver=GraphDatabase().driver(NEO4J_URL, auth=(NEO4J_USERNAME, NEO4J_PASSWORD))
     )
     assert Pastry(name="Croissant").save()
 
 
+@mark_sync_test
 def test_config_driver_works():
     # Verify that current connection is up
     assert Pastry(name="Chausson aux pommes").save()
     db.close_connection()
 
     # Test connection using a driver defined in config
-    driver = GraphDatabase().driver(NEO4J_URL, auth=(NEO4J_USERNAME, NEO4J_PASSWORD))
+    driver: Driver = GraphDatabase().driver(
+        NEO4J_URL, auth=(NEO4J_USERNAME, NEO4J_PASSWORD)
+    )
 
     config.DRIVER = driver
     assert Pastry(name="Grignette").save()
 
     # Clear config
     # No need to close connection - pytest teardown will do it
     config.DRIVER = None
 
 
-@pytest.mark.skipif(
-    db.database_edition != "enterprise",
-    reason="Skipping test for community edition - no multi database in CE",
-)
+@mark_sync_test
 def test_connect_to_non_default_database():
+    if not db.edition_is_enterprise():
+        pytest.skip("Skipping test for community edition - no multi database in CE")
     database_name = "pastries"
     db.cypher_query(f"CREATE DATABASE {database_name} IF NOT EXISTS")
     db.close_connection()
 
     # Set database name in url - for url init only
     db.set_connection(url=f"{config.DATABASE_URL}/{database_name}")
     assert get_current_database_name() == "pastries"
@@ -101,25 +105,27 @@
     assert get_current_database_name() == "pastries"
 
     # Clear config
     # No need to close connection - pytest teardown will do it
     config.DATABASE_NAME = None
 
 
+@mark_sync_test
 @pytest.mark.parametrize(
     "url", ["bolt://user:password", "http://user:password@localhost:7687"]
 )
 def test_wrong_url_format(url):
     with pytest.raises(
         ValueError,
         match=rf"Expecting url format: bolt://user:password@localhost:7687 got {url}",
     ):
         db.set_connection(url=url)
 
 
+@mark_sync_test
 @pytest.mark.parametrize("protocol", ["neo4j+s", "neo4j+ssc", "bolt+s", "bolt+ssc"])
 def test_connect_to_aura(protocol):
     cypher_return = "hello world"
     default_cypher_query = f"RETURN '{cypher_return}'"
     db.close_connection()
 
     _set_connection(protocol=protocol)
```

### Comparing `neomodel-5.2.1/test/test_contrib/test_spatial_datatypes.py` & `neomodel-5.3.0/test/async_/test_contrib/test_spatial_datatypes.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.2.1/test/test_contrib/test_spatial_properties.py` & `neomodel-5.3.0/test/async_/test_contrib/test_spatial_properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Provides a test case for issue 374 - "Support for Point property type".
 
 For more information please see: https://github.com/neo4j-contrib/neomodel/issues/374
 """
 
-import os
 import random
+from test._async_compat import mark_async_test
 
 import neo4j.spatial
 import pytest
 
 import neomodel
 import neomodel.contrib.spatial_properties
 
@@ -152,26 +152,27 @@
             expected_point,
             deflated_point,
             "{}, received {}".format(a_value[1], deflated_point),
             check_neo4j_points=True,
         )
 
 
-def test_default_value():
+@mark_async_test
+async def test_default_value():
     """
     Tests that the default value passing mechanism works as expected with NeomodelPoint values.
     :return:
     """
 
     def get_some_point():
         return neomodel.contrib.spatial_properties.NeomodelPoint(
             (random.random(), random.random())
         )
 
-    class LocalisableEntity(neomodel.StructuredNode):
+    class LocalisableEntity(neomodel.AsyncStructuredNode):
         """
         A very simple entity to try out the default value assignment.
         """
 
         identifier = neomodel.UniqueIdProperty()
         location = neomodel.contrib.spatial_properties.PointProperty(
             crs="cartesian", default=get_some_point
@@ -179,104 +180,112 @@
 
     # Neo4j versions lower than 3.4.0 do not support Point. In that case, skip the test.
     check_and_skip_neo4j_least_version(
         340, "This version does not support spatial data types."
     )
 
     # Save an object
-    an_object = LocalisableEntity().save()
+    an_object = await LocalisableEntity().save()
     coords = an_object.location.coords[0]
     # Retrieve it
-    retrieved_object = LocalisableEntity.nodes.get(identifier=an_object.identifier)
+    retrieved_object = await LocalisableEntity.nodes.get(
+        identifier=an_object.identifier
+    )
     # Check against an independently created value
     assert (
         retrieved_object.location
         == neomodel.contrib.spatial_properties.NeomodelPoint(coords)
     ), ("Default value assignment failed.")
 
 
-def test_array_of_points():
+@mark_async_test
+async def test_array_of_points():
     """
     Tests that Arrays of Points work as expected.
 
     :return:
     """
 
-    class AnotherLocalisableEntity(neomodel.StructuredNode):
+    class AnotherLocalisableEntity(neomodel.AsyncStructuredNode):
         """
         A very simple entity with an array of locations
         """
 
         identifier = neomodel.UniqueIdProperty()
         locations = neomodel.ArrayProperty(
             neomodel.contrib.spatial_properties.PointProperty(crs="cartesian")
         )
 
     # Neo4j versions lower than 3.4.0 do not support Point. In that case, skip the test.
     check_and_skip_neo4j_least_version(
         340, "This version does not support spatial data types."
     )
 
-    an_object = AnotherLocalisableEntity(
+    an_object = await AnotherLocalisableEntity(
         locations=[
             neomodel.contrib.spatial_properties.NeomodelPoint((0.0, 0.0)),
             neomodel.contrib.spatial_properties.NeomodelPoint((1.0, 0.0)),
         ]
     ).save()
 
-    retrieved_object = AnotherLocalisableEntity.nodes.get(
+    retrieved_object = await AnotherLocalisableEntity.nodes.get(
         identifier=an_object.identifier
     )
 
     assert (
         type(retrieved_object.locations) is list
     ), "Array of Points definition failed."
     assert retrieved_object.locations == [
         neomodel.contrib.spatial_properties.NeomodelPoint((0.0, 0.0)),
         neomodel.contrib.spatial_properties.NeomodelPoint((1.0, 0.0)),
     ], "Array of Points incorrect values."
 
 
-def test_simple_storage_retrieval():
+@mark_async_test
+async def test_simple_storage_retrieval():
     """
     Performs a simple Create, Retrieve via .save(), .get() which, due to the way Q objects operate, tests the
     __copy__, __deepcopy__ operations of NeomodelPoint.
     :return:
     """
 
-    class TestStorageRetrievalProperty(neomodel.StructuredNode):
+    class TestStorageRetrievalProperty(neomodel.AsyncStructuredNode):
         uid = neomodel.UniqueIdProperty()
         description = neomodel.StringProperty()
         location = neomodel.contrib.spatial_properties.PointProperty(crs="cartesian")
 
     # Neo4j versions lower than 3.4.0 do not support Point. In that case, skip the test.
     check_and_skip_neo4j_least_version(
         340, "This version does not support spatial data types."
     )
 
-    a_restaurant = TestStorageRetrievalProperty(
+    a_restaurant = await TestStorageRetrievalProperty(
         description="Milliways",
         location=neomodel.contrib.spatial_properties.NeomodelPoint((0, 0)),
     ).save()
 
-    a_property = TestStorageRetrievalProperty.nodes.get(
+    a_property = await TestStorageRetrievalProperty.nodes.get(
         location=neomodel.contrib.spatial_properties.NeomodelPoint((0, 0))
     )
 
     assert a_restaurant.description == a_property.description
 
+
 def test_equality_with_other_objects():
     """
     Performs equality tests and ensures tha ``NeomodelPoint`` can be compared with ShapelyPoint and NeomodelPoint only.
     """
     try:
         import shapely.geometry
         from shapely import __version__
     except ImportError:
         pytest.skip("Shapely module not present")
 
     if int("".join(__version__.split(".")[0:3])) < 200:
         pytest.skip(f"Shapely 2.0 not present (Current version is {__version__}")
 
-    assert neomodel.contrib.spatial_properties.NeomodelPoint((0,0)) == neomodel.contrib.spatial_properties.NeomodelPoint(x=0, y=0)
-    assert neomodel.contrib.spatial_properties.NeomodelPoint((0,0)) == shapely.geometry.Point((0,0))
-
+    assert neomodel.contrib.spatial_properties.NeomodelPoint(
+        (0, 0)
+    ) == neomodel.contrib.spatial_properties.NeomodelPoint(x=0, y=0)
+    assert neomodel.contrib.spatial_properties.NeomodelPoint(
+        (0, 0)
+    ) == shapely.geometry.Point((0, 0))
```

### Comparing `neomodel-5.2.1/test/test_cypher.py` & `neomodel-5.3.0/test/sync_/test_cypher.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import builtins
+from test._async_compat import mark_sync_test
 
 import pytest
 from neo4j.exceptions import ClientError as CypherError
 from numpy import ndarray
 from pandas import DataFrame, Series
 
-from neomodel import StringProperty, StructuredNode
-from neomodel.core import db
+from neomodel import StringProperty, StructuredNode, db
+from neomodel._async_compat.util import Util
 
 
 class User2(StructuredNode):
     name = StringProperty()
     email = StringProperty()
 
 
@@ -32,14 +33,15 @@
         if name == request.param:
             raise ImportError()
         return import_orig(name, *args, **kwargs)
 
     monkeypatch.setattr(builtins, "__import__", mocked_import)
 
 
+@mark_sync_test
 def test_cypher():
     """
     test result format is backward compatible with earlier versions of neomodel
     """
 
     jim = User2(email="jim1@test.com").save()
     data, meta = jim.cypher(
@@ -54,87 +56,110 @@
             MATCH (a)<-[:USER2]-(b)
             RETURN a, b, 3
         """
     )
     assert "a" in meta and "b" in meta
 
 
+@mark_sync_test
 def test_cypher_syntax_error():
     jim = User2(email="jim1@test.com").save()
     try:
         jim.cypher(f"MATCH a WHERE {db.get_id_method()}(a)={{self}} RETURN xx")
     except CypherError as e:
         assert hasattr(e, "message")
         assert hasattr(e, "code")
     else:
         assert False, "CypherError not raised."
 
 
+@mark_sync_test
 @pytest.mark.parametrize("hide_available_pkg", ["pandas"], indirect=True)
 def test_pandas_not_installed(hide_available_pkg):
+    # We run only the async version, because this fails on second run
+    # because import error is thrown only when pandas.py is imported
+    if not Util.is_async_code:
+        pytest.skip("This test is only")
     with pytest.raises(ImportError):
         with pytest.warns(
             UserWarning,
             match="The neomodel.integration.pandas module expects pandas to be installed",
         ):
             from neomodel.integration.pandas import to_dataframe
 
             _ = to_dataframe(db.cypher_query("MATCH (a) RETURN a.name AS name"))
 
 
+@mark_sync_test
 def test_pandas_integration():
     from neomodel.integration.pandas import to_dataframe, to_series
 
     jimla = UserPandas(email="jimla@test.com", name="jimla").save()
     jimlo = UserPandas(email="jimlo@test.com", name="jimlo").save()
 
     # Test to_dataframe
     df = to_dataframe(
-        db.cypher_query("MATCH (a:UserPandas) RETURN a.name AS name, a.email AS email")
+        db.cypher_query(
+            "MATCH (a:UserPandas) RETURN a.name AS name, a.email AS email ORDER BY name"
+        )
     )
 
     assert isinstance(df, DataFrame)
     assert df.shape == (2, 2)
     assert df["name"].tolist() == ["jimla", "jimlo"]
 
     # Also test passing an index and dtype to to_dataframe
     df = to_dataframe(
-        db.cypher_query("MATCH (a:UserPandas) RETURN a.name AS name, a.email AS email"),
+        db.cypher_query(
+            "MATCH (a:UserPandas) RETURN a.name AS name, a.email AS email ORDER BY name"
+        ),
         index=df["email"],
         dtype=str,
     )
 
     assert df.index.inferred_type == "string"
 
     # Next test to_series
-    series = to_series(db.cypher_query("MATCH (a:UserPandas) RETURN a.name AS name"))
+    series = to_series(
+        db.cypher_query("MATCH (a:UserPandas) RETURN a.name AS name ORDER BY name")
+    )
 
     assert isinstance(series, Series)
     assert series.shape == (2,)
     assert df["name"].tolist() == ["jimla", "jimlo"]
 
 
+@mark_sync_test
 @pytest.mark.parametrize("hide_available_pkg", ["numpy"], indirect=True)
 def test_numpy_not_installed(hide_available_pkg):
+    # We run only the async version, because this fails on second run
+    # because import error is thrown only when numpy.py is imported
+    if not Util.is_async_code:
+        pytest.skip("This test is only")
     with pytest.raises(ImportError):
         with pytest.warns(
             UserWarning,
-            match="The neomodel.integration.numpy module expects pandas to be installed",
+            match="The neomodel.integration.numpy module expects numpy to be installed",
         ):
             from neomodel.integration.numpy import to_ndarray
 
-            _ = to_ndarray(db.cypher_query("MATCH (a) RETURN a.name AS name"))
+            _ = to_ndarray(
+                db.cypher_query("MATCH (a) RETURN a.name AS name ORDER BY name")
+            )
 
 
+@mark_sync_test
 def test_numpy_integration():
     from neomodel.integration.numpy import to_ndarray
 
     jimly = UserNP(email="jimly@test.com", name="jimly").save()
     jimlu = UserNP(email="jimlu@test.com", name="jimlu").save()
 
     array = to_ndarray(
-        db.cypher_query("MATCH (a:UserNP) RETURN a.name AS name, a.email AS email")
+        db.cypher_query(
+            "MATCH (a:UserNP) RETURN a.name AS name, a.email AS email ORDER BY name"
+        )
     )
 
     assert isinstance(array, ndarray)
     assert array.shape == (2, 2)
-    assert array[0][0] == "jimly"
+    assert array[0][0] == "jimlu"
```

### Comparing `neomodel-5.2.1/test/test_database_management.py` & `neomodel-5.3.0/test/sync_/test_database_management.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from test._async_compat import mark_sync_test
+
 import pytest
 from neo4j.exceptions import AuthError
 
 from neomodel import (
     IntegerProperty,
     RelationshipTo,
     StringProperty,
     StructuredNode,
     StructuredRel,
     db,
-    util,
 )
 
 
 class City(StructuredNode):
     name = StringProperty()
 
 
@@ -22,56 +23,59 @@
 
 class Venue(StructuredNode):
     name = StringProperty(unique_index=True)
     creator = StringProperty(index=True)
     in_city = RelationshipTo(City, relation_type="IN", model=InCity)
 
 
+@mark_sync_test
 def test_clear_database():
     venue = Venue(name="Royal Albert Hall", creator="Queen Victoria").save()
     city = City(name="London").save()
     venue.in_city.connect(city)
 
     # Clear only the data
-    util.clear_neo4j_database(db)
+    db.clear_neo4j_database()
     database_is_populated, _ = db.cypher_query(
         "MATCH (a) return count(a)>0 as database_is_populated"
     )
 
     assert database_is_populated[0][0] is False
 
+    db.install_all_labels()
     indexes = db.list_indexes(exclude_token_lookup=True)
     constraints = db.list_constraints()
     assert len(indexes) > 0
     assert len(constraints) > 0
 
     # Clear constraints and indexes too
-    util.clear_neo4j_database(db, clear_constraints=True, clear_indexes=True)
+    db.clear_neo4j_database(clear_constraints=True, clear_indexes=True)
 
     indexes = db.list_indexes(exclude_token_lookup=True)
     constraints = db.list_constraints()
     assert len(indexes) == 0
     assert len(constraints) == 0
 
 
+@mark_sync_test
 def test_change_password():
     prev_password = "foobarbaz"
     new_password = "newpassword"
     prev_url = f"bolt://neo4j:{prev_password}@localhost:7687"
     new_url = f"bolt://neo4j:{new_password}@localhost:7687"
 
-    util.change_neo4j_password(db, "neo4j", new_password)
+    db.change_neo4j_password("neo4j", new_password)
     db.close_connection()
 
     db.set_connection(url=new_url)
     db.close_connection()
 
     with pytest.raises(AuthError):
         db.set_connection(url=prev_url)
 
     db.close_connection()
 
     db.set_connection(url=new_url)
-    util.change_neo4j_password(db, "neo4j", prev_password)
+    db.change_neo4j_password("neo4j", prev_password)
     db.close_connection()
 
     db.set_connection(url=prev_url)
```

### Comparing `neomodel-5.2.1/test/test_dbms_awareness.py` & `neomodel-5.3.0/test/sync_/test_dbms_awareness.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-from pytest import mark
+from test._async_compat import mark_sync_test
+
+import pytest
 
 from neomodel import db
 from neomodel.util import version_tag_to_integer
 
 
-@mark.skipif(
-    db.database_version != "5.7.0", reason="Testing a specific database version"
-)
+@mark_sync_test
 def test_version_awareness():
-    assert db.database_version == "5.7.0"
+    db_version = db.database_version
+    if db_version != "5.7.0":
+        pytest.skip("Testing a specific database version")
+    assert db_version == "5.7.0"
     assert db.version_is_higher_than("5.7")
     assert db.version_is_higher_than("5.6.0")
     assert db.version_is_higher_than("5")
     assert db.version_is_higher_than("4")
 
     assert not db.version_is_higher_than("5.8")
 
 
+@mark_sync_test
 def test_edition_awareness():
-    if db.database_edition == "enterprise":
+    db_edition = db.database_edition
+    if db_edition == "enterprise":
         assert db.edition_is_enterprise()
     else:
         assert not db.edition_is_enterprise()
 
 
 def test_version_tag_to_integer():
     assert version_tag_to_integer("5.7.1") == 50701
```

### Comparing `neomodel-5.2.1/test/test_driver_options.py` & `neomodel-5.3.0/test/sync_/test_driver_options.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,52 @@
+from test._async_compat import mark_sync_test
+
 import pytest
 from neo4j.exceptions import ClientError
 from pytest import raises
 
 from neomodel import db
 from neomodel.exceptions import FeatureNotSupported
 
 
-@pytest.mark.skipif(
-    not db.edition_is_enterprise(), reason="Skipping test for community edition"
-)
+@mark_sync_test
 def test_impersonate():
+    if not db.edition_is_enterprise():
+        pytest.skip("Skipping test for community edition")
     with db.impersonate(user="troygreene"):
         results, _ = db.cypher_query("RETURN 'Doo Wacko !'")
         assert results[0][0] == "Doo Wacko !"
 
 
-@pytest.mark.skipif(
-    not db.edition_is_enterprise(), reason="Skipping test for community edition"
-)
+@mark_sync_test
 def test_impersonate_unauthorized():
+    if not db.edition_is_enterprise():
+        pytest.skip("Skipping test for community edition")
     with db.impersonate(user="unknownuser"):
         with raises(ClientError):
             _ = db.cypher_query("RETURN 'Gabagool'")
 
 
-@pytest.mark.skipif(
-    not db.edition_is_enterprise(), reason="Skipping test for community edition"
-)
+@mark_sync_test
 def test_impersonate_multiple_transactions():
+    if not db.edition_is_enterprise():
+        pytest.skip("Skipping test for community edition")
     with db.impersonate(user="troygreene"):
         with db.transaction:
             results, _ = db.cypher_query("RETURN 'Doo Wacko !'")
             assert results[0][0] == "Doo Wacko !"
 
         with db.transaction:
             results, _ = db.cypher_query("SHOW CURRENT USER")
             assert results[0][0] == "troygreene"
 
     results, _ = db.cypher_query("SHOW CURRENT USER")
     assert results[0][0] == "neo4j"
 
 
-@pytest.mark.skipif(
-    db.edition_is_enterprise(), reason="Skipping test for enterprise edition"
-)
+@mark_sync_test
 def test_impersonate_community():
+    if db.edition_is_enterprise():
+        pytest.skip("Skipping test for enterprise edition")
     with raises(FeatureNotSupported):
         with db.impersonate(user="troygreene"):
             _ = db.cypher_query("RETURN 'Gabagoogoo'")
```

### Comparing `neomodel-5.2.1/test/test_exceptions.py` & `neomodel-5.3.0/test/async_/test_exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import pickle
+from test._async_compat import mark_async_test
 
-from neomodel import DoesNotExist, StringProperty, StructuredNode
+from neomodel import AsyncStructuredNode, DoesNotExist, StringProperty
 
 
-class EPerson(StructuredNode):
+class EPerson(AsyncStructuredNode):
     name = StringProperty(unique_index=True)
 
 
-def test_object_does_not_exist():
+@mark_async_test
+async def test_object_does_not_exist():
     try:
-        EPerson.nodes.get(name="johnny")
+        await EPerson.nodes.get(name="johnny")
     except EPerson.DoesNotExist as e:
         pickle_instance = pickle.dumps(e)
         assert pickle_instance
         assert pickle.loads(pickle_instance)
         assert isinstance(pickle.loads(pickle_instance), DoesNotExist)
     else:
         assert False, "Person.DoesNotExist not raised."
```

### Comparing `neomodel-5.2.1/test/test_hooks.py` & `neomodel-5.3.0/test/sync_/test_hooks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from test._async_compat import mark_sync_test
+
 from neomodel import StringProperty, StructuredNode
 
 HOOKS_CALLED = {}
 
 
 class HookTest(StructuredNode):
     name = StringProperty()
@@ -18,14 +20,15 @@
     def pre_delete(self):
         HOOKS_CALLED["pre_delete"] = 1
 
     def post_delete(self):
         HOOKS_CALLED["post_delete"] = 1
 
 
+@mark_sync_test
 def test_hooks():
     ht = HookTest(name="k").save()
     ht.delete()
     assert "pre_save" in HOOKS_CALLED
     assert "post_save" in HOOKS_CALLED
     assert "post_create" in HOOKS_CALLED
     assert "pre_delete" in HOOKS_CALLED
```

### Comparing `neomodel-5.2.1/test/test_indexing.py` & `neomodel-5.3.0/test/sync_/test_indexing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,75 @@
+from test._async_compat import mark_sync_test
+
 import pytest
 from pytest import raises
 
-from neomodel import (
-    IntegerProperty,
-    StringProperty,
-    StructuredNode,
-    UniqueProperty,
-    install_labels,
-)
-from neomodel.core import db
+from neomodel import IntegerProperty, StringProperty, StructuredNode, UniqueProperty, db
 from neomodel.exceptions import ConstraintValidationFailed
 
 
 class Human(StructuredNode):
     name = StringProperty(unique_index=True)
     age = IntegerProperty(index=True)
 
 
+@mark_sync_test
 def test_unique_error():
-    install_labels(Human)
+    db.install_labels(Human)
     Human(name="j1m", age=13).save()
     try:
         Human(name="j1m", age=14).save()
     except UniqueProperty as e:
         assert str(e).find("j1m")
         assert str(e).find("name")
     else:
         assert False, "UniqueProperty not raised."
 
 
-@pytest.mark.skipif(
-    not db.edition_is_enterprise(), reason="Skipping test for community edition"
-)
+@mark_sync_test
 def test_existence_constraint_error():
+    if not db.edition_is_enterprise():
+        pytest.skip("Skipping test for community edition")
     db.cypher_query(
         "CREATE CONSTRAINT test_existence_constraint FOR (n:Human) REQUIRE n.age IS NOT NULL"
     )
     with raises(ConstraintValidationFailed, match=r"must have the property"):
         Human(name="Scarlett").save()
 
     db.cypher_query("DROP CONSTRAINT test_existence_constraint")
 
 
+@mark_sync_test
 def test_optional_properties_dont_get_indexed():
     Human(name="99", age=99).save()
     h = Human.nodes.get(age=99)
     assert h
     assert h.name == "99"
 
     Human(name="98", age=98).save()
     h = Human.nodes.get(age=98)
     assert h
     assert h.name == "98"
 
 
+@mark_sync_test
 def test_escaped_chars():
     _name = "sarah:test"
     Human(name=_name, age=3).save()
     r = Human.nodes.filter(name=_name)
-    assert r
     assert r[0].name == _name
 
 
+@mark_sync_test
 def test_does_not_exist():
     with raises(Human.DoesNotExist):
         Human.nodes.get(name="XXXX")
 
 
+@mark_sync_test
 def test_custom_label_name():
     class Giraffe(StructuredNode):
         __label__ = "Giraffes"
         name = StringProperty(unique_index=True)
 
     jim = Giraffe(name="timothy").save()
     node = Giraffe.nodes.get(name="timothy")
```

### Comparing `neomodel-5.2.1/test/test_issue283.py` & `neomodel-5.3.0/test/sync_/test_issue283.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,140 +5,146 @@
 More information about the same issue at:
 https://github.com/aanastasiou/neomodelInheritanceTest
 
 The following example uses a recursive relationship for economy, but the 
 idea remains the same: "Instantiate the correct type of node at the end of 
 a relationship as specified by the model"
 """
-
-import datetime
-import os
 import random
+from test._async_compat import mark_sync_test
 
 import pytest
 
-import neomodel
+from neomodel import (
+    DateTimeProperty,
+    FloatProperty,
+    RelationshipClassNotDefined,
+    RelationshipClassRedefined,
+    RelationshipTo,
+    StringProperty,
+    StructuredNode,
+    StructuredRel,
+    UniqueIdProperty,
+    db,
+)
+from neomodel.exceptions import NodeClassAlreadyDefined, NodeClassNotDefined
 
 try:
     basestring
 except NameError:
     basestring = str
 
 
 # Set up a very simple model for the tests
-class PersonalRelationship(neomodel.StructuredRel):
+class PersonalRelationship(StructuredRel):
     """
     A very simple relationship between two basePersons that simply records
     the date at which an acquaintance was established.
     This relationship should be carried over to anything that inherits from
     basePerson without any further effort.
     """
 
-    on_date = neomodel.DateTimeProperty(default_now=True)
+    on_date = DateTimeProperty(default_now=True)
 
 
-class BasePerson(neomodel.StructuredNode):
+class BasePerson(StructuredNode):
     """
     Base class for defining some basic sort of an actor.
     """
 
-    name = neomodel.StringProperty(required=True, unique_index=True)
-    friends_with = neomodel.RelationshipTo(
+    name = StringProperty(required=True, unique_index=True)
+    friends_with = RelationshipTo(
         "BasePerson", "FRIENDS_WITH", model=PersonalRelationship
     )
 
 
 class TechnicalPerson(BasePerson):
     """
     A Technical person specialises BasePerson by adding their expertise.
     """
 
-    expertise = neomodel.StringProperty(required=True)
+    expertise = StringProperty(required=True)
 
 
 class PilotPerson(BasePerson):
     """
     A pilot person specialises BasePerson by adding the type of airplane they
     can operate.
     """
 
-    airplane = neomodel.StringProperty(required=True)
+    airplane = StringProperty(required=True)
 
 
-class BaseOtherPerson(neomodel.StructuredNode):
+class BaseOtherPerson(StructuredNode):
     """
     An obviously "wrong" class of actor to befriend BasePersons with.
     """
 
-    car_color = neomodel.StringProperty(required=True)
+    car_color = StringProperty(required=True)
 
 
 class SomePerson(BaseOtherPerson):
     """
     Concrete class that simply derives from BaseOtherPerson.
     """
 
     pass
 
 
 # Test cases
+@mark_sync_test
 def test_automatic_result_resolution():
     """
     Node objects at the end of relationships are instantiated to their
     corresponding Python object.
     """
 
     # Create a few entities
-    A = TechnicalPerson.get_or_create(
-        {"name": "Grumpy", "expertise": "Grumpiness"}
-    )[0]
-    B = TechnicalPerson.get_or_create(
-        {"name": "Happy", "expertise": "Unicorns"}
-    )[0]
-    C = TechnicalPerson.get_or_create(
-        {"name": "Sleepy", "expertise": "Pillows"}
-    )[0]
+    A = (TechnicalPerson.get_or_create({"name": "Grumpy", "expertise": "Grumpiness"}))[
+        0
+    ]
+    B = (TechnicalPerson.get_or_create({"name": "Happy", "expertise": "Unicorns"}))[0]
+    C = (TechnicalPerson.get_or_create({"name": "Sleepy", "expertise": "Pillows"}))[0]
 
     # Add connections
     A.friends_with.connect(B)
     B.friends_with.connect(C)
     C.friends_with.connect(A)
 
+    test = A.friends_with
+
     # If A is friends with B, then A's friends_with objects should be
     # TechnicalPerson (!NOT basePerson!)
-    assert type(A.friends_with[0]) is TechnicalPerson
+    assert type((A.friends_with)[0]) is TechnicalPerson
 
     A.delete()
     B.delete()
     C.delete()
 
 
+@mark_sync_test
 def test_recursive_automatic_result_resolution():
     """
     Node objects are instantiated to native Python objects, both at the top
     level of returned results and in the case where they are returned within
     lists.
     """
 
     # Create a few entities
-    A = TechnicalPerson.get_or_create(
-        {"name": "Grumpier", "expertise": "Grumpiness"}
-    )[0]
-    B = TechnicalPerson.get_or_create(
-        {"name": "Happier", "expertise": "Grumpiness"}
-    )[0]
-    C = TechnicalPerson.get_or_create(
-        {"name": "Sleepier", "expertise": "Pillows"}
-    )[0]
-    D = TechnicalPerson.get_or_create(
-        {"name": "Sneezier", "expertise": "Pillows"}
+    A = (
+        TechnicalPerson.get_or_create({"name": "Grumpier", "expertise": "Grumpiness"})
     )[0]
+    B = (TechnicalPerson.get_or_create({"name": "Happier", "expertise": "Grumpiness"}))[
+        0
+    ]
+    C = (TechnicalPerson.get_or_create({"name": "Sleepier", "expertise": "Pillows"}))[0]
+    D = (TechnicalPerson.get_or_create({"name": "Sneezier", "expertise": "Pillows"}))[0]
 
     # Retrieve mixed results, both at the top level and nested
-    L, _ = neomodel.db.cypher_query(
+    L, _ = db.cypher_query(
         "MATCH (a:TechnicalPerson) "
         "WHERE a.expertise='Grumpiness' "
         "WITH collect(a) as Alpha "
         "MATCH (b:TechnicalPerson) "
         "WHERE b.expertise='Pillows' "
         "WITH Alpha, collect(b) as Beta "
         "RETURN [Alpha, [Beta, [Beta, ['Banana', "
@@ -154,38 +160,39 @@
 
     A.delete()
     B.delete()
     C.delete()
     D.delete()
 
 
+@mark_sync_test
 def test_validation_with_inheritance_from_db():
     """
     Objects descending from the specified class of a relationship's end-node are
     also perfectly valid to appear as end-node values too
     """
 
     # Create a few entities
     # Technical Persons
-    A = TechnicalPerson.get_or_create(
-        {"name": "Grumpy", "expertise": "Grumpiness"}
-    )[0]
-    B = TechnicalPerson.get_or_create(
-        {"name": "Happy", "expertise": "Unicorns"}
-    )[0]
-    C = TechnicalPerson.get_or_create(
-        {"name": "Sleepy", "expertise": "Pillows"}
-    )[0]
+    A = (TechnicalPerson.get_or_create({"name": "Grumpy", "expertise": "Grumpiness"}))[
+        0
+    ]
+    B = (TechnicalPerson.get_or_create({"name": "Happy", "expertise": "Unicorns"}))[0]
+    C = (TechnicalPerson.get_or_create({"name": "Sleepy", "expertise": "Pillows"}))[0]
 
     # Pilot Persons
-    D = PilotPerson.get_or_create(
-        {"name": "Porco Rosso", "airplane": "Savoia-Marchetti"}
+    D = (
+        PilotPerson.get_or_create(
+            {"name": "Porco Rosso", "airplane": "Savoia-Marchetti"}
+        )
     )[0]
-    E = PilotPerson.get_or_create(
-        {"name": "Jack Dalton", "airplane": "Beechcraft Model 18"}
+    E = (
+        PilotPerson.get_or_create(
+            {"name": "Jack Dalton", "airplane": "Beechcraft Model 18"}
+        )
     )[0]
 
     # TechnicalPersons can befriend PilotPersons and vice-versa and that's fine
 
     # TechnicalPersons befriend Technical Persons
     A.friends_with.connect(B)
     B.friends_with.connect(C)
@@ -197,52 +204,53 @@
     # Technical Persons befriend Pilot Persons
     A.friends_with.connect(D)
     E.friends_with.connect(C)
 
     # This now means that friends_with of a TechnicalPerson can
     # either be TechnicalPerson or Pilot Person (!NOT basePerson!)
 
-    assert (type(A.friends_with[0]) is TechnicalPerson) or (
-        type(A.friends_with[0]) is PilotPerson
+    assert (type((A.friends_with)[0]) is TechnicalPerson) or (
+        type((A.friends_with)[0]) is PilotPerson
     )
-    assert (type(A.friends_with[1]) is TechnicalPerson) or (
-        type(A.friends_with[1]) is PilotPerson
+    assert (type((A.friends_with)[1]) is TechnicalPerson) or (
+        type((A.friends_with)[1]) is PilotPerson
     )
-    assert type(D.friends_with[0]) is PilotPerson
+    assert type((D.friends_with)[0]) is PilotPerson
 
     A.delete()
     B.delete()
     C.delete()
     D.delete()
     E.delete()
 
 
+@mark_sync_test
 def test_validation_enforcement_to_db():
     """
     If a connection between wrong types is attempted, raise an exception
     """
 
     # Create a few entities
     # Technical Persons
-    A = TechnicalPerson.get_or_create(
-        {"name": "Grumpy", "expertise": "Grumpiness"}
-    )[0]
-    B = TechnicalPerson.get_or_create(
-        {"name": "Happy", "expertise": "Unicorns"}
-    )[0]
-    C = TechnicalPerson.get_or_create(
-        {"name": "Sleepy", "expertise": "Pillows"}
-    )[0]
+    A = (TechnicalPerson.get_or_create({"name": "Grumpy", "expertise": "Grumpiness"}))[
+        0
+    ]
+    B = (TechnicalPerson.get_or_create({"name": "Happy", "expertise": "Unicorns"}))[0]
+    C = (TechnicalPerson.get_or_create({"name": "Sleepy", "expertise": "Pillows"}))[0]
 
     # Pilot Persons
-    D = PilotPerson.get_or_create(
-        {"name": "Porco Rosso", "airplane": "Savoia-Marchetti"}
+    D = (
+        PilotPerson.get_or_create(
+            {"name": "Porco Rosso", "airplane": "Savoia-Marchetti"}
+        )
     )[0]
-    E = PilotPerson.get_or_create(
-        {"name": "Jack Dalton", "airplane": "Beechcraft Model 18"}
+    E = (
+        PilotPerson.get_or_create(
+            {"name": "Jack Dalton", "airplane": "Beechcraft Model 18"}
+        )
     )[0]
 
     # Some Person
     F = SomePerson(car_color="Blue").save()
 
     # TechnicalPersons can befriend PilotPersons and vice-versa and that's fine
     A.friends_with.connect(B)
@@ -261,215 +269,216 @@
     B.delete()
     C.delete()
     D.delete()
     E.delete()
     F.delete()
 
 
+@mark_sync_test
 def test_failed_result_resolution():
     """
     A Neo4j driver node FROM the database contains labels that are unaware to
     neomodel's Database class. This condition raises ClassDefinitionNotFound
     exception.
     """
 
     class RandomPerson(BasePerson):
-        randomness = neomodel.FloatProperty(default=random.random)
+        randomness = FloatProperty(default=random.random)
 
     # A Technical Person...
-    A = TechnicalPerson.get_or_create(
-        {"name": "Grumpy", "expertise": "Grumpiness"}
-    )[0]
+    A = (TechnicalPerson.get_or_create({"name": "Grumpy", "expertise": "Grumpiness"}))[
+        0
+    ]
 
     # A Random Person...
-    B = RandomPerson.get_or_create({"name": "Mad Hatter"})[0]
+    B = (RandomPerson.get_or_create({"name": "Mad Hatter"}))[0]
 
     A.friends_with.connect(B)
 
     # Simulate the condition where the definition of class RandomPerson is not
     # known yet.
-    del neomodel.db._NODE_CLASS_REGISTRY[
-        frozenset(["RandomPerson", "BasePerson"])
-    ]
+    del db._NODE_CLASS_REGISTRY[frozenset(["RandomPerson", "BasePerson"])]
 
     # Now try to instantiate a RandomPerson
-    A = TechnicalPerson.get_or_create(
-        {"name": "Grumpy", "expertise": "Grumpiness"}
-    )[0]
+    A = (TechnicalPerson.get_or_create({"name": "Grumpy", "expertise": "Grumpiness"}))[
+        0
+    ]
     with pytest.raises(
-        neomodel.exceptions.NodeClassNotDefined,
+        NodeClassNotDefined,
         match=r"Node with labels .* does not resolve to any of the known objects.*",
     ):
-        for some_friend in A.friends_with:
+        friends = A.friends_with.all()
+        for some_friend in friends:
             print(some_friend.name)
 
     A.delete()
     B.delete()
 
 
+@mark_sync_test
 def test_node_label_mismatch():
     """
     A Neo4j driver node FROM the database contains a superset of the known
     labels.
     """
 
     class SuperTechnicalPerson(TechnicalPerson):
-        superness = neomodel.FloatProperty(default=1.0)
+        superness = FloatProperty(default=1.0)
 
     class UltraTechnicalPerson(SuperTechnicalPerson):
-        ultraness = neomodel.FloatProperty(default=3.1415928)
+        ultraness = FloatProperty(default=3.1415928)
 
     # Create a TechnicalPerson...
-    A = TechnicalPerson.get_or_create(
-        {"name": "Grumpy", "expertise": "Grumpiness"}
-    )[0]
+    A = (TechnicalPerson.get_or_create({"name": "Grumpy", "expertise": "Grumpiness"}))[
+        0
+    ]
     # ...that is connected to an UltraTechnicalPerson
-    F = UltraTechnicalPerson(
-        name="Chewbaka", expertise="Aarrr wgh ggwaaah"
-    ).save()
+    F = UltraTechnicalPerson(name="Chewbaka", expertise="Aarrr wgh ggwaaah").save()
     A.friends_with.connect(F)
 
     # Forget about the UltraTechnicalPerson
-    del neomodel.db._NODE_CLASS_REGISTRY[
+    del db._NODE_CLASS_REGISTRY[
         frozenset(
             [
                 "UltraTechnicalPerson",
                 "SuperTechnicalPerson",
                 "TechnicalPerson",
                 "BasePerson",
             ]
         )
     ]
 
     # Recall a TechnicalPerson and enumerate its friends.
     # One of them is UltraTechnicalPerson which would be returned as a valid
     # node to a friends_with query but is currently unknown to the node class registry.
-    A = TechnicalPerson.get_or_create(
-        {"name": "Grumpy", "expertise": "Grumpiness"}
-    )[0]
-    with pytest.raises(neomodel.exceptions.NodeClassNotDefined):
-        for some_friend in A.friends_with:
+    A = (TechnicalPerson.get_or_create({"name": "Grumpy", "expertise": "Grumpiness"}))[
+        0
+    ]
+    with pytest.raises(NodeClassNotDefined):
+        friends = A.friends_with.all()
+        for some_friend in friends:
             print(some_friend.name)
 
 
 def test_attempted_class_redefinition():
     """
-    A neomodel.StructuredNode class is attempted to be redefined.
+    A StructuredNode class is attempted to be redefined.
     """
 
     def redefine_class_locally():
         # Since this test has already set up a class hierarchy in its global scope, we will try to redefine
         # SomePerson here.
         # The internal structure of the SomePerson entity does not matter at all here.
         class SomePerson(BaseOtherPerson):
-            uid = neomodel.UniqueIdProperty()
+            uid = UniqueIdProperty()
 
     with pytest.raises(
-        neomodel.exceptions.NodeClassAlreadyDefined,
+        NodeClassAlreadyDefined,
         match=r"Class .* with labels .* already defined:.*",
     ):
         redefine_class_locally()
 
 
+@mark_sync_test
 def test_relationship_result_resolution():
     """
     A query returning a "Relationship" object can now instantiate it to a data model class
     """
     # Test specific data
-    A = PilotPerson(
-        name="Zantford Granville", airplane="Gee Bee Model R"
-    ).save()
+    A = PilotPerson(name="Zantford Granville", airplane="Gee Bee Model R").save()
     B = PilotPerson(name="Thomas Granville", airplane="Gee Bee Model R").save()
     C = PilotPerson(name="Robert Granville", airplane="Gee Bee Model R").save()
     D = PilotPerson(name="Mark Granville", airplane="Gee Bee Model R").save()
     E = PilotPerson(name="Edward Granville", airplane="Gee Bee Model R").save()
 
     A.friends_with.connect(B)
     B.friends_with.connect(C)
     C.friends_with.connect(D)
     D.friends_with.connect(E)
 
-    query_data = neomodel.db.cypher_query(
+    query_data = db.cypher_query(
         "MATCH (a:PilotPerson)-[r:FRIENDS_WITH]->(b:PilotPerson) "
         "WHERE a.airplane='Gee Bee Model R' and b.airplane='Gee Bee Model R' "
         "RETURN DISTINCT r",
         resolve_objects=True,
     )
 
     # The relationship here should be properly instantiated to a `PersonalRelationship` object.
     assert isinstance(query_data[0][0][0], PersonalRelationship)
 
 
+@mark_sync_test
 def test_properly_inherited_relationship():
     """
     A relationship class extends an existing relationship model that must extended the same previously associated
     relationship label.
     """
 
     # Extends an existing relationship by adding the "relationship_strength" attribute.
     # `ExtendedPersonalRelationship` will now substitute `PersonalRelationship` EVERYWHERE in the system.
     class ExtendedPersonalRelationship(PersonalRelationship):
-        relationship_strength = neomodel.FloatProperty(default=random.random)
+        relationship_strength = FloatProperty(default=random.random)
 
     # Extends SomePerson, establishes "enriched" relationships with any BaseOtherPerson
     class ExtendedSomePerson(SomePerson):
-        friends_with = neomodel.RelationshipTo(
+        friends_with = RelationshipTo(
             "BaseOtherPerson",
             "FRIENDS_WITH",
             model=ExtendedPersonalRelationship,
         )
 
     # Test specific data
     A = ExtendedSomePerson(name="Michael Knight", car_color="Black").save()
     B = ExtendedSomePerson(name="Luke Duke", car_color="Orange").save()
     C = ExtendedSomePerson(name="Michael Schumacher", car_color="Red").save()
 
     A.friends_with.connect(B)
     A.friends_with.connect(C)
 
-    query_data = neomodel.db.cypher_query(
+    query_data = db.cypher_query(
         "MATCH (:ExtendedSomePerson)-[r:FRIENDS_WITH]->(:ExtendedSomePerson) "
         "RETURN DISTINCT r",
         resolve_objects=True,
     )
 
     assert isinstance(query_data[0][0][0], ExtendedPersonalRelationship)
 
 
 def test_improperly_inherited_relationship():
     """
     Attempting to re-define an existing relationship with a completely unrelated class.
     :return:
     """
 
-    class NewRelationship(neomodel.StructuredRel):
-        profile_match_factor = neomodel.FloatProperty()
+    class NewRelationship(StructuredRel):
+        profile_match_factor = FloatProperty()
 
     with pytest.raises(
-        neomodel.RelationshipClassRedefined,
+        RelationshipClassRedefined,
         match=r"Relationship of type .* redefined as .*",
     ):
 
         class NewSomePerson(SomePerson):
-            friends_with = neomodel.RelationshipTo(
+            friends_with = RelationshipTo(
                 "BaseOtherPerson", "FRIENDS_WITH", model=NewRelationship
             )
 
 
+@mark_sync_test
 def test_resolve_inexistent_relationship():
     """
     Attempting to resolve an inexistent relationship should raise an exception
     :return:
     """
 
     # Forget about the FRIENDS_WITH Relationship.
-    del neomodel.db._NODE_CLASS_REGISTRY[frozenset(["FRIENDS_WITH"])]
+    del db._NODE_CLASS_REGISTRY[frozenset(["FRIENDS_WITH"])]
 
     with pytest.raises(
-        neomodel.RelationshipClassNotDefined,
+        RelationshipClassNotDefined,
         match=r"Relationship of type .* does not resolve to any of the known objects.*",
     ):
-        query_data = neomodel.db.cypher_query(
+        query_data = db.cypher_query(
             "MATCH (:ExtendedSomePerson)-[r:FRIENDS_WITH]->(:ExtendedSomePerson) "
             "RETURN DISTINCT r",
             resolve_objects=True,
         )
```

### Comparing `neomodel-5.2.1/test/test_issue600.py` & `neomodel-5.3.0/test/async_/test_issue600.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,87 @@
 """
 Provides a test case for issue 600 - "Pull request #592 cause an error in case of relationship inharitance".
 
 The issue is outlined here: https://github.com/neo4j-contrib/neomodel/issues/600
 """
 
-import datetime
-import os
-import random
+from test._async_compat import mark_async_test
 
-import pytest
-
-import neomodel
+from neomodel import AsyncRelationship, AsyncStructuredNode, AsyncStructuredRel
 
 try:
     basestring
 except NameError:
     basestring = str
 
 
-class Class1(neomodel.StructuredRel):
+class Class1(AsyncStructuredRel):
     pass
 
 
 class SubClass1(Class1):
     pass
 
 
 class SubClass2(Class1):
     pass
 
 
-class RelationshipDefinerSecondSibling(neomodel.StructuredNode):
-    rel_1 = neomodel.Relationship(
+class RelationshipDefinerSecondSibling(AsyncStructuredNode):
+    rel_1 = AsyncRelationship(
         "RelationshipDefinerSecondSibling", "SOME_REL_LABEL", model=Class1
     )
-    rel_2 = neomodel.Relationship(
+    rel_2 = AsyncRelationship(
         "RelationshipDefinerSecondSibling", "SOME_REL_LABEL", model=SubClass1
     )
-    rel_3 = neomodel.Relationship(
+    rel_3 = AsyncRelationship(
         "RelationshipDefinerSecondSibling", "SOME_REL_LABEL", model=SubClass2
     )
 
 
-class RelationshipDefinerParentLast(neomodel.StructuredNode):
-    rel_2 = neomodel.Relationship(
+class RelationshipDefinerParentLast(AsyncStructuredNode):
+    rel_2 = AsyncRelationship(
         "RelationshipDefinerParentLast", "SOME_REL_LABEL", model=SubClass1
     )
-    rel_3 = neomodel.Relationship(
+    rel_3 = AsyncRelationship(
         "RelationshipDefinerParentLast", "SOME_REL_LABEL", model=SubClass2
     )
-    rel_1 = neomodel.Relationship(
+    rel_1 = AsyncRelationship(
         "RelationshipDefinerParentLast", "SOME_REL_LABEL", model=Class1
     )
 
 
 # Test cases
-def test_relationship_definer_second_sibling():
+@mark_async_test
+async def test_relationship_definer_second_sibling():
     # Create a few entities
-    A = RelationshipDefinerSecondSibling.get_or_create({})[0]
-    B = RelationshipDefinerSecondSibling.get_or_create({})[0]
-    C = RelationshipDefinerSecondSibling.get_or_create({})[0]
+    A = (await RelationshipDefinerSecondSibling.get_or_create({}))[0]
+    B = (await RelationshipDefinerSecondSibling.get_or_create({}))[0]
+    C = (await RelationshipDefinerSecondSibling.get_or_create({}))[0]
 
     # Add connections
-    A.rel_1.connect(B)
-    B.rel_2.connect(C)
-    C.rel_3.connect(A)
+    await A.rel_1.connect(B)
+    await B.rel_2.connect(C)
+    await C.rel_3.connect(A)
 
     # Clean up
-    A.delete()
-    B.delete()
-    C.delete()
+    await A.delete()
+    await B.delete()
+    await C.delete()
 
 
-def test_relationship_definer_parent_last():
+@mark_async_test
+async def test_relationship_definer_parent_last():
     # Create a few entities
-    A = RelationshipDefinerParentLast.get_or_create({})[0]
-    B = RelationshipDefinerParentLast.get_or_create({})[0]
-    C = RelationshipDefinerParentLast.get_or_create({})[0]
+    A = (await RelationshipDefinerParentLast.get_or_create({}))[0]
+    B = (await RelationshipDefinerParentLast.get_or_create({}))[0]
+    C = (await RelationshipDefinerParentLast.get_or_create({}))[0]
 
     # Add connections
-    A.rel_1.connect(B)
-    B.rel_2.connect(C)
-    C.rel_3.connect(A)
+    await A.rel_1.connect(B)
+    await B.rel_2.connect(C)
+    await C.rel_3.connect(A)
 
     # Clean up
-    A.delete()
-    B.delete()
-    C.delete()
+    await A.delete()
+    await B.delete()
+    await C.delete()
```

### Comparing `neomodel-5.2.1/test/test_label_drop.py` & `neomodel-5.3.0/test/async_/test_label_drop.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-from neo4j.exceptions import ClientError
+from test._async_compat import mark_async_test
 
-from neomodel import StringProperty, StructuredNode, config
-from neomodel.core import db, remove_all_labels
+from neo4j.exceptions import ClientError
 
-config.AUTO_INSTALL_LABELS = True
+from neomodel import AsyncStructuredNode, StringProperty, adb
 
 
-class ConstraintAndIndex(StructuredNode):
+class ConstraintAndIndex(AsyncStructuredNode):
     name = StringProperty(unique_index=True)
     last_name = StringProperty(index=True)
 
 
-def test_drop_labels():
-    constraints_before = db.list_constraints()
-    indexes_before = db.list_indexes(exclude_token_lookup=True)
+@mark_async_test
+async def test_drop_labels():
+    await adb.install_labels(ConstraintAndIndex)
+    constraints_before = await adb.list_constraints()
+    indexes_before = await adb.list_indexes(exclude_token_lookup=True)
 
     assert len(constraints_before) > 0
     assert len(indexes_before) > 0
 
-    remove_all_labels()
+    await adb.remove_all_labels()
 
-    constraints = db.list_constraints()
-    indexes = db.list_indexes(exclude_token_lookup=True)
+    constraints = await adb.list_constraints()
+    indexes = await adb.list_indexes(exclude_token_lookup=True)
 
     assert len(constraints) == 0
     assert len(indexes) == 0
 
     # Recreating all old constraints and indexes
     for constraint in constraints_before:
         constraint_type_clause = "UNIQUE"
         if constraint["type"] == "NODE_PROPERTY_EXISTENCE":
             constraint_type_clause = "NOT NULL"
         elif constraint["type"] == "NODE_KEY":
             constraint_type_clause = "NODE KEY"
 
-        db.cypher_query(
+        await adb.cypher_query(
             f'CREATE CONSTRAINT {constraint["name"]} FOR (n:{constraint["labelsOrTypes"][0]}) REQUIRE n.{constraint["properties"][0]} IS {constraint_type_clause}'
         )
     for index in indexes_before:
         try:
-            db.cypher_query(
+            await adb.cypher_query(
                 f'CREATE INDEX {index["name"]} FOR (n:{index["labelsOrTypes"][0]}) ON (n.{index["properties"][0]})'
             )
         except ClientError:
             pass
```

### Comparing `neomodel-5.2.1/test/test_label_install.py` & `neomodel-5.3.0/test/sync_/test_label_install.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,21 @@
+from test._async_compat import mark_sync_test
+
 import pytest
 
 from neomodel import (
     RelationshipTo,
     StringProperty,
     StructuredNode,
     StructuredRel,
     UniqueIdProperty,
-    config,
-    install_all_labels,
-    install_labels,
+    db,
 )
-from neomodel.core import db, drop_constraints
 from neomodel.exceptions import ConstraintValidationFailed, FeatureNotSupported
 
-config.AUTO_INSTALL_LABELS = False
-
 
 class NodeWithIndex(StructuredNode):
     name = StringProperty(index=True)
 
 
 class NodeWithConstraint(StructuredNode):
     name = StringProperty(unique_index=True)
@@ -43,100 +40,96 @@
     name = StringProperty(unique_index=True)
 
 
 class SomeNotUniqueNode(StructuredNode):
     id_ = UniqueIdProperty(db_property="id")
 
 
-config.AUTO_INSTALL_LABELS = True
-
-
-def test_labels_were_not_installed():
-    bob = NodeWithConstraint(name="bob").save()
-    bob2 = NodeWithConstraint(name="bob").save()
-    bob3 = NodeWithConstraint(name="bob").save()
-    assert bob.element_id != bob3.element_id
-
-    for n in NodeWithConstraint.nodes.all():
-        n.delete()
-
-
+@mark_sync_test
 def test_install_all():
-    drop_constraints()
-    install_labels(AbstractNode)
+    db.drop_constraints()
+    db.drop_indexes()
+    db.install_labels(AbstractNode)
     # run install all labels
-    install_all_labels()
+    db.install_all_labels()
 
     indexes = db.list_indexes()
     index_names = [index["name"] for index in indexes]
     assert "index_INDEXED_REL_indexed_rel_prop" in index_names
 
     constraints = db.list_constraints()
     constraint_names = [constraint["name"] for constraint in constraints]
     assert "constraint_unique_NodeWithConstraint_name" in constraint_names
     assert "constraint_unique_SomeNotUniqueNode_id" in constraint_names
 
     # remove constraint for above test
     _drop_constraints_for_label_and_property("NoConstraintsSetup", "name")
 
 
+@mark_sync_test
 def test_install_label_twice(capsys):
+    db.drop_constraints()
+    db.drop_indexes()
     expected_std_out = (
         "{code: Neo.ClientError.Schema.EquivalentSchemaRuleAlreadyExists}"
     )
-    install_labels(AbstractNode)
-    install_labels(AbstractNode)
+    db.install_labels(AbstractNode)
+    db.install_labels(AbstractNode)
 
-    install_labels(NodeWithIndex)
-    install_labels(NodeWithIndex, quiet=False)
+    db.install_labels(NodeWithIndex)
+    db.install_labels(NodeWithIndex, quiet=False)
     captured = capsys.readouterr()
     assert expected_std_out in captured.out
 
-    install_labels(NodeWithConstraint)
-    install_labels(NodeWithConstraint, quiet=False)
+    db.install_labels(NodeWithConstraint)
+    db.install_labels(NodeWithConstraint, quiet=False)
     captured = capsys.readouterr()
     assert expected_std_out in captured.out
 
-    install_labels(OtherNodeWithRelationship)
-    install_labels(OtherNodeWithRelationship, quiet=False)
+    db.install_labels(OtherNodeWithRelationship)
+    db.install_labels(OtherNodeWithRelationship, quiet=False)
     captured = capsys.readouterr()
     assert expected_std_out in captured.out
 
     if db.version_is_higher_than("5.7"):
 
         class UniqueIndexRelationship(StructuredRel):
             unique_index_rel_prop = StringProperty(unique_index=True)
 
         class OtherNodeWithUniqueIndexRelationship(StructuredNode):
             has_rel = RelationshipTo(
                 NodeWithRelationship, "UNIQUE_INDEX_REL", model=UniqueIndexRelationship
             )
 
-        install_labels(OtherNodeWithUniqueIndexRelationship)
-        install_labels(OtherNodeWithUniqueIndexRelationship, quiet=False)
+        db.install_labels(OtherNodeWithUniqueIndexRelationship)
+        db.install_labels(OtherNodeWithUniqueIndexRelationship, quiet=False)
         captured = capsys.readouterr()
         assert expected_std_out in captured.out
 
 
+@mark_sync_test
 def test_install_labels_db_property(capsys):
-    drop_constraints()
-    install_labels(SomeNotUniqueNode, quiet=False)
+    db.drop_constraints()
+    db.install_labels(SomeNotUniqueNode, quiet=False)
     captured = capsys.readouterr()
     assert "id" in captured.out
     # make sure that the id_ constraint doesn't exist
     constraint_names = _drop_constraints_for_label_and_property(
         "SomeNotUniqueNode", "id_"
     )
     assert constraint_names == []
     # make sure the id constraint exists and can be removed
     _drop_constraints_for_label_and_property("SomeNotUniqueNode", "id")
 
 
-@pytest.mark.skipif(db.version_is_higher_than("5.7"), reason="Not supported before 5.7")
+@mark_sync_test
 def test_relationship_unique_index_not_supported():
+    if db.version_is_higher_than("5.7"):
+        pytest.skip("Not supported before 5.7")
+
     class UniqueIndexRelationship(StructuredRel):
         name = StringProperty(unique_index=True)
 
     class TargetNodeForUniqueIndexRelationship(StructuredNode):
         pass
 
     with pytest.raises(
@@ -146,31 +139,36 @@
         class NodeWithUniqueIndexRelationship(StructuredNode):
             has_rel = RelationshipTo(
                 TargetNodeForUniqueIndexRelationship,
                 "UNIQUE_INDEX_REL",
                 model=UniqueIndexRelationship,
             )
 
+        db.install_labels(NodeWithUniqueIndexRelationship)
 
-@pytest.mark.skipif(not db.version_is_higher_than("5.7"), reason="Supported from 5.7")
+
+@mark_sync_test
 def test_relationship_unique_index():
+    if not db.version_is_higher_than("5.7"):
+        pytest.skip("Not supported before 5.7")
+
     class UniqueIndexRelationshipBis(StructuredRel):
         name = StringProperty(unique_index=True)
 
     class TargetNodeForUniqueIndexRelationship(StructuredNode):
         pass
 
     class NodeWithUniqueIndexRelationship(StructuredNode):
         has_rel = RelationshipTo(
             TargetNodeForUniqueIndexRelationship,
             "UNIQUE_INDEX_REL_BIS",
             model=UniqueIndexRelationshipBis,
         )
 
-    install_labels(UniqueIndexRelationshipBis)
+    db.install_labels(NodeWithUniqueIndexRelationship)
     node1 = NodeWithUniqueIndexRelationship().save()
     node2 = TargetNodeForUniqueIndexRelationship().save()
     node3 = TargetNodeForUniqueIndexRelationship().save()
     rel1 = node1.has_rel.connect(node2, {"name": "rel1"})
 
     with pytest.raises(
         ConstraintValidationFailed,
```

### Comparing `neomodel-5.2.1/test/test_match_api.py` & `neomodel-5.3.0/test/sync_/test_match_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from datetime import datetime
+from test._async_compat import mark_sync_test
 
 from pytest import raises
 
 from neomodel import (
     INCOMING,
+    ArrayProperty,
     DateTimeProperty,
     IntegerProperty,
     Q,
     RelationshipFrom,
     RelationshipTo,
     StringProperty,
     StructuredNode,
     StructuredRel,
 )
+from neomodel._async_compat.util import Util
 from neomodel.exceptions import MultipleNodesReturned
-from neomodel.match import NodeSet, Optional, QueryBuilder, Traversal
+from neomodel.sync_.match import NodeSet, Optional, QueryBuilder, Traversal
 
 
 class SupplierRel(StructuredRel):
     since = DateTimeProperty(default=datetime.now)
     courier = StringProperty()
 
 
@@ -26,14 +29,15 @@
     name = StringProperty()
     delivery_cost = IntegerProperty()
     coffees = RelationshipTo("Coffee", "COFFEE SUPPLIERS")
 
 
 class Species(StructuredNode):
     name = StringProperty()
+    tags = ArrayProperty(StringProperty(), default=list)
     coffees = RelationshipFrom("Coffee", "COFFEE SPECIES", model=StructuredRel)
 
 
 class Coffee(StructuredNode):
     name = StringProperty(unique_index=True)
     price = IntegerProperty()
     suppliers = RelationshipFrom(Supplier, "COFFEE SUPPLIERS", model=SupplierRel)
@@ -41,14 +45,15 @@
     id_ = IntegerProperty()
 
 
 class Extension(StructuredNode):
     extension = RelationshipTo("Extension", "extension")
 
 
+@mark_sync_test
 def test_filter_exclude_via_labels():
     Coffee(name="Java", price=99).save()
 
     node_set = NodeSet(Coffee)
     qb = QueryBuilder(node_set).build_ast()
 
     results = qb._execute()
@@ -67,14 +72,15 @@
     results = qb._execute()
     assert "(coffee:Coffee)" in qb._ast.match
     assert "NOT" in qb._ast.where[0]
     assert len(results) == 1
     assert results[0].name == "Kenco"
 
 
+@mark_sync_test
 def test_simple_has_via_label():
     nescafe = Coffee(name="Nescafe", price=99).save()
     tesco = Supplier(name="Tesco", delivery_cost=2).save()
     nescafe.suppliers.connect(tesco)
 
     ns = NodeSet(Coffee).has(suppliers=True)
     qb = QueryBuilder(ns).build_ast()
@@ -87,43 +93,47 @@
     ns = NodeSet(Coffee).has(suppliers=False)
     qb = QueryBuilder(ns).build_ast()
     results = qb._execute()
     assert len(results) > 0
     assert "NOT" in qb._ast.where[0]
 
 
+@mark_sync_test
 def test_get():
     Coffee(name="1", price=3).save()
     assert Coffee.nodes.get(name="1")
 
     with raises(Coffee.DoesNotExist):
         Coffee.nodes.get(name="2")
 
     Coffee(name="2", price=3).save()
 
     with raises(MultipleNodesReturned):
         Coffee.nodes.get(price=3)
 
 
+@mark_sync_test
 def test_simple_traverse_with_filter():
     nescafe = Coffee(name="Nescafe2", price=99).save()
     tesco = Supplier(name="Sainsburys", delivery_cost=2).save()
     nescafe.suppliers.connect(tesco)
 
     qb = QueryBuilder(NodeSet(source=nescafe).suppliers.match(since__lt=datetime.now()))
 
-    results = qb.build_ast()._execute()
+    _ast = qb.build_ast()
+    results = _ast._execute()
 
     assert qb._ast.lookup
     assert qb._ast.match
     assert qb._ast.return_clause.startswith("suppliers")
     assert len(results) == 1
     assert results[0].name == "Sainsburys"
 
 
+@mark_sync_test
 def test_double_traverse():
     nescafe = Coffee(name="Nescafe plus", price=99).save()
     tesco = Supplier(name="Asda", delivery_cost=2).save()
     nescafe.suppliers.connect(tesco)
     tesco.coffees.connect(Coffee(name="Decafe", price=2).save())
 
     ns = NodeSet(NodeSet(source=nescafe).suppliers.match()).coffees.match()
@@ -131,103 +141,131 @@
 
     results = qb._execute()
     assert len(results) == 2
     assert results[0].name == "Decafe"
     assert results[1].name == "Nescafe plus"
 
 
+@mark_sync_test
 def test_count():
     Coffee(name="Nescafe Gold", price=99).save()
-    count = QueryBuilder(NodeSet(source=Coffee)).build_ast()._count()
+    ast = QueryBuilder(NodeSet(source=Coffee)).build_ast()
+    count = ast._count()
     assert count > 0
 
     Coffee(name="Kawa", price=27).save()
     node_set = NodeSet(source=Coffee)
     node_set.skip = 1
     node_set.limit = 1
-    count = QueryBuilder(node_set).build_ast()._count()
+    ast = QueryBuilder(node_set).build_ast()
+    count = ast._count()
     assert count == 1
 
 
+@mark_sync_test
 def test_len_and_iter_and_bool():
     iterations = 0
 
     Coffee(name="Icelands finest").save()
 
     for c in Coffee.nodes:
         iterations += 1
         c.delete()
 
     assert iterations > 0
 
     assert len(Coffee.nodes) == 0
 
 
+@mark_sync_test
 def test_slice():
     for c in Coffee.nodes:
         c.delete()
 
     Coffee(name="Icelands finest").save()
     Coffee(name="Britains finest").save()
     Coffee(name="Japans finest").save()
 
-    assert len(list(Coffee.nodes.all()[1:])) == 2
-    assert len(list(Coffee.nodes.all()[:1])) == 1
-    assert isinstance(Coffee.nodes[1], Coffee)
-    assert isinstance(Coffee.nodes[0], Coffee)
-    assert len(list(Coffee.nodes.all()[1:2])) == 1
+    # Branching tests because async needs extra brackets
+    if Util.is_async_code:
+        assert len(list((Coffee.nodes)[1:])) == 2
+        assert len(list((Coffee.nodes)[:1])) == 1
+        assert isinstance((Coffee.nodes)[1], Coffee)
+        assert isinstance((Coffee.nodes)[0], Coffee)
+        assert len(list((Coffee.nodes)[1:2])) == 1
+    else:
+        assert len(list(Coffee.nodes[1:])) == 2
+        assert len(list(Coffee.nodes[:1])) == 1
+        assert isinstance(Coffee.nodes[1], Coffee)
+        assert isinstance(Coffee.nodes[0], Coffee)
+        assert len(list(Coffee.nodes[1:2])) == 1
 
 
+@mark_sync_test
 def test_issue_208():
     # calls to match persist across queries.
 
     b = Coffee(name="basics").save()
     l = Supplier(name="lidl").save()
     a = Supplier(name="aldi").save()
 
     b.suppliers.connect(l, {"courier": "fedex"})
     b.suppliers.connect(a, {"courier": "dhl"})
 
     assert len(b.suppliers.match(courier="fedex"))
     assert len(b.suppliers.match(courier="dhl"))
 
 
+@mark_sync_test
 def test_issue_589():
     node1 = Extension().save()
     node2 = Extension().save()
+    assert node2 not in node1.extension
     node1.extension.connect(node2)
-    assert node2 in node1.extension.all()
+    assert node2 in node1.extension
 
 
+@mark_sync_test
 def test_contains():
     expensive = Coffee(price=1000, name="Pricey").save()
     asda = Coffee(name="Asda", price=1).save()
 
     assert expensive in Coffee.nodes.filter(price__gt=999)
     assert asda not in Coffee.nodes.filter(price__gt=999)
 
     # bad value raises
-    with raises(ValueError):
-        2 in Coffee.nodes
+    with raises(ValueError, match=r"Expecting StructuredNode instance"):
+        if Util.is_async_code:
+            assert Coffee.nodes.__contains__(2)
+        else:
+            assert 2 in Coffee.nodes
 
     # unsaved
-    with raises(ValueError):
-        Coffee() in Coffee.nodes
+    with raises(ValueError, match=r"Unsaved node"):
+        if Util.is_async_code:
+            assert Coffee.nodes.__contains__(Coffee())
+        else:
+            assert Coffee() in Coffee.nodes
 
 
+@mark_sync_test
 def test_order_by():
     for c in Coffee.nodes:
         c.delete()
 
     c1 = Coffee(name="Icelands finest", price=5).save()
     c2 = Coffee(name="Britains finest", price=10).save()
     c3 = Coffee(name="Japans finest", price=35).save()
 
-    assert Coffee.nodes.order_by("price").all()[0].price == 5
-    assert Coffee.nodes.order_by("-price").all()[0].price == 35
+    if Util.is_async_code:
+        assert ((Coffee.nodes.order_by("price"))[0]).price == 5
+        assert ((Coffee.nodes.order_by("-price"))[0]).price == 35
+    else:
+        assert (Coffee.nodes.order_by("price")[0]).price == 5
+        assert (Coffee.nodes.order_by("-price")[0]).price == 35
 
     ns = Coffee.nodes.order_by("-price")
     qb = QueryBuilder(ns).build_ast()
     assert qb._ast.order_by
     ns = ns.order_by(None)
     qb = QueryBuilder(ns).build_ast()
     assert not qb._ast.order_by
@@ -244,45 +282,46 @@
 
     # Test order by on a relationship
     l = Supplier(name="lidl2").save()
     l.coffees.connect(c1)
     l.coffees.connect(c2)
     l.coffees.connect(c3)
 
-    ordered_n = [n for n in l.coffees.order_by("name").all()]
+    ordered_n = [n for n in l.coffees.order_by("name")]
     assert ordered_n[0] == c2
     assert ordered_n[1] == c1
     assert ordered_n[2] == c3
 
 
+@mark_sync_test
 def test_extra_filters():
     for c in Coffee.nodes:
         c.delete()
 
     c1 = Coffee(name="Icelands finest", price=5, id_=1).save()
     c2 = Coffee(name="Britains finest", price=10, id_=2).save()
     c3 = Coffee(name="Japans finest", price=35, id_=3).save()
     c4 = Coffee(name="US extra-fine", price=None, id_=4).save()
 
-    coffees_5_10 = Coffee.nodes.filter(price__in=[10, 5]).all()
+    coffees_5_10 = Coffee.nodes.filter(price__in=[10, 5])
     assert len(coffees_5_10) == 2, "unexpected number of results"
     assert c1 in coffees_5_10, "doesnt contain 5 price coffee"
     assert c2 in coffees_5_10, "doesnt contain 10 price coffee"
 
-    finest_coffees = Coffee.nodes.filter(name__iendswith=" Finest").all()
+    finest_coffees = Coffee.nodes.filter(name__iendswith=" Finest")
     assert len(finest_coffees) == 3, "unexpected number of results"
     assert c1 in finest_coffees, "doesnt contain 1st finest coffee"
     assert c2 in finest_coffees, "doesnt contain 2nd finest coffee"
     assert c3 in finest_coffees, "doesnt contain 3rd finest coffee"
 
-    unpriced_coffees = Coffee.nodes.filter(price__isnull=True).all()
+    unpriced_coffees = Coffee.nodes.filter(price__isnull=True)
     assert len(unpriced_coffees) == 1, "unexpected number of results"
     assert c4 in unpriced_coffees, "doesnt contain unpriced coffee"
 
-    coffees_with_id_gte_3 = Coffee.nodes.filter(id___gte=3).all()
+    coffees_with_id_gte_3 = Coffee.nodes.filter(id___gte=3)
     assert len(coffees_with_id_gte_3) == 2, "unexpected number of results"
     assert c3 in coffees_with_id_gte_3
     assert c4 in coffees_with_id_gte_3
 
     with raises(
         ValueError,
         match=r".*Neo4j internals like id or element_id are not allowed for use in this operation.",
@@ -313,14 +352,15 @@
             "direction": INCOMING,
             "relation_type": "KNOWS",
             "model": None,
         },
     )
 
 
+@mark_sync_test
 def test_empty_filters():
     """Test this case:
      ```
          SomeModel.nodes.filter().filter(Q(arg1=val1)).all()
          SomeModel.nodes.exclude().exclude(Q(arg1=val1)).all()
          SomeModel.nodes.filter().filter(arg1=val1).all()
     ```
@@ -349,14 +389,15 @@
     filter_q_empty_filter = empty_filter.filter(Q(price=5))
     assert len(filter_empty_filter.all()) == 1, "unexpected number of results"
     assert (
         c1 in filter_empty_filter.all()
     ), "doesnt contain c1 in ``filter_empty_filter``"
 
 
+@mark_sync_test
 def test_q_filters():
     # Test where no children and self.connector != conn ?
     for c in Coffee.nodes:
         c.delete()
 
     c1 = Coffee(name="Icelands finest", price=5, id_=1).save()
     c2 = Coffee(name="Britains finest", price=10, id_=2).save()
@@ -414,15 +455,15 @@
     assert (
         len(empty_Q_condition) == 1
     ), "undefined Q leading to unexpected number of results"
     assert c1 in empty_Q_condition
 
     combined_coffees = Coffee.nodes.filter(
         Q(price=35), Q(name="Latte") | Q(name="Cappuccino")
-    )
+    ).all()
     assert len(combined_coffees) == 2
     assert c5 in combined_coffees
     assert c6 in combined_coffees
     assert c3 not in combined_coffees
 
     class QQ:
         pass
@@ -439,14 +480,15 @@
 
     assert ("price", 5) in (Q(price=5) | Q(price=10))
 
     test_hash = set([Q(price_lt=30) | ~Q(price=5), Q(price_lt=30) | ~Q(price=5)])
     assert len(test_hash) == 1
 
 
+@mark_sync_test
 def test_traversal_filter_left_hand_statement():
     nescafe = Coffee(name="Nescafe2", price=99).save()
     nescafe_gold = Coffee(name="Nescafe gold", price=11).save()
 
     tesco = Supplier(name="Sainsburys", delivery_cost=3).save()
     biedronka = Supplier(name="Biedronka", delivery_cost=5).save()
     lidl = Supplier(name="Lidl", delivery_cost=3).save()
@@ -458,14 +500,15 @@
     lidl_supplier = (
         NodeSet(Coffee.nodes.filter(price=11).suppliers).filter(delivery_cost=3).all()
     )
 
     assert lidl in lidl_supplier
 
 
+@mark_sync_test
 def test_fetch_relations():
     arabica = Species(name="Arabica").save()
     robusta = Species(name="Robusta").save()
     nescafe = Coffee(name="Nescafe 1000", price=99).save()
     nescafe_gold = Coffee(name="Nescafe 1001", price=11).save()
 
     tesco = Supplier(name="Sainsburys", delivery_cost=3).save()
@@ -487,18 +530,51 @@
     result = (
         Species.nodes.filter(name="Robusta")
         .fetch_relations(Optional("coffees__suppliers"))
         .all()
     )
     assert result[0][0] is None
 
-    # len() should only consider Suppliers
-    count = len(
-        Supplier.nodes.filter(name="Sainsburys")
-        .fetch_relations("coffees__species")
-        .all()
-    )
-    assert count == 1
+    if Util.is_async_code:
+        count = (
+            Supplier.nodes.filter(name="Sainsburys")
+            .fetch_relations("coffees__species")
+            .__len__()
+        )
+        assert count == 1
 
-    assert tesco in Supplier.nodes.fetch_relations("coffees__species").filter(
-        name="Sainsburys"
-    )
+        assert (
+            Supplier.nodes.fetch_relations("coffees__species")
+            .filter(name="Sainsburys")
+            .__contains__(tesco)
+        )
+    else:
+        count = len(
+            Supplier.nodes.filter(name="Sainsburys")
+            .fetch_relations("coffees__species")
+            .all()
+        )
+        assert count == 1
+
+        assert tesco in Supplier.nodes.fetch_relations("coffees__species").filter(
+            name="Sainsburys"
+        )
+
+
+@mark_sync_test
+def test_in_filter_with_array_property():
+    tags = ["smoother", "sweeter", "chocolate", "sugar"]
+    no_match = ["organic"]
+    arabica = Species(name="Arabica", tags=tags).save()
+
+    assert arabica in Species.nodes.filter(
+        tags__in=tags
+    ), "Species not found by tags given"
+    assert arabica in Species.nodes.filter(
+        Q(tags__in=tags)
+    ), "Species not found with Q by tags given"
+    assert arabica not in Species.nodes.filter(
+        ~Q(tags__in=tags)
+    ), "Species found by tags given in negated query"
+    assert arabica not in Species.nodes.filter(
+        tags__in=no_match
+    ), "Species found by tags with not match tags given"
```

### Comparing `neomodel-5.2.1/test/test_migration_neo4j_5.py` & `neomodel-5.3.0/test/sync_/test_migration_neo4j_5.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from test._async_compat import mark_sync_test
+
 import pytest
 
 from neomodel import (
     IntegerProperty,
     RelationshipTo,
     StringProperty,
     StructuredNode,
     StructuredRel,
+    db,
 )
-from neomodel.core import db
 
 
 class Album(StructuredNode):
     name = StringProperty()
 
 
 class Released(StructuredRel):
@@ -19,33 +21,35 @@
 
 
 class Band(StructuredNode):
     name = StringProperty()
     released = RelationshipTo(Album, relation_type="RELEASED", model=Released)
 
 
+@mark_sync_test
 def test_read_elements_id():
     the_hives = Band(name="The Hives").save()
     lex_hives = Album(name="Lex Hives").save()
     released_rel = the_hives.released.connect(lex_hives)
 
     # Validate element_id properties
-    assert lex_hives.element_id == the_hives.released.single().element_id
+    assert lex_hives.element_id == (the_hives.released.single()).element_id
     assert released_rel._start_node_element_id == the_hives.element_id
     assert released_rel._end_node_element_id == lex_hives.element_id
 
     # Validate id properties
     # Behaviour is dependent on Neo4j version
-    if db.database_version.startswith("4"):
+    db_version = db.database_version
+    if db_version.startswith("4"):
         # Nodes' ids
         assert lex_hives.id == int(lex_hives.element_id)
-        assert lex_hives.id == the_hives.released.single().id
+        assert lex_hives.id == (the_hives.released.single()).id
         # Relationships' ids
-        assert isinstance(released_rel.element_id, int)
-        assert released_rel.element_id == released_rel.id
+        assert isinstance(released_rel.element_id, str)
+        assert int(released_rel.element_id) == released_rel.id
         assert released_rel._start_node_id == int(the_hives.element_id)
         assert released_rel._end_node_id == int(lex_hives.element_id)
     else:
         # Nodes' ids
         expected_error_type = ValueError
         expected_error_message = "id is deprecated in Neo4j version 5, please migrate to element_id\. If you use the id in a Cypher query, replace id\(\) by elementId\(\)\."
         assert isinstance(lex_hives.element_id, str)
```

### Comparing `neomodel-5.2.1/test/test_models.py` & `neomodel-5.3.0/test/sync_/test_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import print_function
 
 from datetime import datetime
+from test._async_compat import mark_sync_test
 
 from pytest import raises
 
 from neomodel import (
     DateProperty,
     IntegerProperty,
     StringProperty,
     StructuredNode,
     StructuredRel,
-    install_labels,
+    db,
 )
-from neomodel.core import db
 from neomodel.exceptions import RequiredProperty, UniqueProperty
 
 
 class User(StructuredNode):
     email = StringProperty(unique_index=True, required=True)
     age = IntegerProperty(index=True)
 
@@ -29,14 +29,15 @@
         self.email = value
 
 
 class NodeWithoutProperty(StructuredNode):
     pass
 
 
+@mark_sync_test
 def test_issue_233():
     class BaseIssue233(StructuredNode):
         __abstract_node__ = True
 
         def __getitem__(self, item):
             return self.__dict__[item]
 
@@ -48,44 +49,42 @@
 
 
 def test_issue_72():
     user = User(email="foo@bar.com")
     assert user.age is None
 
 
+@mark_sync_test
 def test_required():
-    try:
+    with raises(RequiredProperty):
         User(age=3).save()
-    except RequiredProperty:
-        assert True
-    else:
-        assert False
 
 
 def test_repr_and_str():
     u = User(email="robin@test.com", age=3)
-    print(repr(u))
-    print(str(u))
-    assert True
+    assert repr(u) == "<User: {'email': 'robin@test.com', 'age': 3}>"
+    assert str(u) == "{'email': 'robin@test.com', 'age': 3}"
 
 
+@mark_sync_test
 def test_get_and_get_or_none():
     u = User(email="robin@test.com", age=3)
     assert u.save()
     rob = User.nodes.get(email="robin@test.com")
     assert rob.email == "robin@test.com"
     assert rob.age == 3
 
     rob = User.nodes.get_or_none(email="robin@test.com")
     assert rob.email == "robin@test.com"
 
     n = User.nodes.get_or_none(email="robin@nothere.com")
     assert n is None
 
 
+@mark_sync_test
 def test_first_and_first_or_none():
     u = User(email="matt@test.com", age=24)
     assert u.save()
     u2 = User(email="tbrady@test.com", age=40)
     assert u2.save()
     tbrady = User.nodes.order_by("-age").first()
     assert tbrady.email == "tbrady@test.com"
@@ -99,53 +98,59 @@
 
 
 def test_bare_init_without_save():
     """
     If a node model is initialised without being saved, accessing its `element_id` should
     return None.
     """
-    assert(User().element_id is None)
+    assert User().element_id is None
 
 
+@mark_sync_test
 def test_save_to_model():
     u = User(email="jim@test.com", age=3)
     assert u.save()
     assert u.element_id is not None
     assert u.email == "jim@test.com"
     assert u.age == 3
 
 
+@mark_sync_test
 def test_save_node_without_properties():
     n = NodeWithoutProperty()
     assert n.save()
     assert n.element_id is not None
 
 
+@mark_sync_test
 def test_unique():
-    install_labels(User)
+    db.install_labels(User)
     User(email="jim1@test.com", age=3).save()
     with raises(UniqueProperty):
         User(email="jim1@test.com", age=3).save()
 
 
+@mark_sync_test
 def test_update_unique():
     u = User(email="jimxx@test.com", age=3).save()
     u.save()  # this shouldn't fail
 
 
+@mark_sync_test
 def test_update():
     user = User(email="jim2@test.com", age=3).save()
     assert user
     user.email = "jim2000@test.com"
     user.save()
     jim = User.nodes.get(email="jim2000@test.com")
     assert jim
     assert jim.email == "jim2000@test.com"
 
 
+@mark_sync_test
 def test_save_through_magic_property():
     user = User(email_alias="blah@test.com", age=8).save()
     assert user.email_alias == "blah@test.com"
     user = User.nodes.get(email="blah@test.com")
     assert user.email == "blah@test.com"
     assert user.email_alias == "blah@test.com"
 
@@ -159,27 +164,29 @@
 
 class Customer2(StructuredNode):
     __label__ = "customers"
     email = StringProperty(unique_index=True, required=True)
     age = IntegerProperty(index=True)
 
 
+@mark_sync_test
 def test_not_updated_on_unique_error():
-    install_labels(Customer2)
+    db.install_labels(Customer2)
     Customer2(email="jim@bob.com", age=7).save()
     test = Customer2(email="jim1@bob.com", age=2).save()
     test.email = "jim@bob.com"
     with raises(UniqueProperty):
         test.save()
-    customers = Customer2.nodes.all()
+    customers = Customer2.nodes
     assert customers[0].email != customers[1].email
-    assert Customer2.nodes.get(email="jim@bob.com").age == 7
-    assert Customer2.nodes.get(email="jim1@bob.com").age == 2
+    assert (Customer2.nodes.get(email="jim@bob.com")).age == 7
+    assert (Customer2.nodes.get(email="jim1@bob.com")).age == 2
 
 
+@mark_sync_test
 def test_label_not_inherited():
     class Customer3(Customer2):
         address = StringProperty()
 
     assert Customer3.__label__ == "Customer3"
     c = Customer3(email="test@test.com").save()
     assert "customers" in c.labels()
@@ -187,14 +194,15 @@
 
     c = Customer2.nodes.get(email="test@test.com")
     assert isinstance(c, Customer2)
     assert "customers" in c.labels()
     assert "Customer3" in c.labels()
 
 
+@mark_sync_test
 def test_refresh():
     c = Customer2(email="my@email.com", age=16).save()
     c.my_custom_prop = "value"
     copy = Customer2.nodes.get(email="my@email.com")
     copy.age = 20
     copy.save()
 
@@ -206,33 +214,36 @@
 
     c = Customer2.inflate(c.element_id)
     c.age = 30
     c.refresh()
 
     assert c.age == 20
 
-    if db.database_version.startswith("4"):
+    _db_version = db.database_version
+    if _db_version.startswith("4"):
         c = Customer2.inflate(999)
     else:
         c = Customer2.inflate("4:xxxxxx:999")
     with raises(Customer2.DoesNotExist):
         c.refresh()
 
 
+@mark_sync_test
 def test_setting_value_to_none():
     c = Customer2(email="alice@bob.com", age=42).save()
     assert c.age is not None
 
     c.age = None
     c.save()
 
     copy = Customer2.nodes.get(email="alice@bob.com")
     assert copy.age is None
 
 
+@mark_sync_test
 def test_inheritance():
     class User(StructuredNode):
         __abstract_node__ = True
         name = StringProperty(unique_index=True)
 
     class Shopper(User):
         balance = IntegerProperty(index=True)
@@ -244,17 +255,18 @@
     jim = Shopper(name="jimmy", balance=300).save()
     jim.credit_account(50)
 
     assert Shopper.__label__ == "Shopper"
     assert jim.balance == 350
     assert len(jim.inherited_labels()) == 1
     assert len(jim.labels()) == 1
-    assert jim.labels()[0] == "Shopper"
+    assert (jim.labels())[0] == "Shopper"
 
 
+@mark_sync_test
 def test_inherited_optional_labels():
     class BaseOptional(StructuredNode):
         __optional_labels__ = ["Alive"]
         name = StringProperty(unique_index=True)
 
     class ExtendedOptional(BaseOptional):
         __optional_labels__ = ["RewardsMember"]
@@ -271,14 +283,15 @@
     assert henry.balance == 350
     assert len(henry.inherited_labels()) == 2
     assert len(henry.labels()) == 2
 
     assert set(henry.inherited_optional_labels()) == {"Alive", "RewardsMember"}
 
 
+@mark_sync_test
 def test_mixins():
     class UserMixin:
         name = StringProperty(unique_index=True)
         password = StringProperty()
 
     class CreditMixin:
         balance = IntegerProperty(index=True)
@@ -293,17 +306,18 @@
     jim = Shopper2(name="jimmy", balance=300).save()
     jim.credit_account(50)
 
     assert Shopper2.__label__ == "Shopper2"
     assert jim.balance == 350
     assert len(jim.inherited_labels()) == 1
     assert len(jim.labels()) == 1
-    assert jim.labels()[0] == "Shopper2"
+    assert (jim.labels())[0] == "Shopper2"
 
 
+@mark_sync_test
 def test_date_property():
     class DateTest(StructuredNode):
         birthdate = DateProperty()
 
     user = DateTest(birthdate=datetime.now()).save()
```

### Comparing `neomodel-5.2.1/test/test_multiprocessing.py` & `neomodel-5.3.0/test/sync_/test_multiprocessing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from multiprocessing.pool import ThreadPool as Pool
+from test._async_compat import mark_sync_test
 
 from neomodel import StringProperty, StructuredNode, db
 
 
 class ThingyMaBob(StructuredNode):
     name = StringProperty(unique_index=True, required=True)
 
 
 def thing_create(name):
     name = str(name)
     (thing,) = ThingyMaBob.get_or_create({"name": name})
     return thing.name, name
 
 
+@mark_sync_test
 def test_concurrency():
     with Pool(5) as p:
         results = p.map(thing_create, range(50))
-        for returned, sent in results:
+        for to_unpack in results:
+            returned, sent = to_unpack
             assert returned == sent
         db.close_connection()
```

### Comparing `neomodel-5.2.1/test/test_paths.py` & `neomodel-5.3.0/test/sync_/test_paths.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,60 @@
-from neomodel import (StringProperty, StructuredNode, UniqueIdProperty, 
-                      db, RelationshipTo, IntegerProperty, NeomodelPath, StructuredRel)
+from test._async_compat import mark_sync_test
+
+from neomodel import (
+    IntegerProperty,
+    NeomodelPath,
+    RelationshipTo,
+    StringProperty,
+    StructuredNode,
+    StructuredRel,
+    UniqueIdProperty,
+    db,
+)
+
 
 class PersonLivesInCity(StructuredRel):
     """
     Relationship with data that will be instantiated as "stand-alone"
     """
+
     some_num = IntegerProperty(index=True, default=12)
 
+
 class CountryOfOrigin(StructuredNode):
     code = StringProperty(unique_index=True, required=True)
 
+
 class CityOfResidence(StructuredNode):
     name = StringProperty(required=True)
-    country = RelationshipTo(CountryOfOrigin, 'FROM_COUNTRY')
+    country = RelationshipTo(CountryOfOrigin, "FROM_COUNTRY")
+
 
 class PersonOfInterest(StructuredNode):
     uid = UniqueIdProperty()
     name = StringProperty(unique_index=True)
     age = IntegerProperty(index=True, default=0)
 
-    country = RelationshipTo(CountryOfOrigin, 'IS_FROM')
-    city = RelationshipTo(CityOfResidence, 'LIVES_IN', model=PersonLivesInCity)
+    country = RelationshipTo(CountryOfOrigin, "IS_FROM")
+    city = RelationshipTo(CityOfResidence, "LIVES_IN", model=PersonLivesInCity)
 
 
+@mark_sync_test
 def test_path_instantiation():
     """
-    Neo4j driver paths should be instantiated as neomodel paths, with all of 
-    their nodes and relationships resolved to their Python objects wherever 
+    Neo4j driver paths should be instantiated as neomodel paths, with all of
+    their nodes and relationships resolved to their Python objects wherever
     such a mapping is available.
     """
 
-    c1=CountryOfOrigin(code="GR").save()
-    c2=CountryOfOrigin(code="FR").save()
-
-    ct1 = CityOfResidence(name="Athens", country = c1).save()
-    ct2 = CityOfResidence(name="Paris", country = c2).save()
+    c1 = CountryOfOrigin(code="GR").save()
+    c2 = CountryOfOrigin(code="FR").save()
 
+    ct1 = CityOfResidence(name="Athens", country=c1).save()
+    ct2 = CityOfResidence(name="Paris", country=c2).save()
 
     p1 = PersonOfInterest(name="Bill", age=22).save()
     p1.country.connect(c1)
     p1.city.connect(ct1)
 
     p2 = PersonOfInterest(name="Jean", age=28).save()
     p2.country.connect(c2)
@@ -50,15 +65,18 @@
     p3.city.connect(ct2)
 
     p4 = PersonOfInterest(name="Drop", age=16).save()
     p4.country.connect(c1)
     p4.city.connect(ct2)
 
     # Retrieve a single path
-    q = db.cypher_query("MATCH p=(:CityOfResidence)<-[:LIVES_IN]-(:PersonOfInterest)-[:IS_FROM]->(:CountryOfOrigin) RETURN p LIMIT 1", resolve_objects = True)
+    q = db.cypher_query(
+        "MATCH p=(:CityOfResidence)<-[:LIVES_IN]-(:PersonOfInterest)-[:IS_FROM]->(:CountryOfOrigin) RETURN p LIMIT 1",
+        resolve_objects=True,
+    )
 
     path_object = q[0][0][0]
     path_nodes = path_object.nodes
     path_rels = path_object.relationships
 
     assert type(path_object) is NeomodelPath
     assert type(path_nodes[0]) is CityOfResidence
@@ -72,8 +90,7 @@
     c2.delete()
     ct1.delete()
     ct2.delete()
     p1.delete()
     p2.delete()
     p3.delete()
     p4.delete()
-
```

### Comparing `neomodel-5.2.1/test/test_relationship_models.py` & `neomodel-5.3.0/test/sync_/test_relationship_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from datetime import datetime
+from test._async_compat import mark_sync_test
 
 import pytz
 from pytest import raises
 
 from neomodel import (
     DateTimeProperty,
     DeflateError,
     Relationship,
     RelationshipTo,
     StringProperty,
     StructuredNode,
     StructuredRel,
 )
+from neomodel._async_compat.util import Util
 
 HOOKS_CALLED = {"pre_save": 0, "post_save": 0}
 
 
 class FriendRel(StructuredRel):
     since = DateTimeProperty(default=lambda: datetime.now(pytz.utc))
 
@@ -37,14 +39,15 @@
 
 
 class Stoat(StructuredNode):
     name = StringProperty(unique_index=True)
     hates = RelationshipTo("Badger", "HATES", model=HatesRel)
 
 
+@mark_sync_test
 def test_either_connect_with_rel_model():
     paul = Badger(name="Paul").save()
     tom = Badger(name="Tom").save()
 
     # creating rels
     new_rel = tom.friend.disconnect(paul)
     new_rel = tom.friend.connect(paul)
@@ -59,14 +62,15 @@
     # I've tried everything possible to correct this to no avail
     paul = new_rel.start_node()
     tom = new_rel.end_node()
     assert paul.name == "Tom"
     assert tom.name == "Paul"
 
 
+@mark_sync_test
 def test_direction_connect_with_rel_model():
     paul = Badger(name="Paul the badger").save()
     ian = Stoat(name="Ian the stoat").save()
 
     rel = ian.hates.connect(paul, {"reason": "thinks paul should bath more often"})
     assert isinstance(rel.since, datetime)
     assert isinstance(rel, FriendRel)
@@ -99,54 +103,62 @@
             {
                 "reason": "thinks paul should bath more often",
                 "since": "2:30pm",
             },
         )
 
 
+@mark_sync_test
 def test_traversal_where_clause():
     phill = Badger(name="Phill the badger").save()
     tim = Badger(name="Tim the badger").save()
     bob = Badger(name="Bob the badger").save()
     rel = tim.friend.connect(bob)
     now = datetime.now(pytz.utc)
     assert rel.since < now
     rel2 = tim.friend.connect(phill)
     assert rel2.since > now
     friends = tim.friend.match(since__gt=now)
-    assert len(friends) == 1
+    assert len(friends.all()) == 1
 
 
+@mark_sync_test
 def test_multiple_rels_exist_issue_223():
     # check a badger can dislike a stoat for multiple reasons
     phill = Badger(name="Phill").save()
     ian = Stoat(name="Stoat").save()
 
     rel_a = phill.hates.connect(ian, {"reason": "a"})
     rel_b = phill.hates.connect(ian, {"reason": "b"})
     assert rel_a.element_id != rel_b.element_id
 
-    ian_a = phill.hates.match(reason="a")[0]
-    ian_b = phill.hates.match(reason="b")[0]
+    if Util.is_async_code:
+        ian_a = (phill.hates.match(reason="a"))[0]
+        ian_b = (phill.hates.match(reason="b"))[0]
+    else:
+        ian_a = phill.hates.match(reason="a")[0]
+        ian_b = phill.hates.match(reason="b")[0]
     assert ian_a.element_id == ian_b.element_id
 
 
+@mark_sync_test
 def test_retrieve_all_rels():
     tom = Badger(name="tom").save()
     ian = Stoat(name="ian").save()
 
     rel_a = tom.hates.connect(ian, {"reason": "a"})
     rel_b = tom.hates.connect(ian, {"reason": "b"})
 
     rels = tom.hates.all_relationships(ian)
     assert len(rels) == 2
     assert rels[0].element_id in [rel_a.element_id, rel_b.element_id]
     assert rels[1].element_id in [rel_a.element_id, rel_b.element_id]
 
 
+@mark_sync_test
 def test_save_hook_on_rel_model():
     HOOKS_CALLED["pre_save"] = 0
     HOOKS_CALLED["post_save"] = 0
 
     paul = Badger(name="PaulB").save()
     ian = Stoat(name="IanS").save()
```

### Comparing `neomodel-5.2.1/test/test_relationships.py` & `neomodel-5.3.0/test/sync_/test_relationships.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from test._async_compat import mark_sync_test
+
 from pytest import raises
 
 from neomodel import (
     IntegerProperty,
     One,
     Q,
     Relationship,
     RelationshipFrom,
     RelationshipTo,
     StringProperty,
     StructuredNode,
     StructuredRel,
+    db,
 )
-from neomodel.core import db
 
 
 class PersonWithRels(StructuredNode):
     name = StringProperty(unique_index=True)
     age = IntegerProperty(index=True)
     is_from = RelationshipTo("Country", "IS_FROM")
     knows = Relationship("PersonWithRels", "KNOWS")
@@ -37,78 +39,82 @@
 class SuperHero(PersonWithRels):
     power = StringProperty(index=True)
 
     def special_power(self):
         return "I have powers"
 
 
+@mark_sync_test
 def test_actions_on_deleted_node():
     u = PersonWithRels(name="Jim2", age=3).save()
     u.delete()
     with raises(ValueError):
         u.is_from.connect(None)
 
     with raises(ValueError):
         u.is_from.get()
 
     with raises(ValueError):
         u.save()
 
 
+@mark_sync_test
 def test_bidirectional_relationships():
     u = PersonWithRels(name="Jim", age=3).save()
     assert u
 
     de = Country(code="DE").save()
     assert de
 
-    assert not u.is_from
+    assert not u.is_from.all()
 
     assert u.is_from.__class__.__name__ == "ZeroOrMore"
     u.is_from.connect(de)
 
-    assert len(u.is_from) == 1
+    assert len(u.is_from.all()) == 1
 
     assert u.is_from.is_connected(de)
 
-    b = u.is_from.all()[0]
+    b = (u.is_from.all())[0]
     assert b.__class__.__name__ == "Country"
     assert b.code == "DE"
 
-    s = b.inhabitant.all()[0]
+    s = (b.inhabitant.all())[0]
     assert s.name == "Jim"
 
     u.is_from.disconnect(b)
     assert not u.is_from.is_connected(b)
 
 
+@mark_sync_test
 def test_either_direction_connect():
     rey = PersonWithRels(name="Rey", age=3).save()
     sakis = PersonWithRels(name="Sakis", age=3).save()
 
     rey.knows.connect(sakis)
     assert rey.knows.is_connected(sakis)
     assert sakis.knows.is_connected(rey)
     sakis.knows.connect(rey)
 
     result, _ = sakis.cypher(
         f"""MATCH (us), (them)
             WHERE {db.get_id_method()}(us)=$self and {db.get_id_method()}(them)=$them
             MATCH (us)-[r:KNOWS]-(them) RETURN COUNT(r)""",
-        {"them": rey.element_id},
+        {"them": db.parse_element_id(rey.element_id)},
     )
     assert int(result[0][0]) == 1
 
     rel = rey.knows.relationship(sakis)
     assert isinstance(rel, StructuredRel)
 
     rels = rey.knows.all_relationships(sakis)
     assert isinstance(rels[0], StructuredRel)
 
 
+@mark_sync_test
 def test_search_and_filter_and_exclude():
     fred = PersonWithRels(name="Fred", age=13).save()
     zz = Country(code="ZZ").save()
     zx = Country(code="ZX").save()
     zt = Country(code="ZY").save()
     fred.is_from.connect(zz)
     fred.is_from.connect(zx)
@@ -125,22 +131,24 @@
     result = fred.is_from.exclude(Q(code__contains="Y"))
     assert len(result) == 2
 
     result = fred.is_from.filter(Q(code__contains="Z"))
     assert len(result) == 3
 
 
+@mark_sync_test
 def test_custom_methods():
     u = PersonWithRels(name="Joe90", age=13).save()
     assert u.special_power() == "I have no powers"
     u = SuperHero(name="Joe91", age=13, power="xxx").save()
     assert u.special_power() == "I have powers"
     assert u.special_name == "Joe91"
 
 
+@mark_sync_test
 def test_valid_reconnection():
     p = PersonWithRels(name="ElPresidente", age=93).save()
     assert p
 
     pp = PersonWithRels(name="TheAdversary", age=33).save()
     assert pp
 
@@ -155,14 +163,15 @@
     assert c.president.is_connected(pp)
 
     # reelection time
     c.president.reconnect(pp, pp)
     assert c.president.is_connected(pp)
 
 
+@mark_sync_test
 def test_valid_replace():
     brady = PersonWithRels(name="Tom Brady", age=40).save()
     assert brady
 
     gronk = PersonWithRels(name="Rob Gronkowski", age=28).save()
     assert gronk
 
@@ -170,25 +179,26 @@
     assert colbert
 
     hanks = PersonWithRels(name="Tom Hanks", age=61).save()
     assert hanks
 
     brady.knows.connect(gronk)
     brady.knows.connect(colbert)
-    assert len(brady.knows) == 2
+    assert len(brady.knows.all()) == 2
     assert brady.knows.is_connected(gronk)
     assert brady.knows.is_connected(colbert)
 
     brady.knows.replace(hanks)
-    assert len(brady.knows) == 1
+    assert len(brady.knows.all()) == 1
     assert brady.knows.is_connected(hanks)
     assert not brady.knows.is_connected(gronk)
     assert not brady.knows.is_connected(colbert)
 
 
+@mark_sync_test
 def test_props_relationship():
     u = PersonWithRels(name="Mar", age=20).save()
     assert u
 
     c = Country(code="AT").save()
     assert c
```

### Comparing `neomodel-5.2.1/test/test_relative_relationships.py` & `neomodel-5.3.0/test/async_/test_relative_relationships.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from neomodel import RelationshipTo, StringProperty, StructuredNode
+from test._async_compat import mark_async_test
+from test.async_.test_relationships import Country
 
-from .test_relationships import Country
+from neomodel import AsyncRelationshipTo, AsyncStructuredNode, StringProperty
 
 
-class Cat(StructuredNode):
+class Cat(AsyncStructuredNode):
     name = StringProperty()
     # Relationship is defined using a relative class path
-    is_from = RelationshipTo(".test_relationships.Country", "IS_FROM")
+    is_from = AsyncRelationshipTo(".test_relationships.Country", "IS_FROM")
 
 
-def test_relative_relationship():
-    a = Cat(name="snufkin").save()
+@mark_async_test
+async def test_relative_relationship():
+    a = await Cat(name="snufkin").save()
     assert a
 
-    c = Country(code="MG").save()
+    c = await Country(code="MG").save()
     assert c
 
     # connecting an instance of the class defined above
     # the next statement will fail if there's a type mismatch
-    a.is_from.connect(c)
-    assert a.is_from.is_connected(c)
+    await a.is_from.connect(c)
+    assert await a.is_from.is_connected(c)
```

### Comparing `neomodel-5.2.1/test/test_scripts.py` & `neomodel-5.3.0/test/test_scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 
 from neomodel import (
     RelationshipTo,
     StringProperty,
     StructuredNode,
     StructuredRel,
     config,
-    db,
-    install_labels,
-    util,
 )
+from neomodel.sync_.core import db
 
 
 class ScriptsTestRel(StructuredRel):
     some_unique_property = StringProperty(unique_index=db.version_is_higher_than("5.7"))
     some_index_property = StringProperty(index=True)
 
 
@@ -104,17 +102,17 @@
         capture_output=True,
         text=True,
         check=False,
     )
     assert "usage: neomodel_inspect_database" in result.stdout
     assert result.returncode == 0
 
-    util.clear_neo4j_database(db)
-    install_labels(ScriptsTestNode)
-    install_labels(ScriptsTestRel)
+    db.clear_neo4j_database()
+    db.install_labels(ScriptsTestNode)
+    db.install_labels(ScriptsTestRel)
 
     # Create a few nodes and a rel, with indexes and constraints
     node1 = ScriptsTestNode(personal_id="1", name="test").save()
     node2 = ScriptsTestNode(personal_id="2", name="test").save()
     node1.rel.connect(node2, {"some_unique_property": "1", "some_index_property": "2"})
 
     # Create a node with all the parsable property types
```

### Comparing `neomodel-5.2.1/test/test_transactions.py` & `neomodel-5.3.0/test/sync_/test_transactions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,22 @@
+from test._async_compat import mark_sync_test
+
 import pytest
 from neo4j.api import Bookmarks
 from neo4j.exceptions import ClientError, TransactionError
 from pytest import raises
 
-from neomodel import (
-    StringProperty,
-    StructuredNode,
-    UniqueProperty,
-    config,
-    db,
-    install_labels,
-)
+from neomodel import StringProperty, StructuredNode, UniqueProperty, db
 
 
 class APerson(StructuredNode):
     name = StringProperty(unique_index=True)
 
 
+@mark_sync_test
 def test_rollback_and_commit_transaction():
     for p in APerson.nodes:
         p.delete()
 
     APerson(name="Roger").save()
 
     db.begin()
@@ -38,105 +34,112 @@
 
 @db.transaction
 def in_a_tx(*names):
     for n in names:
         APerson(name=n).save()
 
 
+@mark_sync_test
 def test_transaction_decorator():
-    install_labels(APerson)
+    db.install_labels(APerson)
     for p in APerson.nodes:
         p.delete()
 
     # should work
     in_a_tx("Roger")
-    assert True
 
     # should bail but raise correct error
     with raises(UniqueProperty):
         in_a_tx("Jim", "Roger")
 
     assert "Jim" not in [p.name for p in APerson.nodes]
 
 
+@mark_sync_test
 def test_transaction_as_a_context():
     with db.transaction:
         APerson(name="Tim").save()
 
     assert APerson.nodes.filter(name="Tim")
 
     with raises(UniqueProperty):
         with db.transaction:
             APerson(name="Tim").save()
 
 
+@mark_sync_test
 def test_query_inside_transaction():
     for p in APerson.nodes:
         p.delete()
 
     with db.transaction:
         APerson(name="Alice").save()
         APerson(name="Bob").save()
 
         assert len([p.name for p in APerson.nodes]) == 2
 
 
+@mark_sync_test
 def test_read_transaction():
     APerson(name="Johnny").save()
 
     with db.read_transaction:
-        people = APerson.nodes.all()
+        people = APerson.nodes
         assert people
 
     with raises(TransactionError):
         with db.read_transaction:
             with raises(ClientError) as e:
                 APerson(name="Gina").save()
             assert e.value.code == "Neo.ClientError.Statement.AccessMode"
 
 
+@mark_sync_test
 def test_write_transaction():
     with db.write_transaction:
         APerson(name="Amelia").save()
 
     amelia = APerson.nodes.get(name="Amelia")
     assert amelia
 
 
+@mark_sync_test
 def double_transaction():
     db.begin()
     with raises(SystemError, match=r"Transaction in progress"):
         db.begin()
 
     db.rollback()
 
 
 @db.transaction.with_bookmark
-def in_a_tx(*names):
+def in_a_tx_with_bookmark(*names):
     for n in names:
         APerson(name=n).save()
 
 
-def test_bookmark_transaction_decorator(skip_neo4j_before_330):
+@mark_sync_test
+def test_bookmark_transaction_decorator():
     for p in APerson.nodes:
         p.delete()
 
     # should work
-    result, bookmarks = in_a_tx("Ruth", bookmarks=None)
+    result, bookmarks = in_a_tx_with_bookmark("Ruth", bookmarks=None)
     assert result is None
     assert isinstance(bookmarks, Bookmarks)
 
     # should bail but raise correct error
     with raises(UniqueProperty):
-        in_a_tx("Jane", "Ruth")
+        in_a_tx_with_bookmark("Jane", "Ruth")
 
     assert "Jane" not in [p.name for p in APerson.nodes]
 
 
-def test_bookmark_transaction_as_a_context(skip_neo4j_before_330):
+@mark_sync_test
+def test_bookmark_transaction_as_a_context():
     with db.transaction as transaction:
         APerson(name="Tanya").save()
     assert isinstance(transaction.last_bookmark, Bookmarks)
 
     assert APerson.nodes.filter(name="Tanya")
 
     with raises(UniqueProperty):
@@ -154,32 +157,34 @@
         spy_calls.append((args, kwargs))
         return original_begin(*args, **kwargs)
 
     monkeypatch.setattr(db, "begin", begin_spy)
     return spy_calls
 
 
-def test_bookmark_passed_in_to_context(skip_neo4j_before_330, spy_on_db_begin):
+@mark_sync_test
+def test_bookmark_passed_in_to_context(spy_on_db_begin):
     transaction = db.transaction
     with transaction:
         pass
 
-    assert spy_on_db_begin[-1] == ((), {"access_mode": None, "bookmarks": None})
+    assert (spy_on_db_begin)[-1] == ((), {"access_mode": None, "bookmarks": None})
     last_bookmark = transaction.last_bookmark
 
     transaction.bookmarks = last_bookmark
     with transaction:
         pass
     assert spy_on_db_begin[-1] == (
         (),
         {"access_mode": None, "bookmarks": last_bookmark},
     )
 
 
-def test_query_inside_bookmark_transaction(skip_neo4j_before_330):
+@mark_sync_test
+def test_query_inside_bookmark_transaction():
     for p in APerson.nodes:
         p.delete()
 
     with db.transaction as transaction:
         APerson(name="Alice").save()
         APerson(name="Bob").save()
```

