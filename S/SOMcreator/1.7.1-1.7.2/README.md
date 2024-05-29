# Comparing `tmp/somcreator-1.7.1.tar.gz` & `tmp/somcreator-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somcreator-1.7.1.tar", last modified: Tue Apr 23 11:40:20 2024, max compression
+gzip compressed data, was "somcreator-1.7.2.tar", last modified: Wed May 29 14:48:26 2024, max compression
```

## Comparing `somcreator-1.7.1.tar` & `somcreator-1.7.2.tar`

### file list

```diff
@@ -1,97 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.942227 somcreator-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-23 11:40:16.000000 somcreator-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-23 11:40:16.000000 somcreator-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-23 11:40:20.942227 somcreator-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 11:40:16.000000 somcreator-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-23 11:40:16.000000 somcreator-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 11:40:20.942227 somcreator-1.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.926227 somcreator-1.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.926227 somcreator-1.7.1/src/SOMcreator/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.930227 somcreator-1.7.1/src/SOMcreator/Template/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/Template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.930227 somcreator-1.7.1/src/SOMcreator/Template/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/Template/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/Template/bookmark_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/Template/fast_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/Template/ifc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.930227 somcreator-1.7.1/src/SOMcreator/Template/js_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/Template/js_templates/start_check_start.js
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/Template/js_templates/start_koordinaten.js
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/Template/mapping_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/Template/template.txt
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/Template/untested_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39063 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.930227 somcreator-1.7.1/src/SOMcreator/constants/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/constants/ifc_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/constants/json_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/constants/log_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/constants/value_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.934227 somcreator-1.7.1/src/SOMcreator/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/core/export_excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/core/ifctosql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.934227 somcreator-1.7.1/src/SOMcreator/external_software/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.934227 somcreator-1.7.1/src/SOMcreator/external_software/IDS/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/IDS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/IDS/ids_xsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/IDS/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/IDS/xml_xsd.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.934227 somcreator-1.7.1/src/SOMcreator/external_software/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/__pyinstaller/hook-SOMcreator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/allplan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.934227 somcreator-1.7.1/src/SOMcreator/external_software/bim_collab_zoom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/bim_collab_zoom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/bim_collab_zoom/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/bim_collab_zoom/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/bim_collab_zoom/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/bim_collab_zoom/modelcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/bim_collab_zoom/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/card1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.938227 somcreator-1.7.1/src/SOMcreator/external_software/desite/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/desite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/desite/attribute_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/desite/bill_of_quantities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/desite/bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/desite/building_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    20176 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/desite/modelcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/revit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/external_software/vestra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.938227 somcreator-1.7.1/src/SOMcreator/filehandling/
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/filehandling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/filehandling/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/filehandling/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/filehandling/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/filehandling/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/filehandling/inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/filehandling/obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/filehandling/predefined_pset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/filehandling/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/filehandling/property_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/filehandling/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.938227 somcreator-1.7.1/src/SOMcreator/ifc_modification/
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/ifc_modification/grouping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.938227 somcreator-1.7.1/src/SOMcreator/module/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/module/export_excel.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/module/ifctosql.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/module/parsesql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.942227 somcreator-1.7.1/src/SOMcreator/tool/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/tool/export_excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/tool/ifctosql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/tool/parsesql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.942227 somcreator-1.7.1/src/SOMcreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-23 11:40:16.000000 somcreator-1.7.1/src/SOMcreator/tools/merge_projects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:40:20.942227 somcreator-1.7.1/src/SOMcreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-23 11:40:20.000000 somcreator-1.7.1/src/SOMcreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-23 11:40:20.000000 somcreator-1.7.1/src/SOMcreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:40:20.000000 somcreator-1.7.1/src/SOMcreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-23 11:40:20.000000 somcreator-1.7.1/src/SOMcreator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 11:40:20.000000 somcreator-1.7.1/src/SOMcreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 11:40:20.000000 somcreator-1.7.1/src/SOMcreator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.158107 somcreator-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 14:48:21.000000 somcreator-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 14:48:21.000000 somcreator-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-29 14:48:26.158107 somcreator-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-29 14:48:21.000000 somcreator-1.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-29 14:48:21.000000 somcreator-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:48:26.158107 somcreator-1.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.146107 somcreator-1.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.146107 somcreator-1.7.2/src/SOMcreator/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.150107 somcreator-1.7.2/src/SOMcreator/Template/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/Template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.150107 somcreator-1.7.2/src/SOMcreator/Template/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/Template/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/Template/bookmark_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/Template/fast_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/Template/ifc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.150107 somcreator-1.7.2/src/SOMcreator/Template/js_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/Template/js_templates/start_check_start.js
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/Template/js_templates/start_koordinaten.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/Template/mapping_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/Template/template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/Template/untested_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39063 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.150107 somcreator-1.7.2/src/SOMcreator/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/constants/ifc_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/constants/json_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/constants/log_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/constants/value_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.150107 somcreator-1.7.2/src/SOMcreator/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/core/export_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/core/ifctosql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.150107 somcreator-1.7.2/src/SOMcreator/external_software/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.154107 somcreator-1.7.2/src/SOMcreator/external_software/IDS/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/IDS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/IDS/ids_xsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/IDS/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/IDS/xml_xsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.154107 somcreator-1.7.2/src/SOMcreator/external_software/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/__pyinstaller/hook-SOMcreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/allplan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.154107 somcreator-1.7.2/src/SOMcreator/external_software/bim_collab_zoom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/bim_collab_zoom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/bim_collab_zoom/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/bim_collab_zoom/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/bim_collab_zoom/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/bim_collab_zoom/modelcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/bim_collab_zoom/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/card1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.154107 somcreator-1.7.2/src/SOMcreator/external_software/desite/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/desite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/desite/attribute_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/desite/bill_of_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/desite/bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/desite/building_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20202 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/desite/modelcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/revit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/vestra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.154107 somcreator-1.7.2/src/SOMcreator/external_software/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/external_software/xml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.158107 somcreator-1.7.2/src/SOMcreator/filehandling/
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/filehandling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/filehandling/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/filehandling/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/filehandling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/filehandling/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/filehandling/inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/filehandling/obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/filehandling/predefined_pset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/filehandling/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/filehandling/property_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/filehandling/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.158107 somcreator-1.7.2/src/SOMcreator/ifc_modification/
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/ifc_modification/grouping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.158107 somcreator-1.7.2/src/SOMcreator/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/module/export_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/module/ifctosql.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/module/parsesql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.158107 somcreator-1.7.2/src/SOMcreator/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/tool/export_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/tool/ifctosql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/tool/parsesql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.158107 somcreator-1.7.2/src/SOMcreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-29 14:48:21.000000 somcreator-1.7.2/src/SOMcreator/tools/merge_projects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:48:26.158107 somcreator-1.7.2/src/SOMcreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-29 14:48:26.000000 somcreator-1.7.2/src/SOMcreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-29 14:48:26.000000 somcreator-1.7.2/src/SOMcreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:48:26.000000 somcreator-1.7.2/src/SOMcreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 14:48:26.000000 somcreator-1.7.2/src/SOMcreator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-29 14:48:26.000000 somcreator-1.7.2/src/SOMcreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 14:48:26.000000 somcreator-1.7.2/src/SOMcreator.egg-info/top_level.txt
```

### Comparing `somcreator-1.7.1/LICENSE` & `somcreator-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/PKG-INFO` & `somcreator-1.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.7.1
+Version: 1.7.2
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `somcreator-1.7.1/pyproject.toml` & `somcreator-1.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/Template/fast_template.txt` & `somcreator-1.7.2/src/SOMcreator/Template/fast_template.txt`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/Template/ifc.json` & `somcreator-1.7.2/src/SOMcreator/Template/ifc.json`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/Template/js_templates/start_check_start.js` & `somcreator-1.7.2/src/SOMcreator/Template/js_templates/start_check_start.js`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/Template/js_templates/start_koordinaten.js` & `somcreator-1.7.2/src/SOMcreator/Template/js_templates/start_koordinaten.js`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/Template/mapping_template.txt` & `somcreator-1.7.2/src/SOMcreator/Template/mapping_template.txt`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/Template/template.txt` & `somcreator-1.7.2/src/SOMcreator/Template/template.txt`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/Template/untested_template.txt` & `somcreator-1.7.2/src/SOMcreator/Template/untested_template.txt`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/classes.py` & `somcreator-1.7.2/src/SOMcreator/classes.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/constants/ifc_datatypes.py` & `somcreator-1.7.2/src/SOMcreator/constants/ifc_datatypes.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/constants/value_constants.py` & `somcreator-1.7.2/src/SOMcreator/constants/value_constants.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/core/export_excel.py` & `somcreator-1.7.2/src/SOMcreator/core/export_excel.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/core/ifctosql.py` & `somcreator-1.7.2/src/SOMcreator/core/ifctosql.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/IDS/ids_xsd.py` & `somcreator-1.7.2/src/SOMcreator/external_software/IDS/ids_xsd.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/IDS/main.py` & `somcreator-1.7.2/src/SOMcreator/external_software/IDS/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import date
 
 from lxml.etree import Element, ElementTree, SubElement
 
 from . import ids_xsd, xml_xsd
 from ... import classes
 from ...constants import value_constants, ifc_datatypes
