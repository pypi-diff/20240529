# Comparing `tmp/fuzzy_matrix_mamdani-1.0.tar.gz` & `tmp/fuzzy_matrix_mamdani-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzy_matrix_mamdani-1.0.tar", last modified: Wed Apr 26 08:26:16 2023, max compression
+gzip compressed data, was "fuzzy_matrix_mamdani-1.1.tar", last modified: Wed May 29 10:34:04 2024, max compression
```

## Comparing `fuzzy_matrix_mamdani-1.0.tar` & `fuzzy_matrix_mamdani-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 08:26:16.615200 fuzzy_matrix_mamdani-1.0/
--rw-rw-rw-   0        0        0      145 2023-04-26 08:26:16.616196 fuzzy_matrix_mamdani-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3637 2023-04-26 08:09:19.000000 fuzzy_matrix_mamdani-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 08:26:16.592260 fuzzy_matrix_mamdani-1.0/fuzzy_matrix_mamdani/
--rw-rw-rw-   0        0        0    14020 2023-04-26 04:26:06.000000 fuzzy_matrix_mamdani-1.0/fuzzy_matrix_mamdani/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 08:26:16.613207 fuzzy_matrix_mamdani-1.0/fuzzy_matrix_mamdani.egg-info/
--rw-rw-rw-   0        0        0      145 2023-04-26 08:26:16.000000 fuzzy_matrix_mamdani-1.0/fuzzy_matrix_mamdani.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-04-26 08:26:16.000000 fuzzy_matrix_mamdani-1.0/fuzzy_matrix_mamdani.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 08:26:16.000000 fuzzy_matrix_mamdani-1.0/fuzzy_matrix_mamdani.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-26 08:26:16.000000 fuzzy_matrix_mamdani-1.0/fuzzy_matrix_mamdani.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       21 2023-04-26 08:26:16.000000 fuzzy_matrix_mamdani-1.0/fuzzy_matrix_mamdani.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 08:26:16.619188 fuzzy_matrix_mamdani-1.0/setup.cfg
--rw-rw-rw-   0        0        0      255 2023-04-26 08:19:37.000000 fuzzy_matrix_mamdani-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:34:04.080363 fuzzy_matrix_mamdani-1.1/
+-rw-rw-rw-   0        0        0      145 2024-05-29 10:34:04.080363 fuzzy_matrix_mamdani-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3637 2023-04-26 08:09:19.000000 fuzzy_matrix_mamdani-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 10:34:03.974627 fuzzy_matrix_mamdani-1.1/fuzzy_matrix_mamdani/
+-rw-rw-rw-   0        0        0    14020 2023-04-26 04:26:06.000000 fuzzy_matrix_mamdani-1.1/fuzzy_matrix_mamdani/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:34:04.079366 fuzzy_matrix_mamdani-1.1/fuzzy_matrix_mamdani.egg-info/
+-rw-rw-rw-   0        0        0      145 2024-05-29 10:34:03.000000 fuzzy_matrix_mamdani-1.1/fuzzy_matrix_mamdani.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-29 10:34:03.000000 fuzzy_matrix_mamdani-1.1/fuzzy_matrix_mamdani.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 10:34:03.000000 fuzzy_matrix_mamdani-1.1/fuzzy_matrix_mamdani.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-29 10:34:03.000000 fuzzy_matrix_mamdani-1.1/fuzzy_matrix_mamdani.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       21 2024-05-29 10:34:03.000000 fuzzy_matrix_mamdani-1.1/fuzzy_matrix_mamdani.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 10:34:04.083365 fuzzy_matrix_mamdani-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      284 2024-05-29 10:27:03.000000 fuzzy_matrix_mamdani-1.1/setup.py
```

### Comparing `fuzzy_matrix_mamdani-1.0/README.md` & `fuzzy_matrix_mamdani-1.1/README.md`

 * *Files identical despite different names*

### Comparing `fuzzy_matrix_mamdani-1.0/fuzzy_matrix_mamdani/__init__.py` & `fuzzy_matrix_mamdani-1.1/fuzzy_matrix_mamdani/__init__.py`

 * *Files identical despite different names*

