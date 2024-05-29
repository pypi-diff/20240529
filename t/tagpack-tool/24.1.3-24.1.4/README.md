# Comparing `tmp/tagpack_tool-24.1.3.tar.gz` & `tmp/tagpack_tool-24.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagpack_tool-24.1.3.tar", last modified: Mon Apr 29 08:57:40 2024, max compression
+gzip compressed data, was "tagpack_tool-24.1.4.tar", last modified: Wed May 29 12:49:59 2024, max compression
```

## Comparing `tagpack_tool-24.1.3.tar` & `tagpack_tool-24.1.4.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.647755 tagpack_tool-24.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.623755 tagpack_tool-24.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.627755 tagpack_tool-24.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/.github/workflows/test_and_build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    15448 2024-04-29 08:57:40.647755 tagpack_tool-24.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.631755 tagpack_tool-24.1.3/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/docker/env.template
--rwxr-xr-x   0 runner    (1001) docker     (127)     1631 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/docker/init.sh
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/docker/postgres-conf.sql.template
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/docker-compose.monitoring.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.631755 tagpack_tool-24.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.631755 tagpack_tool-24.1.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10106 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-29 08:57:40.647755 tagpack_tool-24.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.623755 tagpack_tool-24.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.635755 tagpack_tool-24.1.3/src/tagpack/
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/actorpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/actorpack_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    59848 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/cmd_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.635755 tagpack_tool-24.1.3/src/tagpack/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/conf/actorpack_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/conf/ks_map.json.template
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/conf/tagpack_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/confidence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.635755 tagpack_tool-24.1.3/src/tagpack/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/db/abuses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    20452 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/db/concepts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/db/confidence.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/db/countries.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10752 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/db/entities.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/db/tagstore_schema.sql
--rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/graphsense.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    21030 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/tagpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/tagpack_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    37080 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/tagstore.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/src/tagpack/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.643755 tagpack_tool-24.1.3/src/tagpack_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15448 2024-04-29 08:57:40.000000 tagpack_tool-24.1.3/src/tagpack_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-29 08:57:40.000000 tagpack_tool-24.1.3/src/tagpack_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:57:40.000000 tagpack_tool-24.1.3/src/tagpack_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 08:57:40.000000 tagpack_tool-24.1.3/src/tagpack_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:56:38.000000 tagpack_tool-24.1.3/src/tagpack_tool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-29 08:57:40.000000 tagpack_tool-24.1.3/src/tagpack_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 08:57:40.000000 tagpack_tool-24.1.3/src/tagpack_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.639755 tagpack_tool-24.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/test_actorpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/test_actorpack_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    19674 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/test_tagpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/test_tagpack_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/test_tagstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.623755 tagpack_tool-24.1.3/tests/testfiles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.639755 tagpack_tool-24.1.3/tests/testfiles/actors/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/actors/ex.actorpack.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.639755 tagpack_tool-24.1.3/tests/testfiles/simple/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/simple/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/simple/duplicate_tag.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/simple/empty_tag_list.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/simple/ex_addr_tagpack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/simple/multiple_tags_for_address.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/simple/with_concepts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.639755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.623755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion/2021/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.639755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion/2021/01/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion/2021/01/20210101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion/2021/01/20210102.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.639755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion/2021/01/special/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion/2021/01/special/20210106-special.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.639755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion/2021/02/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion/2021/02/20210201.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion/header.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.623755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_missing_header/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.623755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_missing_header/2021/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.643755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_missing_header/2021/01/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_missing_header/2021/01/20210101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_missing_header/2021/01/20210102.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.643755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_missing_header/2021/01/special/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_missing_header/2021/01/special/20210106-special.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.643755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_missing_header/2021/02/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_missing_header/2021/02/20210201.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.643755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_multiple/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.623755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_multiple/2021/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.643755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_multiple/2021/01/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_multiple/2021/01/20210101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_multiple/2021/01/20210102.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_multiple/2021/01/header.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.643755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_multiple/2021/01/special/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_multiple/2021/01/special/20210106-special.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:57:40.643755 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_multiple/2021/02/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_multiple/2021/02/20210201.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tests/testfiles/yaml_inclusion_multiple/header.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-29 08:56:32.000000 tagpack_tool-24.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.824283 tagpack_tool-24.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.804283 tagpack_tool-24.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.808282 tagpack_tool-24.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/.github/workflows/test_and_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    15448 2024-05-29 12:49:59.824283 tagpack_tool-24.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.812283 tagpack_tool-24.1.4/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/docker/env.template
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1631 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/docker/init.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/docker/postgres-conf.sql.template
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/docker-compose.monitoring.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.812283 tagpack_tool-24.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.812283 tagpack_tool-24.1.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10106 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-29 12:49:59.828283 tagpack_tool-24.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.804283 tagpack_tool-24.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.816283 tagpack_tool-24.1.4/src/tagpack/
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/actorpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/actorpack_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59848 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/cmd_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.816283 tagpack_tool-24.1.4/src/tagpack/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/conf/actorpack_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/conf/ks_map.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/conf/tagpack_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/confidence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.816283 tagpack_tool-24.1.4/src/tagpack/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/db/abuses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    20452 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/db/concepts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/db/confidence.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/db/countries.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10752 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/db/entities.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/db/tagstore_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/graphsense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21030 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/tagpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/tagpack_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37080 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/tagstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/src/tagpack/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.824283 tagpack_tool-24.1.4/src/tagpack_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15448 2024-05-29 12:49:59.000000 tagpack_tool-24.1.4/src/tagpack_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-29 12:49:59.000000 tagpack_tool-24.1.4/src/tagpack_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:49:59.000000 tagpack_tool-24.1.4/src/tagpack_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 12:49:59.000000 tagpack_tool-24.1.4/src/tagpack_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:48:53.000000 tagpack_tool-24.1.4/src/tagpack_tool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-29 12:49:59.000000 tagpack_tool-24.1.4/src/tagpack_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 12:49:59.000000 tagpack_tool-24.1.4/src/tagpack_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.820283 tagpack_tool-24.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/test_actorpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/test_actorpack_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19674 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/test_tagpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/test_tagpack_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/test_tagstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.808282 tagpack_tool-24.1.4/tests/testfiles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.820283 tagpack_tool-24.1.4/tests/testfiles/actors/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/actors/ex.actorpack.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.820283 tagpack_tool-24.1.4/tests/testfiles/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/simple/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/simple/duplicate_tag.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/simple/empty_tag_list.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/simple/ex_addr_tagpack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/simple/multiple_tags_for_address.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/simple/with_concepts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.820283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.804283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion/2021/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.820283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion/2021/01/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion/2021/01/20210101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion/2021/01/20210102.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.820283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion/2021/01/special/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion/2021/01/special/20210106-special.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.820283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion/2021/02/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion/2021/02/20210201.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion/header.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.804283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_missing_header/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.804283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_missing_header/2021/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.820283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_missing_header/2021/01/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_missing_header/2021/01/20210101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_missing_header/2021/01/20210102.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.820283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_missing_header/2021/01/special/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_missing_header/2021/01/special/20210106-special.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.820283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_missing_header/2021/02/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_missing_header/2021/02/20210201.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.824283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_multiple/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.808282 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_multiple/2021/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.824283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_multiple/2021/01/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_multiple/2021/01/20210101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_multiple/2021/01/20210102.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_multiple/2021/01/header.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.824283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_multiple/2021/01/special/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_multiple/2021/01/special/20210106-special.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:49:59.824283 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_multiple/2021/02/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_multiple/2021/02/20210201.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tests/testfiles/yaml_inclusion_multiple/header.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-29 12:48:43.000000 tagpack_tool-24.1.4/tox.ini
```

### Comparing `tagpack_tool-24.1.3/.coveragerc` & `tagpack_tool-24.1.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/.github/workflows/pypi-publish.yaml` & `tagpack_tool-24.1.4/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/.github/workflows/release.yaml` & `tagpack_tool-24.1.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/.github/workflows/test_and_build.yaml` & `tagpack_tool-24.1.4/.github/workflows/test_and_build.yaml`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/.gitignore` & `tagpack_tool-24.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/.pre-commit-config.yaml` & `tagpack_tool-24.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/CHANGELOG.md` & `tagpack_tool-24.1.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+
+## [24.01.4] 2024-05-29
+### fixed
+- clustermappings for eth did not work
+
 ## [24.01.3] 2024-03-29
 ### changed
 - add new concept for tokens (defi_token)
 
 ## [24.01.2] 2024-03-22
 ### changed
 - allow all concepts to be used in category field (align category and concepts)
```