-
+from ..xml import transform_data_format
 NSMAP = {None: ids_xsd.DEFAULT_NS[1:-1],
          "xs": xml_xsd.NS_XS[1:-1],
          "xsi": xml_xsd.NS_XSI[1:-1]}
 
 
 def _build_info(proj: classes.Project, author, xml_parent: Element) -> None:
     xml_element = SubElement(xml_parent, ids_xsd.INFO, nsmap=NSMAP)
@@ -67,15 +67,15 @@
     SubElement(xml_property_set, ids_xsd.SIMPLEVALUE, nsmap=NSMAP).text = attribute.property_set.name
     xml_name = SubElement(xml_property, ids_xsd.NAME)
     SubElement(xml_name, ids_xsd.SIMPLEVALUE, nsmap=NSMAP).text = attribute.name
     if not attribute.value:
         return
     xml_value = SubElement(xml_property, ids_xsd.VALUE, nsmap=NSMAP)
     xml_restriction = SubElement(xml_value, xml_xsd.RESTRICTION, nsmap=NSMAP)
-    xml_restriction.set(xml_xsd.BASE, value_constants.XS_DATATYPE_DICT[attribute.data_type])
+    xml_restriction.set(xml_xsd.BASE, transform_data_format(attribute.data_type))
 
     if attribute.value_type == value_constants.LIST:
         for value in attribute.value:
             SubElement(xml_restriction, xml_xsd.ENUMERATION, nsmap=NSMAP).set(xml_xsd.VALUE, str(value))
 
     if attribute.value_type == value_constants.RANGE:
         min_value = min(min(v[0] for v in attribute.value), min(v[1] for v in attribute.value))
