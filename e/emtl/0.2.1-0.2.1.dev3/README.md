# Comparing `tmp/emtl-0.2.1.tar.gz` & `tmp/emtl-0.2.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emtl-0.2.1.tar", last modified: Wed May 29 08:21:51 2024, max compression
+gzip compressed data, was "emtl-0.2.1.dev3.tar", last modified: Thu May 23 01:00:46 2024, max compression
```

## Comparing `emtl-0.2.1.tar` & `emtl-0.2.1.dev3.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:51.401201 emtl-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-29 08:21:39.000000 emtl-0.2.1/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-29 08:21:39.000000 emtl-0.2.1/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-29 08:21:39.000000 emtl-0.2.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-29 08:21:39.000000 emtl-0.2.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:51.393201 emtl-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:51.397201 emtl-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-29 08:21:39.000000 emtl-0.2.1/.github/workflows/document.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-29 08:21:39.000000 emtl-0.2.1/.github/workflows/github-actions.yml
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-29 08:21:39.000000 emtl-0.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-29 08:21:39.000000 emtl-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-29 08:21:39.000000 emtl-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 08:21:39.000000 emtl-0.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-29 08:21:39.000000 emtl-0.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-29 08:21:39.000000 emtl-0.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-29 08:21:39.000000 emtl-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-29 08:21:39.000000 emtl-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-29 08:21:51.401201 emtl-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-29 08:21:39.000000 emtl-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:51.397201 emtl-0.2.1/ci/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2867 2024-05-29 08:21:39.000000 emtl-0.2.1/ci/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 08:21:39.000000 emtl-0.2.1/ci/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:51.393201 emtl-0.2.1/ci/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:51.393201 emtl-0.2.1/ci/templates/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:51.397201 emtl-0.2.1/ci/templates/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-29 08:21:39.000000 emtl-0.2.1/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:51.397201 emtl-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 08:21:39.000000 emtl-0.2.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 08:21:39.000000 emtl-0.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-29 08:21:39.000000 emtl-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-29 08:21:39.000000 emtl-0.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-29 08:21:39.000000 emtl-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-29 08:21:39.000000 emtl-0.2.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 08:21:39.000000 emtl-0.2.1/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:51.397201 emtl-0.2.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-29 08:21:39.000000 emtl-0.2.1/docs/reference/emtl.rst
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 08:21:39.000000 emtl-0.2.1/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 08:21:39.000000 emtl-0.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-29 08:21:39.000000 emtl-0.2.1/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-29 08:21:39.000000 emtl-0.2.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-29 08:21:39.000000 emtl-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-29 08:21:39.000000 emtl-0.2.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:21:51.401201 emtl-0.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3055 2024-05-29 08:21:39.000000 emtl-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:51.393201 emtl-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:51.401201 emtl-0.2.1/src/emtl/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-29 08:21:39.000000 emtl-0.2.1/src/emtl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-29 08:21:39.000000 emtl-0.2.1/src/emtl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 08:21:51.000000 emtl-0.2.1/src/emtl/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 08:21:39.000000 emtl-0.2.1/src/emtl/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-29 08:21:39.000000 emtl-0.2.1/src/emtl/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-29 08:21:39.000000 emtl-0.2.1/src/emtl/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:51.401201 emtl-0.2.1/src/emtl/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:39.000000 emtl-0.2.1/src/emtl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-29 08:21:39.000000 emtl-0.2.1/src/emtl/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-29 08:21:39.000000 emtl-0.2.1/src/emtl/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-29 08:21:39.000000 emtl-0.2.1/src/emtl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:21:51.401201 emtl-0.2.1/src/emtl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-29 08:21:51.000000 emtl-0.2.1/src/emtl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-29 08:21:51.000000 emtl-0.2.1/src/emtl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:21:51.000000 emtl-0.2.1/src/emtl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 08:21:51.000000 emtl-0.2.1/src/emtl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:21:51.000000 emtl-0.2.1/src/emtl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 08:21:51.000000 emtl-0.2.1/src/emtl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 08:21:51.000000 emtl-0.2.1/src/emtl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-29 08:21:39.000000 emtl-0.2.1/tox.ini
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      761 2024-05-21 10:21:56.000000 emtl-0.2.1.dev3/.bumpversion.cfg
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1906 2024-05-21 10:21:56.000000 emtl-0.2.1.dev3/.cookiecutterrc
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      149 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.coveragerc
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      353 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.editorconfig
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.956884 emtl-0.2.1.dev3/.github/
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/.github/workflows/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      907 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.github/workflows/document.yml
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2721 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.github/workflows/github-actions.yml
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      734 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.gitignore
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      686 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.pre-commit-config.yaml
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      285 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.readthedocs.yml
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       65 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/AUTHORS.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      550 2024-05-21 10:15:07.000000 emtl-0.2.1.dev3/CHANGELOG.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2274 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/CONTRIBUTING.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1117 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/LICENSE
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2530 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/PKG-INFO
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2423 2024-05-22 10:56:16.000000 emtl-0.2.1.dev3/README.rst
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/ci/
+-rwxr-xr-x   0 riiy      (1000) riiy      (1000)     2867 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/ci/bootstrap.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       72 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/ci/requirements.txt
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.956884 emtl-0.2.1.dev3/ci/templates/
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.956884 emtl-0.2.1.dev3/ci/templates/.github/
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/ci/templates/.github/workflows/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2179 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/docs/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       28 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/authors.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       30 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/changelog.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1150 2024-05-21 10:21:56.000000 emtl-0.2.1.dev3/docs/conf.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       33 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/contributing.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      244 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/index.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       84 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/installation.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       27 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/readme.rst
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/docs/reference/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      146 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/reference/emtl.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       56 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/reference/index.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       14 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/requirements.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      109 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/spelling_wordlist.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      183 2024-05-22 10:57:54.000000 emtl-0.2.1.dev3/docs/usage.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1381 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/pyproject.toml
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1303 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/pytest.ini
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       38 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/setup.cfg
+-rwxr-xr-x   0 riiy      (1000) riiy      (1000)     3055 2024-05-21 10:21:56.000000 emtl-0.2.1.dev3/setup.py
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.956884 emtl-0.2.1.dev3/src/
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/src/emtl/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      547 2024-05-21 10:21:56.000000 emtl-0.2.1.dev3/src/emtl/__init__.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      354 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/src/emtl/__main__.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      424 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl/_version.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      988 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/src/emtl/cli.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1083 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/src/emtl/const.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     7105 2024-05-22 02:20:03.000000 emtl-0.2.1.dev3/src/emtl/core.py
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/src/emtl/tests/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)        0 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/src/emtl/tests/__init__.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      126 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/src/emtl/tests/test_cli.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2215 2024-05-22 02:26:03.000000 emtl-0.2.1.dev3/src/emtl/tests/test_core.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1371 2024-05-20 02:16:50.000000 emtl-0.2.1.dev3/src/emtl/utils.py
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/src/emtl.egg-info/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2530 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/PKG-INFO
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1045 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/SOURCES.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)        1 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/dependency_links.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       38 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/entry_points.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)        1 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/not-zip-safe
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       63 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/requires.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)        5 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/top_level.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1525 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/tox.ini
```

### Comparing `emtl-0.2.1/.bumpversion.cfg` & `emtl-0.2.1.dev3/.bumpversion.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.1
+current_version = 0.2.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = "fallback_version": "{current_version}"
 replace = "fallback_version": "{new_version}"
