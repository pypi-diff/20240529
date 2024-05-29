# Comparing `tmp/excel_normalizer-0.1.tar.gz` & `tmp/excel_normalizer-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel_normalizer-0.1.tar", last modified: Wed May 29 16:28:38 2024, max compression
+gzip compressed data, was "excel_normalizer-0.2.tar", last modified: Wed May 29 16:40:08 2024, max compression
```

## Comparing `excel_normalizer-0.1.tar` & `excel_normalizer-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 imac       (501) staff       (20)        0 2024-05-29 16:28:38.646509 excel_normalizer-0.1/
--rw-r--r--   0 imac       (501) staff       (20)     1064 2024-05-29 16:22:43.000000 excel_normalizer-0.1/LICENSE
--rw-r--r--   0 imac       (501) staff       (20)      318 2024-05-29 16:28:38.645693 excel_normalizer-0.1/PKG-INFO
--rw-r--r--   0 imac       (501) staff       (20)      111 2024-05-29 16:22:43.000000 excel_normalizer-0.1/README.md
-drwxr-xr-x   0 imac       (501) staff       (20)        0 2024-05-29 16:28:38.643077 excel_normalizer-0.1/excel_normalizer/
--rw-r--r--   0 imac       (501) staff       (20)        0 2024-05-29 16:11:14.000000 excel_normalizer-0.1/excel_normalizer/__init__.py
--rwxr-xr-x   0 imac       (501) staff       (20)     1348 2024-05-29 16:09:03.000000 excel_normalizer-0.1/excel_normalizer/cli.py
-drwxr-xr-x   0 imac       (501) staff       (20)        0 2024-05-29 16:28:38.645252 excel_normalizer-0.1/excel_normalizer.egg-info/
--rw-r--r--   0 imac       (501) staff       (20)      318 2024-05-29 16:28:38.000000 excel_normalizer-0.1/excel_normalizer.egg-info/PKG-INFO
--rw-r--r--   0 imac       (501) staff       (20)      321 2024-05-29 16:28:38.000000 excel_normalizer-0.1/excel_normalizer.egg-info/SOURCES.txt
--rw-r--r--   0 imac       (501) staff       (20)        1 2024-05-29 16:28:38.000000 excel_normalizer-0.1/excel_normalizer.egg-info/dependency_links.txt
--rw-r--r--   0 imac       (501) staff       (20)       56 2024-05-29 16:28:38.000000 excel_normalizer-0.1/excel_normalizer.egg-info/entry_points.txt
--rw-r--r--   0 imac       (501) staff       (20)       24 2024-05-29 16:28:38.000000 excel_normalizer-0.1/excel_normalizer.egg-info/requires.txt
--rw-r--r--   0 imac       (501) staff       (20)       17 2024-05-29 16:28:38.000000 excel_normalizer-0.1/excel_normalizer.egg-info/top_level.txt
--rw-r--r--   0 imac       (501) staff       (20)       38 2024-05-29 16:28:38.646678 excel_normalizer-0.1/setup.cfg
--rw-r--r--   0 imac       (501) staff       (20)      544 2024-05-29 16:13:44.000000 excel_normalizer-0.1/setup.py
+drwxr-xr-x   0 imac       (501) staff       (20)        0 2024-05-29 16:40:08.954669 excel_normalizer-0.2/
+-rw-r--r--   0 imac       (501) staff       (20)     1064 2024-05-29 16:22:43.000000 excel_normalizer-0.2/LICENSE
+-rw-r--r--   0 imac       (501) staff       (20)      470 2024-05-29 16:40:08.954278 excel_normalizer-0.2/PKG-INFO
+-rw-r--r--   0 imac       (501) staff       (20)      111 2024-05-29 16:22:43.000000 excel_normalizer-0.2/README.md
+drwxr-xr-x   0 imac       (501) staff       (20)        0 2024-05-29 16:40:08.952045 excel_normalizer-0.2/excel_normalizer/
+-rw-r--r--   0 imac       (501) staff       (20)        0 2024-05-29 16:11:14.000000 excel_normalizer-0.2/excel_normalizer/__init__.py
+-rwxr-xr-x   0 imac       (501) staff       (20)     1348 2024-05-29 16:09:03.000000 excel_normalizer-0.2/excel_normalizer/cli.py
+drwxr-xr-x   0 imac       (501) staff       (20)        0 2024-05-29 16:40:08.953896 excel_normalizer-0.2/excel_normalizer.egg-info/
+-rw-r--r--   0 imac       (501) staff       (20)      470 2024-05-29 16:40:08.000000 excel_normalizer-0.2/excel_normalizer.egg-info/PKG-INFO
+-rw-r--r--   0 imac       (501) staff       (20)      321 2024-05-29 16:40:08.000000 excel_normalizer-0.2/excel_normalizer.egg-info/SOURCES.txt
+-rw-r--r--   0 imac       (501) staff       (20)        1 2024-05-29 16:40:08.000000 excel_normalizer-0.2/excel_normalizer.egg-info/dependency_links.txt
+-rw-r--r--   0 imac       (501) staff       (20)       56 2024-05-29 16:40:08.000000 excel_normalizer-0.2/excel_normalizer.egg-info/entry_points.txt
+-rw-r--r--   0 imac       (501) staff       (20)       24 2024-05-29 16:40:08.000000 excel_normalizer-0.2/excel_normalizer.egg-info/requires.txt
+-rw-r--r--   0 imac       (501) staff       (20)       17 2024-05-29 16:40:08.000000 excel_normalizer-0.2/excel_normalizer.egg-info/top_level.txt
+-rw-r--r--   0 imac       (501) staff       (20)       38 2024-05-29 16:40:08.954957 excel_normalizer-0.2/setup.cfg
+-rw-r--r--   0 imac       (501) staff       (20)      800 2024-05-29 16:36:20.000000 excel_normalizer-0.2/setup.py
```

### Comparing `excel_normalizer-0.1/LICENSE` & `excel_normalizer-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `excel_normalizer-0.1/excel_normalizer/cli.py` & `excel_normalizer-0.2/excel_normalizer/cli.py`

 * *Files identical despite different names*

