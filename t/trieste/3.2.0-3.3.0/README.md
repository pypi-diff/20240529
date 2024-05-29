# Comparing `tmp/trieste-3.2.0.tar.gz` & `tmp/trieste-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trieste-3.2.0.tar", last modified: Thu May  9 09:27:45 2024, max compression
+gzip compressed data, was "trieste-3.3.0.tar", last modified: Wed May 29 10:35:53 2024, max compression
```

## Comparing `trieste-3.2.0.tar` & `trieste-3.3.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.022075 trieste-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-09 09:27:37.000000 trieste-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-09 09:27:45.022075 trieste-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-09 09:27:37.000000 trieste-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-09 09:27:37.000000 trieste-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:27:45.022075 trieste-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-09 09:27:37.000000 trieste-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.010075 trieste-3.2.0/trieste/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.010075 trieste-3.2.0/trieste/acquisition/
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/combination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.014075 trieste-3.2.0/trieste/acquisition/function/
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20754 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/active_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/continuous_thompson_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)    36585 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    77644 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    35334 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/greedy_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    33916 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/multi_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16951 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.014075 trieste-3.2.0/trieste/acquisition/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/multi_objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/multi_objective/dominance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/multi_objective/pareto.py
--rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/multi_objective/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)    42509 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)   117386 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27114 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/ask_tell_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    49911 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/bayesian_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.014075 trieste-3.2.0/trieste/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.014075 trieste-3.2.0/trieste/experimental/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/experimental/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/experimental/plotting/inequality_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    23612 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/experimental/plotting/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/experimental/plotting/plotting_plotly.py
--rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.014075 trieste-3.2.0/trieste/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.018075 trieste-3.2.0/trieste/models/gpflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27404 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/inducing_point_selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    91274 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    41061 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.018075 trieste-3.2.0/trieste/models/gpflux/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflux/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflux/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflux/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    20658 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflux/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    31342 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.018075 trieste-3.2.0/trieste/models/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15525 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/architectures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    26847 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.018075 trieste-3.2.0/trieste/objectives/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/objectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/objectives/multi_objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/objectives/multifidelity_objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)    24268 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/objectives/single_objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/objectives/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/observer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    54241 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.018075 trieste-3.2.0/trieste/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13957 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.022075 trieste-3.2.0/trieste.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-09 09:27:44.000000 trieste-3.2.0/trieste.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-09 09:27:45.000000 trieste-3.2.0/trieste.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:27:44.000000 trieste-3.2.0/trieste.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-09 09:27:44.000000 trieste-3.2.0/trieste.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 09:27:44.000000 trieste-3.2.0/trieste.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.552109 trieste-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 10:35:46.000000 trieste-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-29 10:35:53.552109 trieste-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-29 10:35:46.000000 trieste-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-29 10:35:46.000000 trieste-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:35:53.552109 trieste-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-29 10:35:46.000000 trieste-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.540109 trieste-3.3.0/trieste/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.544109 trieste-3.3.0/trieste/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/combination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.544109 trieste-3.3.0/trieste/acquisition/function/
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20754 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/continuous_thompson_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36585 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77644 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35334 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/greedy_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33916 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/multi_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16951 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.544109 trieste-3.3.0/trieste/acquisition/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/multi_objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/multi_objective/dominance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/multi_objective/pareto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/multi_objective/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42509 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120442 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29749 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/ask_tell_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51213 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/bayesian_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.544109 trieste-3.3.0/trieste/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.548109 trieste-3.3.0/trieste/experimental/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/experimental/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/experimental/plotting/inequality_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23612 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/experimental/plotting/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/experimental/plotting/plotting_plotly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.548109 trieste-3.3.0/trieste/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.548109 trieste-3.3.0/trieste/models/gpflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27404 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/inducing_point_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91274 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41061 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.548109 trieste-3.3.0/trieste/models/gpflux/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflux/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflux/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflux/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20658 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflux/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31342 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.552109 trieste-3.3.0/trieste/models/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15525 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26847 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.552109 trieste-3.3.0/trieste/objectives/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/objectives/multi_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/objectives/multifidelity_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24268 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/objectives/single_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/objectives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54291 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.552109 trieste-3.3.0/trieste/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13957 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.552109 trieste-3.3.0/trieste.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-29 10:35:53.000000 trieste-3.3.0/trieste.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-29 10:35:53.000000 trieste-3.3.0/trieste.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:35:53.000000 trieste-3.3.0/trieste.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-29 10:35:53.000000 trieste-3.3.0/trieste.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 10:35:53.000000 trieste-3.3.0/trieste.egg-info/top_level.txt
```

### Comparing `trieste-3.2.0/LICENSE` & `trieste-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/PKG-INFO` & `trieste-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trieste
-Version: 3.2.0
+Version: 3.3.0
 Summary: A Bayesian optimization research toolbox built on TensorFlow
 Home-page: https://github.com/secondmind-labs/trieste
 Author: The Trieste contributors
 Author-email: labs@secondmind.ai
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `trieste-3.2.0/README.md` & `trieste-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/pyproject.toml` & `trieste-3.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/setup.py` & `trieste-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/__init__.py` & `trieste-3.3.0/trieste/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/__init__.py` & `trieste-3.3.0/trieste/acquisition/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/combination.py` & `trieste-3.3.0/trieste/acquisition/combination.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/function/__init__.py` & `trieste-3.3.0/trieste/acquisition/function/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/function/active_learning.py` & `trieste-3.3.0/trieste/acquisition/function/active_learning.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/function/continuous_thompson_sampling.py` & `trieste-3.3.0/trieste/acquisition/function/continuous_thompson_sampling.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/function/entropy.py` & `trieste-3.3.0/trieste/acquisition/function/entropy.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/function/function.py` & `trieste-3.3.0/trieste/acquisition/function/function.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/function/greedy_batch.py` & `trieste-3.3.0/trieste/acquisition/function/greedy_batch.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/function/multi_objective.py` & `trieste-3.3.0/trieste/acquisition/function/multi_objective.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/function/utils.py` & `trieste-3.3.0/trieste/acquisition/function/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/interface.py` & `trieste-3.3.0/trieste/acquisition/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/multi_objective/__init__.py` & `trieste-3.3.0/trieste/acquisition/multi_objective/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/multi_objective/dominance.py` & `trieste-3.3.0/trieste/acquisition/multi_objective/dominance.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/multi_objective/pareto.py` & `trieste-3.3.0/trieste/acquisition/multi_objective/pareto.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/multi_objective/partition.py` & `trieste-3.3.0/trieste/acquisition/multi_objective/partition.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/optimizer.py` & `trieste-3.3.0/trieste/acquisition/optimizer.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/rule.py` & `trieste-3.3.0/trieste/acquisition/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,22 +166,23 @@
             )
         return self.acquire(
             search_space,
             {OBJECTIVE: model},
             datasets=None if dataset is None else {OBJECTIVE: dataset},
         )
 
+    # AcquisitionRule should really have been generic in StateType, but that's too big a change now
     def filter_datasets(
         self, models: Mapping[Tag, ProbabilisticModelType], datasets: Mapping[Tag, Dataset]
-    ) -> Mapping[Tag, Dataset]:
+    ) -> Mapping[Tag, Dataset] | State[Any | None, Mapping[Tag, Dataset]]:
         """
         Filter the post-acquisition datasets before they are used for model training. For example,
         this can be used to remove points from the post-acquisition datasets that are no longer in
         the search space.
-        Some rules may also update their internal state.
+        Rules that need to update their internal state should return a State callable.
 
         :param models: The model for each tag.
         :param datasets: The updated datasets after previous acquisition step.
         :return: The filtered datasets.
         """
         # No filtering by default.
         return datasets
@@ -194,14 +195,18 @@
     by :class:`BatchTrustRegion`."""
 
     @property
     @abstractmethod
     def num_local_datasets(self) -> int:
         """The number of local datasets required by this rule."""
 
+    @abstractmethod
+    def initialize_subspaces(self, search_space: SearchSpaceType) -> None:
+        """Create local subspaces for when no initial subspaces are provided."""
+
 
 class EfficientGlobalOptimization(
     AcquisitionRule[TensorType, SearchSpaceType, ProbabilisticModelType]
 ):
     """Implements the Efficient Global Optimization, or EGO, algorithm."""
 
     @overload
@@ -1236,42 +1241,53 @@
             }
 
 
 UpdatableTrustRegionType = TypeVar("UpdatableTrustRegionType", bound=UpdatableTrustRegion)
 """ A type variable bound to :class:`UpdatableTrustRegion`. """
 
 
+@dataclass(frozen=True)
+class BatchTrustRegionState(Generic[UpdatableTrustRegionType]):
+    """The acquisition state for the :class:`BatchTrustRegion` acquisition rule."""
+
+    subspaces: Sequence[UpdatableTrustRegionType]
+    """ The acquisition space's subspaces. """
+
+    subspace_tags: Sequence[str]
+    """ The subspaces' tags. """
+
+    def __deepcopy__(
+        self, memo: dict[int, object]
+    ) -> BatchTrustRegionState[UpdatableTrustRegionType]:
+        subspaces_copy = copy.deepcopy(self.subspaces)
+        return BatchTrustRegionState(subspaces_copy, self.subspace_tags)
+
+    @property
+    def acquisition_space(self) -> TaggedMultiSearchSpace:
+        """The acquisition search space."""
+        return TaggedMultiSearchSpace(self.subspaces, self.subspace_tags)
+
+
 class BatchTrustRegion(
     LocalDatasetsAcquisitionRule[
-        types.State[Optional["BatchTrustRegion.State"], TensorType],
+        types.State[Optional[BatchTrustRegionState[UpdatableTrustRegionType]], TensorType],
         SearchSpace,
         ProbabilisticModelType,
     ],
     Generic[ProbabilisticModelType, UpdatableTrustRegionType],
 ):
     """Abstract class for multi trust region acquisition rules. These are batch algorithms where
     each query point is optimized in parallel, with its own separate trust region.
 
     Note: to restart or continue an optimization with this rule, either the same instance of the
     rule must be used, or a new instance must be created with the subspaces from a previous
     state. This is because the internal state of the rule cannot be restored directly from a state
     object.
     """
 
-    @dataclass(frozen=True)
-    class State:
-        """The acquisition state for the :class:`BatchTrustRegion` acquisition rule."""
-
-        acquisition_space: TaggedMultiSearchSpace
-        """ The search space. """
-
-        def __deepcopy__(self, memo: dict[int, object]) -> BatchTrustRegion.State:
-            acquisition_space_copy = copy.deepcopy(self.acquisition_space, memo)
-            return BatchTrustRegion.State(acquisition_space_copy)
-
     def __init__(
         self: "BatchTrustRegion[ProbabilisticModelType, UpdatableTrustRegionType]",
         init_subspaces: Union[
             None, UpdatableTrustRegionType, Sequence[UpdatableTrustRegionType]
         ] = None,
         rule: AcquisitionRule[TensorType, SearchSpace, ProbabilisticModelType] | None = None,
     ):
@@ -1283,46 +1299,46 @@
             subspace.
 
             If `None`, defaults to :class:`~trieste.acquisition.DiscreteThompsonSampling` with
             a batch size of 1 for `TURBOBox` subspaces, and
             :class:`~trieste.acquisition.EfficientGlobalOptimization` otherwise.
         """
         # If init_subspaces are not provided, leave it to the subclasses to create them.
-        self._subspaces = None
+        self._init_subspaces = None
         self._tags = None
         if init_subspaces is not None:
             if not isinstance(init_subspaces, Sequence):
                 init_subspaces = [init_subspaces]
-            self._subspaces = tuple(init_subspaces)
-            for index, subspace in enumerate(self._subspaces):
+            self._init_subspaces = tuple(init_subspaces)
+            for index, subspace in enumerate(self._init_subspaces):
                 subspace.region_index = index  # Override the index.
-            self._tags = tuple(str(index) for index in range(len(init_subspaces)))
+            self._tags = tuple(str(index) for index, _ in enumerate(self._init_subspaces))
 
         self._rule = rule
         # The rules for each subspace. These are only used when we want to run the base rule
         # sequentially for each subspace. Theses are set in `acquire`.
         self._rules: Optional[
             Sequence[AcquisitionRule[TensorType, SearchSpace, ProbabilisticModelType]]
         ] = None
 
     def __repr__(self) -> str:
         """"""
-        return f"""{self.__class__.__name__}({self._subspaces!r}, {self._rule!r})"""
+        return f"""{self.__class__.__name__}({self._init_subspaces!r}, {self._rule!r})"""
 
     @property
     def num_local_datasets(self) -> int:
-        assert self._subspaces is not None, "the subspaces have not been initialized"
-        return len(self._subspaces)
+        assert self._init_subspaces is not None, "the subspaces have not been initialized"
+        return len(self._init_subspaces)
 
     def acquire(
         self,
         search_space: SearchSpace,
         models: Mapping[Tag, ProbabilisticModelType],
         datasets: Optional[Mapping[Tag, Dataset]] = None,
-    ) -> types.State[State | None, TensorType]:
+    ) -> types.State[BatchTrustRegionState[UpdatableTrustRegionType] | None, TensorType]:
         """
         Use the ``rule`` specified at :meth:`~BatchTrustRegion.__init__` to find new
         query points. Return a function that constructs these points given a previous trust region
         state.
 
         If state is None, initialize the subspaces by picking new locations. Otherwise,
         update the existing subspaces.
@@ -1332,22 +1348,25 @@
         :param search_space: The acquisition search space for *this step*.
         :param models: The model for each tag.
         :param datasets: The known observer query points and observations for each tag.
         :return: A function that constructs the next acquisition state and the recommended query
             points from the previous acquisition state.
         """
 
-        # Subspaces should be set by the time we call `acquire`.
+        # initialize subspaces
+        self.initialize_subspaces(search_space)
+
+        # Subspaces should be initialised by the time we call `acquire`.
         assert self._tags is not None
-        assert self._subspaces is not None
+        assert self._init_subspaces is not None
 
         # Implement heuristic defaults for the rule if not specified by the user.
         if self._rule is None:
             # Use first subspace to determine the type of the base rule.
-            if isinstance(self._subspaces[0], TURBOBox):
+            if isinstance(self._init_subspaces[0], TURBOBox):
                 # Default to Thompson sampling with batches of size 1.
                 self._rule = DiscreteThompsonSampling(
                     tf.minimum(100 * search_space.dimension, 5_000), 1
                 )
             else:
                 self._rule = EfficientGlobalOptimization()
 
@@ -1376,39 +1395,41 @@
         # have a list of rules in `self._rules`.
         if self._rules is None and not (
             _num_local_models == 0 and isinstance(self._rule, EfficientGlobalOptimization)
         ):
             self._rules = [copy.deepcopy(self._rule) for _ in range(num_subspaces)]
 
         def state_func(
-            state: BatchTrustRegion.State | None,
-        ) -> Tuple[BatchTrustRegion.State | None, TensorType]:
+            state: BatchTrustRegionState[UpdatableTrustRegionType] | None,
+        ) -> Tuple[BatchTrustRegionState[UpdatableTrustRegionType] | None, TensorType]:
             # Check again to keep mypy happy.
             assert self._tags is not None
-            assert self._subspaces is not None
+            assert self._init_subspaces is not None
             assert self._rule is not None
 
-            # If state is set, the tags should be the same as the tags of the acquisition space
-            # in the state.
+            # If state is set, the tags should be the same as the tags of the initial space.
             if state is not None:
-                assert (
-                    self._tags == state.acquisition_space.subspace_tags
-                ), f"""The tags of the state acquisition space
-                    {state.acquisition_space.subspace_tags} should be the same as the tags of the
-                    BatchTrustRegion acquisition rule {self._tags}"""
-
-            # Never use the subspaces from the passed in state, as we may have modified the
-            # subspaces in filter_datasets.
-            acquisition_space = TaggedMultiSearchSpace(self._subspaces, self._tags)
+                assert self._tags == tuple(state.subspace_tags), (
+                    f"The tags of the state acquisition space "
+                    f"{state.subspace_tags} should be the same as the tags of the "
+                    f"BatchTrustRegion acquisition rule {self._tags}"
+                )
+                assert len(state.subspaces) == len(state.subspace_tags), (
+                    f"Inconsistent number of subspaces: {len(state.subspaces)} subspaces"
+                    f"and {len(state.subspace_tags)} tags"
+                )
+                subspaces = state.subspaces
+            else:
+                subspaces = self._init_subspaces
 
             # If the base rule is a sequence, run it sequentially for each subspace.
             # See earlier comments.
             if self._rules is not None:
                 _points = []
-                for subspace, rule in zip(self._subspaces, self._rules):
+                for tag, subspace, rule in zip(self._tags, subspaces, self._rules):
                     _models = subspace.select_in_region(models)
                     _datasets = subspace.select_in_region(datasets)
                     assert _models is not None
                     # Remap all local tags to global ones. One reason is that single model
                     # acquisition builders expect OBJECTIVE to exist.
                     _models = {
                         LocalizedTag.from_tag(tag).global_tag: model
@@ -1430,19 +1451,19 @@
                     _datasets = {
                         tag: dataset
                         for tag, dataset in datasets.items()
                         if not LocalizedTag.from_tag(tag).is_local
                     }
                 else:
                     _datasets = None
+                acquisition_space = TaggedMultiSearchSpace(subspaces, self._tags)
                 points = self._rule.acquire(acquisition_space, models, _datasets)
 
-            # We may modify the regions in filter_datasets later, so return a copy.
-            state_ = BatchTrustRegion.State(copy.deepcopy(acquisition_space))
-            return state_, tf.reshape(points, [-1, len(self._subspaces), points.shape[-1]])
+            state_ = BatchTrustRegionState(subspaces, self._tags)
+            return state_, tf.reshape(points, [-1, len(subspaces), points.shape[-1]])
 
         return state_func
 
     def maybe_initialize_subspaces(
         self,
         subspaces: Sequence[UpdatableTrustRegionType],
         models: Mapping[Tag, ProbabilisticModelType],
@@ -1484,54 +1505,78 @@
         :param models: The model for each tag.
         :param datasets: The dataset for each tag.
         :return: A boolean mask of length V, where V is the number of subspaces.
         """
 
     def filter_datasets(
         self, models: Mapping[Tag, ProbabilisticModelType], datasets: Mapping[Tag, Dataset]
-    ) -> Mapping[Tag, Dataset]:
-        # Update subspaces with the latest datasets.
-        assert self._subspaces is not None
-        for subspace in self._subspaces:
-            # Re-initialize or update the subspace, depending on the property.
-            if subspace.requires_initialization:
-                subspace.initialize(models, datasets)
+    ) -> types.State[BatchTrustRegionState[UpdatableTrustRegionType] | None, Mapping[Tag, Dataset]]:
+        def state_func(
+            state: BatchTrustRegionState[UpdatableTrustRegionType] | None,
+        ) -> Tuple[BatchTrustRegionState[UpdatableTrustRegionType] | None, Mapping[Tag, Dataset]]:
+            if state is not None:
+                assert self._tags == state.subspace_tags, (
+                    f"The tags of the state acquisition space "
+                    f"{state.subspace_tags} should be the same as the tags of the "
+                    f"BatchTrustRegion acquisition rule {self._tags}"
+                )
+                assert len(state.subspaces) == len(state.subspace_tags), (
+                    f"Inconsistent number of subspaces: {len(state.subspaces)} subspaces"
+                    f"and {len(state.subspace_tags)} tags"
+                )
+                subspaces = tuple(state.subspaces)
             else:
-                subspace.update(models, datasets)
-        self.maybe_initialize_subspaces(self._subspaces, models, datasets)
+                assert self._init_subspaces is not None, "the subspaces have not been initialized"
+                assert self._tags is not None
+                subspaces = self._init_subspaces
+
+            # make a deepcopy to avoid modifying any user copies
+            subspaces = copy.deepcopy(subspaces)
+
+            # Update subspaces with the latest datasets.
+            for subspace in subspaces:
+                # Re-initialize or update the subspace, depending on the property.
+                if subspace.requires_initialization:
+                    subspace.initialize(models, datasets)
+                else:
+                    subspace.update(models, datasets)
+            self.maybe_initialize_subspaces(subspaces, models, datasets)
 
-        # Filter out points that are not in any of the subspaces. This is done by creating a mask
-        # for each local dataset that is True for points that are in any subspace.
-        used_masks = {
-            tag: tf.zeros(dataset.query_points.shape[:-1], dtype=tf.bool)
-            for tag, dataset in datasets.items()
-            if LocalizedTag.from_tag(tag).is_local
-        }
+            # Filter out points that are not in any of the subspaces. This is done by creating a
+            # mask for each local dataset that is True for points that are in any subspace.
+            used_masks = {
+                tag: tf.zeros(dataset.query_points.shape[:-1], dtype=tf.bool)
+                for tag, dataset in datasets.items()
+                if LocalizedTag.from_tag(tag).is_local
+            }
 
-        for subspace in self._subspaces:
-            in_region_masks = subspace.get_datasets_filter_mask(datasets)
-            if in_region_masks is not None:
-                for tag, in_region in in_region_masks.items():
-                    ltag = LocalizedTag.from_tag(tag)
-                    assert ltag.is_local, f"can only filter local tags, got {tag}"
-                    used_masks[tag] = tf.logical_or(used_masks[tag], in_region)
-
-        filtered_datasets = {}
-        for tag, used_mask in used_masks.items():
-            filtered_datasets[tag] = Dataset(
-                tf.boolean_mask(datasets[tag].query_points, used_mask),
-                tf.boolean_mask(datasets[tag].observations, used_mask),
-            )
-
-        # Include global datasets unmodified.
-        for tag, dataset in datasets.items():
-            if not LocalizedTag.from_tag(tag).is_local:
-                filtered_datasets[tag] = dataset
+            for subspace in subspaces:
+                in_region_masks = subspace.get_datasets_filter_mask(datasets)
+                if in_region_masks is not None:
+                    for tag, in_region in in_region_masks.items():
+                        ltag = LocalizedTag.from_tag(tag)
+                        assert ltag.is_local, f"can only filter local tags, got {tag}"
+                        used_masks[tag] = tf.logical_or(used_masks[tag], in_region)
+
+            filtered_datasets = {}
+            for tag, used_mask in used_masks.items():
+                filtered_datasets[tag] = Dataset(
+                    tf.boolean_mask(datasets[tag].query_points, used_mask),
+                    tf.boolean_mask(datasets[tag].observations, used_mask),
+                )
 
-        return filtered_datasets
+            # Include global datasets unmodified.
+            for tag, dataset in datasets.items():
+                if not LocalizedTag.from_tag(tag).is_local:
+                    filtered_datasets[tag] = dataset
+
+            state_ = BatchTrustRegionState(subspaces, self._tags)
+            return state_, filtered_datasets
+
+        return state_func
 
 
 class HypercubeTrustRegion(UpdatableTrustRegion):
     """
     An abstract updatable trust region that defines a hypercube region in the global search space.
     The region is defined by a location and a size in each dimension. This class is used to
     implement different types of search spaces, e.g. continuous (SingleObjectiveTrustRegionBox) and
@@ -1572,15 +1617,15 @@
         # Randomly pick initial value of `self.location` for setting the bounds from the
         # global search space.
         self._init_location()
         self._init_eps()
         self._update_domain()
         # Initial value of the region minimum is set to infinity as we have not yet observed any
         # data.
-        self._y_min = np.inf
+        self._y_min = tf.constant(np.inf, dtype=self.location.dtype)
 
     def _init_eps(self) -> None:
         self.eps = self._zeta * (self.global_search_space.upper - self.global_search_space.lower)
 
     @abstractmethod
     def _update_domain(self) -> None:
         """Update the local domain of the region."""
@@ -1616,15 +1661,17 @@
         # dataset. Per tag it return a local dataset with a matching region index where it can;
         # failing that it will return the global dataset for that tag.
         datasets = self.select_in_region(datasets)
         self._init_location(models, datasets, location_candidate=location_candidate)
         self._step_is_success = False
         self._init_eps()
         self._update_domain()
-        _, self._y_min = self.get_dataset_min(datasets)
+        # We haven't necessarily observed any data yet for this region; force first step to always
+        # be successful by setting the minimum to infinity.
+        self._y_min = tf.constant(np.inf, dtype=self.location.dtype)
         self._initialized = True
 
     def update(
         self,
         models: Optional[Mapping[Tag, ProbabilisticModelType]] = None,
         datasets: Optional[Mapping[Tag, Dataset]] = None,
     ) -> None:
@@ -1815,51 +1862,53 @@
 
 class BatchTrustRegionBox(BatchTrustRegion[ProbabilisticModelType, UpdatableTrustRegionBox]):
     """
     Implements the :class:`BatchTrustRegion` *trust region* acquisition rule for box regions.
     This is intended to be used for single-objective optimization with batching.
     """
 
-    def acquire(
-        self,
-        search_space: SearchSpace,
-        models: Mapping[Tag, ProbabilisticModelType],
-        datasets: Optional[Mapping[Tag, Dataset]] = None,
-    ) -> types.State[BatchTrustRegion.State | None, TensorType]:
-        if self._subspaces is None:
-            # If no initial subspaces were provided, create N default subspaces, where N is the
-            # number of query points in the base-rule.
-            # Currently the detection for N is only implemented for EGO.
-            # Note: the reason we don't create the default subspaces in `__init__` is because we
-            # don't have the global search space at that point.
+    def initialize_subspaces(self, search_space: SearchSpace) -> None:
+        # If no initial subspaces were provided, create N default subspaces, where N is the
+        # number of query points in the base-rule.
+        # Currently the detection for N is only implemented for EGO.
+        # Note: the reason we don't create the default subspaces in `__init__` is because we
+        # don't have the global search space at that point.
+        if self._init_subspaces is None:
             if isinstance(self._rule, EfficientGlobalOptimization):
                 num_query_points = self._rule._num_query_points
             else:
                 num_query_points = 1
 
             assert isinstance(
                 search_space, Box
             ), f"search space should be a Box, got {type(search_space)}"
             init_subspaces: Tuple[UpdatableTrustRegionBox, ...] = tuple(
                 SingleObjectiveTrustRegionBox(search_space) for _ in range(num_query_points)
             )
-            self._subspaces = init_subspaces
-            for index, subspace in enumerate(self._subspaces):
+            self._init_subspaces = init_subspaces
+            for index, subspace in enumerate(self._init_subspaces):
                 subspace.region_index = index  # Override the index.
             self._tags = tuple(str(index) for index in range(self.num_local_datasets))
 
+    def acquire(
+        self,
+        search_space: SearchSpace,
+        models: Mapping[Tag, ProbabilisticModelType],
+        datasets: Optional[Mapping[Tag, Dataset]] = None,
+    ) -> types.State[BatchTrustRegionState[UpdatableTrustRegionBox] | None, TensorType]:
         # Ensure passed in global search space is always the same as the search space passed to
         # the subspaces.
-        for subspace in self._subspaces:
-            assert subspace.global_search_space == search_space, (
-                "The global search space of the subspaces should be the same as the "
-                "search space passed to the BatchTrustRegionBox acquisition rule. "
-                "If you want to change the global search space, you should recreate the rule. "
-                "Note: all subspaces should be initialized with the same global search space."
-            )
+        if self._init_subspaces is not None:
+            for subspace in self._init_subspaces:
+                assert subspace.global_search_space == search_space, (
+                    "The global search space of the subspaces should be the same as the "
+                    "search space passed to the BatchTrustRegionBox acquisition rule. "
+                    "If you want to change the global search space, you should recreate the rule. "
+                    "Note: all subspaces should be initialized with the same global search space."
+                )
 
         return super().acquire(search_space, models, datasets)
 
     @inherit_check_shapes
     def get_initialize_subspaces_mask(
         self,
         subspaces: Sequence[UpdatableTrustRegionBox],
@@ -1893,24 +1942,26 @@
     """
 
     def __init__(
         self,
         global_search_space: Box,
         beta: float = 0.7,
         kappa: float = 1e-4,
+        zeta: float = 0.5,
         min_eps: float = 1e-2,
         region_index: Optional[int] = None,
         input_active_dims: Optional[Union[slice, Sequence[int]]] = None,
     ):
         self._is_global = False
         super().__init__(
-            global_search_space,
-            beta,
-            kappa,
-            min_eps,
+            global_search_space=global_search_space,
+            beta=beta,
+            kappa=kappa,
+            zeta=zeta,
+            min_eps=min_eps,
             region_index=region_index,
             input_active_dims=input_active_dims,
         )
 
     @property
     def eps(self) -> TensorType:
         """The size of the search space."""
@@ -2491,21 +2542,16 @@
     BatchTrustRegion[ProbabilisticModelType, UpdatableTrustRegionProduct]
 ):
     """
     Implements the :class:`BatchTrustRegion` *trust region* acquisition rule for mixed search
     spaces. This is intended to be used for single-objective optimization with batching.
     """
 
-    def acquire(
-        self,
-        search_space: SearchSpace,
-        models: Mapping[Tag, ProbabilisticModelType],
-        datasets: Optional[Mapping[Tag, Dataset]] = None,
-    ) -> types.State[BatchTrustRegion.State | None, TensorType]:
-        if self._subspaces is None:
+    def initialize_subspaces(self, search_space: SearchSpaceType) -> None:
+        if self._init_subspaces is None:
             # If no initial subspaces were provided, create N default subspaces, where N is the
             # number of query points in the base-rule.
             # Currently the detection for N is only implemented for EGO.
             # Note: the reason we don't create the default subspaces in `__init__` is because we
             # don't have the global search space at that point.
             if isinstance(self._rule, EfficientGlobalOptimization):
                 num_query_points = self._rule._num_query_points
@@ -2530,28 +2576,35 @@
                     else:
                         raise ValueError(f"unsupported search space type: {type(subspace)}")
                 return subregions
 
             init_subspaces: Tuple[UpdatableTrustRegionProduct, ...] = tuple(
                 UpdatableTrustRegionProduct(create_subregions()) for _ in range(num_query_points)
             )
-            self._subspaces = init_subspaces
-            for index, subspace in enumerate(self._subspaces):
+            self._init_subspaces = init_subspaces
+            for index, subspace in enumerate(self._init_subspaces):
                 subspace.region_index = index  # Override the index.
             self._tags = tuple(str(index) for index in range(self.num_local_datasets))
 
+    def acquire(
+        self,
+        search_space: SearchSpace,
+        models: Mapping[Tag, ProbabilisticModelType],
+        datasets: Optional[Mapping[Tag, Dataset]] = None,
+    ) -> types.State[BatchTrustRegionState[UpdatableTrustRegionProduct] | None, TensorType]:
         # Ensure passed in global search space is always the same as the search space passed to
         # the subspaces.
-        for subspace in self._subspaces:
-            assert subspace.global_search_space == search_space, (
-                "The global search space of the subspaces should be the same as the "
-                "search space passed to the BatchTrustRegionProduct acquisition rule. "
-                "If you want to change the global search space, you should recreate the rule. "
-                "Note: all subspaces should be initialized with the same global search space."
-            )
+        if self._init_subspaces is not None:
+            for subspace in self._init_subspaces:
+                assert subspace.global_search_space == search_space, (
+                    "The global search space of the subspaces should be the same as the "
+                    "search space passed to the BatchTrustRegionProduct acquisition rule. "
+                    "If you want to change the global search space, you should recreate the rule. "
+                    "Note: all subspaces should be initialized with the same global search space."
+                )
 
         return super().acquire(search_space, models, datasets)
 
     @inherit_check_shapes
     def get_initialize_subspaces_mask(
         self,
         subspaces: Sequence[UpdatableTrustRegionProduct],
```

