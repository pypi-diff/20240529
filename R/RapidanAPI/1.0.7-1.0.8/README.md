# Comparing `tmp/RapidanAPI-1.0.7.tar.gz` & `tmp/RapidanAPI-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RapidanAPI-1.0.7.tar", last modified: Wed May 29 00:48:54 2024, max compression
+gzip compressed data, was "RapidanAPI-1.0.8.tar", last modified: Wed May 29 02:11:44 2024, max compression
```

## Comparing `RapidanAPI-1.0.7.tar` & `RapidanAPI-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:48:54.717196 RapidanAPI-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 00:48:29.000000 RapidanAPI-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-29 00:48:54.717196 RapidanAPI-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9321 2024-05-29 00:48:29.000000 RapidanAPI-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:48:54.713196 RapidanAPI-1.0.7/RapidanAPI/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-29 00:48:29.000000 RapidanAPI-1.0.7/RapidanAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-29 00:48:29.000000 RapidanAPI-1.0.7/RapidanAPI/energy_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 00:48:29.000000 RapidanAPI-1.0.7/RapidanAPI/global_oil_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:48:54.717196 RapidanAPI-1.0.7/RapidanAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-29 00:48:54.000000 RapidanAPI-1.0.7/RapidanAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-29 00:48:54.000000 RapidanAPI-1.0.7/RapidanAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 00:48:54.000000 RapidanAPI-1.0.7/RapidanAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 00:48:54.000000 RapidanAPI-1.0.7/RapidanAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 00:48:54.000000 RapidanAPI-1.0.7/RapidanAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 00:48:54.717196 RapidanAPI-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-29 00:48:29.000000 RapidanAPI-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:11:44.110383 RapidanAPI-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 02:11:22.000000 RapidanAPI-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-29 02:11:44.110383 RapidanAPI-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9321 2024-05-29 02:11:22.000000 RapidanAPI-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:11:44.110383 RapidanAPI-1.0.8/RapidanAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-29 02:11:22.000000 RapidanAPI-1.0.8/RapidanAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-29 02:11:22.000000 RapidanAPI-1.0.8/RapidanAPI/energy_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-29 02:11:22.000000 RapidanAPI-1.0.8/RapidanAPI/global_oil_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:11:44.110383 RapidanAPI-1.0.8/RapidanAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-29 02:11:44.000000 RapidanAPI-1.0.8/RapidanAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-29 02:11:44.000000 RapidanAPI-1.0.8/RapidanAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 02:11:44.000000 RapidanAPI-1.0.8/RapidanAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 02:11:44.000000 RapidanAPI-1.0.8/RapidanAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 02:11:44.000000 RapidanAPI-1.0.8/RapidanAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 02:11:44.110383 RapidanAPI-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-29 02:11:22.000000 RapidanAPI-1.0.8/setup.py
```

### Comparing `RapidanAPI-1.0.7/LICENSE` & `RapidanAPI-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `RapidanAPI-1.0.7/README.md` & `RapidanAPI-1.0.8/README.md`

 * *Files identical despite different names*

