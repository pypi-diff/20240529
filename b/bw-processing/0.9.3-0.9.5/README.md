# Comparing `tmp/bw_processing-0.9.3.tar.gz` & `tmp/bw_processing-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_processing-0.9.3.tar", last modified: Sun May 12 09:52:23 2024, max compression
+gzip compressed data, was "bw_processing-0.9.5.tar", last modified: Wed May 29 13:19:12 2024, max compression
```

## Comparing `bw_processing-0.9.3.tar` & `bw_processing-0.9.5.tar`

### file list

```diff
@@ -1,49 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:23.351599 bw_processing-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-12 09:52:19.000000 bw_processing-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 09:52:19.000000 bw_processing-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-05-12 09:52:23.351599 bw_processing-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-05-12 09:52:19.000000 bw_processing-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:23.347599 bw_processing-0.9.3/bw_processing/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/array_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    44620 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/datapackage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:23.351599 bw_processing-0.9.3/bw_processing/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/examples/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/examples/parquet_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/examples/simple.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/io_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/io_parquet_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/io_pyarrow_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/merging.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/unique_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-12 09:52:19.000000 bw_processing-0.9.3/bw_processing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:23.351599 bw_processing-0.9.3/bw_processing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-05-12 09:52:23.000000 bw_processing-0.9.3/bw_processing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-12 09:52:23.000000 bw_processing-0.9.3/bw_processing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 09:52:23.000000 bw_processing-0.9.3/bw_processing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 09:52:23.000000 bw_processing-0.9.3/bw_processing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-12 09:52:23.000000 bw_processing-0.9.3/bw_processing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-12 09:52:23.000000 bw_processing-0.9.3/bw_processing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:23.347599 bw_processing-0.9.3/dev/
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-12 09:52:19.000000 bw_processing-0.9.3/dev/calculation_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-12 09:52:19.000000 bw_processing-0.9.3/dev/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-12 09:52:19.000000 bw_processing-0.9.3/dev/processed_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-12 09:52:19.000000 bw_processing-0.9.3/dev/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-12 09:52:19.000000 bw_processing-0.9.3/dev/speed_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:23.347599 bw_processing-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-12 09:52:19.000000 bw_processing-0.9.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-12 09:52:19.000000 bw_processing-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-12 09:52:23.351599 bw_processing-0.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:23.351599 bw_processing-0.9.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:23.347599 bw_processing-0.9.3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-12 09:52:19.000000 bw_processing-0.9.3/tests/fixtures/basic_arrays.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:23.347599 bw_processing-0.9.3/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-12 09:52:19.000000 bw_processing-0.9.3/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-12 09:52:19.000000 bw_processing-0.9.3/tests/helpers/basic_array_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-12 09:52:19.000000 bw_processing-0.9.3/tests/test_utils.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-29 13:19:12.127644 bw_processing-0.9.5/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1456 2024-04-04 08:00:20.000000 bw_processing-0.9.5/LICENSE
+-rw-r--r--   0 cmutel     (501) staff       (20)      116 2024-05-28 19:48:33.000000 bw_processing-0.9.5/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)    16467 2024-05-29 13:19:12.127260 bw_processing-0.9.5/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)    14929 2024-05-28 19:26:54.000000 bw_processing-0.9.5/README.md
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-29 13:19:12.122655 bw_processing-0.9.5/bw_processing/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1376 2024-05-29 13:18:24.000000 bw_processing-0.9.5/bw_processing/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     5844 2024-05-11 22:54:08.000000 bw_processing-0.9.5/bw_processing/array_creation.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1340 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/constants.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    44188 2024-05-22 11:58:14.000000 bw_processing-0.9.5/bw_processing/datapackage.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1400 2024-05-11 22:54:08.000000 bw_processing-0.9.5/bw_processing/errors.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-29 13:19:12.124170 bw_processing-0.9.5/bw_processing/examples/
+-rw-r--r--   0 cmutel     (501) staff       (20)       73 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/examples/__init__.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-29 13:19:12.124397 bw_processing-0.9.5/bw_processing/examples/__pycache__/
+-rw-r--r--   0 cmutel     (501) staff       (20)      342 2024-05-11 01:13:00.000000 bw_processing-0.9.5/bw_processing/examples/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-29 13:19:12.126183 bw_processing-0.9.5/bw_processing/examples/datapackage_1/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1012 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/examples/datapackage_1/another name.indices.parquet
+-rw-r--r--   0 cmutel     (501) staff       (20)     3391 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/examples/datapackage_1/datapackage.json
+-rw-r--r--   0 cmutel     (501) staff       (20)      679 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/examples/datapackage_1/sa-data-vector-from-dict.data.parquet
+-rw-r--r--   0 cmutel     (501) staff       (20)     2360 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/examples/datapackage_1/sa-data-vector-from-dict.distributions.parquet
+-rw-r--r--   0 cmutel     (501) staff       (20)      577 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/examples/datapackage_1/sa-data-vector-from-dict.flip.parquet
+-rw-r--r--   0 cmutel     (501) staff       (20)     1012 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/examples/datapackage_1/sa-data-vector-from-dict.indices.parquet
+-rw-r--r--   0 cmutel     (501) staff       (20)      753 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/examples/datapackage_1/some name.data.parquet
+-rw-r--r--   0 cmutel     (501) staff       (20)      577 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/examples/datapackage_1/some name.flip.parquet
+-rw-r--r--   0 cmutel     (501) staff       (20)     1012 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/examples/datapackage_1/some name.indices.parquet
+-rw-r--r--   0 cmutel     (501) staff       (20)     5606 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/examples/datapackage_2.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)      602 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/examples/interfaces.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3705 2024-05-28 19:36:24.000000 bw_processing-0.9.5/bw_processing/examples/parquet_files.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      772 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/examples/simple.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)     1631 2024-05-22 11:58:13.000000 bw_processing-0.9.5/bw_processing/filesystem.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     5673 2024-05-22 11:58:13.000000 bw_processing-0.9.5/bw_processing/indexing.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     5003 2024-05-22 11:58:13.000000 bw_processing-0.9.5/bw_processing/io_helpers.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4916 2024-05-28 19:31:35.000000 bw_processing-0.9.5/bw_processing/io_parquet_helpers.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     8365 2024-05-22 11:58:13.000000 bw_processing-0.9.5/bw_processing/io_pyarrow_helpers.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     6248 2024-05-22 11:58:13.000000 bw_processing-0.9.5/bw_processing/merging.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      493 2024-05-11 22:54:08.000000 bw_processing-0.9.5/bw_processing/proxies.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3823 2024-04-04 08:00:20.000000 bw_processing-0.9.5/bw_processing/unique_fields.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3200 2024-05-12 09:50:17.000000 bw_processing-0.9.5/bw_processing/utils.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-29 13:19:12.126527 bw_processing-0.9.5/bw_processing.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)    16467 2024-05-29 13:19:12.000000 bw_processing-0.9.5/bw_processing.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     2276 2024-05-29 13:19:12.000000 bw_processing-0.9.5/bw_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-29 13:19:12.000000 bw_processing-0.9.5/bw_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)      163 2024-05-29 13:19:12.000000 bw_processing-0.9.5/bw_processing.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       14 2024-05-29 13:19:12.000000 bw_processing-0.9.5/bw_processing.egg-info/top_level.txt
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-29 13:19:12.119113 bw_processing-0.9.5/dev/
+-rw-r--r--   0 cmutel     (501) staff       (20)     6528 2024-04-04 08:00:20.000000 bw_processing-0.9.5/dev/calculation_package.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4240 2024-04-04 08:00:20.000000 bw_processing-0.9.5/dev/loading.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     9654 2024-04-04 08:00:20.000000 bw_processing-0.9.5/dev/processed_package.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      741 2024-04-04 08:00:20.000000 bw_processing-0.9.5/dev/resources.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1195 2024-04-04 08:00:20.000000 bw_processing-0.9.5/dev/speed_tests.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-29 13:19:12.119238 bw_processing-0.9.5/docs/
+-rw-r--r--   0 cmutel     (501) staff       (20)     2872 2024-05-10 20:43:49.000000 bw_processing-0.9.5/docs/conf.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2465 2024-05-28 19:45:20.000000 bw_processing-0.9.5/pyproject.toml
+-rw-r--r--   0 cmutel     (501) staff       (20)       38 2024-05-29 13:19:12.127694 bw_processing-0.9.5/setup.cfg
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-29 13:19:12.126339 bw_processing-0.9.5/tests/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-29 13:19:12.119471 bw_processing-0.9.5/tests/fixtures/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1065 2024-04-04 08:00:20.000000 bw_processing-0.9.5/tests/fixtures/basic_arrays.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-29 13:19:12.119945 bw_processing-0.9.5/tests/helpers/
+-rw-r--r--   0 cmutel     (501) staff       (20)      112 2024-04-04 08:00:20.000000 bw_processing-0.9.5/tests/helpers/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      843 2024-04-04 08:00:20.000000 bw_processing-0.9.5/tests/helpers/basic_array_helpers.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     6803 2024-05-22 11:58:12.000000 bw_processing-0.9.5/tests/test_utils.py
```

### Comparing `bw_processing-0.9.3/LICENSE` & `bw_processing-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/PKG-INFO` & `bw_processing-0.9.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 Metadata-Version: 2.1
-Name: bw-processing
-Version: 0.9.3
-Summary: Tools to create structured arrays in a common format
-Home-page: https://github.com/brightway-lca/bw_processing
-Author: Chris Mutel
-Author-email: <cmutel@gmail.com>
-Maintainer: Chris Mutel
-Maintainer-email: <cmutel@gmail.com>
-License: BSD-3-Clause
+Name: bw_processing
+Version: 0.9.5
+Summary: Foo
+Author-email: Chris Mutel <cmutel@gmail.com>
+Maintainer-email: Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/brightway-lca/bw_processing
 Project-URL: homepage, https://github.com/brightway-lca/bw_processing
 Project-URL: tracker, https://github.com/brightway-lca/bw_processing/issues
