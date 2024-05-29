# Comparing `tmp/crunch_uml-0.2.5.tar.gz` & `tmp/crunch_uml-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch_uml-0.2.5.tar", last modified: Wed May 29 15:27:32 2024, max compression
+gzip compressed data, was "crunch_uml-0.2.7.tar", last modified: Wed May 29 17:44:21 2024, max compression
```

## Comparing `crunch_uml-0.2.5.tar` & `crunch_uml-0.2.7.tar`

### file list

```diff
@@ -1,83 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:27:32.193184 crunch_uml-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-29 15:27:32.193184 crunch_uml-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:27:32.153185 crunch_uml-0.2.5/crunch_uml/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/db.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/excpetions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:27:32.153185 crunch_uml-0.2.5/crunch_uml/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/parsers/eaxmiparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/parsers/multiple_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15512 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/parsers/xmiparser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:27:32.157184 crunch_uml-0.2.5/crunch_uml/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/renderers/jinja2renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/renderers/lodrenderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/renderers/pandasrenderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/renderers/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/renderers/sqlarenderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/renderers/xlsxrenderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:27:32.157184 crunch_uml-0.2.5/crunch_uml/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/templates/ddas_markdown.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/templates/ggm_markdown.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/templates/ggm_sqlalchemy.j2
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/crunch_uml/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:27:32.189185 crunch_uml-0.2.5/crunch_uml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-29 15:27:32.000000 crunch_uml-0.2.5/crunch_uml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-29 15:27:32.000000 crunch_uml-0.2.5/crunch_uml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:27:32.000000 crunch_uml-0.2.5/crunch_uml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-29 15:27:32.000000 crunch_uml-0.2.5/crunch_uml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 15:27:32.000000 crunch_uml-0.2.5/crunch_uml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 15:27:32.000000 crunch_uml-0.2.5/crunch_uml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:27:32.193184 crunch_uml-0.2.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1735 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:27:32.149185 crunch_uml-0.2.5/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:27:32.189185 crunch_uml-0.2.5/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)    39363 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/AlleRelatieSitiuaties.xml
--rw-r--r--   0 runner    (1001) docker     (127)    76406 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/GGM_Erfgoed.xml
--rw-r--r--   0 runner    (1001) docker     (127)   145378 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/GGM_Monumenten_EA2.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)   224799 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/GGM_Onderwijs_EA2.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    44609 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/GGM_Onderwijs_XMI.2.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/Gemeentelijk Gegevensmodel RDF
--rw-r--r--   0 runner    (1001) docker     (127) 21424811 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/Gemeentelijk Gegevensmodel.xml
--rw-r--r--   0 runner    (1001) docker     (127)    24384 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/Materialize_Generalizations.xml
--rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/Monumenten.json
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/Monumenten_changes.json
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/Onderwijs.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    10938 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/Onderwijs_changes.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/RelTestExtra.json
--rw-r--r--   0 runner    (1001) docker     (127)    58976 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/RelationTest.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1540096 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/TestProject.qea
--rw-r--r--   0 runner    (1001) docker     (127)    23963 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/Voorbeeld Componenten.xml
--rw-r--r--   0 runner    (1001) docker     (127)   541253 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/Voorbeeld Generatie Relaties
--rw-r--r--   0 runner    (1001) docker     (127)   541253 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/data/Voorbeeld Generatie Relaties.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:27:32.189185 crunch_uml-0.2.5/test/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_01_import_monumenten.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_01b_import_url_monumenten.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_02_alle_relatie_situaties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_03_relations_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_04_import_onderwijs.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_05_import_onderwijs empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_05_json_parser_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_06_xlsx_parser_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_07_relations_test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_08_markdown_monumenten_onderwijs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_09_lod_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_10_import_multiple_same_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_10a_import_multiple_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_11_monumenten_cascade_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_12_copy_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_12a_copy_onderwijs.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-29 15:27:00.000000 crunch_uml-0.2.5/test/unit/test_12b_copy_and_materialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:44:21.878937 crunch_uml-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-29 17:44:21.878937 crunch_uml-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:44:21.838937 crunch_uml-0.2.7/crunch_uml/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/excpetions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:44:21.838937 crunch_uml-0.2.7/crunch_uml/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/parsers/eaxmiparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/parsers/multiple_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15512 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/parsers/xmiparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:44:21.842937 crunch_uml-0.2.7/crunch_uml/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/renderers/jinja2renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/renderers/lodrenderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/renderers/pandasrenderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/renderers/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/renderers/sqlarenderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/renderers/xlsxrenderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:44:21.842937 crunch_uml-0.2.7/crunch_uml/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/templates/ddas_markdown.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/templates/ggm_markdown.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/templates/ggm_sqlalchemy.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:44:21.842937 crunch_uml-0.2.7/crunch_uml/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/transformers/copytransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/transformers/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/crunch_uml/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:44:21.878937 crunch_uml-0.2.7/crunch_uml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-29 17:44:21.000000 crunch_uml-0.2.7/crunch_uml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-29 17:44:21.000000 crunch_uml-0.2.7/crunch_uml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:44:21.000000 crunch_uml-0.2.7/crunch_uml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-29 17:44:21.000000 crunch_uml-0.2.7/crunch_uml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 17:44:21.000000 crunch_uml-0.2.7/crunch_uml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 17:44:21.000000 crunch_uml-0.2.7/crunch_uml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:44:21.878937 crunch_uml-0.2.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1735 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:44:21.834936 crunch_uml-0.2.7/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:44:21.874937 crunch_uml-0.2.7/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    39363 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/test/data/AlleRelatieSitiuaties.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    76406 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/test/data/GGM_Erfgoed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   145378 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/test/data/GGM_Monumenten_EA2.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   224799 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/test/data/GGM_Onderwijs_EA2.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    44609 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/test/data/GGM_Onderwijs_XMI.2.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-29 17:43:49.000000 crunch_uml-0.2.7/test/data/Gemeentelijk Gegevensmodel RDF
+-rw-r--r--   0 runner    (1001) docker     (127) 21424811 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/data/Gemeentelijk Gegevensmodel.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    24384 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/data/Materialize_Generalizations.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/data/Monumenten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/data/Monumenten_changes.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/data/Onderwijs.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    10938 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/data/Onderwijs_changes.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/data/RelTestExtra.json
+-rw-r--r--   0 runner    (1001) docker     (127)    58976 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/data/RelationTest.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1540096 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/data/TestProject.qea
+-rw-r--r--   0 runner    (1001) docker     (127)    23963 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/data/Voorbeeld Componenten.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   541253 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/data/Voorbeeld Generatie Relaties
+-rw-r--r--   0 runner    (1001) docker     (127)   541253 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/data/Voorbeeld Generatie Relaties.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:44:21.878937 crunch_uml-0.2.7/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_01_import_monumenten.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_01b_import_url_monumenten.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_02_alle_relatie_situaties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_03_relations_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_04_import_onderwijs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_05_import_onderwijs empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_05_json_parser_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_06_xlsx_parser_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_07_relations_test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_08_markdown_monumenten_onderwijs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_09_lod_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_10_import_multiple_same_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_10a_import_multiple_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_11_monumenten_cascade_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_12_copy_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_12a_copy_onderwijs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-29 17:43:50.000000 crunch_uml-0.2.7/test/unit/test_12b_copy_and_materialize.py
```

### Comparing `crunch_uml-0.2.5/LICENSE` & `crunch_uml-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/PKG-INFO` & `crunch_uml-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crunch_uml
-Version: 0.2.5
+Version: 0.2.7
 Summary: Reads UML Class model from multiple formats (including XMI) and renders them to other formats (including Markdown).
 Home-page: http://github.com/brienen/crunch_uml
 Author: Arjen Brienen
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `crunch_uml-0.2.5/README.md` & `crunch_uml-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/cli.py` & `crunch_uml-0.2.7/crunch_uml/cli.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/db.py` & `crunch_uml-0.2.7/crunch_uml/db.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/parsers/eaxmiparser.py` & `crunch_uml-0.2.7/crunch_uml/parsers/eaxmiparser.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/parsers/multiple_parsers.py` & `crunch_uml-0.2.7/crunch_uml/parsers/multiple_parsers.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/parsers/parser.py` & `crunch_uml-0.2.7/crunch_uml/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/parsers/xmiparser.py` & `crunch_uml-0.2.7/crunch_uml/parsers/xmiparser.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/registry.py` & `crunch_uml-0.2.7/crunch_uml/registry.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/renderers/jinja2renderer.py` & `crunch_uml-0.2.7/crunch_uml/renderers/jinja2renderer.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/renderers/lodrenderer.py` & `crunch_uml-0.2.7/crunch_uml/renderers/lodrenderer.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/renderers/pandasrenderer.py` & `crunch_uml-0.2.7/crunch_uml/renderers/pandasrenderer.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/renderers/renderer.py` & `crunch_uml-0.2.7/crunch_uml/renderers/renderer.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/renderers/sqlarenderer.py` & `crunch_uml-0.2.7/crunch_uml/renderers/sqlarenderer.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/renderers/xlsxrenderer.py` & `crunch_uml-0.2.7/crunch_uml/renderers/xlsxrenderer.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/schema.py` & `crunch_uml-0.2.7/crunch_uml/schema.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/templates/ddas_markdown.j2` & `crunch_uml-0.2.7/crunch_uml/templates/ddas_markdown.j2`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/templates/ggm_markdown.j2` & `crunch_uml-0.2.7/crunch_uml/templates/ggm_markdown.j2`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/templates/ggm_sqlalchemy.j2` & `crunch_uml-0.2.7/crunch_uml/templates/ggm_sqlalchemy.j2`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml/util.py` & `crunch_uml-0.2.7/crunch_uml/util.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/crunch_uml.egg-info/PKG-INFO` & `crunch_uml-0.2.7/crunch_uml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crunch_uml
-Version: 0.2.5
+Version: 0.2.7
 Summary: Reads UML Class model from multiple formats (including XMI) and renders them to other formats (including Markdown).
 Home-page: http://github.com/brienen/crunch_uml
 Author: Arjen Brienen
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `crunch_uml-0.2.5/crunch_uml.egg-info/SOURCES.txt` & `crunch_uml-0.2.7/crunch_uml.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 crunch_uml/renderers/pandasrenderer.py
 crunch_uml/renderers/renderer.py
 crunch_uml/renderers/sqlarenderer.py
 crunch_uml/renderers/xlsxrenderer.py
 crunch_uml/templates/ddas_markdown.j2
 crunch_uml/templates/ggm_markdown.j2
 crunch_uml/templates/ggm_sqlalchemy.j2
+crunch_uml/transformers/copytransformer.py
+crunch_uml/transformers/transformer.py
 test/data/AlleRelatieSitiuaties.xml
 test/data/GGM_Erfgoed.xml
 test/data/GGM_Monumenten_EA2.1.xml
 test/data/GGM_Onderwijs_EA2.1.xml
 test/data/GGM_Onderwijs_XMI.2.1.xml
 test/data/Gemeentelijk Gegevensmodel RDF
 test/data/Gemeentelijk Gegevensmodel.xml
```

