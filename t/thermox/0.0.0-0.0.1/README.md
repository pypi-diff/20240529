# Comparing `tmp/thermox-0.0.0.tar.gz` & `tmp/thermox-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thermox-0.0.0.tar", last modified: Sun Feb 25 18:24:39 2024, max compression
+gzip compressed data, was "thermox-0.0.1.tar", last modified: Wed May 29 16:25:31 2024, max compression
```

## Comparing `thermox-0.0.0.tar` & `thermox-0.0.1.tar`

### file list

```diff
@@ -1,11 +1,23 @@
-drwxr-xr-x   0 samddd     (501) staff       (20)        0 2024-02-25 18:24:39.096983 thermox-0.0.0/
--rw-r--r--   0 samddd     (501) staff       (20)      127 2024-02-25 18:24:39.096766 thermox-0.0.0/PKG-INFO
--rw-r--r--   0 samddd     (501) staff       (20)      145 2024-02-25 18:24:24.000000 thermox-0.0.0/pyproject.toml
--rw-r--r--   0 samddd     (501) staff       (20)       38 2024-02-25 18:24:39.097035 thermox-0.0.0/setup.cfg
-drwxr-xr-x   0 samddd     (501) staff       (20)        0 2024-02-25 18:24:39.095818 thermox-0.0.0/thermox/
--rw-r--r--   0 samddd     (501) staff       (20)        0 2024-02-25 18:22:25.000000 thermox-0.0.0/thermox/__init__.py
-drwxr-xr-x   0 samddd     (501) staff       (20)        0 2024-02-25 18:24:39.096575 thermox-0.0.0/thermox.egg-info/
--rw-r--r--   0 samddd     (501) staff       (20)      127 2024-02-25 18:24:39.000000 thermox-0.0.0/thermox.egg-info/PKG-INFO
--rw-r--r--   0 samddd     (501) staff       (20)      158 2024-02-25 18:24:39.000000 thermox-0.0.0/thermox.egg-info/SOURCES.txt
--rw-r--r--   0 samddd     (501) staff       (20)        1 2024-02-25 18:24:39.000000 thermox-0.0.0/thermox.egg-info/dependency_links.txt
--rw-r--r--   0 samddd     (501) staff       (20)        8 2024-02-25 18:24:39.000000 thermox-0.0.0/thermox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:25:31.108213 thermox-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 16:25:26.000000 thermox-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-29 16:25:31.108213 thermox-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-29 16:25:26.000000 thermox-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-29 16:25:26.000000 thermox-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 16:25:31.108213 thermox-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:25:31.104213 thermox-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-29 16:25:26.000000 thermox-0.0.1/tests/test_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-29 16:25:26.000000 thermox-0.0.1/tests/test_log_prob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-29 16:25:26.000000 thermox-0.0.1/tests/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-29 16:25:26.000000 thermox-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:25:31.108213 thermox-0.0.1/thermox/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-29 16:25:26.000000 thermox-0.0.1/thermox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-29 16:25:26.000000 thermox-0.0.1/thermox/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-29 16:25:26.000000 thermox-0.0.1/thermox/prob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-29 16:25:26.000000 thermox-0.0.1/thermox/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-29 16:25:26.000000 thermox-0.0.1/thermox/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:25:31.108213 thermox-0.0.1/thermox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-29 16:25:31.000000 thermox-0.0.1/thermox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-29 16:25:31.000000 thermox-0.0.1/thermox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:25:31.000000 thermox-0.0.1/thermox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-29 16:25:31.000000 thermox-0.0.1/thermox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 16:25:31.000000 thermox-0.0.1/thermox.egg-info/top_level.txt
```

