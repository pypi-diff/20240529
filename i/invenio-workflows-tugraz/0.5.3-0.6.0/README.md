# Comparing `tmp/invenio-workflows-tugraz-0.5.3.tar.gz` & `tmp/invenio-workflows-tugraz-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-workflows-tugraz-0.5.3.tar", last modified: Thu Mar 14 19:40:02 2024, max compression
+gzip compressed data, was "invenio-workflows-tugraz-0.6.0.tar", last modified: Wed May 29 12:52:45 2024, max compression
```

## Comparing `invenio-workflows-tugraz-0.5.3.tar` & `invenio-workflows-tugraz-0.6.0.tar`

### file list

```diff
@@ -1,82 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:40:02.654600 invenio-workflows-tugraz-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:40:02.642600 invenio-workflows-tugraz-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:40:02.646600 invenio-workflows-tugraz-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-03-14 19:40:02.658600 invenio-workflows-tugraz-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:40:02.650600 invenio-workflows-tugraz-0.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:40:02.650600 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:40:02.650600 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/data/
--rw-r--r--   0 runner    (1001) docker     (127)   939307 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/data/iso6393.json
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:40:02.654600 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/openaccess/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/openaccess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/openaccess/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/openaccess/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/openaccess/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/openaccess/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:40:02.654600 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:40:02.654600 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/alembic/02845ec6893c_update_theses_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/alembic/2b99bb26b381_create_theses_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/alembic/937ba80502f3_change_to_pid_column_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/alembic/9d446c6a77e2_create_theses_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/alembic/eca8ae6a6bc1_update_states_theses_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/theses.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:40:02.650600 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-03-14 19:40:02.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-14 19:40:02.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 19:40:02.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-14 19:40:02.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 19:40:02.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-14 19:40:02.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-14 19:40:02.000000 invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1246 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-14 19:40:02.658600 invenio-workflows-tugraz-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:40:02.654600 invenio-workflows-tugraz-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/tests/test_invenio_workflows_tugraz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:40:02.654600 invenio-workflows-tugraz-0.5.3/tests/theses/
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-03-14 19:39:56.000000 invenio-workflows-tugraz-0.5.3/tests/theses/test_theses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.362666 invenio-workflows-tugraz-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.350666 invenio-workflows-tugraz-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.354666 invenio-workflows-tugraz-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-29 12:52:45.362666 invenio-workflows-tugraz-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.354666 invenio-workflows-tugraz-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.358666 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.358666 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   939307 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/data/iso6393.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.358666 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/imoox/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/imoox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/imoox/visiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/imoox/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.358666 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/openaccess/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/openaccess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/openaccess/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/openaccess/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/openaccess/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/openaccess/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.362666 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.362666 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/alembic/02845ec6893c_update_theses_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/alembic/2b99bb26b381_create_theses_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/alembic/937ba80502f3_change_to_pid_column_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/alembic/9d446c6a77e2_create_theses_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/alembic/eca8ae6a6bc1_update_states_theses_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11619 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/theses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.358666 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-29 12:52:45.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-29 12:52:45.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:52:45.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-29 12:52:45.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:52:45.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-29 12:52:45.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 12:52:45.000000 invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1252 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-29 12:52:45.362666 invenio-workflows-tugraz-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.362666 invenio-workflows-tugraz-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.362666 invenio-workflows-tugraz-0.6.0/tests/imoox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/tests/imoox/test_imoox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/tests/test_invenio_workflows_tugraz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:52:45.362666 invenio-workflows-tugraz-0.6.0/tests/theses/
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-29 12:52:41.000000 invenio-workflows-tugraz-0.6.0/tests/theses/test_theses.py
```

### Comparing `invenio-workflows-tugraz-0.5.3/.editorconfig` & `invenio-workflows-tugraz-0.6.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/.github/workflows/tests.yml` & `invenio-workflows-tugraz-0.6.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/CHANGES.rst` & `invenio-workflows-tugraz-0.6.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     invenio-workflows-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.6.0 (release 2024-05-29)
+
+- add imoox workflow
+
+
 Version v0.5.3 (release 2024-03-14)
 
 - fix: thesis tasks wrong wording
 
 
 Version v0.5.2 (release 2024-03-12)
