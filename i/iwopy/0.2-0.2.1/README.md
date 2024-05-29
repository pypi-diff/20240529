# Comparing `tmp/iwopy-0.2.tar.gz` & `tmp/iwopy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iwopy-0.2.tar", last modified: Thu Feb  8 09:49:05 2024, max compression
+gzip compressed data, was "iwopy-0.2.1.tar", last modified: Wed May 29 15:07:23 2024, max compression
```

## Comparing `iwopy-0.2.tar` & `iwopy-0.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.039325 iwopy-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-08 09:48:55.000000 iwopy-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8107 2024-02-08 09:48:55.000000 iwopy-0.2/Logo_IWOPY_white.svg
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-08 09:48:55.000000 iwopy-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-02-08 09:49:05.039325 iwopy-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-02-08 09:48:55.000000 iwopy-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.027325 iwopy-0.2/iwopy/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.031325 iwopy-0.2/iwopy/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.031325 iwopy-0.2/iwopy/benchmarks/branin/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/benchmarks/branin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/benchmarks/branin/branin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.031325 iwopy-0.2/iwopy/benchmarks/rosenbrock/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/benchmarks/rosenbrock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/benchmarks/rosenbrock/rosenbrock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.031325 iwopy-0.2/iwopy/core/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/core/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/core/constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/core/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    13338 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/core/function_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/core/function_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/core/objective.py
--rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/core/opt_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/core/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30676 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/core/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.031325 iwopy-0.2/iwopy/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.031325 iwopy-0.2/iwopy/interfaces/pygmo/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/interfaces/pygmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/interfaces/pygmo/algos.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/interfaces/pygmo/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/interfaces/pygmo/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/interfaces/pygmo/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.035325 iwopy-0.2/iwopy/interfaces/pymoo/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/interfaces/pymoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/interfaces/pymoo/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/interfaces/pymoo/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/interfaces/pymoo/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13043 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/interfaces/pymoo/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.035325 iwopy-0.2/iwopy/interfaces/scipy/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/interfaces/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/interfaces/scipy/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.035325 iwopy-0.2/iwopy/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/optimizers/gg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.035325 iwopy-0.2/iwopy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36671 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/utils/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/utils/stdout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.035325 iwopy-0.2/iwopy/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/wrappers/discretize_reg_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/wrappers/local_fd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/wrappers/problem_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/wrappers/simple_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/wrappers/simple_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-02-08 09:48:55.000000 iwopy-0.2/iwopy/wrappers/simple_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:49:05.035325 iwopy-0.2/iwopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-02-08 09:49:05.000000 iwopy-0.2/iwopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-02-08 09:49:05.000000 iwopy-0.2/iwopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 09:49:05.000000 iwopy-0.2/iwopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-08 09:49:05.000000 iwopy-0.2/iwopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-08 09:49:05.000000 iwopy-0.2/iwopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 09:49:04.000000 iwopy-0.2/iwopy.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-08 09:48:55.000000 iwopy-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-08 09:49:05.039325 iwopy-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-08 09:48:55.000000 iwopy-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.460595 iwopy-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-29 15:07:18.000000 iwopy-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8107 2024-05-29 15:07:18.000000 iwopy-0.2.1/Logo_IWOPY_white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-29 15:07:18.000000 iwopy-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-05-29 15:07:23.460595 iwopy-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-05-29 15:07:18.000000 iwopy-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.452595 iwopy-0.2.1/iwopy/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.452595 iwopy-0.2.1/iwopy/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.452595 iwopy-0.2.1/iwopy/benchmarks/branin/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/benchmarks/branin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/benchmarks/branin/branin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.452595 iwopy-0.2.1/iwopy/benchmarks/rosenbrock/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/benchmarks/rosenbrock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/benchmarks/rosenbrock/rosenbrock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.456595 iwopy-0.2.1/iwopy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/core/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/core/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13338 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/core/function_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/core/function_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/core/objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/core/opt_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/core/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30676 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/core/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.456595 iwopy-0.2.1/iwopy/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.456595 iwopy-0.2.1/iwopy/interfaces/pygmo/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/interfaces/pygmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/interfaces/pygmo/algos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/interfaces/pygmo/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/interfaces/pygmo/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/interfaces/pygmo/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.456595 iwopy-0.2.1/iwopy/interfaces/pymoo/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/interfaces/pymoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/interfaces/pymoo/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/interfaces/pymoo/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/interfaces/pymoo/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13043 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/interfaces/pymoo/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.456595 iwopy-0.2.1/iwopy/interfaces/scipy/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/interfaces/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/interfaces/scipy/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.456595 iwopy-0.2.1/iwopy/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/optimizers/gg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.456595 iwopy-0.2.1/iwopy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36671 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/utils/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/utils/stdout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.460595 iwopy-0.2.1/iwopy/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/wrappers/discretize_reg_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/wrappers/local_fd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/wrappers/problem_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/wrappers/simple_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/wrappers/simple_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-05-29 15:07:18.000000 iwopy-0.2.1/iwopy/wrappers/simple_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:07:23.460595 iwopy-0.2.1/iwopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-05-29 15:07:23.000000 iwopy-0.2.1/iwopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-29 15:07:23.000000 iwopy-0.2.1/iwopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:07:23.000000 iwopy-0.2.1/iwopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-29 15:07:23.000000 iwopy-0.2.1/iwopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 15:07:23.000000 iwopy-0.2.1/iwopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:07:23.000000 iwopy-0.2.1/iwopy.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 15:07:18.000000 iwopy-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-29 15:07:23.460595 iwopy-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 15:07:18.000000 iwopy-0.2.1/setup.py
```

### Comparing `iwopy-0.2/LICENSE` & `iwopy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/Logo_IWOPY_white.svg` & `iwopy-0.2.1/Logo_IWOPY_white.svg`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/PKG-INFO` & `iwopy-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iwopy
-Version: 0.2
+Version: 0.2.1
 Summary: Fraunhofer IWES optimization tools in Python
 Home-page: https://github.com/FraunhoferIWES/iwopy
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/iwopy
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/iwopy/issues
@@ -16,26 +16,30 @@
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
+Provides-Extra: opt
+Requires-Dist: pygmo; extra == "opt"
+Requires-Dist: pymoo>=0.6; extra == "opt"
 Provides-Extra: test
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pygmo; extra == "test"
 Requires-Dist: pymoo>=0.6; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-immaterial; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: ipykernel; extra == "doc"
 Requires-Dist: ipywidgets; extra == "doc"
 Requires-Dist: m2r2; extra == "doc"
+Requires-Dist: lxml_html_clean; extra == "doc"
 Provides-Extra: all
 Requires-Dist: flake8; extra == "all"
 Requires-Dist: pytest; extra == "all"
 Requires-Dist: pygmo; extra == "all"
 Requires-Dist: pymoo>=0.6; extra == "all"
 Requires-Dist: sphinx; extra == "all"
 Requires-Dist: sphinx-immaterial; extra == "all"
@@ -74,31 +78,34 @@
 
 Source code: [https://github.com/FraunhoferIWES/iwopy](https://github.com/FraunhoferIWES/iwopy)
 
 PyPi reference: [https://pypi.org/project/iwopy/](https://pypi.org/project/iwopy/)
 
 Anaconda reference: [https://anaconda.org/conda-forge/iwopy](https://anaconda.org/conda-forge/iwopy)
 
+## Contributing
+
+Please feel invited to contribute to `iwopy`! Here is how:
+
+1. Fork _iwopy_ on _github_.
+2. Create a branch (`git checkout -b new_branch`)
+3. Commit your changes (`git commit -am "your awesome message"`)
+4. Push to the branch (`git push origin new_branch`)
+5. Create a pull request [here](https://github.com/FraunhoferIWES/iwopy/pulls)
+
 ## Requirements
 
 The supported Python versions are:
 
 - `Python 3.7`
 - `Python 3.8`
 - `Python 3.9`
 - `Python 3.10`
 - `Python 3.11`
-
-## Installation via conda
-
-The `iwopy` package is available on the channel [conda-forge](https://anaconda.org/conda-forge/iwopy). You can install the latest version by
-
-```console
-conda install -c conda-forge iwopy
-```
+- `Python 3.12`
 
 ## Installation via pip
 
 ### Virtual Python environment
 
 We recommend working in a Python virtual environment and install `iwopy` there. Such an environment can be created by
 
@@ -126,14 +133,29 @@
 
 This in general corresponds to the `main` branch at [github](https://github.com/FraunhoferIWES/iwopy). Alternatively, you can decide to install the latest pre-release developments (non-stable) by
 
 ```console
 pip install git+https://github.com/FraunhoferIWES/iwopy@dev#egg=iwopy
 ```
 
+Notice that the above default installation does not install the third-party optimization
+packages. `iwopy` will tell you in an error message that it is missing a package, with
+a hint of installation advice. You can avoid this step by installing all supported
+optimzer packages by installing those optoinal packages by addig `[opt]`:
+
+```console
+pip install iwopy[opt]
+```
+
+or
+
+```console
+pip install git+https://github.com/FraunhoferIWES/iwopy@dev#egg=iwopy[opt]
+```
+
 ### Developers
 
 The first step as a developer is to clone the `iwopy` repository by
 
 ```console
 git clone https://github.com/FraunhoferIWES/iwopy.git
 ```
@@ -146,28 +168,75 @@
 
 Then you can either install from this directory via
 
 ```console
 pip install -e .
 ```
 
+Notice that the above default installation does not install the third-party optimization
+packages. `iwopy` will tell you in an error message that it is missing a package, with
+a hint of installation advice. You can avoid this step by installing all supported
+optimzer packages by installing those optoinal packages by addig `[opt]`:
+
+```console
+pip install -e .[opt]
+```
+
+## Installation via conda
+
+### Preparation (optional)
+
+It is strongly recommend to use the `libmamba` dependency solver instead of the default solver. Install it once by
+
+```console
+conda install conda-libmamba-solver -n base -c conda-forge
+```
+
+We recommend that you set this to be your default solver, by
+
+```console
+conda config --set solver libmamba
+```
+
+### Standard users
+
+The `iwopy` package is available on the channel [conda-forge](https://anaconda.org/conda-forge/iwopy). You can install the latest version by
+
+```console
+conda install -c conda-forge iwopy
+```
+
+### Developers
+
+For developers using `conda`, we recommend first installing `iwopy` as described above, then removing only the `iwopy` package while keeping the dependencies, and then adding `iwopy` again from a git using `conda develop`:
+
+```console
+conda install iwopy conda-build -c conda-forge
+conda remove iwopy --force
+git clone https://github.com/FraunhoferIWES/iwopy.git
+cd iwopy
+conda develop .
+```
+
+Concerning the `git clone` line, we actually recommend that you fork `iwopy` on GitHub and then replace that command by cloning your fork instead.
+
 ## Testing
 
-For testing, please clone the repository and install the required dependencies:
+For testing, please clone the repository and install the required dependencies
+(`flake8`, `pytest`, `pygmo`, `pymoo`):
+
 ```console
 git clone https://github.com/FraunhoferIWES/iwopy.git
 cd iwopy
