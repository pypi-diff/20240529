# Comparing `tmp/mr_torch_utils-0.1.0.tar.gz` & `tmp/mr_torch_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mr_torch_utils-0.1.0.tar", last modified: Tue May 28 08:45:57 2024, max compression
+gzip compressed data, was "mr_torch_utils-0.1.1.tar", last modified: Wed May 29 10:53:36 2024, max compression
```

## Comparing `mr_torch_utils-0.1.0.tar` & `mr_torch_utils-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:57.222154 mr_torch_utils-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      325 2024-05-28 08:45:57.222154 mr_torch_utils-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-27 15:16:52.000000 mr_torch_utils-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      525 2024-05-28 08:45:36.000000 mr_torch_utils-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-28 08:45:57.222154 mr_torch_utils-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:57.212154 mr_torch_utils-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:57.212154 mr_torch_utils-0.1.0/src/mr_torch_utils.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      325 2024-05-28 08:45:57.000000 mr_torch_utils-0.1.0/src/mr_torch_utils.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      318 2024-05-28 08:45:57.000000 mr_torch_utils-0.1.0/src/mr_torch_utils.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-28 08:45:57.000000 mr_torch_utils-0.1.0/src/mr_torch_utils.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-28 08:45:57.000000 mr_torch_utils-0.1.0/src/mr_torch_utils.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-28 08:45:57.000000 mr_torch_utils-0.1.0/src/mr_torch_utils.egg-info/top_level.txt
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:57.212154 mr_torch_utils-0.1.0/src/torch_utils/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      119 2024-05-27 15:18:38.000000 mr_torch_utils-0.1.0/src/torch_utils/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-27 15:19:09.000000 mr_torch_utils-0.1.0/src/torch_utils/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      546 2024-05-27 19:10:05.000000 mr_torch_utils-0.1.0/src/torch_utils/datasets.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:36.249603 mr_torch_utils-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      325 2024-05-29 10:53:36.249603 mr_torch_utils-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-27 15:16:52.000000 mr_torch_utils-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      525 2024-05-29 10:53:29.000000 mr_torch_utils-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-29 10:53:36.249603 mr_torch_utils-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:36.249603 mr_torch_utils-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:36.249603 mr_torch_utils-0.1.1/src/mr_torch_utils.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      325 2024-05-29 10:53:36.000000 mr_torch_utils-0.1.1/src/mr_torch_utils.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      318 2024-05-29 10:53:36.000000 mr_torch_utils-0.1.1/src/mr_torch_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-29 10:53:36.000000 mr_torch_utils-0.1.1/src/mr_torch_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-29 10:53:36.000000 mr_torch_utils-0.1.1/src/mr_torch_utils.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-29 10:53:36.000000 mr_torch_utils-0.1.1/src/mr_torch_utils.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:36.249603 mr_torch_utils-0.1.1/src/torch_utils/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      119 2024-05-27 15:18:38.000000 mr_torch_utils-0.1.1/src/torch_utils/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       88 2024-05-29 10:39:55.000000 mr_torch_utils-0.1.1/src/torch_utils/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      856 2024-05-29 10:46:54.000000 mr_torch_utils-0.1.1/src/torch_utils/datasets.py
```

### Comparing `mr_torch_utils-0.1.0/pyproject.toml` & `mr_torch_utils-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mr-torch-utils"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "package_description"
 dependencies = [
   "lazy-loader"
 ]
```

