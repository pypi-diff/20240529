# Comparing `tmp/flox-0.9.7.tar.gz` & `tmp/flox-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flox-0.9.7.tar", last modified: Wed May  8 13:41:11 2024, max compression
+gzip compressed data, was "flox-0.9.8.tar", last modified: Wed May 29 15:16:31 2024, max compression
```

## Comparing `flox-0.9.7.tar` & `flox-0.9.8.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.627633 flox-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 13:40:54.000000 flox-0.9.7/.git_archival.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.607633 flox-0.9.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-08 13:40:54.000000 flox-0.9.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.607633 flox-0.9.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 13:40:54.000000 flox-0.9.7/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-08 13:40:54.000000 flox-0.9.7/.github/workflows/ci-additional.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-08 13:40:54.000000 flox-0.9.7/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 13:40:54.000000 flox-0.9.7/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-08 13:40:54.000000 flox-0.9.7/.github/workflows/testpypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-08 13:40:54.000000 flox-0.9.7/.github/workflows/upstream-dev-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-08 13:40:54.000000 flox-0.9.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-08 13:40:54.000000 flox-0.9.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 13:40:54.000000 flox-0.9.7/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-08 13:40:54.000000 flox-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-05-08 13:41:11.627633 flox-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-08 13:40:54.000000 flox-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.607633 flox-0.9.7/asv_bench/
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-08 13:40:54.000000 flox-0.9.7/asv_bench/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.607633 flox-0.9.7/asv_bench/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-08 13:40:54.000000 flox-0.9.7/asv_bench/benchmarks/README_CI.md
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-08 13:40:54.000000 flox-0.9.7/asv_bench/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-08 13:40:54.000000 flox-0.9.7/asv_bench/benchmarks/cohorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-08 13:40:54.000000 flox-0.9.7/asv_bench/benchmarks/combine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-08 13:40:54.000000 flox-0.9.7/asv_bench/benchmarks/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.611633 flox-0.9.7/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-08 13:40:54.000000 flox-0.9.7/ci/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 13:40:54.000000 flox-0.9.7/ci/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-08 13:40:54.000000 flox-0.9.7/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 13:40:54.000000 flox-0.9.7/ci/minimal-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-08 13:40:54.000000 flox-0.9.7/ci/no-dask.yml
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 13:40:54.000000 flox-0.9.7/ci/no-numba.yml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-08 13:40:54.000000 flox-0.9.7/ci/no-xarray.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-08 13:40:54.000000 flox-0.9.7/ci/upstream-dev-env.yml
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 13:40:54.000000 flox-0.9.7/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.611633 flox-0.9.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-08 13:40:54.000000 flox-0.9.7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.615633 flox-0.9.7/docs/diagrams/
--rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/bitmask-patterns-perfect.png
--rw-r--r--   0 runner    (1001) docker     (127)    43022 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/blockwise.png
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/cohorts-month-chunk4.png
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/cohorts-month-chunk5.png
--rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/containment.png
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/counties-bitmask-containment.png
--rw-r--r--   0 runner    (1001) docker     (127)    46006 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/map-reduce.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-blockwise-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (127)    38910 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-blockwise.svg
--rw-r--r--   0 runner    (1001) docker     (127)   102136 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-cohorts-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (127)    60369 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-cohorts.svg
--rw-r--r--   0 runner    (1001) docker     (127)   105406 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-map-reduce-reindex-False-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (127)    62434 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-map-reduce-reindex-False.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101278 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-map-reduce-reindex-True-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (127)    62159 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-map-reduce-reindex-True.svg
--rw-r--r--   0 runner    (1001) docker     (127)   177642 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-split-apply-combine-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (127)   153059 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/nwm-cohorts.png
--rw-r--r--   0 runner    (1001) docker     (127)    61350 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/split-apply-combine.svg
--rw-r--r--   0 runner    (1001) docker     (127)    55442 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/split-reduce.png
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-08 13:40:54.000000 flox-0.9.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 13:40:54.000000 flox-0.9.7/docs/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.619633 flox-0.9.7/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.619633 flox-0.9.7/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/aggregations.md
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/arrays.md
--rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/engines.md
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/implementation.md
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.619633 flox-0.9.7/docs/source/user-stories/
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/climatology-hourly-cubed.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    74240 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/climatology-hourly.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/climatology.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/custom-aggregations.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   733833 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/hourly-climatology.html
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/nD-bins.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/overlaps.md
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/xarray.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.623633 flox-0.9.7/flox/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-08 13:40:54.000000 flox-0.9.7/flox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 13:41:11.000000 flox-0.9.7/flox/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-05-08 13:40:54.000000 flox-0.9.7/flox/aggregate_flox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-08 13:40:54.000000 flox-0.9.7/flox/aggregate_npg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-08 13:40:54.000000 flox-0.9.7/flox/aggregate_numbagg.py
--rw-r--r--   0 runner    (1001) docker     (127)    21913 2024-05-08 13:40:54.000000 flox-0.9.7/flox/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-08 13:40:54.000000 flox-0.9.7/flox/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    96440 2024-05-08 13:40:54.000000 flox-0.9.7/flox/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:54.000000 flox-0.9.7/flox/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-08 13:40:54.000000 flox-0.9.7/flox/visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)    25338 2024-05-08 13:40:54.000000 flox-0.9.7/flox/xarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-08 13:40:54.000000 flox-0.9.7/flox/xrdtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12005 2024-05-08 13:40:54.000000 flox-0.9.7/flox/xrutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.623633 flox-0.9.7/flox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-05-08 13:41:11.000000 flox-0.9.7/flox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-08 13:41:11.000000 flox-0.9.7/flox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:41:11.000000 flox-0.9.7/flox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 13:41:11.000000 flox-0.9.7/flox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 13:41:11.000000 flox-0.9.7/flox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-08 13:40:54.000000 flox-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-08 13:40:54.000000 flox-0.9.7/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:41:11.627633 flox-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-08 13:40:54.000000 flox-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.623633 flox-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-08 13:40:54.000000 flox-0.9.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-08 13:40:54.000000 flox-0.9.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    61218 2024-05-08 13:40:54.000000 flox-0.9.7/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    24647 2024-05-08 13:40:54.000000 flox-0.9.7/tests/test_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.611394 flox-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 15:16:09.000000 flox-0.9.8/.git_archival.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.595394 flox-0.9.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 15:16:09.000000 flox-0.9.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.595394 flox-0.9.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-29 15:16:09.000000 flox-0.9.8/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-29 15:16:09.000000 flox-0.9.8/.github/workflows/ci-additional.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-29 15:16:09.000000 flox-0.9.8/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-29 15:16:09.000000 flox-0.9.8/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-29 15:16:09.000000 flox-0.9.8/.github/workflows/testpypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-29 15:16:09.000000 flox-0.9.8/.github/workflows/upstream-dev-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-29 15:16:09.000000 flox-0.9.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-29 15:16:09.000000 flox-0.9.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-29 15:16:09.000000 flox-0.9.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-29 15:16:09.000000 flox-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-05-29 15:16:31.611394 flox-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-29 15:16:09.000000 flox-0.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.595394 flox-0.9.8/asv_bench/
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-29 15:16:09.000000 flox-0.9.8/asv_bench/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.595394 flox-0.9.8/asv_bench/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-29 15:16:09.000000 flox-0.9.8/asv_bench/benchmarks/README_CI.md
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-29 15:16:09.000000 flox-0.9.8/asv_bench/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-05-29 15:16:09.000000 flox-0.9.8/asv_bench/benchmarks/cohorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-29 15:16:09.000000 flox-0.9.8/asv_bench/benchmarks/combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-29 15:16:09.000000 flox-0.9.8/asv_bench/benchmarks/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.599393 flox-0.9.8/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 15:16:09.000000 flox-0.9.8/ci/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-29 15:16:09.000000 flox-0.9.8/ci/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-29 15:16:09.000000 flox-0.9.8/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 15:16:09.000000 flox-0.9.8/ci/minimal-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 15:16:09.000000 flox-0.9.8/ci/no-dask.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-29 15:16:09.000000 flox-0.9.8/ci/no-numba.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-29 15:16:09.000000 flox-0.9.8/ci/no-xarray.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-29 15:16:09.000000 flox-0.9.8/ci/upstream-dev-env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 15:16:09.000000 flox-0.9.8/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.599393 flox-0.9.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-29 15:16:09.000000 flox-0.9.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.603394 flox-0.9.8/docs/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/bitmask-patterns-perfect.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43022 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/blockwise.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/cohorts-month-chunk4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/cohorts-month-chunk5.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/containment.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/counties-bitmask-containment.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46006 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/map-reduce.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/new-blockwise-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    38910 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/new-blockwise.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   102136 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/new-cohorts-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    60369 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/new-cohorts.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   105406 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/new-map-reduce-reindex-False-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    62434 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/new-map-reduce-reindex-False.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101278 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/new-map-reduce-reindex-True-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    62159 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/new-map-reduce-reindex-True.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   177642 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/new-split-apply-combine-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   153059 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/nwm-cohorts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61350 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/split-apply-combine.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    55442 2024-05-29 15:16:09.000000 flox-0.9.8/docs/diagrams/split-reduce.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-29 15:16:09.000000 flox-0.9.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 15:16:09.000000 flox-0.9.8/docs/requirements-docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.603394 flox-0.9.8/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.603394 flox-0.9.8/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/aggregations.md
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/arrays.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/engines.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/implementation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.607394 flox-0.9.8/docs/source/user-stories/
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/user-stories/climatology-hourly-cubed.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    74240 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/user-stories/climatology-hourly.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/user-stories/climatology.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/user-stories/custom-aggregations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   733833 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/user-stories/hourly-climatology.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/user-stories/nD-bins.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/user-stories/overlaps.md
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/user-stories.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-29 15:16:09.000000 flox-0.9.8/docs/source/xarray.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.611394 flox-0.9.8/flox/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-29 15:16:09.000000 flox-0.9.8/flox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 15:16:31.000000 flox-0.9.8/flox/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-05-29 15:16:09.000000 flox-0.9.8/flox/aggregate_flox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-29 15:16:09.000000 flox-0.9.8/flox/aggregate_npg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-29 15:16:09.000000 flox-0.9.8/flox/aggregate_numbagg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21913 2024-05-29 15:16:09.000000 flox-0.9.8/flox/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 15:16:09.000000 flox-0.9.8/flox/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97910 2024-05-29 15:16:09.000000 flox-0.9.8/flox/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:09.000000 flox-0.9.8/flox/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-29 15:16:09.000000 flox-0.9.8/flox/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25338 2024-05-29 15:16:09.000000 flox-0.9.8/flox/xarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-29 15:16:09.000000 flox-0.9.8/flox/xrdtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12005 2024-05-29 15:16:09.000000 flox-0.9.8/flox/xrutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.611394 flox-0.9.8/flox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-05-29 15:16:31.000000 flox-0.9.8/flox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-29 15:16:31.000000 flox-0.9.8/flox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:16:31.000000 flox-0.9.8/flox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-29 15:16:31.000000 flox-0.9.8/flox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 15:16:31.000000 flox-0.9.8/flox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-29 15:16:09.000000 flox-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-29 15:16:09.000000 flox-0.9.8/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:16:31.611394 flox-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 15:16:09.000000 flox-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:16:31.611394 flox-0.9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-29 15:16:09.000000 flox-0.9.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 15:16:09.000000 flox-0.9.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62342 2024-05-29 15:16:09.000000 flox-0.9.8/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24647 2024-05-29 15:16:09.000000 flox-0.9.8/tests/test_xarray.py
```

### Comparing `flox-0.9.7/.github/workflows/benchmarks.yml` & `flox-0.9.8/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/.github/workflows/ci-additional.yaml` & `flox-0.9.8/.github/workflows/ci-additional.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/.github/workflows/ci.yaml` & `flox-0.9.8/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/.github/workflows/pypi.yaml` & `flox-0.9.8/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/.github/workflows/testpypi-release.yaml` & `flox-0.9.8/.github/workflows/testpypi-release.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/.github/workflows/upstream-dev-ci.yaml` & `flox-0.9.8/.github/workflows/upstream-dev-ci.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/.gitignore` & `flox-0.9.8/.gitignore`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/.pre-commit-config.yaml` & `flox-0.9.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/LICENSE` & `flox-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/PKG-INFO` & `flox-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flox
-Version: 0.9.7
+Version: 0.9.8
 Summary: GroupBy operations for dask.array
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flox-0.9.7/README.md` & `flox-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/asv_bench/asv.conf.json` & `flox-0.9.8/asv_bench/asv.conf.json`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/asv_bench/benchmarks/README_CI.md` & `flox-0.9.8/asv_bench/benchmarks/README_CI.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/asv_bench/benchmarks/__init__.py` & `flox-0.9.8/asv_bench/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/asv_bench/benchmarks/cohorts.py` & `flox-0.9.8/asv_bench/benchmarks/cohorts.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     def result(self):
         return flox.groupby_reduce(self.array, self.by, func="sum", axis=self.axis)[0]
 
     def containment(self):
         asfloat = self.bitmask().astype(float)
         chunks_per_label = asfloat.sum(axis=0)
         containment = (asfloat.T @ asfloat) / chunks_per_label
