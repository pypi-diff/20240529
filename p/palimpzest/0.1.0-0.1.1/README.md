# Comparing `tmp/palimpzest-0.1.0.tar.gz` & `tmp/palimpzest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palimpzest-0.1.0.tar", last modified: Tue May 28 21:59:06 2024, max compression
+gzip compressed data, was "palimpzest-0.1.1.tar", last modified: Wed May 29 18:46:22 2024, max compression
```

## Comparing `palimpzest-0.1.0.tar` & `palimpzest-0.1.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.322499 palimpzest-0.1.0/
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1079 2024-05-28 21:48:17.000000 palimpzest-0.1.0/LICENSE
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-28 21:59:06.322293 palimpzest-0.1.0/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)     7187 2024-05-28 21:48:17.000000 palimpzest-0.1.0/README.md
--rw-r--r--   0 matthewrusso   (501) staff       (20)     2321 2024-05-28 21:58:15.000000 palimpzest-0.1.0/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-05-28 21:59:06.322534 palimpzest-0.1.0/setup.cfg
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.313133 palimpzest-0.1.0/src/
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.314544 palimpzest-0.1.0/src/cli/
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/cli/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9182 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/cli/cli_main.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.315019 palimpzest-0.1.0/src/palimpzest/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      311 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/__init__.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.315909 palimpzest-0.1.0/src/palimpzest/config/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       27 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/config/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3070 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/config/config.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    12383 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/constants.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.316272 palimpzest-0.1.0/src/palimpzest/corelib/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       48 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/corelib/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3038 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/corelib/functions.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3746 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/corelib/schemas.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.316488 palimpzest-0.1.0/src/palimpzest/datamanager/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       39 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/datamanager/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    10958 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/datamanager/datamanager.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.316711 palimpzest-0.1.0/src/palimpzest/datasources/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/datasources/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     4939 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/datasources/datasources.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/deploy.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.317615 palimpzest-0.1.0/src/palimpzest/elements/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      175 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/elements/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      948 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/elements/aggregatefunction.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    10207 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/elements/elements.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1441 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/elements/filters.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      717 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/elements/functions.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     2254 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/elements/groupbysig.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1666 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/elements/pzlist.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3840 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/elements/records.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.317836 palimpzest-0.1.0/src/palimpzest/execution/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      103 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/execution/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9426 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/execution/execution.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.318185 palimpzest-0.1.0/src/palimpzest/generators/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       52 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/generators/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     7141 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/generators/dspy_utils.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    25348 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/generators/generators.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.318579 palimpzest-0.1.0/src/palimpzest/operators/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       49 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/operators/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    43298 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/operators/operators.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    91407 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/operators/physical.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.318857 palimpzest-0.1.0/src/palimpzest/parallel/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/parallel/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1386 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/parallel/pzmodal.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.319110 palimpzest-0.1.0/src/palimpzest/policy/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/policy/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    11539 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/policy/policy.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.319609 palimpzest-0.1.0/src/palimpzest/profiler/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       75 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/profiler/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     4720 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/profiler/attentive_trim.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     4677 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/profiler/profiler.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    44230 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/profiler/stats.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.319867 palimpzest-0.1.0/src/palimpzest/sampler/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/sampler/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      241 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/sampler/sampler.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.320085 palimpzest-0.1.0/src/palimpzest/sets/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       20 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/sets/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    14395 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/sets/sets.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.320902 palimpzest-0.1.0/src/palimpzest/solver/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/solver/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    30444 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/solver/query_strategies.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    20606 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/solver/solver.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1465 2024-05-24 19:15:09.000000 palimpzest-0.1.0/src/palimpzest/solver/task_descriptors.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.321570 palimpzest-0.1.0/src/palimpzest/tools/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      483 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/tools/README.md
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/tools/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1813 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/tools/allenpdf.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    11036 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/tools/pdfparser.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1229 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/tools/skema_tools.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.321909 palimpzest-0.1.0/src/palimpzest/utils/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       45 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/utils/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9909 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/utils/codegen.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     5778 2024-05-24 18:51:05.000000 palimpzest-0.1.0/src/palimpzest/utils/sandbox.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-28 21:59:06.322067 palimpzest-0.1.0/src/palimpzest.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-28 21:59:06.000000 palimpzest-0.1.0/src/palimpzest.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)     2143 2024-05-28 21:59:06.000000 palimpzest-0.1.0/src/palimpzest.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-05-28 21:59:06.000000 palimpzest-0.1.0/src/palimpzest.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       41 2024-05-28 21:59:06.000000 palimpzest-0.1.0/src/palimpzest.egg-info/entry_points.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)      624 2024-05-28 21:59:06.000000 palimpzest-0.1.0/src/palimpzest.egg-info/requires.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       15 2024-05-28 21:59:06.000000 palimpzest-0.1.0/src/palimpzest.egg-info/top_level.txt
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.478496 palimpzest-0.1.1/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1079 2024-05-29 15:41:00.000000 palimpzest-0.1.1/LICENSE
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-29 18:46:22.478293 palimpzest-0.1.1/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     7187 2024-05-29 15:41:00.000000 palimpzest-0.1.1/README.md
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     2321 2024-05-29 18:46:20.000000 palimpzest-0.1.1/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-05-29 18:46:22.478528 palimpzest-0.1.1/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.468848 palimpzest-0.1.1/src/
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.470313 palimpzest-0.1.1/src/cli/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/cli/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9182 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/cli/cli_main.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.470840 palimpzest-0.1.1/src/palimpzest/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      311 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/__init__.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.471731 palimpzest-0.1.1/src/palimpzest/config/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       27 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/config/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3070 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/config/config.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    12383 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/constants.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.472074 palimpzest-0.1.1/src/palimpzest/corelib/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       48 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/corelib/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3038 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/corelib/functions.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3746 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/corelib/schemas.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.472300 palimpzest-0.1.1/src/palimpzest/datamanager/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       39 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/datamanager/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    11011 2024-05-29 18:18:09.000000 palimpzest-0.1.1/src/palimpzest/datamanager/datamanager.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.472541 palimpzest-0.1.1/src/palimpzest/datasources/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/datasources/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     4939 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/datasources/datasources.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/deploy.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.473462 palimpzest-0.1.1/src/palimpzest/elements/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      175 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/elements/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      948 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/elements/aggregatefunction.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    10207 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/elements/elements.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1441 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/elements/filters.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      717 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/elements/functions.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     2254 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/elements/groupbysig.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1666 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/elements/pzlist.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3840 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/elements/records.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.473693 palimpzest-0.1.1/src/palimpzest/execution/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      112 2024-05-29 01:56:02.000000 palimpzest-0.1.1/src/palimpzest/execution/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    16122 2024-05-29 18:39:47.000000 palimpzest-0.1.1/src/palimpzest/execution/execution.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.474250 palimpzest-0.1.1/src/palimpzest/generators/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       52 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/generators/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     7141 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/generators/dspy_utils.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    25348 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/generators/generators.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.474712 palimpzest-0.1.1/src/palimpzest/operators/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       49 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/operators/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    43298 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/operators/operators.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    91407 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/operators/physical.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.475001 palimpzest-0.1.1/src/palimpzest/parallel/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/parallel/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1386 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/parallel/pzmodal.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.475218 palimpzest-0.1.1/src/palimpzest/policy/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/policy/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    11539 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/policy/policy.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.475713 palimpzest-0.1.1/src/palimpzest/profiler/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       75 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/profiler/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     4720 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/profiler/attentive_trim.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     4677 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/profiler/profiler.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    44230 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/profiler/stats.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.475975 palimpzest-0.1.1/src/palimpzest/sampler/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/sampler/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      241 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/sampler/sampler.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.476214 palimpzest-0.1.1/src/palimpzest/sets/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       20 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/sets/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    14861 2024-05-29 18:07:06.000000 palimpzest-0.1.1/src/palimpzest/sets/sets.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.476909 palimpzest-0.1.1/src/palimpzest/solver/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/solver/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    30444 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/solver/query_strategies.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    20606 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/solver/solver.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1465 2024-05-29 15:41:00.000000 palimpzest-0.1.1/src/palimpzest/solver/task_descriptors.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.477509 palimpzest-0.1.1/src/palimpzest/tools/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      483 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/tools/README.md
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/tools/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1813 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/tools/allenpdf.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    11036 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/tools/pdfparser.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1229 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/tools/skema_tools.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.477881 palimpzest-0.1.1/src/palimpzest/utils/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       45 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/utils/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9909 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/utils/codegen.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     5778 2024-05-24 18:51:05.000000 palimpzest-0.1.1/src/palimpzest/utils/sandbox.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:46:22.478048 palimpzest-0.1.1/src/palimpzest.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-29 18:46:22.000000 palimpzest-0.1.1/src/palimpzest.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     2143 2024-05-29 18:46:22.000000 palimpzest-0.1.1/src/palimpzest.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-05-29 18:46:22.000000 palimpzest-0.1.1/src/palimpzest.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       41 2024-05-29 18:46:22.000000 palimpzest-0.1.1/src/palimpzest.egg-info/entry_points.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      624 2024-05-29 18:46:22.000000 palimpzest-0.1.1/src/palimpzest.egg-info/requires.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       15 2024-05-29 18:46:22.000000 palimpzest-0.1.1/src/palimpzest.egg-info/top_level.txt
```

### Comparing `palimpzest-0.1.0/LICENSE` & `palimpzest-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/PKG-INFO` & `palimpzest-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palimpzest
-Version: 0.1.0
+Version: 0.1.1
 Summary: Palimpzest is a system which enables anyone to process AI-powered analytical queries simply by defining them in a declarative language
 Author-email: MIT DSG Semantic Management Lab <michjc@csail.mit.edu>
 Project-URL: homepage, https://github.com/mitdbg/palimpzest/
 Project-URL: repository, https://https://github.com/mitdbg/palimpzest/
 Keywords: relational,optimization,llm,AI programming,extraction,tools,document,search,integration
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `palimpzest-0.1.0/README.md` & `palimpzest-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/pyproject.toml` & `palimpzest-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "palimpzest"
-version = "0.1.0"
+version = "0.1.1"
 description = "Palimpzest is a system which enables anyone to process AI-powered analytical queries simply by defining them in a declarative language"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["relational", "optimization", "llm", "AI programming", "extraction", "tools", "document", "search", "integration"]
 authors = [
     {name="MIT DSG Semantic Management Lab", email="michjc@csail.mit.edu"},
 ]
```

