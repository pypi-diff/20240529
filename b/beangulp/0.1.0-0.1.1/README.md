# Comparing `tmp/beangulp-0.1.0.tar.gz` & `tmp/beangulp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beangulp-0.1.0.tar", last modified: Wed May 29 19:38:15 2024, max compression
+gzip compressed data, was "beangulp-0.1.1.tar", last modified: Wed May 29 19:58:11 2024, max compression
```

## Comparing `beangulp-0.1.0.tar` & `beangulp-0.1.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:38:15.986034 beangulp-0.1.0/
--rw-r--r--   0 daniele    (501) wheel        (0)    18092 2024-05-29 19:37:41.000000 beangulp-0.1.0/LICENSE
--rw-r--r--   0 daniele    (501) wheel        (0)    22837 2024-05-29 19:38:15.984630 beangulp-0.1.0/PKG-INFO
--rw-r--r--   0 daniele    (501) wheel        (0)      887 2024-05-29 19:37:41.000000 beangulp-0.1.0/README.rst
-drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:38:15.917318 beangulp-0.1.0/beangulp/
--rw-r--r--   0 daniele    (501) wheel        (0)     9996 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/__init__.py
--rw-r--r--   0 daniele    (501) wheel        (0)     2461 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/archive.py
--rw-r--r--   0 daniele    (501) wheel        (0)     1962 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/archive_test.py
--rw-r--r--   0 daniele    (501) wheel        (0)     6926 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/cache.py
--rw-r--r--   0 daniele    (501) wheel        (0)     6252 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/cache_test.py
--rw-r--r--   0 daniele    (501) wheel        (0)     5808 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/csv_utils.py
--rw-r--r--   0 daniele    (501) wheel        (0)     7706 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/csv_utils_test.py
--rw-r--r--   0 daniele    (501) wheel        (0)      612 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/date_utils.py
--rw-r--r--   0 daniele    (501) wheel        (0)      228 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/date_utils_test.py
--rw-r--r--   0 daniele    (501) wheel        (0)     1477 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/exceptions.py
--rw-r--r--   0 daniele    (501) wheel        (0)     8376 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/extract.py
--rw-r--r--   0 daniele    (501) wheel        (0)     3850 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/extract_test.py
--rw-r--r--   0 daniele    (501) wheel        (0)     1361 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/file_type.py
--rw-r--r--   0 daniele    (501) wheel        (0)     3306 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/file_type_test.py
-drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:38:15.933552 beangulp-0.1.0/beangulp/file_type_testdata/
--rwxr-xr-x   0 daniele    (501) wheel        (0)      141 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/file_type_testdata/example.py
--rw-r--r--   0 daniele    (501) wheel        (0)     1004 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/identify.py
--rw-r--r--   0 daniele    (501) wheel        (0)     1369 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/identify_test.py
--rw-r--r--   0 daniele    (501) wheel        (0)     7682 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importer.py
--rw-r--r--   0 daniele    (501) wheel        (0)      676 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importer_test.py
-drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:38:15.952511 beangulp-0.1.0/beangulp/importers/
--rw-r--r--   0 daniele    (501) wheel        (0)        0 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importers/__init__.py
--rw-r--r--   0 daniele    (501) wheel        (0)     2798 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importers/config.py
--rw-r--r--   0 daniele    (501) wheel        (0)     1589 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importers/config_test.py
--rw-r--r--   0 daniele    (501) wheel        (0)    20609 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importers/csv.py
--rw-r--r--   0 daniele    (501) wheel        (0)    21362 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importers/csv_test.py
--rw-r--r--   0 daniele    (501) wheel        (0)    11625 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importers/csvbase.py
--rw-r--r--   0 daniele    (501) wheel        (0)    14165 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importers/csvbase_test.py
--rw-r--r--   0 daniele    (501) wheel        (0)      447 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importers/fileonly.py
--rw-r--r--   0 daniele    (501) wheel        (0)     1281 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importers/fileonly_test.py
-drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:38:15.956396 beangulp-0.1.0/beangulp/importers/mixins/
--rw-r--r--   0 daniele    (501) wheel        (0)        0 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importers/mixins/__init__.py
--rw-r--r--   0 daniele    (501) wheel        (0)     1895 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importers/mixins/config.py
--rw-r--r--   0 daniele    (501) wheel        (0)     1487 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importers/mixins/filing.py
--rw-r--r--   0 daniele    (501) wheel        (0)     2227 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/importers/mixins/identifier.py
--rw-r--r--   0 daniele    (501) wheel        (0)      858 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/mimetypes.py
--rw-r--r--   0 daniele    (501) wheel        (0)     4514 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/petl_utils.py
--rw-r--r--   0 daniele    (501) wheel        (0)     1574 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/petl_utils_test.py
--rw-r--r--   0 daniele    (501) wheel        (0)      331 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/scripts_utils.py
--rw-r--r--   0 daniele    (501) wheel        (0)     5452 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/similar.py
--rw-r--r--   0 daniele    (501) wheel        (0)     5711 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/similar_test.py
--rw-r--r--   0 daniele    (501) wheel        (0)     9816 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/testing.py
-drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:38:15.966822 beangulp-0.1.0/beangulp/tests/
--rw-r--r--   0 daniele    (501) wheel        (0)       34 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/tests/__init__.py
--rw-r--r--   0 daniele    (501) wheel        (0)      741 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/tests/doctests_test.py
--rw-r--r--   0 daniele    (501) wheel        (0)     1534 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/tests/utils.py
--rw-r--r--   0 daniele    (501) wheel        (0)     4422 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/utils.py
--rw-r--r--   0 daniele    (501) wheel        (0)     3397 2024-05-29 19:37:41.000000 beangulp-0.1.0/beangulp/utils_test.py
-drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:38:15.982447 beangulp-0.1.0/beangulp.egg-info/
--rw-r--r--   0 daniele    (501) wheel        (0)    22837 2024-05-29 19:38:15.000000 beangulp-0.1.0/beangulp.egg-info/PKG-INFO
--rw-r--r--   0 daniele    (501) wheel        (0)     1638 2024-05-29 19:38:15.000000 beangulp-0.1.0/beangulp.egg-info/SOURCES.txt
--rw-r--r--   0 daniele    (501) wheel        (0)        1 2024-05-29 19:38:15.000000 beangulp-0.1.0/beangulp.egg-info/dependency_links.txt
--rw-r--r--   0 daniele    (501) wheel        (0)      104 2024-05-29 19:38:15.000000 beangulp-0.1.0/beangulp.egg-info/requires.txt
--rw-r--r--   0 daniele    (501) wheel        (0)       33 2024-05-29 19:38:15.000000 beangulp-0.1.0/beangulp.egg-info/top_level.txt
-drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:38:15.968696 beangulp-0.1.0/examples/
--rwxr-xr-x   0 daniele    (501) wheel        (0)     2386 2024-05-29 19:37:41.000000 beangulp-0.1.0/examples/import.py
-drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:38:15.975297 beangulp-0.1.0/examples/importers/
--rw-r--r--   0 daniele    (501) wheel        (0)        0 2024-05-29 19:37:41.000000 beangulp-0.1.0/examples/importers/__init__.py
--rw-r--r--   0 daniele    (501) wheel        (0)     1943 2024-05-29 19:37:41.000000 beangulp-0.1.0/examples/importers/acme.py
--rw-r--r--   0 daniele    (501) wheel        (0)      892 2024-05-29 19:37:41.000000 beangulp-0.1.0/examples/importers/csvbank.py
--rw-r--r--   0 daniele    (501) wheel        (0)    10777 2024-05-29 19:37:41.000000 beangulp-0.1.0/examples/importers/ofx.py
-drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:38:15.979750 beangulp-0.1.0/examples/importers/tests/
--rw-r--r--   0 daniele    (501) wheel        (0)        0 2024-05-29 19:37:41.000000 beangulp-0.1.0/examples/importers/tests/__init__.py
--rw-r--r--   0 daniele    (501) wheel        (0)    17969 2024-05-29 19:37:41.000000 beangulp-0.1.0/examples/importers/tests/test_ofx.py
--rw-r--r--   0 daniele    (501) wheel        (0)     9169 2024-05-29 19:37:41.000000 beangulp-0.1.0/examples/importers/utrade.py
--rw-r--r--   0 daniele    (501) wheel        (0)     1773 2024-05-29 19:37:41.000000 beangulp-0.1.0/pyproject.toml
--rw-r--r--   0 daniele    (501) wheel        (0)       38 2024-05-29 19:38:15.986242 beangulp-0.1.0/setup.cfg
--rw-r--r--   0 daniele    (501) wheel        (0)       37 2024-05-29 19:37:41.000000 beangulp-0.1.0/setup.py
-drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:38:15.981053 beangulp-0.1.0/tools/
--rwxr-xr-x   0 daniele    (501) wheel        (0)     2176 2024-05-29 19:37:41.000000 beangulp-0.1.0/tools/migrate_files.py
+drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:58:11.608833 beangulp-0.1.1/
+-rw-r--r--   0 daniele    (501) wheel        (0)    18092 2024-05-29 19:37:41.000000 beangulp-0.1.1/LICENSE
+-rw-r--r--   0 daniele    (501) wheel        (0)    22937 2024-05-29 19:58:11.607573 beangulp-0.1.1/PKG-INFO
+-rw-r--r--   0 daniele    (501) wheel        (0)      887 2024-05-29 19:37:41.000000 beangulp-0.1.1/README.rst
+drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:58:11.544896 beangulp-0.1.1/beangulp/
+-rw-r--r--   0 daniele    (501) wheel        (0)     9996 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/__init__.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     2461 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/archive.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     1962 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/archive_test.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     6926 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/cache.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     6252 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/cache_test.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     5808 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/csv_utils.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     7706 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/csv_utils_test.py
+-rw-r--r--   0 daniele    (501) wheel        (0)      612 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/date_utils.py
+-rw-r--r--   0 daniele    (501) wheel        (0)      228 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/date_utils_test.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     1477 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/exceptions.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     8376 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/extract.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     3850 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/extract_test.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     1361 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/file_type.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     3306 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/file_type_test.py
+drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:58:11.552400 beangulp-0.1.1/beangulp/file_type_testdata/
+-rwxr-xr-x   0 daniele    (501) wheel        (0)      141 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/file_type_testdata/example.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     1004 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/identify.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     1369 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/identify_test.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     7682 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importer.py
+-rw-r--r--   0 daniele    (501) wheel        (0)      676 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importer_test.py
+drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:58:11.574010 beangulp-0.1.1/beangulp/importers/
+-rw-r--r--   0 daniele    (501) wheel        (0)        0 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importers/__init__.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     2798 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importers/config.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     1589 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importers/config_test.py
+-rw-r--r--   0 daniele    (501) wheel        (0)    20609 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importers/csv.py
+-rw-r--r--   0 daniele    (501) wheel        (0)    21362 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importers/csv_test.py
+-rw-r--r--   0 daniele    (501) wheel        (0)    11625 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importers/csvbase.py
+-rw-r--r--   0 daniele    (501) wheel        (0)    14165 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importers/csvbase_test.py
+-rw-r--r--   0 daniele    (501) wheel        (0)      447 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importers/fileonly.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     1281 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importers/fileonly_test.py
+drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:58:11.586130 beangulp-0.1.1/beangulp/importers/mixins/
+-rw-r--r--   0 daniele    (501) wheel        (0)        0 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importers/mixins/__init__.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     1895 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importers/mixins/config.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     1487 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importers/mixins/filing.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     2227 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/importers/mixins/identifier.py
+-rw-r--r--   0 daniele    (501) wheel        (0)      858 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/mimetypes.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     4514 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/petl_utils.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     1574 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/petl_utils_test.py
+-rw-r--r--   0 daniele    (501) wheel        (0)      331 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/scripts_utils.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     5452 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/similar.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     5711 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/similar_test.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     9816 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/testing.py
+drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:58:11.590398 beangulp-0.1.1/beangulp/tests/
+-rw-r--r--   0 daniele    (501) wheel        (0)       34 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/tests/__init__.py
+-rw-r--r--   0 daniele    (501) wheel        (0)      741 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/tests/doctests_test.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     1534 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/tests/utils.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     4422 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/utils.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     3397 2024-05-29 19:37:41.000000 beangulp-0.1.1/beangulp/utils_test.py
+drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:58:11.605996 beangulp-0.1.1/beangulp.egg-info/
+-rw-r--r--   0 daniele    (501) wheel        (0)    22937 2024-05-29 19:58:11.000000 beangulp-0.1.1/beangulp.egg-info/PKG-INFO
+-rw-r--r--   0 daniele    (501) wheel        (0)     1638 2024-05-29 19:58:11.000000 beangulp-0.1.1/beangulp.egg-info/SOURCES.txt
+-rw-r--r--   0 daniele    (501) wheel        (0)        1 2024-05-29 19:58:11.000000 beangulp-0.1.1/beangulp.egg-info/dependency_links.txt
+-rw-r--r--   0 daniele    (501) wheel        (0)      104 2024-05-29 19:58:11.000000 beangulp-0.1.1/beangulp.egg-info/requires.txt
+-rw-r--r--   0 daniele    (501) wheel        (0)       33 2024-05-29 19:58:11.000000 beangulp-0.1.1/beangulp.egg-info/top_level.txt
+drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:58:11.591780 beangulp-0.1.1/examples/
+-rwxr-xr-x   0 daniele    (501) wheel        (0)     2386 2024-05-29 19:37:41.000000 beangulp-0.1.1/examples/import.py
+drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:58:11.600248 beangulp-0.1.1/examples/importers/
+-rw-r--r--   0 daniele    (501) wheel        (0)        0 2024-05-29 19:37:41.000000 beangulp-0.1.1/examples/importers/__init__.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     1943 2024-05-29 19:37:41.000000 beangulp-0.1.1/examples/importers/acme.py
+-rw-r--r--   0 daniele    (501) wheel        (0)      892 2024-05-29 19:37:41.000000 beangulp-0.1.1/examples/importers/csvbank.py
+-rw-r--r--   0 daniele    (501) wheel        (0)    10777 2024-05-29 19:37:41.000000 beangulp-0.1.1/examples/importers/ofx.py
+drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:58:11.602660 beangulp-0.1.1/examples/importers/tests/
+-rw-r--r--   0 daniele    (501) wheel        (0)        0 2024-05-29 19:37:41.000000 beangulp-0.1.1/examples/importers/tests/__init__.py
+-rw-r--r--   0 daniele    (501) wheel        (0)    17969 2024-05-29 19:37:41.000000 beangulp-0.1.1/examples/importers/tests/test_ofx.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     9169 2024-05-29 19:37:41.000000 beangulp-0.1.1/examples/importers/utrade.py
+-rw-r--r--   0 daniele    (501) wheel        (0)     1863 2024-05-29 19:57:50.000000 beangulp-0.1.1/pyproject.toml
+-rw-r--r--   0 daniele    (501) wheel        (0)       38 2024-05-29 19:58:11.608973 beangulp-0.1.1/setup.cfg
+-rw-r--r--   0 daniele    (501) wheel        (0)       37 2024-05-29 19:37:41.000000 beangulp-0.1.1/setup.py
+drwxr-xr-x   0 daniele    (501) wheel        (0)        0 2024-05-29 19:58:11.604728 beangulp-0.1.1/tools/
+-rwxr-xr-x   0 daniele    (501) wheel        (0)     2176 2024-05-29 19:37:41.000000 beangulp-0.1.1/tools/migrate_files.py
```

### Comparing `beangulp-0.1.0/LICENSE` & `beangulp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/PKG-INFO` & `beangulp-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beangulp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Importers Framework for Beancount
 Author-email: Martin Blais <blais@furius.ca>, Daniele Nicolodi <daniele@grinta.net>
 Maintainer-email: Daniele Nicolodi <daniele@grinta.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -340,23 +340,25 @@
         
         This General Public License does not permit incorporating your program into
         proprietary programs.  If your program is a subroutine library, you may
         consider it more useful to permit linking proprietary applications with the
         library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.
         
