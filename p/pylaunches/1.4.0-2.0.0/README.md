# Comparing `tmp/pylaunches-1.4.0.tar.gz` & `tmp/pylaunches-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylaunches-1.4.0.tar", last modified: Sun Apr 16 20:02:32 2023, max compression
+gzip compressed data, was "pylaunches-2.0.0.tar", max compression
```

## Comparing `pylaunches-1.4.0.tar` & `pylaunches-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:02:32.661250 pylaunches-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-16 20:02:25.000000 pylaunches-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-16 20:02:32.661250 pylaunches-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-16 20:02:25.000000 pylaunches-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:02:32.661250 pylaunches-1.4.0/pylaunches/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:02:32.661250 pylaunches-1.4.0/pylaunches/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/objects/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/objects/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/objects/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/objects/starship.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:02:32.661250 pylaunches-1.4.0/pylaunches.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-16 20:02:32.000000 pylaunches-1.4.0/pylaunches.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-16 20:02:32.000000 pylaunches-1.4.0/pylaunches.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 20:02:32.000000 pylaunches-1.4.0/pylaunches.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 20:02:32.000000 pylaunches-1.4.0/pylaunches.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 20:02:32.000000 pylaunches-1.4.0/pylaunches.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-16 20:02:32.661250 pylaunches-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-16 20:02:32.000000 pylaunches-1.4.0/setup.py
+-rw-r--r--   0        0        0     1082 2024-05-29 08:31:43.312153 pylaunches-2.0.0/LICENSE
+-rw-r--r--   0        0        0      339 2024-05-29 08:31:43.312153 pylaunches-2.0.0/README.md
+-rw-r--r--   0        0        0      144 2024-05-29 08:31:43.316153 pylaunches-2.0.0/pylaunches/__init__.py
+-rw-r--r--   0        0        0     4742 2024-05-29 08:31:43.316153 pylaunches-2.0.0/pylaunches/api.py
+-rw-r--r--   0        0        0      314 2024-05-29 08:31:43.316153 pylaunches-2.0.0/pylaunches/const.py
+-rw-r--r--   0        0        0      107 2024-05-29 08:31:43.316153 pylaunches-2.0.0/pylaunches/exceptions.py
+-rw-r--r--   0        0        0     3299 2024-05-29 08:31:43.316153 pylaunches-2.0.0/pylaunches/types.py
+-rw-r--r--   0        0        0      753 2024-05-29 08:31:51.484136 pylaunches-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 pylaunches-2.0.0/PKG-INFO
```

### Comparing `pylaunches-1.4.0/LICENSE` & `pylaunches-2.0.0/LICENSE`

 * *Files identical despite different names*

