# Comparing `tmp/MatplotLibAPI-1.0.tar.gz` & `tmp/MatplotLibAPI-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MatplotLibAPI-1.0.tar", last modified: Fri Oct 13 08:36:55 2023, max compression
+gzip compressed data, was "MatplotLibAPI-2.0.2.tar", last modified: Fri Oct 13 11:06:50 2023, max compression
```

## Comparing `MatplotLibAPI-1.0.tar` & `MatplotLibAPI-2.0.2.tar`

### file list

```diff
@@ -1,13 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 08:36:55.894468 MatplotLibAPI-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-13 08:36:43.000000 MatplotLibAPI-1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 08:36:55.894468 MatplotLibAPI-1.0/MatplotLibAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2023-10-13 08:36:55.000000 MatplotLibAPI-1.0/MatplotLibAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-10-13 08:36:55.000000 MatplotLibAPI-1.0/MatplotLibAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 08:36:55.000000 MatplotLibAPI-1.0/MatplotLibAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-13 08:36:55.000000 MatplotLibAPI-1.0/MatplotLibAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 08:36:55.000000 MatplotLibAPI-1.0/MatplotLibAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2023-10-13 08:36:55.894468 MatplotLibAPI-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-10-13 08:36:43.000000 MatplotLibAPI-1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-10-13 08:36:43.000000 MatplotLibAPI-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-13 08:36:55.894468 MatplotLibAPI-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-10-13 08:36:43.000000 MatplotLibAPI-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 11:06:50.381023 MatplotLibAPI-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 11:06:50.377023 MatplotLibAPI-2.0.2/MatplotLibAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/Bubble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/Composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/Network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/Pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/Table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/MatplotLibAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 11:06:50.377023 MatplotLibAPI-2.0.2/MatplotLibAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2023-10-13 11:06:50.000000 MatplotLibAPI-2.0.2/MatplotLibAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2023-10-13 11:06:50.000000 MatplotLibAPI-2.0.2/MatplotLibAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 11:06:50.000000 MatplotLibAPI-2.0.2/MatplotLibAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-13 11:06:50.000000 MatplotLibAPI-2.0.2/MatplotLibAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-13 11:06:50.000000 MatplotLibAPI-2.0.2/MatplotLibAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2023-10-13 11:06:50.381023 MatplotLibAPI-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-13 11:06:50.381023 MatplotLibAPI-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2023-10-13 11:06:37.000000 MatplotLibAPI-2.0.2/setup.py
```

### Comparing `MatplotLibAPI-1.0/LICENSE` & `MatplotLibAPI-2.0.2/LICENSE`

 * *Files identical despite different names*