-        print(containment.nnz / np.prod(containment.shape))
         return containment.todense()
 
     def chunks_cohorts(self):
         return flox.core.find_group_cohorts(
             self.by,
             [self.array.chunks[ax] for ax in self.axis],
             expected_groups=self.expected,
```

### Comparing `flox-0.9.7/asv_bench/benchmarks/combine.py` & `flox-0.9.8/asv_bench/benchmarks/combine.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/asv_bench/benchmarks/reduce.py` & `flox-0.9.8/asv_bench/benchmarks/reduce.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/ci/upstream-dev-env.yml` & `flox-0.9.8/ci/upstream-dev-env.yml`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/Makefile` & `flox-0.9.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/bitmask-patterns-perfect.png` & `flox-0.9.8/docs/diagrams/bitmask-patterns-perfect.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/blockwise.png` & `flox-0.9.8/docs/diagrams/blockwise.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/cohorts-month-chunk4.png` & `flox-0.9.8/docs/diagrams/cohorts-month-chunk4.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/cohorts-month-chunk5.png` & `flox-0.9.8/docs/diagrams/cohorts-month-chunk5.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/containment.png` & `flox-0.9.8/docs/diagrams/containment.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/counties-bitmask-containment.png` & `flox-0.9.8/docs/diagrams/counties-bitmask-containment.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/map-reduce.png` & `flox-0.9.8/docs/diagrams/map-reduce.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/new-blockwise-annotated.svg` & `flox-0.9.8/docs/diagrams/new-blockwise-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/new-blockwise.svg` & `flox-0.9.8/docs/diagrams/new-blockwise.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/new-cohorts-annotated.svg` & `flox-0.9.8/docs/diagrams/new-cohorts-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/new-cohorts.svg` & `flox-0.9.8/docs/diagrams/new-cohorts.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/new-map-reduce-reindex-False-annotated.svg` & `flox-0.9.8/docs/diagrams/new-map-reduce-reindex-False-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/new-map-reduce-reindex-False.svg` & `flox-0.9.8/docs/diagrams/new-map-reduce-reindex-False.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/new-map-reduce-reindex-True-annotated.svg` & `flox-0.9.8/docs/diagrams/new-map-reduce-reindex-True-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/new-map-reduce-reindex-True.svg` & `flox-0.9.8/docs/diagrams/new-map-reduce-reindex-True.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/new-split-apply-combine-annotated.svg` & `flox-0.9.8/docs/diagrams/new-split-apply-combine-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/nwm-cohorts.png` & `flox-0.9.8/docs/diagrams/nwm-cohorts.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/split-apply-combine.svg` & `flox-0.9.8/docs/diagrams/split-apply-combine.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/diagrams/split-reduce.png` & `flox-0.9.8/docs/diagrams/split-reduce.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/make.bat` & `flox-0.9.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/aggregations.md` & `flox-0.9.8/docs/source/aggregations.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/api.rst` & `flox-0.9.8/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/arrays.md` & `flox-0.9.8/docs/source/arrays.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/conf.py` & `flox-0.9.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/engines.md` & `flox-0.9.8/docs/source/engines.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/implementation.md` & `flox-0.9.8/docs/source/implementation.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/index.md` & `flox-0.9.8/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/intro.md` & `flox-0.9.8/docs/source/intro.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/user-stories/climatology-hourly-cubed.ipynb` & `flox-0.9.8/docs/source/user-stories/climatology-hourly-cubed.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9625%*

 * *Differences: {"'cells'": "{insert: [(7, OrderedDict([('cell_type', 'markdown'), ('id', '7'), ('metadata', "*

 * *            "OrderedDict()), ('source', ['## Other climatologies: resampling by month\\n', '\\n', "*

 * *            '\'This uses the "blockwise" strategy.\'])])), (8, OrderedDict([(\'cell_type\', '*

 * *            "'code'), ('execution_count', None), ('id', '8'), ('metadata', OrderedDict()), "*

 * *            "('outputs', []), ('source', ['monthly = "*

 * *            'ds.tp.resample(time="ME").sum(method="blockwise")\\n\', \'mont […]*

```diff
@@ -82,14 +82,45 @@
             "execution_count": null,
             "id": "6",
             "metadata": {},
             "outputs": [],
             "source": [
                 "hourly.compute()"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "7",
+            "metadata": {},
+            "source": [
+                "## Other climatologies: resampling by month\n",
+                "\n",
+                "This uses the \"blockwise\" strategy."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "8",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "monthly = ds.tp.resample(time=\"ME\").sum(method=\"blockwise\")\n",
+                "monthly"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "9",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "monthly.compute()"
+            ]
         }
     ],
     "metadata": {
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
```

### Comparing `flox-0.9.7/docs/source/user-stories/climatology-hourly.ipynb` & `flox-0.9.8/docs/source/user-stories/climatology-hourly.ipynb`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/user-stories/climatology.ipynb` & `flox-0.9.8/docs/source/user-stories/climatology.ipynb`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/user-stories/custom-aggregations.ipynb` & `flox-0.9.8/docs/source/user-stories/custom-aggregations.ipynb`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/user-stories/hourly-climatology.html` & `flox-0.9.8/docs/source/user-stories/hourly-climatology.html`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/user-stories/nD-bins.ipynb` & `flox-0.9.8/docs/source/user-stories/nD-bins.ipynb`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/user-stories/overlaps.md` & `flox-0.9.8/docs/source/user-stories/overlaps.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/docs/source/xarray.md` & `flox-0.9.8/docs/source/xarray.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/flox/aggregate_flox.py` & `flox-0.9.8/flox/aggregate_flox.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/flox/aggregate_npg.py` & `flox-0.9.8/flox/aggregate_npg.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/flox/aggregate_numbagg.py` & `flox-0.9.8/flox/aggregate_numbagg.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/flox/aggregations.py` & `flox-0.9.8/flox/aggregations.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/flox/core.py` & `flox-0.9.8/flox/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1794,95 +1794,131 @@
     import cubed
     import cubed.core.groupby
 
     # I think _tree_reduce expects this
     assert isinstance(axis, Sequence)
     assert all(ax >= 0 for ax in axis)
 
-    inds = tuple(range(array.ndim))
+    if method == "blockwise":
+        assert by.ndim == 1
+        assert expected_groups is not None
+
+        def _reduction_func(a, by, axis, start_group, num_groups):
+            # adjust group labels to start from 0 for each chunk
+            by_for_chunk = by - start_group
+            expected_groups_for_chunk = pd.RangeIndex(num_groups)
+
+            axis = (axis,)  # convert integral axis to tuple
+
+            blockwise_method = partial(
+                _reduce_blockwise,
+                agg=agg,
+                axis=axis,
+                expected_groups=expected_groups_for_chunk,
+                fill_value=fill_value,
+                engine=engine,
+                sort=sort,
+                reindex=reindex,
+            )
+            out = blockwise_method(a, by_for_chunk)
+            return out[agg.name]
+
+        num_groups = len(expected_groups)
+        result = cubed.core.groupby.groupby_blockwise(
+            array, by, axis=axis, func=_reduction_func, num_groups=num_groups
+        )
+        groups = (expected_groups.to_numpy(),)
+        return (result, groups)
 
-    by_input = by
+    else:
+        inds = tuple(range(array.ndim))
+
+        by_input = by
+
+        # Unifying chunks is necessary for argreductions.
+        # We need to rechunk before zipping up with the index
+        # let's always do it anyway
+        if not is_chunked_array(by):
+            # chunk numpy arrays like the input array
+            chunks = tuple(
+                array.chunks[ax] if by.shape[ax] != 1 else (1,) for ax in range(-by.ndim, 0)
+            )
 
-    # Unifying chunks is necessary for argreductions.
-    # We need to rechunk before zipping up with the index
-    # let's always do it anyway
-    if not is_chunked_array(by):
-        # chunk numpy arrays like the input array
-        chunks = tuple(array.chunks[ax] if by.shape[ax] != 1 else (1,) for ax in range(-by.ndim, 0))
-
-        by = cubed.from_array(by, chunks=chunks, spec=array.spec)
-    _, (array, by) = cubed.core.unify_chunks(array, inds, by, inds[-by.ndim :])
-
-    # Cubed's groupby_reduction handles the generation of "intermediates", and the
-    # "map-reduce" combination step, so we don't have to do that here.
-    # Only the equivalent of "_simple_combine" is supported, there is no
-    # support for "_grouped_combine".
-    labels_are_unknown = is_chunked_array(by_input) and expected_groups is None
-    do_simple_combine = not _is_arg_reduction(agg) and not labels_are_unknown
-
-    assert do_simple_combine
-    assert method == "map-reduce"
-    assert expected_groups is not None
-    assert reindex is True
-    assert len(axis) == 1  # one axis/grouping
-
-    def _groupby_func(a, by, axis, intermediate_dtype, num_groups):
-        blockwise_method = partial(
-            _get_chunk_reduction(agg.reduction_type),
-            func=agg.chunk,
-            fill_value=agg.fill_value["intermediate"],
-            dtype=agg.dtype["intermediate"],
-            reindex=reindex,
-            user_dtype=agg.dtype["user"],
+            by = cubed.from_array(by, chunks=chunks, spec=array.spec)
+        _, (array, by) = cubed.core.unify_chunks(array, inds, by, inds[-by.ndim :])
+
+        # Cubed's groupby_reduction handles the generation of "intermediates", and the
+        # "map-reduce" combination step, so we don't have to do that here.
+        # Only the equivalent of "_simple_combine" is supported, there is no
+        # support for "_grouped_combine".
+        labels_are_unknown = is_chunked_array(by_input) and expected_groups is None
+        do_simple_combine = not _is_arg_reduction(agg) and not labels_are_unknown
+
+        assert do_simple_combine
+        assert method == "map-reduce"
+        assert expected_groups is not None
+        assert reindex is True
+        assert len(axis) == 1  # one axis/grouping
+
+        def _groupby_func(a, by, axis, intermediate_dtype, num_groups):
+            blockwise_method = partial(
+                _get_chunk_reduction(agg.reduction_type),
+                func=agg.chunk,
+                fill_value=agg.fill_value["intermediate"],
+                dtype=agg.dtype["intermediate"],
+                reindex=reindex,
+                user_dtype=agg.dtype["user"],
+                axis=axis,
+                expected_groups=expected_groups,
+                engine=engine,
+                sort=sort,
+            )
+            out = blockwise_method(a, by)
+            # Convert dict to one that cubed understands, dropping groups since they are
+            # known, and the same for every block.
+            return {
+                f"f{idx}": intermediate for idx, intermediate in enumerate(out["intermediates"])
+            }
+
+        def _groupby_combine(a, axis, dummy_axis, dtype, keepdims):
+            # this is similar to _simple_combine, except the dummy axis and concatenation is handled by cubed
+            # only combine over the dummy axis, to preserve grouping along 'axis'
+            dtype = dict(dtype)
+            out = {}
+            for idx, combine in enumerate(agg.simple_combine):
+                field = f"f{idx}"
+                out[field] = combine(a[field], axis=dummy_axis, keepdims=keepdims)
+            return out
+
+        def _groupby_aggregate(a):
+            # Convert cubed dict to one that _finalize_results works with
+            results = {"groups": expected_groups, "intermediates": a.values()}
+            out = _finalize_results(results, agg, axis, expected_groups, fill_value, reindex)
+            return out[agg.name]
+
+        # convert list of dtypes to a structured dtype for cubed
+        intermediate_dtype = [(f"f{i}", dtype) for i, dtype in enumerate(agg.dtype["intermediate"])]
+        dtype = agg.dtype["final"]
+        num_groups = len(expected_groups)
+
+        result = cubed.core.groupby.groupby_reduction(
+            array,
+            by,
+            func=_groupby_func,
+            combine_func=_groupby_combine,
+            aggregate_func=_groupby_aggregate,
             axis=axis,
-            expected_groups=expected_groups,
-            engine=engine,
-            sort=sort,
+            intermediate_dtype=intermediate_dtype,
+            dtype=dtype,
+            num_groups=num_groups,
         )
-        out = blockwise_method(a, by)
-        # Convert dict to one that cubed understands, dropping groups since they are
-        # known, and the same for every block.
-        return {f"f{idx}": intermediate for idx, intermediate in enumerate(out["intermediates"])}
-
-    def _groupby_combine(a, axis, dummy_axis, dtype, keepdims):
-        # this is similar to _simple_combine, except the dummy axis and concatenation is handled by cubed
-        # only combine over the dummy axis, to preserve grouping along 'axis'
-        dtype = dict(dtype)
-        out = {}
-        for idx, combine in enumerate(agg.simple_combine):
-            field = f"f{idx}"
-            out[field] = combine(a[field], axis=dummy_axis, keepdims=keepdims)
-        return out
-
-    def _groupby_aggregate(a):
-        # Convert cubed dict to one that _finalize_results works with
-        results = {"groups": expected_groups, "intermediates": a.values()}
-        out = _finalize_results(results, agg, axis, expected_groups, fill_value, reindex)
-        return out[agg.name]
-
-    # convert list of dtypes to a structured dtype for cubed
-    intermediate_dtype = [(f"f{i}", dtype) for i, dtype in enumerate(agg.dtype["intermediate"])]
-    dtype = agg.dtype["final"]
-    num_groups = len(expected_groups)
-
-    result = cubed.core.groupby.groupby_reduction(
-        array,
-        by,
-        func=_groupby_func,
-        combine_func=_groupby_combine,
-        aggregate_func=_groupby_aggregate,
-        axis=axis,
-        intermediate_dtype=intermediate_dtype,
-        dtype=dtype,
-        num_groups=num_groups,
-    )
 
-    groups = (expected_groups.to_numpy(),)
+        groups = (expected_groups.to_numpy(),)
 
-    return (result, groups)
+        return (result, groups)
 
 
 def _collapse_blocks_along_axes(reduced: DaskArray, axis: T_Axes, group_chunks) -> DaskArray:
     import dask.array
     from dask.highlevelgraph import HighLevelGraph
 
     nblocks = tuple(reduced.numblocks[ax] for ax in axis)
@@ -2463,17 +2499,17 @@
     kwargs["engine"] = _choose_engine(by_, agg) if engine is None else engine
 
     groups: tuple[np.ndarray | DaskArray, ...]
     if has_cubed:
         if method is None:
             method = "map-reduce"
 
-        if method != "map-reduce":
+        if method not in ("map-reduce", "blockwise"):
             raise NotImplementedError(
-                "Reduction for Cubed arrays is only implemented for method 'map-reduce'."
+                "Reduction for Cubed arrays is only implemented for methods 'map-reduce' and 'blockwise'."
             )
 
         partial_agg = partial(cubed_groupby_agg, **kwargs)
 
         result, groups = partial_agg(
             array,
             by_,
```

### Comparing `flox-0.9.7/flox/visualize.py` & `flox-0.9.8/flox/visualize.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/flox/xarray.py` & `flox-0.9.8/flox/xarray.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/flox/xrdtypes.py` & `flox-0.9.8/flox/xrdtypes.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/flox/xrutils.py` & `flox-0.9.8/flox/xrutils.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/flox.egg-info/PKG-INFO` & `flox-0.9.8/flox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flox
-Version: 0.9.7
+Version: 0.9.8
 Summary: GroupBy operations for dask.array
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flox-0.9.7/flox.egg-info/SOURCES.txt` & `flox-0.9.8/flox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/pyproject.toml` & `flox-0.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/tests/__init__.py` & `flox-0.9.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.7/tests/test_core.py` & `flox-0.9.8/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1201,14 +1201,48 @@
         expected_groups=edges,
         **kwargs,
     )
     expected = np.broadcast_to(expected, (2, 3, expected.shape[-1]))
     assert_equal(expected, actual)
 
 
