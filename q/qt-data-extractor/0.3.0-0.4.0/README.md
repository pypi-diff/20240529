# Comparing `tmp/qt_data_extractor-0.3.0.tar.gz` & `tmp/qt_data_extractor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qt_data_extractor-0.3.0.tar", last modified: Mon May 13 16:10:33 2024, max compression
+gzip compressed data, was "qt_data_extractor-0.4.0.tar", last modified: Wed May 29 18:05:33 2024, max compression
```

## Comparing `qt_data_extractor-0.3.0.tar` & `qt_data_extractor-0.4.0.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.949024 qt_data_extractor-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.953024 qt_data_extractor-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/data-extractor.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.957024 qt_data_extractor-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.957024 qt_data_extractor-0.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.949024 qt_data_extractor-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.957024 qt_data_extractor-0.3.0/src/qt_data_extractor/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.957024 qt_data_extractor-0.3.0/src/qt_data_extractor/design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/copy-progress.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/copy-prompt.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/create_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    27560 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/main-window.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/manage-connections.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/pandas_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/src/qt_data_extractor/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/hooks/hook-qt_data_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    33419 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/worker_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/static/
--rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/static/logo-256.ico
--rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/static/logo-48.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/wix.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:33.480023 qt_data_extractor-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:33.468023 qt_data_extractor-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:33.472023 qt_data_extractor-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-29 18:05:33.480023 qt_data_extractor-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/data-extractor.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:33.476023 qt_data_extractor-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:33.476023 qt_data_extractor-0.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/docs/aspen-ip21.md
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/docs/osisoft-pi.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-29 18:05:33.480023 qt_data_extractor-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:33.468023 qt_data_extractor-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:33.476023 qt_data_extractor-0.4.0/src/qt_data_extractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/src/qt_data_extractor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:33.476023 qt_data_extractor-0.4.0/src/qt_data_extractor/design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/src/qt_data_extractor/design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/src/qt_data_extractor/design/copy-progress.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/src/qt_data_extractor/design/copy-prompt.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/src/qt_data_extractor/design/create_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27560 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/src/qt_data_extractor/design/main-window.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/src/qt_data_extractor/design/manage-connections.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/src/qt_data_extractor/design/pandas_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:33.476023 qt_data_extractor-0.4.0/src/qt_data_extractor/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/src/qt_data_extractor/hooks/hook-qt_data_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/src/qt_data_extractor/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33419 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/src/qt_data_extractor/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/src/qt_data_extractor/worker_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:33.480023 qt_data_extractor-0.4.0/src/qt_data_extractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-29 18:05:33.000000 qt_data_extractor-0.4.0/src/qt_data_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-29 18:05:33.000000 qt_data_extractor-0.4.0/src/qt_data_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:05:33.000000 qt_data_extractor-0.4.0/src/qt_data_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-29 18:05:33.000000 qt_data_extractor-0.4.0/src/qt_data_extractor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:05:33.000000 qt_data_extractor-0.4.0/src/qt_data_extractor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-29 18:05:33.000000 qt_data_extractor-0.4.0/src/qt_data_extractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 18:05:33.000000 qt_data_extractor-0.4.0/src/qt_data_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:33.480023 qt_data_extractor-0.4.0/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/static/logo-256.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/static/logo-48.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:33.480023 qt_data_extractor-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-29 18:05:07.000000 qt_data_extractor-0.4.0/wix.json
```

### Comparing `qt_data_extractor-0.3.0/.coveragerc` & `qt_data_extractor-0.4.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/.github/workflows/ci.yml` & `qt_data_extractor-0.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/.gitignore` & `qt_data_extractor-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/.pre-commit-config.yaml` & `qt_data_extractor-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/.readthedocs.yml` & `qt_data_extractor-0.4.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/CONTRIBUTING.md` & `qt_data_extractor-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/LICENSE.txt` & `qt_data_extractor-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/PKG-INFO` & `qt_data_extractor-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-data-extractor
-Version: 0.3.0
+Version: 0.4.0
 Summary: Extract data from industrial historians
 Home-page: https://github.com/imubit/qt-data-extractor/
 Author: Meir Tseitlin
 Author-email: meir@imubit.com
 License: LGPLv3
 Project-URL: Documentation, https://github.com/imubit/qt-data-extractor/
 Project-URL: Source, https://github.com/imubit/qt-data-extractor/
@@ -15,93 +15,70 @@
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: pandas
 Requires-Dist: openpyxl
 Requires-Dist: PySide6
 Requires-Dist: data-agent>=0.2.0
 Requires-Dist: data-agent-osisoft-pi>=0.3.0
