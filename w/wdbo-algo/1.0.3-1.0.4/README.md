# Comparing `tmp/wdbo_algo-1.0.3.tar.gz` & `tmp/wdbo_algo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wdbo_algo-1.0.3.tar", last modified: Wed May 29 16:26:36 2024, max compression
+gzip compressed data, was "wdbo_algo-1.0.4.tar", last modified: Wed May 29 16:42:54 2024, max compression
```

## Comparing `wdbo_algo-1.0.3.tar` & `wdbo_algo-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 flxinxout  (1000) flxinxout  (1000)        0 2024-05-29 16:26:36.944210 wdbo_algo-1.0.3/
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)     1688 2024-05-28 20:39:29.000000 wdbo_algo-1.0.3/LICENCE
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      370 2024-05-29 16:26:36.944210 wdbo_algo-1.0.3/PKG-INFO
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       42 2024-05-29 15:49:42.000000 wdbo_algo-1.0.3/README.md
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       85 2024-05-29 14:05:51.000000 wdbo_algo-1.0.3/pyproject.toml
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       38 2024-05-29 16:26:36.944210 wdbo_algo-1.0.3/setup.cfg
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      461 2024-05-29 16:26:13.000000 wdbo_algo-1.0.3/setup.py
-drwxr-xr-x   0 flxinxout  (1000) flxinxout  (1000)        0 2024-05-29 16:26:36.944210 wdbo_algo-1.0.3/wdbo_algo.egg-info/
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      370 2024-05-29 16:26:36.000000 wdbo_algo-1.0.3/wdbo_algo.egg-info/PKG-INFO
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      205 2024-05-29 16:26:36.000000 wdbo_algo-1.0.3/wdbo_algo.egg-info/SOURCES.txt
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)        1 2024-05-29 16:26:36.000000 wdbo_algo-1.0.3/wdbo_algo.egg-info/dependency_links.txt
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       38 2024-05-29 16:26:36.000000 wdbo_algo-1.0.3/wdbo_algo.egg-info/requires.txt
--rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)        1 2024-05-29 16:26:36.000000 wdbo_algo-1.0.3/wdbo_algo.egg-info/top_level.txt
+drwxr-xr-x   0 flxinxout  (1000) flxinxout  (1000)        0 2024-05-29 16:42:54.574203 wdbo_algo-1.0.4/
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)     1688 2024-05-28 20:39:29.000000 wdbo_algo-1.0.4/LICENCE
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      370 2024-05-29 16:42:54.574203 wdbo_algo-1.0.4/PKG-INFO
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       42 2024-05-29 15:49:42.000000 wdbo_algo-1.0.4/README.md
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       85 2024-05-29 14:05:51.000000 wdbo_algo-1.0.4/pyproject.toml
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       38 2024-05-29 16:42:54.574203 wdbo_algo-1.0.4/setup.cfg
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      461 2024-05-29 16:42:27.000000 wdbo_algo-1.0.4/setup.py
+drwxr-xr-x   0 flxinxout  (1000) flxinxout  (1000)        0 2024-05-29 16:42:54.574203 wdbo_algo-1.0.4/wdbo_algo.egg-info/
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      370 2024-05-29 16:42:54.000000 wdbo_algo-1.0.4/wdbo_algo.egg-info/PKG-INFO
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)      205 2024-05-29 16:42:54.000000 wdbo_algo-1.0.4/wdbo_algo.egg-info/SOURCES.txt
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)        1 2024-05-29 16:42:54.000000 wdbo_algo-1.0.4/wdbo_algo.egg-info/dependency_links.txt
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)       38 2024-05-29 16:42:54.000000 wdbo_algo-1.0.4/wdbo_algo.egg-info/requires.txt
+-rw-r--r--   0 flxinxout  (1000) flxinxout  (1000)        1 2024-05-29 16:42:54.000000 wdbo_algo-1.0.4/wdbo_algo.egg-info/top_level.txt
```

### Comparing `wdbo_algo-1.0.3/LICENCE` & `wdbo_algo-1.0.4/LICENCE`

 * *Files identical despite different names*