### Comparing `tagpack_tool-24.1.3/LICENSE` & `tagpack_tool-24.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/Makefile` & `tagpack_tool-24.1.4/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 SHELL := /bin/bash
 PROJECT := tagpack-tool
 VENV := .venv
-RELEASE := 'v24.01.3'
+RELEASE := 'v24.01.4'
 # RELEASESEM := 'v1.9.0'
 
 all: format lint test build
 
 tag-version:
 	#-git diff --exit-code && git diff --staged --exit-code && git tag -a $(RELEASESEM) -m 'Release $(RELEASE)' || (echo "Repo is dirty please commit first" && exit 1)
 	git diff --exit-code && git diff --staged --exit-code && git tag -a $(RELEASE) -m 'Release $(RELEASE)' || (echo "Repo is dirty please commit first" && exit 1)
```

### Comparing `tagpack_tool-24.1.3/PKG-INFO` & `tagpack_tool-24.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagpack-tool
-Version: 24.1.3
+Version: 24.1.4
 Summary: GraphSense TagPack Management Tool
 Home-page: https://graphsense.github.io/
 Author: GraphSense Core Team
 Author-email: tech@ikna.io
 License: MIT
 Project-URL: Source, https://github.com/graphsense/graphsense-tagpack-tool
 Project-URL: Changelog, https://github.com/graphsense/graphsense-tagpack-tool/blob/master/CHANGELOG.md
