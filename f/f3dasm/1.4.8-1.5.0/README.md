# Comparing `tmp/f3dasm-1.4.8.tar.gz` & `tmp/f3dasm-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f3dasm-1.4.8.tar", last modified: Fri May 17 13:49:38 2024, max compression
+gzip compressed data, was "f3dasm-1.5.0.tar", last modified: Wed May 29 13:44:57 2024, max compression
```

## Comparing `f3dasm-1.4.8.tar` & `f3dasm-1.5.0.tar`

### file list

```diff
@@ -1,84 +1,66 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.406901 f3dasm-1.4.8/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1531 2023-03-30 12:29:51.000000 f3dasm-1.4.8/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-07-07 13:46:05.000000 f3dasm-1.4.8/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)     5938 2024-05-17 13:49:38.406901 f3dasm-1.4.8/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     4276 2024-05-17 13:36:49.000000 f3dasm-1.4.8/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)        5 2024-05-17 13:36:49.000000 f3dasm-1.4.8/VERSION
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.394902 f3dasm-1.4.8/docs/
--rw-rw-r--   0 martin    (1000) martin    (1000)      103 2024-05-17 13:36:49.000000 f3dasm-1.4.8/docs/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      457 2023-07-15 20:12:10.000000 f3dasm-1.4.8/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)       85 2023-09-06 16:39:06.000000 f3dasm-1.4.8/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     1435 2024-05-17 13:49:38.406901 f3dasm-1.4.8/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.390902 f3dasm-1.4.8/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.394902 f3dasm-1.4.8/src/f3dasm/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1804 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       27 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/__version__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.398902 f3dasm-1.4.8/src/f3dasm/_src/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/_src/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1241 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/_argparser.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.398902 f3dasm-1.4.8/src/f3dasm/_src/datageneration/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1385 2023-12-07 15:18:37.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.398902 f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5136 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/abaqus_functions.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5479 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/abaqus_simulator.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1510 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8018 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/datagenerator.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.398902 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/
--rw-rw-r--   0 martin    (1000) martin    (1000)     5229 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.398902 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)      125 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8220 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4389 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9183 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/function.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1794 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/function_factory.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    80508 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/pybenchfunction.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.402902 f3dasm-1.4.8/src/f3dasm/_src/design/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/_src/design/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    21658 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/design/domain.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10505 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/design/parameter.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.402902 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3673 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_columns.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    17943 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_data.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10131 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_io.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10455 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_jobqueue.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    23185 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_newdata.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    68231 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/experimentdata.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    12764 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/experimentsample.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    12801 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/samplers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1618 2023-12-07 15:18:37.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2125 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/hydra_utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4025 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/logger.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.402902 f3dasm-1.4.8/src/f3dasm/_src/machinelearning/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/_src/machinelearning/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.402902 f3dasm-1.4.8/src/f3dasm/_src/optimization/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1751 2023-12-07 15:18:37.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.402902 f3dasm-1.4.8/src/f3dasm/_src/optimization/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2407 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/adapters/scipy_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1157 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/cg.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1258 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/lbfgsb.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1324 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/neldermead.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5903 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/optimizer.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2097 2023-12-07 15:18:37.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/optimizer_factory.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1770 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/randomsearch.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8914 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/run_optimization.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.406901 f3dasm-1.4.8/src/f3dasm/datageneration/
--rw-rw-r--   0 martin    (1000) martin    (1000)      773 2024-04-22 07:46:23.000000 f3dasm-1.4.8/src/f3dasm/datageneration/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      993 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/datageneration/abaqus.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      906 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/datageneration/functions.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1351 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/design.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      791 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/hydra_tools.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1665 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/optimization.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.406901 f3dasm-1.4.8/src/f3dasm.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     5938 2024-05-17 13:49:38.000000 f3dasm-1.4.8/src/f3dasm.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2450 2024-05-17 13:49:38.000000 f3dasm-1.4.8/src/f3dasm.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-05-17 13:49:38.000000 f3dasm-1.4.8/src/f3dasm.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      132 2024-05-17 13:49:38.000000 f3dasm-1.4.8/src/f3dasm.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        7 2024-05-17 13:49:38.000000 f3dasm-1.4.8/src/f3dasm.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.406901 f3dasm-1.4.8/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-08-17 09:47:40.000000 f3dasm-1.4.8/tests/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      141 2022-08-31 10:13:29.000000 f3dasm-1.4.8/tests/__init__.pyc
--rw-rw-r--   0 martin    (1000) martin    (1000)      855 2023-10-02 00:02:33.000000 f3dasm-1.4.8/tests/conftest.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       29 2023-03-10 12:07:18.000000 f3dasm-1.4.8/tests/requirements.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.992264 f3dasm-1.5.0/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1531 2024-05-24 09:01:59.000000 f3dasm-1.5.0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)       74 2024-05-24 09:01:59.000000 f3dasm-1.5.0/MANIFEST.in
+-rw-r--r--   0 martin    (1000) martin    (1000)     4991 2024-05-29 13:44:56.992264 f3dasm-1.5.0/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3329 2024-05-29 13:42:22.000000 f3dasm-1.5.0/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)        5 2024-05-29 13:42:22.000000 f3dasm-1.5.0/VERSION
+-rw-rw-r--   0 martin    (1000) martin    (1000)      457 2024-05-24 09:01:59.000000 f3dasm-1.5.0/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       85 2024-05-24 09:01:59.000000 f3dasm-1.5.0/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1435 2024-05-29 13:44:56.992264 f3dasm-1.5.0/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.984264 f3dasm-1.5.0/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1481 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       27 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/__version__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/_src/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1241 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/_argparser.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/_src/datageneration/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1309 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5153 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/datagenerator.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5229 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      125 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8220 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4389 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9056 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/function.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1794 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/function_factory.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    80508 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/pybenchfunction.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/_src/design/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/design/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    21530 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/design/domain.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10505 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/design/parameter.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.988264 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3673 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_columns.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17943 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_data.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10131 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_io.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10455 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_jobqueue.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    23185 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_newdata.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    68077 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/experimentdata.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12635 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/experimentsample.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12662 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/samplers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1618 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/experimentdata/utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2125 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/hydra_utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3478 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/logger.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.992264 f3dasm-1.5.0/src/f3dasm/_src/optimization/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1549 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.992264 f3dasm-1.5.0/src/f3dasm/_src/optimization/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2534 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/adapters/scipy_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1765 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/numpy_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7538 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/optimizer.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2116 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/optimizer_factory.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2336 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/_src/optimization/scipy_implementations.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.992264 f3dasm-1.5.0/src/f3dasm/datageneration/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      755 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/datageneration/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      906 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/datageneration/functions.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      903 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/design.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      791 2024-05-24 09:01:59.000000 f3dasm-1.5.0/src/f3dasm/hydra_tools.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      823 2024-05-29 13:42:22.000000 f3dasm-1.5.0/src/f3dasm/optimization.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-29 13:44:56.992264 f3dasm-1.5.0/src/f3dasm.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     4991 2024-05-29 13:44:56.000000 f3dasm-1.5.0/src/f3dasm.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1967 2024-05-29 13:44:56.000000 f3dasm-1.5.0/src/f3dasm.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-05-29 13:44:56.000000 f3dasm-1.5.0/src/f3dasm.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      132 2024-05-29 13:44:56.000000 f3dasm-1.5.0/src/f3dasm.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        7 2024-05-29 13:44:56.000000 f3dasm-1.5.0/src/f3dasm.egg-info/top_level.txt
```

### Comparing `f3dasm-1.4.8/LICENSE` & `f3dasm-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/PKG-INFO` & `f3dasm-1.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: f3dasm
-Version: 1.4.8
-Summary: f3dasm - Framework for Data-driven development and Analysis of Structures and Materials
+Version: 1.5.0
+Summary: f3dasm - Framework for Data-driven Development and Analysis of Structures and Materials
 Home-page: https://github.com/bessagroup/f3dasm
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD
 Project-URL: Documentation, https://f3dasm.readthedocs.io/
 Project-URL: Wiki, https://github.com/bessagroup/f3dasm/wiki
 Keywords: data-driven materials framework,machine learning