+pip install .[test]
+```
+
+If you are a developer you might want to replace the last line by
+```console
 pip install -e .[test]
 ```
+for dynamic installation from the local code base.
 
 The tests are then run by
 ```console
 pytest tests
 ```
-
-## Contributing
-
-1. Fork _iwopy_ on _github_.
-2. Create a branch (`git checkout -b new_branch`)
-3. Commit your changes (`git commit -am "your awesome message"`)
-4. Push to the branch (`git push origin new_branch`)
-5. Create a pull request [here](https://github.com/FraunhoferIWES/iwopy/pulls)
```

### Comparing `iwopy-0.2/iwopy/__init__.py` & `iwopy-0.2.1/iwopy/__init__.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/benchmarks/branin/branin.py` & `iwopy-0.2.1/iwopy/benchmarks/branin/branin.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/benchmarks/rosenbrock/rosenbrock.py` & `iwopy-0.2.1/iwopy/benchmarks/rosenbrock/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/core/base.py` & `iwopy-0.2.1/iwopy/core/base.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/core/constraint.py` & `iwopy-0.2.1/iwopy/core/constraint.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/core/function.py` & `iwopy-0.2.1/iwopy/core/function.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/core/function_list.py` & `iwopy-0.2.1/iwopy/core/function_list.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/core/function_subset.py` & `iwopy-0.2.1/iwopy/core/function_subset.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/core/memory.py` & `iwopy-0.2.1/iwopy/core/memory.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/core/opt_results.py` & `iwopy-0.2.1/iwopy/core/opt_results.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/core/optimizer.py` & `iwopy-0.2.1/iwopy/core/optimizer.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/core/problem.py` & `iwopy-0.2.1/iwopy/core/problem.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/interfaces/pygmo/algos.py` & `iwopy-0.2.1/iwopy/interfaces/pygmo/algos.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/interfaces/pygmo/imports.py` & `iwopy-0.2.1/iwopy/interfaces/pygmo/imports.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/interfaces/pygmo/optimizer.py` & `iwopy-0.2.1/iwopy/interfaces/pygmo/optimizer.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/interfaces/pygmo/problem.py` & `iwopy-0.2.1/iwopy/interfaces/pygmo/problem.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/interfaces/pymoo/factory.py` & `iwopy-0.2.1/iwopy/interfaces/pymoo/factory.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/interfaces/pymoo/imports.py` & `iwopy-0.2.1/iwopy/interfaces/pymoo/imports.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/interfaces/pymoo/optimizer.py` & `iwopy-0.2.1/iwopy/interfaces/pymoo/optimizer.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/interfaces/pymoo/problem.py` & `iwopy-0.2.1/iwopy/interfaces/pymoo/problem.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/interfaces/scipy/optimizer.py` & `iwopy-0.2.1/iwopy/interfaces/scipy/optimizer.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/optimizers/gg.py` & `iwopy-0.2.1/iwopy/optimizers/gg.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/utils/discretization.py` & `iwopy-0.2.1/iwopy/utils/discretization.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/utils/load.py` & `iwopy-0.2.1/iwopy/utils/load.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/utils/stdout.py` & `iwopy-0.2.1/iwopy/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/wrappers/discretize_reg_grid.py` & `iwopy-0.2.1/iwopy/wrappers/discretize_reg_grid.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/wrappers/local_fd.py` & `iwopy-0.2.1/iwopy/wrappers/local_fd.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/wrappers/problem_wrapper.py` & `iwopy-0.2.1/iwopy/wrappers/problem_wrapper.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/wrappers/simple_constraint.py` & `iwopy-0.2.1/iwopy/wrappers/simple_constraint.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/wrappers/simple_objective.py` & `iwopy-0.2.1/iwopy/wrappers/simple_objective.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy/wrappers/simple_problem.py` & `iwopy-0.2.1/iwopy/wrappers/simple_problem.py`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/iwopy.egg-info/PKG-INFO` & `iwopy-0.2.1/iwopy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iwopy
-Version: 0.2
+Version: 0.2.1
 Summary: Fraunhofer IWES optimization tools in Python
 Home-page: https://github.com/FraunhoferIWES/iwopy
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/iwopy
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/iwopy/issues
@@ -16,26 +16,30 @@
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
+Provides-Extra: opt
+Requires-Dist: pygmo; extra == "opt"
+Requires-Dist: pymoo>=0.6; extra == "opt"
 Provides-Extra: test
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pygmo; extra == "test"
 Requires-Dist: pymoo>=0.6; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-immaterial; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: ipykernel; extra == "doc"
 Requires-Dist: ipywidgets; extra == "doc"
 Requires-Dist: m2r2; extra == "doc"
