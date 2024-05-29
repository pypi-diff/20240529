# Comparing `tmp/ubkg_api-2.1.3.tar.gz` & `tmp/ubkg_api-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubkg_api-2.1.3.tar", last modified: Fri May 17 14:15:47 2024, max compression
+gzip compressed data, was "ubkg_api-2.1.4.tar", last modified: Wed May 29 14:57:05 2024, max compression
```

## Comparing `ubkg_api-2.1.3.tar` & `ubkg_api-2.1.4.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.322982 ubkg_api-2.1.3/
--rw-r--r--   0 ZHY19      (503) staff       (20)     1087 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/LICENSE
--rw-r--r--   0 ZHY19      (503) staff       (20)    12051 2024-05-17 14:15:47.322163 ubkg_api-2.1.3/PKG-INFO
--rw-r--r--   0 ZHY19      (503) staff       (20)    11349 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/README.md
--rw-r--r--   0 ZHY19      (503) staff       (20)      813 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/pyproject.toml
--rw-r--r--   0 ZHY19      (503) staff       (20)       38 2024-05-17 14:15:47.323037 ubkg_api-2.1.3/setup.cfg
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.153609 ubkg_api-2.1.3/src/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/__init__.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.161433 ubkg_api-2.1.3/src/ubkg_api/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     5679 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/app.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.177891 ubkg_api-2.1.3/src/ubkg_api/common_routes/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/__init__.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.181122 ubkg_api-2.1.3/src/ubkg_api/common_routes/codes/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/codes/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2280 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/codes/codes_controller.py
--rw-r--r--   0 ZHY19      (503) staff       (20)    41167 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/common_neo4j_logic.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.184887 ubkg_api-2.1.3/src/ubkg_api/common_routes/concepts/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/concepts/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)    18131 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/concepts/concepts_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.186832 ubkg_api-2.1.3/src/ubkg_api/common_routes/database/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/database/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      479 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/database/database_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.187303 ubkg_api-2.1.3/src/ubkg_api/common_routes/deprecated/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/deprecated/__init__.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.189253 ubkg_api-2.1.3/src/ubkg_api/common_routes/deprecated/tui/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/deprecated/tui/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      803 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/deprecated/tui/tui_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.192127 ubkg_api-2.1.3/src/ubkg_api/common_routes/node_types/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/node_types/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     6174 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/node_types/node_types_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.194376 ubkg_api-2.1.3/src/ubkg_api/common_routes/property_types/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/property_types/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1009 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/property_types/property_types_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.197171 ubkg_api-2.1.3/src/ubkg_api/common_routes/relationship_types/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/relationship_types/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1046 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/relationship_types/relationship_types_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.202215 ubkg_api-2.1.3/src/ubkg_api/common_routes/sabs/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/sabs/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     7433 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/sabs/sabs_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.205362 ubkg_api-2.1.3/src/ubkg_api/common_routes/semantics/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/semantics/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     5563 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/semantics/semantics_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.207745 ubkg_api-2.1.3/src/ubkg_api/common_routes/sources/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/sources/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1441 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/sources/sources_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.209603 ubkg_api-2.1.3/src/ubkg_api/common_routes/status/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/status/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      930 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/status/status_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.212139 ubkg_api-2.1.3/src/ubkg_api/common_routes/terms/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/terms/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2675 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/terms/terms_controller.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      364 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/common_routes/validate.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.244230 ubkg_api-2.1.3/src/ubkg_api/cypher/
--rw-r--r--   0 ZHY19      (503) staff       (20)     1048 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/codes_code_id_codes.cypher
--rw-r--r--   0 ZHY19      (503) staff       (20)     2542 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/concepts_expand.cypher
--rw-r--r--   0 ZHY19      (503) staff       (20)     3210 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/concepts_nodes.cypher
--rw-r--r--   0 ZHY19      (503) staff       (20)     2399 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/concepts_shortestpath.cypher
--rw-r--r--   0 ZHY19      (503) staff       (20)     2615 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/concepts_spanning_tree.cypher
--rw-r--r--   0 ZHY19      (503) staff       (20)     2331 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/concepts_subgraph.cypher
--rw-r--r--   0 ZHY19      (503) staff       (20)      730 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/node_types.cypher
--rw-r--r--   0 ZHY19      (503) staff       (20)     1183 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/node_types_by_sab.cypher
--rw-r--r--   0 ZHY19      (503) staff       (20)      509 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/sabs_codes_counts.cypher
--rw-r--r--   0 ZHY19      (503) staff       (20)      862 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/sabs_codes_details.cypher
--rw-r--r--   0 ZHY19      (503) staff       (20)      537 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/sabs_term_types.cypher
--rw-r--r--   0 ZHY19      (503) staff       (20)      849 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/semantics_semantic_subtypes.cypher
--rw-r--r--   0 ZHY19      (503) staff       (20)      750 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/semantics_semantic_types.cypher
--rw-r--r--   0 ZHY19      (503) staff       (20)     5033 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/cypher/sources.cypher
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.298761 ubkg_api-2.1.3/src/ubkg_api/models/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1900 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/base_model_.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2518 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/codes_codes_obj.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2037 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/concept_detail.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     5760 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/concept_graph.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1512 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/concept_node.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     4715 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/concept_path_hop.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2126 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/concept_prefterm.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2615 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/concept_sab_rel.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3336 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/concept_sab_rel_depth.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1909 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/concept_term.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.308873 ubkg_api-2.1.3/src/ubkg_api/models/deprecated/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/deprecated/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3438 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/deprecated/concept_path.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1946 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/deprecated/semantic_stn.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2351 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/deprecated/sty_tui_stn.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1418 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/node_type.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     5645 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3704 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/qconcept_tconcept_sab_rel.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3677 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/qqst.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1988 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/sab_definition.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3895 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/sab_relationship_concept_prefterm.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3537 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/sab_relationship_concept_term.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2198 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/semantictype.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1949 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/termtype_code.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      809 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/typing_utils.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3507 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/models/util.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     6991 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/neo4j_connection_helper.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.317118 ubkg_api-2.1.3/src/ubkg_api/utils/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/utils/__init__.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.320453 ubkg_api-2.1.3/src/ubkg_api/utils/deprecated/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/utils/deprecated/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2038 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/utils/deprecated/path_get_endpoints.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     9745 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/utils/http_error_string.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1716 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/utils/http_parameter.py
--rwxr-xr-x   0 ZHY19      (503) staff       (20)      185 2024-05-17 14:05:25.000000 ubkg_api-2.1.3/src/ubkg_api/wsgi.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:15:47.321714 ubkg_api-2.1.3/src/ubkg_api.egg-info/
--rw-r--r--   0 ZHY19      (503) staff       (20)    12051 2024-05-17 14:15:47.000000 ubkg_api-2.1.3/src/ubkg_api.egg-info/PKG-INFO
--rw-r--r--   0 ZHY19      (503) staff       (20)     3718 2024-05-17 14:15:47.000000 ubkg_api-2.1.3/src/ubkg_api.egg-info/SOURCES.txt
--rw-r--r--   0 ZHY19      (503) staff       (20)        1 2024-05-17 14:15:47.000000 ubkg_api-2.1.3/src/ubkg_api.egg-info/dependency_links.txt
--rw-r--r--   0 ZHY19      (503) staff       (20)       69 2024-05-17 14:15:47.000000 ubkg_api-2.1.3/src/ubkg_api.egg-info/requires.txt
--rw-r--r--   0 ZHY19      (503) staff       (20)       18 2024-05-17 14:15:47.000000 ubkg_api-2.1.3/src/ubkg_api.egg-info/top_level.txt
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.403162 ubkg_api-2.1.4/
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1087 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/LICENSE
+-rw-r--r--   0 ZHY19      (503) staff       (20)    12051 2024-05-29 14:57:05.402728 ubkg_api-2.1.4/PKG-INFO
+-rw-r--r--   0 ZHY19      (503) staff       (20)    11349 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/README.md
+-rw-r--r--   0 ZHY19      (503) staff       (20)      813 2024-05-29 01:58:02.000000 ubkg_api-2.1.4/pyproject.toml
+-rw-r--r--   0 ZHY19      (503) staff       (20)       38 2024-05-29 14:57:05.403240 ubkg_api-2.1.4/setup.cfg
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.234992 ubkg_api-2.1.4/src/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.244583 ubkg_api-2.1.4/src/ubkg_api/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5679 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/app.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.255403 ubkg_api-2.1.4/src/ubkg_api/common_routes/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.258293 ubkg_api-2.1.4/src/ubkg_api/common_routes/codes/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/codes/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2280 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/codes/codes_controller.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)    41240 2024-05-29 14:55:28.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/common_neo4j_logic.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.261451 ubkg_api-2.1.4/src/ubkg_api/common_routes/concepts/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/concepts/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)    18131 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/concepts/concepts_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.263563 ubkg_api-2.1.4/src/ubkg_api/common_routes/database/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/database/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      479 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/database/database_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.263930 ubkg_api-2.1.4/src/ubkg_api/common_routes/deprecated/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/deprecated/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.266179 ubkg_api-2.1.4/src/ubkg_api/common_routes/deprecated/tui/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/deprecated/tui/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      803 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/deprecated/tui/tui_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.268842 ubkg_api-2.1.4/src/ubkg_api/common_routes/node_types/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/node_types/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     6174 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/node_types/node_types_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.273090 ubkg_api-2.1.4/src/ubkg_api/common_routes/property_types/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/property_types/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1009 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/property_types/property_types_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.275349 ubkg_api-2.1.4/src/ubkg_api/common_routes/relationship_types/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/relationship_types/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1046 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/relationship_types/relationship_types_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.278787 ubkg_api-2.1.4/src/ubkg_api/common_routes/sabs/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/sabs/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     7433 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/sabs/sabs_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.281983 ubkg_api-2.1.4/src/ubkg_api/common_routes/semantics/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/semantics/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5563 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/semantics/semantics_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.285027 ubkg_api-2.1.4/src/ubkg_api/common_routes/sources/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/sources/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1896 2024-05-29 14:55:28.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/sources/sources_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.288286 ubkg_api-2.1.4/src/ubkg_api/common_routes/status/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/status/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      930 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/status/status_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.291018 ubkg_api-2.1.4/src/ubkg_api/common_routes/terms/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/terms/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2675 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/terms/terms_controller.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      364 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/common_routes/validate.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.322595 ubkg_api-2.1.4/src/ubkg_api/cypher/
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1048 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/codes_code_id_codes.cypher
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2542 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/concepts_expand.cypher
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3210 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/concepts_nodes.cypher
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2399 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/concepts_shortestpath.cypher
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2615 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/concepts_spanning_tree.cypher
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2331 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/concepts_subgraph.cypher
+-rw-r--r--   0 ZHY19      (503) staff       (20)      730 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/node_types.cypher
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1183 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/node_types_by_sab.cypher
+-rw-r--r--   0 ZHY19      (503) staff       (20)      509 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/sabs_codes_counts.cypher
+-rw-r--r--   0 ZHY19      (503) staff       (20)      862 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/sabs_codes_details.cypher
+-rw-r--r--   0 ZHY19      (503) staff       (20)      537 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/sabs_term_types.cypher
+-rw-r--r--   0 ZHY19      (503) staff       (20)      849 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/semantics_semantic_subtypes.cypher
+-rw-r--r--   0 ZHY19      (503) staff       (20)      750 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/semantics_semantic_types.cypher
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5033 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/cypher/sources.cypher
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.384716 ubkg_api-2.1.4/src/ubkg_api/models/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1900 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/base_model_.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2518 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/codes_codes_obj.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2037 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/concept_detail.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5760 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/concept_graph.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1512 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/concept_node.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     4715 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/concept_path_hop.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2126 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/concept_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2615 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/concept_sab_rel.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3336 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/concept_sab_rel_depth.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1909 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/concept_term.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.392439 ubkg_api-2.1.4/src/ubkg_api/models/deprecated/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/deprecated/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3438 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/deprecated/concept_path.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1946 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/deprecated/semantic_stn.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2351 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/deprecated/sty_tui_stn.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1418 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/node_type.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5645 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3704 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/qconcept_tconcept_sab_rel.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3677 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/qqst.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1988 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/sab_definition.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3895 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/sab_relationship_concept_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3537 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/sab_relationship_concept_term.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2198 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/semantictype.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1949 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/termtype_code.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      809 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/typing_utils.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3507 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/models/util.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     6991 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/neo4j_connection_helper.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.397681 ubkg_api-2.1.4/src/ubkg_api/utils/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/utils/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.401606 ubkg_api-2.1.4/src/ubkg_api/utils/deprecated/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/utils/deprecated/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2038 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/utils/deprecated/path_get_endpoints.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     9745 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/utils/http_error_string.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1716 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/utils/http_parameter.py
+-rwxr-xr-x   0 ZHY19      (503) staff       (20)      185 2024-05-17 14:05:25.000000 ubkg_api-2.1.4/src/ubkg_api/wsgi.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-29 14:57:05.402272 ubkg_api-2.1.4/src/ubkg_api.egg-info/
+-rw-r--r--   0 ZHY19      (503) staff       (20)    12051 2024-05-29 14:57:05.000000 ubkg_api-2.1.4/src/ubkg_api.egg-info/PKG-INFO
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3718 2024-05-29 14:57:05.000000 ubkg_api-2.1.4/src/ubkg_api.egg-info/SOURCES.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)        1 2024-05-29 14:57:05.000000 ubkg_api-2.1.4/src/ubkg_api.egg-info/dependency_links.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)       69 2024-05-29 14:57:05.000000 ubkg_api-2.1.4/src/ubkg_api.egg-info/requires.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)       18 2024-05-29 14:57:05.000000 ubkg_api-2.1.4/src/ubkg_api.egg-info/top_level.txt
```

### Comparing `ubkg_api-2.1.3/LICENSE` & `ubkg_api-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/PKG-INFO` & `ubkg_api-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubkg_api
-Version: 2.1.3
+Version: 2.1.4
 Summary: A REST API in front of the Unified Biomedical Knowlegde Graph
 Author-email: HuBMAP Consortium <api-developers@hubmapconsortium.org>
 Project-URL: Homepage, https://github.com/x-atlas-consortia/ubkg-api
 Project-URL: Bug Tracker, https://github.com/x-atlas-consortia/ubkg-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ubkg_api-2.1.3/README.md` & `ubkg_api-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/pyproject.toml` & `ubkg_api-2.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.package-data]
 "*" = ["*.cypher"]
 
 [project]
 name = "ubkg_api"