-Keywords: "brightway","development"
-Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fs
+Requires-Dist: fsspec
+Requires-Dist: morefs
 Requires-Dist: numpy
 Requires-Dist: pandas
 Provides-Extra: testing
-Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: bw_processing; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pyarrow; extra == "testing"
+Requires-Dist: python-coveralls; extra == "testing"
 Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
-Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: myst_parser; extra == "docs"
-Requires-Dist: furo; extra == "docs"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-randomly; extra == "dev"
+Requires-Dist: setuptools; extra == "dev"
 
 # bw-processing
 
 Library for storing numeric data for use in matrix-based calculations. Designed for use with the [Brightway life cycle assessment framework](https://brightway.dev/).
 
 [![PyPI](https://img.shields.io/pypi/v/bw-processing.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/bw-processing.svg)][pypi status]
@@ -144,41 +143,41 @@
 ```
 
 #### Interface dehydrating and rehydrating
 
 Serialized datapackages cannot contain executable code, both because of our chosen data formats, and for security reasons. Therefore, when loading a datapackage with an interface, that interface object needs to be reconstituted as Python code - we call this cycle dehydration and rehydration. Dehydration happens automatically when a datapackage is finalized with `finalize_serialization()`, but rehydration needs to be done manually using `rehydrate_interface()`. For example:
 
 ```python
-from fs.zipfs import ZipFS
+from fsspec.implementations.zip import ZipFileSystem
 from bw_processing import load_datapackage
 
-my_dp = load_datapackage(ZipFS("some-path.zip"))
+my_dp = load_datapackage(ZipFileSystem("some-path.zip"))
 my_dp.rehydrate_interface("some-resource-name", ExampleVectorInterface())
 ```
 
 You can list the dehydrated interfaces present with `.dehydrated_interfaces()`.
 
 You can store useful information for the interface object initialization under the resource key `config`. This can be used in instantiating an interface if you pass `initialize_with_config`:
 
 ```python
-from fs.zipfs import ZipFS
+from fsspec.implementations.zip import ZipFileSystem
 from bw_processing import load_datapackage
 import requests
 import numpy as np
 
 
 class MyInterface:
     def __init__(self, url):
         self.url = url
 
     def __next__(self):
         return np.array(requests.get(self.url).json())
 
 
-my_dp = load_datapackage(ZipFS("some-path.zip"))
+my_dp = load_datapackage(ZipFileSystem("some-path.zip"))
 data_obj, resource_metadata = my_dp.get_resource("some-interface")
 print(resource_metadata['config'])
 >>> {"url": "example.com"}
 
 my_dp.rehydrate_interface("some-interface", MyInterface, initialize_with_config=True)
 # interface is substituted, need to retrieve it again
 data_obj, resource_metadata = my_dp.get_resource("some-interface")
```

### Comparing `bw_processing-0.9.3/README.md` & `bw_processing-0.9.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -103,41 +103,41 @@
 ```
 
 #### Interface dehydrating and rehydrating
 
 Serialized datapackages cannot contain executable code, both because of our chosen data formats, and for security reasons. Therefore, when loading a datapackage with an interface, that interface object needs to be reconstituted as Python code - we call this cycle dehydration and rehydration. Dehydration happens automatically when a datapackage is finalized with `finalize_serialization()`, but rehydration needs to be done manually using `rehydrate_interface()`. For example:
 
 ```python
-from fs.zipfs import ZipFS
+from fsspec.implementations.zip import ZipFileSystem
 from bw_processing import load_datapackage
 
-my_dp = load_datapackage(ZipFS("some-path.zip"))
+my_dp = load_datapackage(ZipFileSystem("some-path.zip"))
 my_dp.rehydrate_interface("some-resource-name", ExampleVectorInterface())
 ```
 
 You can list the dehydrated interfaces present with `.dehydrated_interfaces()`.
 
 You can store useful information for the interface object initialization under the resource key `config`. This can be used in instantiating an interface if you pass `initialize_with_config`:
 
 ```python
-from fs.zipfs import ZipFS
+from fsspec.implementations.zip import ZipFileSystem
 from bw_processing import load_datapackage
 import requests
 import numpy as np
 
 
 class MyInterface:
     def __init__(self, url):
         self.url = url
 
     def __next__(self):
         return np.array(requests.get(self.url).json())
 
 
-my_dp = load_datapackage(ZipFS("some-path.zip"))
+my_dp = load_datapackage(ZipFileSystem("some-path.zip"))
 data_obj, resource_metadata = my_dp.get_resource("some-interface")
 print(resource_metadata['config'])
 >>> {"url": "example.com"}
 
 my_dp.rehydrate_interface("some-interface", MyInterface, initialize_with_config=True)
 # interface is substituted, need to retrieve it again
 data_obj, resource_metadata = my_dp.get_resource("some-interface")
```

### Comparing `bw_processing-0.9.3/bw_processing/__init__.py` & `bw_processing-0.9.5/bw_processing/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,24 +22,19 @@
     "reset_index",
     "safe_filename",
     "simple_graph",
     "UNCERTAINTY_DTYPE",
     "UndefinedInterface",
 )
 
-__version__ = "0.9.3"
+__version__ = "0.9.5"
 
 
 from .array_creation import create_array, create_structured_array
-from .constants import (
-    DEFAULT_LICENSES,
-    INDICES_DTYPE,
-    UNCERTAINTY_DTYPE,
-    MatrixSerializeFormat,
-)
+from .constants import DEFAULT_LICENSES, INDICES_DTYPE, UNCERTAINTY_DTYPE, MatrixSerializeFormat
 from .datapackage import (
     Datapackage,
     DatapackageBase,
     FilteredDatapackage,
     create_datapackage,
     load_datapackage,
     simple_graph,
```

### Comparing `bw_processing-0.9.3/bw_processing/array_creation.py` & `bw_processing-0.9.5/bw_processing/array_creation.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/bw_processing/constants.py` & `bw_processing-0.9.5/bw_processing/constants.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/bw_processing/datapackage.py` & `bw_processing-0.9.5/bw_processing/datapackage.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import uuid
 from abc import ABC
 from functools import partial
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
-from fs.base import FS
-from fs.errors import ResourceNotFound
-from fs.memoryfs import MemoryFS
+from fsspec import AbstractFileSystem
+
+# Use this instead of fsspec MemoryFileSystem because that is a singleton!?
+from morefs.dict import DictFS
 
 from .constants import (
     DEFAULT_LICENSES,
     INDICES_DTYPE,
     NUMPY_SERIALIZE_FORMAT_EXTENSION,
     NUMPY_SERIALIZE_FORMAT_NAME,
     PARQUET_SERIALIZE_FORMAT_EXTENSION,
@@ -105,55 +106,45 @@
                 raise NonUnique("This name present at indices: {}".format(indices))
             else:
                 return indices[0]
 
     def del_resource(self, name_or_index: Union[str, int]) -> None:
         """Remove a resource, and delete its data file, if any."""
         if self._modified:
-            raise PotentialInconsistency(
-                "Datapackage is modified; save modifications or reload"
-            )
+            raise PotentialInconsistency("Datapackage is modified; save modifications or reload")
 
         index = self._get_index(name_or_index)
 
         try:
-            self.fs.remove(self.resources[index]["path"])
-        except (KeyError, ResourceNotFound):
+            self.fs.rm(self.resources[index]["path"])
+        except (KeyError, FileNotFoundError):
             # Interface has no path
             pass
 
         del self.resources[index]
         del self.data[index]
 
     def del_resource_group(self, name: str) -> None:
         """Remove a resource group, and delete its data files, if any.
 
         Use ``exclude_resource_group`` if you want to keep the underlying resource in the filesystem.
         """
         if self._modified:
-            raise PotentialInconsistency(
-                "Datapackage is modified; save modifications or reload"
-            )
+            raise PotentialInconsistency("Datapackage is modified; save modifications or reload")
 
-        indices = [
-            i
-            for i, resource in enumerate(self.resources)
-            if resource.get("group") == name
-        ]
+        indices = [i for i, resource in enumerate(self.resources) if resource.get("group") == name]
 
         for obj in (obj for i, obj in enumerate(self.resources) if i in indices):
             try:
-                self.fs.remove(obj["path"])
-            except (KeyError, ResourceNotFound):
+                self.fs.rm(obj["path"])
+            except (KeyError, FileNotFoundError):
                 # Interface has no path
                 pass
 
-        self.resources = [
-            obj for i, obj in enumerate(self.resources) if i not in indices
-        ]
+        self.resources = [obj for i, obj in enumerate(self.resources) if i not in indices]
         self.data = [obj for i, obj in enumerate(self.data) if i not in indices]
 
     def get_resource(self, name_or_index: Union[str, int]) -> (Any, dict):
         """Return data and metadata for ``name_or_index``.
 
         Args:
 
@@ -184,17 +175,15 @@
 
         This method was introduced to allow for the efficient construction of matrices; each datapackage can have data for multiple matrices, and we can then create filtered datapackages which exclusively have data for the matrix of interest. As such, they should be considered read-only, though this is not enforced.
         """
         fdp = FilteredDatapackage()
         fdp.fs = self.fs
         fdp.metadata = {k: v for k, v in self.metadata.items() if k != "resources"}
         fdp.metadata["resources"] = []
-        to_include = [
-            i for i, resource in enumerate(self.resources) if resource.get(key) == value
-        ]
+        to_include = [i for i, resource in enumerate(self.resources) if resource.get(key) == value]
         fdp.data = [o for i, o in enumerate(self.data) if i in to_include]
         fdp.resources = [o for i, o in enumerate(self.resources) if i in to_include]
         if hasattr(self, "indexer"):
             fdp.indexer = self.indexer
         return fdp
 
     def exclude(self, filters: Dict[str, str]) -> "FilteredDatapackage":
@@ -221,25 +210,21 @@
 
         indices_to_include = [
             i
             for i, resource in enumerate(self.resources)
             if any(resource.get(key) != value for key, value in filters.items())
         ]
         fdp.data = [o for i, o in enumerate(self.data) if i in indices_to_include]
-        fdp.resources = [
-            o for i, o in enumerate(self.resources) if i in indices_to_include
-        ]
+        fdp.resources = [o for i, o in enumerate(self.resources) if i in indices_to_include]
         return fdp
 
     def _dehydrate_interfaces(self) -> None:
         """Substitute an interface resource with ``UndefinedInterface``, in preparation for finalizing data on disk."""
         interface_indices = [
-            index
-            for index, obj in enumerate(self.resources)
-            if obj["profile"] == "interface"
+            index for index, obj in enumerate(self.resources) if obj["profile"] == "interface"
         ]
 
         for index in interface_indices:
             self.data[index] = UndefinedInterface()
 
     def dehydrated_interfaces(self) -> List[str]:
         """Return a list of the resource groups which have dehydrated interfaces"""
@@ -297,26 +282,26 @@
     """
 
     # To allow these packages to be used as Python keys
     def __hash__(self):
         return hash((self.fs, self.metadata))
 
     def __eq__(self, other):
-        return (self.fs, self.metadata) == (other.fs, other.metadata)
+        return (id(self.fs), self.metadata) == (id(other.fs), other.metadata)
 
     def _check_length_consistency(self) -> None:
         if len(self.resources) != len(self.data):
             raise LengthMismatch(
                 "Number of resources ({}) doesn't match number of data objects ({})".format(
                     len(self.resources), len(self.data)
                 )
             )
 
     def _load(
-        self, fs: FS, mmap_mode: Optional[str] = None, proxy: bool = False
+        self, fs: AbstractFileSystem, mmap_mode: Optional[str] = None, proxy: bool = False
     ) -> None:
         self.fs = fs
         self.metadata = file_reader(
             fs=self.fs, resource="datapackage.json", mimetype="application/json"
         )
         self.data = []
         self._load_all(mmap_mode=mmap_mode, proxy=proxy)
@@ -334,15 +319,15 @@
                     )
                 )
             except (InvalidMimetype, KeyError):
                 self.data.append(UndefinedInterface())
 
     def _create(
         self,
-        fs: Optional[FS],
+        fs: Optional[AbstractFileSystem],
         name: Optional[str],
         id_: Optional[str],
         metadata: Optional[dict],
         combinatorial: bool = False,
         sequential: bool = False,
         seed: Optional[int] = None,
         sum_intra_duplicates: bool = True,
@@ -354,15 +339,15 @@
         All metadata elements should follow the `datapackage specification <https://frictionlessdata.io/specs/data-package/>`__.
 
         Licenses are specified as a list in ``metadata``. The default license is the `Open Data Commons Public Domain Dedication and License v1.0 <http://opendatacommons.org/licenses/pddl/>`__.
         """
         name = clean_datapackage_name(name or uuid.uuid4().hex)
         check_name(name)
 
-        self.fs = fs or MemoryFS()
+        self.fs = fs or DictFS()
         if not isinstance(matrix_serialize_format_type, MatrixSerializeFormat):
             raise TypeError(
                 f"Matrix serialize format type ({matrix_serialize_format_type}) not recognized!"
             )
         self._matrix_serialize_format_type = matrix_serialize_format_type
 
         self.metadata = {
@@ -384,27 +369,28 @@
                 self.metadata[k] = v
 
         self.data = []
 
     def finalize_serialization(self) -> None:
         if self._finalized:
             raise Closed("Datapackage already finalized")
-        elif isinstance(self.fs, MemoryFS):
+        elif isinstance(self.fs, DictFS):
             raise ValueError("In-memory file systems can't be serialized")
 
         self._dehydrate_interfaces()
         self._check_length_consistency()
 
         file_writer(
             data=self.metadata,
             fs=self.fs,
             resource="datapackage.json",
             mimetype="application/json",
         )
-        self.fs.close()
+        if hasattr(self.fs, "close"):
+            self.fs.close()
         self._finalized = True
 
     def _prepare_modifications(self) -> None:
         self._check_length_consistency()
 
         if self._finalized:
             raise Closed("Datapackage already finalized")
@@ -467,17 +453,15 @@
         **kwargs,
     ) -> None:
         """ """
         self._prepare_modifications()
 
         # Check lengths
 
-        kwargs.update(
-            {"matrix": matrix, "category": "vector", "nrows": len(indices_array)}
-        )
+        kwargs.update({"matrix": matrix, "category": "vector", "nrows": len(indices_array)})
         name = self._prepare_name(name)
 
         indices_array = load_bytes(indices_array)
         self._add_numpy_array_resource(
             array=indices_array,
             name=name + ".indices",
             group=name,
@@ -512,17 +496,15 @@
                 meta_object="vector",
                 meta_type="generic",
                 **kwargs,
             )
         if distributions_array is not None:
             distributions_array = load_bytes(distributions_array)
             # If no uncertainty, don't need to store it
-            if (distributions_array["uncertainty_type"] < 2).sum() < len(
-                distributions_array
-            ):
+            if (distributions_array["uncertainty_type"] < 2).sum() < len(distributions_array):
                 if distributions_array.shape != indices_array.shape:
                     raise ShapeMismatch(
                         "`distributions_array` shape ({}) doesn't match `indices_array` ({}).".format(
                             distributions_array.shape, indices_array.shape
                         )
                     )
                 self._add_numpy_array_resource(
@@ -538,17 +520,15 @@
                 )
         if flip_array is not None:
             flip_array = load_bytes(flip_array)
             # If no flips, don't need to store it
             if flip_array.sum():
                 if flip_array.dtype != bool:
                     raise WrongDatatype(
-                        "`flip_array` dtype is {}, but must be `bool`".format(
-                            flip_array.dtype
-                        )
+                        "`flip_array` dtype is {}, but must be `bool`".format(flip_array.dtype)
                     )
                 elif flip_array.shape != indices_array.shape:
                     raise ShapeMismatch(
                         "`flip_array` shape ({}) doesn't match `indices_array` ({}).".format(
                             flip_array.shape, indices_array.shape
                         )
                     )
@@ -575,17 +555,15 @@
         keep_proxy: bool = False,
         matrix_serialize_format_type: Optional[MatrixSerializeFormat] = None,
         **kwargs,
     ) -> None:
         """ """
         self._prepare_modifications()
 
-        kwargs.update(
-            {"matrix": matrix, "category": "array", "nrows": len(indices_array)}
-        )
+        kwargs.update({"matrix": matrix, "category": "array", "nrows": len(indices_array)})
         name = self._prepare_name(name)
 
         indices_array = load_bytes(indices_array)
         self._add_numpy_array_resource(
             array=indices_array,
             name=name + ".indices",
             kind="indices",
@@ -622,17 +600,15 @@
             **kwargs,
         )
         if flip_array is not None:
             flip_array = load_bytes(flip_array)
             if flip_array.sum():
                 if flip_array.dtype != bool:
                     raise WrongDatatype(
-                        "`flip_array` dtype is {}, but must be `bool`".format(
-                            flip_array.dtype
-                        )
+                        "`flip_array` dtype is {}, but must be `bool`".format(flip_array.dtype)
                     )
                 elif flip_array.shape != indices_array.shape:
                     raise ShapeMismatch(
                         "`flip_array` shape ({}) doesn't match `indices_array` ({}).".format(
                             flip_array.shape, indices_array.shape
                         )
                     )
@@ -712,17 +688,15 @@
         kind: str,
         keep_proxy: bool = False,
         matrix_serialize_format_type: Optional[MatrixSerializeFormat] = None,
         meta_object: Optional[str] = None,
         meta_type: Optional[str] = None,
         **kwargs,
     ) -> None:
-        assert (
-            array.ndim <= 2
-        ), f"Numpy array should be of dim 2 or less instead of {array.ndim}!"
+        assert array.ndim <= 2, f"Numpy array should be of dim 2 or less instead of {array.ndim}!"
 
         if matrix_serialize_format_type is None:
             # use instance default serialization format
             matrix_serialize_format_type = self._matrix_serialize_format_type
         else:
             assert isinstance(
                 matrix_serialize_format_type, MatrixSerializeFormat
@@ -737,21 +711,21 @@
             filename = check_suffix(name, PARQUET_SERIALIZE_FORMAT_EXTENSION)
             format = PARQUET_SERIALIZE_FORMAT_NAME
         else:
             raise TypeError(
                 f"Matrix serialize format type {matrix_serialize_format_type} is not recognized!"
             )
 
-        if not isinstance(self.fs, MemoryFS):
+        if not isinstance(self.fs, DictFS):
             file_writer(
                 data=array,
                 fs=self.fs,
                 resource=filename,
                 mimetype="application/octet-stream",
-                matrix_serialize_format_type=matrix_serialize_format_type,  # NIKO
+                matrix_serialize_format_type=matrix_serialize_format_type,
                 meta_object=meta_object,
                 meta_type=meta_type,
             )
 
         if keep_proxy:
             self.data.append(
                 file_reader(
@@ -789,17 +763,15 @@
         flip_array: Optional[np.ndarray] = None,  # Not interface
         keep_proxy: bool = False,
         matrix_serialize_format_type: Optional[MatrixSerializeFormat] = None,
         **kwargs,
     ) -> None:
         self._prepare_modifications()
 
-        kwargs.update(
-            {"matrix": matrix, "category": "vector", "nrows": len(indices_array)}
-        )
+        kwargs.update({"matrix": matrix, "category": "vector", "nrows": len(indices_array)})
         name = self._prepare_name(name)
 
         indices_array = load_bytes(indices_array)
         self._add_numpy_array_resource(
             array=indices_array,
             name=name + ".indices",
             group=name,
@@ -811,17 +783,15 @@
             **kwargs,
         )
         if flip_array is not None:
             flip_array = load_bytes(flip_array)
             if flip_array.sum():
                 if flip_array.dtype != bool:
                     raise WrongDatatype(
-                        "`flip_array` dtype is {}, but must be `bool`".format(
-                            flip_array.dtype
-                        )
+                        "`flip_array` dtype is {}, but must be `bool`".format(flip_array.dtype)
                     )
                 elif flip_array.shape != indices_array.shape:
                     raise ShapeMismatch(
                         "`flip_array` shape ({}) doesn't match `indices_array` ({}).".format(
                             flip_array.shape, indices_array.shape
                         )
                     )
@@ -861,17 +831,15 @@
     ) -> None:
         """`interface` must support the presamples API."""
         self._prepare_modifications()
 
         if isinstance(flip_array, np.ndarray) and not flip_array.sum():
             flip_array = None
 
-        kwargs.update(
-            {"matrix": matrix, "category": "array", "nrows": len(indices_array)}
-        )
+        kwargs.update({"matrix": matrix, "category": "array", "nrows": len(indices_array)})
         name = self._prepare_name(name)
 
         indices_array = load_bytes(indices_array)
         self._add_numpy_array_resource(
             array=indices_array,
             name=name + ".indices",
             group=name,
@@ -883,17 +851,15 @@
             **kwargs,
         )
         if flip_array is not None:
             flip_array = load_bytes(flip_array)
             if flip_array.sum():
                 if flip_array.dtype != bool:
                     raise WrongDatatype(
-                        "`flip_array` dtype is {}, but must be `bool`".format(
-                            flip_array.dtype
-                        )
+                        "`flip_array` dtype is {}, but must be `bool`".format(flip_array.dtype)
                     )
                 elif flip_array.shape != indices_array.shape:
                     raise ShapeMismatch(
                         "`flip_array` shape ({}) doesn't match `indices_array` ({}).".format(
                             flip_array.shape, indices_array.shape
                         )
                     )
@@ -973,17 +939,15 @@
                 "name": name,
                 # Brightway specific
                 "valid_for": valid_for,
             }
         )
         self.resources.append(kwargs)
 
-    def add_json_metadata(
-        self, *, data: Any, valid_for: str, name: str = None, **kwargs
-    ) -> None:
+    def add_json_metadata(self, *, data: Any, valid_for: str, name: str = None, **kwargs) -> None:
         """Add an iterable metadata object to be stored as a JSON file.
 
         The purpose of storing metadata is to enable data exchange; therefore, this method assumes that data is written to disk.
 
         The normal use case of this method is to provide names and other metadata for parameters whose values are stored as presamples arrays. The length of ``data`` should match the number of rows in the corresponding presamples array, and ``data`` is just a list of string labels for the parameters. However, this method can also be used to store other metadata, e.g. for external data resources.
 
         In contrast to ``self.create_structured_array``, this always stores the dataframe in ``self.data``; no proxies are used.
@@ -1011,17 +975,15 @@
         self._prepare_modifications()
 
         name = name or uuid.uuid4().hex
         check_name(name)
 
         filename = check_suffix(name, ".json")
 
-        file_writer(
-            data=data, fs=self.fs, resource=filename, mimetype="application/json"
-        )
+        file_writer(data=data, fs=self.fs, resource=filename, mimetype="application/json")
         self.data.append(data)
 
         kwargs.update(
             {
                 # Datapackage generic
                 "profile": "data-resource",
                 "mediatype": "application/json",
@@ -1031,35 +993,35 @@
                 "valid_for": valid_for,
             }
         )
         self.resources.append(kwargs)
 
 
 def create_datapackage(
-    fs: Optional[FS] = None,
+    fs: Optional[AbstractFileSystem] = None,
     name: Optional[str] = None,
     id_: Optional[str] = None,
     metadata: Optional[dict] = None,
     combinatorial: bool = False,
     sequential: bool = False,
     seed: Optional[int] = None,
     sum_intra_duplicates: bool = True,
     sum_inter_duplicates: bool = False,
     matrix_serialize_format_type: MatrixSerializeFormat = MatrixSerializeFormat.NUMPY,
 ) -> Datapackage:
     """Create a new data package.
 
-    All arguments are optional; if a `PyFilesystem2 <https://docs.pyfilesystem.org/en/latest/>`__ filesystem is not provided, a `MemoryFS <https://docs.pyfilesystem.org/en/latest/reference/memoryfs.html>`__ will be used.
+    All arguments are optional; if a `fsspec <https://filesystem-spec.readthedocs.io/en/latest/>`__ filesystem is not provided, an in-memory `DictFS <https://github.com/iterative/morefs?tab=readme-ov-file#dictfs>`__ will be used.
 
     All metadata elements should follow the `datapackage specification <https://frictionlessdata.io/specs/data-package/>`__.
 
     Licenses are specified as a list in ``metadata``. The default license is the `Open Data Commons Public Domain Dedication and License v1.0 <http://opendatacommons.org/licenses/pddl/>`__.
 
     Args:
-        * fs: A ``Filesystem``, optional. A new ``MemoryFS`` is used if not provided.
+        * fs: A ``Filesystem``, optional. A new ``DictFS`` is used if not provided.
         * name: ``str``, optional. A new uuid is used if not provided.
         * `id_`: ``str``, optional. A new uuid is used if not provided.
         * metadata: ``dict``, optional. Metadata dictionary following datapackage specification; see above.
         * combinatorial: ``bool``, default ``False`` .: Policy on how to sample columns across multiple data arrays; see readme.
         * sequential: ``bool``, default ``False`` .: Policy on how to sample columns in data arrays; see readme.
         * seed: ``int``, optional. Seed to use in random number generator.
         * sum_intra_duplicates: ``bool``, default ``True``. Should duplicate elements in a single data resource be summed together, or should the last value replace previous values.
@@ -1084,15 +1046,15 @@
         sum_inter_duplicates=sum_inter_duplicates,
         matrix_serialize_format_type=matrix_serialize_format_type,
     )
     return obj
 
 
 def load_datapackage(
-    fs_or_obj: Union[DatapackageBase, FS],
+    fs_or_obj: Union[DatapackageBase, AbstractFileSystem],
     mmap_mode: Optional[str] = None,
     proxy: bool = False,
 ) -> Datapackage:
     """Load an existing datapackage.
 
     Can load proxies to data instead of the data itself, which can be useful when interacting with large arrays or large packages where only a subset of the data will be accessed.
 
@@ -1113,15 +1075,15 @@
         obj = fs_or_obj
     else:
         obj = Datapackage()
         obj._load(fs=fs_or_obj, mmap_mode=mmap_mode, proxy=proxy)
     return obj
 
 
-def simple_graph(data: dict, fs: Optional[FS] = None, **metadata) -> Datapackage:
+def simple_graph(data: dict, fs: Optional[AbstractFileSystem] = None, **metadata) -> Datapackage:
     """Easy creation of simple datapackages with only persistent vectors.
 
     Args:
         * data: is a dictionary.
             The data dictionary has the form::
 
                 {
@@ -1136,21 +1098,19 @@
         * fs: is a filesystem.
         * metadata: are passed as kwargs to ``create_datapackage()``.
 
     Returns:
         the datapackage.
 
     """
-    dp = create_datapackage(fs=fs, **metadata)
+    dp = create_datapackage(fs=fs or DictFS(), **metadata)
     for key, value in data.items():
         indices_array = np.array([row[:2] for row in value], dtype=INDICES_DTYPE)
         data_array = np.array([row[2] for row in value])
-        flip_array = np.array(
-            [row[3] if len(row) > 3 else False for row in value], dtype=bool
-        )
+        flip_array = np.array([row[3] if len(row) > 3 else False for row in value], dtype=bool)
         dp.add_persistent_vector(
             matrix=key,
             data_array=data_array,
             name=f"{key}-data",
             indices_array=indices_array,
             nrows=len(value),
             flip_array=flip_array,
```

### Comparing `bw_processing-0.9.3/bw_processing/errors.py` & `bw_processing-0.9.5/bw_processing/errors.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/bw_processing/examples/interfaces.py` & `bw_processing-0.9.5/bw_processing/examples/interfaces.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/bw_processing/examples/parquet_files.py` & `bw_processing-0.9.5/bw_processing/examples/parquet_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 """
 A basic example on how to use parquet files.
 """
 from pathlib import Path
 
 import numpy as np
-from fs.osfs import OSFS
-from fs.zipfs import ZipFS
+from fsspec.implementations.zip import ZipFileSystem
 
 import bw_processing as bwp
+from bw_processing.io_helpers import generic_directory_filesystem
 
 if __name__ == "__main__":
     print("This is a basic example on how to use parquet files.")
     print("Trying to construct a basic datapackage...")
     indices_array = np.array([(0, 1), (1, 0), (1, 1)], dtype=bwp.INDICES_DTYPE)
     data_array = np.array([1, 2, 3])
     flip_array = np.array([True, False, False])
@@ -26,21 +26,21 @@
         bwp.MatrixSerializeFormat.NUMPY
     )  # bwp.MatrixSerializeFormat.PARQUET
 
     if USE_OSFS:
         # VERSION OSFS
         # Directory must exist for OSFS otherwise use OSFS(dirpath, create=True)!
         # Every created object will be saved in that same directory
-        dp_dir = OSFS(str(dirpath / "datapackage_1"), create=True)
+        dp_dir = generic_directory_filesystem(dirpath=dirpath / "datapackage_1", create=True)
         dp = bwp.create_datapackage(
             fs=dp_dir, matrix_serialize_format_type=bwp.MatrixSerializeFormat.NUMPY
         )
     else:
         # VERSION ZIP
-        dp_zip_file = ZipFS(str(dirpath / "datapackage_2.zip"), write=True)
+        dp_zip_file = ZipFileSystem(str(dirpath / "datapackage_2.zip"), mode="w")
         dp = bwp.create_datapackage(
             fs=dp_zip_file, matrix_serialize_format_type=bwp.MatrixSerializeFormat.NUMPY
         )  # bwp.create_datapackage(fs=dp_zip_file, serialize_type=SerializeENum.parquet)
 
     # Add some data to the Datapackage
     # We ask to serialize/save in parquet format specifically
     # Note that you can save some data in numpy format and other data in paquet format for the same Datapackage object
@@ -94,16 +94,16 @@
     dp.finalize_serialization()
     print("Done!")
     print("=" * 80)
     print("Trying to load datapackage back...")
     # OSFS must be open! (and it was closed with finalize_serialization())
 
     if USE_OSFS:
-        dp_dir = OSFS(str(dirpath / "datapackage_1"))
+        dp_dir = generic_directory_filesystem(dirpath=dirpath / "datapackage_1")
         dp2 = bwp.load_datapackage(fs_or_obj=dp_dir)
     else:
-        dp_zip_file = ZipFS(str(dirpath / "datapackage_2.zip"))
+        dp_zip_file = ZipFileSystem(dirpath / "datapackage_2.zip")
         dp2 = bwp.load_datapackage(fs_or_obj=dp_zip_file)
 
     print("Done!")
     print("Print Datapackage resources:")
     print(dp2.resources)
```

### Comparing `bw_processing-0.9.3/bw_processing/examples/simple.zip` & `bw_processing-0.9.5/bw_processing/examples/simple.zip`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/bw_processing/filesystem.py` & `bw_processing-0.9.5/bw_processing/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 def clean_datapackage_name(name: str) -> str:
     """Clean string ``name`` of characters not allowed in data package names.
 
     Replaces with underscores, and drops multiple underscores."""
     return re.sub(MULTI_RE, "_", re.sub(SUBSTITUTION_RE, "_", name).strip("_")).strip()
 
 
-def safe_filename(
-    string: Union[str, bytes], add_hash: bool = True, full: bool = False
-) -> str:
+def safe_filename(string: Union[str, bytes], add_hash: bool = True, full: bool = False) -> str:
     """Convert arbitrary strings to make them safe for filenames. Substitutes strange characters, and uses unicode normalization.
 
     if `add_hash`, appends hash of `string` to avoid name collisions.
 
     From http://stackoverflow.com/questions/295135/turn-a-string-into-a-valid-filename-in-python
     """
     safe = re.sub(
```

### Comparing `bw_processing-0.9.3/bw_processing/indexing.py` & `bw_processing-0.9.5/bw_processing/indexing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from collections.abc import Iterable
 from typing import List, Union
 
 import numpy as np
 import pandas as pd
-from fs.base import FS
+from fsspec import AbstractFileSystem
 
 from .datapackage import Datapackage, load_datapackage
 from .errors import NonUnique
 
 
 def _get_csv_data(
-    datapackage: Union[Datapackage, FS], metadata_name: str
+    datapackage: Union[Datapackage, AbstractFileSystem], metadata_name: str
 ) -> (Datapackage, pd.DataFrame, dict, List[np.ndarray], List[int]):
     """Utility function to get CSV data from datapackage.
 
     Args:
 
         * datapackage: datapackage or `Filesystem`. Input to `load_datapackage` function.
         * metadata_name: Name identifying a CSV metadata resource in ``datapackage``
@@ -36,22 +36,23 @@
     """
 
     dp = load_datapackage(datapackage)
     df, metadata = dp.get_resource(metadata_name)
     if not isinstance(df, pd.DataFrame):
         raise ValueError("Given metadata is not a CSV file")
     resources = [
-        dp.get_resource(key + ".indices")[0][label]
-        for key, label in metadata["valid_for"]
+        dp.get_resource(key + ".indices")[0][label] for key, label in metadata["valid_for"]
     ]
     indices = [dp._get_index(key + ".indices") for key, _ in metadata["valid_for"]]
     return dp, df, metadata, resources, indices
 
 
-def reset_index(datapackage: Union[Datapackage, FS], metadata_name: str) -> Datapackage:
+def reset_index(
+    datapackage: Union[Datapackage, AbstractFileSystem], metadata_name: str
+) -> Datapackage:
     """Reset the numerical indices in ``datapackage`` to sequential integers starting from zero.
 
     Updates the datapackage in place.
 
     Args:
 
         * datapackage: datapackage or `Filesystem`. Input to `load_datapackage` function.
@@ -75,15 +76,15 @@
 
     dp._modified.update(indices)
 
     return dp
 
 
 def reindex(
-    datapackage: Union[Datapackage, FS],
+    datapackage: Union[Datapackage, AbstractFileSystem],
     metadata_name: str,
     data_iterable: Iterable,
     fields: List[str] = None,
     id_field_datapackage: str = "id",
     id_field_destination: str = "id",
 ) -> None:
     """Use the metadata to set the integer indices in ``datapackage`` to those used in ``data_iterable``.
```

### Comparing `bw_processing-0.9.3/bw_processing/io_helpers.py` & `bw_processing-0.9.5/bw_processing/io_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import json
 from mimetypes import guess_type
 from pathlib import Path
 from typing import Any, Optional, Union
 
 import numpy as np
 import pandas as pd
-from fs.base import FS
-from fs.osfs import OSFS
-from fs.zipfs import ZipFS
+from fsspec import AbstractFileSystem
+from fsspec.implementations.dirfs import DirFileSystem
+from fsspec.implementations.local import LocalFileSystem
+from fsspec.implementations.zip import ZipFileSystem
+from morefs.dict import DictFS
 
 from .constants import MatrixSerializeFormat
 from .errors import InvalidMimetype
 from .proxies import Proxy
 
 try:
     from .io_parquet_helpers import load_ndarray_from_parquet, save_arr_to_parquet
@@ -19,37 +21,35 @@
     PARQUET = True
 except ImportError:
     load_ndarray_from_parquet = None
     save_arr_to_parquet = None
     PARQUET = False
 
 
-def generic_directory_filesystem(*, dirpath: Path) -> OSFS:
+def generic_directory_filesystem(*, dirpath: Path) -> DirFileSystem:
     assert isinstance(dirpath, Path), "`dirpath` must be a `pathlib.Path` instance"
     if not dirpath.is_dir():
         if not dirpath.parent.is_dir():
-            raise ValueError(
-                "Parent directory `{}` doesn't exist".format(dirpath.parent)
-            )
+            raise ValueError("Parent directory `{}` doesn't exist".format(dirpath.parent))
         dirpath.mkdir()
-    return OSFS(dirpath)
+    return DirFileSystem(path=dirpath, fs=LocalFileSystem())
 
 
 def generic_zipfile_filesystem(
     *, dirpath: Path, filename: str, write: bool = True
-) -> ZipFS:
+) -> ZipFileSystem:
     assert isinstance(dirpath, Path), "`dirpath` must be a `pathlib.Path` instance"
     if not dirpath.is_dir():
         raise ValueError("Destination directory `{}` doesn't exist".format(dirpath))
-    return ZipFS(dirpath / filename, write=write)
+    return ZipFileSystem(dirpath / filename, mode="w" if write else "r")
 
 
 def file_reader(
     *,
-    fs: FS,
+    fs: AbstractFileSystem,
     resource: str,
     mimetype: str,
     proxy: bool = False,
     mmap_mode: Union[str, None] = None,
     **kwargs,
 ) -> Any:
     if resource.endswith(".npy"):  # TODO: constant
@@ -112,28 +112,29 @@
     else:
         return func(**kwargs)
 
 
 def file_writer(
     *,
     data: Any,
-    fs: FS,
+    fs: AbstractFileSystem,
     resource: str,
     mimetype: str,
     matrix_serialize_format_type: MatrixSerializeFormat = MatrixSerializeFormat.NUMPY,  # NIKO
     meta_object: Optional[str] = None,
     meta_type: Optional[str] = None,
     **kwargs,
 ) -> None:
     if isinstance(resource, Path):
         resource = str(resource)
 
     if mimetype == "application/octet-stream":
         if matrix_serialize_format_type == MatrixSerializeFormat.NUMPY:
-            return np.save(fs.open(resource, mode="wb"), data, allow_pickle=False)
+            with fs.open(resource, mode="wb") as fo:
+                return np.save(fo, data, allow_pickle=False)
         elif matrix_serialize_format_type == MatrixSerializeFormat.PARQUET:
             if not PARQUET:
                 raise ImportError("`pyarrow` library not installed")
             assert meta_type is not None
             assert meta_object is not None
 
             return save_arr_to_parquet(
```

### Comparing `bw_processing-0.9.3/bw_processing/io_parquet_helpers.py` & `bw_processing-0.9.5/bw_processing/io_parquet_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 This module contains some helpers to serialize/deserialize `numpy.ndarray` objects to/from Apache `parquet` files.
 We convert the `nympy.ndarray` objects to `pyarrow.Table` objects to do so.
 """
 import contextlib
 import os
 
 # for annotation
-from io import BufferedWriter, RawIOBase
+from io import BufferedWriter, IOBase, RawIOBase
 
 import numpy
 import numpy as np
 import pyarrow.parquet as pq
-from fs.iotools import RawWrapper
 
-from bw_processing.errors import WrongDatatype
-from bw_processing.io_pyarrow_helpers import (
+from .errors import WrongDatatype
+from .io_pyarrow_helpers import (
     numpy_distributions_vector_to_pyarrow_distributions_vector_table,
     numpy_generic_matrix_to_pyarrow_generic_matrix_table,
     numpy_generic_vector_to_pyarrow_generic_vector_table,
     numpy_indices_vector_to_pyarrow_indices_vector_table,
     pyarrow_distributions_vector_table_to_numpy_distributions_vector,
     pyarrow_generic_matrix_table_to_numpy_generic_matrix,
     pyarrow_generic_vector_table_to_numpy_generic_vector,
@@ -45,73 +44,65 @@
         table = numpy_generic_matrix_to_pyarrow_generic_matrix_table(arr=arr)
     elif meta_object == "vector":
         if meta_type == "indices":
             table = numpy_indices_vector_to_pyarrow_indices_vector_table(arr=arr)
         elif meta_type == "generic":
             table = numpy_generic_vector_to_pyarrow_generic_vector_table(arr=arr)
         elif meta_type == "distributions":
-            table = numpy_distributions_vector_to_pyarrow_distributions_vector_table(
-                arr=arr
-            )
+            table = numpy_distributions_vector_to_pyarrow_distributions_vector_table(arr=arr)
         else:
             raise NotImplementedError(f"Vector of type {meta_type} is not recognized!")
     else:
         raise NotImplementedError(f"Object {meta_object} is not recognized!")
 
     # Save it:
     pq.write_table(table, file)
 
 
-def read_parquet_file_to_ndarray(file: RawWrapper) -> numpy.ndarray:
+def read_parquet_file_to_ndarray(file: RawIOBase) -> numpy.ndarray:
     """
     Read an `ndarray` from a `parquet` file.
 
     Args:
-        file (fs.iotools.RawWrapper): File to read from.
+        file (io.RawIOBase or fsspec file object): File to read from.
 
     Raises:
         `WrongDatatype` if the correct metadata is not found in the `parquet` file.
 
     Returns:
         The corresponding `numpy` `ndarray`.
     """
     table = pq.read_table(file)
 
     # reading metadata from parquet file
     try:
         binary_meta_object = table.schema.metadata[b"object"]
         binary_meta_type = table.schema.metadata[b"type"]
     except KeyError:
-        raise WrongDatatype(
-            f"Parquet file {file} does not contain the right metadata format!"
-        )
+        raise WrongDatatype(f"Parquet file {file} does not contain the right metadata format!")
 
     arr = None
     if binary_meta_object == b"matrix":
         arr = pyarrow_generic_matrix_table_to_numpy_generic_matrix(table=table)
     elif binary_meta_object == b"vector":
         if binary_meta_type == b"indices":
             arr = pyarrow_indices_vector_table_to_numpy_indices_vector(table=table)
         elif binary_meta_type == b"generic":
             arr = pyarrow_generic_vector_table_to_numpy_generic_vector(table=table)
         elif binary_meta_type == b"distributions":
-            arr = pyarrow_distributions_vector_table_to_numpy_distributions_vector(
-                table=table
-            )
+            arr = pyarrow_distributions_vector_table_to_numpy_distributions_vector(table=table)
         else:
             raise NotImplementedError("Vector type not recognized")
     else:
         raise NotImplementedError("Metadata object not recognized")
 
     return arr
 
 
-def save_arr_to_parquet(
-    file: RawIOBase, arr: np.ndarray, meta_object: str, meta_type: str
-) -> None:
+def save_arr_to_parquet(file: RawIOBase, arr: np.ndarray, meta_object: str, meta_type: str) -> None:
     """
     Serialize a `numpy` `ndarray` to a `parquet` `file`.
 
     Parameters
         file (RawIOBase): The file to save to.
         arr (ndarray): The array object to save.
         meta_object (str): "vector" or "matrix".
@@ -123,25 +114,23 @@
         file = os.fspath(file)
         if not file.endswith(".parquet"):
             file = file + ".parquet"
         file_ctx = open(file, "wb")
 
     with file_ctx as fid:
         arr = np.asanyarray(arr)
-        write_ndarray_to_parquet_file(
-            fid, arr, meta_object=meta_object, meta_type=meta_type
-        )
+        write_ndarray_to_parquet_file(fid, arr, meta_object=meta_object, meta_type=meta_type)
 
 
-def load_ndarray_from_parquet(file: RawWrapper) -> np.ndarray:
+def load_ndarray_from_parquet(file: RawIOBase) -> np.ndarray:
     """
     Deserialize a `numpy` `ndarray` from a `parquet` `file`.
 
     Parameters
-        file (fs.iotools.RawWrapper): File to read from.
+        file (io.RawIOBase or fsspec file object): File to read from.
 
     Returns
         The corresponding `numpy` `ndarray`.
     """
     if hasattr(file, "read"):
         file_ctx = contextlib.nullcontext(file)
     else:
```

### Comparing `bw_processing-0.9.3/bw_processing/io_pyarrow_helpers.py` & `bw_processing-0.9.5/bw_processing/io_pyarrow_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,17 +156,15 @@
     for i in range(NBR_UNCERTAINTY_FIELDS)
 ]
 
 UNCERTAINTY_SCHEMA = pa.schema(
     PA_UNCERTAINTY_FIELDS, metadata={"object": "vector", "type": "distributions"}
 )
 
-UNCERTAINTY_FIELDS_NAMES = [
-    UNCERTAINTY_DTYPE[i][0] for i in range(NBR_UNCERTAINTY_FIELDS)
-]
+UNCERTAINTY_FIELDS_NAMES = [UNCERTAINTY_DTYPE[i][0] for i in range(NBR_UNCERTAINTY_FIELDS)]
 
 
 def numpy_distributions_vector_to_pyarrow_distributions_vector_table(
     arr: np.ndarray,
 ) -> pa.Table:
     """
     Convert a specific distributions (numpy) vector to a (arrow) table.
@@ -220,17 +218,15 @@
 
     distributions_arrays_list = [
         table[UNCERTAINTY_FIELDS_NAMES[i]] for i in range(NBR_UNCERTAINTY_FIELDS)
     ]
 
     distributions_array = []
     for el in zip(*distributions_arrays_list):
-        distributions_array.append(
-            tuple(el[i].as_py() for i in range(NBR_UNCERTAINTY_FIELDS))
-        )
+        distributions_array.append(tuple(el[i].as_py() for i in range(NBR_UNCERTAINTY_FIELDS)))
     arr = np.array(distributions_array, dtype=UNCERTAINTY_DTYPE)
 
     return arr
 
 
 ############
 # MATRICES #
@@ -250,18 +246,15 @@
     """
     assert isinstance(arr, np.ndarray)
     assert arr.ndim == 2
 
     arr_dtype = arr.dtype
     metadata = {"object": "matrix", "type": "generic"}
     nbr_rows, nbr_cols = arr.shape
-    arrays = [
-        pa.array(arr[:, j], type=pa.from_numpy_dtype(arr_dtype))
-        for j in range(nbr_cols)
-    ]
+    arrays = [pa.array(arr[:, j], type=pa.from_numpy_dtype(arr_dtype)) for j in range(nbr_cols)]
     table = pa.Table.from_arrays(
         arrays=arrays,
         names=[str(j) for j in range(nbr_cols)],  # give names to each column
         metadata=metadata,
     )
 
     return table
```

### Comparing `bw_processing-0.9.3/bw_processing/merging.py` & `bw_processing-0.9.5/bw_processing/merging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import warnings
 from collections.abc import Iterable
 from typing import Any, Optional
 
 import numpy as np
 import pandas as pd
-from fs.base import FS
-from fs.memoryfs import MemoryFS
+from fsspec import AbstractFileSystem
+from morefs.dict import DictFS
 
 from .datapackage import DatapackageBase, create_datapackage
 from .errors import LengthMismatch
 from .io_helpers import file_writer
 
 
 def mask_resource(obj: Any, mask: np.ndarray) -> Any:
@@ -59,16 +59,16 @@
     rest = metadata["name"][: -len(last) - 1]
     for key in {"name", "path", "group"}:
         metadata[key] = metadata[key].replace(rest, rest + suffix)
 
     return metadata
 
 
-def write_data_to_fs(resource: dict, data: Any, fs: FS) -> None:
-    if isinstance(fs, MemoryFS):
+def write_data_to_fs(resource: dict, data: Any, fs: AbstractFileSystem) -> None:
+    if isinstance(fs, DictFS):
         return
     file_writer(
         data=data,
         fs=fs,
         resource=resource["path"],
         mimetype=resource["mediatype"],
     )
@@ -76,15 +76,15 @@
 
 def merge_datapackages_with_mask(
     first_dp: DatapackageBase,
     first_resource_group_label: str,
     second_dp: DatapackageBase,
     second_resource_group_label: str,
     mask_array: np.ndarray,
-    output_fs: Optional[FS] = None,
+    output_fs: Optional[AbstractFileSystem] = None,
     metadata: Optional[dict] = None,
 ) -> DatapackageBase:
     """Merge two resources using a Numpy boolean mask. Returns elements from ``first_dp`` where the mask is ``True``, otherwise ``second_dp``.
 
     Both resource arrays, and the filter mask, must have the same length.
 
     Both datapackages must be static, i.e. not interfaces. This is because we don't yet have the functionality to select only some of the values in a resource group in ``matrix_utils``.
@@ -104,43 +104,35 @@
     Returns:
 
         A `Datapackage` instance. Will write the resulting datapackage to ``output_fs`` if provided.
 
     """
     if first_resource_group_label == second_resource_group_label:
         add_suffix = True
-        warnings.warn(
-            "Adding suffixes '_true' and '_false' as resource group labels are identical"
-        )
+        warnings.warn("Adding suffixes '_true' and '_false' as resource group labels are identical")
     else:
         add_suffix = False
 
     try:
         first_dp = first_dp.groups[first_resource_group_label]
     except KeyError:
-        raise ValueError(
-            f"Resource group not {first_resource_group_label} not in ``first_dp``"
-        )
+        raise ValueError(f"Resource group not {first_resource_group_label} not in ``first_dp``")
     try:
         second_dp = second_dp.groups[second_resource_group_label]
     except KeyError:
-        raise ValueError(
-            f"Resource group not {second_resource_group_label} not in ``second_dp``"
-        )
+        raise ValueError(f"Resource group not {second_resource_group_label} not in ``second_dp``")
 
     DIMENSION_ERROR = """Dimension mismatch. All array lengths must be the same, but got:\n\tFirst DP: {}\n\tSecond DP: {}\n\t Mask array: {}"""
     if not (len(first_dp.data[0]) == len(first_dp.data[0]) == len(mask_array)):
         raise LengthMismatch(
-            DIMENSION_ERROR.format(
-                len(first_dp.data[0]), len(first_dp.data[0]), len(mask_array)
-            )
+            DIMENSION_ERROR.format(len(first_dp.data[0]), len(first_dp.data[0]), len(mask_array))
         )
 
     if output_fs is None:
-        output_fs = MemoryFS()
+        output_fs = DictFS()
 
     if any(resource["profile"] == "interface" for resource in first_dp.resources):
         raise ValueError("Unsupported interface found in ``first_dp``")
     if any(resource["profile"] == "interface" for resource in second_dp.resources):
         raise ValueError("Unsupported interface found in ``second_dp``")
 
     if metadata is None:
```

### Comparing `bw_processing-0.9.3/bw_processing/unique_fields.py` & `bw_processing-0.9.5/bw_processing/unique_fields.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/bw_processing/utils.py` & `bw_processing-0.9.5/bw_processing/utils.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/bw_processing.egg-info/PKG-INFO` & `bw_processing-0.9.5/bw_processing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 Metadata-Version: 2.1
-Name: bw-processing
-Version: 0.9.3
-Summary: Tools to create structured arrays in a common format
-Home-page: https://github.com/brightway-lca/bw_processing
-Author: Chris Mutel
-Author-email: <cmutel@gmail.com>
-Maintainer: Chris Mutel
-Maintainer-email: <cmutel@gmail.com>
-License: BSD-3-Clause
+Name: bw_processing
+Version: 0.9.5
+Summary: Foo
+Author-email: Chris Mutel <cmutel@gmail.com>
+Maintainer-email: Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/brightway-lca/bw_processing
 Project-URL: homepage, https://github.com/brightway-lca/bw_processing
 Project-URL: tracker, https://github.com/brightway-lca/bw_processing/issues
-Keywords: "brightway","development"
-Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fs
+Requires-Dist: fsspec
+Requires-Dist: morefs
 Requires-Dist: numpy
 Requires-Dist: pandas
 Provides-Extra: testing
-Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: bw_processing; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pyarrow; extra == "testing"
+Requires-Dist: python-coveralls; extra == "testing"
 Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
-Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: myst_parser; extra == "docs"
-Requires-Dist: furo; extra == "docs"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-randomly; extra == "dev"
+Requires-Dist: setuptools; extra == "dev"
 
 # bw-processing
 
 Library for storing numeric data for use in matrix-based calculations. Designed for use with the [Brightway life cycle assessment framework](https://brightway.dev/).
 
 [![PyPI](https://img.shields.io/pypi/v/bw-processing.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/bw-processing.svg)][pypi status]
@@ -144,41 +143,41 @@
 ```
 
 #### Interface dehydrating and rehydrating
 
 Serialized datapackages cannot contain executable code, both because of our chosen data formats, and for security reasons. Therefore, when loading a datapackage with an interface, that interface object needs to be reconstituted as Python code - we call this cycle dehydration and rehydration. Dehydration happens automatically when a datapackage is finalized with `finalize_serialization()`, but rehydration needs to be done manually using `rehydrate_interface()`. For example:
 
 ```python
-from fs.zipfs import ZipFS
+from fsspec.implementations.zip import ZipFileSystem
 from bw_processing import load_datapackage
 
-my_dp = load_datapackage(ZipFS("some-path.zip"))
+my_dp = load_datapackage(ZipFileSystem("some-path.zip"))
 my_dp.rehydrate_interface("some-resource-name", ExampleVectorInterface())
 ```
 
 You can list the dehydrated interfaces present with `.dehydrated_interfaces()`.
 
 You can store useful information for the interface object initialization under the resource key `config`. This can be used in instantiating an interface if you pass `initialize_with_config`:
 
 ```python
-from fs.zipfs import ZipFS
+from fsspec.implementations.zip import ZipFileSystem
 from bw_processing import load_datapackage
 import requests
 import numpy as np
 
 
 class MyInterface:
     def __init__(self, url):
         self.url = url
 
     def __next__(self):
         return np.array(requests.get(self.url).json())
 
 
-my_dp = load_datapackage(ZipFS("some-path.zip"))
+my_dp = load_datapackage(ZipFileSystem("some-path.zip"))
 data_obj, resource_metadata = my_dp.get_resource("some-interface")
 print(resource_metadata['config'])
 >>> {"url": "example.com"}
 
 my_dp.rehydrate_interface("some-interface", MyInterface, initialize_with_config=True)
 # interface is substituted, need to retrieve it again
 data_obj, resource_metadata = my_dp.get_resource("some-interface")
```

### Comparing `bw_processing-0.9.3/bw_processing.egg-info/SOURCES.txt` & `bw_processing-0.9.5/bw_processing.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 ./bw_processing/__init__.py
 ./bw_processing/array_creation.py
 ./bw_processing/constants.py
 ./bw_processing/datapackage.py
 ./bw_processing/errors.py
 ./bw_processing/filesystem.py
 ./bw_processing/indexing.py
@@ -25,15 +24,42 @@
 ./dev/processed_package.py
 ./dev/resources.py
 ./dev/speed_tests.py
 ./docs/conf.py
 ./tests/fixtures/basic_arrays.py
 ./tests/helpers/__init__.py
 ./tests/helpers/basic_array_helpers.py
+bw_processing/__init__.py
+bw_processing/array_creation.py
+bw_processing/constants.py
+bw_processing/datapackage.py
+bw_processing/errors.py
+bw_processing/filesystem.py
+bw_processing/indexing.py
+bw_processing/io_helpers.py
+bw_processing/io_parquet_helpers.py
+bw_processing/io_pyarrow_helpers.py
+bw_processing/merging.py
+bw_processing/proxies.py
+bw_processing/unique_fields.py
+bw_processing/utils.py
 bw_processing.egg-info/PKG-INFO
 bw_processing.egg-info/SOURCES.txt
 bw_processing.egg-info/dependency_links.txt
-bw_processing.egg-info/not-zip-safe
 bw_processing.egg-info/requires.txt
 bw_processing.egg-info/top_level.txt
+bw_processing/examples/__init__.py
+bw_processing/examples/datapackage_2.zip
+bw_processing/examples/interfaces.py
+bw_processing/examples/parquet_files.py
 bw_processing/examples/simple.zip
+bw_processing/examples/__pycache__/__init__.cpython-312.pyc
+bw_processing/examples/datapackage_1/another name.indices.parquet
+bw_processing/examples/datapackage_1/datapackage.json
+bw_processing/examples/datapackage_1/sa-data-vector-from-dict.data.parquet
+bw_processing/examples/datapackage_1/sa-data-vector-from-dict.distributions.parquet
+bw_processing/examples/datapackage_1/sa-data-vector-from-dict.flip.parquet
+bw_processing/examples/datapackage_1/sa-data-vector-from-dict.indices.parquet
+bw_processing/examples/datapackage_1/some name.data.parquet
+bw_processing/examples/datapackage_1/some name.flip.parquet
+bw_processing/examples/datapackage_1/some name.indices.parquet
 tests/test_utils.py
```

### Comparing `bw_processing-0.9.3/dev/calculation_package.py` & `bw_processing-0.9.5/dev/calculation_package.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/dev/loading.py` & `bw_processing-0.9.5/dev/loading.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/dev/processed_package.py` & `bw_processing-0.9.5/dev/processed_package.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/dev/resources.py` & `bw_processing-0.9.5/dev/resources.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/dev/speed_tests.py` & `bw_processing-0.9.5/dev/speed_tests.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/docs/conf.py` & `bw_processing-0.9.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/tests/fixtures/basic_arrays.py` & `bw_processing-0.9.5/tests/fixtures/basic_arrays.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/tests/helpers/basic_array_helpers.py` & `bw_processing-0.9.5/tests/helpers/basic_array_helpers.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.3/tests/test_utils.py` & `bw_processing-0.9.5/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,15 @@
 from pathlib import Path
 
 import numpy as np
 import pytest
 
 from bw_processing import __version__
 from bw_processing.errors import InvalidName
-from bw_processing.utils import (
-    check_name,
-    check_suffix,
-    dictionary_formatter,
-    load_bytes,
-)
+from bw_processing.utils import check_name, check_suffix, dictionary_formatter, load_bytes
 
 
 def test_version():
     assert isinstance(__version__, str)
 
 
 def test_load_bytes():
```