-Project-URL: homepage, https://github.com/beancount/beanquery
-Project-URL: issues, https://github.com/beancount/beanquery/issues
+Project-URL: homepage, https://github.com/beancount/beangulp
+Project-URL: issues, https://github.com/beancount/beangulp/issues
 Keywords: accounting,ledger,beancount,importer,import,converter,conversion
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Text Processing :: General
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: beancount>=2.3.5
 Requires-Dist: beautifulsoup4
 Requires-Dist: chardet
```

### Comparing `beangulp-0.1.0/README.rst` & `beangulp-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/__init__.py` & `beangulp-0.1.1/beangulp/__init__.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/archive.py` & `beangulp-0.1.1/beangulp/archive.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/archive_test.py` & `beangulp-0.1.1/beangulp/archive_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/cache.py` & `beangulp-0.1.1/beangulp/cache.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/cache_test.py` & `beangulp-0.1.1/beangulp/cache_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/csv_utils.py` & `beangulp-0.1.1/beangulp/csv_utils.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/csv_utils_test.py` & `beangulp-0.1.1/beangulp/csv_utils_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/date_utils.py` & `beangulp-0.1.1/beangulp/date_utils.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/exceptions.py` & `beangulp-0.1.1/beangulp/exceptions.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/extract.py` & `beangulp-0.1.1/beangulp/extract.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/extract_test.py` & `beangulp-0.1.1/beangulp/extract_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/file_type.py` & `beangulp-0.1.1/beangulp/file_type.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/file_type_test.py` & `beangulp-0.1.1/beangulp/file_type_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/identify.py` & `beangulp-0.1.1/beangulp/identify.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/identify_test.py` & `beangulp-0.1.1/beangulp/identify_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/importer.py` & `beangulp-0.1.1/beangulp/importer.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/importer_test.py` & `beangulp-0.1.1/beangulp/importer_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/importers/config.py` & `beangulp-0.1.1/beangulp/importers/config.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/importers/config_test.py` & `beangulp-0.1.1/beangulp/importers/config_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/importers/csv.py` & `beangulp-0.1.1/beangulp/importers/csv.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/importers/csv_test.py` & `beangulp-0.1.1/beangulp/importers/csv_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/importers/csvbase.py` & `beangulp-0.1.1/beangulp/importers/csvbase.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/importers/csvbase_test.py` & `beangulp-0.1.1/beangulp/importers/csvbase_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/importers/fileonly_test.py` & `beangulp-0.1.1/beangulp/importers/fileonly_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/importers/mixins/config.py` & `beangulp-0.1.1/beangulp/importers/mixins/config.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/importers/mixins/filing.py` & `beangulp-0.1.1/beangulp/importers/mixins/filing.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/importers/mixins/identifier.py` & `beangulp-0.1.1/beangulp/importers/mixins/identifier.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/mimetypes.py` & `beangulp-0.1.1/beangulp/mimetypes.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/petl_utils.py` & `beangulp-0.1.1/beangulp/petl_utils.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/petl_utils_test.py` & `beangulp-0.1.1/beangulp/petl_utils_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/similar.py` & `beangulp-0.1.1/beangulp/similar.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/similar_test.py` & `beangulp-0.1.1/beangulp/similar_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/testing.py` & `beangulp-0.1.1/beangulp/testing.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/tests/doctests_test.py` & `beangulp-0.1.1/beangulp/tests/doctests_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/tests/utils.py` & `beangulp-0.1.1/beangulp/tests/utils.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/utils.py` & `beangulp-0.1.1/beangulp/utils.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp/utils_test.py` & `beangulp-0.1.1/beangulp/utils_test.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/beangulp.egg-info/PKG-INFO` & `beangulp-0.1.1/beangulp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beangulp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Importers Framework for Beancount
 Author-email: Martin Blais <blais@furius.ca>, Daniele Nicolodi <daniele@grinta.net>
 Maintainer-email: Daniele Nicolodi <daniele@grinta.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -340,23 +340,25 @@
         
         This General Public License does not permit incorporating your program into
         proprietary programs.  If your program is a subroutine library, you may
         consider it more useful to permit linking proprietary applications with the
         library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.
         