```

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/IDS/xml_xsd.py` & `somcreator-1.7.2/src/SOMcreator/external_software/IDS/xml_xsd.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/allplan.py` & `somcreator-1.7.2/src/SOMcreator/external_software/allplan.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/bim_collab_zoom/condition.py` & `somcreator-1.7.2/src/SOMcreator/external_software/bim_collab_zoom/condition.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/bim_collab_zoom/constants.py` & `somcreator-1.7.2/src/SOMcreator/external_software/bim_collab_zoom/constants.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/bim_collab_zoom/modelcheck.py` & `somcreator-1.7.2/src/SOMcreator/external_software/bim_collab_zoom/modelcheck.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/bim_collab_zoom/rule.py` & `somcreator-1.7.2/src/SOMcreator/external_software/bim_collab_zoom/rule.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/card1.py` & `somcreator-1.7.2/src/SOMcreator/external_software/card1.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/desite/__init__.py` & `somcreator-1.7.2/src/SOMcreator/external_software/desite/__init__.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/desite/attribute_json.py` & `somcreator-1.7.2/src/SOMcreator/external_software/desite/attribute_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 import json
 import os
 from ... import classes
 from ...constants import json_constants, value_constants
+from ...external_software import xml
 
 
 def _iter_attributes(property_set: classes.PropertySet, pset_dict: dict) -> None:
     for attribute in property_set.attributes:
         pset_dict[attribute.name] = dict()
         attribute_dict = pset_dict[attribute.name]
 
-        attribute_dict[json_constants.DATA_TYPE] = value_constants.XS_DATATYPE_DICT[attribute.data_type]
+        attribute_dict[json_constants.DATA_TYPE] = xml.transform_data_format(attribute.data_type)
         if not attribute.value:
             attribute_dict[json_constants.VALUE_TYPE] = value_constants.EXISTS
         else:
             attribute_dict[json_constants.VALUE_TYPE] = attribute.value_type
         attribute_dict[json_constants.VALUE] = attribute.value
```

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/desite/bill_of_quantities.py` & `somcreator-1.7.2/src/SOMcreator/external_software/desite/bill_of_quantities.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/desite/bookmarks.py` & `somcreator-1.7.2/src/SOMcreator/external_software/desite/bookmarks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 import os
 import jinja2
 from lxml import etree
 from ...Template import HOME_DIR, BOOKMARK_TEMPLATE
 from ... import classes