```

### Comparing `invenio-workflows-tugraz-0.5.3/CONTRIBUTING.rst` & `invenio-workflows-tugraz-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/LICENSE` & `invenio-workflows-tugraz-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/MANIFEST.in` & `invenio-workflows-tugraz-0.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/PKG-INFO` & `invenio-workflows-tugraz-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: invenio-workflows-tugraz
-Version: 0.5.3
+Version: 0.6.0
 Summary: "Package serves as a place for the workflows of the repository of the TU Graz."
 Home-page: https://github.com/tu-graz-library/invenio-workflows-tugraz
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio workflows TUGraz
 Platform: any
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Provides-Extra: tests
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # invenio-workflows-tugraz
@@ -26,14 +27,19 @@
     invenio-workflows-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.6.0 (release 2024-05-29)
+
+- add imoox workflow
+
+
 Version v0.5.3 (release 2024-03-14)
 
 - fix: thesis tasks wrong wording
 
 
 Version v0.5.2 (release 2024-03-12)
```

### Comparing `invenio-workflows-tugraz-0.5.3/babel.ini` & `invenio-workflows-tugraz-0.6.0/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/docs/Makefile` & `invenio-workflows-tugraz-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/docs/conf.py` & `invenio-workflows-tugraz-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/docs/index.rst` & `invenio-workflows-tugraz-0.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/docs/make.bat` & `invenio-workflows-tugraz-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/__init__.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 # details.
 
 """Package serves as a place for the workflows of the repository of the TU Graz."""
 
 from .ext import InvenioWorkflowsTugraz
 from .proxies import current_workflows_tugraz
 
-__version__ = "0.5.3"
+__version__ = "0.6.0"
 
 __all__ = (
     "__version__",
     "InvenioWorkflowsTugraz",
     "current_workflows_tugraz",
 )
```

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/config.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,47 +4,52 @@
 #
 # invenio-workflows-tugraz is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Configuration file."""
 
+from .imoox import imoox_import_func
 from .openaccess import pure_import_func, pure_sieve_func
 from .theses import (
     create_func,
     duplicate_func,
     import_from_alma_func,
     import_from_cms_func,
     theses_create_aggregator,
     theses_filter,
     theses_update_aggregator,
     update_func,
 )
 
-WORKFLOW_ALMA_REPOSITORY_RECORDS_IMPORT_FUNC = import_from_alma_func
+WORKFLOWS_ALMA_REPOSITORY_RECORDS_IMPORT_FUNC = import_from_alma_func
 """"""
 
-WORKFLOW_ALMA_REPOSITORY_RECORDS_UPDATE_AGGREGATOR = theses_update_aggregator
+WORKFLOWS_ALMA_REPOSITORY_RECORDS_UPDATE_AGGREGATOR = theses_update_aggregator
 """"""
 
-WORKFLOW_ALMA_REPOSITORY_RECORDS_UPDATE_FUNC = update_func
+WORKFLOWS_ALMA_REPOSITORY_RECORDS_UPDATE_FUNC = update_func
 """"""
 
-WORKFLOW_ALMA_ALMA_RECORDS_CREATE_FUNC = create_func
+WORKFLOWS_ALMA_ALMA_RECORDS_CREATE_FUNC = create_func
 """"""
 
-WORKFLOW_ALMA_ALMA_RECORDS_CREATE_AGGREGATOR = theses_create_aggregator
+WORKFLOWS_ALMA_ALMA_RECORDS_CREATE_AGGREGATOR = theses_create_aggregator
 """"""
 
-WORKFLOW_CAMPUSONLINE_THESES_FILTER = theses_filter()
+WORKFLOWS_CAMPUSONLINE_THESES_FILTER = theses_filter()
 """"""
 
-WORKFLOW_CAMPUSONLINE_IMPORT_FUNC = import_from_cms_func
+WORKFLOWS_CAMPUSONLINE_IMPORT_FUNC = import_from_cms_func
 """"""
 
-WORKFLOW_CAMPUSONLINE_DUPLICATE_FUNC = duplicate_func
+WORKFLOWS_CAMPUSONLINE_DUPLICATE_FUNC = duplicate_func
 """"""
 
-WORKFLOW_PURE_IMPORT_FUNC = pure_import_func
+WORKFLOWS_PURE_IMPORT_FUNC = pure_import_func
 """See corresponding varaible in invenio-pure."""
 
-WORKFLOW_PURE_SIEVE_FUNC = pure_sieve_func
+WORKFLOWS_PURE_SIEVE_FUNC = pure_sieve_func
+""""""
+
+WORKFLOWS_IMOOX_REPOSITORY_IMPORT_FUNC = imoox_import_func
+""""""
```

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/data/iso6393.json` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/data/iso6393.json`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/openaccess/convert.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/openaccess/convert.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/openaccess/utils.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/openaccess/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/openaccess/workflow.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/openaccess/workflow.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/__init__.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/alembic/02845ec6893c_update_theses_tables.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/alembic/02845ec6893c_update_theses_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/alembic/2b99bb26b381_create_theses_tables.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/alembic/2b99bb26b381_create_theses_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/alembic/937ba80502f3_change_to_pid_column_name.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/alembic/937ba80502f3_change_to_pid_column_name.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/alembic/9d446c6a77e2_create_theses_branch.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/alembic/9d446c6a77e2_create_theses_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/alembic/eca8ae6a6bc1_update_states_theses_tables.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/alembic/eca8ae6a6bc1_update_states_theses_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/api.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/api.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/cli.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/config.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/config.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/convert.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/convert.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/decorators.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/models.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/models.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/service.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/service.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/tasks.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/theses.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/theses.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     convert_json_to_marc21xml,
     create_record,
     current_records_marc21,
 )
 from invenio_records_marc21.services.record.types import ACNumber
 from invenio_records_resources.services.records.results import RecordItem
 from marshmallow.exceptions import ValidationError
