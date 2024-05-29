# Comparing `tmp/dplutils-0.5.2.tar.gz` & `tmp/dplutils-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dplutils-0.5.2.tar", last modified: Thu Apr 11 15:11:21 2024, max compression
+gzip compressed data, was "dplutils-0.5.3.tar", last modified: Wed May 29 15:44:29 2024, max compression
```

## Comparing `dplutils-0.5.2.tar` & `dplutils-0.5.3.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.352961 dplutils-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 15:11:10.000000 dplutils-0.5.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-11 15:11:10.000000 dplutils-0.5.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.340961 dplutils-0.5.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 15:11:10.000000 dplutils-0.5.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.340961 dplutils-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-11 15:11:10.000000 dplutils-0.5.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-11 15:11:10.000000 dplutils-0.5.2/.github/workflows/dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-11 15:11:10.000000 dplutils-0.5.2/.github/workflows/security.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-11 15:11:10.000000 dplutils-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-11 15:11:10.000000 dplutils-0.5.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-11 15:11:10.000000 dplutils-0.5.2/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-11 15:11:10.000000 dplutils-0.5.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-11 15:11:10.000000 dplutils-0.5.2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-11 15:11:10.000000 dplutils-0.5.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-11 15:11:10.000000 dplutils-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-11 15:11:21.352961 dplutils-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-11 15:11:10.000000 dplutils-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.340961 dplutils-0.5.2/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-11 15:11:10.000000 dplutils-0.5.2/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-04-11 15:11:10.000000 dplutils-0.5.2/docker/startray.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.340961 dplutils-0.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.340961 dplutils-0.5.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/_static/.DS_Store
--rwxr-xr-x   0 runner    (1001) docker     (127)    33376 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/_static/SSEC_logo_horiz_blue_1152x263.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    72437 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/_static/SSEC_logo_vert_white_lg_1184x661.png
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.344961 dplutils-0.5.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/api_cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/api_observers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/api_pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/api_streaming.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/execution.rst
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/extending.rst
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/tasks_graphs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.344961 dplutils-0.5.2/dplutils/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.348961 dplutils-0.5.2/dplutils/observer/
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/observer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/observer/aim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/observer/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/observer/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.348961 dplutils-0.5.2/dplutils/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/ray.py
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.352961 dplutils-0.5.2/dplutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.348961 dplutils-0.5.2/githooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      322 2024-04-11 15:11:10.000000 dplutils-0.5.2/githooks/pre-push
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-11 15:11:10.000000 dplutils-0.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.348961 dplutils-0.5.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-11 15:11:10.000000 dplutils-0.5.2/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 15:11:10.000000 dplutils-0.5.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-11 15:11:10.000000 dplutils-0.5.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 15:11:10.000000 dplutils-0.5.2/requirements/prd.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 15:11:10.000000 dplutils-0.5.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:11:21.352961 dplutils-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.348961 dplutils-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.348961 dplutils-0.5.2/tests/observer/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/observer/test_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/observer/test_observer_aim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/observer/test_observer_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/observer/test_observer_ray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.352961 dplutils-0.5.2/tests/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_executor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_pipeline_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_pipeline_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_pipeline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_ray_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_ray_stream_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_stream_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-11 15:11:10.000000 dplutils-0.5.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.540121 dplutils-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-29 15:44:18.000000 dplutils-0.5.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-29 15:44:18.000000 dplutils-0.5.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.524121 dplutils-0.5.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 15:44:18.000000 dplutils-0.5.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.524121 dplutils-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-29 15:44:18.000000 dplutils-0.5.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-29 15:44:18.000000 dplutils-0.5.3/.github/workflows/dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-29 15:44:18.000000 dplutils-0.5.3/.github/workflows/security.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-29 15:44:18.000000 dplutils-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-29 15:44:18.000000 dplutils-0.5.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-29 15:44:18.000000 dplutils-0.5.3/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-29 15:44:18.000000 dplutils-0.5.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-29 15:44:18.000000 dplutils-0.5.3/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-29 15:44:18.000000 dplutils-0.5.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-29 15:44:18.000000 dplutils-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-05-29 15:44:29.536121 dplutils-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-29 15:44:18.000000 dplutils-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.524121 dplutils-0.5.3/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-29 15:44:18.000000 dplutils-0.5.3/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-29 15:44:18.000000 dplutils-0.5.3/docker/startray.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.524121 dplutils-0.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.528121 dplutils-0.5.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/_static/.DS_Store
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33376 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/_static/SSEC_logo_horiz_blue_1152x263.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72437 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/_static/SSEC_logo_vert_white_lg_1184x661.png
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.528121 dplutils-0.5.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/api_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/api_observers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/api_pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/api_streaming.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/execution.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/observing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/tasks_graphs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-29 15:44:18.000000 dplutils-0.5.3/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.528121 dplutils-0.5.3/dplutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 15:44:29.000000 dplutils-0.5.3/dplutils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.532121 dplutils-0.5.3/dplutils/observer/
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/observer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/observer/aim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/observer/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/observer/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.532121 dplutils-0.5.3/dplutils/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/pipeline/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/pipeline/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/pipeline/ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/pipeline/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/pipeline/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/pipeline/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-29 15:44:18.000000 dplutils-0.5.3/dplutils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.536121 dplutils-0.5.3/dplutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-05-29 15:44:29.000000 dplutils-0.5.3/dplutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-29 15:44:29.000000 dplutils-0.5.3/dplutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:44:29.000000 dplutils-0.5.3/dplutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:44:29.000000 dplutils-0.5.3/dplutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-29 15:44:29.000000 dplutils-0.5.3/dplutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 15:44:29.000000 dplutils-0.5.3/dplutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.532121 dplutils-0.5.3/githooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      322 2024-05-29 15:44:18.000000 dplutils-0.5.3/githooks/pre-push
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-29 15:44:18.000000 dplutils-0.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.532121 dplutils-0.5.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-29 15:44:18.000000 dplutils-0.5.3/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 15:44:18.000000 dplutils-0.5.3/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-29 15:44:18.000000 dplutils-0.5.3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-29 15:44:18.000000 dplutils-0.5.3/requirements/prd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 15:44:18.000000 dplutils-0.5.3/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:44:29.540121 dplutils-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.532121 dplutils-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.536121 dplutils-0.5.3/tests/observer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/observer/test_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/observer/test_observer_aim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/observer/test_observer_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/observer/test_observer_ray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:44:29.536121 dplutils-0.5.3/tests/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/pipeline/test_executor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/pipeline/test_pipeline_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/pipeline/test_pipeline_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/pipeline/test_pipeline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/pipeline/test_ray_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/pipeline/test_ray_stream_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/pipeline/test_stream_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/pipeline/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-29 15:44:18.000000 dplutils-0.5.3/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-29 15:44:18.000000 dplutils-0.5.3/tox.ini
```

### Comparing `dplutils-0.5.2/.github/workflows/ci.yml` & `dplutils-0.5.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/.github/workflows/dist.yml` & `dplutils-0.5.3/.github/workflows/dist.yml`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/.github/workflows/security.yml` & `dplutils-0.5.3/.github/workflows/security.yml`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/.gitignore` & `dplutils-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/.readthedocs.yaml` & `dplutils-0.5.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/.zenodo.json` & `dplutils-0.5.3/.zenodo.json`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/CITATION.cff` & `dplutils-0.5.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/CODE_OF_CONDUCT.md` & `dplutils-0.5.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/LICENSE` & `dplutils-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/PKG-INFO` & `dplutils-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dplutils
-Version: 0.5.2
+Version: 0.5.3
 Author-email: Scientifc Software Engineering Center at JHU <ssec@jhu.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scientific Software Engineering Center at JHU
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `dplutils-0.5.2/README.md` & `dplutils-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/docker/Dockerfile` & `dplutils-0.5.3/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/docs/Makefile` & `dplutils-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/docs/_static/.DS_Store` & `dplutils-0.5.3/docs/_static/.DS_Store`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/docs/_static/SSEC_logo_horiz_blue_1152x263.png` & `dplutils-0.5.3/docs/_static/SSEC_logo_horiz_blue_1152x263.png`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/docs/_static/SSEC_logo_vert_white_lg_1184x661.png` & `dplutils-0.5.3/docs/_static/SSEC_logo_vert_white_lg_1184x661.png`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/docs/make.bat` & `dplutils-0.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/docs/source/api_observers.rst` & `dplutils-0.5.3/docs/source/api_observers.rst`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/docs/source/conf.py` & `dplutils-0.5.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/docs/source/quickstart.rst` & `dplutils-0.5.3/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/dplutils/cli.py` & `dplutils-0.5.3/dplutils/cli.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/dplutils/observer/__init__.py` & `dplutils-0.5.3/dplutils/observer/__init__.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/dplutils/observer/aim.py` & `dplutils-0.5.3/dplutils/observer/aim.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/dplutils/observer/mlflow.py` & `dplutils-0.5.3/dplutils/observer/mlflow.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/dplutils/observer/ray.py` & `dplutils-0.5.3/dplutils/observer/ray.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/dplutils/pipeline/executor.py` & `dplutils-0.5.3/dplutils/pipeline/executor.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/dplutils/pipeline/graph.py` & `dplutils-0.5.3/dplutils/pipeline/graph.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/dplutils/pipeline/ray.py` & `dplutils-0.5.3/dplutils/pipeline/ray.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/dplutils/pipeline/stream.py` & `dplutils-0.5.3/dplutils/pipeline/stream.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/dplutils/pipeline/task.py` & `dplutils-0.5.3/dplutils/pipeline/task.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/dplutils.egg-info/PKG-INFO` & `dplutils-0.5.3/dplutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dplutils
-Version: 0.5.2
+Version: 0.5.3
 Author-email: Scientifc Software Engineering Center at JHU <ssec@jhu.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scientific Software Engineering Center at JHU
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `dplutils-0.5.2/dplutils.egg-info/SOURCES.txt` & `dplutils-0.5.3/dplutils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 docs/source/api_streaming.rst
 docs/source/command_line.rst
 docs/source/conf.py
 docs/source/configuration.rst
 docs/source/execution.rst
 docs/source/extending.rst
 docs/source/index.rst
+docs/source/observing.rst
 docs/source/quickstart.rst
 docs/source/tasks_graphs.rst
 docs/source/usage.rst
 dplutils/__init__.py
 dplutils/_version.py
 dplutils/cli.py
 dplutils/util.py
```