+Requires-Dist: data-agent-aspen-ip21
 Requires-Dist: data-agent-zip
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Provides-Extra: winexe
 Requires-Dist: pyinstaller; extra == "winexe"
 
 <!-- These are examples of badges you might want to add to your README:
      please update the URLs accordingly
 
-[![ReadTheDocs](https://readthedocs.org/projects/qt-data-extractor/badge/?version=latest)](https://qt-data-extractor.readthedocs.io/en/stable/)
 [![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/qt-data-extractor.svg)](https://anaconda.org/conda-forge/qt-data-extractor)
 [![Monthly Downloads](https://pepy.tech/badge/qt-data-extractor/month)](https://pepy.tech/project/qt-data-extractor)
 [![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/qt-data-extractor)
 -->
 
+[![ReadTheDocs](https://readthedocs.org/projects/qt-data-extractor/badge/?version=latest)](https://qt-data-extractor.readthedocs.io/en/stable/)
 [![PyPI-Server](https://img.shields.io/pypi/v/qt-data-extractor.svg)](https://pypi.org/project/qt-data-extractor/)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # Industrial Data Extractor
 
 Industrial Data Extractor is an open-source Windows application to extract process data from industrial systems
-and historians.
-
-The following systems are currently supported:
+and historians. The extractor supports browsing historian tags and extracting periods of data into zipped CSV files.
 
-* [Osisoft PI](https://github.com/imubit/data-agent-osisoft-pi)
+Supported historians are:
 
-It supports browsing and selecting tags on the target system and extract periods of data into zipped CSVs.
+* [Aveva (Osisoft) PI](osisoft-pi)
+* [AspenTech InfoPlus.21](aspen-ip21)
 
 ## Installation
 
 Please use https://github.com/imubit/qt-data-extractor/releases to download the latest version of the extractor.
-
-If you would like to extract data from Osisoft PI historian (which is the only one supported at this point). Please
-make sure you have [PI SDK](https://techsupport.osisoft.com/Products/PI-System-Access/PI-SDK/Overview) and AF SDK installed and configured on your workstation.
-
-## Getting Started
-
-* Configure the target historian using `Server` drop down.
-* Using left panel filter editor to browse for tags or import an Excel sheet with a list of tags.
-* Select tags you would like to extract on left panel and add then to the right panel with `Add to Selected Tags` button.
-* Select a period to be extracted and sample rate (use `Raw Data` option to extract the original sample rate that is stored within the historian).
-* Select `Save Directory` in which your archive will be populated.
-* Click `Extract` and confirm your selection.
-* Wait until extraction is finished.
-
-## Development
+You can use Windows setup file to install Data Extractor on Windows workstation or you can use Extractor executable to run the extractor without installation.
 
 ### Python Install
 
+Python package distribution is available in addition to Windows installer:
+
 ```python
 pip install qt-data-extractor
 ```
 
-### Running under CLI
+Starting the application from Windows Power Shell:
 
 ```
 PS C:\> qt-data-extractor
 ```
 
 * If the application is not starting this way, Python Scripts directory is probably not in the PATH. In this case you can run the script from Python installation directory (i.e. `c:\Python\Python39\Scripts\qt-data-extractor.exe`)
 
-### Building Windows Executable
-
-```bash
-pipx run tox -e winexe
-```
-
-### Building MSI Installer
-
-Install environment
-
-```
-Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
-choco install -y go-msi
-
-
-```
+## Getting Started
 
-Build MSI
+* Configure the target historian using `Server` drop down.
+* Using left panel filter editor to browse for tags or import an Excel sheet with a list of tags.
+* Select tags you would like to extract on left panel and add then to the right panel with `Add to Selected Tags` button.
+* Select a period to be extracted and sample rate (use `Raw Data` option to extract the original sample rate that is stored within the historian).
+* Select `Save Directory` in which your archive will be populated.
+* Click `Extract` and confirm your selection.
+* Wait until extraction is finished.
 
-```
-go-msi make --msi dist\windows-msi\ --version 0.1.1
-```
+Read documentation for a specific historian before attempting to extract data.
```

### Comparing `qt_data_extractor-0.3.0/README.md` & `qt_data_extractor-0.4.0/src/qt_data_extractor.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,84 @@
+Metadata-Version: 2.1
+Name: qt-data-extractor
+Version: 0.4.0
+Summary: Extract data from industrial historians
+Home-page: https://github.com/imubit/qt-data-extractor/
+Author: Meir Tseitlin
+Author-email: meir@imubit.com
+License: LGPLv3
+Project-URL: Documentation, https://github.com/imubit/qt-data-extractor/
+Project-URL: Source, https://github.com/imubit/qt-data-extractor/
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+License-File: LICENSE.txt
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: pandas
+Requires-Dist: openpyxl
+Requires-Dist: PySide6
+Requires-Dist: data-agent>=0.2.0
+Requires-Dist: data-agent-osisoft-pi>=0.3.0
+Requires-Dist: data-agent-aspen-ip21
+Requires-Dist: data-agent-zip
+Provides-Extra: testing
+Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Provides-Extra: winexe
+Requires-Dist: pyinstaller; extra == "winexe"
+
 <!-- These are examples of badges you might want to add to your README:
      please update the URLs accordingly
 
-[![ReadTheDocs](https://readthedocs.org/projects/qt-data-extractor/badge/?version=latest)](https://qt-data-extractor.readthedocs.io/en/stable/)
 [![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/qt-data-extractor.svg)](https://anaconda.org/conda-forge/qt-data-extractor)
 [![Monthly Downloads](https://pepy.tech/badge/qt-data-extractor/month)](https://pepy.tech/project/qt-data-extractor)
 [![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/qt-data-extractor)
 -->
 
+[![ReadTheDocs](https://readthedocs.org/projects/qt-data-extractor/badge/?version=latest)](https://qt-data-extractor.readthedocs.io/en/stable/)
 [![PyPI-Server](https://img.shields.io/pypi/v/qt-data-extractor.svg)](https://pypi.org/project/qt-data-extractor/)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # Industrial Data Extractor
 
 Industrial Data Extractor is an open-source Windows application to extract process data from industrial systems
-and historians.
+and historians. The extractor supports browsing historian tags and extracting periods of data into zipped CSV files.
 
-The following systems are currently supported:
+Supported historians are:
 
-* [Osisoft PI](https://github.com/imubit/data-agent-osisoft-pi)
-
-It supports browsing and selecting tags on the target system and extract periods of data into zipped CSVs.
+* [Aveva (Osisoft) PI](osisoft-pi)
+* [AspenTech InfoPlus.21](aspen-ip21)
 
 ## Installation
 
 Please use https://github.com/imubit/qt-data-extractor/releases to download the latest version of the extractor.
-
-If you would like to extract data from Osisoft PI historian (which is the only one supported at this point). Please
-make sure you have [PI SDK](https://techsupport.osisoft.com/Products/PI-System-Access/PI-SDK/Overview) and AF SDK installed and configured on your workstation.
-
-## Getting Started
-
-* Configure the target historian using `Server` drop down.
-* Using left panel filter editor to browse for tags or import an Excel sheet with a list of tags.
-* Select tags you would like to extract on left panel and add then to the right panel with `Add to Selected Tags` button.
-* Select a period to be extracted and sample rate (use `Raw Data` option to extract the original sample rate that is stored within the historian).
-* Select `Save Directory` in which your archive will be populated.
-* Click `Extract` and confirm your selection.
-* Wait until extraction is finished.
-
-## Development
+You can use Windows setup file to install Data Extractor on Windows workstation or you can use Extractor executable to run the extractor without installation.
 
 ### Python Install
 
+Python package distribution is available in addition to Windows installer:
+
 ```python
 pip install qt-data-extractor
 ```
 
-### Running under CLI
+Starting the application from Windows Power Shell:
 
 ```
 PS C:\> qt-data-extractor
 ```
 
 * If the application is not starting this way, Python Scripts directory is probably not in the PATH. In this case you can run the script from Python installation directory (i.e. `c:\Python\Python39\Scripts\qt-data-extractor.exe`)
 
-### Building Windows Executable
-
-```bash
-pipx run tox -e winexe
-```
-
-### Building MSI Installer
-
-Install environment
-
-```
-Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
-choco install -y go-msi
-
-
-```
+## Getting Started
 
-Build MSI
+* Configure the target historian using `Server` drop down.
+* Using left panel filter editor to browse for tags or import an Excel sheet with a list of tags.
+* Select tags you would like to extract on left panel and add then to the right panel with `Add to Selected Tags` button.
+* Select a period to be extracted and sample rate (use `Raw Data` option to extract the original sample rate that is stored within the historian).
+* Select `Save Directory` in which your archive will be populated.
+* Click `Extract` and confirm your selection.
+* Wait until extraction is finished.
 
-```
-go-msi make --msi dist\windows-msi\ --version 0.1.1
-```
+Read documentation for a specific historian before attempting to extract data.
```

### Comparing `qt_data_extractor-0.3.0/data-extractor.spec` & `qt_data_extractor-0.4.0/data-extractor.spec`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     datas=[('src/qt_data_extractor/design/*.ui', 'design')],
     hiddenimports=['win32timezone', 'data_agent'],
     hookspath=['src/qt_data_extractor/hooks'],
     hooksconfig={},
     runtime_hooks=[],
     excludes=[],
     noarchive=False,
+    optimize=0,
 )
 pyz = PYZ(a.pure)
 
 exe = EXE(
     pyz,
     a.scripts,
     a.binaries,
```

### Comparing `qt_data_extractor-0.3.0/docs/Makefile` & `qt_data_extractor-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/docs/conf.py` & `qt_data_extractor-0.4.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     "sphinx.ext.autosummary",
     "sphinx.ext.viewcode",
     "sphinx.ext.coverage",
     "sphinx.ext.doctest",
     "sphinx.ext.ifconfig",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
+    'sphinx_rtd_theme',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 
 # Enable markdown
@@ -101,16 +102,16 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = "qt-data-extractor"
-copyright = "2023, Meir Tseitlin"
+project = "Industrial Data Extractor"
+copyright = "2023 Imubit Inc. All Rights Reserved"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # version: The short X.Y version.
 # release: The full version, including alpha/beta/rc tags.
@@ -167,42 +168,54 @@
 todo_emit_warnings = True
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "alabaster"
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
-    "sidebar_width": "300px",
-    "page_width": "1200px"
+    # 'analytics_id': 'G-XXXXXXXXXX',  #  Provided by Google in your dashboard
+    'analytics_anonymize_ip': False,
+    'logo_only': False,
+    'display_version': True,
+    'prev_next_buttons_location': 'bottom',
+    'style_external_links': False,
+    'vcs_pageview_mode': '',
+    'style_nav_header_background': 'white',
+    # Toc options
+    'collapse_navigation': True,
+    'sticky_navigation': True,
+    'navigation_depth': 4,
+    'includehidden': True,
+    'titles_only': False
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 # html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-# html_logo = ""
+html_logo = "static/logo-256.ico"
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-# html_favicon = None
+html_favicon = "static/logo-48.ico"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
```

### Comparing `qt_data_extractor-0.3.0/setup.cfg` & `qt_data_extractor-0.4.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	pandas
 	openpyxl
 	PySide6
 	data-agent>=0.2.0
 	data-agent-osisoft-pi>=0.3.0
+	data-agent-aspen-ip21
 	data-agent-zip
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `qt_data_extractor-0.3.0/setup.py` & `qt_data_extractor-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/src/qt_data_extractor/__init__.py` & `qt_data_extractor-0.4.0/src/qt_data_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/src/qt_data_extractor/design/copy-progress.ui` & `qt_data_extractor-0.4.0/src/qt_data_extractor/design/copy-progress.ui`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/src/qt_data_extractor/design/copy-prompt.ui` & `qt_data_extractor-0.4.0/src/qt_data_extractor/design/copy-prompt.ui`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/src/qt_data_extractor/design/create_connection.py` & `qt_data_extractor-0.4.0/src/qt_data_extractor/design/create_connection.py`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/src/qt_data_extractor/design/main-window.ui` & `qt_data_extractor-0.4.0/src/qt_data_extractor/design/main-window.ui`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/src/qt_data_extractor/design/manage-connections.ui` & `qt_data_extractor-0.4.0/src/qt_data_extractor/design/manage-connections.ui`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/src/qt_data_extractor/design/pandas_model.py` & `qt_data_extractor-0.4.0/src/qt_data_extractor/design/pandas_model.py`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/src/qt_data_extractor/main.py` & `qt_data_extractor-0.4.0/src/qt_data_extractor/main.py`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/src/qt_data_extractor/mainwindow.py` & `qt_data_extractor-0.4.0/src/qt_data_extractor/mainwindow.py`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/src/qt_data_extractor/worker_thread.py` & `qt_data_extractor-0.4.0/src/qt_data_extractor/worker_thread.py`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/SOURCES.txt` & `qt_data_extractor-0.4.0/src/qt_data_extractor.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,20 +12,23 @@
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 wix.json
 .github/workflows/ci.yml
 docs/Makefile
+docs/aspen-ip21.md
 docs/authors.md
 docs/changelog.md
 docs/conf.py
 docs/contributing.md
+docs/development.md
 docs/index.md
 docs/license.md
+docs/osisoft-pi.md
 docs/readme.md
 docs/requirements.txt
 docs/_static/.gitignore
 src/qt_data_extractor/__init__.py
 src/qt_data_extractor/main.py
 src/qt_data_extractor/mainwindow.py
 src/qt_data_extractor/worker_thread.py
```

### Comparing `qt_data_extractor-0.3.0/static/logo-256.ico` & `qt_data_extractor-0.4.0/static/logo-256.ico`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/static/logo-48.ico` & `qt_data_extractor-0.4.0/static/logo-48.ico`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/tox.ini` & `qt_data_extractor-0.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `qt_data_extractor-0.3.0/wix.json` & `qt_data_extractor-0.4.0/wix.json`

 * *Files identical despite different names*