+from opensearchpy.exceptions import RequestError
 from sqlalchemy.orm.exc import NoResultFound, StaleDataError
 
 from ..proxies import current_workflows_tugraz
 from .convert import CampusOnlineToMarc21
 from .types import CampusOnlineId
 
 error_record = NamedTuple("ErrorRecord", ["id"])
@@ -308,14 +309,17 @@
     try:
         marc21_service.edit(id_=marc_id, identity=identity)
         marc21_service.update_draft(id_=marc_id, identity=identity, data=data)
         marc21_service.publish(id_=marc_id, identity=identity)
     except ValidationError as error:
         msg = f"ValidationError cms_id: {cms_id}, error: {error}"
         raise RuntimeError(msg) from error
+    except RequestError as error:
+        msg = f"RequestError cms_id: {cms_id}, error: {error}"
+        raise RuntimeError(msg) from error
 
     theses_service.set_state(identity, id_=marc_id, state="updated_in_repo")
 
 
 def duplicate_func(cms_id: str) -> bool:
     """Check if the cms_id has already been imported."""
     try:
```

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/theses/views.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/theses/views.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz/types.py` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz/types.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz.egg-info/PKG-INFO` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: invenio-workflows-tugraz
-Version: 0.5.3
+Version: 0.6.0
 Summary: "Package serves as a place for the workflows of the repository of the TU Graz."
 Home-page: https://github.com/tu-graz-library/invenio-workflows-tugraz
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio workflows TUGraz
 Platform: any
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Provides-Extra: tests
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # invenio-workflows-tugraz
@@ -26,14 +27,19 @@
     invenio-workflows-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.6.0 (release 2024-05-29)
+
+- add imoox workflow
+
+
 Version v0.5.3 (release 2024-03-14)
 
 - fix: thesis tasks wrong wording
 
 
 Version v0.5.2 (release 2024-03-12)
```

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz.egg-info/SOURCES.txt` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 invenio_workflows_tugraz.egg-info/SOURCES.txt
 invenio_workflows_tugraz.egg-info/dependency_links.txt
 invenio_workflows_tugraz.egg-info/entry_points.txt
 invenio_workflows_tugraz.egg-info/not-zip-safe
 invenio_workflows_tugraz.egg-info/requires.txt
 invenio_workflows_tugraz.egg-info/top_level.txt
 invenio_workflows_tugraz/data/iso6393.json
+invenio_workflows_tugraz/imoox/__init__.py
+invenio_workflows_tugraz/imoox/visiter.py
+invenio_workflows_tugraz/imoox/workflows.py
 invenio_workflows_tugraz/openaccess/__init__.py
 invenio_workflows_tugraz/openaccess/convert.py
 invenio_workflows_tugraz/openaccess/types.py
 invenio_workflows_tugraz/openaccess/utils.py
 invenio_workflows_tugraz/openaccess/workflow.py
 invenio_workflows_tugraz/theses/__init__.py
 invenio_workflows_tugraz/theses/api.py
@@ -62,8 +65,9 @@
 invenio_workflows_tugraz/theses/alembic/2b99bb26b381_create_theses_tables.py
 invenio_workflows_tugraz/theses/alembic/937ba80502f3_change_to_pid_column_name.py
 invenio_workflows_tugraz/theses/alembic/9d446c6a77e2_create_theses_branch.py
 invenio_workflows_tugraz/theses/alembic/__init__.py
 invenio_workflows_tugraz/theses/alembic/eca8ae6a6bc1_update_states_theses_tables.py
 tests/conftest.py
 tests/test_invenio_workflows_tugraz.py
+tests/imoox/test_imoox.py
 tests/theses/test_theses.py
```