-Project-URL: homepage, https://github.com/beancount/beanquery
-Project-URL: issues, https://github.com/beancount/beanquery/issues
+Project-URL: homepage, https://github.com/beancount/beangulp
+Project-URL: issues, https://github.com/beancount/beangulp/issues
 Keywords: accounting,ledger,beancount,importer,import,converter,conversion
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Text Processing :: General
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: beancount>=2.3.5
 Requires-Dist: beautifulsoup4
 Requires-Dist: chardet
```

### Comparing `beangulp-0.1.0/beangulp.egg-info/SOURCES.txt` & `beangulp-0.1.1/beangulp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/examples/import.py` & `beangulp-0.1.1/examples/import.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/examples/importers/acme.py` & `beangulp-0.1.1/examples/importers/acme.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/examples/importers/csvbank.py` & `beangulp-0.1.1/examples/importers/csvbank.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/examples/importers/ofx.py` & `beangulp-0.1.1/examples/importers/ofx.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/examples/importers/tests/test_ofx.py` & `beangulp-0.1.1/examples/importers/tests/test_ofx.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/examples/importers/utrade.py` & `beangulp-0.1.1/examples/importers/utrade.py`

 * *Files identical despite different names*

### Comparing `beangulp-0.1.0/pyproject.toml` & `beangulp-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools >= 60.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'beangulp'
-version = '0.1.0'
+version = '0.1.1'
 license = { file = 'LICENSE' }
 description = 'Importers Framework for Beancount'
 readme = 'README.rst'
 authors = [
     { name = 'Martin Blais', email = 'blais@furius.ca' },
     { name = 'Daniele Nicolodi', email = 'daniele@grinta.net' },
 ]
@@ -19,29 +19,31 @@
 classifiers = [
     'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Topic :: Office/Business :: Financial :: Accounting',
     'Topic :: Text Processing :: General',
 ]
 dependencies = [
     'beancount >=2.3.5',
     'beautifulsoup4',
     'chardet',
     'click >8.0',
     'lxml',
     'python-magic >=0.4.12; sys_platform != "win32"',
 ]
 
 [project.urls]
-homepage = 'https://github.com/beancount/beanquery'
-issues = 'https://github.com/beancount/beanquery/issues'
+homepage = 'https://github.com/beancount/beangulp'
+issues = 'https://github.com/beancount/beangulp/issues'
 
 [tool.setuptools.packages]
 find = {}
 
 [tool.ruff]
 line-length = 128
 target-version = 'py37'
```

### Comparing `beangulp-0.1.0/tools/migrate_files.py` & `beangulp-0.1.1/tools/migrate_files.py`

 * *Files identical despite different names*