-version = "2.1.3"
+version = "2.1.4"
 authors = [
   { name="HuBMAP Consortium", email="api-developers@hubmapconsortium.org" },
 ]
 description = "A REST API in front of the Unified Biomedical Knowlegde Graph"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ubkg_api-2.1.3/src/ubkg_api/app.py` & `ubkg_api-2.1.4/src/ubkg_api/app.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/common_routes/codes/codes_controller.py` & `ubkg_api-2.1.4/src/ubkg_api/common_routes/codes/codes_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/common_routes/common_neo4j_logic.py` & `ubkg_api-2.1.4/src/ubkg_api/common_routes/common_neo4j_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1058,18 +1058,19 @@
     # Filter by code SAB.
     if len(sab) == 0:
         querytxt = querytxt.replace('$sabfilter', '')
     else:
         querytxt = querytxt.replace('$sabfilter', f" AND t.name IN {sab}")
 
     # Filter by ubkg context.
+    # JAS 24 May 2024 bug fix - replace t.name with tContext.name
     if len(context) == 0:
         querytxt = querytxt.replace('$contextfilter', '')
     else:
-        querytxt = querytxt.replace('$contextfilter', f" AND t.name IN {context}")
+        querytxt = querytxt.replace('$contextfilter', f" AND tContext.name IN {context}")
 
     # Set timeout for query based on value in app.cfg.
     query = neo4j.Query(text=querytxt, timeout=neo4j_instance.timeout)
 
     with neo4j_instance.driver.session() as session:
         recds: neo4j.Result = session.run(query)
         for record in recds:
```

### Comparing `ubkg_api-2.1.3/src/ubkg_api/common_routes/concepts/concepts_controller.py` & `ubkg_api-2.1.4/src/ubkg_api/common_routes/concepts/concepts_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/common_routes/deprecated/tui/tui_controller.py` & `ubkg_api-2.1.4/src/ubkg_api/common_routes/deprecated/tui/tui_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/common_routes/node_types/node_types_controller.py` & `ubkg_api-2.1.4/src/ubkg_api/common_routes/node_types/node_types_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/common_routes/property_types/property_types_controller.py` & `ubkg_api-2.1.4/src/ubkg_api/common_routes/property_types/property_types_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/common_routes/relationship_types/relationship_types_controller.py` & `ubkg_api-2.1.4/src/ubkg_api/common_routes/relationship_types/relationship_types_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/common_routes/sabs/sabs_controller.py` & `ubkg_api-2.1.4/src/ubkg_api/common_routes/sabs/sabs_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/common_routes/semantics/semantics_controller.py` & `ubkg_api-2.1.4/src/ubkg_api/common_routes/semantics/semantics_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/common_routes/sources/sources_controller.py` & `ubkg_api-2.1.4/src/ubkg_api/common_routes/sources/sources_controller.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,14 +19,24 @@
     # Check for invalid parameter names.
     err = validate_query_parameter_names(parameter_name_list=['sab', 'context'])
     if err != 'ok':
         return make_response(err, 400)
 
     sab = parameter_as_list(param_name='sab')
     context = parameter_as_list(param_name='context')
