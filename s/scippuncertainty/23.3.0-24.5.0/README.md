# Comparing `tmp/scippuncertainty-23.3.0.tar.gz` & `tmp/scippuncertainty-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scippuncertainty-23.3.0.tar", last modified: Mon Mar 20 09:02:37 2023, max compression
+gzip compressed data, was "scippuncertainty-24.5.0.tar", last modified: Wed May 29 08:07:47 2024, max compression
```

## Comparing `scippuncertainty-23.3.0.tar` & `scippuncertainty-24.5.0.tar`

### file list

```diff
@@ -1,83 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.175410 scippuncertainty-23.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.159409 scippuncertainty-23.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.163409 scippuncertainty-23.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3608 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1980 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2981 2023-03-20 09:02:37.175410 scippuncertainty-23.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.163409 scippuncertainty-23.3.0/conda/
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.163409 scippuncertainty-23.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.163409 scippuncertainty-23.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    32018 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.163409 scippuncertainty-23.3.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/_templates/scipp-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/_templates/scipp-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.163409 scippuncertainty-23.3.0/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/_templates/sections/header-article.html
--rw-r--r--   0 runner    (1001) docker     (122)     3436 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/bibliography.bib
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7117 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.163409 scippuncertainty-23.3.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.163409 scippuncertainty-23.3.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/user-guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)    28414 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/user-guide/mc.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     4178 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/docs/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.167410 scippuncertainty-23.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      480 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)     5282 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.167410 scippuncertainty-23.3.0/resources/
--rw-r--r--   0 runner    (1001) docker     (122)   115301 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/resources/logo-2023.svg
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-03-20 09:02:37.175410 scippuncertainty-23.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.159409 scippuncertainty-23.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.171409 scippuncertainty-23.3.0/src/scippuncertainty/
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/src/scippuncertainty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5604 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/src/scippuncertainty/_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/src/scippuncertainty/_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1392 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/src/scippuncertainty/correlation.py
--rw-r--r--   0 runner    (1001) docker     (122)      423 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/src/scippuncertainty/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.171409 scippuncertainty-23.3.0/src/scippuncertainty/mc/
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/src/scippuncertainty/mc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8494 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/src/scippuncertainty/mc/accumulator.py
--rw-r--r--   0 runner    (1001) docker     (122)     7177 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/src/scippuncertainty/mc/driver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4404 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/src/scippuncertainty/mc/sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/src/scippuncertainty/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/src/scippuncertainty/random.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.171409 scippuncertainty-23.3.0/src/scippuncertainty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2981 2023-03-20 09:02:37.000000 scippuncertainty-23.3.0/src/scippuncertainty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-03-20 09:02:37.000000 scippuncertainty-23.3.0/src/scippuncertainty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-20 09:02:37.000000 scippuncertainty-23.3.0/src/scippuncertainty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-03-20 09:02:37.000000 scippuncertainty-23.3.0/src/scippuncertainty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-03-20 09:02:37.000000 scippuncertainty-23.3.0/src/scippuncertainty.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.171409 scippuncertainty-23.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1711 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/tests/correlation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:37.175410 scippuncertainty-23.3.0/tests/mc/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/tests/mc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8329 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/tests/mc/accumulator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7569 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/tests/mc/driver_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     8146 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/tests/mc/sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/tests/random_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/tests/util_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-03-20 09:02:22.000000 scippuncertainty-23.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.420634 scippuncertainty-24.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.404634 scippuncertainty-24.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.408634 scippuncertainty-24.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/.github/workflows/nightly_at_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/.github/workflows/nightly_at_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/.github/workflows/python-version-ci
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/.github/workflows/unpinned.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-29 08:07:47.420634 scippuncertainty-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.408634 scippuncertainty-24.5.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.408634 scippuncertainty-24.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.408634 scippuncertainty-24.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/_static/anaconda-icon.js
+-rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    32277 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32018 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.408634 scippuncertainty-24.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/_templates/class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/_templates/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/_templates/module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.408634 scippuncertainty-24.5.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/about/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.412634 scippuncertainty-24.5.0/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/bibliography.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7580 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.412634 scippuncertainty-24.5.0/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/developer/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.412634 scippuncertainty-24.5.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/user-guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    28339 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/docs/user-guide/mc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.416634 scippuncertainty-24.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/basetest.in
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/basetest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/make_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/nightly.in
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/nightly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.416634 scippuncertainty-24.5.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   115301 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/resources/logo-2023.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:07:47.420634 scippuncertainty-24.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.404634 scippuncertainty-24.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.416634 scippuncertainty-24.5.0/src/scippuncertainty/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/src/scippuncertainty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/src/scippuncertainty/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/src/scippuncertainty/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/src/scippuncertainty/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/src/scippuncertainty/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.420634 scippuncertainty-24.5.0/src/scippuncertainty/mc/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/src/scippuncertainty/mc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/src/scippuncertainty/mc/accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/src/scippuncertainty/mc/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/src/scippuncertainty/mc/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/src/scippuncertainty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/src/scippuncertainty/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.420634 scippuncertainty-24.5.0/src/scippuncertainty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-29 08:07:47.000000 scippuncertainty-24.5.0/src/scippuncertainty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-29 08:07:47.000000 scippuncertainty-24.5.0/src/scippuncertainty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:07:47.000000 scippuncertainty-24.5.0/src/scippuncertainty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 08:07:47.000000 scippuncertainty-24.5.0/src/scippuncertainty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 08:07:47.000000 scippuncertainty-24.5.0/src/scippuncertainty.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.420634 scippuncertainty-24.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/tests/correlation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:47.420634 scippuncertainty-24.5.0/tests/mc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/tests/mc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/tests/mc/accumulator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/tests/mc/driver_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/tests/mc/sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/tests/package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/tests/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/tests/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-29 08:07:39.000000 scippuncertainty-24.5.0/tox.ini
```

### Comparing `scippuncertainty-23.3.0/.github/workflows/docs.yml` & `scippuncertainty-24.5.0/.github/workflows/docs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -6,55 +6,68 @@
       publish:
         default: false
         type: boolean
       version:
         default: ''
         required: false
         type: string
+      branch:
+        description: 'Branch/tag with documentation source. If not set, the current branch will be used.'
+        default: ''
+        required: false
+        type: string
   workflow_call:
     inputs:
       publish:
         default: false
         type: boolean
       version:
         default: ''
         required: false
         type: string
+      branch:
+        description: 'Branch/tag with documentation source. If not set, the current branch will be used.'
+        default: ''
+        required: false
+        type: string
+      linkcheck:
+        description: 'Run the link checker. If not set the link checker will not be run.'
+        default: false
+        required: false
+        type: boolean
 
 env:
   VERSION: ${{ inputs.version }}
 
 jobs:
   docs:
     name: Build documentation
-    runs-on: ubuntu-20.04
+    runs-on: 'ubuntu-22.04'
     steps:
       - run: sudo apt install --yes graphviz pandoc
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
-          ref: ${{ inputs.version }}
+          ref: ${{ inputs.branch == '' && github.ref_name || inputs.branch }}
+          repository: ${{ github.event.pull_request.head.repo.full_name }}
           fetch-depth: 0  # history required so cmake can determine version
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v5
         with:
-          python-version: 3.8
+          python-version-file: '.github/workflows/python-version-ci'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
-      - run: |
-          tox --skip-pkg-install -e docs -- scippuncertainty==${VERSION}
-          echo "target=$(python docs/version.py --repo=scippuncertainty --version=${VERSION} --action=get-target)" >> $GITHUB_ENV
-        if: ${{ inputs.publish }}
+      - run: tox -e releasedocs -- ${VERSION}
+        if: ${{ inputs.version != '' }}
       - run: tox -e docs
-        if: ${{ !inputs.publish }}
-      - uses: actions/upload-artifact@v3
+        if: ${{ inputs.version == '' }}
+      - run: tox -e linkcheck
+        if: ${{ inputs.linkcheck }}
+      - uses: actions/upload-artifact@v4
         with:
-          name: html
+          name: docs_html
           path: html/
 
-      - uses: JamesIves/github-pages-deploy-action@v4.4.1
+      - uses: JamesIves/github-pages-deploy-action@v4.6.1
         if: ${{ inputs.publish }}
         with:
           branch: gh-pages
           folder: html
-          target-folder: ${{ env.target }}
           single-commit: true
-          clean-exclude: release
-          ssh-key: ${{ secrets.GH_PAGES_DEPLOY_KEY }}
```

### Comparing `scippuncertainty-23.3.0/.github/workflows/release.yml` & `scippuncertainty-24.5.0/.github/workflows/release.yml`

 * *Files 20% similar despite different names*

```diff
@@ -8,110 +8,106 @@
 defaults:
   run:
     shell: bash -l {0}  # required for conda env
 
 jobs:
   build_conda:
     name: Conda build
-    runs-on: ubuntu-20.04
+    runs-on: 'ubuntu-22.04'
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
         with:
           submodules: true
-          fetch-depth: 0  # history required so cmake can determine version
+          fetch-depth: 0  # history required so setuptools_scm can determine version
 
-      - uses: conda-incubator/setup-miniconda@v2
-      - run: conda install --yes conda-build
-      - run: conda build --channel conda-forge --channel scipp --python=3.8 --no-anaconda-upload --override-channels --output-folder conda/package conda
+      - uses: mamba-org/setup-micromamba@v1
+        with:
+          environment-name: build-env
+          create-args: >-
+            conda-build
+            boa
+      - run: conda mambabuild --channel conda-forge --channel scipp --no-anaconda-upload --override-channels --output-folder conda/package conda
 
-      - uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v4
         with:
           name: conda-package-noarch
