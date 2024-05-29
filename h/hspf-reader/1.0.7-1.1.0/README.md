# Comparing `tmp/hspf_reader-1.0.7.tar.gz` & `tmp/hspf_reader-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspf_reader-1.0.7.tar", last modified: Sun Mar 31 20:07:56 2024, max compression
+gzip compressed data, was "hspf_reader-1.1.0.tar", last modified: Wed May 29 02:22:09 2024, max compression
```

## Comparing `hspf_reader-1.0.7.tar` & `hspf_reader-1.1.0.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-03-31 20:07:56.980650 hspf_reader-1.0.7/
--rw-r--r--   0 tim       (1000) tim       (1000)      102 2024-03-31 20:01:18.000000 hspf_reader-1.0.7/.deepsource.toml
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-03-31 20:07:56.972649 hspf_reader-1.0.7/.github/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-03-31 20:07:56.972649 hspf_reader-1.0.7/.github/workflows/
--rw-r--r--   0 tim       (1000) tim       (1000)      501 2024-03-31 20:01:18.000000 hspf_reader-1.0.7/.github/workflows/clean-workflow-runs.yml
--rw-r--r--   0 tim       (1000) tim       (1000)     2121 2024-03-31 20:01:18.000000 hspf_reader-1.0.7/.github/workflows/python-package.yml
--rw-r--r--   0 tim       (1000) tim       (1000)      335 2023-03-05 18:51:19.000000 hspf_reader-1.0.7/.gitignore
--rw-rw-r--   0 tim       (1000) tim       (1000)     2654 2024-03-31 20:03:04.000000 hspf_reader-1.0.7/.pre-commit-config.yaml
--rw-rw-r--   0 tim       (1000) tim       (1000)     1825 2024-03-31 20:01:18.000000 hspf_reader-1.0.7/.sourcery.yaml
--rw-r--r--   0 tim       (1000) tim       (1000)       50 2022-08-30 21:29:29.000000 hspf_reader-1.0.7/AUTHORS.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1036 2022-09-27 21:47:42.000000 hspf_reader-1.0.7/BADGES.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      992 2024-03-31 20:07:41.000000 hspf_reader-1.0.7/CHANGELOG.md
--rw-r--r--   0 tim       (1000) tim       (1000)     3179 2022-08-30 21:29:29.000000 hspf_reader-1.0.7/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1488 2022-08-30 21:29:29.000000 hspf_reader-1.0.7/LICENSE.txt
--rw-r--r--   0 tim       (1000) tim       (1000)     5279 2024-03-31 20:07:56.980650 hspf_reader-1.0.7/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)     2676 2023-06-10 05:29:49.000000 hspf_reader-1.0.7/README.rst
--rw-r--r--   0 tim       (1000) tim       (1000)        6 2024-03-31 20:07:41.000000 hspf_reader-1.0.7/VERSION
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-03-31 20:07:56.972649 hspf_reader-1.0.7/docs/
--rw-r--r--   0 tim       (1000) tim       (1000)     5712 2022-08-30 21:28:21.000000 hspf_reader-1.0.7/docs/Makefile
--rw-r--r--   0 tim       (1000) tim       (1000)       55 2022-11-05 05:41:26.000000 hspf_reader-1.0.7/docs/authors.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      360 2024-03-31 20:01:18.000000 hspf_reader-1.0.7/docs/command_line.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     9668 2023-01-22 03:38:21.000000 hspf_reader-1.0.7/docs/conf.py
--rw-r--r--   0 tim       (1000) tim       (1000)       60 2022-11-05 05:41:26.000000 hspf_reader-1.0.7/docs/contributing.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      273 2024-03-31 05:49:24.000000 hspf_reader-1.0.7/docs/function_summary.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      466 2022-11-05 05:42:41.000000 hspf_reader-1.0.7/docs/index.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       79 2022-11-05 05:41:26.000000 hspf_reader-1.0.7/docs/license.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     5104 2022-08-30 21:28:21.000000 hspf_reader-1.0.7/docs/make.bat
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2022-11-05 05:41:26.000000 hspf_reader-1.0.7/docs/readme.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      797 2024-03-31 17:19:00.000000 hspf_reader-1.0.7/publish.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2952 2024-03-31 20:07:41.000000 hspf_reader-1.0.7/pyproject.toml
--rw-r--r--   0 tim       (1000) tim       (1000)      261 2022-10-16 16:07:40.000000 hspf_reader-1.0.7/requirements.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2024-03-31 20:07:56.980650 hspf_reader-1.0.7/setup.cfg
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-03-31 20:07:56.972649 hspf_reader-1.0.7/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-03-31 20:07:56.972649 hspf_reader-1.0.7/src/hspf_reader/
--rw-r--r--   0 tim       (1000) tim       (1000)       67 2023-01-22 03:38:21.000000 hspf_reader-1.0.7/src/hspf_reader/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    10175 2023-11-19 06:43:07.000000 hspf_reader-1.0.7/src/hspf_reader/hspf_reader.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-03-31 20:07:56.976649 hspf_reader-1.0.7/src/hspf_reader.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)     5279 2024-03-31 20:07:56.000000 hspf_reader-1.0.7/src/hspf_reader.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     1043 2024-03-31 20:07:56.000000 hspf_reader-1.0.7/src/hspf_reader.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2024-03-31 20:07:56.000000 hspf_reader-1.0.7/src/hspf_reader.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       61 2024-03-31 20:07:56.000000 hspf_reader-1.0.7/src/hspf_reader.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      296 2024-03-31 20:07:56.000000 hspf_reader-1.0.7/src/hspf_reader.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       12 2024-03-31 20:07:56.000000 hspf_reader-1.0.7/src/hspf_reader.egg-info/top_level.txt
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-03-31 20:07:56.976649 hspf_reader-1.0.7/tests/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2023-01-22 03:38:21.000000 hspf_reader-1.0.7/tests/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)      482 2023-01-22 03:38:21.000000 hspf_reader-1.0.7/tests/capture.py
--rw-r--r--   0 tim       (1000) tim       (1000)    81920 2022-08-30 21:28:23.000000 hspf_reader-1.0.7/tests/data.wdm
--rw-r--r--   0 tim       (1000) tim       (1000)   822321 2022-08-30 21:28:23.000000 hspf_reader-1.0.7/tests/data_6b_np1.hbn
--rw-rw-r--   0 tim       (1000) tim       (1000)    62131 2022-08-31 19:57:44.000000 hspf_reader-1.0.7/tests/data_plotgen.plt
--rw-rw-r--   0 tim       (1000) tim       (1000)   172779 2022-09-27 13:00:11.000000 hspf_reader-1.0.7/tests/data_wdm_1.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)   264240 2022-09-27 13:13:16.000000 hspf_reader-1.0.7/tests/data_wdm_2.csv
--rw-r--r--   0 tim       (1000) tim       (1000)   822321 2022-09-21 23:17:47.000000 hspf_reader-1.0.7/tests/data_yearly.hbn
--rw-rw-r--   0 tim       (1000) tim       (1000)        0 2022-08-31 21:31:44.000000 hspf_reader-1.0.7/tests/debug_hspf_reader
--rw-r--r--   0 tim       (1000) tim       (1000)    30250 2022-09-21 23:52:50.000000 hspf_reader-1.0.7/tests/sunspot_area.csv
--rw-r--r--   0 tim       (1000) tim       (1000)    15138 2022-09-21 23:53:58.000000 hspf_reader-1.0.7/tests/sunspot_area_with_missing.csv
--rw-r--r--   0 tim       (1000) tim       (1000)     2496 2023-11-19 06:43:07.000000 hspf_reader-1.0.7/tests/test_hbn.py
--rw-r--r--   0 tim       (1000) tim       (1000)    35501 2023-11-19 06:43:07.000000 hspf_reader-1.0.7/tests/test_plotgen.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1259 2024-03-08 18:16:57.000000 hspf_reader-1.0.7/tests/test_wdm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.978034 hspf_reader-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.966035 hspf_reader-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.966035 hspf_reader-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.github/workflows/clean-workflow-runs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/BADGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-29 02:22:09.978034 hspf_reader-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.966035 hspf_reader-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/function_summary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 02:22:09.978034 hspf_reader-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.962035 hspf_reader-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.970034 hspf_reader-1.1.0/src/hspf_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/src/hspf_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/src/hspf_reader/hspf_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.974034 hspf_reader-1.1.0/src/hspf_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-29 02:22:09.000000 hspf_reader-1.1.0/src/hspf_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-29 02:22:09.000000 hspf_reader-1.1.0/src/hspf_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 02:22:09.000000 hspf_reader-1.1.0/src/hspf_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 02:22:09.000000 hspf_reader-1.1.0/src/hspf_reader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-29 02:22:09.000000 hspf_reader-1.1.0/src/hspf_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 02:22:09.000000 hspf_reader-1.1.0/src/hspf_reader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.974034 hspf_reader-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81920 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/data.wdm
+-rw-r--r--   0 runner    (1001) docker     (127)   822321 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/data_6b_np1.hbn
+-rw-r--r--   0 runner    (1001) docker     (127)    62131 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/data_plotgen.plt
+-rw-r--r--   0 runner    (1001) docker     (127)   172779 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/data_wdm_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   264240 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/data_wdm_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   822321 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/data_yearly.hbn
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/debug_hspf_reader
+-rw-r--r--   0 runner    (1001) docker     (127)    30250 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/sunspot_area.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15138 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/sunspot_area_with_missing.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/test_hbn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35532 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/test_plotgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/test_wdm.py
```

### Comparing `hspf_reader-1.0.7/.pre-commit-config.yaml` & `hspf_reader-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/.sourcery.yaml` & `hspf_reader-1.1.0/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/BADGES.rst` & `hspf_reader-1.1.0/BADGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.. image:: https://github.com/timcera/hspf_reader/actions/workflows/python-package.yml/badge.svg
+.. image:: https://github.com/timcera/hspf_reader/actions/workflows/pypi-package.yml/badge.svg
     :alt: Tests