-from ...constants.value_constants import XS_DATATYPE_DICT
-
+from ...external_software import xml
 
 def _handle_bookmark_list(proj: classes.Project) -> etree.ElementTree:
     xml_bookmarks = etree.Element("bookmarks")
     xml_bookmarks.set("xmlnsxsi", "http://www.w3.org/2001/XMLSchema-instance")
     xml_bookmark_list = etree.SubElement(xml_bookmarks, "cBookmarkList")
 
     obj: classes.Object
@@ -24,34 +23,34 @@
         xml_col = etree.SubElement(xml_bookmark, "col")
         xml_col.set("v", "Type##xs:string")
 
         attribute = obj.ident_attrib
         if attribute is None:
             continue
         xml_col = etree.SubElement(xml_bookmark, "col")
-        data_type = XS_DATATYPE_DICT[attribute.data_type]
+        data_type = xml.transform_data_format(attribute.data_type)
         text = f"{attribute.property_set.name}:{attribute.name}##{data_type}"
         xml_col.set("v", text)
 
         for property_set in obj.property_sets:
             for attribute in property_set.attributes:
                 if attribute != obj.ident_attrib:
                     xml_col = etree.SubElement(xml_bookmark, "col")
-                    data_type = XS_DATATYPE_DICT[attribute.data_type]
+                    data_type = xml.transform_data_format(attribute.data_type)
                     text = f"{property_set.name}:{attribute.name}##{data_type}"
                     xml_col.set("v", text)
     return etree.ElementTree(xml_bookmarks)
 
 
 def _get_attribute_dict(proj: classes.Project) -> dict[str, str]:
     attribute_dict = {}
     for obj in proj.objects:
         for property_set in obj.property_sets:
             for attribute in property_set.attributes:
-                attribute_dict[f"{property_set.name}:{attribute.name}"] = XS_DATATYPE_DICT[attribute.data_type]
+                attribute_dict[f"{property_set.name}:{attribute.name}"] = xml.transform_data_format(attribute.data_type)
 
     return attribute_dict
 
 
 def export_bookmarks(proj: classes.Project, path: str) -> None:
     if not os.path.isdir(path):
         return