-          path: conda/package/*/scippuncertainty*.tar.bz2
+          path: conda/package/noarch/*.tar.bz2
 
   build_wheels:
     name: Wheels
-    runs-on: ubuntu-20.04
+    runs-on: 'ubuntu-22.04'
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0  # history required so setuptools_scm can determine version
 
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v5
         with:
-          python-version: 3.8
+          python-version-file: '.github/workflows/python-version-ci'
 
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/wheels.txt
 
       - name: Build wheels
         run: python -m build
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v4
         with:
           name: dist
           path: dist
 
   upload_pypi:
     name: Deploy PyPI
     needs: [build_wheels, build_conda]
-    runs-on: ubuntu-20.04
+    runs-on: 'ubuntu-22.04'
+    environment: release
+    permissions:
+      id-token: write
     if: github.event_name == 'release' && github.event.action == 'published'
-
     steps:
-      - uses: actions/download-artifact@v2
-      - uses: actions/setup-python@v3
-      - uses: pypa/gh-action-pypi-publish@v1.8.1
-        with:
-          user: __token__
-          password: ${{ secrets.PYPI_TOKEN }}
+      - uses: actions/download-artifact@v4
+      - uses: pypa/gh-action-pypi-publish@v1.8.14
 
   upload_conda:
-    name: Deploy Conda Forge
+    name: Deploy Conda
     needs: [build_wheels, build_conda]
-    runs-on: ubuntu-20.04
+    runs-on: 'ubuntu-22.04'
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
-      - uses: actions/download-artifact@v2
-      - uses: conda-incubator/setup-miniconda@v2
-      - run: conda install -c conda-forge --yes anaconda-client
-      - run: anaconda --token ${{ secrets.ANACONDATOKEN }} upload --user scipp --label main $(ls conda-package-*/*/*.tar.bz2)
-
-  manage-versions:
-    name: Manage Versions
-    runs-on: ubuntu-20.04
-    outputs:
-      version-new: ${{ steps.version.outputs.new }}
-      version-replaced: ${{ steps.version.outputs.replaced }}
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v3
+      - uses: actions/download-artifact@v4
+      - uses: mamba-org/setup-micromamba@v1
         with:
-          python-version: 3.8
-      - run: python -m pip install --upgrade pip
-      - run: python -m pip install -r requirements/ci.txt
-      - name: Set outputs
-        id: version
-        run: |
-          echo "new=$(python docs/version.py --repo=scippuncertainty --version=${GITHUB_REF_NAME} --action=is-new)" >> $GITHUB_OUTPUT
-          echo "replaced=$(python docs/version.py --repo=scippuncertainty --version=${GITHUB_REF_NAME} --action=get-replaced)" >> $GITHUB_OUTPUT
+          environment-name: upload-env
+          # frozen python due to breaking removal of 'imp' in 3.12
+          create-args: >-
+            anaconda-client
+            python=3.11
+      - run: anaconda --token ${{ secrets.ANACONDATOKEN }} upload --user scipp --label main $(ls conda-package-noarch/*.tar.bz2)
 
   docs:
-    needs: [upload_conda, upload_pypi, manage-versions]
+    needs: [upload_conda, upload_pypi]
     uses: ./.github/workflows/docs.yml
     with:
       publish: ${{ github.event_name == 'release' && github.event.action == 'published' }}
-      version: ${{ github.ref_name }}
     secrets: inherit
 
-  replaced-docs:
+  assets:
+    name: Upload docs
     needs: docs
-    if: github.event_name == 'release' && github.event.action == 'published' && needs.manage-versions.outputs.version-new == 'True'
-    uses: ./.github/workflows/docs.yml
-    with:
-      publish: true
-      version: ${{ needs.manage-versions.outputs.version-replaced }}
-    secrets: inherit
+    runs-on: 'ubuntu-22.04'
+    permissions:
+      contents: write  # This is needed so that the action can upload the asset
+    steps:
+    - uses: actions/download-artifact@v4
+    - name: Zip documentation
+      run: |
+        mv docs_html documentation-${{ github.ref_name }}
+        zip -r documentation-${{ github.ref_name }}.zip documentation-${{ github.ref_name }}
+    - name: Upload release assets
+      uses: svenstaro/upload-release-action@v2
+      with:
+        file: ./documentation-${{ github.ref_name }}.zip
+        overwrite: false
```

### Comparing `scippuncertainty-23.3.0/LICENSE` & `scippuncertainty-24.5.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Sci++
+Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
+All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `scippuncertainty-23.3.0/conda/meta.yaml` & `scippuncertainty-24.5.0/conda/meta.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 package:
   name: scippuncertainty
+
   version: {{ GIT_DESCRIBE_TAG }}
+
 source:
   path: ..
 
+
+{% set pyproject = load_file_data('pyproject.toml') %}
+{% set dependencies = pyproject.get('project', {}).get('dependencies', {}) %}
+
+
 requirements:
   build:
     - setuptools
     - setuptools_scm
   run:
-    - python>=3.8
-    - scipp>=23.01.1
+    - python>=3.10
+
+  {% for package in dependencies %}
+    - {% if package == "graphviz" %}python-graphviz{% else %}{{ package }}{% endif %}
+  {% endfor %}
 
 test:
   imports:
     - scippuncertainty
   requires:
     - pytest
   source_files:
     - pyproject.toml
     - tests/
   commands:
-    - python -m pytest tests
+    # We ignore warnings during release package builds
+    - python -m pytest -Wignore tests
 
 build:
   noarch: python
   script:
-    - pip install .
+    - python -m pip install .
 
 about:
   home: https://github.com/scipp/scippuncertainty
   license: BSD-3-Clause
   summary: Advanced uncertainty propagation with Scipp
   description: Advanced uncertainty propagation with Scipp
   dev_url: https://github.com/scipp/scippuncertainty
```

### Comparing `scippuncertainty-23.3.0/docs/_static/favicon.ico` & `scippuncertainty-24.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scippuncertainty-23.3.0/docs/_static/logo.svg` & `scippuncertainty-24.5.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `scippuncertainty-23.3.0/docs/_templates/scipp-class-template.rst` & `scippuncertainty-24.5.0/docs/_templates/class-template.rst`

 * *Files identical despite different names*

### Comparing `scippuncertainty-23.3.0/docs/_templates/scipp-module-template.rst` & `scippuncertainty-24.5.0/docs/_templates/module-template.rst`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
    {% block classes %}
    {% if classes %}
    .. rubric:: {{ _('Classes') }}
 
    .. autosummary::
       :toctree:
-      :template: scipp-class-template.rst
+      :template: class-template.rst
    {% for item in classes %}
       {{ item }}
    {%- endfor %}
    {% endif %}
    {% endblock %}
 
    {% block exceptions %}
@@ -53,14 +53,14 @@
 
 {% block modules %}
 {% if modules %}
 .. rubric:: Modules
 
 .. autosummary::
    :toctree:
-   :template: scipp-module-template.rst
+   :template: module-template.rst
    :recursive:
 {% for item in modules %}
    {{ item }}
 {%- endfor %}
 {% endif %}
 {% endblock %}
```

### Comparing `scippuncertainty-23.3.0/docs/bibliography.bib` & `scippuncertainty-24.5.0/docs/bibliography.bib`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     journal = {Technometrics},
     volume = {4},
     number = {3},
     pages = {419-420},
     year = {1962},
     publisher = {Taylor & Francis},
     doi = {10.1080/00401706.1962.10490022},
-    URL = {https://www.tandfonline.com/doi/abs/10.1080/00401706.1962.10490022},
 }
 
 @InProceedings{chan:1982,
     author = "Chan, T. F. and Golub, G. H. and LeVeque, R. J.",
     editor = "Caussinus, H. and Ettinger, P. and Tomassone, R.",
     title = "Updating Formulae and a Pairwise Algorithm for Computing Sample Variances",
     booktitle = "COMPSTAT 1982 5th Symposium held at Toulouse 1982",
```

### Comparing `scippuncertainty-23.3.0/docs/conf.py` & `scippuncertainty-24.5.0/docs/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,220 +1,251 @@
 import doctest
-import os
-import sys
-from typing import Any, Dict, Optional
-
-import sphinx_book_theme
-from docutils.nodes import document
-from sphinx.application import Sphinx
-
-import scippuncertainty
-
-sys.path.insert(0, os.path.abspath("."))
-
-from version import VersionInfo  # noqa: E402
+from importlib.metadata import version as get_version
 
 # General information about the project.
-project = "scippuncertainty"
-copyright = "2023 Scipp contributors"
-author = "Scipp contributors"
-
-version_info = VersionInfo(repo=project)
-long_version = scippuncertainty.__version__
-outdated = not version_info.is_latest(long_version)
-
-
-def add_buttons(
-    app: Sphinx,
-    pagename: str,
-    templatename: str,
-    context: Dict[str, Any],
-    doctree: Optional[document],
-):
-    base = "https://scipp.github.io"
-    l1 = []
-    l1.append({"type": "link", "text": "scipp", "url": f"{base}"})
-    l1.append({"type": "link", "text": "plopp", "url": f"{base}/plopp"})
-    l1.append({"type": "link", "text": "scippnexus", "url": f"{base}/scippnexus"})
-    l1.append({"type": "link", "text": "scippneutron", "url": f"{base}/scippneutron"})
-    l1.append({"type": "link", "text": "ess", "url": f"{base}/ess"})
-    l1.append(
-        {"type": "link", "text": "scippuncertainty", "url": f"{base}/scippuncertainty"}
-    )
-    header_buttons = context["header_buttons"]
-    header_buttons.append(
-        {
-            "type": "group",
-            "buttons": l1,
-            "icon": "fa fa-caret-down",
-            "text": "Related projects",
-        }
-    )
-    releases = version_info.minor_releases(first="0.8")
-    if outdated:
-        current = f"{long_version} (outdated)"
-        latest = "latest"
-        entries = [".".join(long_version.split(".")[:2])]
-    elif not releases:
-        current = "unknown"
-        latest = "unknown"
-        entries = []
-    else:
-        current = f"{long_version} (latest)"
-        latest = f"{releases[0]} (latest)"
-        entries = releases[1:]
-    lines = [{"type": "link", "text": latest, "url": f"{base}"}]
-    for r in entries:
-        lines.append({"type": "link", "text": f"{r}", "url": f"{base}/release/{r}"})
-    header_buttons.append(
-        {"type": "group", "buttons": lines, "icon": "fa fa-caret-down", "text": current}
-    )
-
-
-sphinx_book_theme.add_launch_buttons = add_buttons
+project = 'ScippUncertainty'
+copyright = '2024 Scipp contributors'
+author = 'Scipp contributors'
 
 html_show_sourcelink = True
 
-# -- General configuration ------------------------------------------------
+extensions = [
+    'sphinx.ext.autodoc',
+    'sphinx.ext.autosummary',
+    'sphinx.ext.doctest',
+    'sphinx.ext.githubpages',
+    'sphinx.ext.intersphinx',
+    'sphinx.ext.mathjax',
+    'sphinx.ext.napoleon',
+    'sphinxcontrib.bibtex',
+    'sphinx.ext.viewcode',
+    'sphinx_autodoc_typehints',
+    'sphinx_copybutton',
+    'sphinx_design',
+    'nbsphinx',
+    'myst_parser',
+]
 
-# If your documentation needs a minimal Sphinx version, state it here.
-#
-# needs_sphinx = '1.0'
+try:
+    import sciline.sphinxext.domain_types  # noqa: F401
 
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
-# ones.
-extensions = [
-    "sphinx.ext.autodoc",
-    "sphinx.ext.autosummary",
-    "sphinx.ext.doctest",
-    "sphinx.ext.intersphinx",
-    "sphinx.ext.mathjax",
-    "sphinx.ext.napoleon",
-    "sphinx.ext.viewcode",
-    "sphinxcontrib.bibtex",
-    "sphinx_autodoc_typehints",
-    "sphinx_copybutton",
-    "nbsphinx",
+    extensions.append('sciline.sphinxext.domain_types')
+except ModuleNotFoundError:
+    pass
+
+
+myst_enable_extensions = [
+    "amsmath",
+    "colon_fence",
+    "deflist",
+    "dollarmath",
+    "fieldlist",
+    "html_admonition",
+    "html_image",
+    "replacements",
+    "smartquotes",
+    "strikethrough",
+    "substitution",
+    "tasklist",
 ]
 
+myst_heading_anchors = 3
+
+autodoc_type_aliases = {
+    'array_like': 'array_like',
+}
+
 intersphinx_mapping = {
-    "numpy": ("https://numpy.org/doc/stable/", None),
-    "python": ("https://docs.python.org/3", None),
-    "scipp": ("https://scipp.github.io/", None),
+    'python': ('https://docs.python.org/3', None),
+    'numpy': ('https://numpy.org/doc/stable/', None),
+    'scipp': ('https://scipp.github.io/', None),
 }
 
 # autodocs includes everything, even irrelevant API internals. autosummary
 # looks more suitable in the long run when the API grows.
 # For a nice example see how xarray handles its API documentation.
 autosummary_generate = True
 
 napoleon_google_docstring = False
 napoleon_numpy_docstring = True
 napoleon_use_param = True
 napoleon_use_rtype = False
 napoleon_preprocess_types = True
-typehints_defaults = "comma"
+napoleon_type_aliases = {
+    # objects without namespace: numpy
+    "ndarray": "~numpy.ndarray",
+}
+typehints_defaults = 'comma'
 typehints_use_rtype = False
 
+
+sciline_domain_types_prefix = 'scippuncertainty'
+sciline_domain_types_aliases = {
+    'scipp._scipp.core.DataArray': 'scipp.DataArray',
+    'scipp._scipp.core.Dataset': 'scipp.Dataset',
+    'scipp._scipp.core.DType': 'scipp.DType',
+    'scipp._scipp.core.Unit': 'scipp.Unit',
+    'scipp._scipp.core.Variable': 'scipp.Variable',
+    'scipp.core.data_group.DataGroup': 'scipp.DataGroup',
+}
+
+
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
+templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
-# source_suffix = ['.rst', '.md']
-source_suffix = ".rst"
-html_sourcelink_suffix = ""  # Avoid .ipynb.txt extensions in sources
+source_suffix = ['.rst', '.md']
+html_sourcelink_suffix = ''  # Avoid .ipynb.txt extensions in sources
 
 # The master toctree document.
-master_doc = "index"
+master_doc = 'index'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-# The short X.Y version.
-version = scippuncertainty.__version__
-# The full version, including alpha/beta/rc tags.
-release = scippuncertainty.__version__
+
+release = get_version("scippuncertainty")
+version = ".".join(release.split('.')[:3])  # CalVer
 
 warning_is_error = True
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", "**.ipynb_checkpoints"]
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store', '**.ipynb_checkpoints']
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = "sphinx"
+pygments_style = 'sphinx'
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 # -- Options for HTML output ----------------------------------------------
-html_theme = "sphinx_book_theme"
+
+html_theme = "pydata_sphinx_theme"
 html_theme_options = {
-    "repository_url": f"https://github.com/scipp/{project}",
-    "repository_branch": "main",
-    "path_to_docs": "docs",
-    "use_repository_button": True,
-    "use_issues_button": True,
-    "use_edit_page_button": True,
-    "show_toc_level": 2,  # Show subheadings in secondary sidebar
+    "primary_sidebar_end": ["edit-this-page", "sourcelink"],
+    "secondary_sidebar_items": [],
+    "navbar_persistent": ["search-button"],
+    "show_nav_level": 1,
+    # Adjust this to ensure external links are moved to "Move" menu
+    "header_links_before_dropdown": 4,
+    "pygment_light_style": "github-light-high-contrast",
+    "pygment_dark_style": "github-dark-high-contrast",
+    "logo": {
+        "image_light": "_static/logo.svg",
+        "image_dark": "_static/logo-dark.svg",
+    },
+    "external_links": [
+        {"name": "Plopp", "url": "https://scipp.github.io/plopp"},
+        {"name": "Scipp", "url": "https://scipp.github.io"},
+    ],
+    "icon_links": [
+        {
+            "name": "GitHub",
+            "url": "https://github.com/scipp/scippuncertainty",
+            "icon": "fa-brands fa-github",
+            "type": "fontawesome",
+        },
+        {
+            "name": "PyPI",
+            "url": "https://pypi.org/project/scippuncertainty/",
+            "icon": "fa-brands fa-python",
+            "type": "fontawesome",
+        },
+        {
+            "name": "Conda",
+            "url": "https://anaconda.org/scipp/scippuncertainty",
+            "icon": "fa-custom fa-anaconda",
+            "type": "fontawesome",
+        },
+    ],
+    "footer_start": ["copyright", "sphinx-version"],
+    "footer_end": ["doc_version", "theme-version"],
+}
+html_context = {
+    "doc_path": "docs",
+}
+html_sidebars = {
+    "**": ["sidebar-nav-bs", "page-toc"],
 }
 
 html_title = "ScippUncertainty"
 html_logo = "_static/logo.svg"
 html_favicon = "_static/favicon.ico"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
+html_static_path = ['_static']
+html_css_files = []
+html_js_files = ["anaconda-icon.js"]
 
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = "scippuncertaintydoc"
+htmlhelp_basename = 'scippuncertaintydoc'
+
+# -- Options for Matplotlib in notebooks ----------------------------------
+
+nbsphinx_execute_arguments = [
+    "--Session.metadata=scipp_sphinx_build=True",
+]
 
 # -- Options for doctest --------------------------------------------------
 
 # sc.plot returns a Figure object and doctest compares that against the
 # output written in the docstring. But we only want to show an image of the
 # figure, not its `repr`.
 # In addition, there is no need to make plots in doctest as the documentation
 # build already tests if those plots can be made.
 # So we simply disable plots in doctests.
-doctest_global_setup = """
-"""
+doctest_global_setup = '''
+import numpy as np
+
+try:
+    import scipp as sc
+
+    def do_not_plot(*args, **kwargs):
+        pass
 
+    sc.plot = do_not_plot
+    sc.Variable.plot = do_not_plot
+    sc.DataArray.plot = do_not_plot
+    sc.DataGroup.plot = do_not_plot
+    sc.Dataset.plot = do_not_plot
+except ImportError:
+    # Scipp is not needed by docs if it is not installed.
+    pass
+'''
+
+# Using normalize whitespace because many __str__ functions in scipp produce
+# extraneous empty lines and it would look strange to include them in the docs.
 doctest_default_flags = (
     doctest.ELLIPSIS
     | doctest.IGNORE_EXCEPTION_DETAIL
     | doctest.DONT_ACCEPT_TRUE_FOR_1
     | doctest.NORMALIZE_WHITESPACE
 )
 
 # -- Options for linkcheck ------------------------------------------------
 
 linkcheck_ignore = [
-    # Specific lines in GitHub blobs cannot be found by linkcheck.
-    r"https?://github\.com/.*?/blob/[a-f0-9]+/.+?#",
+    # Specific lines in Github blobs cannot be found by linkcheck.
+    r'https?://github\.com/.*?/blob/[a-f0-9]+/.+?#',
+    # DOIs in the bibliography lead to redirects that linkcheck struggles with.
+    r"https?://doi\.org/.*",
 ]
 
 # -- Options for bibtex ---------------------------------------------------
 bibtex_bibfiles = ["bibliography.bib"]
 bibtex_reference_style = "label"
-
-# -- Options for Matplotlib in notebooks ----------------------------------
-
-nbsphinx_execute_arguments = [
-    "--Session.metadata=scipp_sphinx_build=True",
-]
```

### Comparing `scippuncertainty-23.3.0/docs/user-guide/mc.ipynb` & `scippuncertainty-24.5.0/docs/user-guide/mc.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966950860361147%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'This guide introduces the "*

 * *            '[mc](../api-reference/index.md#monte-carlo) sub package for propagation of '*

 * *            "uncertainties using Monte-Carlo.\\n')], delete: [2]}}, 1: {'source': {delete: [1, "*

 * *            "0]}}, 2: {'source': {insert: [(3, 'variances = rng.uniform(0.01, 0.05, n) ** 2\\n')], "*

 * *            "delete: [3]}}, 6: {'source': {insert: [(0, 'def compute_speed(pos: sc.DataArray, "*

 * *            "time: sc.DataArray) -> dict[str, sc.DataArra […]*

```diff
@@ -3,15 +3,15 @@
         {
             "cell_type": "markdown",
             "id": "56c96f55-5fd4-413a-a16c-3b32adbf8943",
             "metadata": {},
             "source": [
                 "# Monte-Carlo propagation of uncertainties\n",
                 "\n",
-                "This guide introduces the [mc](../reference/index.rst#monte-carlo) sub package for propagation of uncertainties using Monte-Carlo.\n",
+                "This guide introduces the [mc](../api-reference/index.md#monte-carlo) sub package for propagation of uncertainties using Monte-Carlo.\n",
                 "\n",
                 "Monte-Carlo (MC) can propagate uncertainties through most operations including non-differentiable ones and operations that introduce correlations.\n",
                 "It does so by sampling new data from an input with uncertainties, performing the desired operation on each sample, and combining the results to compute, e.g., a mean and variance.\n",
                 "While this method is powerful, it is very expensive and in practice only applicable to relatively small and well behaved data.\n",
                 "\n",
                 "Mathematically, the mc package does the following (the examples below will make the terminology more concrete).\n",
                 "\n",
@@ -40,16 +40,14 @@
             "execution_count": null,
             "id": "3b02603a-a0a8-4152-887e-016b9535fe34",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "from typing import Dict\n",
-                "\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import plopp as pp\n",
                 "import scipp as sc\n",
                 "\n",
                 "from scippuncertainty import mc\n",
                 "\n",
@@ -68,15 +66,15 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "rng = np.random.default_rng(381)\n",
                 "n = 10\n",
                 "x = sc.linspace(\"x\", 1, 2, n)\n",
-                "variances = rng.uniform(0.01, 0.05, n)**2\n",
+                "variances = rng.uniform(0.01, 0.05, n) ** 2\n",
                 "pos = sc.DataArray(\n",
                 "    sc.array(\n",
                 "        dims=[\"x\"],\n",
                 "        values=x.values + rng.normal(4.0, np.sqrt(variances)),\n",
                 "        variances=variances,\n",
                 "        unit=\"m\",\n",
                 "    ),\n",
@@ -123,17 +121,15 @@
             "execution_count": null,
             "id": "afe16c9b-04ce-4088-9f3d-f8d831d1b89d",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "def compute_speed(\n",
-                "    pos: sc.DataArray, time: sc.DataArray\n",
-                ") -> Dict[str, sc.DataArray]:\n",
+                "def compute_speed(pos: sc.DataArray, time: sc.DataArray) -> dict[str, sc.DataArray]:\n",
                 "    return {\"speed\": pos / time}"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3882f319-2e5c-4083-8272-dad8682d5e2c",
             "metadata": {},
@@ -252,16 +248,15 @@
             "execution_count": null,
             "id": "e7056e81-2da3-4a2f-bcf1-45cc969a2c4c",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "pp.plot({\"regular\": speed_regular, \"mc\": speed_mc},\n",
-                "        ls='-', marker=None)"
+                "pp.plot({\"regular\": speed_regular, \"mc\": speed_mc}, ls='-', marker=None)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "bbd6dc7f-2611-4922-a71e-f7dea2a8bc3e",
             "metadata": {},
             "source": [
@@ -374,15 +369,15 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "def compute_average_speed(\n",
                 "    pos: sc.DataArray, time: sc.DataArray\n",
-                ") -> Dict[str, sc.DataArray]:\n",
+                ") -> dict[str, sc.DataArray]:\n",
                 "    speed = pos / time\n",
                 "    return {\"speed\": speed, \"average_speed\": sc.mean(speed)}"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f140b3ce-7c20-4d1a-b164-c8bcf52cd45f",
@@ -500,16 +495,18 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "results = mc.run(\n",
                 "    compute_average_speed,\n",
                 "    samplers={\"pos\": pos_sampler, \"time\": time_sampler},\n",
-                "    accumulators={\"speed\": speed_accumulator,\n",
-                "                  \"average_speed\": average_speed_accumulator},\n",
+                "    accumulators={\n",
+                "        \"speed\": speed_accumulator,\n",
+                "        \"average_speed\": average_speed_accumulator,\n",
+                "    },\n",
                 "    n_samples=10_000,\n",
                 "    progress=False,\n",
                 ")\n",
                 "speed_mc = results[\"speed\"]\n",
                 "average_speed_mc = results[\"average_speed\"]"
             ]
         },
@@ -624,17 +621,15 @@
             "execution_count": null,
             "id": "4fd90b82-9ead-4d1f-9041-022bf302f95e",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "def compute_speed_cov(\n",
-                "    pos: sc.DataArray, time: sc.DataArray\n",
-                ") -> Dict[str, sc.DataArray]:\n",
+                "def compute_speed_cov(pos: sc.DataArray, time: sc.DataArray) -> dict[str, sc.DataArray]:\n",
                 "    speed = pos / time\n",
                 "    return {\"speed\": speed, \"speed_cov\": speed}"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "dce32218-55a5-49c5-9a36-08c311ad3b39",
@@ -651,16 +646,15 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "results = mc.run(\n",
                 "    compute_speed_cov,\n",
                 "    samplers={\"pos\": pos_sampler, \"time\": time_sampler},\n",
-                "    accumulators={\"speed\": variance_accumulator,\n",
-                "                  \"speed_cov\": covariance_accumulator},\n",
+                "    accumulators={\"speed\": variance_accumulator, \"speed_cov\": covariance_accumulator},\n",
                 "    n_samples=10_000,\n",
                 "    progress=False,\n",
                 ")\n",
                 "speed_mc = results[\"speed\"]\n",
                 "speed_cov = results[\"speed_cov\"]"
             ]
         },
@@ -782,16 +776,18 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "results = mc.run(\n",
                 "    compute_average_speed,\n",
                 "    samplers={\"pos\": pos_sampler, \"time\": time_sampler},\n",
-                "    accumulators={\"speed\": speed_accumulator,\n",
-                "                  \"average_speed\": average_speed_accumulator},\n",
+                "    accumulators={\n",
+                "        \"speed\": speed_accumulator,\n",
+                "        \"average_speed\": average_speed_accumulator,\n",
+                "    },\n",
                 "    n_samples=10,\n",
                 "    progress=False,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
@@ -826,28 +822,28 @@
             "execution_count": null,
             "id": "a70c97b9-a21d-40cb-82f2-2fd820a085c9",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "def skipping_op(da: sc.DataArray) -> Dict[str, sc.DataArray]:\n",
+                "def skipping_op(da: sc.DataArray) -> dict[str, sc.DataArray]:\n",
                 "    if sc.any(da < sc.scalar(0)).value:\n",
                 "        return mc.SkipSample\n",
                 "    return {\"sqrt\": sc.sqrt(da)}"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2e29ab4c-7aed-4ca7-80ce-79477b6bdb6d",
             "metadata": {},
             "source": [
-                "Note, though, failed samples still count towards `n_samples`.\n",
+                "Note, though, that failed samples still count towards the target `n_samples` passed to `mc.run`.\n",
                 "So the actual number of samples used for the output variance can be different.\n",
-                "To find out, look at the `\"n_samples\"'` attribute:"
+                "To find out, look at the `n_samples'` property:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f37ebb5e-dc14-4706-9fff-9e89b0446552",
             "metadata": {
@@ -870,15 +866,15 @@
                 "results = mc.run(\n",
                 "    skipping_op,\n",
                 "    samplers={\"da\": mc.NormalDenseSampler(da)},\n",
                 "    accumulators={\"sqrt\": mc.VarianceAccum()},\n",
                 "    n_samples=100,\n",
                 "    progress=False,\n",
                 ")\n",
-                "results[\"sqrt\"].attrs[\"n_samples\"]"
+                "results.n_samples"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -890,13 +886,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.8.17"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scippuncertainty-23.3.0/requirements/ci.txt` & `scippuncertainty-24.5.0/requirements/ci.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,56 @@
-# SHA1:0ec664e87e8dccff0900d55d3a102599a0d0d382
+# SHA1:6344d52635ea11dca331a3bc6eb1833c4c64d585
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-cachetools==5.3.0
+cachetools==5.3.3
     # via tox
-chardet==5.1.0
+certifi==2024.2.2
+    # via requests
+chardet==5.2.0
     # via tox
+charset-normalizer==3.3.2
+    # via requests
 colorama==0.4.6
     # via tox
-distlib==0.3.6
+distlib==0.3.8
     # via virtualenv
-filelock==3.10.0
+filelock==3.14.0
     # via
     #   tox
     #   virtualenv
-gitdb==4.0.10
+gitdb==4.0.11
     # via gitpython
-gitpython==3.1.31
-    # via -r requirements/ci.in
-packaging==23.0
+gitpython==3.1.43
+    # via -r ci.in
+idna==3.7
+    # via requests
+packaging==24.0
     # via
+    #   -r ci.in
     #   pyproject-api
     #   tox
-platformdirs==3.1.1
+platformdirs==4.2.2
     # via
     #   tox
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.5.0
     # via tox
-pyproject-api==1.5.1
+pyproject-api==1.6.1
     # via tox
-smmap==5.0.0
+requests==2.32.2
+    # via -r ci.in
+smmap==5.0.1
     # via gitdb
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.4.7
-    # via -r requirements/ci.in
-virtualenv==20.21.0
+tox==4.15.0
+    # via -r ci.in
+urllib3==2.2.1
+    # via requests
+virtualenv==20.26.2
     # via tox
```

### Comparing `scippuncertainty-23.3.0/requirements/docs.txt` & `scippuncertainty-24.5.0/requirements/docs.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,274 +1,274 @@
-# SHA1:0c6a913e6f2f58333f64363a4d6c3acd21181a1b
+# SHA1:8a21add67fd82f1b85b66f09e2c9b8f0eedeb643
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
-alabaster==0.7.13
+accessible-pygments==0.0.5
+    # via pydata-sphinx-theme
+alabaster==0.7.16
     # via sphinx
-asttokens==2.2.1
+asttokens==2.4.1
     # via stack-data
-attrs==22.2.0
-    # via jsonschema
-babel==2.12.1
-    # via sphinx
-backcall==0.2.0
-    # via ipython
-beautifulsoup4==4.11.2
+attrs==23.2.0
+    # via
+    #   jsonschema
+    #   referencing
+babel==2.15.0
+    # via
+    #   pydata-sphinx-theme
+    #   sphinx
+beautifulsoup4==4.12.3
     # via
     #   nbconvert
     #   pydata-sphinx-theme
-bleach==6.0.0
+bleach==6.1.0
     # via nbconvert
-certifi==2022.12.7
+certifi==2024.2.2
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.3.2
     # via requests
-comm==0.1.2
+comm==0.2.2
     # via ipykernel
-contourpy==1.0.7
+contourpy==1.2.1
     # via matplotlib
-cycler==0.11.0
+cycler==0.12.1
     # via matplotlib
-debugpy==1.6.6
+debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
-docutils==0.17.1
+docutils==0.21.2
     # via
+    #   myst-parser
     #   nbsphinx
     #   pybtex-docutils
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinxcontrib-bibtex
-executing==1.2.0
+exceptiongroup==1.2.1
+    # via ipython
+executing==2.0.1
     # via stack-data
-fastjsonschema==2.16.3
+fastjsonschema==2.19.1
     # via nbformat
-fonttools==4.39.2
+fonttools==4.52.1
     # via matplotlib
-gitdb==4.0.10
-    # via gitpython
-gitpython==3.1.31
-    # via -r requirements/docs.in
-idna==3.4
+idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.0.0
+ipykernel==6.29.4
+    # via -r docs.in
+ipython==8.24.0
     # via
-    #   jupyter-client
-    #   nbconvert
-    #   sphinx
-    #   sphinxcontrib-bibtex
-importlib-resources==5.12.0
-    # via matplotlib
-ipykernel==6.21.3
-    # via
-    #   -r requirements/docs.in
-    #   ipywidgets
-ipympl==0.9.3
-    # via -r requirements/docs.in
-ipython==8.11.0
-    # via
-    #   -r requirements/docs.in
+    #   -r docs.in
     #   ipykernel
-    #   ipympl
-    #   ipywidgets
-ipython-genutils==0.2.0
-    # via ipympl
-ipywidgets==8.0.4
-    # via
-    #   -r requirements/docs.in
-    #   ipympl
-jedi==0.18.2
+jedi==0.19.1
     # via ipython
-jinja2==3.1.2
+jinja2==3.1.4
     # via
+    #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
-jsonschema==4.17.3
+jsonschema==4.22.0
     # via nbformat
-jupyter-client==8.0.3
+jsonschema-specifications==2023.12.1
+    # via jsonschema
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.3.0
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbconvert
     #   nbformat
-jupyterlab-pygments==0.2.2
+jupyterlab-pygments==0.3.0
     # via nbconvert
-jupyterlab-widgets==3.0.5
-    # via ipywidgets
-kiwisolver==1.4.4
+kiwisolver==1.4.5
     # via matplotlib
-latexcodec==2.0.1
+latexcodec==3.0.0
     # via pybtex
-markupsafe==2.1.2
+markdown-it-py==3.0.0
+    # via
+    #   mdit-py-plugins
+    #   myst-parser
+markupsafe==2.1.5
     # via
     #   jinja2
     #   nbconvert
-matplotlib==3.7.1
-    # via
-    #   -r requirements/docs.in
-    #   ipympl
-    #   plopp
-matplotlib-inline==0.1.6
+matplotlib==3.9.0
+    # via plopp
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mistune==2.0.5
+mdit-py-plugins==0.4.1
+    # via myst-parser
+mdurl==0.1.2
+    # via markdown-it-py
+mistune==3.0.2
     # via nbconvert
-nbclient==0.7.2
+myst-parser==3.0.1
+    # via -r docs.in
+nbclient==0.10.0
     # via nbconvert
-nbconvert==7.2.10
+nbconvert==7.16.4
     # via nbsphinx
-nbformat==5.7.3
+nbformat==5.10.4
     # via
     #   nbclient
     #   nbconvert
     #   nbsphinx
-nbsphinx==0.9.1
-    # via -r requirements/docs.in
-nest-asyncio==1.5.6
+nbsphinx==0.9.4
+    # via -r docs.in
+nest-asyncio==1.6.0
     # via ipykernel
-packaging==23.0
+packaging==24.0
     # via
     #   ipykernel
     #   matplotlib
     #   nbconvert
     #   pydata-sphinx-theme
     #   sphinx
-pandocfilters==1.5.0
+pandocfilters==1.5.1
     # via nbconvert
-parso==0.8.3
+parso==0.8.4
     # via jedi
-pexpect==4.8.0
-    # via ipython
-pickleshare==0.7.5
+pexpect==4.9.0
     # via ipython
-pillow==9.4.0
-    # via
-    #   ipympl
-    #   matplotlib
-platformdirs==3.1.1
+pillow==10.3.0
+    # via matplotlib
+platformdirs==4.2.2
     # via jupyter-core
-plopp==23.3.0
-    # via -r requirements/docs.in
-prompt-toolkit==3.0.38
+plopp==24.5.0
+    # via -r docs.in
+prompt-toolkit==3.0.43
     # via ipython
-psutil==5.9.4
+psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
     # via
     #   pybtex-docutils
     #   sphinxcontrib-bibtex
-pybtex-docutils==1.0.2
+pybtex-docutils==1.0.3
     # via sphinxcontrib-bibtex
-pydata-sphinx-theme==0.8.1
-    # via sphinx-book-theme
-pyparsing==3.0.9
+pydata-sphinx-theme==0.15.2
+    # via -r docs.in
+pygments==2.18.0
+    # via
+    #   accessible-pygments
+    #   ipython
+    #   nbconvert
+    #   pydata-sphinx-theme
+    #   sphinx
+pyparsing==3.1.2
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   jupyter-client
     #   matplotlib
-pyzmq==25.0.1
+pyyaml==6.0.1
+    # via
+    #   myst-parser
+    #   pybtex
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
-requests==2.28.2
+referencing==0.35.1
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+requests==2.32.2
     # via sphinx
+rpds-py==0.18.1
+    # via
+    #   jsonschema
+    #   referencing
 six==1.16.0
     # via
     #   asttokens
     #   bleach
-    #   latexcodec
     #   pybtex
     #   python-dateutil
-smmap==5.0.0
-    # via gitdb
 snowballstemmer==2.2.0
     # via sphinx
-soupsieve==2.4
+soupsieve==2.5
     # via beautifulsoup4
-sphinx==4.5.0
+sphinx==7.3.7
     # via
-    #   -r requirements/docs.in
+    #   -r docs.in
+    #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
-    #   sphinx-book-theme
     #   sphinx-copybutton
+    #   sphinx-design
     #   sphinxcontrib-bibtex
-sphinx-autodoc-typehints==1.18.3
-    # via -r requirements/docs.in
-sphinx-book-theme==0.3.3
-    # via -r requirements/docs.in
-sphinx-copybutton==0.5.1
-    # via -r requirements/docs.in
-sphinxcontrib-applehelp==1.0.4
-    # via sphinx
-sphinxcontrib-bibtex==2.5.0
-    # via -r requirements/docs.in
-sphinxcontrib-devhelp==1.0.2
+sphinx-autodoc-typehints==2.1.0
+    # via -r docs.in
+sphinx-copybutton==0.5.2
+    # via -r docs.in
+sphinx-design==0.6.0
+    # via -r docs.in
+sphinxcontrib-applehelp==1.0.8
+    # via sphinx
+sphinxcontrib-bibtex==2.6.2
+    # via -r docs.in
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-stack-data==0.6.2
+stack-data==0.6.3
     # via ipython
-tinycss2==1.2.1
+tinycss2==1.3.0
     # via nbconvert
-tornado==6.2
+tomli==2.0.1
+    # via sphinx
+tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-traitlets==5.9.0
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
-    #   ipympl
     #   ipython
-    #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbconvert
     #   nbformat
     #   nbsphinx
-urllib3==1.26.15
+typing-extensions==4.12.0
+    # via
+    #   ipython
+    #   pydata-sphinx-theme
+urllib3==2.2.1
     # via requests
-wcwidth==0.2.6
+wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-widgetsnbextension==4.0.5
-    # via ipywidgets
-zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
```

### Comparing `scippuncertainty-23.3.0/resources/logo-2023.svg` & `scippuncertainty-24.5.0/resources/logo-2023.svg`

 * *Files identical despite different names*

### Comparing `scippuncertainty-23.3.0/src/scippuncertainty/_progress.py` & `scippuncertainty-24.5.0/src/scippuncertainty/_progress.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """Progress bars."""
 
+from collections.abc import Iterable, Iterator, Sequence
 from contextlib import contextmanager
 from typing import (
     Any,
-    Iterable,
-    Iterator,
-    List,
-    Optional,
     Protocol,
-    Sequence,
     TypeVar,
-    Union,
 )
 
 ProgressType = TypeVar("ProgressType")
 
 
 class Progress(Protocol):
     """Progress bar to track iteration over a sequence.
 
     Only works if the display has been initialized with ``MultiProgress.prepare``.
     """
 
     def track(
         self,
-        sequence: Union[Iterable[ProgressType], Sequence[ProgressType]],
+        sequence: Iterable[ProgressType] | Sequence[ProgressType],
         description: str,
-        total: Optional[float] = None,
+        total: float | None = None,
     ) -> Iterable[ProgressType]:
         """Display and update a progress bar based on the provided sequence.
 
         Parameters
         ----------
         sequence:
             Iterable to iterate over and track progress.
@@ -49,17 +44,17 @@
 
 
 class SilentProgress:
     """'Progress bar' that shows nothing."""
 
     @staticmethod
     def track(
-        sequence: Union[Iterable[ProgressType], Sequence[ProgressType]],
+        sequence: Iterable[ProgressType] | Sequence[ProgressType],
         description: str,
-        total: Optional[float] = None,
+        total: float | None = None,
     ) -> Iterable[ProgressType]:
         """Return the input sequence.
 
         Parameters
         ----------
         sequence:
             Iterable to iterate over and track progress.
@@ -95,17 +90,17 @@
             TextColumn("ETA:"),
             TimeRemainingColumn(),
             refresh_per_second=1,
         )
 
     def track(
         self,
-        sequence: Union[Iterable[ProgressType], Sequence[ProgressType]],
+        sequence: Iterable[ProgressType] | Sequence[ProgressType],
         description: str,
-        total: Optional[float] = None,
+        total: float | None = None,
     ) -> Iterable[ProgressType]:
         """Display and update a progress bar based on the provided sequence.
 
         Parameters
         ----------
         sequence:
             Iterable to iterate over and track progress.
@@ -128,35 +123,35 @@
         return self._progress
 
 
 class MultiProgress(Protocol):
     """Manager for multiple progress bars."""
 
     @contextmanager
-    def prepare(self, n: int) -> Iterator[List[Progress]]:
+    def prepare(self, n: int) -> Iterator[list[Progress]]:
         """Create individual progress bars and set up display.
 
         The bars may only be used while this contextmanager is active.
         """
 
 
 class SilentMultiProgress:
     """Manager for multiple silent progress bars."""
 
     @contextmanager
-    def prepare(self, n: int) -> Iterator[List[Progress]]:
+    def prepare(self, n: int) -> Iterator[list[Progress]]:
         """Create individual silent progress bars and set up display."""
         yield [SilentProgress() for _ in range(n)]
 
 
 class RichMultiProgress:
     """Manager for multiple rich progress bars."""
 
     @contextmanager
-    def prepare(self, n: int) -> Iterator[List[Progress]]:
+    def prepare(self, n: int) -> Iterator[list[Progress]]:
         """Create individual rich progress bars and set up display.
 
         The bars may only be used while this contextmanager is active.
         """
         from rich.console import Group
         from rich.live import Live
 
@@ -169,15 +164,15 @@
     try:
         import rich  # noqa: F401
     except ImportError:
         return False
     return True
 
 
-def progress_bars(visible: Optional[bool]) -> MultiProgress:
+def progress_bars(visible: bool | None) -> MultiProgress:
     """Construct a multi progress bar.
 
     Parameters
     ----------
     visible:
         - If ``None``, pick an implementation automatically.
         - If ``True``, use ``RichMultiProgress``,
```

### Comparing `scippuncertainty-23.3.0/src/scippuncertainty/correlation.py` & `scippuncertainty-24.5.0/src/scippuncertainty/correlation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """Computing correlations."""
 
-from typing import TypeVar, Union
+from typing import TypeVar
 
 import numpy as np
 import scipp as sc
 
-T = TypeVar("T", bound=Union[sc.Variable, sc.DataArray])
+T = TypeVar("T", bound=sc.Variable | sc.DataArray)
 
 
 def pearson_correlation(cov: T) -> T:
     r"""Compute the Pearson correlation coefficient from a covariance matrix.
 
     The Pearson correlation coefficient is a measure of linear correlation.
     Given a variance-covariance matrix :math:`\Sigma`, it is ddefined as:
```

### Comparing `scippuncertainty-23.3.0/src/scippuncertainty/mc/__init__.py` & `scippuncertainty-24.5.0/src/scippuncertainty/mc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """Monte-Carlo uncertainty propagation."""
 
 from .accumulator import Accumulator, CovarianceAccum, VarianceAccum
-from .driver import (
-    SkipSample,
-    resample,
-    resample_n,
-    run,  # noqa: F401
-)
+from .driver import run  # noqa: F401
+from .driver import SkipSample, resample, resample_n
 from .sampler import NormalDenseSampler, PoissonDenseSampler, Sampler
 
 __all__ = [
     "resample",
     "resample_n",
     "Accumulator",
     "CovarianceAccum",
```

### Comparing `scippuncertainty-23.3.0/src/scippuncertainty/mc/accumulator.py` & `scippuncertainty-24.5.0/src/scippuncertainty/mc/accumulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """Compute desired statistics on processed data."""
+
 from __future__ import annotations
 
-from typing import List, Optional, Protocol, Tuple, TypeVar, Union
+from dataclasses import dataclass
+from typing import Protocol, TypeVar
 
 import scipp as sc
 
 A = TypeVar("A", bound="Accumulator")
 
 
+@dataclass(frozen=True)
+class Accumulated:
+    """Accumulated data and metadata."""
+
+    data: sc.DataArray
+    n_samples: int
+    samples: tuple[sc.DataArray, ...] | None = None
+
+
 class Accumulator(Protocol):
     """Compute statistics on bootstrap results."""
 
     def add(self, sample: sc.DataArray) -> None:
         """Register a single sample."""
 
     def add_from(self: A, other: A) -> None:
         """Merge results from ``other`` into ``self``."""
 
-    def get(self) -> sc.DataArray:
+    def get(self) -> Accumulated:
         """Return the current result."""
 
     def new(self: A) -> A:
         """Return a new accumulator of the same type as ``self``.
 
         The new instance does not contain any samples even if ``self`` does.
         """
@@ -57,18 +68,18 @@
 
         Parameters
         ----------
         keep_samples:
             If ``True``, all samples are kept and returned as an attribute called
             ``samples`` with dimension ``monte_carlo``.
         """
-        self._mean: Optional[sc.DataArray] = None
-        self._m2_dist: Optional[sc.Variable] = None
+        self._mean: sc.DataArray | None = None
+        self._m2_dist: sc.Variable | None = None
         self._n_samples = 0
-        self._samples: Optional[List[sc.DataArray]] = [] if keep_samples else None
+        self._samples: list[sc.DataArray] | None = [] if keep_samples else None
 
     def add(self, sample: sc.DataArray) -> None:
         """Register a single sample."""
         self._n_samples += 1
         if self._mean is None:
             self._mean = sample.copy()
             self._m2_dist = sc.zeros(sizes=sample.sizes, unit=sample.unit**2)
@@ -101,27 +112,29 @@
         self._n_samples += other._n_samples
 
         if (self._samples is None) ^ (other._samples is None):
             raise RuntimeError("Both accumulators must have values")
         if self._samples is not None:
             self._samples.extend(other._samples)
 
-    def get(self) -> sc.DataArray:
+    def get(self) -> Accumulated:
         """Return the current result."""
         if self._n_samples == 0:
             raise RuntimeError("There are no results to get.")
         mean = self._mean
         var = self._m2_dist / (self._n_samples - 1)
 
         res = mean
         res.variances = var.values
-        res.attrs["n_samples"] = sc.index(self._n_samples)
-        if self._samples is not None:
-            res.attrs["samples"] = sc.index(sc.concat(self._samples, "monte_carlo"))
-        return res
+
+        return Accumulated(
+            data=res,
+            n_samples=self._n_samples,
+            samples=tuple(self._samples) if self._samples is not None else None,
+        )
 
     def new(self) -> VarianceAccum:
         """Return a new VarianceAccum.
 
         The new instance does not contain any samples even if ``self`` does.
         """
         return VarianceAccum(keep_samples=self._samples is not None)
@@ -152,17 +165,15 @@
     (except for an attribute ``n-samples``).
     """
 
     # See also the article on Wikipedia for an overview:
     # https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance#Covariance
     # In particular the 'Online' section.
 
-    def __init__(
-        self, *, dims: Optional[Union[List[str], Tuple[str, str]]] = None
-    ) -> None:
+    def __init__(self, *, dims: list[str] | tuple[str, str] | None = None) -> None:
         """Initialize a CovarianceAccum instance.
 
         Parameters
         ----------
         dims:
             Dimension names for the covariance matrix.
             Must be length-2.
@@ -177,16 +188,14 @@
         if sample.ndim != 1:
             raise sc.DimensionError("Can only handle 1-d values")
         sample = sample.rename({sample.dims[0]: self._dims[0]})
         for key in list(sample.coords):
             del sample.coords[key]
         for key in list(sample.masks):
             del sample.masks[key]
-        for key in list(sample.attrs):
-            del sample.attrs[key]
 
         self._n_samples += 1
         if self._mean is None:
             self._mean = sample.copy()
             self._c = sc.zeros(
                 sizes={self._dims[0]: sample.shape[0], self._dims[1]: sample.shape[0]},
                 unit=sample.unit**2,
@@ -208,29 +217,30 @@
                 self._mean - other._mean
             ) * (self._mean - other._mean).rename({self._dims[0]: self._dims[1]})
             self._mean = self._mean * (self._n_samples / n) + other._mean * (
                 other._n_samples / n
             )
         self._n_samples += other._n_samples
 
-    def get(self) -> sc.DataArray:
+    def get(self) -> Accumulated:
         """Return the current result."""
         if self._n_samples == 0:
             raise RuntimeError("There are no results to get.")
         cov = self._c / (self._n_samples - 1)
         if isinstance(cov, sc.Variable):
             # This happens when there is only 1 sample.
             cov = sc.DataArray(
                 cov,
                 coords=self._mean.coords,
-                attrs=self._mean.attrs,
                 masks=self._mean.masks,
             )
-        cov.attrs["n_samples"] = sc.index(self._n_samples)
-        return cov
+        return Accumulated(
+            data=cov,
+            n_samples=self._n_samples,
+        )
 
     def new(self) -> CovarianceAccum:
         """Return a new CovarianceAccum.
 
         The new instance does not contain any samples even if ``self`` does.
         """
         return CovarianceAccum(dims=self._dims)
```

### Comparing `scippuncertainty-23.3.0/src/scippuncertainty/mc/driver.py` & `scippuncertainty-24.5.0/src/scippuncertainty/mc/driver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,101 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """Control bootstrap resampling."""
+
 from __future__ import annotations
 
+from collections.abc import Callable, Generator, Mapping
 from concurrent.futures import ThreadPoolExecutor
 from itertools import islice
-from typing import Callable, Dict, Generator, List, Optional, Union
 
 import numpy as np
 import scipp as sc
 
 from .._progress import Progress, SilentProgress, progress_bars
 from .._util import distribute_evenly
 from ..random import make_rngs
-from .accumulator import Accumulator
+from .accumulator import Accumulated, Accumulator
 from .sampler import Sampler
 
 
-def _n_samples_per_thread(n_samples: int, n_thread: int) -> List[int]:
+class MCResult(dict):
+    """Result of a Monte-Carlo error estimation.
+
+    Behaves like a :class:`dict` of strings to data arrays but has additional properties
+    that encode the number of samples that were computed and lists of those samples.
+    """
+
+    def __init__(
+        self,
+        *,
+        data: dict[str, sc.DataArray],
+        n_samples: int,
+        samples: dict[str, tuple[sc.DataArray, ...] | None],
+    ) -> None:
+        super().__init__(data)
+        self._n_samples = n_samples
+        self._samples = samples
+
+    @classmethod
+    def assemble(cls, results: dict[str, Accumulated]) -> MCResult:
+        """Instantiate from results of individual accumulators."""
+        n_samples = {val.n_samples for val in results.values()}
+        if len(n_samples) != 1:
+            raise RuntimeError(
+                "Accumulators returned different numbers of samples. "
+                "This is either an internal bug or you started with "
+                "accumulators that already contained samples."
+            )
+
+        data = {key: val.data for key, val in results.items()}
+        samples = {key: val.samples for key, val in results.items()}
+        return MCResult(data=data, n_samples=next(iter(n_samples)), samples=samples)
+
+    def __setitem__(self, key: str, val: sc.DataArray) -> None:
+        """Setting items is not allowed."""
+        raise TypeError("MCResult is immutable")
+
+    @property
+    def n_samples(self) -> int:
+        """Number of samples."""
+        return self._n_samples
+
+    @property
+    def samples(self) -> Mapping[str, tuple[sc.DataArray, ...] | None]:
+        """Recorded samples for each accumulator."""
+        return self._samples
+
+
+def _n_samples_per_thread(n_samples: int, n_thread: int) -> list[int]:
     return distribute_evenly(n_samples, n_thread)
 
 
 def _resample_once(
-    samplers: Dict[str, Sampler], rng: np.random.Generator
-) -> Dict[str, sc.DataArray]:
+    samplers: dict[str, Sampler], rng: np.random.Generator
+) -> dict[str, sc.DataArray]:
     return {key: sampler.sample_once(rng) for key, sampler in samplers.items()}
 
 
 def resample(
-    *, samplers: Dict[str, Sampler], rng: np.random.Generator
-) -> Generator[Dict[str, sc.DataArray], None, None]:
+    *, samplers: dict[str, Sampler], rng: np.random.Generator
+) -> Generator[dict[str, sc.DataArray], None, None]:
     """Draw samples from given samplers forever."""
     while True:
         yield _resample_once(samplers, rng)
 
 
 def resample_n(
     *,
-    samplers: Dict[str, Sampler],
+    samplers: dict[str, Sampler],
     rng: np.random.Generator,
     n: int,
-    progress: Optional[Progress] = None,
+    progress: Progress | None = None,
     description: str = "Monte-Carlo",
-) -> Generator[Dict[str, sc.DataArray], None, None]:
+) -> Generator[dict[str, sc.DataArray], None, None]:
     """Draw n samples.
 
     Passes the RNG to samplers in the following order:
 
     .. code:: python
 
         for _ in range(n):
@@ -77,32 +126,29 @@
         islice(resample(samplers=samplers, rng=rng), n),
         total=n,
         description=description,
     )
 
 
 def run(
-    fn: Callable[..., Union[Dict[str, sc.DataArray], SkipSampleType]],
+    fn: Callable[..., dict[str, sc.DataArray] | SkipSampleType],
     *,
     n_samples: int,
-    samplers: Dict[str, Sampler],
-    accumulators: Optional[Dict[str, Accumulator]] = None,
+    samplers: dict[str, Sampler],
+    accumulators: dict[str, Accumulator] | None = None,
     n_threads: int = 1,
-    seed: Optional[
-        Union[
-            np.random.Generator,
-            List[np.random.Generator],
-            int,
-            List[int],
-            np.random.SeedSequence,
-        ]
-    ] = None,
-    progress: Optional[bool] = None,
+    seed: np.random.Generator
+    | list[np.random.Generator]
+    | int
+    | list[int]
+    | np.random.SeedSequence
+    | None = None,
+    progress: bool | None = None,
     description: str = "Monte-Carlo",
-) -> Dict[str, sc.DataArray]:
+) -> MCResult:
     """Propagate uncertainties using Monte-Carlo.
 
     This function drives the propagation by drawing samples, calling the provided
     function on each, anc accumulating the results.
 
     Parameters
     ----------
@@ -143,40 +189,47 @@
         It contains one item per accumulator with the same key.
     """
     rngs = make_rngs(seed=seed, n=n_threads)
     results = []
     with progress_bars(visible=progress).prepare(len(rngs)) as p_bars:
         with ThreadPoolExecutor(max_workers=len(rngs)) as executor:
             for i, (rng, n_thread_samples, progress_bar) in enumerate(
-                zip(rngs, _n_samples_per_thread(n_samples, len(rngs)), p_bars)
+                zip(
+                    rngs,
+                    _n_samples_per_thread(n_samples, len(rngs)),
+                    p_bars,
+                    strict=True,
+                )
             ):
                 job = _Job(
                     id_=i,
                     base_samplers=samplers,
                     base_accumulators=accumulators,
                     rng=rng,
                     progress_bar=progress_bar,
                     description=description,
                 )
                 results.append(executor.submit(job, fn, n_samples=n_thread_samples))
 
     accumulators = results[0].result()
     for res in results[1:]:
-        for a, b in zip(accumulators.values(), res.result().values()):
+        for a, b in zip(accumulators.values(), res.result().values(), strict=True):
             a.add_from(b)
-    return {name: accum.get() for name, accum in accumulators.items()}
+    return MCResult.assemble(
+        {name: accum.get() for name, accum in accumulators.items()}
+    )
 
 
 class _Job:
     def __init__(
         self,
         *,
         id_: int,
-        base_samplers: Dict[str, Sampler],
-        base_accumulators: Dict[str, Accumulator],
+        base_samplers: dict[str, Sampler],
+        base_accumulators: dict[str, Accumulator],
         rng: np.random.Generator,
         progress_bar: Progress,
         description: str,
     ) -> None:
         self._id = id_
         self._samplers = {
             key: sampler.clone() for key, sampler in base_samplers.items()
@@ -186,18 +239,18 @@
         }
         self._rng = rng
         self._progress_bar = progress_bar
         self._description = description + f"[{self._id}]"
 
     def __call__(
         self,
-        fn: Callable[..., Union[Dict[str, sc.DataArray], SkipSampleType]],
+        fn: Callable[..., dict[str, sc.DataArray] | SkipSampleType],
         *,
         n_samples: int,
-    ) -> Dict[str, Accumulator]:
+    ) -> dict[str, Accumulator]:
         for inputs in resample_n(
             samplers=self._samplers,
             rng=self._rng,
             n=n_samples,
             progress=self._progress_bar,
             description=self._description,
         ):
```

### Comparing `scippuncertainty-23.3.0/src/scippuncertainty/mc/sampler.py` & `scippuncertainty-24.5.0/src/scippuncertainty/mc/sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """Data (re-)sampling."""
+
 from __future__ import annotations
 
 from typing import Protocol, TypeVar
 
 import numpy as np
 import scipp as sc
```

### Comparing `scippuncertainty-23.3.0/src/scippuncertainty/random.py` & `scippuncertainty-24.5.0/src/scippuncertainty/random.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """Random number generators."""
 
-from typing import List, Optional, Union
-
 import numpy as np
 
 from .logging import get_logger
 
 
 def make_rngs(
-    seed: Optional[
-        Union[
-            np.random.Generator,
-            List[np.random.Generator],
-            int,
-            List[int],
-            np.random.SeedSequence,
-        ]
-    ],
+    seed: np.random.Generator
+    | list[np.random.Generator]
+    | int
+    | list[int]
+    | np.random.SeedSequence
+    | None,
     *,
     n: int,
-) -> List[np.random.Generator]:
+) -> list[np.random.Generator]:
     """Instantiate new random number generators.
 
     Creates the given number of random generators using
     :func:`numpy.random.default_rng` with :class:`numpy.random.SeedSequence`.
     ``n`` separate seed sequences are spawned from ``seed`` and generators constructed
     from those.
     These generators are independent with high probability which makes them
@@ -78,14 +73,14 @@
         rngs[0],
         np.__version__,
     )
     return rngs
 
 
 def _make_seed_sequence(
-    seed: Optional[Union[int, List[int], np.random.SeedSequence]]
+    seed: int | list[int] | np.random.SeedSequence | None,
 ) -> np.random.SeedSequence:
     if seed is None:
         return np.random.SeedSequence()
     if not isinstance(seed, np.random.SeedSequence):
         return np.random.SeedSequence(seed)
     return seed
```

### Comparing `scippuncertainty-23.3.0/tests/correlation_test.py` & `scippuncertainty-24.5.0/tests/correlation_test.py`

 * *Files identical despite different names*

### Comparing `scippuncertainty-23.3.0/tests/mc/accumulator_test.py` & `scippuncertainty-24.5.0/tests/mc/accumulator_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import numpy as np
 import pytest
 import scipp as sc
+import scipp.testing
 
 from scippuncertainty.mc import CovarianceAccum, VarianceAccum
 
 
 def test_variance_accum_returns_single_sample():
     da = sc.DataArray(
         sc.arange("w", 6.0, unit="kg"), coords={"h": sc.arange("w", 6) * 0.1}
     )
     accum = VarianceAccum()
     accum.add(da)
 
     res = accum.get()
-    assert sc.identical(sc.values(res.data), da.data)
-    assert sc.identical(sc.values(res.coords["h"]), da.coords["h"])
+    data, n_samples = res.data, res.n_samples
+
+    assert n_samples == 1
+    assert sc.identical(sc.values(data.data), da.data)
+    assert sc.identical(sc.values(data.coords["h"]), da.coords["h"])
     # Cannot have variances with one sample
-    assert sc.all(sc.isnan(sc.variances(res.data)))
+    assert sc.all(sc.isnan(sc.variances(data.data)))
 
 
 def test_variance_accum_returns_expected_result():
     rng = np.random.default_rng(912)
     da = sc.DataArray(
         sc.array(dims=["observation", "p"], values=rng.normal(0.0, 1.0, (15, 7)))
     )
 
     accum = VarianceAccum()
     for i in range(15):
         accum.add(da["observation", i])
 
-    res = accum.get()
+    res = accum.get().data
     np.testing.assert_allclose(res.values, sc.mean(da, dim="observation").values)
     np.testing.assert_allclose(res.variances, np.var(da.values, axis=0, ddof=1))
 
 
 def test_variance_accum_returns_expected_result_2d():
     rng = np.random.default_rng(8341)
     da = sc.DataArray(
@@ -45,72 +49,89 @@
         )
     )
 
     accum = VarianceAccum()
     for i in range(11):
         accum.add(da["observation", i])
 
-    res = accum.get()
+    res = accum.get().data
     np.testing.assert_allclose(res.values, sc.mean(da, dim="observation").values)
     np.testing.assert_allclose(res.variances, np.var(da.values, axis=0, ddof=1))
 
 
 def test_variance_accum_returns_number_of_samples():
     da = sc.DataArray(
         sc.arange("u", 3.0, unit="s"), coords={"o": sc.arange("u", 3) * 0.1}
     )
     accum = VarianceAccum()
     accum.add(da)
     accum.add(da)
     accum.add(da)
     accum.add(da)
 
-    res = accum.get()
-    assert sc.identical(res.attrs["n_samples"], sc.index(4))
+    assert accum.get().n_samples == 4
 
 
 def test_variance_accum_can_return_samples():
     da = sc.DataArray(
         sc.arange("u", 3.0, unit="s"), coords={"o": sc.arange("u", 3) * 0.1}
     )
-    expected = sc.concat([da, 2 * da], "monte_carlo")
+    expected0 = da.copy()
+    expected1 = 2 * da.copy()
 
     accum = VarianceAccum(keep_samples=True)
     accum.add(da)
     da *= 2  # doing in-place modification to test copy behavior
     accum.add(da)
 
-    res = accum.get()
-    assert sc.identical(res.attrs["samples"].value, expected)
+    samples = accum.get().samples
+    assert len(samples) == 2
+    sc.testing.assert_identical(samples[0], expected0)
+    sc.testing.assert_identical(samples[1], expected1)
+
+
+def test_variance_accum_does_not_return_samples_if_disabled():
+    da = sc.DataArray(
+        sc.arange("u", 3.0, unit="s"), coords={"o": sc.arange("u", 3) * 0.1}
+    )
+
+    accum = VarianceAccum(keep_samples=False)
+    accum.add(da)
+    da *= 2  # doing in-place modification to test copy behavior
+    accum.add(da)
+
+    assert accum.get().samples is None
 
 
 def test_variance_accum_preserves_metadata():
     rng = np.random.default_rng(83)
     da = sc.DataArray(
         sc.array(dims=["variable", "observation"], values=rng.normal(0.0, 1.0, (9, 2))),
-        coords={"x": sc.arange("variable", 9, unit="kg")},
+        coords={
+            "x": sc.arange("variable", 9, unit="kg"),
+            "y": -sc.arange("variable", 9),
+        },
         masks={"m": sc.arange("variable", 9) < 7},
-        attrs={"a": sc.index(4), "b": sc.scalar("a string")},
     )
+    da.coords.set_aligned("y", aligned=False)
 
     accum = VarianceAccum()
     accum.add(da["observation", 0])
     accum.add(da["observation", 1])
-    res = accum.get()
+    res = accum.get().data
 
-    assert set(res.coords.keys()) == {"x"}
+    assert set(res.coords.keys()) == {"x", "y"}
     assert sc.identical(res.coords["x"], sc.arange("variable", 9, unit="kg"))
+    assert sc.identical(res.coords["y"], -sc.arange("variable", 9))
+    assert res.coords["x"].aligned
+    assert not res.coords["y"].aligned
 
     assert set(res.masks.keys()) == {"m"}
     assert sc.identical(res.masks["m"], sc.arange("variable", 9) < 7)
 
-    assert set(res.attrs.keys()) == {"a", "b", "n_samples"}
-    assert sc.identical(res.attrs["a"], sc.index(4))
-    assert sc.identical(res.attrs["b"], sc.scalar("a string"))
-
 
 def test_variance_accum_add_from():
     rng = np.random.default_rng(83)
     da = sc.DataArray(
         sc.array(dims=["observation", "variable"], values=rng.normal(0.0, 1.0, (14, 8)))
     )
     chunk0 = da["observation", :5]
@@ -130,16 +151,16 @@
         accum1.add(chunk1["observation", i])
     for i in range(7):
         accum2.add(chunk2["observation", i])
 
     accum0.add_from(accum1)
     accum0.add_from(accum2)
 
-    a = accum0.get()
-    b = accum_total.get()
+    a = accum0.get().data
+    b = accum_total.get().data
     np.testing.assert_allclose(a.values, b.values)
     np.testing.assert_allclose(a.variances, b.variances)
 
 
 def test_variance_accum_new_does_not_return_stored_samples():
     da = sc.DataArray(
         sc.arange("u", 3.0, unit="s"), coords={"o": sc.arange("u", 3) * 0.1}
@@ -149,87 +170,85 @@
     accum.add(da)
 
     new = accum.new()
     with pytest.raises(RuntimeError):
         new.get()  # has no samples to get
 
 
-@pytest.mark.parametrize("keep_samples", (True, False))
+@pytest.mark.parametrize("keep_samples", [True, False])
 def test_variance_accum_new_passes_keep_samples_along(keep_samples):
     da = sc.DataArray(
         sc.arange("u", 3.0, unit="s"), coords={"o": sc.arange("u", 3) * 0.1}
     )
 
     accum = VarianceAccum(keep_samples=keep_samples)
     new = accum.new()
     new.add(da)
 
-    assert ("samples" in new.get().attrs) == keep_samples
+    assert (new.get().samples is not None) == keep_samples
 
 
 def test_covariance_accum_returns_expected_result():
     rng = np.random.default_rng(512)
     da = sc.DataArray(
         sc.array(dims=["variable", "observation"], values=rng.normal(0.0, 1.0, (5, 19)))
     )
 
     accum = CovarianceAccum()
     for i in range(19):
         accum.add(da["observation", i])
 
-    res = accum.get()
+    res = accum.get().data
     expected = np.cov(da.values)
     np.testing.assert_allclose(res.values, expected)
     assert res.variances is None
 
 
 def test_covariance_accum_returns_expected_result_1_sample():
     rng = np.random.default_rng(32)
     da = sc.DataArray(sc.array(dims=["variable"], values=rng.normal(0.0, 1.0, 6)))
 
     accum = CovarianceAccum()
     accum.add(da)
 
     res = accum.get()
-    assert sc.all(sc.isnan(res)).value
-    assert res.attrs["n_samples"] == sc.index(1)
+    assert sc.all(sc.isnan(res.data)).value
+    assert res.n_samples == 1
 
 
 def test_covariance_accum_returns_number_of_samples():
     rng = np.random.default_rng(823)
     da = sc.DataArray(sc.array(dims=["variable"], values=rng.normal(0.0, 1.0, 6)))
 
     accum = CovarianceAccum()
     accum.add(da)
     accum.add(da)
     accum.add(da)
     accum.add(da)
     accum.add(da)
 
-    res = accum.get()
-    assert sc.identical(res.attrs["n_samples"], sc.index(5))
+    assert accum.get().n_samples == 5
 
 
 def test_covariance_accum_erases_metadata():
     rng = np.random.default_rng(44)
     da = sc.DataArray(
         sc.array(dims=["variable", "observation"], values=rng.normal(0.0, 1.0, (9, 2))),
         coords={"x": sc.arange("variable", 9, unit="kg")},
         masks={"m": sc.arange("variable", 9) < 7},
         attrs={"a": sc.index(4), "b": sc.scalar("a string")},
     )
 
     accum = CovarianceAccum()
     accum.add(da["observation", 0])
     accum.add(da["observation", 1])
-    res = accum.get()
+    res = accum.get().data
 
     assert not res.coords.keys()
     assert not res.masks.keys()
-    assert set(res.attrs.keys()) == {"n_samples"}
 
 
 def test_covariance_accum_add_from():
     rng = np.random.default_rng(231)
     da = sc.DataArray(
         sc.array(dims=["variable", "observation"], values=rng.normal(0.0, 1.0, (5, 19)))
     )
@@ -250,34 +269,34 @@
         accum1.add(chunk1["observation", i])
     for i in range(9):
         accum2.add(chunk2["observation", i])
 
     accum0.add_from(accum1)
     accum0.add_from(accum2)
 
-    a = accum0.get()
-    b = accum_total.get()
+    a = accum0.get().data
+    b = accum_total.get().data
     np.testing.assert_allclose(a.values, b.values)
 
 
 def test_covariance_accum_new_does_not_return_stored_samples():
     rng = np.random.default_rng(412)
     da = sc.DataArray(sc.array(dims=["variable"], values=rng.normal(0.0, 1.0, 7)))
     accum = CovarianceAccum()
     accum.add(da)
 
     new = accum.new()
     with pytest.raises(RuntimeError):
         new.get()  # has no samples to get
 
 
-@pytest.mark.parametrize("dims", (None, ("x", "y")))
+@pytest.mark.parametrize("dims", [None, ("x", "y")])
 def test_covariance_accum_new_passes_dims_along(dims):
     rng = np.random.default_rng(9)
     da = sc.DataArray(sc.array(dims=["variable"], values=rng.normal(0.0, 1.0, 8)))
     accum = CovarianceAccum(dims=dims)
     new = accum.new()
 
     accum.add(da)
     new.add(da)
 
-    assert accum.get().dims == new.get().dims
+    assert accum.get().data.dims == new.get().data.dims
```

### Comparing `scippuncertainty-23.3.0/tests/mc/driver_test.py` & `scippuncertainty-24.5.0/tests/mc/driver_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         samplers={"d": NormalDenseSampler(da)},
         accumulators={"r": VarianceAccum()},
         seed=412,
         n_threads=1,
         progress=False,
     )
 
-    assert res["r"].attrs["n_samples"] == sc.index(10)
+    assert res.n_samples == 10
 
 
 def test_run_raises_if_sampler_is_missing():
     def f(a, b):
         return {"r": a + b}
 
     rng = np.random.default_rng(125)
@@ -212,15 +212,17 @@
         sc.array(
             dims=["x"],
             values=rng.normal(4.0, 0.5, n),
             variances=rng.uniform(0.01, 0.1, n),
         )
     )
 
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError, match="Mismatch in accumulators and function return value"
+    ):
         run(
             f,
             n_samples=20,
             samplers={"a": NormalDenseSampler(da)},
             accumulators={"r": VarianceAccum()},
             seed=83,
             n_threads=1,
@@ -238,15 +240,17 @@
         sc.array(
             dims=["x"],
             values=rng.normal(4.0, 0.5, n),
             variances=rng.uniform(0.01, 0.1, n),
         )
     )
 
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError, match="Mismatch in accumulators and function return value"
+    ):
         run(
             f,
             n_samples=20,
             samplers={"a": NormalDenseSampler(da)},
             accumulators={"r": VarianceAccum(), "s": VarianceAccum()},
             seed=83,
             n_threads=1,
@@ -264,15 +268,17 @@
         sc.array(
             dims=["x"],
             values=rng.normal(4.0, 0.5, n),
             variances=rng.uniform(0.01, 0.1, n),
         )
     )
 
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError, match="Mismatch in accumulators and function return value"
+    ):
         run(
             f,
             n_samples=20,
             samplers={"a": NormalDenseSampler(da)},
             accumulators={"r": VarianceAccum(), "rs": VarianceAccum()},
             seed=83,
             n_threads=1,
```

### Comparing `scippuncertainty-23.3.0/tests/mc/sampler_test.py` & `scippuncertainty-24.5.0/tests/mc/sampler_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import numpy as np
 import pytest
 import scipp as sc
+import scipp.testing
 
 from scippuncertainty.mc import NormalDenseSampler, PoissonDenseSampler
 
 
 @pytest.mark.parametrize("sampler_type", [PoissonDenseSampler, NormalDenseSampler])
 def test_dense_samplers_produce_no_variances(sampler_type):
     rng = np.random.default_rng(67176)
@@ -48,35 +49,26 @@
     rng = np.random.default_rng(512)
     da = sc.DataArray(
         sc.array(
             dims=["xx"],
             values=rng.uniform(0.0, 1.0, 10),
             variances=rng.uniform(0.001, 0.1, 10),
         ),
-        coords={"xx": sc.arange("xx", 10, unit="s")},
-        masks={"m": sc.arange("xx", 10) < 5},
-        attrs={
-            "a": sc.scalar(8),
-            "b": sc.scalar("a string"),
-            "c": sc.arange("xx", 10) * 2,
+        coords={
+            "xx": sc.arange("xx", 10, unit="s"),
+            "a": -sc.arange("xx", 10, unit="s"),
         },
+        masks={"m": sc.arange("xx", 10) < 5},
     )
+    da.coords.set_aligned("a", aligned=False)
     sampler = sampler_type(da)
     sample = sampler.sample_once(rng)
 
-    assert set(sample.coords.keys()) == set(da.coords.keys())
-    assert sc.identical(sample.coords["xx"], da.coords["xx"])
-
-    assert set(sample.masks.keys()) == set(da.masks.keys())
-    assert sc.identical(sample.masks["m"], da.masks["m"])
-
-    assert set(sample.attrs.keys()) == set(da.attrs.keys())
-    assert sc.identical(sample.attrs["a"], da.attrs["a"])
-    assert sc.identical(sample.attrs["b"], da.attrs["b"])
-    assert sc.identical(sample.attrs["c"], da.attrs["c"])
+    sc.testing.assert_identical(sample.coords, da.coords)
+    sc.testing.assert_identical(sample.masks, da.masks)
 
 
 @pytest.mark.parametrize("sampler_type", [PoissonDenseSampler, NormalDenseSampler])
 def test_dense_samplers_copy_results(sampler_type):
     rng = np.random.default_rng(2241)
     da = sc.DataArray(
         sc.array(
```

### Comparing `scippuncertainty-23.3.0/tests/random_test.py` & `scippuncertainty-24.5.0/tests/random_test.py`

 * *Files identical despite different names*