-    :target: https://github.com/timcera/hspf_reader/actions/workflows/python-package.yml
+    :target: https://github.com/timcera/hspf_reader/actions/workflows/pypi-package.yml
     :height: 20
 
 .. image:: https://img.shields.io/coveralls/github/timcera/hspf_reader
     :alt: Test Coverage
     :target: https://coveralls.io/r/timcera/hspf_reader?branch=master
     :height: 20
```

### Comparing `hspf_reader-1.0.7/CHANGELOG.md` & `hspf_reader-1.1.0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## v1.1.0 (2024-05-28)
+
+### Feat
+
+- include local copy of toolbox_utils using git submodules
+- reworked the about functions
+
+### Fix
+
+- requirements.txt to reduce vulnerabilities
+- requirements.txt to reduce vulnerabilities
+
 ## v1.0.7 (2024-03-31)
 
 ## v1.0.6 (2023-12-16)
 
 ### Refactor
 
 - sourcery refactor
```

### Comparing `hspf_reader-1.0.7/CONTRIBUTING.rst` & `hspf_reader-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/LICENSE.txt` & `hspf_reader-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/PKG-INFO` & `hspf_reader-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspf_reader
-Version: 1.0.7
+Version: 1.1.0
 Summary: Command line script and Python library to read HSPF WDM, binary, and plotgen time series.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/hspf_reader/docs/index.html#hspf_reader-documentation
 Project-URL: github, https://github.com/timcera/hspf_reader
 Project-URL: bitbucket, https://bitbucket.org/timcera/hspf_reader/src/main/
 Keywords: time-series,hspf,simulation,hydrology,hydrologic,python,cli,command line,script,cli-application