### Comparing `palimpzest-0.1.0/src/cli/cli_main.py` & `palimpzest-0.1.1/src/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/config/config.py` & `palimpzest-0.1.1/src/palimpzest/config/config.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/constants.py` & `palimpzest-0.1.1/src/palimpzest/constants.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/corelib/functions.py` & `palimpzest-0.1.1/src/palimpzest/corelib/functions.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/corelib/schemas.py` & `palimpzest-0.1.1/src/palimpzest/corelib/schemas.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/datamanager/datamanager.py` & `palimpzest-0.1.1/src/palimpzest/datamanager/datamanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,18 @@
     def putCachedData(self, cacheName, cacheKey, cacheVal):
         self.allCaches.setdefault(cacheName, {})[cacheKey] = cacheVal
 
     def rmCachedData(self, cacheName):
         if cacheName in self.allCaches:
             del self.allCaches[cacheName]
 
+    def rmCache(self):
+        self.allCaches = {}
+
+
 # TODO: possibly rename to the PZManager, as it also manages the current config
 class DataDirectory(metaclass=DataDirectorySingletonMeta):
     """The DataDirectory is a registry of data sources."""
 
     def __init__(self):
         self._registry = {}
         self._cache = {}
```

### Comparing `palimpzest-0.1.0/src/palimpzest/datasources/datasources.py` & `palimpzest-0.1.1/src/palimpzest/datasources/datasources.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/elements/aggregatefunction.py` & `palimpzest-0.1.1/src/palimpzest/elements/aggregatefunction.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/elements/elements.py` & `palimpzest-0.1.1/src/palimpzest/elements/elements.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/elements/filters.py` & `palimpzest-0.1.1/src/palimpzest/elements/filters.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/elements/functions.py` & `palimpzest-0.1.1/src/palimpzest/elements/functions.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/elements/groupbysig.py` & `palimpzest-0.1.1/src/palimpzest/elements/groupbysig.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/elements/pzlist.py` & `palimpzest-0.1.1/src/palimpzest/elements/pzlist.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/elements/records.py` & `palimpzest-0.1.1/src/palimpzest/elements/records.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/generators/dspy_utils.py` & `palimpzest-0.1.1/src/palimpzest/generators/dspy_utils.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/generators/generators.py` & `palimpzest-0.1.1/src/palimpzest/generators/generators.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/operators/operators.py` & `palimpzest-0.1.1/src/palimpzest/operators/operators.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/operators/physical.py` & `palimpzest-0.1.1/src/palimpzest/operators/physical.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/parallel/pzmodal.py` & `palimpzest-0.1.1/src/palimpzest/parallel/pzmodal.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/policy/policy.py` & `palimpzest-0.1.1/src/palimpzest/policy/policy.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/profiler/attentive_trim.py` & `palimpzest-0.1.1/src/palimpzest/profiler/attentive_trim.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/profiler/profiler.py` & `palimpzest-0.1.1/src/palimpzest/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/profiler/stats.py` & `palimpzest-0.1.1/src/palimpzest/profiler/stats.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/sets/sets.py` & `palimpzest-0.1.1/src/palimpzest/sets/sets.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,16 +167,21 @@
     def dumpSyntacticTree(self):
         """Return the syntactic tree of this Set."""
         if isinstance(self._source, DataSource):
             return (self, None)
 
         return (self, self._source.dumpSyntacticTree())
 