+@requires_cubed
+@pytest.mark.parametrize("method", ["blockwise", "map-reduce"])
+def test_group_by_datetime_cubed(engine, method):
+    kwargs = dict(
+        func="mean",
+        method=method,
+        engine=engine,
+    )
+    t = pd.date_range("2000-01-01", "2000-12-31", freq="D").to_series()
+    data = t.dt.dayofyear
+    cubedarray = cubed.from_array(data.values, chunks=30)
+
+    actual, _ = groupby_reduce(cubedarray, t, **kwargs)
+    expected = data.to_numpy().astype(float)
+    assert_equal(expected, actual)
+
+    edges = pd.date_range("1999-12-31", "2000-12-31", freq="ME").to_series().to_numpy()
+    actual, _ = groupby_reduce(
+        cubedarray, t.to_numpy(), isbin=True, expected_groups=edges, **kwargs
+    )
+    expected = data.resample("ME").mean().to_numpy()
+    assert_equal(expected, actual)
+
+    actual, _ = groupby_reduce(
+        cubed.array_api.broadcast_to(cubedarray, (2, 3, cubedarray.shape[-1])),
+        t.to_numpy(),
+        isbin=True,
+        expected_groups=edges,
+        **kwargs,
+    )
+    expected = np.broadcast_to(expected, (2, 3, expected.shape[-1]))
+    assert_equal(expected, actual)
+
+
 def test_factorize_values_outside_bins():
     # pd.factorize returns intp
     vals = factorize_(
         (np.arange(10).reshape(5, 2), np.arange(10).reshape(5, 2)),
         axes=(0, 1),
         expected_groups=(
             pd.IntervalIndex.from_breaks(np.arange(2, 8, 1)),
```

### Comparing `flox-0.9.7/tests/test_xarray.py` & `flox-0.9.8/tests/test_xarray.py`

 * *Files identical despite different names*

