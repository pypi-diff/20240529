# Comparing `tmp/morgana_engine-0.3.1.tar.gz` & `tmp/morgana_engine-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morgana_engine-0.3.1.tar", last modified: Mon Mar 18 21:40:26 2024, max compression
+gzip compressed data, was "morgana_engine-0.4.0.tar", last modified: Wed May 29 18:14:54 2024, max compression
```

## Comparing `morgana_engine-0.3.1.tar` & `morgana_engine-0.4.0.tar`

### file list

```diff
@@ -1,50 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:40:26.850793 morgana_engine-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-03-18 21:40:26.850793 morgana_engine-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:40:26.846794 morgana_engine-0.3.1/morgana_engine/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:40:26.846794 morgana_engine-0.3.1/morgana_engine/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:40:26.846794 morgana_engine-0.3.1/morgana_engine/adapters/repository/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/adapters/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8711 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/adapters/repository/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/adapters/repository/dataio.py
--rw-r--r--   0 runner    (1001) docker     (127)    33055 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/adapters/repository/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:40:26.846794 morgana_engine-0.3.1/morgana_engine/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/models/parsedsql.py
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/models/readingfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/models/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:40:26.846794 morgana_engine-0.3.1/morgana_engine/services/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/services/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:40:26.850793 morgana_engine-0.3.1/morgana_engine/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/utils/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/morgana_engine/utils/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:40:26.850793 morgana_engine-0.3.1/morgana_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-03-18 21:40:26.000000 morgana_engine-0.3.1/morgana_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-18 21:40:26.000000 morgana_engine-0.3.1/morgana_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 21:40:26.000000 morgana_engine-0.3.1/morgana_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-18 21:40:26.000000 morgana_engine-0.3.1/morgana_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-18 21:40:26.000000 morgana_engine-0.3.1/morgana_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 21:40:26.850793 morgana_engine-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:40:26.850793 morgana_engine-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:40:26.850793 morgana_engine-0.3.1/tests/morgana_engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/tests/morgana_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:40:26.850793 morgana_engine-0.3.1/tests/morgana_engine/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/tests/morgana_engine/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:40:26.850793 morgana_engine-0.3.1/tests/morgana_engine/adapters/repository/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/tests/morgana_engine/adapters/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/tests/morgana_engine/adapters/repository/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/tests/morgana_engine/adapters/repository/test_dataio.py
--rw-r--r--   0 runner    (1001) docker     (127)    30854 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/tests/morgana_engine/adapters/repository/test_processing_select.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:40:26.850793 morgana_engine-0.3.1/tests/morgana_engine/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/tests/morgana_engine/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/tests/morgana_engine/models/test_readingfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-03-18 21:39:13.000000 morgana_engine-0.3.1/tests/morgana_engine/models/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.072538 morgana_engine-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-05-29 18:14:54.072538 morgana_engine-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.068538 morgana_engine-0.4.0/morgana_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.068538 morgana_engine-0.4.0/morgana_engine/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.068538 morgana_engine-0.4.0/morgana_engine/adapters/repository/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/adapters/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8711 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/adapters/repository/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/adapters/repository/dataio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.068538 morgana_engine-0.4.0/morgana_engine/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/models/parsedsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/models/readingfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/models/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/models/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.068538 morgana_engine-0.4.0/morgana_engine/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.068538 morgana_engine-0.4.0/morgana_engine/services/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/services/interpreters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/services/interpreters/lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/services/interpreters/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.068538 morgana_engine-0.4.0/morgana_engine/services/interpreters/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/services/interpreters/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37440 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/services/interpreters/parsers/select.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.068538 morgana_engine-0.4.0/morgana_engine/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/utils/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/morgana_engine/utils/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.072538 morgana_engine-0.4.0/morgana_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-05-29 18:14:54.000000 morgana_engine-0.4.0/morgana_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-29 18:14:54.000000 morgana_engine-0.4.0/morgana_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:14:54.000000 morgana_engine-0.4.0/morgana_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-29 18:14:54.000000 morgana_engine-0.4.0/morgana_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 18:14:54.000000 morgana_engine-0.4.0/morgana_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 18:14:54.072538 morgana_engine-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.072538 morgana_engine-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.072538 morgana_engine-0.4.0/tests/morgana_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.072538 morgana_engine-0.4.0/tests/morgana_engine/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.072538 morgana_engine-0.4.0/tests/morgana_engine/adapters/repository/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/adapters/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/adapters/repository/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/adapters/repository/test_dataio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.072538 morgana_engine-0.4.0/tests/morgana_engine/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/models/test_readingfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/models/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.072538 morgana_engine-0.4.0/tests/morgana_engine/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.072538 morgana_engine-0.4.0/tests/morgana_engine/services/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/services/interpreters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:14:54.072538 morgana_engine-0.4.0/tests/morgana_engine/services/interpreters/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/services/interpreters/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18196 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/services/interpreters/parsers/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/services/interpreters/test_lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:13:50.000000 morgana_engine-0.4.0/tests/morgana_engine/services/interpreters/test_parse.py
```

### Comparing `morgana_engine-0.3.1/LICENSE` & `morgana_engine-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morgana_engine-0.3.1/PKG-INFO` & `morgana_engine-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: morgana_engine
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python module for handling partitioned data using SQL queries.
 Home-page: https://github.com/rjmalves/morgana_engine
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: sqlparse
-Requires-Dist: jsonschema
+Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: python-dotenv
 Requires-Dist: pyarrow
 Requires-Dist: boto3
 Requires-Dist: s3fs>=2023.10.0
 
 # morgana-engine
```

### Comparing `morgana_engine-0.3.1/README.md` & `morgana_engine-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `morgana_engine-0.3.1/morgana_engine/adapters/repository/connection.py` & `morgana_engine-0.4.0/morgana_engine/adapters/repository/connection.py`

 * *Files identical despite different names*

### Comparing `morgana_engine-0.3.1/morgana_engine/adapters/repository/dataio.py` & `morgana_engine-0.4.0/morgana_engine/adapters/repository/dataio.py`

 * *Files identical despite different names*