```

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/desite/building_structure.py` & `somcreator-1.7.2/src/SOMcreator/external_software/desite/building_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from xml.etree.ElementTree import Element
 
 from lxml import etree
 
 from ... import classes
 from ...constants import value_constants
 from . import handle_header
+from ...external_software import xml
 
 def _handle_section(id_dict, aggregation: classes.Aggregation, xml_item: Element) -> None:
     xml_child = etree.SubElement(xml_item, "section")
     id_dict[aggregation] = aggregation.uuid
     xml_child.set("ID", aggregation.uuid)
     xml_child.set("name", aggregation.object.name)
     xml_child.set("pre", "")
@@ -54,15 +55,15 @@
     for attribute in classes.Attribute:
         # use attribute_text instead of attribute to remove duplicates
         attribute_text = f"{attribute.property_set.name}:{attribute.name}"
         if attribute_text not in attribute_dict:
             xml_ptype = etree.SubElement(xml_property_type_section, "ptype")
             xml_ptype.set("key", str(i))
             xml_ptype.set("name", attribute_text)
-            xml_ptype.set("datatype", value_constants.XS_DATATYPE_DICT[attribute.data_type])
+            xml_ptype.set("datatype", xml.transform_data_format(attribute.data_type))
             xml_ptype.set("unit", "")
             xml_ptype.set("inh", "false")
             attribute_dict[attribute_text] = i
             i += 1
 
     return attribute_dict
```

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/desite/modelcheck.py` & `somcreator-1.7.2/src/SOMcreator/external_software/desite/modelcheck.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from xml.etree.ElementTree import Element
 
 import jinja2
 from lxml import etree
 from typing import TypedDict
 
 from . import handle_header, output_date_time
-from ...constants.value_constants import XS_DATATYPE_DICT
+from ...external_software import xml
 from ..bim_collab_zoom.rule import merge_list
 from ... import classes, constants, Template
 from ...constants import json_constants, value_constants
 
 JS_EXPORT = "JS"
 TABLE_EXPORT = "TABLE"
 
@@ -177,15 +177,15 @@
             return
         xml_checkrun = _handle_checkrun(xml_container, obj.name, author)
         xml_rule = _handle_rule(xml_checkrun, "Attributes")
         xml_attribute_rule_list = _handle_attribute_rule_list(xml_rule)
         xml_rule_script = _handle_rule_script(xml_attribute_rule_list, name=obj.name)
         xml_code = _handle_code(xml_rule_script)
         cdata_code = template.render(pset_dict=pset_dict, constants=value_constants,
-                                     ignore_pset=json_constants.IGNORE_PSET, xs_dict=XS_DATATYPE_DICT)
+                                     ignore_pset=json_constants.IGNORE_PSET, xs_dict=xml.DATA_TYPE_MAPPING_DICT)
         xml_code.text = cdata_code
         _handle_rule(xml_checkrun, "UniquePattern")
 
         xml_object_dict[xml_checkrun] = obj
 
     def create_table_object(xml_container):
         obj, pset_dict, abort = check_basics(parent_obj)
@@ -222,15 +222,15 @@
     pattern = "||".join(f">={v_min}&&<={v_max}" for v_min, v_max in sorted_range_list)
     return pattern
 
 
 def _build_basics_rule_item(xml_parent: etree.Element, attribute: classes.Attribute) -> etree.Element:
     xml_attrib = etree.SubElement(xml_parent, "ruleItem")
     xml_attrib.set("ID", attribute.uuid)
-    data_type = XS_DATATYPE_DICT[attribute.data_type]
+    data_type = xml.transform_data_format(attribute.data_type)
     xml_attrib.set("name", f"{attribute.property_set.name}:{attribute.name}##{data_type}")
     xml_attrib.set("type", "simple")
     return xml_attrib
 
 
 def _handle_rule_item_attribute(xml_parent: etree.Element, attribute: classes.Attribute):
     xml_attrib = _build_basics_rule_item(xml_parent, attribute)
