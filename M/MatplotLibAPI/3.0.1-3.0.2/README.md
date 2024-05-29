# Comparing `tmp/matplotlibapi-3.0.1.tar.gz` & `tmp/matplotlibapi-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlibapi-3.0.1.tar", last modified: Wed May 29 09:25:37 2024, max compression
+gzip compressed data, was "matplotlibapi-3.0.2.tar", last modified: Wed May 29 10:07:56 2024, max compression
```

## Comparing `matplotlibapi-3.0.1.tar` & `matplotlibapi-3.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:25:37.717265 matplotlibapi-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 09:25:33.000000 matplotlibapi-3.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:25:37.713265 matplotlibapi-3.0.1/MatplotLibAPI/
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-29 09:25:33.000000 matplotlibapi-3.0.1/MatplotLibAPI/Bubble.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-29 09:25:33.000000 matplotlibapi-3.0.1/MatplotLibAPI/Composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-29 09:25:33.000000 matplotlibapi-3.0.1/MatplotLibAPI/Network.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-29 09:25:33.000000 matplotlibapi-3.0.1/MatplotLibAPI/Pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-29 09:25:33.000000 matplotlibapi-3.0.1/MatplotLibAPI/Style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-29 09:25:33.000000 matplotlibapi-3.0.1/MatplotLibAPI/Table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-29 09:25:33.000000 matplotlibapi-3.0.1/MatplotLibAPI/Timeserie.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-29 09:25:33.000000 matplotlibapi-3.0.1/MatplotLibAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-29 09:25:33.000000 matplotlibapi-3.0.1/MatplotLibAPI/pdAccessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:25:37.717265 matplotlibapi-3.0.1/MatplotLibAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-29 09:25:37.000000 matplotlibapi-3.0.1/MatplotLibAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 09:25:37.000000 matplotlibapi-3.0.1/MatplotLibAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:25:37.000000 matplotlibapi-3.0.1/MatplotLibAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-29 09:25:37.000000 matplotlibapi-3.0.1/MatplotLibAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 09:25:37.000000 matplotlibapi-3.0.1/MatplotLibAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-29 09:25:37.717265 matplotlibapi-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-29 09:25:33.000000 matplotlibapi-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-29 09:25:33.000000 matplotlibapi-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:25:37.717265 matplotlibapi-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-29 09:25:33.000000 matplotlibapi-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:07:56.630848 matplotlibapi-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 10:07:48.000000 matplotlibapi-3.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:07:56.626848 matplotlibapi-3.0.2/MatplotLibAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-29 10:07:48.000000 matplotlibapi-3.0.2/MatplotLibAPI/Bubble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-29 10:07:48.000000 matplotlibapi-3.0.2/MatplotLibAPI/Composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-29 10:07:48.000000 matplotlibapi-3.0.2/MatplotLibAPI/Network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-29 10:07:48.000000 matplotlibapi-3.0.2/MatplotLibAPI/Pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-29 10:07:48.000000 matplotlibapi-3.0.2/MatplotLibAPI/Style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-29 10:07:48.000000 matplotlibapi-3.0.2/MatplotLibAPI/Table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-29 10:07:48.000000 matplotlibapi-3.0.2/MatplotLibAPI/Timeserie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-29 10:07:48.000000 matplotlibapi-3.0.2/MatplotLibAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-29 10:07:48.000000 matplotlibapi-3.0.2/MatplotLibAPI/pdAccessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:07:56.630848 matplotlibapi-3.0.2/MatplotLibAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-29 10:07:56.000000 matplotlibapi-3.0.2/MatplotLibAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 10:07:56.000000 matplotlibapi-3.0.2/MatplotLibAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:07:56.000000 matplotlibapi-3.0.2/MatplotLibAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-29 10:07:56.000000 matplotlibapi-3.0.2/MatplotLibAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 10:07:56.000000 matplotlibapi-3.0.2/MatplotLibAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-29 10:07:56.630848 matplotlibapi-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-29 10:07:48.000000 matplotlibapi-3.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-29 10:07:48.000000 matplotlibapi-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:07:56.630848 matplotlibapi-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-29 10:07:48.000000 matplotlibapi-3.0.2/setup.py
```

### Comparing `matplotlibapi-3.0.1/LICENSE` & `matplotlibapi-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlibapi-3.0.1/MatplotLibAPI/Bubble.py` & `matplotlibapi-3.0.2/MatplotLibAPI/Bubble.py`

 * *Files identical despite different names*

### Comparing `matplotlibapi-3.0.1/MatplotLibAPI/Composite.py` & `matplotlibapi-3.0.2/MatplotLibAPI/Composite.py`

 * *Files identical despite different names*

### Comparing `matplotlibapi-3.0.1/MatplotLibAPI/Network.py` & `matplotlibapi-3.0.2/MatplotLibAPI/Network.py`

 * *Files identical despite different names*

### Comparing `matplotlibapi-3.0.1/MatplotLibAPI/Pivot.py` & `matplotlibapi-3.0.2/MatplotLibAPI/Pivot.py`

 * *Files identical despite different names*

### Comparing `matplotlibapi-3.0.1/MatplotLibAPI/Style.py` & `matplotlibapi-3.0.2/MatplotLibAPI/Style.py`

 * *Files identical despite different names*

### Comparing `matplotlibapi-3.0.1/MatplotLibAPI/Table.py` & `matplotlibapi-3.0.2/MatplotLibAPI/Table.py`

 * *Files identical despite different names*

### Comparing `matplotlibapi-3.0.1/MatplotLibAPI/Timeserie.py` & `matplotlibapi-3.0.2/MatplotLibAPI/Timeserie.py`

 * *Files identical despite different names*

### Comparing `matplotlibapi-3.0.1/MatplotLibAPI/pdAccessor.py` & `matplotlibapi-3.0.2/MatplotLibAPI/pdAccessor.py`

 * *Files identical despite different names*