### Comparing `dplutils-0.5.2/pyproject.toml` & `dplutils-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tests/conftest.py` & `dplutils-0.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tests/observer/test_observer.py` & `dplutils-0.5.3/tests/observer/test_observer.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tests/observer/test_observer_aim.py` & `dplutils-0.5.3/tests/observer/test_observer_aim.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tests/observer/test_observer_mlflow.py` & `dplutils-0.5.3/tests/observer/test_observer_mlflow.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tests/observer/test_observer_ray.py` & `dplutils-0.5.3/tests/observer/test_observer_ray.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tests/pipeline/test_executor_base.py` & `dplutils-0.5.3/tests/pipeline/test_executor_base.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tests/pipeline/test_pipeline_graph.py` & `dplutils-0.5.3/tests/pipeline/test_pipeline_graph.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tests/pipeline/test_pipeline_task.py` & `dplutils-0.5.3/tests/pipeline/test_pipeline_task.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tests/pipeline/test_ray_executor.py` & `dplutils-0.5.3/tests/pipeline/test_ray_executor.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tests/pipeline/test_ray_stream_executor.py` & `dplutils-0.5.3/tests/pipeline/test_ray_stream_executor.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tests/pipeline/test_stream_executor.py` & `dplutils-0.5.3/tests/pipeline/test_stream_executor.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tests/pipeline/test_suite.py` & `dplutils-0.5.3/tests/pipeline/test_suite.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tests/test_cli.py` & `dplutils-0.5.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.2/tox.ini` & `dplutils-0.5.3/tox.ini`

 * *Files identical despite different names*