+Requires-Dist: lxml_html_clean; extra == "doc"
 Provides-Extra: all
 Requires-Dist: flake8; extra == "all"
 Requires-Dist: pytest; extra == "all"
 Requires-Dist: pygmo; extra == "all"
 Requires-Dist: pymoo>=0.6; extra == "all"
 Requires-Dist: sphinx; extra == "all"
 Requires-Dist: sphinx-immaterial; extra == "all"
@@ -74,31 +78,34 @@
 
 Source code: [https://github.com/FraunhoferIWES/iwopy](https://github.com/FraunhoferIWES/iwopy)
 
 PyPi reference: [https://pypi.org/project/iwopy/](https://pypi.org/project/iwopy/)
 
 Anaconda reference: [https://anaconda.org/conda-forge/iwopy](https://anaconda.org/conda-forge/iwopy)
 
+## Contributing
+
+Please feel invited to contribute to `iwopy`! Here is how:
+
+1. Fork _iwopy_ on _github_.
+2. Create a branch (`git checkout -b new_branch`)
+3. Commit your changes (`git commit -am "your awesome message"`)
+4. Push to the branch (`git push origin new_branch`)
+5. Create a pull request [here](https://github.com/FraunhoferIWES/iwopy/pulls)
+
 ## Requirements
 
 The supported Python versions are:
 
 - `Python 3.7`
 - `Python 3.8`
 - `Python 3.9`
 - `Python 3.10`
 - `Python 3.11`
-
-## Installation via conda
-
-The `iwopy` package is available on the channel [conda-forge](https://anaconda.org/conda-forge/iwopy). You can install the latest version by
-
-```console
-conda install -c conda-forge iwopy
-```
+- `Python 3.12`
 
 ## Installation via pip
 
 ### Virtual Python environment
 
 We recommend working in a Python virtual environment and install `iwopy` there. Such an environment can be created by
 
@@ -126,14 +133,29 @@
 
 This in general corresponds to the `main` branch at [github](https://github.com/FraunhoferIWES/iwopy). Alternatively, you can decide to install the latest pre-release developments (non-stable) by
 
 ```console
 pip install git+https://github.com/FraunhoferIWES/iwopy@dev#egg=iwopy
 ```
 
+Notice that the above default installation does not install the third-party optimization
+packages. `iwopy` will tell you in an error message that it is missing a package, with
+a hint of installation advice. You can avoid this step by installing all supported
+optimzer packages by installing those optoinal packages by addig `[opt]`:
+
+```console
+pip install iwopy[opt]
+```
+
+or
+
+```console
+pip install git+https://github.com/FraunhoferIWES/iwopy@dev#egg=iwopy[opt]
+```
+
 ### Developers
 
 The first step as a developer is to clone the `iwopy` repository by
 
 ```console
 git clone https://github.com/FraunhoferIWES/iwopy.git
 ```
@@ -146,28 +168,75 @@
 
 Then you can either install from this directory via
 
 ```console
 pip install -e .
 ```
 
+Notice that the above default installation does not install the third-party optimization
+packages. `iwopy` will tell you in an error message that it is missing a package, with
+a hint of installation advice. You can avoid this step by installing all supported
+optimzer packages by installing those optoinal packages by addig `[opt]`:
+
+```console
+pip install -e .[opt]
+```
+
+## Installation via conda
+
+### Preparation (optional)
+
+It is strongly recommend to use the `libmamba` dependency solver instead of the default solver. Install it once by
+
+```console
+conda install conda-libmamba-solver -n base -c conda-forge
+```
+
+We recommend that you set this to be your default solver, by
+
+```console
+conda config --set solver libmamba
+```
+
+### Standard users
+
+The `iwopy` package is available on the channel [conda-forge](https://anaconda.org/conda-forge/iwopy). You can install the latest version by
+
+```console
+conda install -c conda-forge iwopy
+```
+
+### Developers
+
+For developers using `conda`, we recommend first installing `iwopy` as described above, then removing only the `iwopy` package while keeping the dependencies, and then adding `iwopy` again from a git using `conda develop`:
+
+```console
+conda install iwopy conda-build -c conda-forge
+conda remove iwopy --force
+git clone https://github.com/FraunhoferIWES/iwopy.git
+cd iwopy
+conda develop .
+```
+
+Concerning the `git clone` line, we actually recommend that you fork `iwopy` on GitHub and then replace that command by cloning your fork instead.
+
 ## Testing
 
-For testing, please clone the repository and install the required dependencies:
+For testing, please clone the repository and install the required dependencies
+(`flake8`, `pytest`, `pygmo`, `pymoo`):
+
 ```console
 git clone https://github.com/FraunhoferIWES/iwopy.git
 cd iwopy
+pip install .[test]
+```
+
+If you are a developer you might want to replace the last line by
+```console
 pip install -e .[test]
 ```
+for dynamic installation from the local code base.
 
 The tests are then run by
 ```console
 pytest tests
 ```
-
-## Contributing
-
-1. Fork _iwopy_ on _github_.
-2. Create a branch (`git checkout -b new_branch`)
-3. Commit your changes (`git commit -am "your awesome message"`)
-4. Push to the branch (`git push origin new_branch`)
-5. Create a pull request [here](https://github.com/FraunhoferIWES/iwopy/pulls)
```

### Comparing `iwopy-0.2/iwopy.egg-info/SOURCES.txt` & `iwopy-0.2.1/iwopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iwopy-0.2/setup.cfg` & `iwopy-0.2.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -28,26 +28,30 @@
 	>=3.7
 install_requires = 
 	numpy
 	scipy
 	matplotlib
 
 [options.extras_require]
+opt = 
+	pygmo
+	pymoo>=0.6
 test = 
 	flake8
 	pytest
 	pygmo
 	pymoo>=0.6
 doc = 
 	sphinx
 	sphinx-immaterial
 	nbsphinx
 	ipykernel
 	ipywidgets
 	m2r2
+	lxml_html_clean
 all = 
 	flake8
 	pytest
 	pygmo
 	pymoo>=0.6
 	sphinx
 	sphinx-immaterial
```