### Comparing `crunch_uml-0.2.5/setup.py` & `crunch_uml-0.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = None
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='crunch_uml',
-    version='0.2.5',
+    version='0.2.7',
     description='Reads UML Class model from multiple formats (including XMI) and renders them to other formats (including Markdown).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/brienen/crunch_uml',
     author='Arjen Brienen',
     license='MIT',
     include_package_data=True,
```

### Comparing `crunch_uml-0.2.5/test/data/AlleRelatieSitiuaties.xml` & `crunch_uml-0.2.7/test/data/AlleRelatieSitiuaties.xml`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/GGM_Erfgoed.xml` & `crunch_uml-0.2.7/test/data/GGM_Erfgoed.xml`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/GGM_Monumenten_EA2.1.xml` & `crunch_uml-0.2.7/test/data/GGM_Monumenten_EA2.1.xml`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/GGM_Onderwijs_EA2.1.xml` & `crunch_uml-0.2.7/test/data/GGM_Onderwijs_EA2.1.xml`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/GGM_Onderwijs_XMI.2.1.xml` & `crunch_uml-0.2.7/test/data/GGM_Onderwijs_XMI.2.1.xml`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/Gemeentelijk Gegevensmodel.xml` & `crunch_uml-0.2.7/test/data/Gemeentelijk Gegevensmodel.xml`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/Materialize_Generalizations.xml` & `crunch_uml-0.2.7/test/data/Materialize_Generalizations.xml`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/Monumenten.json` & `crunch_uml-0.2.7/test/data/Monumenten.json`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/Monumenten_changes.json` & `crunch_uml-0.2.7/test/data/Monumenten_changes.json`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/Onderwijs.xlsx` & `crunch_uml-0.2.7/test/data/Onderwijs.xlsx`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/Onderwijs_changes.xlsx` & `crunch_uml-0.2.7/test/data/Onderwijs_changes.xlsx`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/RelTestExtra.json` & `crunch_uml-0.2.7/test/data/RelTestExtra.json`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/RelationTest.xml` & `crunch_uml-0.2.7/test/data/RelationTest.xml`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/TestProject.qea` & `crunch_uml-0.2.7/test/data/TestProject.qea`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/Voorbeeld Componenten.xml` & `crunch_uml-0.2.7/test/data/Voorbeeld Componenten.xml`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/Voorbeeld Generatie Relaties` & `crunch_uml-0.2.7/test/data/Voorbeeld Generatie Relaties`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/data/Voorbeeld Generatie Relaties.xml` & `crunch_uml-0.2.7/test/data/Voorbeeld Generatie Relaties.xml`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_01_import_monumenten.py` & `crunch_uml-0.2.7/test/unit/test_01_import_monumenten.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_01b_import_url_monumenten.py` & `crunch_uml-0.2.7/test/unit/test_01b_import_url_monumenten.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_02_alle_relatie_situaties.py` & `crunch_uml-0.2.7/test/unit/test_02_alle_relatie_situaties.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_03_relations_extended.py` & `crunch_uml-0.2.7/test/unit/test_03_relations_extended.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_04_import_onderwijs.py` & `crunch_uml-0.2.7/test/unit/test_04_import_onderwijs.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_05_import_onderwijs empty.py` & `crunch_uml-0.2.7/test/unit/test_05_import_onderwijs empty.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_05_json_parser_renderer.py` & `crunch_uml-0.2.7/test/unit/test_05_json_parser_renderer.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_06_xlsx_parser_renderer.py` & `crunch_uml-0.2.7/test/unit/test_06_xlsx_parser_renderer.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_07_relations_test_json.py` & `crunch_uml-0.2.7/test/unit/test_07_relations_test_json.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_08_markdown_monumenten_onderwijs.py` & `crunch_uml-0.2.7/test/unit/test_08_markdown_monumenten_onderwijs.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_09_lod_renderer.py` & `crunch_uml-0.2.7/test/unit/test_09_lod_renderer.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_10_import_multiple_same_schema.py` & `crunch_uml-0.2.7/test/unit/test_10_import_multiple_same_schema.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_10a_import_multiple_schema.py` & `crunch_uml-0.2.7/test/unit/test_10a_import_multiple_schema.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_11_monumenten_cascade_delete.py` & `crunch_uml-0.2.7/test/unit/test_11_monumenten_cascade_delete.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_12_copy_structure.py` & `crunch_uml-0.2.7/test/unit/test_12_copy_structure.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_12a_copy_onderwijs.py` & `crunch_uml-0.2.7/test/unit/test_12a_copy_onderwijs.py`

 * *Files identical despite different names*

### Comparing `crunch_uml-0.2.5/test/unit/test_12b_copy_and_materialize.py` & `crunch_uml-0.2.7/test/unit/test_12b_copy_and_materialize.py`

 * *Files identical despite different names*