### Comparing `morgana_engine-0.3.1/morgana_engine/adapters/repository/processing.py` & `morgana_engine-0.4.0/morgana_engine/services/interpreters/parsers/select.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,173 +1,193 @@
-from abc import ABC
-from morgana_engine.adapters.repository.connection import Connection
-from morgana_engine.adapters.repository.dataio import factory as io_factory
-from morgana_engine.models.readingfilter import (
-    type_factory as readingfilter_factory,
+from morgana_engine.models.sql import (
+    SQLTokenType,
+    SQLToken,
+    SQLStatement,
+    SQLParser,
+    ParsingResult,
+    OPERATION_TOKEN_TYPES,
 )
+
+import numpy as np
 import pandas as pd
 from pandas.api.types import is_datetime64_any_dtype as is_datetime
 from pandas.api.types import is_float_dtype as is_float
 from pandas.api.types import is_integer_dtype as is_integer
 from pandas.api.types import is_bool_dtype as is_boolean
 from pandas.api.types import is_string_dtype as is_string
-
-from sqlparse.sql import (  # type: ignore
-    Token,
-    Parenthesis,
-    Comparison,
-    Where,
-    Identifier,
-    IdentifierList,
-)
-from typing import Any, Union, Optional
-from os.path import join
-from morgana_engine.models.readingfilter import ReadingFilter
-from morgana_engine.utils.types import casting_functions
+from morgana_engine.adapters.repository.connection import Connection
+from morgana_engine.adapters.repository.dataio import factory as io_factory
+from morgana_engine.models.readingfilter import type_factory, ReadingFilter
 from morgana_engine.models.parsedsql import Column, Table, QueryingFilter
+from morgana_engine.utils.types import casting_functions
 from morgana_engine.utils.sql import (
     partitions_in_file,
     partition_value_in_file,
 )
-from morgana_engine.utils.sql import (
-    column_from_token,
-    table_from_column_token,
-    add_column_information_from_token,
-    filter_spacing_tokens,
-    filter_punctuation_tokens,
-    filter_spacing_and_punctuation_tokens,
-    split_token_list_in_and_or_keywords,
-    group_set_tokens_parentheses,
-)
-
-
-class Processing(ABC):
-    @classmethod
-    def process(cls, tokens: list[Token], conn: Connection) -> dict:
-        """
-        Processes the tokens associated with the statement in the
-        database specified in the connection.
-        """
-        raise NotImplementedError
-
-
-class CREATE(Processing):
-    @classmethod
-    def process(cls, tokens: list[Token], conn: Connection) -> dict:
-        raise NotImplementedError
-
-
-class ALTER(Processing):
-    @classmethod
-    def process(cls, tokens: list[Token], conn: Connection) -> dict:
-        raise NotImplementedError
-
-
-class DROP(Processing):
-    @classmethod
-    def process(cls, tokens: list[Token], conn: Connection) -> dict:
-        raise NotImplementedError
-
-
-class INSERT(Processing):
-    @classmethod
-    def process(cls, tokens: list[Token], conn: Connection) -> dict:
-        raise NotImplementedError
-
-
-class UPDATE(Processing):
-    @classmethod
-    def process(cls, tokens: list[Token], conn: Connection) -> dict:
-        raise NotImplementedError
-
-
-class DELETE(Processing):
-    @classmethod
-    def process(cls, tokens: list[Token], conn: Connection) -> dict:
-        raise NotImplementedError
-
+from os.path import join
+from typing import Optional, Union, List, Tuple, Any
 
-class SELECT(Processing):
-    """
-    Processes a SELECT statement, for reading data.
 
-    TODO - validate and handle errors
-    TODO - support wildcard * in identifier list
-    TODO - support joins
-    TODO - support joins without aliases
-    TODO - support GROUP BY
-    TODO - support ORDER BY
-    TODO - suport COUNT() function
-    TODO - support LIMIT
-    TODO - support OFFSET
-    """
+class SELECTParser(SQLParser):
+    def __init__(self, statement: SQLStatement, conn: Connection):
+        super().__init__(statement, conn)
+        self.__tables: List[Table] = []
+        self.__select_index: int = -1
+        self.__from_index: int = -1
+        self.__where_index: int = -1
+        self.__filtered: bool = False
+        self.__joining_columns: List[Tuple[Column, Column, str]] = []
+        self.__reading_filters: List[ReadingFilter] = []
+        self.__querying_filters: List[Union[QueryingFilter, str]] = []
+
+    @staticmethod
+    def match_statement(statement: SQLStatement) -> bool:
+        return statement.tokens[0].type == SQLTokenType.SELECT
+
+    def __validate_select_from(self) -> Optional[ParsingResult]:
+        tokens = self.statement.tokens
+        select_tokens = list(
+            filter(lambda t: t.type == SQLTokenType.SELECT, tokens)
+        )
+        if len(select_tokens) != 1:
+            return ParsingResult(
+                status=False,
+                message="The statement must contain 1 SELECT",
+                data=None,
+            )
+        from_tokens = list(
+            filter(lambda t: t.type == SQLTokenType.FROM, tokens)
+        )
+        if len(from_tokens) != 1:
+            return ParsingResult(
+                status=False,
+                message="The statement must contain FROM",
+                data=None,
+            )
+        self.__select_index = tokens.index(select_tokens[0])
+        self.__from_index = tokens.index(from_tokens[0])
+        last_index = len(tokens)
+        if self.__from_index - self.__select_index < 2:
+            return ParsingResult(
+                status=False,
+                message="The statement must contain at least"
+                + " one entity between SELECT and FROM",
+                data=None,
+            )
+        if last_index - self.__from_index < 2:
+            return ParsingResult(
+                status=False,
+                message="The statement must contain at least"
+                + " one entity after FROM",
+                data=None,
+            )
+        return None
 
-    @classmethod
-    def _process_table_identifiers(cls, tokens: list[Token]) -> list[Table]:
-        """
-        Processes the tokens associated with the tables identifiers in
-        order to obtain a list of tables that are related to the query.
+    def __validate_where(self) -> Optional[ParsingResult]:
+        tokens = self.statement.tokens
+        where_tokens = list(
+            filter(lambda t: t.type == SQLTokenType.WHERE, tokens)
+        )
+        if len(where_tokens) > 1:
+            return ParsingResult(
+                status=False,
+                message="The statement may contain 1 WHERE",
+                data=None,
+            )
+        self.__filtered = len(where_tokens) == 1
+        self.__where_index = (
+            tokens.index(where_tokens[0]) if self.__filtered else -1
+        )
+        if self.__filtered:
+            last_index = len(tokens)
+            if last_index - self.__where_index < 2:
+                return ParsingResult(
+                    status=False,
+                    message="The statement must contain at least"
+                    + " one entity after WHERE",
+                    data=None,
+                )
+        return None
+
+    @staticmethod
+    def __split_by_token_type(
+        tokens: list[SQLToken],
+        token_types: SQLTokenType | list[SQLTokenType],
+    ) -> list[list[SQLToken]]:
+        if isinstance(token_types, SQLTokenType):
+            token_types = [token_types]
+
+        def __filter_by_token_type(token: SQLToken) -> bool:
+            return token.type in token_types
+
+        tokens_of_type = list(filter(__filter_by_token_type, tokens))
+        tokens_indices = (
+            [-1] + [tokens.index(c) for c in tokens_of_type] + [len(tokens)]
+        )
+        splitting_indices = []
+        for i in range(len(tokens_indices) - 1):
+            splitting_indices.append(
+                (tokens_indices[i] + 1, tokens_indices[i + 1])
+            )
+        return [tokens[s:e] for s, e in splitting_indices]
 
-        Parameters:
-        -----------
-        tokens :  list[Token]
-            A list of tokens that were parsed from the query with the SELECT
-            statement.
+    def __get_querying_tables(self) -> Optional[ParsingResult]:
+        last_index = (
+            self.__where_index
+            if self.__filtered
+            else len(self.statement.tokens)
+        )
+        tokens = self.statement.tokens[self.__from_index + 1 : last_index]
 
-        Returns:
-        --------
-        list[Table]
-            A list of Table objects with their names and aliases, but with
-            no column information up to this point.
+        joining_tokens = self.__split_by_token_type(tokens, SQLTokenType.JOIN)
 
-        """
-        # Iterate on tokens and find the table identifiers
-        identifier_list = [t for t in tokens if type(t) is Identifier]
-        alias_map: dict[str, str] = {
-            t.get_alias(): t.get_real_name() for t in identifier_list
-        }
-        return [
-            Table(name=v, alias=k, columns=[]) for k, v in alias_map.items()
-        ]
+        for table_token_group in joining_tokens:
+            table_tokens = self.__split_by_token_type(
+                table_token_group, SQLTokenType.COMMA
+            )
+            for column_token_group in table_tokens:
+                aliases_tokens = self.__split_by_token_type(
+                    column_token_group, SQLTokenType.AS
+                )
+                table_name = aliases_tokens[0][0].text
+                table_alias = (
+                    aliases_tokens[-1][0].text
+                    if len(aliases_tokens) > 1
+                    else None
+                )
 
-    @classmethod
-    def _process_column_wildcard(
-        cls,
-        tables_to_select: list[Table],
-        conn: Connection,
-    ):
-        """
-        Accesses the schema data for filling all column information
-        since the select data is a wildcard.
+                self.__tables.append(
+                    Table(name=table_name, alias=table_alias, columns=[])
+                )
 
-        Parameters:
-        -----------
-        tables_to_select : list[Table]
-            A list of tables that are related to the query.
-        conn : Connection
-            The connection to the database where the tables are located.
+        return None
 
-        """
-        for table in tables_to_select:
-            table_conn = conn.access(table.name)
+    def __get_schema_elements(self) -> Optional[ParsingResult]:
+        for table in self.__tables:
+            table_conn = self.conn.access(table.name)
             if not table_conn.schema.is_table:
-                raise ValueError(f"Schema {table.name} is not a table")
+                return ParsingResult(
+                    status=False,
+                    message=f"Table {table.name} not found",
+                    data=None,
+                )
             for (
                 column_name,
                 column_type,
             ) in table_conn.schema.columns.items():
                 table.columns.append(
                     Column(
                         name=column_name,
                         alias=None,
                         type_str=column_type,
                         table_name=table.name,
                         table_alias=table.alias,
                         has_parent_in_token=False,
                         partition=False,
+                        querying=False,
                     )
                 )
             for (
                 partition_name,
                 partition_type,
             ) in table_conn.schema.partitions.items():
                 table.columns.append(
@@ -175,371 +195,487 @@
                         name=partition_name,
                         alias=None,
                         type_str=partition_type,
                         table_name=table.name,
                         table_alias=table.alias,
                         has_parent_in_token=False,
                         partition=True,
+                        querying=False,
                     )
                 )
+        return None
 
-    @classmethod
-    def _process_column_identifiers(
-        cls,
-        tokens: list[Token],
-        tables_to_select: list[Table],
-        conn: Connection,
-    ):
-        """
-        Processes the tokens associated with the column identifiers in
-        order to obtain a map of table_alias: {column_alias: column_name}
-        and add their information to the table list that was previously
-        parsed from the query.
+    def __get_table_from_token_list(
+        self, name_or_alias: str
+    ) -> Union[Table, ParsingResult]:
+        # Finds the table with the given name / alias
+        tables = list(
+            filter(
+                lambda t: t.name == name_or_alias or t.alias == name_or_alias,
+                self.__tables,
+            )
+        )
+        if len(tables) != 1:
+            return ParsingResult(
+                status=False,
+                message=f"Table {name_or_alias} not found or is ambiguous",
+                data=None,
+            )
+        return tables[0]
 
-        Parameters:
-        -----------
-        tokens :  list[Token]
-            A list of tokens that were parsed from the query
-        tables_to_select : list[Table]
-            A list of tables that are related to the query.
-        conn : Connection
-            The connection to the database where the tables are located.
+    def __get_column_from_token_list(
+        self, tokens: List[SQLToken]
+    ) -> Union[Column, ParsingResult]:
+        columns_with_table = self.__split_by_token_type(
+            tokens, SQLTokenType.DOT
+        )
+        if len(columns_with_table) > 1:
+            table_name_or_alias = columns_with_table[0][0].text
+            column_name = columns_with_table[1][0].text
+            has_parent_in_token = True
+
+            # Finds the table with the given name / alias
+            table = self.__get_table_from_token_list(table_name_or_alias)
+            if isinstance(table, ParsingResult):
+                return table
+        else:
+            table = self.__tables[0]
+            column_name = columns_with_table[0][0].text
+            has_parent_in_token = False
 
-        """
-        if "*" in [t.normalized for t in tokens]:
-            cls._process_column_wildcard(tables_to_select, conn)
+        table_column = list(
+            filter(lambda c: c.name == column_name, table.columns)
+        )
+
+        found_column = False
+        if len(table_column) == 1:
+            found_column = True
         else:
-            # Else, iterate on tokens and find the column identifiers
-            identifier_list = [t for t in tokens if type(t) is IdentifierList][
-                0
-            ]
-            identifier_tokens: list[Identifier] = [
-                t for t in identifier_list.tokens if type(t) is Identifier
-            ]
-            # Adds the column information to the table list
-            for t in identifier_tokens:
-                add_column_information_from_token(t, tables_to_select)
-            # Adds data type information from the schemas
-            for table in tables_to_select:
-                table_conn = conn.access(table.name)
-                if not table_conn.schema.is_table:
-                    raise ValueError(f"Schema {table.name} is not a table")
-                for column in table.columns:
-                    column_schemas = list(
-                        filter(
-                            lambda column_pair: column_pair[0] == column.name,
-                            table_conn.schema.columns.items(),
-                        )
-                    )
-                    partition_schemas = list(
-                        filter(
-                            lambda partition_pair: partition_pair[0]
-                            == column.name,
-                            table_conn.schema.partitions.items(),
-                        )
-                    )
-                    if len(column_schemas) == 1:
-                        column.type_str = column_schemas[0][1]
-                        column.partition = False
-                    if len(partition_schemas) == 1:
-                        column.type_str = partition_schemas[0][1]
-                        column.partition = True
-
-        return tables_to_select
-
-    @classmethod
-    def _process_join_mappings(
-        cls, tokens: list[Token], tables_to_select: list[Table]
-    ) -> list[tuple[Column, Column]]:
-        """
-        Processes the tokens associated with the join mappings in order
-        to obtain a map of each join type with the tables that must be joined.
+            table_column = list(
+                filter(lambda c: c.alias == column_name, table.columns)
+            )
+            if len(table_column) == 1:
+                found_column = True
+        if not found_column:
+            return ParsingResult(
+                status=False,
+                message=f"Column {column_name} not found in table {table.name}",
+                data=None,
+            )
+        table_column[0].has_parent_in_token = has_parent_in_token
+        return table_column[0]
 
-        Parameters:
-        -----------
-        tokens :  list[Token]
-            A list of tokens that were parsed from the query
-        tables_to_select : list[Table]
-            A list of tables that are related to the query.
+    def __get_querying_columns(self) -> Optional[ParsingResult]:
+        # Gets tokens between SELECT and FROM
+        # for considering as columns
+        tokens = self.statement.tokens[
+            self.__select_index + 1 : self.__from_index
+        ]
 
-        Returns:
-        --------
-        list[tuple[Column, Column]]
-            A list of tuples that define tables that must be joined,
-            specifying the joining columns.
+        # Shortcut for the wildcard case
+        if any([t.type == SQLTokenType.WILDCARD for t in tokens]):
+            for table in self.__tables:
+                for column in table.columns:
+                    column.querying = True
+            return None
 
-        """
+        # Splits the tokens by commas
+        # into sublists for each column,
+        # possibly with aliases
+        column_tokens = self.__split_by_token_type(tokens, SQLTokenType.COMMA)
+        for column_token_group in column_tokens:
+            aliases_tokens = self.__split_by_token_type(
+                column_token_group, SQLTokenType.AS
+            )
+            column_alias = (
+                aliases_tokens[-1][0].text if len(aliases_tokens) > 1 else None
+            )
+            r = self.__get_column_from_token_list(aliases_tokens[0])
+            if isinstance(r, ParsingResult):
+                return r
+            else:
+                table_column = r
+                table_column.querying = True
+                table_column.alias = column_alias
+
+        return None
+
+    def __get_joining_columns(self) -> Optional[ParsingResult]:
+        last_index = (
+            self.__where_index
+            if self.__filtered
+            else len(self.statement.tokens)
+        )
+        tokens = self.statement.tokens[self.__from_index + 1 : last_index]
 
-        def __find_column_by_token(
-            token: Identifier, columns: list[Column]
-        ) -> Optional[Column]:
-            for column in columns:
-                table_name_or_alias = token.get_parent_name()
-                table_match = (
-                    column.table_alias == table_name_or_alias
-                    or column.table_name == table_name_or_alias
-                )
-                column_name_or_alias = token.get_real_name()
-                column_match = (
-                    column.alias == column_name_or_alias
-                    or column.name == column_name_or_alias
-                )
-                if table_match and column_match:
-                    return column
+        joining_tokens = self.__split_by_token_type(tokens, SQLTokenType.JOIN)
+        num_joins = len(joining_tokens) - 1
+        if num_joins == 0:
             return None
 