@@ -24,18 +24,26 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: cltoolbox<3.0.0,>=2.0.0
-Requires-Dist: typing-extensions
-Requires-Dist: toolbox_utils<6.0.0,>=5.0.0
+Requires-Dist: dateparser
+Requires-Dist: numpy
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: pandas[excel]
+Requires-Dist: pint!=0.21.*
+Requires-Dist: pint<0.22; python_version < "3.9"
+Requires-Dist: pint-pandas
+Requires-Dist: pydantic
+Requires-Dist: scipy
+Requires-Dist: tabulate
+Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: bandit; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: blacken-docs; extra == "dev"
 Requires-Dist: black-nbconvert; extra == "dev"
 Requires-Dist: cleanpy; extra == "dev"
 Requires-Dist: commitizen; extra == "dev"
@@ -54,17 +62,17 @@
 Requires-Dist: pytest-mpl; extra == "dev"
 Requires-Dist: pyupgrade; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: unimport; extra == "dev"
 Requires-Dist: velin; extra == "dev"
 Requires-Dist: vulture; extra == "dev"
 
-.. image:: https://github.com/timcera/hspf_reader/actions/workflows/python-package.yml/badge.svg
+.. image:: https://github.com/timcera/hspf_reader/actions/workflows/pypi-package.yml/badge.svg
     :alt: Tests