### Comparing `trieste-3.2.0/trieste/acquisition/sampler.py` & `trieste-3.3.0/trieste/acquisition/sampler.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/acquisition/utils.py` & `trieste-3.3.0/trieste/acquisition/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/ask_tell_optimization.py` & `trieste-3.3.0/trieste/ask_tell_optimization.py`

 * *Files 6% similar despite different names*

```diff
@@ -221,15 +221,15 @@
             assumes that the initial datasets are global.
         :raise ValueError: If any of the following are true:
             - the keys in ``datasets`` and ``models`` do not match
             - ``datasets`` or ``models`` are empty
             - default acquisition is used but incompatible with other inputs
         """
         self._search_space = search_space
-        self._acquisition_state = acquisition_state
+        self._acquisition_record = self._acquisition_state = acquisition_state
 
         if not datasets or not models:
             raise ValueError("dicts of datasets and models must be populated.")
 
         if isinstance(datasets, Dataset):
             datasets = {OBJECTIVE: datasets}
         if not isinstance(models, Mapping):
@@ -284,15 +284,25 @@
                 else:
                     self._dataset_ixs = [
                         tf.range(self._dataset_len) for _ in range(num_local_datasets)
                     ]
                 datasets = with_local_datasets(
                     self._datasets, num_local_datasets, self._dataset_ixs
                 )
-        self._filtered_datasets = self._acquisition_rule.filter_datasets(self._models, datasets)
+            self._acquisition_rule.initialize_subspaces(search_space)
+
+        filtered_datasets: Mapping[Tag, Dataset] | State[
+            StateType | None, Mapping[Tag, Dataset]
+        ] = self._acquisition_rule.filter_datasets(self._models, datasets)
+        if callable(filtered_datasets):
+            self._acquisition_state, self._filtered_datasets = filtered_datasets(
+                self._acquisition_state
+            )
+        else:
+            self._filtered_datasets = filtered_datasets
 
         if fit_model:
             with Timer() as initial_model_fitting_timer:
                 for tag, model in self._models.items():
                     # Prefer local dataset if available.
                     tags = [tag, LocalizedTag.from_tag(tag).global_tag]
                     _, dataset = get_value_for_tag(self._filtered_datasets, *tags)
@@ -416,14 +426,16 @@
 
         :param record: Optimization state record.
         :param search_space: The space over which to search for the next query point.
         :param acquisition_rule: The acquisition rule, which defines how to search for a new point
             on each optimization step. Defaults to
             :class:`~trieste.acquisition.rule.EfficientGlobalOptimization` with default
             arguments.
+        :param track_data: Whether the optimizer tracks the changing datasets via a local copy.
+        :param local_data_ixs: Indices to local data for local rules with `track_data` False.
         :return: New instance of :class:`~AskTellOptimizer`.
         """
         # we are recovering previously saved optimization state
         # so the model was already trained
         # thus there is no need to train it again
 
         # type ignore below is because this relies on subclasses not overriding __init__
@@ -447,15 +459,18 @@
             is not supported for all model types. However, continuing the optimization will
             modify the original state.
         :return: An optimization state record.
         """
         try:
             datasets_copy = deepcopy(self._datasets) if copy else self._datasets
             models_copy = deepcopy(self._models) if copy else self._models
-            state_copy = deepcopy(self._acquisition_state) if copy else self._acquisition_state
+            # use the state as it was at acquisition time, not the one modified in
+            # filter_datasets in preparation for the next acquisition, so we can reinitialise
+            # the AskTellOptimizer using the record
+            state_copy = deepcopy(self._acquisition_record) if copy else self._acquisition_record
         except Exception as e:
             raise NotImplementedError(
                 "Failed to copy the optimization state. Some models do not support "
                 "deecopying (this is particularly common for deep neural network models). "
                 "For these models, the `copy` argument of the `to_record` or `to_result` "
                 "methods should be set to `False`. This means that the returned state may be "
                 "modified by subsequent optimization."
@@ -471,14 +486,47 @@
             is not supported for all model types. However, continuing the optimization will
             modify the original state.
         :return: A :class:`~trieste.data.OptimizationResult` object.
         """
         record: Record[StateType, ProbabilisticModelType] = self.to_record(copy=copy)
         return OptimizationResult(Ok(record), [])
 
+    @classmethod
+    def from_state(
+        cls: Type[AskTellOptimizerType],
+        state: AskTellOptimizerState[StateType, ProbabilisticModelType],
+        search_space: SearchSpaceType,
+        acquisition_rule: AcquisitionRule[
+            TensorType | State[StateType | None, TensorType],
+            SearchSpaceType,
+            ProbabilisticModelType,
+        ]
+        | None = None,
+        track_data: bool = True,
+    ) -> AskTellOptimizerType:
+        """Creates new :class:`~AskTellOptimizer` instance from provided AskTellOptimizer state.
+        Model training isn't triggered upon creation of the instance.
+
+        :param state: AskTellOptimizer state.
+        :param search_space: The space over which to search for the next query point.
+        :param acquisition_rule: The acquisition rule, which defines how to search for a new point
+            on each optimization step. Defaults to
+            :class:`~trieste.acquisition.rule.EfficientGlobalOptimization` with default
+            arguments.
+        :param track_data: Whether the optimizer tracks the changing datasets via a local copy.
+        :return: New instance of :class:`~AskTellOptimizer`.
+        """
+        return cls.from_record(  # type: ignore
+            state.record,
+            search_space,
+            acquisition_rule,
+            track_data=track_data,
+            local_data_ixs=state.local_data_ixs,
+        )
+
     def to_state(
         self, copy: bool = False
     ) -> AskTellOptimizerState[StateType, ProbabilisticModelType]:
         """Returns the AskTellOptimizer state, comprising the current optimization state
         alongside any internal AskTellOptimizer state.
 
         :param copy: Whether to return a copy of the current state or the original. Copying
@@ -507,14 +555,16 @@
         with Timer() as query_point_generation_timer:
             points_or_stateful = self._acquisition_rule.acquire(
                 self._search_space, self._models, datasets=self._filtered_datasets
             )
 
         if callable(points_or_stateful):
             self._acquisition_state, query_points = points_or_stateful(self._acquisition_state)
+            # also keep a copy of the state to return in to_record
+            self._acquisition_record = self._acquisition_state
         else:
             query_points = points_or_stateful
 
         summary_writer = logging.get_tensorboard_writer()
         if summary_writer:
             with summary_writer.as_default(step=logging.get_step_number()):
                 write_summary_query_points(
@@ -593,15 +643,21 @@
                         f"expected {num_local_datasets}"
                     )
                 for i in range(num_local_datasets):
                     self._dataset_ixs[i] = tf.concat([self._dataset_ixs[i], new_data_ixs[i]], -1)
             datasets = with_local_datasets(new_data, num_local_datasets, self._dataset_ixs)
             self._dataset_len = self.dataset_len(datasets)
 
-        self._filtered_datasets = self._acquisition_rule.filter_datasets(self._models, datasets)
+        filtered_datasets = self._acquisition_rule.filter_datasets(self._models, datasets)
+        if callable(filtered_datasets):
+            self._acquisition_state, self._filtered_datasets = filtered_datasets(
+                self._acquisition_state
+            )
+        else:
+            self._filtered_datasets = filtered_datasets
 
         with Timer() as model_fitting_timer:
             for tag, model in self._models.items():
                 # Always use the matching dataset to the model. If the model is
                 # local, then the dataset should be too by this stage.
                 dataset = self._filtered_datasets[tag]
                 self.update_model(model, dataset)
```