```

### Comparing `emtl-0.2.1/.cookiecutterrc` & `emtl-0.2.1.dev3/.cookiecutterrc`

 * *Files 0% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     setup_py_uses_setuptools_scm: "yes"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://emtl.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "alabaster"
     test_matrix_separate_coverage: "yes"
     tests_inside_package: "yes"
-    version: "0.2.1"
+    version: "0.2.0"
     version_manager: "bump2version"
     website: "riiy.gihub.io/emtl"
     year_from: "2024"
     year_to: "2025"
```

### Comparing `emtl-0.2.1/.github/workflows/document.yml` & `emtl-0.2.1.dev3/.github/workflows/document.yml`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/.github/workflows/github-actions.yml` & `emtl-0.2.1.dev3/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/.gitignore` & `emtl-0.2.1.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/.pre-commit-config.yaml` & `emtl-0.2.1.dev3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/CHANGELOG.rst` & `emtl-0.2.1.dev3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/CONTRIBUTING.rst` & `emtl-0.2.1.dev3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/LICENSE` & `emtl-0.2.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/PKG-INFO` & `emtl-0.2.1.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: emtl
-Version: 0.2.1
+Version: 0.2.1.dev3
 Summary: 东方财富自动交易接口
 Home-page: https://github.com/riiy/emtl
 Author: Riiy
 Author-email: riiyzhou@gmail.com
 License: MIT
 Project-URL: Documentation, https://emtl.readthedocs.io/
 Project-URL: Changelog, https://emtl.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/riiy/emtl/issues
 Keywords: autotrade,trade,东方财富,股票,交易,交易机器人
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -128,7 +129,9 @@
 * delete macos actions
 
 
 0.2.0 (2024-05-21)
 ------------------
 
 * complete all method
