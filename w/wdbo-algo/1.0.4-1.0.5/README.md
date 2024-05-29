# Comparing `tmp/wdbo_algo-1.0.4.tar.gz` & `tmp/wdbo_algo-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wdbo_algo-1.0.4.tar", last modified: Wed May 29 16:42:54 2024, max compression
+gzip compressed data, was "wdbo_algo-1.0.5.tar", last modified: Wed May 29 16:58:15 2024, max compression
```

## Comparing `wdbo_algo-1.0.4.tar` & `wdbo_algo-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 flxinxout  (1000) flxinxout  (1000)        0 2024-05-29 16:42:54.574203 wdbo_algo-1.0.4/
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)     1688 2024-05-28 20:39:29.000000 wdbo_algo-1.0.4/LICENCE
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      370 2024-05-29 16:42:54.574203 wdbo_algo-1.0.4/PKG-INFO
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       42 2024-05-29 15:49:42.000000 wdbo_algo-1.0.4/README.md
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       85 2024-05-29 14:05:51.000000 wdbo_algo-1.0.4/pyproject.toml
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       38 2024-05-29 16:42:54.574203 wdbo_algo-1.0.4/setup.cfg
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      461 2024-05-29 16:42:27.000000 wdbo_algo-1.0.4/setup.py
-drwxr-xr-x   0 flxinxout  (1000) flxinxout  (1000)        0 2024-05-29 16:42:54.574203 wdbo_algo-1.0.4/wdbo_algo.egg-info/
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      370 2024-05-29 16:42:54.000000 wdbo_algo-1.0.4/wdbo_algo.egg-info/PKG-INFO
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      205 2024-05-29 16:42:54.000000 wdbo_algo-1.0.4/wdbo_algo.egg-info/SOURCES.txt
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)        1 2024-05-29 16:42:54.000000 wdbo_algo-1.0.4/wdbo_algo.egg-info/dependency_links.txt
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       38 2024-05-29 16:42:54.000000 wdbo_algo-1.0.4/wdbo_algo.egg-info/requires.txt
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)        1 2024-05-29 16:42:54.000000 wdbo_algo-1.0.4/wdbo_algo.egg-info/top_level.txt
+drwxr-xr-x   0 flxinxout  (1000) flxinxout  (1000)        0 2024-05-29 16:58:15.834214 wdbo_algo-1.0.5/
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)     1688 2024-05-28 20:39:29.000000 wdbo_algo-1.0.5/LICENCE
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      567 2024-05-29 16:58:15.834214 wdbo_algo-1.0.5/PKG-INFO
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       42 2024-05-29 15:49:42.000000 wdbo_algo-1.0.5/README.md
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      586 2024-05-29 16:57:51.000000 wdbo_algo-1.0.5/pyproject.toml
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       38 2024-05-29 16:58:15.834214 wdbo_algo-1.0.5/setup.cfg
+drwxr-xr-x   0 flxinxout  (1000) flxinxout  (1000)        0 2024-05-29 16:58:15.834214 wdbo_algo-1.0.5/src/
+drwxr-xr-x   0 flxinxout  (1000) flxinxout  (1000)        0 2024-05-29 16:58:15.834214 wdbo_algo-1.0.5/src/wdbo_algo/
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       35 2024-05-29 16:54:40.000000 wdbo_algo-1.0.5/src/wdbo_algo/__init__.py
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)     4017 2024-05-28 16:47:42.000000 wdbo_algo-1.0.5/src/wdbo_algo/model.py
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)     7825 2024-05-28 20:49:35.000000 wdbo_algo-1.0.5/src/wdbo_algo/optimizer.py
+drwxr-xr-x   0 flxinxout  (1000) flxinxout  (1000)        0 2024-05-29 16:58:15.834214 wdbo_algo-1.0.5/src/wdbo_algo.egg-info/
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      567 2024-05-29 16:58:15.000000 wdbo_algo-1.0.5/src/wdbo_algo.egg-info/PKG-INFO
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      292 2024-05-29 16:58:15.000000 wdbo_algo-1.0.5/src/wdbo_algo.egg-info/SOURCES.txt
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)        1 2024-05-29 16:58:15.000000 wdbo_algo-1.0.5/src/wdbo_algo.egg-info/dependency_links.txt
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       38 2024-05-29 16:58:15.000000 wdbo_algo-1.0.5/src/wdbo_algo.egg-info/requires.txt
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       10 2024-05-29 16:58:15.000000 wdbo_algo-1.0.5/src/wdbo_algo.egg-info/top_level.txt
```

### Comparing `wdbo_algo-1.0.4/LICENCE` & `wdbo_algo-1.0.5/LICENCE`

 * *Files identical despite different names*