-        def __find_table_and_column_by_token(
-            token: Identifier, tables: list[Table]
-        ) -> Column:
-            all_columns = [c for t in tables for c in t.columns]
-            c = __find_column_by_token(token, all_columns)
-            if c:
-                return c
-
-            raise ValueError(f"Column {token.get_alias()} not found")
-
-        comparison_tokens = [t for t in tokens if type(t) is Comparison]
-        mappings: list[tuple[Column, Column]] = []
-        for c in comparison_tokens:
-            identifiers = [
-                t
-                for t in filter_punctuation_tokens(c.tokens)
-                if type(t) is Identifier
-            ]
-            mappings.append(
-                (
-                    __find_table_and_column_by_token(
-                        identifiers[0], tables_to_select
-                    ),
-                    __find_table_and_column_by_token(
-                        identifiers[1], tables_to_select
-                    ),
-                )
-            )
-        return mappings
-
-    @classmethod
-    def _extract_reading_filters(
-        cls,
-        token_or_list: Token | list[Token],
-        tables_to_select: list[Table],
-    ) -> list[ReadingFilter]:
-        """
-        Processes the tokens after the WHERE for extracting filters
-        for optimizing partition reading.
+        for left_joining_tokens, right_joining_tokens in zip(
+            joining_tokens[:-1], joining_tokens[1:]
+        ):
+            tables: List[Table] = []
+            for token_set in [left_joining_tokens, right_joining_tokens]:
+                aliases_tokens = self.__split_by_token_type(
+                    token_set, SQLTokenType.AS
+                )
+                table_name = aliases_tokens[0][0].text
+                table = self.__get_table_from_token_list(table_name)
+                if isinstance(table, ParsingResult):
+                    return table
+
+                tables.append(table)
+
+            join_kind_token = left_joining_tokens[-1]
+
+            on_tokens = self.__split_by_token_type(
+                right_joining_tokens, SQLTokenType.ON
+            )[1]
 
-        Parameters:
-        -----------
-        token_or_list : Token | list[Token]
-            A token or list of tokens that were parsed from the query
-        tables_to_select : list[Table]
-            A list of tables that are related to the query.
+            joining_column_tokens = self.__split_by_token_type(
+                on_tokens, SQLTokenType.EQUALS
+            )
+            columns: List[Column] = []
+            for column_tokens in joining_column_tokens:
+                column = self.__get_column_from_token_list(column_tokens)
+                if isinstance(column, ParsingResult):
+                    return column
+                columns.append(column)
+            column_tuple = (
+                columns[0],
+                columns[1],
+                join_kind_token.text.lower(),
+            )
+            self.__joining_columns.append(column_tuple)
 
-        Returns:
-        --------
-        list[ReadingFilter]
-            A list of ReadingFilters that should be applied to the reading
-            process of each table. The default table receives the `None` alias.
+        return None
 
-        """
-        if type(token_or_list) is Parenthesis:
-            splitted_list = split_token_list_in_and_or_keywords(
-                filter_spacing_tokens(token_or_list.tokens)
-            )
-            filters = []
-            for token_list in splitted_list:
-                filters += cls._extract_reading_filters(
-                    token_list, tables_to_select
-                )
-            return filters
-        elif type(token_or_list) is Comparison:
-            # First case of interest:
-            # Equality and Unequality
-            comparison_tokens = filter_spacing_tokens(token_or_list.tokens)
-            identifiers = [
-                t for t in comparison_tokens if type(t) is Identifier
+    def __filter_querying_columns(self) -> Optional[ParsingResult]:
+        for table in self.__tables:
+            table.columns = list(filter(lambda c: c.querying, table.columns))
+
+        return None
+
+    def __recursive_get_reading_filters(
+        self, tokens: List[SQLToken], context_depths: np.ndarray
+    ) -> Union[Tuple[List[SQLToken], np.ndarray], ParsingResult]:
+        # Get deepest context and extract tokens
+        max_context_depth = max(context_depths)
+        indices = np.where(context_depths == max_context_depth)[0]
+        internal_tokens: List[SQLToken] = [tokens[i] for i in indices]
+        initial_index = indices[0]
+        final_index = indices[-1]
+        before_tokens, before_depths = (
+            tokens[:initial_index],
+            context_depths[:initial_index],
+        )
+        after_tokens, after_depths = (
+            tokens[final_index + 1 :],
+            context_depths[final_index + 1 :],
+        )
+        if SQLTokenType.LPAREN in [t.type for t in internal_tokens]:
+            initial_index += 1
+            internal_tokens = internal_tokens[1:]
+        if SQLTokenType.RPAREN in [t.type for t in internal_tokens]:
+            final_index -= 1
+            internal_tokens = internal_tokens[:-1]
+
+        if all(
+            [
+                t.type in [SQLTokenType.ENTITY, SQLTokenType.COMMA]
+                for t in internal_tokens
             ]
-            filter_type = readingfilter_factory(comparison_tokens)
-            if filter_type:
-                # Find the table with the given alias
-                table = table_from_column_token(
-                    identifiers[0], tables_to_select
-                )
-                return [filter_type(comparison_tokens, table)]
-        elif type(token_or_list) is list:
-            # Second case of interest:
-            # Belonging and Not Belonging to Set
-            comparison_tokens = filter_spacing_tokens(token_or_list)
-            if len(comparison_tokens) == 1:
-                return cls._extract_reading_filters(
-                    comparison_tokens[0], tables_to_select
-                )
-            elif len(comparison_tokens) in [3, 4]:
-                identifiers = [
-                    t for t in comparison_tokens if type(t) is Identifier
-                ]
-                filter_type = readingfilter_factory(comparison_tokens)
-                if filter_type:
-                    # Find the table with the given alias
-                    table = table_from_column_token(
-                        identifiers[0], tables_to_select
+            + [len(tokens) > 0]
+        ):
+            # If there are only entities and commas, it is a list
+            # of values.
+            value_list_token = SQLToken(
+                SQLTokenType.ENTITY,
+                text=" ".join([t.text for t in internal_tokens]),
+            )
+            tokens_to_add = [value_list_token]
+            depths_to_add = np.array(
+                [max_context_depth - 1] * len(tokens_to_add), dtype=int
+            )
+        else:
+            tokens_to_add = []
+            depths_to_add = np.array([])
+            # Split be AND and OR operators
+            subfilters = self.__split_by_token_type(
+                internal_tokens, [SQLTokenType.AND, SQLTokenType.OR]
+            )
+            # Create each reading filter
+            for f in subfilters:
+                operation = list(
+                    filter(
+                        lambda t: t.type in OPERATION_TOKEN_TYPES,
+                        f,
                     )
-                    return [filter_type(comparison_tokens, table)]
-
-        return []
+                )
+                if len(operation) == 0:
+                    return ParsingResult(
+                        status=False,
+                        message="No operation found in filter"
+                        + f" {[str(t) for t in f]}",
+                        data=None,
+                    )
+                else:
+                    column_tokens = f[: f.index(operation[0])]
+                    value_tokens = f[f.index(operation[-1]) + 1 :]
+                    if len(operation) == 2:
+                        if not all(
+                            [
+                                t.type
+                                in [
+                                    SQLTokenType.NOT,
+                                    SQLTokenType.IN,
+                                ]
+                                for t in operation
+                            ]
+                        ):
+                            return ParsingResult(
+                                status=False,
+                                message="Invalid operation found in filter"
+                                + f" {[str(t) for t in operation]}",
+                                data=None,
+                            )
+                        else:
+                            operation = [
+                                SQLToken(SQLTokenType.NOT_IN, text="NOT IN")
+                            ]
+                column_or_result = self.__get_column_from_token_list(
+                    column_tokens
+                )
 
-    @classmethod
-    def _process_filters_for_reading(
-        cls,
-        tokens: list[Token],
-        tables_to_select: list[Table],
-    ) -> list[ReadingFilter]:
-        """
-        Filters the tokens after the WHERE that might help deciding which
-        partition files must be read, optimizing reading time.
+                if isinstance(column_or_result, ParsingResult):
+                    return column_or_result
+                else:
+                    column = column_or_result
+                reading_filter_type = type_factory(operation[0])
+                r = reading_filter_type(column, operation[0], value_tokens)
+                self.__reading_filters.append(r)
+
+        return (
+            before_tokens + tokens_to_add + after_tokens,
+            np.concatenate([before_depths, depths_to_add, after_depths]),
+        )
 
-        Filters that are considered:
+    def __get_reading_filters(self) -> Optional[ParsingResult]:
+        def __add_token_context_depths(tokens: List[SQLToken]) -> np.ndarray:
+            context_depths: np.ndarray = np.zeros_like(tokens, dtype=int)
+            current_context = 0
+            for i, t in enumerate(tokens):
+                if t.type == SQLTokenType.LPAREN:
+                    current_context += 1
+                context_depths[i] = current_context
+                if t.type == SQLTokenType.RPAREN:
+                    current_context -= 1
+            return context_depths
 
-        - Column equality to constant
-        - Column unequality to constant
-        - Column belonging to set
-        - Column not belonging to set
+        if self.__where_index == -1:
+            return None
 
-        Parameters:
-        -----------
-        tokens :  list[Token]
-            A list of tokens that were parsed from the query
-        tables_to_select : list[Table]
-            A list of tables that are related to the query.
+        tokens = self.statement.tokens[self.__where_index + 1 :]
+        context_depths = __add_token_context_depths(tokens)
 
-        Returns:
-        --------
-        list[ReadingFilter]
-            A list of ReadingFilters that should be applied to the reading
-            process of each table. The default table receives the `None` alias.
+        # Recursively parses tokens and context depths, replacing
+        # inner contexts with single tokens whenever possible
+        # and creating the reading filters
+
+        while len(tokens) > 0:
+            r = self.__recursive_get_reading_filters(tokens, context_depths)
+            if isinstance(r, ParsingResult):
+                return r
+            else:
+                tokens, context_depths = r
+        return None
 
-        """
-        where_tokens = [t for t in tokens if type(t) is Where]
-        if len(where_tokens) > 0:
-            splitted_tokens = split_token_list_in_and_or_keywords(
-                filter_spacing_and_punctuation_tokens(
-                    where_tokens[0].tokens[1:]
-                )
+    def __recursive_get_querying_filters(
+        self, tokens: List[SQLToken], context_depths: np.ndarray
+    ) -> Union[Tuple[List[SQLToken], np.ndarray], ParsingResult]:
+        # Get deepest context and extract tokens
+        max_context_depth = max(context_depths)
+        indices = np.where(context_depths == max_context_depth)[0]
+        internal_tokens: List[SQLToken] = [tokens[i] for i in indices]
+        initial_index = indices[0]
+        final_index = indices[-1]
+        before_tokens, before_depths = (
+            tokens[:initial_index],
+            context_depths[:initial_index],
+        )
+        after_tokens, after_depths = (
+            tokens[final_index + 1 :],
+            context_depths[final_index + 1 :],
+        )
+        if SQLTokenType.LPAREN in [t.type for t in internal_tokens]:
+            initial_index += 1
+            internal_tokens = internal_tokens[1:]
+        if SQLTokenType.RPAREN in [t.type for t in internal_tokens]:
+            final_index -= 1
+            internal_tokens = internal_tokens[:-1]
+
+        if all(
+            [
+                t.type in [SQLTokenType.ENTITY, SQLTokenType.COMMA]
+                for t in internal_tokens
+            ]
+            + [len(tokens) > 0]
+        ):
+            # If there are only entities and commas, it is a list
+            # of values.
+            value_list_token = SQLToken(
+                SQLTokenType.ENTITY,
+                text=" ".join([t.text for t in internal_tokens]),
+            )
+            tokens_to_add = [value_list_token]
+            depths_to_add = np.array(
+                [max_context_depth - 1] * len(tokens_to_add), dtype=int
             )
         else:
-            splitted_tokens = []
-        filtermaps: list[ReadingFilter] = []
-        for token_set in splitted_tokens:
-            t_map = cls._extract_reading_filters(token_set, tables_to_select)
-            filtermaps += t_map
-
-        return filtermaps
-
-    @classmethod
-    def _process_filters_for_querying(
-        cls, tokens: list[Token], tables_to_select: list[Table]
-    ) -> list[Union[QueryingFilter, Column, str]]:
-        """
-        Filters the tokens after the WHERE that should be used for
-        querying the DataFrame.
-
-        Parameters:
-        -----------
-        tokens :  list[Token]
-            A list of tokens that were parsed from the query
-        tables_to_select : list[Table]
-            A list of tables that are related to the query.
-
-        Returns:
-        --------
-        list[Union[QueryingFilter, Column, str]]
-            A collection of elements that will be used to
-            compose the query string (column_name, operator, value) or
-            just a separator "&", "|" or "~".
-
-        """
-
-        def process_filters_to_pandas_query(
-            token_or_list: Token | list[Token],
-        ) -> Union[QueryingFilter, Column, str]:
-            """
-            Filters the tokens after the WHERE that should be used for
-            querying the DataFrame.
-
-            Parameters:
-            -----------
-            token_or_list :  Token | list[Token]
-                A token or list of tokens that were parsed from the query
-
-            Returns:
-            --------
-            QueryingFilter | Column | str
-                An element that compose a filter for the query string.
-
-            """
-            logical_operator_mappings: dict[str, str] = {
-                "=": "==",
-                "AND": "&",
-                "OR": "|",
-                "NOT": "not",
-                "IN": "in",
-            }
-            if (type(token_or_list) is Parenthesis) or (
-                type(token_or_list) is IdentifierList
-            ):
-                return process_filters_to_pandas_query(
-                    filter_spacing_tokens(token_or_list.tokens)
-                )
-            elif type(token_or_list) is Comparison:
-                comparison_tokens = token_or_list.tokens
-                col = column_from_token(comparison_tokens[0], tables_to_select)
-                operator_tokens = comparison_tokens[1:-1]
-                if len(operator_tokens) == 1:
-                    operator = logical_operator_mappings.get(
-                        operator_tokens[0].normalized,
-                        operator_tokens[0].normalized,
+            tokens_to_add = []
+            depths_to_add = np.array([])
+            # Split be AND and OR operators
+            subfilters = self.__split_by_token_type(
+                internal_tokens, [SQLTokenType.AND, SQLTokenType.OR]
+            )
+            filter_delimiters = [
+                t
+                for t in internal_tokens
+                if t.type in [SQLTokenType.AND, SQLTokenType.OR]
+            ]
+            # Create each reading filter
+            for i, f in enumerate(subfilters):
+                operation = list(
+                    filter(
+                        lambda t: t.type in OPERATION_TOKEN_TYPES,
+                        f,
+                    )
+                )
+                if len(operation) == 0:
+                    return ParsingResult(
+                        status=False,
+                        message="No operation found in filter"
+                        + f" {[str(t) for t in f]}",
+                        data=None,
                     )
                 else:
-                    operator = " ".join(
-                        [
-                            logical_operator_mappings.get(
-                                t.normalized, t.normalized
+                    column_tokens = f[: f.index(operation[0])]
+                    value_tokens = f[f.index(operation[-1]) + 1 :]
+                    if len(operation) == 2:
+                        if not all(
+                            [
+                                t.type
+                                in [
+                                    SQLTokenType.NOT,
+                                    SQLTokenType.IN,
+                                ]
+                                for t in operation
+                            ]
+                        ):
+                            return ParsingResult(
+                                status=False,
+                                message="Invalid operation found in filter"
+                                + f" {[str(t) for t in operation]}",
+                                data=None,
                             )
-                            for t in operator_tokens
-                        ]
+                        else:
+                            operation = [
+                                SQLToken(SQLTokenType.NOT_IN, text="NOT IN")
+                            ]
+                column_or_result = self.__get_column_from_token_list(
+                    column_tokens
+                )
+                if isinstance(column_or_result, ParsingResult):
+                    return column_or_result
+                else:
+                    column = column_or_result
+                logical_operator_mappings: dict[str, str] = {
+                    "=": "==",
+                    "AND": "&",
+                    "OR": "|",
+                    "NOT IN": "not in",
+                    "IN": "in",
+                }
+                operation_token = operation[0]
+                operator = logical_operator_mappings.get(
+                    operation_token.text,
+                    operation_token.text,
+                )
+                value_str = (
+                    "(" + value_tokens[0].text + ")"
+                    if operation_token.type
+                    in [SQLTokenType.IN, SQLTokenType.NOT_IN]
+                    else value_tokens[0].text
+                )
+                q = QueryingFilter(column, operator, value_str)
+                self.__querying_filters.append(q)
+                if i < len(filter_delimiters):
+                    delimiter = logical_operator_mappings.get(
+                        filter_delimiters[i].text,
+                        filter_delimiters[i].text,
                     )
-                value = comparison_tokens[-1].normalized
-                return QueryingFilter(col, operator, value)  # type: ignore
-            elif type(token_or_list) is Identifier:
-                return column_from_token(token_or_list, tables_to_select)
-            elif type(token_or_list) is Token:
-                value = str(token_or_list.normalized)
-                return logical_operator_mappings.get(value, value)
+                    self.__querying_filters.append(delimiter)
+
+        return (
+            before_tokens + tokens_to_add + after_tokens,
+            np.concatenate([before_depths, depths_to_add, after_depths]),
+        )
+
+    def __get_querying_filters(self) -> Optional[ParsingResult]:
+        def __add_token_context_depths(tokens: List[SQLToken]) -> np.ndarray:
+            context_depths: np.ndarray = np.zeros_like(tokens, dtype=int)
+            current_context = 0
+            for i, t in enumerate(tokens):
+                if t.type == SQLTokenType.LPAREN:
+                    current_context += 1
+                context_depths[i] = current_context
+                if t.type == SQLTokenType.RPAREN:
+                    current_context -= 1
+            return context_depths
+
+        if self.__where_index == -1:
+            return None
+
+        tokens = self.statement.tokens[self.__where_index + 1 :]
+        context_depths = __add_token_context_depths(tokens)
+
+        # Recursively parses tokens and context depths, replacing
+        # inner contexts with single tokens whenever possible
+        # and creating the reading filters
+
+        while len(tokens) > 0:
+            r = self.__recursive_get_querying_filters(tokens, context_depths)
+            if isinstance(r, ParsingResult):
+                return r
             else:
-                raise ValueError(
-                    f"Unknown token type {type(token_or_list)} in "
-                    f"process_filters_to_pandas_query"
-                )
-
-        filters = [t for t in tokens if type(t) is Where]
-        if len(filters) > 0:
-            pandas_query_elements = []
-            where_tokens = filter_spacing_tokens(filters[0].tokens[1:])
-            # Explicitly group IN operations
-            where_tokens = group_set_tokens_parentheses(where_tokens)
-            for t in where_tokens:
-                pandas_query_elements.append(
-                    process_filters_to_pandas_query(t)
-                )
-            return pandas_query_elements
-        else:
-            return []
+                tokens, context_depths = r
+        return None
 
-    @classmethod
-    def _dataframe_column_type_casting_keyword(cls, column: pd.Series) -> str:
+    def validate(self) -> Optional[ParsingResult]:
+        validators = [
+            self.__validate_select_from,
+            self.__validate_where,
+            self.__get_querying_tables,
+            self.__get_schema_elements,
+            self.__get_querying_columns,
+            self.__filter_querying_columns,
+            self.__get_joining_columns,
+            self.__get_reading_filters,
+            self.__get_querying_filters,
+        ]
+        for v in validators:
+            r = v()
+            if r:
+                return r
+
+        return None
+
+    def __dataframe_column_type_casting_keyword(self, column: pd.Series) -> str:
         """
         Checks the column type among all supported data types in the DataFrame
         and returns the keyword that should by used by the casting function
         to perform the correct casting, enabling the query string.
         """
         column_type_inference_function_map = {
             "int": is_integer,
@@ -552,26 +688,23 @@
             typestring,
             checking_function,
         ) in column_type_inference_function_map.items():
             if checking_function(column):
                 return typestring
         return "string"
 
-    @classmethod
-    def _compose_query_and_query_dataframe(
-        cls,
+    def __compose_query_and_query_dataframe(
+        self,
         df: pd.DataFrame,
-        parsed_filters: list[Union[QueryingFilter, Column, str]],
     ) -> pd.DataFrame:
-
         def __cast_unquoting_value(f: QueryingFilter) -> Any:
             value = f.value
             column = f.column.fullname
             casting_function_keyword = (
-                cls._dataframe_column_type_casting_keyword(df[column])
+                self.__dataframe_column_type_casting_keyword(df[column])
             )
             unquoted_value = value.replace("'", "").replace('"', "").strip()
             if f.is_collection:
                 str_values = (
                     unquoted_value.replace("(", "").replace(")", "").split(",")
                 )
                 return tuple(
@@ -586,36 +719,38 @@
                 return casting_functions(casting_function_keyword)(
                     unquoted_value
                 )
 
         casted_filter_values: list[Any] = []
         query_string_parts: list[str] = []
         num_filters = 0
-        for f in parsed_filters:
+        for f in self.__querying_filters:
             if isinstance(f, QueryingFilter):
                 query_string_part = (
-                    f"{f.column.fullname} {f.operator}"
+                    "("
+                    + f"{f.column.fullname} {f.operator}"
                     + f" @casted_filter_values[{num_filters}]"
+                    + ")"
                 )
                 casted_filter_values.append(__cast_unquoting_value(f))
                 query_string_parts.append(query_string_part)
                 num_filters += 1
             else:
-                query_string_parts.append(str(f))
+                query_string_parts.append(f)
+
         query_string = " ".join(query_string_parts)
         if num_filters > 0:
             # All filters have a (column, operator, value) format
             df = df.query(query_string)
             return df
         else:
             return df
 
-    @classmethod
-    def _read_files_with_partitions(
-        cls,
+    def __read_files_with_partitions(
+        self,
         conn: Connection,
         partition_columns: dict[str, str],
         filters: list[ReadingFilter],
     ) -> list[str]:
         """
         Lists the files that must be read from a table with partitions,
         considering the desired filters for each partitioned column.
@@ -675,17 +810,16 @@
             value_files = []
             for v in filtered_values:
                 value_files += partition_maps[v]
             files_to_read += value_files
         files_to_read = list(set(files_to_read))
         return files_to_read
 
-    @classmethod
-    def _process_select_from_table(
-        cls, table: Table, filters: list[ReadingFilter], conn: Connection
+    def __select_from_table(
+        self, table: Table, filters: list[ReadingFilter], conn: Connection
     ) -> dict:
         """
         Processes the content of the SELECT statement with respect
         to a single table, reading the files that are necessary, casting
         data types if needed and returning the requested columns.
 
         Parameters:
@@ -717,15 +851,15 @@
         partition_columns: dict[str, str] = table_conn.schema.partitions
         # The main result is the list of filenames that must be read
         # and concatenated.
         files_to_read: list[str] = []
         if len(partition_columns) == 0:
             files_to_read.append(table.name)
         else:
-            files_to_read += cls._read_files_with_partitions(
+            files_to_read += self.__read_files_with_partitions(
                 table_conn, partition_columns, filters
             )
 
         dfs: list[pd.DataFrame] = []
         for f in files_to_read:
             dff = table_io.read(
                 join(table_conn.uri, f),
@@ -760,21 +894,15 @@
         df = df.rename(columns=column_mappings)
 
         return {
             "processedFiles": files_to_read,
             "data": df,
         }
 
-    @classmethod
-    def _process_select_from_tables(
-        cls,
-        tables_to_select: list[Table],
-        reading_filters: list[ReadingFilter],
-        conn: Connection,
-    ) -> dict:
+    def __select_from_tables(self) -> dict:
         """
         Processes the SELECT statement for each table separately,
         using the reading_filters for optimizing the file reading steps.
 
         Parameters:
         -----------
         tables_to_select :  dict[str, str]
@@ -792,132 +920,80 @@
         dict
             A dict with the dataframe with the requested data from the table
             and some metadata regarding the reading process.
 
         """
         files: list[str] = []
         dfs: list[pd.DataFrame] = []
-        for table in tables_to_select:
+        for table in self.__tables:
             name = table.name
-            table_select_result = cls._process_select_from_table(
+            table_select_result = self.__select_from_table(
                 table,
-                [f for f in reading_filters if f.column.table_name == name],
-                conn,
+                [
+                    f
+                    for f in self.__reading_filters
+                    if f.column.table_name == name
+                ],
+                self.conn,
             )
             files += table_select_result["processedFiles"]
             dfs.append(table_select_result["data"])
         return {
             "processedFiles": files,
             "data": dfs,
         }
 
-    @classmethod
-    def _process_join_tables(
-        cls,
+    def __join_tables(
+        self,
         dfs: list[pd.DataFrame],
-        table_join_mappings: list[tuple[Column, Column]],
-    ) -> pd.DataFrame:
+    ) -> Union[pd.DataFrame, ParsingResult]:
         """
         Processes the JOIN keywords in the query, joining the tables in the order
         they appear in the statement.
 
         Parameters:
         -----------
         dfs : list[pd.DataFrame]
             List of dataframes that were read from each table
-        table_join_mappings : list[tuple[Column, Column]]
-            A mapping of table columns that should be joined.
 
         Returns:
         --------
         pd.DataFrame
             The dataframe resulting from the JOIN operations.
 
         """
-        num_joins = len(table_join_mappings)
+
+        supported_joins = ["inner", "left", "right", "outer"]
+
+        num_joins = len(self.__joining_columns)
         if num_joins > 0:
             for i in range(num_joins):
                 df_left = dfs[i]
-                left_col = table_join_mappings[i][0]
+                left_col = self.__joining_columns[i][0]
                 df_right = dfs[i + 1]
-                right_col = table_join_mappings[i][1]
+                right_col = self.__joining_columns[i][1]
+                join_kind = self.__joining_columns[i][2]
+                if join_kind not in supported_joins:
+                    return ParsingResult(
+                        status=False,
+                        message="Join kind not supported",
+                        data=None,
+                    )
                 df_right.set_index(right_col.fullname, inplace=True)
                 dfs[i + 1] = df_left.join(
                     df_right,
                     on=left_col.fullname,
-                    how="inner",
+                    how=join_kind,  # type: ignore
                 )
             return dfs[-1]
         else:
             return dfs[0]
 
-    @classmethod
-    def process(cls, tokens: list[Token], conn: Connection) -> dict:
-        """
-        Processes a list of tokens that were parsed from a SELECT statement.
-        The processing includes the following steps:
-            1. Processing the table identifiers
-            2. Processing the column identifiers
-            3. Processing the join mappings
-            4. Processing the filters for reading (optimizing partitions)
-            5. Processing the filters for querying (pandas query string)
-            6. Processing the SELECT of each table (list of DataFrames)
-            7. Processing the JOIN keywords (single DataFrame)
-            8. Querying the DataFrame if needed
-
-        Parameters:
-        -----------
-        tokens : list[Token]
-            A list of tokens that were parsed from the query with the SELECT
-            statement.
-        conn: Connection
-            The connection to the database where the tables are located.
-
-        Returns:
-        --------
-        dict
-            A dict with a the result of the query processing. Might contain
-            a dataframe with the requested data or an error code and message.
-
-        """
-        tables_to_select = cls._process_table_identifiers(tokens)
-        tables_to_select = cls._process_column_identifiers(
-            tokens, tables_to_select, conn
-        )
-        table_join_mappings = cls._process_join_mappings(
-            tokens, tables_to_select
-        )
-        reading_filters = cls._process_filters_for_reading(
-            tokens, tables_to_select
-        )
-        querying_filters = cls._process_filters_for_querying(
-            tokens, tables_to_select
-        )
-        select_result = cls._process_select_from_tables(
-            tables_to_select, reading_filters, conn
-        )
-        df = cls._process_join_tables(
-            select_result["data"], table_join_mappings
+    def parse(self) -> ParsingResult:
+        select_result = self.__select_from_tables()
+        df = self.__join_tables(select_result["data"])
+        if isinstance(df, ParsingResult):
+            return df
+        df = self.__compose_query_and_query_dataframe(df)
+        return ParsingResult(
+            status=True, message=str(select_result["processedFiles"]), data=df
         )
-        # The query string must be built here, referencing external
-        # variables with the correct types.
-        df = cls._compose_query_and_query_dataframe(df, querying_filters)
-        return {
-            "statusCode": 200,
-            "data": df,
-            "processedFiles": select_result["processedFiles"],
-        }
-
-
-MAPPING: dict[str, type[Processing]] = {
-    "CREATE": CREATE,
-    "ALTER": ALTER,
-    "DROP": DROP,
-    "INSERT": INSERT,
-    "UPDATE": UPDATE,
-    "DELETE": DELETE,
-    "SELECT": SELECT,
-}
-
-
-def factory(kind: str) -> type[Processing]:
-    return MAPPING[kind]
```

### Comparing `morgana_engine-0.3.1/morgana_engine/models/parsedsql.py` & `morgana_engine-0.4.0/morgana_engine/models/parsedsql.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,23 +11,25 @@
         "name",
         "alias",
         "type_str",
         "table_name",
         "table_alias",
         "has_parent_in_token",
         "partition",
+        "querying",
     ]
 
     name: str
     alias: str | None
     type_str: str | None
     table_name: str
     table_alias: str | None
     has_parent_in_token: bool
     partition: bool
+    querying: bool
 
     @property
     def fullname(self) -> str:
         if self.alias:
             fullname = self.alias
         elif not self.alias and self.table_alias and self.has_parent_in_token:
             fullname = f"{self.name}_{self.table_alias}"
```

### Comparing `morgana_engine-0.3.1/morgana_engine/models/schema.py` & `morgana_engine-0.4.0/morgana_engine/models/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,12 +78,10 @@
             return {c["name"]: c["type"] for c in self._json_dict["columns"]}
         else:
             return {}
 
     @property
     def partitions(self) -> dict[str, str]:
         if self.is_table:
-            return {
-                k["name"]: k["type"] for k in self._json_dict["partitions"]
-            }
+            return {k["name"]: k["type"] for k in self._json_dict["partitions"]}
         else:
             return {}
```

### Comparing `morgana_engine-0.3.1/morgana_engine/utils/types.py` & `morgana_engine-0.4.0/morgana_engine/utils/types.py`

 * *Files identical despite different names*

### Comparing `morgana_engine-0.3.1/morgana_engine/utils/uri.py` & `morgana_engine-0.4.0/morgana_engine/utils/uri.py`

 * *Files identical despite different names*

### Comparing `morgana_engine-0.3.1/morgana_engine.egg-info/PKG-INFO` & `morgana_engine-0.4.0/morgana_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: morgana_engine
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python module for handling partitioned data using SQL queries.
 Home-page: https://github.com/rjmalves/morgana_engine
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: sqlparse
-Requires-Dist: jsonschema
+Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: python-dotenv
 Requires-Dist: pyarrow
 Requires-Dist: boto3
 Requires-Dist: s3fs>=2023.10.0
 
 # morgana-engine
```

### Comparing `morgana_engine-0.3.1/morgana_engine.egg-info/SOURCES.txt` & `morgana_engine-0.4.0/morgana_engine.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,28 +8,37 @@
 morgana_engine.egg-info/dependency_links.txt
 morgana_engine.egg-info/requires.txt
 morgana_engine.egg-info/top_level.txt
 morgana_engine/adapters/__init__.py
 morgana_engine/adapters/repository/__init__.py
 morgana_engine/adapters/repository/connection.py
 morgana_engine/adapters/repository/dataio.py
-morgana_engine/adapters/repository/processing.py
 morgana_engine/models/__init__.py
 morgana_engine/models/parsedsql.py
 morgana_engine/models/readingfilter.py
 morgana_engine/models/schema.py
+morgana_engine/models/sql.py
 morgana_engine/services/__init__.py
-morgana_engine/services/handlers.py
+morgana_engine/services/interpreters/__init__.py
+morgana_engine/services/interpreters/lex.py
+morgana_engine/services/interpreters/parse.py
+morgana_engine/services/interpreters/parsers/__init__.py
+morgana_engine/services/interpreters/parsers/select.py
 morgana_engine/utils/__init__.py
 morgana_engine/utils/sql.py
 morgana_engine/utils/types.py
 morgana_engine/utils/uri.py
 tests/__init__.py
 tests/morgana_engine/__init__.py
 tests/morgana_engine/adapters/__init__.py
 tests/morgana_engine/adapters/repository/__init__.py
 tests/morgana_engine/adapters/repository/test_connection.py
 tests/morgana_engine/adapters/repository/test_dataio.py
-tests/morgana_engine/adapters/repository/test_processing_select.py
 tests/morgana_engine/models/__init__.py
 tests/morgana_engine/models/test_readingfilter.py
-tests/morgana_engine/models/test_schema.py
+tests/morgana_engine/models/test_schema.py
+tests/morgana_engine/services/__init__.py
+tests/morgana_engine/services/interpreters/__init__.py
+tests/morgana_engine/services/interpreters/test_lex.py
+tests/morgana_engine/services/interpreters/test_parse.py
+tests/morgana_engine/services/interpreters/parsers/__init__.py
+tests/morgana_engine/services/interpreters/parsers/test_select.py
```

### Comparing `morgana_engine-0.3.1/setup.py` & `morgana_engine-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `morgana_engine-0.3.1/tests/morgana_engine/adapters/repository/test_connection.py` & `morgana_engine-0.4.0/tests/morgana_engine/adapters/repository/test_connection.py`

 * *Files identical despite different names*

### Comparing `morgana_engine-0.3.1/tests/morgana_engine/adapters/repository/test_dataio.py` & `morgana_engine-0.4.0/tests/morgana_engine/adapters/repository/test_dataio.py`

 * *Files identical despite different names*

### Comparing `morgana_engine-0.3.1/tests/morgana_engine/models/test_readingfilter.py` & `morgana_engine-0.4.0/tests/morgana_engine/models/test_readingfilter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,318 +1,288 @@
 from morgana_engine.models.readingfilter import (
     ReadingFilter,
     EqualityReadingFilter,
     UnequalityReadingFilter,
     InSetReadingFilter,
     NotInSetReadingFilter,
 )
-from morgana_engine.models.parsedsql import Column, Table
-from morgana_engine.utils.sql import query2tokens, filter_spacing_tokens
+from morgana_engine.models.parsedsql import Column
+from morgana_engine.models.sql import SQLToken, SQLTokenType
 import pytest
 
 
 class TestReadingFilter:
-    tokens = query2tokens("SELECT * FROM table WHERE colname > 10")
-    parsed_tokens = filter_spacing_tokens(tokens[-1].tokens[1:])[0].tokens
-    table = Table(
-        name="table",
+    column = Column(
+        name="colname",
         alias=None,
-        columns=[
-            Column(
-                name="colname",
-                alias=None,
-                type_str=None,
-                table_name="table",
-                table_alias=None,
-                has_parent_in_token=False,
-                partition=False,
-            )
-        ],
+        type_str=None,
+        table_name="table",
+        table_alias=None,
+        has_parent_in_token=False,
+        partition=False,
+        querying=True,
     )
 
-    def test_column(self):
-        filter = ReadingFilter(TestReadingFilter.parsed_tokens, self.table)
-        assert filter.column == Column(
-            name="colname",
-            alias=None,
-            type_str=None,
-            table_name="table",
-            table_alias=None,
-            has_parent_in_token=False,
-            partition=False,
-        )
-
     def test_eq(self):
-        with pytest.raises(NotImplementedError):
-            tokens2 = query2tokens("SELECT * FROM table WHERE colname < 10")
-            parsed_tokens2 = filter_spacing_tokens(tokens2[-1].tokens[1:])[
-                0
-            ].tokens
-            filter1 = ReadingFilter(
-                TestReadingFilter.parsed_tokens, self.table
-            )
-            tokens2 = query2tokens("SELECT * FROM table WHERE column < 5")
-            filter2 = ReadingFilter(
-                parsed_tokens2,
-                Table(
-                    name="table",
-                    alias=None,
-                    columns=[
-                        Column(
-                            name="column",
-                            alias=None,
-                            type_str=None,
-                            table_name="table",
-                            table_alias=None,
-                            has_parent_in_token=False,
-                            partition=False,
-                        )
-                    ],
-                ),
-            )
-            assert filter1 == filter1
-            assert filter1 != filter2
+        filter1 = ReadingFilter(
+            TestReadingFilter.column,
+            SQLToken(SQLTokenType.EQUALS, "="),
+            [SQLToken(SQLTokenType.ENTITY, "10")],
+        )
+        filter2 = ReadingFilter(
+            TestReadingFilter.column,
+            SQLToken(SQLTokenType.LESS, "<"),
+            [SQLToken(SQLTokenType.ENTITY, "5")],
+        )
+        assert filter1 == filter1
+        assert filter1 != filter2
 
     def test_is_filter(self):
         with pytest.raises(NotImplementedError):
-            assert ReadingFilter.is_filter(TestReadingFilter.parsed_tokens)
+            assert ReadingFilter.is_filter(SQLToken(SQLTokenType.EQUALS, "="))
 
     def test_apply(self):
         with pytest.raises(NotImplementedError):
-            filter = ReadingFilter(TestReadingFilter.parsed_tokens, self.table)
+            filter = ReadingFilter(
+                TestReadingFilter.column,
+                SQLToken(SQLTokenType.EQUALS, "="),
+                [SQLToken(SQLTokenType.ENTITY, "10")],
+            )
             values = [5, 10, 15, 20]
             casting_func = int
             filter.apply(values, casting_func)
 
 
 class TestEqualityReadingFilter:
-    equal_tokens = query2tokens("SELECT * FROM table WHERE colname = 10")
-    parsed_equal_tokens = filter_spacing_tokens(equal_tokens[-1].tokens[1:])[
-        0
-    ].tokens
-    diff_tokens = query2tokens("SELECT * FROM table WHERE colname != 10")
-    parsed_diff_tokens = filter_spacing_tokens(diff_tokens[-1].tokens[1:])[
-        0
-    ].tokens
-    table = Table(
-        name="table",
+    equal_token = SQLToken(SQLTokenType.EQUALS, "=")
+    diff_token = SQLToken(SQLTokenType.DIFFERENT, "!=")
+    column = Column(
+        name="colname",
         alias=None,
-        columns=[
-            Column(
-                name="colname",
-                alias=None,
-                type_str=None,
-                table_name="table",
-                table_alias=None,
-                has_parent_in_token=False,
-                partition=False,
-            )
-        ],
+        type_str="int",
+        table_name="table",
+        table_alias=None,
+        has_parent_in_token=False,
+        partition=False,
+        querying=True,
     )
 
     def test_is_filter(self):
         assert EqualityReadingFilter.is_filter(
-            TestEqualityReadingFilter.parsed_equal_tokens
+            TestEqualityReadingFilter.equal_token
         )
         assert EqualityReadingFilter.is_filter(
-            TestEqualityReadingFilter.parsed_diff_tokens
+            TestEqualityReadingFilter.diff_token
         )
 
     def test_operators(self):
         filter = EqualityReadingFilter(
-            TestEqualityReadingFilter.parsed_equal_tokens,
-            TestEqualityReadingFilter.table,
+            TestEqualityReadingFilter.column,
+            TestEqualityReadingFilter.equal_token,
+            [SQLToken(SQLTokenType.ENTITY, "10")],
+        )
+        assert (
+            filter.operator.type == TestEqualityReadingFilter.equal_token.type
         )
-        assert filter.operators == ["="]
         filter = EqualityReadingFilter(
-            TestEqualityReadingFilter.parsed_diff_tokens,
-            TestEqualityReadingFilter.table,
+            TestEqualityReadingFilter.column,
+            TestEqualityReadingFilter.diff_token,
+            [SQLToken(SQLTokenType.ENTITY, "10")],
         )
-        assert filter.operators == ["!="]
+        assert filter.operator.type == TestEqualityReadingFilter.diff_token.type
 
     def test_values(self):
         filter = EqualityReadingFilter(
-            TestEqualityReadingFilter.parsed_equal_tokens,
-            TestEqualityReadingFilter.table,
+            TestEqualityReadingFilter.column,
+            TestEqualityReadingFilter.equal_token,
+            [SQLToken(SQLTokenType.ENTITY, "10")],
         )
         assert filter.values == ["10"]
 
     def test_apply(self):
         filter = EqualityReadingFilter(
-            TestEqualityReadingFilter.parsed_equal_tokens,
-            TestEqualityReadingFilter.table,
+            TestEqualityReadingFilter.column,
+            TestEqualityReadingFilter.equal_token,
+            [SQLToken(SQLTokenType.ENTITY, "10")],
         )
         values = [5, 10, 15, 20]
         casting_func = int
         assert filter.apply(values, casting_func) == [10]
         filter = EqualityReadingFilter(
-            TestEqualityReadingFilter.parsed_diff_tokens,
-            TestEqualityReadingFilter.table,
+            TestEqualityReadingFilter.column,
+            TestEqualityReadingFilter.diff_token,
+            [SQLToken(SQLTokenType.ENTITY, "10")],
         )
         values = [5, 10, 15, 20]
         casting_func = int
         assert filter.apply(values, casting_func) == [5, 15, 20]
 
 
 class TestUnequalityReadingFilter:
-    direct_gt_tokens = query2tokens("SELECT * FROM table WHERE colname > 10")
-    parsed_direct_gt_tokens = filter_spacing_tokens(
-        direct_gt_tokens[-1].tokens[1:]
-    )[0].tokens
-    reverse_le_tokens = query2tokens("SELECT * FROM table WHERE 10 <= colname")
-    parsed_reverse_le_tokens = filter_spacing_tokens(
-        reverse_le_tokens[-1].tokens[1:]
-    )[0].tokens
-    table = Table(
-        name="table",
+    gt_token = SQLToken(SQLTokenType.GREATER, ">")
+    le_token = SQLToken(SQLTokenType.LESS_EQUAL, "<=")
+    column = Column(
+        name="colname",
         alias=None,
-        columns=[
-            Column(
-                name="colname",
-                alias=None,
-                type_str=None,
-                table_name="table",
-                table_alias=None,
-                has_parent_in_token=False,
-                partition=False,
-            )
-        ],
+        type_str="int",
+        table_name="table",
+        table_alias=None,
+        has_parent_in_token=False,
+        partition=False,
+        querying=True,
     )
 
     def test_is_filter(self):
         assert UnequalityReadingFilter.is_filter(
-            TestUnequalityReadingFilter.parsed_direct_gt_tokens
+            TestUnequalityReadingFilter.gt_token
         )
         assert UnequalityReadingFilter.is_filter(
-            TestUnequalityReadingFilter.parsed_reverse_le_tokens
+            TestUnequalityReadingFilter.le_token
         )
 
     def test_operators(self):
         filter = UnequalityReadingFilter(
-            TestUnequalityReadingFilter.parsed_direct_gt_tokens,
-            TestUnequalityReadingFilter.table,
+            TestUnequalityReadingFilter.column,
+            TestUnequalityReadingFilter.gt_token,
+            [SQLToken(SQLTokenType.ENTITY, "10")],
         )
-        assert filter.operators == [">"]
+        assert filter.operator.type == TestUnequalityReadingFilter.gt_token.type
         filter = UnequalityReadingFilter(
-            TestUnequalityReadingFilter.parsed_reverse_le_tokens,
-            TestUnequalityReadingFilter.table,
+            TestUnequalityReadingFilter.column,
+            TestUnequalityReadingFilter.le_token,
+            [SQLToken(SQLTokenType.ENTITY, "10")],
         )
-        assert filter.operators == [">="]
+        assert filter.operator.type == TestUnequalityReadingFilter.le_token.type
 
     def test_values(self):
         filter = UnequalityReadingFilter(
-            TestUnequalityReadingFilter.parsed_direct_gt_tokens,
-            TestUnequalityReadingFilter.table,
+            TestUnequalityReadingFilter.column,
+            TestUnequalityReadingFilter.gt_token,
+            [SQLToken(SQLTokenType.ENTITY, "10")],
         )
         assert filter.values == ["10"]
 
     def test_apply(self):
         filter = UnequalityReadingFilter(
-            TestUnequalityReadingFilter.parsed_direct_gt_tokens,
-            TestUnequalityReadingFilter.table,
+            TestUnequalityReadingFilter.column,
+            TestUnequalityReadingFilter.gt_token,
+            [SQLToken(SQLTokenType.ENTITY, "10")],
         )
         values = [5, 10, 15, 20]
         casting_func = int
         assert filter.apply(values, casting_func) == [15, 20]
         filter = UnequalityReadingFilter(
-            TestUnequalityReadingFilter.parsed_reverse_le_tokens,
-            TestUnequalityReadingFilter.table,
+            TestUnequalityReadingFilter.column,
+            TestUnequalityReadingFilter.le_token,
+            [SQLToken(SQLTokenType.ENTITY, "10")],
         )
         values = [5, 10, 15, 20]
         casting_func = int
-        assert filter.apply(values, casting_func) == [10, 15, 20]
+        assert filter.apply(values, casting_func) == [5, 10]
 
 
 class TestInSetReadingFilter:
-    tokens = query2tokens("SELECT * FROM table WHERE colname IN (10, 15)")
-    parsed_tokens = filter_spacing_tokens(tokens[-1].tokens[1:])
-    table = Table(
-        name="table",
+    in_token = SQLToken(SQLTokenType.IN, "IN")
+    column = Column(
+        name="colname",
         alias=None,
-        columns=[
-            Column(
-                name="colname",
-                alias=None,
-                type_str=None,
-                table_name="table",
-                table_alias=None,
-                has_parent_in_token=False,
-                partition=False,
-            )
-        ],
+        type_str="int",
+        table_name="table",
+        table_alias=None,
+        has_parent_in_token=False,
+        partition=False,
+        querying=True,
     )
 
     def test_is_filter(self):
-        assert InSetReadingFilter.is_filter(
-            TestInSetReadingFilter.parsed_tokens
-        )
+        assert InSetReadingFilter.is_filter(TestInSetReadingFilter.in_token)
 
     def test_operators(self):
         filter = InSetReadingFilter(
-            TestInSetReadingFilter.parsed_tokens,
-            TestInSetReadingFilter.table,
+            TestInSetReadingFilter.column,
+            TestInSetReadingFilter.in_token,
+            [
+                SQLToken(SQLTokenType.ENTITY, "10"),
+                SQLToken(SQLTokenType.ENTITY, "15"),
+            ],
         )
-        assert filter.operators == ["IN"]
+        assert filter.operator.type == TestInSetReadingFilter.in_token.type
 
     def test_values(self):
         filter = InSetReadingFilter(
-            TestInSetReadingFilter.parsed_tokens,
-            TestInSetReadingFilter.table,
+            TestInSetReadingFilter.column,
+            TestInSetReadingFilter.in_token,
+            [
+                SQLToken(SQLTokenType.ENTITY, "10"),
+                SQLToken(SQLTokenType.ENTITY, "15"),
+            ],
         )
         assert filter.values == ["10", "15"]
 
     def test_apply(self):
         filter = InSetReadingFilter(
-            TestInSetReadingFilter.parsed_tokens,
-            TestInSetReadingFilter.table,
+            TestInSetReadingFilter.column,
+            TestInSetReadingFilter.in_token,
+            [
+                SQLToken(SQLTokenType.ENTITY, "10"),
+                SQLToken(SQLTokenType.ENTITY, "15"),
+            ],
         )
         values = [5, 10, 15, 20]
         casting_func = int
         assert filter.apply(values, casting_func) == [10, 15]
 
 
 class TestNotInSetReadingFilter:
-    tokens = query2tokens("SELECT * FROM table WHERE colname NOT IN (10, 15)")
-    parsed_tokens = filter_spacing_tokens(tokens[-1].tokens[1:])
-    table = Table(
-        name="table",
+    not_in_token = SQLToken(SQLTokenType.NOT_IN, "NOT IN")
+    column = Column(
+        name="colname",
         alias=None,
-        columns=[
-            Column(
-                name="colname",
-                alias=None,
-                type_str=None,
-                table_name="table",
-                table_alias=None,
-                has_parent_in_token=False,
-                partition=False,
-            )
-        ],
+        type_str="int",
+        table_name="table",
+        table_alias=None,
+        has_parent_in_token=False,
+        partition=False,
+        querying=True,
     )
 
     def test_is_filter(self):
         assert NotInSetReadingFilter.is_filter(
-            TestNotInSetReadingFilter.parsed_tokens
+            TestNotInSetReadingFilter.not_in_token
         )
 
     def test_operators(self):
         filter = NotInSetReadingFilter(
-            TestNotInSetReadingFilter.parsed_tokens,
-            TestNotInSetReadingFilter.table,
+            TestNotInSetReadingFilter.column,
+            TestNotInSetReadingFilter.not_in_token,
+            [
+                SQLToken(SQLTokenType.ENTITY, "10"),
+                SQLToken(SQLTokenType.ENTITY, "15"),
+            ],
+        )
+        assert (
+            filter.operator.type == TestNotInSetReadingFilter.not_in_token.type
         )
-        assert filter.operators == ["NOT", "IN"]
 
     def test_values(self):
         filter = NotInSetReadingFilter(
-            TestNotInSetReadingFilter.parsed_tokens,
-            TestNotInSetReadingFilter.table,
+            TestNotInSetReadingFilter.column,
+            TestNotInSetReadingFilter.not_in_token,
+            [
+                SQLToken(SQLTokenType.ENTITY, "10"),
+                SQLToken(SQLTokenType.ENTITY, "15"),
+            ],
         )
         assert filter.values == ["10", "15"]
 
     def test_apply(self):
         filter = NotInSetReadingFilter(
-            TestNotInSetReadingFilter.parsed_tokens,
-            TestNotInSetReadingFilter.table,
+            TestNotInSetReadingFilter.column,
+            TestNotInSetReadingFilter.not_in_token,
+            [
+                SQLToken(SQLTokenType.ENTITY, "10"),
+                SQLToken(SQLTokenType.ENTITY, "15"),
+            ],
         )
         values = [5, 10, 15, 20]
         casting_func = int
         assert filter.apply(values, casting_func) == [5, 20]
```

### Comparing `morgana_engine-0.3.1/tests/morgana_engine/models/test_schema.py` & `morgana_engine-0.4.0/tests/morgana_engine/models/test_schema.py`

 * *Files identical despite different names*