### Comparing `invenio-workflows-tugraz-0.5.3/invenio_workflows_tugraz.egg-info/entry_points.txt` & `invenio-workflows-tugraz-0.6.0/invenio_workflows_tugraz.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/run-tests.sh` & `invenio-workflows-tugraz-0.6.0/run-tests.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022-2023 Graz University of Technology.
+# Copyright (C) 2022-2024 Graz University of Technology.
 #
 # invenio-workflows-tugraz is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 # Quit on errors
 set -o errexit
@@ -37,13 +37,13 @@
 done
 
 if [[ ${keep_services} -eq 0 ]]; then
   trap cleanup EXIT
 fi
 
 
-ruff .
+ruff check .
 
 python -m check_manifest
 python -m sphinx.cmd.build -qnNW docs docs/_build/html
 eval "$(docker-services-cli up --db ${DB:-postgresql} --search ${SEARCH:-opensearch} --env)"
 python -m pytest ${pytest_args[@]+"${pytest_args[@]}"}
```

### Comparing `invenio-workflows-tugraz-0.5.3/setup.cfg` & `invenio-workflows-tugraz-0.6.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -9,32 +9,35 @@
 author_email = info@tugraz.at
 platforms = any
 url = https://github.com/tu-graz-library/invenio-workflows-tugraz
 classifiers = 
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Development Status :: 5 - Production/Stable
 
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.8
 zip_safe = False
 install_requires = 
 
 [options.extras_require]
 tests = 
-	pytest-black>=0.3.0
-	pytest-invenio>=1.4.0
-	invenio-search[opensearch2]>=2.1.0
 	invenio-alma>=0.7.1
+	invenio-app>=1.5.0
 	invenio-campusonline>=0.1.1
 	invenio-config-tugraz>=0.4.0
 	invenio-pure>=0.1.1
+	invenio-records-lom>=0.13.0
+	invenio-search[opensearch2]>=2.1.0
+	pytest-black-ng>=0.4.0
+	pytest-invenio>=1.4.0
 	ruff>=0.0.263
 	sphinx>=4.5
 
 [options.entry_points]
 flask.commands = 
 	workflows = invenio_workflows_tugraz.cli:workflows
 invenio_base.apps =
```

### Comparing `invenio-workflows-tugraz-0.5.3/tests/conftest.py` & `invenio-workflows-tugraz-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/tests/test_invenio_workflows_tugraz.py` & `invenio-workflows-tugraz-0.6.0/tests/test_invenio_workflows_tugraz.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.5.3/tests/theses/test_theses.py` & `invenio-workflows-tugraz-0.6.0/tests/theses/test_theses.py`

 * *Files identical despite different names*