+    # JAS 24 May 2024
+    # Validate context parameter against enum.
+    val_enum = ['base_context', 'data_distillery_context', 'hubmap_sennet_context']
+    if context is not None:
+        for c in context:
+            c = c.lower()
+            err = validate_parameter_value_in_enum(param_name='context', param_value=c,
+                                               enum_list=val_enum)
+        if err != 'ok':
+            return make_response(err, 400)
 
     result = sources_get_logic(neo4j_instance, sab=sab, context=context)
     iserr = result is None or result == []
 
     if not iserr:
         # Check for no results.
         sources = result.get('sources')
```

### Comparing `ubkg_api-2.1.3/src/ubkg_api/common_routes/status/status_controller.py` & `ubkg_api-2.1.4/src/ubkg_api/common_routes/status/status_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/common_routes/terms/terms_controller.py` & `ubkg_api-2.1.4/src/ubkg_api/common_routes/terms/terms_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/cypher/codes_code_id_codes.cypher` & `ubkg_api-2.1.4/src/ubkg_api/cypher/codes_code_id_codes.cypher`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/cypher/concepts_expand.cypher` & `ubkg_api-2.1.4/src/ubkg_api/cypher/concepts_expand.cypher`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/cypher/concepts_nodes.cypher` & `ubkg_api-2.1.4/src/ubkg_api/cypher/concepts_nodes.cypher`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/cypher/concepts_shortestpath.cypher` & `ubkg_api-2.1.4/src/ubkg_api/cypher/concepts_shortestpath.cypher`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/cypher/concepts_spanning_tree.cypher` & `ubkg_api-2.1.4/src/ubkg_api/cypher/concepts_spanning_tree.cypher`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/cypher/concepts_subgraph.cypher` & `ubkg_api-2.1.4/src/ubkg_api/cypher/concepts_subgraph.cypher`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/cypher/node_types.cypher` & `ubkg_api-2.1.4/src/ubkg_api/cypher/node_types.cypher`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/cypher/node_types_by_sab.cypher` & `ubkg_api-2.1.4/src/ubkg_api/cypher/node_types_by_sab.cypher`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/cypher/sabs_codes_details.cypher` & `ubkg_api-2.1.4/src/ubkg_api/cypher/sabs_codes_details.cypher`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/cypher/sabs_term_types.cypher` & `ubkg_api-2.1.4/src/ubkg_api/cypher/sabs_term_types.cypher`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/cypher/semantics_semantic_subtypes.cypher` & `ubkg_api-2.1.4/src/ubkg_api/cypher/semantics_semantic_subtypes.cypher`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/cypher/semantics_semantic_types.cypher` & `ubkg_api-2.1.4/src/ubkg_api/cypher/semantics_semantic_types.cypher`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/cypher/sources.cypher` & `ubkg_api-2.1.4/src/ubkg_api/cypher/sources.cypher`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/base_model_.py` & `ubkg_api-2.1.4/src/ubkg_api/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/codes_codes_obj.py` & `ubkg_api-2.1.4/src/ubkg_api/models/codes_codes_obj.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/concept_detail.py` & `ubkg_api-2.1.4/src/ubkg_api/models/concept_detail.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/concept_graph.py` & `ubkg_api-2.1.4/src/ubkg_api/models/concept_graph.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/concept_node.py` & `ubkg_api-2.1.4/src/ubkg_api/models/concept_node.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/concept_path_hop.py` & `ubkg_api-2.1.4/src/ubkg_api/models/concept_path_hop.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/concept_prefterm.py` & `ubkg_api-2.1.4/src/ubkg_api/models/concept_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/concept_sab_rel.py` & `ubkg_api-2.1.4/src/ubkg_api/models/concept_sab_rel.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/concept_sab_rel_depth.py` & `ubkg_api-2.1.4/src/ubkg_api/models/concept_sab_rel_depth.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/concept_term.py` & `ubkg_api-2.1.4/src/ubkg_api/models/concept_term.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/deprecated/concept_path.py` & `ubkg_api-2.1.4/src/ubkg_api/models/deprecated/concept_path.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/deprecated/semantic_stn.py` & `ubkg_api-2.1.4/src/ubkg_api/models/deprecated/semantic_stn.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/deprecated/sty_tui_stn.py` & `ubkg_api-2.1.4/src/ubkg_api/models/deprecated/sty_tui_stn.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/node_type.py` & `ubkg_api-2.1.4/src/ubkg_api/models/node_type.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py` & `ubkg_api-2.1.4/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/qconcept_tconcept_sab_rel.py` & `ubkg_api-2.1.4/src/ubkg_api/models/qconcept_tconcept_sab_rel.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/qqst.py` & `ubkg_api-2.1.4/src/ubkg_api/models/qqst.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/sab_definition.py` & `ubkg_api-2.1.4/src/ubkg_api/models/sab_definition.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/sab_relationship_concept_prefterm.py` & `ubkg_api-2.1.4/src/ubkg_api/models/sab_relationship_concept_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/sab_relationship_concept_term.py` & `ubkg_api-2.1.4/src/ubkg_api/models/sab_relationship_concept_term.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/semantictype.py` & `ubkg_api-2.1.4/src/ubkg_api/models/semantictype.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/termtype_code.py` & `ubkg_api-2.1.4/src/ubkg_api/models/termtype_code.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/typing_utils.py` & `ubkg_api-2.1.4/src/ubkg_api/models/typing_utils.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/models/util.py` & `ubkg_api-2.1.4/src/ubkg_api/models/util.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/neo4j_connection_helper.py` & `ubkg_api-2.1.4/src/ubkg_api/neo4j_connection_helper.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/utils/deprecated/path_get_endpoints.py` & `ubkg_api-2.1.4/src/ubkg_api/utils/deprecated/path_get_endpoints.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/utils/http_error_string.py` & `ubkg_api-2.1.4/src/ubkg_api/utils/http_error_string.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api/utils/http_parameter.py` & `ubkg_api-2.1.4/src/ubkg_api/utils/http_parameter.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.3/src/ubkg_api.egg-info/PKG-INFO` & `ubkg_api-2.1.4/src/ubkg_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubkg_api
-Version: 2.1.3
+Version: 2.1.4
 Summary: A REST API in front of the Unified Biomedical Knowlegde Graph
 Author-email: HuBMAP Consortium <api-developers@hubmapconsortium.org>
 Project-URL: Homepage, https://github.com/x-atlas-consortia/ubkg-api
 Project-URL: Bug Tracker, https://github.com/x-atlas-consortia/ubkg-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ubkg_api-2.1.3/src/ubkg_api.egg-info/SOURCES.txt` & `ubkg_api-2.1.4/src/ubkg_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

