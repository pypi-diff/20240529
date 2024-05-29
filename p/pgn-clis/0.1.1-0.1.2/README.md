# Comparing `tmp/pgn_clis-0.1.1.tar.gz` & `tmp/pgn_clis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgn_clis-0.1.1.tar", last modified: Wed May 29 09:00:59 2024, max compression
+gzip compressed data, was "pgn_clis-0.1.2.tar", last modified: Wed May 29 10:53:30 2024, max compression
```

## Comparing `pgn_clis-0.1.1.tar` & `pgn_clis-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 09:00:59.108512 pgn_clis-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      340 2024-05-29 09:00:59.108512 pgn_clis-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-05-29 07:07:00.000000 pgn_clis-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      739 2024-05-29 09:00:55.000000 pgn_clis-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-29 09:00:59.108512 pgn_clis-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 09:00:59.098512 pgn_clis-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 09:00:59.098512 pgn_clis-0.1.1/src/pgn_clis/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-05-29 07:07:00.000000 pgn_clis-0.1.1/src/pgn_clis/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 09:00:59.108512 pgn_clis-0.1.1/src/pgn_clis/lib/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:42.000000 pgn_clis-0.1.1/src/pgn_clis/lib/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      340 2024-05-29 07:13:23.000000 pgn_clis-0.1.1/src/pgn_clis/lib/clean.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      278 2024-05-29 09:00:48.000000 pgn_clis-0.1.1/src/pgn_clis/lib/download.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-05-29 07:53:22.000000 pgn_clis-0.1.1/src/pgn_clis/lib/sans2ucis.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-05-29 08:19:20.000000 pgn_clis-0.1.1/src/pgn_clis/lib/style_sans.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 09:00:59.108512 pgn_clis-0.1.1/src/pgn_clis/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:52.000000 pgn_clis-0.1.1/src/pgn_clis/scripts/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      243 2024-05-29 07:14:41.000000 pgn_clis-0.1.1/src/pgn_clis/scripts/clean.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      432 2024-05-29 08:12:42.000000 pgn_clis-0.1.1/src/pgn_clis/scripts/download.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-29 07:53:46.000000 pgn_clis-0.1.1/src/pgn_clis/scripts/sans2ucis.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      526 2024-05-29 08:19:54.000000 pgn_clis-0.1.1/src/pgn_clis/scripts/style_sans.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 09:00:59.108512 pgn_clis-0.1.1/src/pgn_clis.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      340 2024-05-29 09:00:59.000000 pgn_clis-0.1.1/src/pgn_clis.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      577 2024-05-29 09:00:59.000000 pgn_clis-0.1.1/src/pgn_clis.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-29 09:00:59.000000 pgn_clis-0.1.1/src/pgn_clis.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      199 2024-05-29 09:00:59.000000 pgn_clis-0.1.1/src/pgn_clis.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-05-29 09:00:59.000000 pgn_clis-0.1.1/src/pgn_clis.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-29 09:00:59.000000 pgn_clis-0.1.1/src/pgn_clis.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:30.096379 pgn_clis-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      370 2024-05-29 10:53:30.096379 pgn_clis-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-05-29 07:07:00.000000 pgn_clis-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      757 2024-05-29 10:53:22.000000 pgn_clis-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-29 10:53:30.096379 pgn_clis-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:30.076380 pgn_clis-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:30.076380 pgn_clis-0.1.2/src/pgn_clis/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-05-29 07:07:00.000000 pgn_clis-0.1.2/src/pgn_clis/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:30.086380 pgn_clis-0.1.2/src/pgn_clis/lib/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:42.000000 pgn_clis-0.1.2/src/pgn_clis/lib/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      340 2024-05-29 07:13:23.000000 pgn_clis-0.1.2/src/pgn_clis/lib/clean.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      278 2024-05-29 09:00:48.000000 pgn_clis-0.1.2/src/pgn_clis/lib/download.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-05-29 07:53:22.000000 pgn_clis-0.1.2/src/pgn_clis/lib/sans2ucis.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-05-29 08:19:20.000000 pgn_clis-0.1.2/src/pgn_clis/lib/style_sans.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:30.096379 pgn_clis-0.1.2/src/pgn_clis/scripts/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:52.000000 pgn_clis-0.1.2/src/pgn_clis/scripts/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      243 2024-05-29 07:14:41.000000 pgn_clis-0.1.2/src/pgn_clis/scripts/clean.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      432 2024-05-29 08:12:42.000000 pgn_clis-0.1.2/src/pgn_clis/scripts/download.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-29 07:53:46.000000 pgn_clis-0.1.2/src/pgn_clis/scripts/sans2ucis.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      526 2024-05-29 08:19:54.000000 pgn_clis-0.1.2/src/pgn_clis/scripts/style_sans.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:30.096379 pgn_clis-0.1.2/src/pgn_clis.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      370 2024-05-29 10:53:30.000000 pgn_clis-0.1.2/src/pgn_clis.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      577 2024-05-29 10:53:30.000000 pgn_clis-0.1.2/src/pgn_clis.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-29 10:53:30.000000 pgn_clis-0.1.2/src/pgn_clis.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      199 2024-05-29 10:53:30.000000 pgn_clis-0.1.2/src/pgn_clis.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-29 10:53:30.000000 pgn_clis-0.1.2/src/pgn_clis.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-29 10:53:30.000000 pgn_clis-0.1.2/src/pgn_clis.egg-info/top_level.txt
```

### Comparing `pgn_clis-0.1.1/pyproject.toml` & `pgn_clis-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pgn-clis"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "package_description"
 dependencies = [
-  "chess-utils", "fs-tools"
+  "chess-utils", "chess-notation", "fs-tools"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/REPO.git"
```

### Comparing `pgn_clis-0.1.1/src/pgn_clis/scripts/sans2ucis.py` & `pgn_clis-0.1.2/src/pgn_clis/scripts/sans2ucis.py`

 * *Files identical despite different names*

### Comparing `pgn_clis-0.1.1/src/pgn_clis/scripts/style_sans.py` & `pgn_clis-0.1.2/src/pgn_clis/scripts/style_sans.py`

 * *Files identical despite different names*

### Comparing `pgn_clis-0.1.1/src/pgn_clis.egg-info/SOURCES.txt` & `pgn_clis-0.1.2/src/pgn_clis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

