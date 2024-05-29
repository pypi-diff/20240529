# Comparing `tmp/ensembl_utils-0.1.1.tar.gz` & `tmp/ensembl_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensembl_utils-0.1.1.tar", last modified: Wed May 29 15:36:25 2024, max compression
+gzip compressed data, was "ensembl_utils-0.1.2.tar", last modified: Wed May 29 16:13:00 2024, max compression
```

## Comparing `ensembl_utils-0.1.1.tar` & `ensembl_utils-0.1.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.067272 ensembl_utils-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.055272 ensembl_utils-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.051272 ensembl_utils-0.1.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.055272 ensembl_utils-0.1.1/.github/actions/python_build/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/.github/actions/python_build/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.055272 ensembl_utils-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-29 15:36:25.063272 ensembl_utils-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.055272 ensembl_utils-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/docs/code_of_conduct.md
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/docs/gen_ref_pages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.055272 ensembl_utils-0.1.1/docs/img/
--rw-r--r--   0 runner    (1001) docker     (127)   133459 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/docs/img/ebang.png
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/docs/install.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.059272 ensembl_utils-0.1.1/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:36:25.067272 ensembl_utils-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.051272 ensembl_utils-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.051272 ensembl_utils-0.1.1/src/ensembl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.059272 ensembl_utils-0.1.1/src/ensembl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/src/ensembl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/src/ensembl/utils/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/src/ensembl/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/src/ensembl/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/src/ensembl/utils/rloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.063272 ensembl_utils-0.1.1/src/ensembl_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-29 15:36:25.000000 ensembl_utils-0.1.1/src/ensembl_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-29 15:36:25.000000 ensembl_utils-0.1.1/src/ensembl_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:36:25.000000 ensembl_utils-0.1.1/src/ensembl_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 15:36:25.000000 ensembl_utils-0.1.1/src/ensembl_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-29 15:36:25.000000 ensembl_utils-0.1.1/src/ensembl_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 15:36:25.000000 ensembl_utils-0.1.1/src/ensembl_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.059272 ensembl_utils-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.059272 ensembl_utils-0.1.1/tests/archive/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.059272 ensembl_utils-0.1.1/tests/archive/test_archive/
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/archive/test_archive/sample.tar
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/archive/test_archive/sample.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/archive/test_archive/sample.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/archive/test_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.059272 ensembl_utils-0.1.1/tests/argparse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.059272 ensembl_utils-0.1.1/tests/argparse/test_argparse/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/argparse/test_argparse/sample.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/argparse/test_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.059272 ensembl_utils-0.1.1/tests/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/logging/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.063272 ensembl_utils-0.1.1/tests/rloader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:36:25.063272 ensembl_utils-0.1.1/tests/rloader/test_rloader/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/rloader/test_rloader/sample.env
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/rloader/test_rloader/sample.ini
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/rloader/test_rloader/sample.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/rloader/test_rloader/sample.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/rloader/test_rloader/sample.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-29 15:36:14.000000 ensembl_utils-0.1.1/tests/rloader/test_rloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.067073 ensembl_utils-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.055073 ensembl_utils-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.051073 ensembl_utils-0.1.2/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.055073 ensembl_utils-0.1.2/.github/actions/python_build/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/.github/actions/python_build/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.055073 ensembl_utils-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-29 16:13:00.063073 ensembl_utils-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.055073 ensembl_utils-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/docs/code_of_conduct.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/docs/gen_ref_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   133459 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/docs/img/ebang.png
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/docs/install.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 16:13:00.067073 ensembl_utils-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.055073 ensembl_utils-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.051073 ensembl_utils-0.1.2/src/ensembl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/src/ensembl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/src/ensembl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/src/ensembl/utils/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/src/ensembl/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/src/ensembl/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/src/ensembl/utils/rloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.063073 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-29 16:13:00.000000 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-29 16:13:00.000000 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:13:00.000000 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 16:13:00.000000 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-29 16:13:00.000000 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 16:13:00.000000 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/archive/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/archive/test_archive/
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/archive/test_archive/sample.tar
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/archive/test_archive/sample.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/archive/test_archive/sample.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/archive/test_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/argparse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/argparse/test_argparse/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/argparse/test_argparse/sample.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/argparse/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/logging/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/rloader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.063073 ensembl_utils-0.1.2/tests/rloader/test_rloader/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/rloader/test_rloader/sample.env
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/rloader/test_rloader/sample.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/rloader/test_rloader/sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/rloader/test_rloader/sample.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/rloader/test_rloader/sample.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/rloader/test_rloader.py
```

### Comparing `ensembl_utils-0.1.1/.github/actions/python_build/action.yml` & `ensembl_utils-0.1.2/.github/actions/python_build/action.yml`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/.github/dependabot.yml` & `ensembl_utils-0.1.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/.github/workflows/ci.yml` & `ensembl_utils-0.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/.github/workflows/publish.yml` & `ensembl_utils-0.1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/.gitignore` & `ensembl_utils-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/LICENSE` & `ensembl_utils-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/PKG-INFO` & `ensembl_utils-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: ensembl-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Ensembl Python general-purpose utils
 Author-email: Ensembl <dev@ensembl.org>
 License: Apache License 2.0
 Project-URL: homepage, https://www.ensembl.org
+Project-URL: documentation, https://ensembl.github.io/ensembl-utils/
 Project-URL: repository, https://github.com/Ensembl/ensembl-utils
 Keywords: ensembl,python,utils
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -61,22 +62,22 @@
 
 For more information, please consult this repository's [GitHub pages](https://ensembl.github.io/ensembl-utils/).
 
 ## Getting Started
 
 ### Basic installation
 
-This library is publicly available in [pypi.org](https://pypi.org) so it can be easily installed with your favourite Python dependency and packaging management, e.g.
+This library is publicly available in [PyPI](https://pypi.org/project/ensembl-utils/) so it can be easily installed with your favourite Python dependency and packaging management, e.g.
 ```bash
 pip install ensembl-utils
 ```
 
 ### Installing the development environment (with Python `venv`)
 
 If you want to install this library in editable mode, we suggest you to do so via Python's virtual environment module ([venv](https://docs.python.org/3/library/venv.html)):
 ```bash
 python -m venv <VIRTUAL_ENVIRONMENT_NAME>
 source <VIRTUAL_ENVIRONMENT_NAME>/bin/activate
 git clone https://github.com/Ensembl/ensembl-utils.git
 cd ensembl-utils