+
+
```

### Comparing `emtl-0.2.1/README.rst` & `emtl-0.2.1.dev3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/emtl
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/emtl.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/emtl
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/riiy/emtl/v0.2.1.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/riiy/emtl/v0.2.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/riiy/emtl/compare/v0.2.1...master
+    :target: https://github.com/riiy/emtl/compare/v0.2.0...master
 
 
 
 .. end-badges
 
 东方财富自动交易接口
```

### Comparing `emtl-0.2.1/ci/bootstrap.py` & `emtl-0.2.1.dev3/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/ci/templates/.github/workflows/github-actions.yml` & `emtl-0.2.1.dev3/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/docs/conf.py` & `emtl-0.2.1.dev3/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from pkg_resources import get_distribution
 
     version = release = get_distribution("emtl").version
 except Exception:
     import traceback
 
     traceback.print_exc()
-    version = release = "0.2.1"
+    version = release = "0.2.0"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/riiy/emtl/issues/%s", "#%s"),
     "pr": ("https://github.com/riiy/emtl/pull/%s", "PR #%s"),
 }
```

### Comparing `emtl-0.2.1/pyproject.toml` & `emtl-0.2.1.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/pytest.ini` & `emtl-0.2.1.dev3/pytest.ini`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/setup.py` & `emtl-0.2.1.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 setup(
     name="emtl",
     use_scm_version={
         "local_scheme": "dirty-tag",
         "write_to": "src/emtl/_version.py",
-        "fallback_version": "0.2.1",
+        "fallback_version": "0.2.0",
     },
     license="MIT",
     description="东方财富自动交易接口",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
```

### Comparing `emtl-0.2.1/src/emtl/__init__.py` & `emtl-0.2.1.dev3/src/emtl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.1"
+__version__ = "0.2.0"
 
 from .core import cancel_order
 from .core import insert_order
 from .core import login
 from .core import query_asset_and_position
 from .core import query_funds_flow
 from .core import query_history_orders
```

### Comparing `emtl-0.2.1/src/emtl/cli.py` & `emtl-0.2.1.dev3/src/emtl/cli.py`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/src/emtl/const.py` & `emtl-0.2.1.dev3/src/emtl/const.py`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/src/emtl/core.py` & `emtl-0.2.1.dev3/src/emtl/core.py`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/src/emtl/tests/test_core.py` & `emtl-0.2.1.dev3/src/emtl/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/src/emtl/utils.py` & `emtl-0.2.1.dev3/src/emtl/utils.py`

 * *Files identical despite different names*

### Comparing `emtl-0.2.1/src/emtl.egg-info/PKG-INFO` & `emtl-0.2.1.dev3/src/emtl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: emtl
-Version: 0.2.1
+Version: 0.2.1.dev3
 Summary: 东方财富自动交易接口
 Home-page: https://github.com/riiy/emtl
 Author: Riiy
 Author-email: riiyzhou@gmail.com
 License: MIT
 Project-URL: Documentation, https://emtl.readthedocs.io/
 Project-URL: Changelog, https://emtl.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/riiy/emtl/issues
 Keywords: autotrade,trade,东方财富,股票,交易,交易机器人
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -128,7 +129,9 @@
 * delete macos actions
 
 
 0.2.0 (2024-05-21)
 ------------------
 
 * complete all method
+
+
```

### Comparing `emtl-0.2.1/src/emtl.egg-info/SOURCES.txt` & `emtl-0.2.1.dev3/src/emtl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 README.rst
 pyproject.toml
 pytest.ini
 setup.py
 tox.ini
 .github/workflows/document.yml
 .github/workflows/github-actions.yml
-.github/workflows/release.yml
 ci/bootstrap.py
 ci/requirements.txt
 ci/templates/.github/workflows/github-actions.yml
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
```

### Comparing `emtl-0.2.1/tox.ini` & `emtl-0.2.1.dev3/tox.ini`

 * *Files identical despite different names*