### Comparing `trieste-3.2.0/trieste/bayesian_optimizer.py` & `trieste-3.3.0/trieste/bayesian_optimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -705,14 +705,15 @@
                 SearchSpaceType, TrainableProbabilisticModelType
             ]()
 
         history: list[
             FrozenRecord[StateType, TrainableProbabilisticModelType]
             | Record[StateType, TrainableProbabilisticModelType]
         ] = []
+        history_state = acquisition_state
         query_plot_dfs: dict[int, pd.DataFrame] = {}
         observation_plot_dfs = observation_plot_init(datasets)
 
         summary_writer = logging.get_tensorboard_writer()
         if summary_writer:
             with summary_writer.as_default(step=0):
                 write_summary_init(
@@ -730,23 +731,26 @@
             if early_stop_callback and early_stop_callback(datasets, models, acquisition_state):
                 tf.print("Optimization terminated early", output_stream=absl.logging.INFO)
                 break
 
             try:
                 if track_state:
                     try:
+                        # note that we use the state as it was at acquisition time, not the one
+                        # modified in filter_datasets in preparation for the next acquisition,
+                        # so we can restart the optimization correctly (and also for plotting)
                         if track_path is None:
                             datasets_copy = copy.deepcopy(datasets)
                             models_copy = copy.deepcopy(models)
-                            acquisition_state_copy = copy.deepcopy(acquisition_state)
-                            record = Record(datasets_copy, models_copy, acquisition_state_copy)
+                            history_state_copy = copy.deepcopy(history_state)
+                            record = Record(datasets_copy, models_copy, history_state_copy)
                             history.append(record)
                         else:
                             track_path = Path(track_path)
-                            record = Record(datasets, models, acquisition_state)
+                            record = Record(datasets, models, history_state)
                             file_name = OptimizationResult.step_filename(step, num_steps)
                             history.append(record.save(track_path / file_name))
                     except Exception as e:
                         raise NotImplementedError(
                             "Failed to save the optimization state. Some models do not support "
                             "deecopying or serialization and cannot be saved. "
                             "(This is particularly common for deep neural network models, though "
@@ -759,15 +763,25 @@
 
                 if step == 1:
                     # See explanation in AskTellOptimizer.__init__().
                     if isinstance(acquisition_rule, LocalDatasetsAcquisitionRule):
                         datasets = with_local_datasets(
                             datasets, acquisition_rule.num_local_datasets
                         )
-                    filtered_datasets = acquisition_rule.filter_datasets(models, datasets)
+                        acquisition_rule.initialize_subspaces(self._search_space)
+
+                    filtered_datasets_or_callable: Mapping[Tag, Dataset] | State[
+                        StateType | None, Mapping[Tag, Dataset]
+                    ] = acquisition_rule.filter_datasets(models, datasets)
+                    if callable(filtered_datasets_or_callable):
+                        acquisition_state, filtered_datasets = filtered_datasets_or_callable(
+                            acquisition_state
+                        )
+                    else:
+                        filtered_datasets = filtered_datasets_or_callable
 
                     if fit_model and fit_initial_model:
                         with Timer() as initial_model_fitting_timer:
                             for tag, model in models.items():
                                 # Prefer local dataset if available.
                                 tags = [tag, LocalizedTag.from_tag(tag).global_tag]
                                 _, dataset = get_value_for_tag(filtered_datasets, *tags)
@@ -785,14 +799,15 @@
                 with Timer() as total_step_wallclock_timer:
                     with Timer() as query_point_generation_timer:
                         points_or_stateful = acquisition_rule.acquire(
                             self._search_space, models, datasets=filtered_datasets
                         )
                         if callable(points_or_stateful):
                             acquisition_state, query_points = points_or_stateful(acquisition_state)
+                            history_state = acquisition_state
                         else:
                             query_points = points_or_stateful
 
                     observer = self._observer
                     # If query_points are rank 3, then use a batched observer.
                     if tf.rank(query_points) == 3:
                         observer = mk_batch_observer(observer)
@@ -802,15 +817,24 @@
                         observer_output
                         if isinstance(observer_output, Mapping)
                         else {OBJECTIVE: observer_output}
                     )
 
                     for tag, new_dataset in tagged_output.items():
                         datasets[tag] += new_dataset
-                    filtered_datasets = acquisition_rule.filter_datasets(models, datasets)
+
+                    filtered_datasets_or_callable = acquisition_rule.filter_datasets(
+                        models, datasets
+                    )
+                    if callable(filtered_datasets_or_callable):
+                        acquisition_state, filtered_datasets = filtered_datasets_or_callable(
+                            acquisition_state
+                        )
+                    else:
+                        filtered_datasets = filtered_datasets_or_callable
 
                     with Timer() as model_fitting_timer:
                         if fit_model:
                             for tag, model in models.items():
                                 # Always use the matching dataset to the model. If the model is
                                 # local, then the dataset should be too by this stage.
                                 dataset = filtered_datasets[tag]
@@ -856,15 +880,15 @@
                 result = OptimizationResult(Err(error), history)
                 if track_state and track_path is not None:
                     result.save_result(Path(track_path) / OptimizationResult.RESULTS_FILENAME)
                 return result
 
         tf.print("Optimization completed without errors", output_stream=absl.logging.INFO)
 
-        record = Record(datasets, models, acquisition_state)
+        record = Record(datasets, models, history_state)
         result = OptimizationResult(Ok(record), history)
         if track_state and track_path is not None:
             result.save_result(Path(track_path) / OptimizationResult.RESULTS_FILENAME)
         return result
 
     def continue_optimization(
         self,
```

### Comparing `trieste-3.2.0/trieste/data.py` & `trieste-3.3.0/trieste/data.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/experimental/plotting/__init__.py` & `trieste-3.3.0/trieste/experimental/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/experimental/plotting/inequality_constraints.py` & `trieste-3.3.0/trieste/experimental/plotting/inequality_constraints.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/experimental/plotting/plotting.py` & `trieste-3.3.0/trieste/experimental/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/experimental/plotting/plotting_plotly.py` & `trieste-3.3.0/trieste/experimental/plotting/plotting_plotly.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/logging.py` & `trieste-3.3.0/trieste/logging.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/__init__.py` & `trieste-3.3.0/trieste/models/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/gpflow/__init__.py` & `trieste-3.3.0/trieste/models/gpflow/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/gpflow/builders.py` & `trieste-3.3.0/trieste/models/gpflow/builders.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/gpflow/inducing_point_selectors.py` & `trieste-3.3.0/trieste/models/gpflow/inducing_point_selectors.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/gpflow/interface.py` & `trieste-3.3.0/trieste/models/gpflow/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/gpflow/models.py` & `trieste-3.3.0/trieste/models/gpflow/models.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/gpflow/optimizer.py` & `trieste-3.3.0/trieste/models/gpflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/gpflow/sampler.py` & `trieste-3.3.0/trieste/models/gpflow/sampler.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/gpflow/utils.py` & `trieste-3.3.0/trieste/models/gpflow/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/gpflux/__init__.py` & `trieste-3.3.0/trieste/models/gpflux/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/gpflux/builders.py` & `trieste-3.3.0/trieste/models/gpflux/builders.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/gpflux/interface.py` & `trieste-3.3.0/trieste/models/gpflux/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/gpflux/models.py` & `trieste-3.3.0/trieste/models/gpflux/models.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/gpflux/sampler.py` & `trieste-3.3.0/trieste/models/gpflux/sampler.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/interfaces.py` & `trieste-3.3.0/trieste/models/interfaces.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/keras/__init__.py` & `trieste-3.3.0/trieste/models/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/keras/architectures.py` & `trieste-3.3.0/trieste/models/keras/architectures.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/keras/builders.py` & `trieste-3.3.0/trieste/models/keras/builders.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/keras/interface.py` & `trieste-3.3.0/trieste/models/keras/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/keras/models.py` & `trieste-3.3.0/trieste/models/keras/models.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/keras/sampler.py` & `trieste-3.3.0/trieste/models/keras/sampler.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/keras/utils.py` & `trieste-3.3.0/trieste/models/keras/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/optimizer.py` & `trieste-3.3.0/trieste/models/optimizer.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/models/utils.py` & `trieste-3.3.0/trieste/models/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/objectives/__init__.py` & `trieste-3.3.0/trieste/objectives/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/objectives/multi_objectives.py` & `trieste-3.3.0/trieste/objectives/multi_objectives.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/objectives/multifidelity_objectives.py` & `trieste-3.3.0/trieste/objectives/multifidelity_objectives.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/objectives/single_objectives.py` & `trieste-3.3.0/trieste/objectives/single_objectives.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/objectives/utils.py` & `trieste-3.3.0/trieste/objectives/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/observer.py` & `trieste-3.3.0/trieste/observer.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/space.py` & `trieste-3.3.0/trieste/space.py`

 * *Files 1% similar despite different names*

```diff
@@ -623,15 +623,15 @@
         start: int,
         num_samples: int,
         seed: Optional[int] = None,
     ) -> TensorType:
         # Internal common method to sample from the space using a Halton sequence.
         tf.debugging.assert_non_negative(num_samples)
         if num_samples == 0:
-            return tf.constant([])
+            return tf.constant([], dtype=self._lower.dtype)
         if seed is not None:  # ensure reproducibility
             tf.random.set_seed(seed)
         dim = tf.shape(self._lower)[-1]
         sequence_indices = tf.range(start=start, limit=start + num_samples, dtype=tf.int32)
         return (self._upper - self._lower) * tfp.mcmc.sample_halton_sequence(
             dim=dim, sequence_indices=sequence_indices, dtype=self._lower.dtype, seed=seed
         ) + self._lower
@@ -656,15 +656,15 @@
         :param num_samples: The number of points to sample from this search space.
         :param skip: The number of initial points of the Sobol sequence to skip
         :return: ``num_samples`` of points, using sobol sequence with shape '[num_samples, D]' ,
             where D is the search space dimension.
         """
         tf.debugging.assert_non_negative(num_samples)
         if num_samples == 0:
-            return tf.constant([])
+            return tf.constant([], dtype=self._lower.dtype)
         if skip is None:  # generate random skip
             skip = tf.random.uniform([1], maxval=2**16, dtype=tf.int32)[0]
         dim = tf.shape(self._lower)[-1]
         return (self._upper - self._lower) * tf.math.sobol_sample(
             dim=dim, num_results=num_samples, dtype=self._lower.dtype, skip=skip
         ) + self._lower
```

### Comparing `trieste-3.2.0/trieste/types.py` & `trieste-3.3.0/trieste/types.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/utils/__init__.py` & `trieste-3.3.0/trieste/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/utils/misc.py` & `trieste-3.3.0/trieste/utils/misc.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste/version.py` & `trieste-3.3.0/trieste/version.py`

 * *Files identical despite different names*

### Comparing `trieste-3.2.0/trieste.egg-info/PKG-INFO` & `trieste-3.3.0/trieste.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trieste
-Version: 3.2.0
+Version: 3.3.0
 Summary: A Bayesian optimization research toolbox built on TensorFlow
 Home-page: https://github.com/secondmind-labs/trieste
 Author: The Trieste contributors
 Author-email: labs@secondmind.ai
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `trieste-3.2.0/trieste.egg-info/SOURCES.txt` & `trieste-3.3.0/trieste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