-    :target: https://github.com/timcera/hspf_reader/actions/workflows/python-package.yml
+    :target: https://github.com/timcera/hspf_reader/actions/workflows/pypi-package.yml
     :height: 20
 
 .. image:: https://img.shields.io/coveralls/github/timcera/hspf_reader
     :alt: Test Coverage
     :target: https://coveralls.io/r/timcera/hspf_reader?branch=master
     :height: 20
```

### Comparing `hspf_reader-1.0.7/README.rst` & `hspf_reader-1.1.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.. image:: https://github.com/timcera/hspf_reader/actions/workflows/python-package.yml/badge.svg
+.. image:: https://github.com/timcera/hspf_reader/actions/workflows/pypi-package.yml/badge.svg
     :alt: Tests
-    :target: https://github.com/timcera/hspf_reader/actions/workflows/python-package.yml
+    :target: https://github.com/timcera/hspf_reader/actions/workflows/pypi-package.yml
     :height: 20
 
 .. image:: https://img.shields.io/coveralls/github/timcera/hspf_reader
     :alt: Test Coverage
     :target: https://coveralls.io/r/timcera/hspf_reader?branch=master
     :height: 20
```

### Comparing `hspf_reader-1.0.7/docs/Makefile` & `hspf_reader-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/docs/conf.py` & `hspf_reader-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/docs/make.bat` & `hspf_reader-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/pyproject.toml` & `hspf_reader-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,26 @@
 [project]
 name = "hspf_reader"
 dynamic = ["version"]
 readme = "README.rst"
 description = "Command line script and Python library to read HSPF WDM, binary, and plotgen time series."
 dependencies = [
     "cltoolbox >= 2.0.0, < 3.0.0",
-    "typing-extensions",
-    "toolbox_utils >= 5.0.0, < 6.0.0",
+    "dateparser",
     "numpy",
-    "pandas"
+    "numpy",
+    "pandas",
+    "pandas[excel]",
+    "pint!=0.21.*",
+    "pint<0.22; python_version < '3.9'",
+    "pint-pandas",
+    "pydantic",
+    "scipy",
+    "tabulate",
+    "typing-extensions"
 ]
 authors = [
     {name = "Tim Cera", email = "tim@cerazone.net"}
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
@@ -99,23 +107,29 @@
     ".ipynb_checkpoints/*"
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "1.0.7"
+version = "1.1.0"
 version_files = ["VERSION"]
 
 [tool.isort]
 profile = "black"
 
 [tool.jupytext]
 formats = "ipynb,py:percent"
 
+[tool.pytest.ini_options]
+minversion = "6.0"
+testpaths = [
+    "tests"
+]
+
 [tool.setuptools]
 license-files = ["LICENSE.txt"]
 include-package-data = true
 
 [tool.setuptools.dynamic]
 readme = {file = "README.rst"}
 version = {file = "VERSION"}
```

### Comparing `hspf_reader-1.0.7/src/hspf_reader/hspf_reader.py` & `hspf_reader-1.1.0/src/hspf_reader/hspf_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """Collection of functions for reading different time series from HSPF."""
 
 import os.path as _os_path
 import sys as _sys
 import warnings as _warnings
 
 import pandas as pd
-from toolbox_utils import tsutils
-from toolbox_utils.readers.hbn import hbn_extract as _hbn
-from toolbox_utils.readers.plotgen import plotgen_extract as _plotgen
-from toolbox_utils.readers.wdm import wdm_extract as _wdm
+
+from hspf_reader.toolbox_utils.src.toolbox_utils import tsutils
+from hspf_reader.toolbox_utils.src.toolbox_utils.readers.hbn import hbn_extract as _hbn
+from hspf_reader.toolbox_utils.src.toolbox_utils.readers.plotgen import (
+    plotgen_extract as _plotgen,
+)
+from hspf_reader.toolbox_utils.src.toolbox_utils.readers.wdm import wdm_extract as _wdm
 
 _warnings.filterwarnings("ignore")
 
 
+def about():
+    """Display version number and system information."""
+    return tsutils.about("hspf_reader")
+
+
 @tsutils.doc(tsutils.docstrings)
 def hbn(hbnpath, interval, *labels, **kwds):
     r"""Prints out data to the screen from a HSPF binary output file.
 
     Parameters
     ----------
     hbnpath : str
@@ -266,14 +274,21 @@
     """Set debug, register *_cli functions, and run cltoolbox.main function."""
     import cltoolbox
     from cltoolbox.rst_text_formatter import RSTHelpFormatter
 
     if not _os_path.exists("debug_hspf_reader"):
         _sys.tracebacklimit = 0
 
+    @cltoolbox.command("about")
+    def _about_cli():
+        """Display version number and system information."""
+        about_dict = about()
+        for key in about_dict:
+            print(f"{key}: {about_dict[key]}")
+
     @cltoolbox.command("hbn", formatter_class=RSTHelpFormatter)
     @tsutils.copy_doc(hbn)
     def _hbn_cli(
         hbnpath,
         interval,
         start_date=None,
         end_date=None,
@@ -302,17 +317,12 @@
 
     @cltoolbox.command("wdm", formatter_class=RSTHelpFormatter)
     @tsutils.copy_doc(wdm)
     def _wdm_cli(start_date=None, end_date=None, *wdmpath):
         """docstring replaced by tsutils.copy_doc"""
         tsutils.printiso(wdm(*wdmpath, start_date=start_date, end_date=end_date))
 
-    @cltoolbox.command()
-    def about():
-        """Display version number and system information."""
-        tsutils.about(__name__)
-
     cltoolbox.main()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hspf_reader-1.0.7/src/hspf_reader.egg-info/PKG-INFO` & `hspf_reader-1.1.0/src/hspf_reader.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspf_reader
-Version: 1.0.7
+Version: 1.1.0
 Summary: Command line script and Python library to read HSPF WDM, binary, and plotgen time series.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/hspf_reader/docs/index.html#hspf_reader-documentation
 Project-URL: github, https://github.com/timcera/hspf_reader
 Project-URL: bitbucket, https://bitbucket.org/timcera/hspf_reader/src/main/
 Keywords: time-series,hspf,simulation,hydrology,hydrologic,python,cli,command line,script,cli-application
@@ -24,18 +24,26 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: cltoolbox<3.0.0,>=2.0.0
-Requires-Dist: typing-extensions
-Requires-Dist: toolbox_utils<6.0.0,>=5.0.0
+Requires-Dist: dateparser
+Requires-Dist: numpy
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: pandas[excel]
+Requires-Dist: pint!=0.21.*
+Requires-Dist: pint<0.22; python_version < "3.9"
+Requires-Dist: pint-pandas
+Requires-Dist: pydantic
+Requires-Dist: scipy
+Requires-Dist: tabulate
+Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: bandit; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: blacken-docs; extra == "dev"
 Requires-Dist: black-nbconvert; extra == "dev"
 Requires-Dist: cleanpy; extra == "dev"
 Requires-Dist: commitizen; extra == "dev"
@@ -54,17 +62,17 @@
 Requires-Dist: pytest-mpl; extra == "dev"
 Requires-Dist: pyupgrade; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: unimport; extra == "dev"
 Requires-Dist: velin; extra == "dev"
 Requires-Dist: vulture; extra == "dev"
 
-.. image:: https://github.com/timcera/hspf_reader/actions/workflows/python-package.yml/badge.svg
+.. image:: https://github.com/timcera/hspf_reader/actions/workflows/pypi-package.yml/badge.svg
     :alt: Tests
-    :target: https://github.com/timcera/hspf_reader/actions/workflows/python-package.yml
+    :target: https://github.com/timcera/hspf_reader/actions/workflows/pypi-package.yml
     :height: 20
 
 .. image:: https://img.shields.io/coveralls/github/timcera/hspf_reader
     :alt: Test Coverage
     :target: https://coveralls.io/r/timcera/hspf_reader?branch=master
     :height: 20
```

### Comparing `hspf_reader-1.0.7/src/hspf_reader.egg-info/SOURCES.txt` & `hspf_reader-1.1.0/src/hspf_reader.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 .deepsource.toml
 .gitignore
+.gitmodules
 .pre-commit-config.yaml
 .sourcery.yaml
 AUTHORS.rst
 BADGES.rst
 CHANGELOG.md
 CONTRIBUTING.rst
 LICENSE.txt
 README.rst
 VERSION
-publish.py
 pyproject.toml
 requirements.txt
+.github/dependabot.yml
 .github/workflows/clean-workflow-runs.yml
-.github/workflows/python-package.yml
+.github/workflows/pypi-package.yml
+.github/workflows/tests.yml
 docs/Makefile
 docs/authors.rst
 docs/command_line.rst
 docs/conf.py
 docs/contributing.rst
 docs/function_summary.rst
 docs/index.rst
```

### Comparing `hspf_reader-1.0.7/tests/data.wdm` & `hspf_reader-1.1.0/tests/data.wdm`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/tests/data_6b_np1.hbn` & `hspf_reader-1.1.0/tests/data_6b_np1.hbn`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/tests/data_plotgen.plt` & `hspf_reader-1.1.0/tests/data_plotgen.plt`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/tests/data_wdm_1.csv` & `hspf_reader-1.1.0/tests/data_wdm_1.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/tests/data_wdm_2.csv` & `hspf_reader-1.1.0/tests/data_wdm_2.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/tests/data_yearly.hbn` & `hspf_reader-1.1.0/tests/data_yearly.hbn`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/tests/sunspot_area.csv` & `hspf_reader-1.1.0/tests/sunspot_area.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/tests/sunspot_area_with_missing.csv` & `hspf_reader-1.1.0/tests/sunspot_area_with_missing.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.7/tests/test_hbn.py` & `hspf_reader-1.1.0/tests/test_hbn.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 import subprocess
 import sys
 from io import BytesIO, StringIO
 from unittest import TestCase
 
 import pandas as pd
 from pandas.testing import assert_frame_equal
-from toolbox_utils import tsutils
 
 from hspf_reader.hspf_reader import hbn
+from hspf_reader.toolbox_utils.src.toolbox_utils import tsutils
 
 
 def capture(func, *args, **kwds):
     sys.stdout = StringIO()  # capture output
     out = func(*args, **kwds)
     out = sys.stdout.getvalue()  # release output
     try:
```

### Comparing `hspf_reader-1.0.7/tests/test_plotgen.py` & `hspf_reader-1.1.0/tests/test_plotgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 import shlex
 import subprocess
 import sys
 from unittest import TestCase
 
 from pandas.testing import assert_frame_equal
-from toolbox_utils import tsutils
+
+from hspf_reader.toolbox_utils.src.toolbox_utils import tsutils
 
 try:
     from StringIO import StringIO
 except ImportError:
     from io import StringIO
 
 import pandas as pd
```

### Comparing `hspf_reader-1.0.7/tests/test_wdm.py` & `hspf_reader-1.1.0/tests/test_wdm.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 Tests for `hspf_reader` module.
 """
 
 import sys
 
 import pandas as pd
-from toolbox_utils import tsutils
+
+from hspf_reader.toolbox_utils.src.toolbox_utils import tsutils
 
 try:
     from cStringIO import StringIO
 except Exception:
     from io import StringIO
 
 from unittest import TestCase
```