@@ -356,15 +356,15 @@
     rule_script.set("active", "true")
     rule_script.set("resume", "false")
     code = etree.SubElement(rule_script, "code")
     code.text = str(template.render(pset_name=main_pset, attribute_name=main_attribute))
 
 
 def _handle_attribute_rule(attribute: classes.Attribute) -> str:
-    data_type = XS_DATATYPE_DICT[attribute.data_type]
+    data_type = xml.transform_data_format(attribute.data_type)
     pset_name = attribute.property_set.name
 
     if attribute.value_type == value_constants.RANGE:
         row = ["R", "", f"{pset_name}:{attribute.name}", data_type, "*", f"Pruefung"]
         return ";".join(row)
 
     if not attribute.value:
@@ -384,15 +384,15 @@
     xml_checkrun = _handle_checkrun(base_xml_container, "Main Check", author)
     xml_rule = _handle_rule(xml_checkrun, "Attributes")
     xml_attribute_rule_list = _handle_attribute_rule_list(xml_rule)
     xml_rule_script = _handle_rule_script(xml_attribute_rule_list, name="Main Check")
     xml_code = _handle_code(xml_rule_script)
     cdata_code = template.render(object_dict=required_data_dict, main_pset=main_pset, main_attrib=main_attrib,
                                  constants=value_constants,
-                                 ignore_pset=json_constants.IGNORE_PSET, xs_dict=XS_DATATYPE_DICT)
+                                 ignore_pset=json_constants.IGNORE_PSET, xs_dict=xml.DATA_TYPE_MAPPING_DICT)
     xml_code.text = cdata_code
     _handle_rule(xml_checkrun, "UniquePattern")
     return {xml_checkrun: None}
 
 
 def build_full_data_dict(proj: classes.Project) -> dict[
     classes.Object, dict[classes.PropertySet, list[classes.Attribute]]]:
@@ -437,15 +437,15 @@
     lines.append(";".join(["#", f"Created by SOMcreator v{__version__}"]))
     lines.append("H;Property Name;;Data Type;Rule;Comment")
 
     for obj, pset_dict in required_data_dict.items():
         if obj.ident_attrib is None:
             continue
         ident_attrib = f"{obj.ident_attrib.property_set.name}:{obj.ident_attrib.name}"
-        data_type = XS_DATATYPE_DICT[obj.ident_attrib.data_type]
+        data_type = xml.transform_data_format(obj.ident_attrib.data_type)
         lines.append(";".join(
             ["C", ident_attrib, "", data_type, f"'{obj.ident_value}'", f"Nach Objekt {obj.name} filtern"]))
 
         for pset, attribute_list in pset_dict.items():
             for attribute in attribute_list:
                 if attribute.value_type != value_constants.RANGE:
                     lines.append(_handle_attribute_rule(attribute))