@@ -38,15 +38,16 @@
 Requires-Dist: filelock
 Provides-Extra: benchmark
 Requires-Dist: abaqus2py==1.0.0; extra == "benchmark"
 Requires-Dist: f3dasm_optimize; extra == "benchmark"
 
 f3dasm
 ------
-*Framework for data-driven design \& analysis of structures and materials*
+
+<div align="center"><img src="https://raw.githubusercontent.com/bessagroup/f3dasm/pr/1.5/paper/f3dasm_logo_long.png" width="800"/></div>
 
 ***
 
 [![Python](https://img.shields.io/pypi/pyversions/f3dasm)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/f3dasm.svg)](https://pypi.org/project/f3dasm/)
 [![GitHub license](https://img.shields.io/badge/license-BSD-blue)](https://github.com/bessagroup/f3dasm)
 [![Documentation Status](https://readthedocs.org/projects/f3dasm/badge/?version=latest)](https://f3dasm.readthedocs.io/en/latest/?badge=latest)
@@ -79,39 +80,25 @@
 
 ## Getting started
 
 The best way to get started is to follow the [installation instructions](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html).
 
 ## Illustrative benchmarks
 
-This package includes a collection of illustrative benchmark studies that demonstrate the capabilities of the framework. These studies are available in the `/studies` folder, and include the following studies:
+This package includes a collection of illustrative benchmark studies that demonstrate the capabilities of the framework. These studies are available in the `/studies/` folder, and include the following studies:
 
 - Benchmarking optimization algorithms against well-known benchmark functions
 - 'Fragile Becomes Supercompressible' ([Bessa et al. (2019)](https://onlinelibrary.wiley.com/doi/full/10.1002/adma.201904845))
 
 ## Authorship
 
-* Current created and developer: [M.P. van der Schelling](https://github.com/mpvanderschelling/) (M.P.vanderSchelling@tudelft.nl)
+* Current creator and developer: [M.P. van der Schelling](https://github.com/mpvanderschelling/) (M.P.vanderSchelling@tudelft.nl)
 
 The Bessa research group at TU Delft is small... At the moment, we have limited availability to help future users/developers adapting the code to new problems, but we will do our best to help!
 
-
-
-## Referencing
-
-If you use or edit our work, please cite at least one of the appropriate references:
-
-[1] Bessa, M. A., Bostanabad, R., Liu, Z., Hu, A., Apley, D. W., Brinson, C., Chen, W., & Liu, W. K. (2017). A framework for data-driven analysis of materials under uncertainty: Countering the curse of dimensionality. Computer Methods in Applied Mechanics and Engineering, 320, 633-667.
-
-[2] Bessa, M. A., & Pellegrino, S. (2018). Design of ultra-thin shell structures in the stochastic post-buckling range using Bayesian machine learning and optimization. International Journal of Solids and Structures, 139, 174-188.
-
-[3] Bessa, M. A., Glowacki, P., & Houlder, M. (2019). Bayesian machine learning in metamaterial design: fragile becomes super-compressible. Advanced Materials, 31(48), 1904845.
-
-[4] Mojtaba, M., Bostanabad, R., Chen, W., Ehmann, K., Cao, J., & Bessa, M. A. (2019). Deep learning predicts path-dependent plasticity. Proceedings of the National Academy of Sciences, 116(52), 26414-26420.
-
 ## Community Support
 
 If you find any **issues, bugs or problems** with this template, please use the [GitHub issue tracker](https://github.com/bessagroup/f3dasm/issues) to report them.
 
 ## License
 
 Copyright 2024, Martin van der Schelling
```

### Comparing `f3dasm-1.4.8/README.md` & `f3dasm-1.5.0/src/f3dasm.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,53 @@
+Metadata-Version: 2.1
+Name: f3dasm
+Version: 1.5.0
+Summary: f3dasm - Framework for Data-driven Development and Analysis of Structures and Materials
+Home-page: https://github.com/bessagroup/f3dasm
+Author: Martin van der Schelling
+Author-email: M.P.vanderSchelling@tudelft.nl
+License: BSD
+Project-URL: Documentation, https://f3dasm.readthedocs.io/
+Project-URL: Wiki, https://github.com/bessagroup/f3dasm/wiki
+Keywords: data-driven materials framework,machine learning
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pandas
+Requires-Dist: xarray
+Requires-Dist: matplotlib
+Requires-Dist: hydra-core
+Requires-Dist: pathos>=0.3.0
+Requires-Dist: autograd
+Requires-Dist: SALib
+Requires-Dist: filelock
+Provides-Extra: benchmark
+Requires-Dist: abaqus2py==1.0.0; extra == "benchmark"
+Requires-Dist: f3dasm_optimize; extra == "benchmark"
+
 f3dasm
 ------
-*Framework for data-driven design \& analysis of structures and materials*
+
+<div align="center"><img src="https://raw.githubusercontent.com/bessagroup/f3dasm/pr/1.5/paper/f3dasm_logo_long.png" width="800"/></div>
 
 ***
 
 [![Python](https://img.shields.io/pypi/pyversions/f3dasm)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/f3dasm.svg)](https://pypi.org/project/f3dasm/)
 [![GitHub license](https://img.shields.io/badge/license-BSD-blue)](https://github.com/bessagroup/f3dasm)
 [![Documentation Status](https://readthedocs.org/projects/f3dasm/badge/?version=latest)](https://f3dasm.readthedocs.io/en/latest/?badge=latest)
@@ -37,43 +80,29 @@
 
 ## Getting started
 
 The best way to get started is to follow the [installation instructions](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html).
 
 ## Illustrative benchmarks
 
-This package includes a collection of illustrative benchmark studies that demonstrate the capabilities of the framework. These studies are available in the `/studies` folder, and include the following studies:
+This package includes a collection of illustrative benchmark studies that demonstrate the capabilities of the framework. These studies are available in the `/studies/` folder, and include the following studies:
 
 - Benchmarking optimization algorithms against well-known benchmark functions
 - 'Fragile Becomes Supercompressible' ([Bessa et al. (2019)](https://onlinelibrary.wiley.com/doi/full/10.1002/adma.201904845))
 
 ## Authorship
 
-* Current created and developer: [M.P. van der Schelling](https://github.com/mpvanderschelling/) (M.P.vanderSchelling@tudelft.nl)
+* Current creator and developer: [M.P. van der Schelling](https://github.com/mpvanderschelling/) (M.P.vanderSchelling@tudelft.nl)
 
 The Bessa research group at TU Delft is small... At the moment, we have limited availability to help future users/developers adapting the code to new problems, but we will do our best to help!
 
-
-
-## Referencing
-
-If you use or edit our work, please cite at least one of the appropriate references:
-
-[1] Bessa, M. A., Bostanabad, R., Liu, Z., Hu, A., Apley, D. W., Brinson, C., Chen, W., & Liu, W. K. (2017). A framework for data-driven analysis of materials under uncertainty: Countering the curse of dimensionality. Computer Methods in Applied Mechanics and Engineering, 320, 633-667.
-
-[2] Bessa, M. A., & Pellegrino, S. (2018). Design of ultra-thin shell structures in the stochastic post-buckling range using Bayesian machine learning and optimization. International Journal of Solids and Structures, 139, 174-188.
-
-[3] Bessa, M. A., Glowacki, P., & Houlder, M. (2019). Bayesian machine learning in metamaterial design: fragile becomes super-compressible. Advanced Materials, 31(48), 1904845.
-
-[4] Mojtaba, M., Bostanabad, R., Chen, W., Ehmann, K., Cao, J., & Bessa, M. A. (2019). Deep learning predicts path-dependent plasticity. Proceedings of the National Academy of Sciences, 116(52), 26414-26420.
-
 ## Community Support
 
 If you find any **issues, bugs or problems** with this template, please use the [GitHub issue tracker](https://github.com/bessagroup/f3dasm/issues) to report them.
 
 ## License
 
 Copyright 2024, Martin van der Schelling
 
 All rights reserved.
 
-This project is licensed under the BSD 3-Clause License. See [LICENSE](https://github.com/bessagroup/f3dasm/blob/main/LICENSE) for the full license text.
+This project is licensed under the BSD 3-Clause License. See [LICENSE](https://github.com/bessagroup/f3dasm/blob/main/LICENSE) for the full license text.
```

### Comparing `f3dasm-1.4.8/setup.cfg` & `f3dasm-1.5.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = f3dasm
 version = file: VERSION
-description = f3dasm - Framework for Data-driven development and Analysis of Structures and Materials
+description = f3dasm - Framework for Data-driven Development and Analysis of Structures and Materials
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bessagroup/f3dasm
 project_urls = 
 	Documentation = https://f3dasm.readthedocs.io/
 	Wiki = https://github.com/bessagroup/f3dasm/wiki
 author = Martin van der Schelling
```

### Comparing `f3dasm-1.4.8/src/f3dasm/__init__.py` & `f3dasm-1.5.0/src/f3dasm/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 
 from .__version__ import __version__
 from ._src._argparser import HPC_JOBID
 from ._src.experimentdata._io import StoreProtocol
 from ._src.experimentdata.experimentdata import ExperimentData
 from ._src.experimentdata.experimentsample import ExperimentSample
 from ._src.logger import DistributedFileHandler, logger
-from ._src.run_optimization import (OptimizationResult, calculate_mean_std,
-                                    run_multiple_realizations,
-                                    run_optimization)
 
 #                                                        Authorship and Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 #
@@ -36,14 +33,9 @@
 logger.info(f"Imported f3dasm (version: {__version__})")
 
 __all__ = [
     'ExperimentData',
     'ExperimentSample',
     'DistributedFileHandler',
     'logger',
-    'OptimizationResult',
-    'run_multiple_realizations',
-    'run_optimization',
     'HPC_JOBID',
-    'calculate_mean_std',
-    'StoreProtocol',
 ]
```

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/_argparser.py` & `f3dasm-1.5.0/src/f3dasm/_src/_argparser.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/datageneration/__init__.py` & `f3dasm-1.5.0/src/f3dasm/_src/datageneration/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 #                                                                       Modules
 # =============================================================================
 
 # Standard
 from typing import List
 
 # Local
-from .abaqus.abaqus_simulator import AbaqusSimulator
 from .datagenerator import DataGenerator
 from .functions import pybenchfunction
 from .functions.adapters.augmentor import (FunctionAugmentor, Noise, Offset,
                                            Scale)
 from .functions.function import Function
 from .functions.pybenchfunction import *  # NOQA
 
@@ -37,10 +36,9 @@
     'DataGenerator',
     'Function',
     'FunctionAugmentor',
     'Noise',
     'Offset',
     'Scale',
     'DATAGENERATORS',
-    'AbaqusSimulator',
     *pybenchfunction.__all__
 ]
```

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/abaqus_functions.py` & `f3dasm-1.5.0/src/f3dasm/_src/datageneration/datagenerator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,143 +1,153 @@
 """
-This file contains the functions that are used to run Abaqus simulations.
-
-Note
-----
-I'm assuming that every process could have a different pre-processing,
-execution and post-processing function.
-But they are used in that order and only once.
-If multiple e.g. pre_process steps need to be taken, then they should
-be combined in one function.
+Interface class for data generators
 """
 
 #                                                                       Modules
 # =============================================================================
 
+
+from __future__ import annotations
+
 # Standard
-import os
-import pickle
-from pathlib import Path
+import inspect
+from abc import abstractmethod
+from typing import Any, Callable, Dict, List, Optional
+
+# Third-party
+import numpy as np
 
 # Local
-from ...experimentdata.experimentsample import ExperimentSample
+from ..design.domain import Domain
+from ..experimentdata.experimentsample import (ExperimentSample,
+                                               _experimentsample_factory)
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = "Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)"
 __credits__ = ["Martin van der Schelling"]
 __status__ = "Alpha"
 # =============================================================================
 #
 # =============================================================================
 
 
-def pre_process(
-        experiment_sample: ExperimentSample, folder_path: str,
-        python_file: str, function_name: str = "main", name: str = "job",
-        remove_temp_files: bool = True, **kwargs) -> None:
-    """Function that handles the pre-processing of Abaqus with a Python script
-
-    Parameters
-    ----------
-    experiment_sample : ExperimentSample
-        The design to run the data generator on. Will be handled by
-        the pipeline.
-    folder_path : str
-        Path of the folder where the python script is located
-    python_file : str
-        Name of the python file to be executed
-    function_name : str, optional
-        Name of the function within the python file to be executed,
-        by default "main"
-    name : str, optional
-        Name of the job, by default "job"
-    remove_temp_files : bool, optional
-
-    Note
-    ----
-    The python file should create an .inp input-file based on the
-    information of the experiment sample named <job_number>.inp.
+class DataGenerator:
+    """Base class for a data generator"""
+    @abstractmethod
+    def execute(self, **kwargs) -> None:
+        """Interface function that handles the execution of the data generator
+
+        Raises
+        ------
+        NotImplementedError
+            If the function is not implemented by the user
+
+        Note
+        ----
+        The experiment_sample is cached inside the data generator. This
+        allows the user to access the experiment_sample in
+        the execute and function as a class variable called
+        self.experiment_sample.
+        """
+        ...
+
+    def _run(
+            self, experiment_sample: ExperimentSample | np.ndarray,
+            domain: Optional[Domain] = None,
+            **kwargs) -> ExperimentSample:
+        """
+        Run the data generator.
+
+        The function also caches the experiment_sample in the data generator.
+        This allows the user to access the experiment_sample in the
+        execute function as a class variable
+        called self.experiment_sample.
+
+        Parameters
+        ----------
+        ExperimentSample : ExperimentSample
+            The design to run the data generator on
+        domain : Domain, optional
+            The domain of the data generator, by default None
+
+        kwargs : dict
+            The keyword arguments to pass to the pre_process, execute \
+            and post_process
+
+        Returns
+        -------
+        ExperimentSample
+            Processed design with the response of the data generator \
+            saved in the experiment_sample
+        """
+        # Cache the design
+        self.experiment_sample: ExperimentSample = _experimentsample_factory(
+            experiment_sample=experiment_sample, domain=domain)
+
+        self.execute(**kwargs)
+
+        return self.experiment_sample
+
+
+def convert_function(f: Callable,
+                     output: Optional[List[str]] = None,
+                     kwargs: Optional[Dict[str, Any]] = None,
+                     to_disk: Optional[List[str]] = None) -> DataGenerator:
     """
-
-    sim_info = kwargs
-    working_dir = Path("datageneration") / \
-        Path(f"{name}_{experiment_sample.job_number}")
-
-    # Updating simulation info with experiment sample data
-    sim_info.update(experiment_sample.to_dict())
-
-    filename = working_dir / "sim_info.pkl"
-    with open(filename, "wb") as fp:
-        pickle.dump(sim_info, fp, protocol=0)
-
-    with open(f"{working_dir / 'preprocess.py'}", "w") as f:
-        f.write("import os\n")
-        f.write("import sys\n")
-        f.write("import pickle\n")
-        f.write(f"sys.path.extend([r'{folder_path}'])\n")
-        f.write(
-            f"from {python_file} import {function_name}\n"
-        )
-        f.write(f"with open(r'{filename}', 'rb') as f:\n")
-        f.write("    dict = pickle.load(f)\n")
-        f.write(f"os.chdir(r'{working_dir}')\n")
-        f.write(f"{function_name}(dict)\n")
-
-    os.system(f"abaqus cae noGUI={working_dir / 'preprocess.py'} -mesa")
-
-    if remove_temp_files:
-        Path(working_dir / "preprocess.py").unlink(missing_ok=True)
-        Path(working_dir / "sim_info.pkl").unlink(missing_ok=True)
-
-
-def post_process(
-        experiment_sample: ExperimentSample, folder_path: str,
-        python_file: str, function_name: str = "main", name: str = "job",
-        remove_temp_files: bool = True, **kwargs) -> None:
-    """Function that handles the post-processing of Abaqus with a Python script
+    Converts a given function `f` into a `DataGenerator` object.
 
     Parameters
     ----------
-    experiment_sample : ExperimentSample
-        The design to run the data generator on.
-        Will be handled by the pipeline.
-    folder_path : str
-        Path of the folder where the python script is located
-    python_file : str
-        Name of the python file to be executed
-    function_name : str, optional
-        Name of the function within the python file to be executed,
-        by default "main"
-    name : str, optional
-        Name of the job, by default "job"
-    remove_temp_files : bool, optional
-        Whether to remove the temporary files, by default True
-
-    Note
-    ----
-    The post-processing python file should write the results of your
-    simulation to a pickle file
-    with the name: results.pkl. This file will be handled by the pipeline.
+    f : Callable
+        The function to be converted.
+    output : Optional[List[str]], optional
+        A list of names for the return values of the function.
+        Defaults to None.
+    kwargs : Optional[Dict[str, Any]], optional
+        Additional keyword arguments passed to the function. Defaults to None.
+    to_disk : Optional[List[str]], optional
+        The list of output names where the value needs to be stored on disk.
+        Defaults to None.
+
+    Returns
+    -------
+    DataGenerator
+        A converted `DataGenerator` object.
+
+    Notes
+    -----
+
+    The function `f` can have any number of arguments and any number of returns
+    as long as they are consistent with the `input` and `output` arguments that
+    are given to this function.
     """
+    signature = inspect.signature(f)
+    input = list(signature.parameters)
+    kwargs = kwargs if kwargs is not None else {}
+    to_disk = to_disk if to_disk is not None else []
+    output = output if output is not None else []
+
+    class TempDataGenerator(DataGenerator):
+        def execute(self, **_kwargs) -> None:
+            _input = {input_name: self.experiment_sample.get(input_name)
+                      for input_name in input if input_name not in kwargs}
+            _output = f(**_input, **kwargs)
+
+            # check if output is empty
+            if output is None:
+                return
+
+            if len(output) == 1:
+                _output = (_output,)
+
+            for name, value in zip(output, _output):
+                if name in to_disk:
+                    self.experiment_sample.store(name=name,
+                                                 object=value,
+                                                 to_disk=True)
+                else:
+                    self.experiment_sample.store(name=name,
+                                                 object=value,
+                                                 to_disk=False)
 
-    working_dir = Path("datageneration") / \
-        Path(f"{name}_{experiment_sample.job_number}")
-
-    with open(f"{working_dir / 'post.py'}", "w") as f:
-        f.write("import os\n")
-        f.write("import sys\n")
-        f.write("from abaqus import session\n")
-        f.write(f"sys.path.extend([r'{folder_path}'])\n")
-        f.write(
-            f"from {python_file} import {function_name}\n"
-        )
-        f.write(
-            f"odb = session.openOdb(\
-                name=r'{working_dir / str(experiment_sample.job_number)}\
-                    .odb')\n")
-        f.write(f"os.chdir(r'{working_dir}')\n")
-        f.write(f"{function_name}(odb)\n")
-
-    os.system(f"abaqus cae noGUI={working_dir / 'post.py'} -mesa")
-    if remove_temp_files:
-        Path(working_dir / "post.py").unlink(missing_ok=True)
+    return TempDataGenerator()
```

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/__init__.py` & `f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py` & `f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py` & `f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/function.py` & `f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/function.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,15 @@
 """
 #                                                                       Modules
 # =============================================================================
 
 from __future__ import annotations
 
 # Standard
-import sys
-from typing import Optional, Tuple
-
-if sys.version_info < (3, 8):  # NOQA
-    from typing_extensions import Protocol  # NOQA
-else:
-    from typing import Protocol
+from typing import Optional, Protocol, Tuple
 
 # Third-party core
 import autograd.numpy as np
 import matplotlib.colors as mcol
 import matplotlib.pyplot as plt
 from autograd import grad
 from autograd.numpy.numpy_boxes import ArrayBox
@@ -289,17 +283,17 @@
             ax.plot_surface(
                 xv,
                 yv,
                 Y_shifted,
                 rstride=1,
                 cstride=1,
                 edgecolor="none",
-                alpha=0.8,
+                alpha=0.9,
                 cmap="viridis",
-                norm=mcol.LogNorm(),  # mcol.LogNorm()
+                # norm=mcol.LogNorm(),  # mcol.LogNorm()
                 zorder=1,
             )
             ax.set_zlabel("$f(X)$", fontsize=16)
 
         ax.set_xticks(np.linspace(domain[0, 0], domain[0, 1], num=11))
         ax.set_yticks(np.linspace(domain[1, 0], domain[1, 1], num=11))
```

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/function_factory.py` & `f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/function_factory.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/pybenchfunction.py` & `f3dasm-1.5.0/src/f3dasm/_src/datageneration/functions/pybenchfunction.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/design/domain.py` & `f3dasm-1.5.0/src/f3dasm/_src/design/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,18 @@
 # =============================================================================
 
 from __future__ import annotations
 
 # Standard
 import math
 import pickle
-import sys
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import (Any, Dict, Iterable, Iterator, List, Optional, Sequence,
-                    Type)
-
-if sys.version_info < (3, 8):  # NOQA
-    from typing_extensions import Literal  # NOQA
-else:
-    from typing import Literal
+from typing import (Any, Dict, Iterable, Iterator, List, Literal, Optional,
+                    Sequence, Type)
 
 # Third-party core
 import numpy as np
 import pandas as pd
 from omegaconf import DictConfig, OmegaConf
 
 # Local
```

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/design/parameter.py` & `f3dasm-1.5.0/src/f3dasm/_src/design/parameter.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_columns.py` & `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_columns.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_data.py` & `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_data.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_io.py` & `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_io.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_jobqueue.py` & `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_jobqueue.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_newdata.py` & `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/_newdata.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/experimentdata.py` & `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/experimentdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,23 @@
 """
 
 #                                                                       Modules
 # =============================================================================
 
 from __future__ import annotations
 
-import inspect
 # Standard
-import sys
+import inspect
 import traceback
+from copy import copy
 from functools import wraps
 from pathlib import Path
 from time import sleep
-from typing import (Any, Callable, Dict, Iterable, Iterator, List, Optional,
-                    Tuple, Type)
-
-if sys.version_info < (3, 8):  # NOQA
-    from typing_extensions import Literal  # NOQA
-else:
-    from typing import Literal
+from typing import (Any, Callable, Dict, Iterable, Iterator, List, Literal,
+                    Optional, Tuple, Type)
 
 # Third-party
 import numpy as np
 import pandas as pd
 import xarray as xr
 from filelock import FileLock
 from hydra.utils import get_original_cwd
@@ -1436,34 +1431,37 @@
         """
         # Create the data generator object if a string reference is passed
         if isinstance(data_generator, str):
             data_generator: DataGenerator = _datagenerator_factory(
                 data_generator=data_generator,
                 domain=self.domain, kwargs=kwargs)
 
+        # Create a copy of the optimizer object
+        _optimizer = copy(optimizer)
+
         # Create the optimizer object if a string reference is passed
-        if isinstance(optimizer, str):
-            optimizer: Optimizer = _optimizer_factory(
-                optimizer, self.domain, hyperparameters)
+        if isinstance(_optimizer, str):
+            _optimizer: Optimizer = _optimizer_factory(
+                _optimizer, self.domain, hyperparameters)
 
         # Create the sampler object if a string reference is passed
         if isinstance(sampler, str):
             sampler: Sampler = _sampler_factory(sampler, self.domain)
 
-        if optimizer.type == 'scipy':
+        if _optimizer.type == 'scipy':
             self._iterate_scipy(
-                optimizer=optimizer, data_generator=data_generator,
+                optimizer=_optimizer, data_generator=data_generator,
                 iterations=iterations, kwargs=kwargs,
                 x0_selection=x0_selection,
                 sampler=sampler,
                 overwrite=overwrite,
                 callback=callback)
         else:
             self._iterate(
-                optimizer=optimizer, data_generator=data_generator,
+                optimizer=_optimizer, data_generator=data_generator,
                 iterations=iterations, kwargs=kwargs,
                 x0_selection=x0_selection,
                 sampler=sampler,
                 overwrite=overwrite,
                 callback=callback)
 
     def _iterate(self, optimizer: Optimizer, data_generator: DataGenerator,
@@ -1519,26 +1517,26 @@
             Raised when invalid x0_selection is specified
         """
         last_index = self.index[-1] if not self.index.empty else -1
 
         if isinstance(x0_selection, str):
             if x0_selection == 'new':
 
-                if iterations < optimizer.hyperparameters.population:
+                if iterations < optimizer._population:
                     raise ValueError(
                         f'For creating new samples, the total number of '
                         f'requested iterations ({iterations}) cannot be '
                         f'smaller than the population size '
-                        f'({optimizer.hyperparameters.population})')
+                        f'({optimizer._population})')
 
                 init_samples = ExperimentData.from_sampling(
                     domain=self.domain,
                     sampler=sampler,
-                    n_samples=optimizer.hyperparameters.population,
-                    seed=optimizer.seed)
+                    n_samples=optimizer._population,
+                    seed=optimizer._seed)
 
                 init_samples.evaluate(
                     data_generator=data_generator, kwargs=kwargs,
                     mode='sequential')
 
                 if callback is not None:
                     callback(init_samples)
@@ -1550,27 +1548,27 @@
                         indices=_indices,
                         add_if_not_exist=True)
 
                 else:
                     self.add_experiments(init_samples)
 
                 x0_selection = 'last'
-                iterations -= optimizer.hyperparameters.population
+                iterations -= optimizer._population
 
         x0 = x0_factory(experiment_data=self, mode=x0_selection,
-                        n_samples=optimizer.hyperparameters.population)
-        optimizer.set_data(x0)
+                        n_samples=optimizer._population)
+        optimizer._set_data(x0)
 
         optimizer._check_number_of_datapoints()
 
         optimizer._construct_model(data_generator)
 
         for _ in range(number_of_updates(
                 iterations,
-                population=optimizer.hyperparameters.population)):
+                population=optimizer._population)):
             new_samples = optimizer.update_step(data_generator)
 
             # If new_samples is a tuple of input_data and output_data
             if isinstance(new_samples, tuple):
                 new_samples = ExperimentData(
                     domain=self.domain,
                     input_data=new_samples[0],
@@ -1588,23 +1586,24 @@
                 self._overwrite_experiments(experiment_sample=new_samples,
                                             indices=_indices,
                                             add_if_not_exist=True)
 
             else:
                 self.add_experiments(new_samples)
 
-            optimizer.set_data(self)
+            optimizer._set_data(self)
 
         if not overwrite:
             # Remove overiterations
             self.remove_rows_bottom(number_of_overiterations(
-                iterations, population=optimizer.hyperparameters.population))
+                iterations,
+                population=optimizer._population))
 
         # Reset the optimizer
-        optimizer.reset(ExperimentData(domain=self.domain))
+        # optimizer.reset(ExperimentData(domain=self.domain))
 
     def _iterate_scipy(self, optimizer: Optimizer,
                        data_generator: DataGenerator,
                        iterations: int, kwargs: dict,
                        x0_selection: str | ExperimentData,
                        sampler: Sampler, overwrite: bool,
                        callback: Callable):
@@ -1659,26 +1658,26 @@
         """
         last_index = self.index[-1] if not self.index.empty else -1
         n_data_before_iterate = len(self)
 
         if isinstance(x0_selection, str):
             if x0_selection == 'new':
 
-                if iterations < optimizer.hyperparameters.population:
+                if iterations < optimizer._population:
                     raise ValueError(
                         f'For creating new samples, the total number of '
                         f'requested iterations ({iterations}) cannot be '
                         f'smaller than the population size '
-                        f'({optimizer.hyperparameters.population})')
+                        f'({optimizer._population})')
 
                 init_samples = ExperimentData.from_sampling(
                     domain=self.domain,
                     sampler=sampler,
-                    n_samples=optimizer.hyperparameters.population,
-                    seed=optimizer.seed)
+                    n_samples=optimizer._population,
+                    seed=optimizer._seed)
 
                 init_samples.evaluate(
                     data_generator=data_generator, kwargs=kwargs,
                     mode='sequential')
 
                 if callback is not None:
                     callback(init_samples)
@@ -1692,16 +1691,16 @@
 
                 else:
                     self.add_experiments(init_samples)
 
                 x0_selection = 'last'
 
         x0 = x0_factory(experiment_data=self, mode=x0_selection,
-                        n_samples=optimizer.hyperparameters.population)
-        optimizer.set_data(x0)
+                        n_samples=optimizer._population)
+        optimizer._set_data(x0)
 
         optimizer._check_number_of_datapoints()
 
         optimizer.run_algorithm(iterations, data_generator)
 
         new_samples: ExperimentData = optimizer.data.select(
             optimizer.data.index[1:])
@@ -1736,15 +1735,15 @@
                 while len(self) < n_data_before_iterate + iterations:
                     self.add_experiments(last_design)
 
         # Evaluate the function on the extra iterations
         self.evaluate(data_generator, mode='sequential', kwargs=kwargs)
 
         # Reset the optimizer
-        optimizer.reset(ExperimentData(domain=self.domain))
+        # optimizer.reset(ExperimentData(domain=self.domain))
 
     #                                                                  Sampling
     # =========================================================================
 
     def sample(self, sampler: Sampler | SamplerNames, n_samples: int = 1,
                seed: Optional[int] = None, **kwargs) -> None:
         """Sample data from the domain providing the sampler strategy
```

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/experimentsample.py` & `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/experimentsample.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,16 @@
 
 #                                                                       Modules
 # =============================================================================
 
 from __future__ import annotations
 
 # Standard
-import sys
 from pathlib import Path
-
-if sys.version_info < (3, 8):  # NOQA
-    from typing_extensions import Literal  # NOQA
-else:
-    from typing import Literal
-
-from typing import Any, Dict, Optional, Tuple, Type
+from typing import Any, Dict, Literal, Optional, Tuple, Type
 
 # Third-party
 import autograd.numpy as np
 
 # Local
 from ..design.domain import Domain
 from ..logger import logger
```

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/samplers.py` & `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/samplers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,16 @@
 
 #                                                                       Modules
 # =============================================================================
 
 from __future__ import annotations
 
 # Standard
-import sys
 from itertools import product
-
-if sys.version_info < (3, 8):  # NOQA
-    from typing_extensions import Literal, Protocol  # NOQA
-else:
-    from typing import Literal, Protocol
-
-from typing import Dict, Optional
+from typing import Dict, Literal, Optional, Protocol
 
 # Third-party
 import numpy as np
 import pandas as pd
 from SALib.sample import latin as salib_latin
 from SALib.sample import sobol_sequence
```

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/utils.py` & `f3dasm-1.5.0/src/f3dasm/_src/experimentdata/utils.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/hydra_utils.py` & `f3dasm-1.5.0/src/f3dasm/_src/hydra_utils.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/logger.py` & `f3dasm-1.5.0/src/f3dasm/_src/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 from time import sleep
 
 if os.name == 'nt':
     import msvcrt
 else:
     import fcntl
 
-from functools import partial, wraps
-from time import perf_counter
-from typing import Any, Callable
-
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
 #
@@ -115,25 +111,7 @@
     file
         file object that returns from open()
     """
     if os.name == 'nt':  # for Windows
         msvcrt.locking(file.fileno(), msvcrt.LK_UNLCK, 1)
     else:  # for Unix
         fcntl.flock(file, fcntl.LOCK_UN)
-
-
-def _time_and_log(
-    func: Callable, logger=logging.Logger
-) -> Callable:
-    @wraps(func)
-    def wrapper(*args: Any, **kwargs: Any) -> Any:
-        start_time = perf_counter()
-        value = func(*args, **kwargs)
-        logger.debug(
-            f"Called {func.__name__} and time taken: \
-                {perf_counter() - start_time:.2f}s")
-        return value
-
-    return wrapper
-
-
-time_and_log = partial(_time_and_log, logger=logger)
```

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/optimization/__init__.py` & `f3dasm-1.5.0/src/f3dasm/_src/optimization/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 #                                                                       Modules
 # =============================================================================
 
 # Standard
 from typing import List
 
 # Local
-from .cg import CG, CG_Parameters
-from .lbfgsb import LBFGSB, LBFGSB_Parameters
-from .neldermead import NelderMead, NelderMead_Parameters
+from .numpy_implementations import RandomSearch
 from .optimizer import Optimizer
-from .randomsearch import RandomSearch, RandomSearch_Parameters
+from .scipy_implementations import CG, LBFGSB, NelderMead
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
@@ -25,22 +23,18 @@
 
 # List of available optimizers
 _OPTIMIZERS: List[Optimizer] = [RandomSearch, CG, LBFGSB, NelderMead]
 
 
 __all__ = [
     'CG',
-    'CG_Parameters',
     'LBFGSB',
-    'LBFGSB_Parameters',
     'NelderMead',
-    'NelderMead_Parameters',
     'Optimizer',
     'RandomSearch',
-    'RandomSearch_Parameters',
     '_OPTIMIZERS',
     'find_optimizer',
 ]
 
 
 def find_optimizer(query: str) -> Optimizer:
     """Find a optimizer from the f3dasm.optimizer submodule
```

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/optimization/adapters/scipy_implementations.py` & `f3dasm-1.5.0/src/f3dasm/_src/optimization/adapters/scipy_implementations.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # Third-party core
 import autograd.numpy as np
 from scipy.optimize import minimize
 
 # Locals
 from ...datageneration.datagenerator import DataGenerator
+from ...design.domain import Domain
 from ...experimentdata.experimentsample import ExperimentSample
 from ..optimizer import Optimizer
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
@@ -25,14 +26,19 @@
 warnings.filterwarnings(
     "ignore", message="^OptimizeWarning: Unknown solver options.*")
 
 
 class _SciPyOptimizer(Optimizer):
     type: str = 'scipy'
 
+    def __init__(self, domain: Domain, method: str, **hyperparameters):
+        self.domain = domain
+        self.method = method
+        self.options = {**hyperparameters}
+
     def _callback(self, xk: np.ndarray, *args, **kwargs) -> None:
         self.data.add_experiments(
             ExperimentSample.from_numpy(xk, domain=self.domain))
 
     def update_step(self):
         """Update step function"""
         raise ValueError(
@@ -53,21 +59,19 @@
 
         def fun(x):
             sample: ExperimentSample = data_generator._run(
                 x, domain=self.domain)
             _, y = sample.to_numpy()
             return float(y)
 
-        self.hyperparameters.maxiter = iterations
+        self.options['maxiter'] = iterations
 
         minimize(
             fun=fun,
             method=self.method,
             jac=data_generator.dfdx,
             x0=self.data.get_n_best_output(1).to_numpy()[0].ravel(),
             callback=self._callback,
-            options=self.hyperparameters.__dict__,
+            options=self.options,
             bounds=self.domain.get_bounds(),
             tol=0.0,
         )
-
-        # self.data.evaluate(data_generator=data_generator)
```

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/optimization/optimizer_factory.py` & `f3dasm-1.5.0/src/f3dasm/_src/optimization/optimizer_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 Module for the data generator factory.
 """
 #                                                                       Modules
 # =============================================================================
 
+# Standard
 from typing import Any, Dict, Optional
 
+# Local
 from ..design.domain import Domain
 from . import _OPTIMIZERS
 from .optimizer import Optimizer
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
```

### Comparing `f3dasm-1.4.8/src/f3dasm/_src/optimization/randomsearch.py` & `f3dasm-1.5.0/src/f3dasm/_src/optimization/numpy_implementations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 """
-Random Search optimizer
+Optimizers based from the numpy library
 """
 
 #                                                                       Modules
 # =============================================================================
 
 # Standard
-from dataclasses import dataclass
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 # Third-party core
-import autograd.numpy as np
+import numpy as np
 
 # Locals
 from ..datageneration.datagenerator import DataGenerator
-from .optimizer import Optimizer, OptimizerParameters
+from ..design.domain import Domain
+from .optimizer import Optimizer
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
 #
 # =============================================================================
 
 
-@dataclass
-class RandomSearch_Parameters(OptimizerParameters):
-    """Hyperparameters for RandomSearch optimizer"""
-
-    pass
-
-
 class RandomSearch(Optimizer):
     """Naive random search"""
     require_gradients: bool = False
-    hyperparameters: RandomSearch_Parameters = RandomSearch_Parameters()
 
-    def set_seed(self):
-        np.random.seed(self.seed)
+    def __init__(self, domain: Domain, seed: Optional[int] = None, **kwargs):
+        self.domain = domain
+        self.seed = seed
+        self._set_algorithm()
+
+    def _set_algorithm(self):
+        self.algorithm = np.random.default_rng(self.seed)
 
     def update_step(
             self, data_generator: DataGenerator
     ) -> Tuple[np.ndarray, np.ndarray]:
         x_new = np.atleast_2d(
             [
-                np.random.uniform(
+                self.algorithm.uniform(
                     low=self.domain.get_bounds()[d, 0],
                     high=self.domain.get_bounds()[d, 1])
                 for d in range(len(self.domain))
             ]
         )
 
         # return the data
         return x_new, None
 
-    def get_info(self) -> List[str]:
+    def _get_info(self) -> List[str]:
         return ['Fast', 'Single-Solution']
```

### Comparing `f3dasm-1.4.8/src/f3dasm/datageneration/functions.py` & `f3dasm-1.5.0/src/f3dasm/datageneration/functions.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.8/src/f3dasm/hydra_tools.py` & `f3dasm-1.5.0/src/f3dasm/hydra_tools.py`

 * *Files identical despite different names*