-pip install -e .[cicd,dev,doc]
+pip install -e .[cicd,docs]
 ```
```

### Comparing `ensembl_utils-0.1.1/README.md` & `ensembl_utils-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 For more information, please consult this repository's [GitHub pages](https://ensembl.github.io/ensembl-utils/).
 
 ## Getting Started
 
 ### Basic installation
 
-This library is publicly available in [pypi.org](https://pypi.org) so it can be easily installed with your favourite Python dependency and packaging management, e.g.
+This library is publicly available in [PyPI](https://pypi.org/project/ensembl-utils/) so it can be easily installed with your favourite Python dependency and packaging management, e.g.
 ```bash
 pip install ensembl-utils
 ```
 
 ### Installing the development environment (with Python `venv`)
 
 If you want to install this library in editable mode, we suggest you to do so via Python's virtual environment module ([venv](https://docs.python.org/3/library/venv.html)):
 ```bash
 python -m venv <VIRTUAL_ENVIRONMENT_NAME>
 source <VIRTUAL_ENVIRONMENT_NAME>/bin/activate
 git clone https://github.com/Ensembl/ensembl-utils.git
 cd ensembl-utils
-pip install -e .[cicd,dev,doc]
+pip install -e .[cicd,docs]
 ```
```

### Comparing `ensembl_utils-0.1.1/docs/gen_ref_pages.py` & `ensembl_utils-0.1.2/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/docs/img/ebang.png` & `ensembl_utils-0.1.2/docs/img/ebang.png`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/docs/index.md` & `ensembl_utils-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/docs/install.md` & `ensembl_utils-0.1.2/docs/install.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 
 If you want to install this library in editable mode, we suggest you to do so via Python's virtual environment module ([venv](https://docs.python.org/3/library/venv.html)):
 ```bash
 python -m venv <VIRTUAL_ENVIRONMENT_NAME>
 source <VIRTUAL_ENVIRONMENT_NAME>/bin/activate
 git clone https://github.com/Ensembl/ensembl-utils.git
 cd ensembl-utils
-pip install -e .[cicd,doc]
+pip install -e .[cicd,docs]
 ```
 
-Note that the documentation (`doc` tag) is generated using _mkdocs_. For full information visit [mkdocs.org](https://www.mkdocs.org).
+Note that the documentation (`docs` tag) is generated using _mkdocs_. For full information visit [mkdocs.org](https://www.mkdocs.org).
```

### Comparing `ensembl_utils-0.1.1/mkdocs.yml` & `ensembl_utils-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/pyproject.toml` & `ensembl_utils-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     "mkdocs-section-index",
     "mkdocstrings",
     "mkdocstrings-python",
 ]
 
 [project.urls]
 homepage = "https://www.ensembl.org"
+documentation = "https://ensembl.github.io/ensembl-utils/"
 repository = "https://github.com/Ensembl/ensembl-utils"
 
 [project.scripts]
 extract_file = "ensembl.utils.archive:extract_file_cli"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
@@ -153,8 +154,8 @@
     # Do not complain if non-runnable code is not run
     "if __name__ == .__main__.:",
     "if TYPE_CHECKING:",
     "def main",
     "def .*_cli",
     # Do not complain about abstract methods, they are not run
     "@(abc\\.)?abstractmethod",
-]
+]
```

### Comparing `ensembl_utils-0.1.1/setup.py` & `ensembl_utils-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/src/ensembl/utils/__init__.py` & `ensembl_utils-0.1.2/src/ensembl/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Ensembl Python general-purpose utils library."""
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 __all__ = [
     "StrPath",
 ]
 
 import os
 from typing import Union
```

### Comparing `ensembl_utils-0.1.1/src/ensembl/utils/archive.py` & `ensembl_utils-0.1.2/src/ensembl/utils/archive.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/src/ensembl/utils/argparse.py` & `ensembl_utils-0.1.2/src/ensembl/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/src/ensembl/utils/logging.py` & `ensembl_utils-0.1.2/src/ensembl/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/src/ensembl/utils/rloader.py` & `ensembl_utils-0.1.2/src/ensembl/utils/rloader.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/src/ensembl_utils.egg-info/PKG-INFO` & `ensembl_utils-0.1.2/src/ensembl_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: ensembl-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Ensembl Python general-purpose utils
 Author-email: Ensembl <dev@ensembl.org>
 License: Apache License 2.0
 Project-URL: homepage, https://www.ensembl.org
+Project-URL: documentation, https://ensembl.github.io/ensembl-utils/
 Project-URL: repository, https://github.com/Ensembl/ensembl-utils
 Keywords: ensembl,python,utils
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -61,22 +62,22 @@
 
 For more information, please consult this repository's [GitHub pages](https://ensembl.github.io/ensembl-utils/).
 
 ## Getting Started
 
 ### Basic installation
 
-This library is publicly available in [pypi.org](https://pypi.org) so it can be easily installed with your favourite Python dependency and packaging management, e.g.
+This library is publicly available in [PyPI](https://pypi.org/project/ensembl-utils/) so it can be easily installed with your favourite Python dependency and packaging management, e.g.
 ```bash
 pip install ensembl-utils
 ```
 
 ### Installing the development environment (with Python `venv`)
 
 If you want to install this library in editable mode, we suggest you to do so via Python's virtual environment module ([venv](https://docs.python.org/3/library/venv.html)):
 ```bash
 python -m venv <VIRTUAL_ENVIRONMENT_NAME>
 source <VIRTUAL_ENVIRONMENT_NAME>/bin/activate
 git clone https://github.com/Ensembl/ensembl-utils.git
 cd ensembl-utils
-pip install -e .[cicd,dev,doc]
+pip install -e .[cicd,docs]
 ```
```

### Comparing `ensembl_utils-0.1.1/src/ensembl_utils.egg-info/SOURCES.txt` & `ensembl_utils-0.1.2/src/ensembl_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/tests/archive/test_archive/sample.tar` & `ensembl_utils-0.1.2/tests/archive/test_archive/sample.tar`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/tests/archive/test_archive.py` & `ensembl_utils-0.1.2/tests/archive/test_archive.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/tests/argparse/test_argparse.py` & `ensembl_utils-0.1.2/tests/argparse/test_argparse.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/tests/conftest.py` & `ensembl_utils-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/tests/logging/test_logging.py` & `ensembl_utils-0.1.2/tests/logging/test_logging.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.1/tests/rloader/test_rloader.py` & `ensembl_utils-0.1.2/tests/rloader/test_rloader.py`

 * *Files identical despite different names*