```

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/revit.py` & `somcreator-1.7.2/src/SOMcreator/external_software/revit.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/external_software/vestra.py` & `somcreator-1.7.2/src/SOMcreator/external_software/vestra.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from lxml import etree, builder
 from openpyxl import load_workbook
 
 from .. import classes
-from .. constants.value_constants import XS_DATATYPE_DICT
+from ..external_software import xml
 
 def create_mapping(excel_path: str, folder_path: str, project: classes.Project) -> None:
     def create_xml(name: str, obj: classes.Object):
         xsd = "http://www.w3.org/2001/XMLSchema"
         xsi = "http://www.w3.org/2001/XMLSchema-instance"
 
         def create_key_rule() -> None:
@@ -31,15 +31,16 @@
                     xml_key = etree.SubElement(xml_manipulation_base, "Key", )
                     xml_key.text = attribut.name
                     xml_value = etree.SubElement(xml_manipulation_base, "Value", )
                     if attribut == obj.ident_attrib:
                         xml_value.text = attribut.value[0]
                     else:
                         xml_value.text = ""
-                    xml_value.set(f"{{{xsi}}}type", XS_DATATYPE_DICT[attribut.data_type].replace("xs:", "xsd:"))
+                    xml_data_type = xml.transform_data_format(attribut.data_type)
+                    xml_value.set(f"{{{xsi}}}type", xml_data_type.replace("xs:", "xsd:"))
 
         element_maker = builder.ElementMaker(nsmap={"xsd": xsd, "xsi": xsi})
         xml_role = element_maker.Role()
         xml_name = etree.SubElement(xml_role, "Name")
         xml_name.text = name
         xml_rules = etree.SubElement(xml_role, "Rules")
         xml_manipulation_rule = etree.SubElement(xml_rules, "ManipulationRule")
```

### Comparing `somcreator-1.7.1/src/SOMcreator/filehandling/aggregation.py` & `somcreator-1.7.2/src/SOMcreator/filehandling/aggregation.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/filehandling/attribute.py` & `somcreator-1.7.2/src/SOMcreator/filehandling/attribute.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/filehandling/constants.py` & `somcreator-1.7.2/src/SOMcreator/filehandling/constants.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/filehandling/core.py` & `somcreator-1.7.2/src/SOMcreator/filehandling/core.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/filehandling/inheritance.py` & `somcreator-1.7.2/src/SOMcreator/filehandling/inheritance.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/filehandling/obj.py` & `somcreator-1.7.2/src/SOMcreator/filehandling/obj.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/filehandling/predefined_pset.py` & `somcreator-1.7.2/src/SOMcreator/filehandling/predefined_pset.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/filehandling/project.py` & `somcreator-1.7.2/src/SOMcreator/filehandling/project.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/filehandling/property_set.py` & `somcreator-1.7.2/src/SOMcreator/filehandling/property_set.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/filehandling/typing.py` & `somcreator-1.7.2/src/SOMcreator/filehandling/typing.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/ifc_modification/grouping.py` & `somcreator-1.7.2/src/SOMcreator/ifc_modification/grouping.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/tool/export_excel.py` & `somcreator-1.7.2/src/SOMcreator/tool/export_excel.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/tool/ifctosql.py` & `somcreator-1.7.2/src/SOMcreator/tool/ifctosql.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/tool/parsesql.py` & `somcreator-1.7.2/src/SOMcreator/tool/parsesql.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator/tools/merge_projects.py` & `somcreator-1.7.2/src/SOMcreator/tools/merge_projects.py`

 * *Files identical despite different names*

### Comparing `somcreator-1.7.1/src/SOMcreator.egg-info/PKG-INFO` & `somcreator-1.7.2/src/SOMcreator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.7.1
+Version: 1.7.2
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `somcreator-1.7.1/src/SOMcreator.egg-info/SOURCES.txt` & `somcreator-1.7.2/src/SOMcreator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 src/SOMcreator/external_software/bim_collab_zoom/rule.py
 src/SOMcreator/external_software/desite/__init__.py
 src/SOMcreator/external_software/desite/attribute_json.py
 src/SOMcreator/external_software/desite/bill_of_quantities.py
 src/SOMcreator/external_software/desite/bookmarks.py
 src/SOMcreator/external_software/desite/building_structure.py
 src/SOMcreator/external_software/desite/modelcheck.py
+src/SOMcreator/external_software/xml/__init__.py
 src/SOMcreator/filehandling/__init__.py
 src/SOMcreator/filehandling/aggregation.py
 src/SOMcreator/filehandling/attribute.py
 src/SOMcreator/filehandling/constants.py
 src/SOMcreator/filehandling/core.py
 src/SOMcreator/filehandling/inheritance.py
 src/SOMcreator/filehandling/obj.py
```