-    def getLogicalTree(self) -> LogicalOperator:
+    def getLogicalTree(self, *args, **kwargs) -> LogicalOperator:
         """Return the logical tree of operators on Sets."""
+        # set _num_samples, _scan_start_idx, and _nocache if specified
+        self._num_samples = kwargs.get('num_samples', None)
+        self._scan_start_idx = kwargs.get('scan_start_idx', 0)
+        self._nocache = kwargs.get('nocache', False)
+
         # first, check to see if this set has previously been cached
         uid = self.universalIdentifier()
         if not self._nocache and DataDirectory().hasCachedAnswer(uid):
             return CacheScan(self._schema, uid, self._num_samples, self._scan_start_idx)
 
         # otherwise, if this Set's source is a DataSource
         if isinstance(self._source, DataSource):
@@ -186,27 +191,27 @@
             if self._schema == sourceSchema:
                 return BaseScan(self._schema, dataset_id, self._num_samples, self._scan_start_idx)
             else:
                 return ConvertScan(self._schema, BaseScan(sourceSchema, dataset_id, self._num_samples, self._scan_start_idx), targetCacheId=uid)
 
         # if the Set's source is another Set, apply the appropriate scan to the Set
         if self._filter is not None:
-            return FilteredScan(self._schema, self._source.getLogicalTree(), self._filter, self._depends_on, targetCacheId=uid)
+            return FilteredScan(self._schema, self._source.getLogicalTree(*args, **kwargs), self._filter, self._depends_on, targetCacheId=uid)
         elif self._groupBy is not None:
-            return GroupByAggregate(self._schema, self._source.getLogicalTree(), self._groupBy, targetCacheId=uid)
+            return GroupByAggregate(self._schema, self._source.getLogicalTree(*args, **kwargs), self._groupBy, targetCacheId=uid)
         elif self._aggFunc is not None:
-            return ApplyAggregateFunction(self._schema, self._source.getLogicalTree(), self._aggFunc, targetCacheId=uid)
+            return ApplyAggregateFunction(self._schema, self._source.getLogicalTree(*args, **kwargs), self._aggFunc, targetCacheId=uid)
         elif self._limit is not None:
-            return LimitScan(self._schema, self._source.getLogicalTree(), self._limit, targetCacheId=uid)
+            return LimitScan(self._schema, self._source.getLogicalTree(*args, **kwargs), self._limit, targetCacheId=uid)
         elif self._fnid is not None:
-            return ApplyUserFunction(self._schema, self._source.getLogicalTree(), self._fnid, targetCacheId=uid)
+            return ApplyUserFunction(self._schema, self._source.getLogicalTree(*args, **kwargs), self._fnid, targetCacheId=uid)
         elif not self._schema == self._source._schema:
-            return ConvertScan(self._schema, self._source.getLogicalTree(), self._cardinality, self._image_conversion, self._depends_on, targetCacheId=uid)
+            return ConvertScan(self._schema, self._source.getLogicalTree(*args, **kwargs), self._cardinality, self._image_conversion, self._depends_on, targetCacheId=uid)
         else:
-            return self._source.getLogicalTree()
+            return self._source.getLogicalTree(*args, **kwargs)
 
 
 class Dataset(Set):
     """
     A Dataset is the intended abstraction for programmers to interact with when manipulating Sets.
 
     Users instantiate a Dataset by specifying a `source` that either points to a
@@ -220,14 +225,15 @@
     To construct a Dataset, users must provide three pieces of information. First, they must
     give the Dataset a unique name using the dataset_id. Second, they need to provide a source
     or source_id, depending on whether the Dataset takes its input from a raw source (e.g. a
     directory, an S3 prefix, etc.) or from another Dataset, respectively. Third, users must
     provide a Schema for the Dataset. This Schema will be enforced when the Dataset iterates
     over the source in its __iter__ method and constructs DataRecords.
     """
+    # TODO: remove num_samples, scan_start_idx, and nocache from Dataset (and Set) constructors
     def __init__(self, source: Union[str, Set], schema: Schema=File, cardinality: str = None, desc: str=None, filter: Filter=None, groupBy: GroupBySig=None, aggFunc: AggregateFunction=None, limit: int=None, fnid: str=None, image_conversion: bool=None, depends_on: Union[str, List[str]]=None, num_samples: int=None, scan_start_idx: int=0, nocache: bool=False):
         # convert source (str) -> source (DataSource) if need be
         self.source = (
             DataDirectory().getRegisteredDataset(source)
             if isinstance(source, str)
             else source
         )
```

### Comparing `palimpzest-0.1.0/src/palimpzest/solver/query_strategies.py` & `palimpzest-0.1.1/src/palimpzest/solver/query_strategies.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/solver/solver.py` & `palimpzest-0.1.1/src/palimpzest/solver/solver.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/solver/task_descriptors.py` & `palimpzest-0.1.1/src/palimpzest/solver/task_descriptors.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/tools/allenpdf.py` & `palimpzest-0.1.1/src/palimpzest/tools/allenpdf.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/tools/pdfparser.py` & `palimpzest-0.1.1/src/palimpzest/tools/pdfparser.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/tools/skema_tools.py` & `palimpzest-0.1.1/src/palimpzest/tools/skema_tools.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/utils/codegen.py` & `palimpzest-0.1.1/src/palimpzest/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest/utils/sandbox.py` & `palimpzest-0.1.1/src/palimpzest/utils/sandbox.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest.egg-info/PKG-INFO` & `palimpzest-0.1.1/src/palimpzest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palimpzest
-Version: 0.1.0
+Version: 0.1.1
 Summary: Palimpzest is a system which enables anyone to process AI-powered analytical queries simply by defining them in a declarative language
 Author-email: MIT DSG Semantic Management Lab <michjc@csail.mit.edu>
 Project-URL: homepage, https://github.com/mitdbg/palimpzest/
 Project-URL: repository, https://https://github.com/mitdbg/palimpzest/
 Keywords: relational,optimization,llm,AI programming,extraction,tools,document,search,integration
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `palimpzest-0.1.0/src/palimpzest.egg-info/SOURCES.txt` & `palimpzest-0.1.1/src/palimpzest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.0/src/palimpzest.egg-info/requires.txt` & `palimpzest-0.1.1/src/palimpzest.egg-info/requires.txt`

 * *Files identical despite different names*