```

### Comparing `tagpack_tool-24.1.3/README.md` & `tagpack_tool-24.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/docker/init.sh` & `tagpack_tool-24.1.4/docker/init.sh`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/docker-compose.monitoring.yml` & `tagpack_tool-24.1.4/docker-compose.monitoring.yml`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/docker-compose.yml` & `tagpack_tool-24.1.4/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/docs/Makefile` & `tagpack_tool-24.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/docs/conf.py` & `tagpack_tool-24.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/docs/index.md` & `tagpack_tool-24.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/setup.cfg` & `tagpack_tool-24.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/setup.py` & `tagpack_tool-24.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/__init__.py` & `tagpack_tool-24.1.4/src/tagpack/__init__.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/actorpack.py` & `tagpack_tool-24.1.4/src/tagpack/actorpack.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/actorpack_schema.py` & `tagpack_tool-24.1.4/src/tagpack/actorpack_schema.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/cli.py` & `tagpack_tool-24.1.4/src/tagpack/cli.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/cmd_utils.py` & `tagpack_tool-24.1.4/src/tagpack/cmd_utils.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/conf/actorpack_schema.yaml` & `tagpack_tool-24.1.4/src/tagpack/conf/actorpack_schema.yaml`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/conf/tagpack_schema.yaml` & `tagpack_tool-24.1.4/src/tagpack/conf/tagpack_schema.yaml`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/confidence.py` & `tagpack_tool-24.1.4/src/tagpack/confidence.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/db/abuses.yaml` & `tagpack_tool-24.1.4/src/tagpack/db/abuses.yaml`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/db/concepts.yaml` & `tagpack_tool-24.1.4/src/tagpack/db/concepts.yaml`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/db/confidence.csv` & `tagpack_tool-24.1.4/src/tagpack/db/confidence.csv`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/db/countries.csv` & `tagpack_tool-24.1.4/src/tagpack/db/countries.csv`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/db/entities.yaml` & `tagpack_tool-24.1.4/src/tagpack/db/entities.yaml`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/db/tagstore_schema.sql` & `tagpack_tool-24.1.4/src/tagpack/db/tagstore_schema.sql`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/graphsense.py` & `tagpack_tool-24.1.4/src/tagpack/graphsense.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 
         statement = self.session.prepare(query)
         parameters = df_temp[["address_prefix", "address"]].to_records(index=False)
 
         result = self._execute_query(statement, parameters)
 
         if currency == "ETH":
-            result["address"] = result["address"].apply(lambda x: eth_address_to_hex(x))
+            result["address"] = result["address"].apply(eth_address_to_hex_str)
         elif currency == "TRX":
             # convert evm to t-style address
             result["address"] = result["address"].apply(try_convert_to_tron)
 
         return result
 
     def get_cluster_ids(self, df: DataFrame, currency: str) -> DataFrame:
```

### Comparing `tagpack_tool-24.1.3/src/tagpack/schema.py` & `tagpack_tool-24.1.4/src/tagpack/schema.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/tagpack.py` & `tagpack_tool-24.1.4/src/tagpack/tagpack.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/tagpack_schema.py` & `tagpack_tool-24.1.4/src/tagpack/tagpack_schema.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/tagstore.py` & `tagpack_tool-24.1.4/src/tagpack/tagstore.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/taxonomy.py` & `tagpack_tool-24.1.4/src/tagpack/taxonomy.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack/utils.py` & `tagpack_tool-24.1.4/src/tagpack/utils.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack_tool.egg-info/PKG-INFO` & `tagpack_tool-24.1.4/src/tagpack_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagpack-tool
-Version: 24.1.3
+Version: 24.1.4
 Summary: GraphSense TagPack Management Tool
 Home-page: https://graphsense.github.io/
 Author: GraphSense Core Team
 Author-email: tech@ikna.io
 License: MIT
 Project-URL: Source, https://github.com/graphsense/graphsense-tagpack-tool
 Project-URL: Changelog, https://github.com/graphsense/graphsense-tagpack-tool/blob/master/CHANGELOG.md
```

### Comparing `tagpack_tool-24.1.3/src/tagpack_tool.egg-info/SOURCES.txt` & `tagpack_tool-24.1.4/src/tagpack_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/src/tagpack_tool.egg-info/requires.txt` & `tagpack_tool-24.1.4/src/tagpack_tool.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/tests/test_actorpack.py` & `tagpack_tool-24.1.4/tests/test_actorpack.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/tests/test_actorpack_schema.py` & `tagpack_tool-24.1.4/tests/test_actorpack_schema.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/tests/test_main.py` & `tagpack_tool-24.1.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/tests/test_tagpack.py` & `tagpack_tool-24.1.4/tests/test_tagpack.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/tests/test_tagpack_schema.py` & `tagpack_tool-24.1.4/tests/test_tagpack_schema.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/tests/test_tagstore.py` & `tagpack_tool-24.1.4/tests/test_tagstore.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/tests/test_utils.py` & `tagpack_tool-24.1.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tagpack_tool-24.1.3/tox.ini` & `tagpack_tool-24.1.4/tox.ini`

 * *Files identical despite different names*

