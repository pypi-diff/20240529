# Comparing `tmp/turbo2csv-0.1.tar.gz` & `tmp/turbo2csv-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo2csv-0.1.tar", last modified: Tue May 28 20:22:43 2024, max compression
+gzip compressed data, was "turbo2csv-1.1.0.tar", last modified: Tue May 28 20:24:42 2024, max compression
```

## Comparing `turbo2csv-0.1.tar` & `turbo2csv-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 ziya       (501) staff       (20)        0 2024-05-28 20:22:43.868993 turbo2csv-0.1/
--rw-r--r--   0 ziya       (501) staff       (20)     1070 2024-05-28 19:44:18.000000 turbo2csv-0.1/LICENSE
--rw-r--r--   0 ziya       (501) staff       (20)       97 2024-05-28 20:22:43.868766 turbo2csv-0.1/PKG-INFO
--rw-r--r--   0 ziya       (501) staff       (20)     1324 2024-05-28 20:10:42.000000 turbo2csv-0.1/README.md
--rw-r--r--   0 ziya       (501) staff       (20)       38 2024-05-28 20:22:43.869132 turbo2csv-0.1/setup.cfg
--rw-r--r--   0 ziya       (501) staff       (20)      289 2024-05-28 20:05:28.000000 turbo2csv-0.1/setup.py
-drwxr-xr-x   0 ziya       (501) staff       (20)        0 2024-05-28 20:22:43.866749 turbo2csv-0.1/tests/
--rw-r--r--   0 ziya       (501) staff       (20)      665 2024-05-28 20:03:55.000000 turbo2csv-0.1/tests/test_scrape.py
-drwxr-xr-x   0 ziya       (501) staff       (20)        0 2024-05-28 20:22:43.867214 turbo2csv-0.1/turbo2csv/
--rw-r--r--   0 ziya       (501) staff       (20)        0 2024-05-28 20:04:06.000000 turbo2csv-0.1/turbo2csv/__init__.py
--rw-r--r--   0 ziya       (501) staff       (20)     2827 2024-05-28 20:00:09.000000 turbo2csv-0.1/turbo2csv/scraper.py
-drwxr-xr-x   0 ziya       (501) staff       (20)        0 2024-05-28 20:22:43.868487 turbo2csv-0.1/turbo2csv.egg-info/
--rw-r--r--   0 ziya       (501) staff       (20)       97 2024-05-28 20:22:43.000000 turbo2csv-0.1/turbo2csv.egg-info/PKG-INFO
--rw-r--r--   0 ziya       (501) staff       (20)      290 2024-05-28 20:22:43.000000 turbo2csv-0.1/turbo2csv.egg-info/SOURCES.txt
--rw-r--r--   0 ziya       (501) staff       (20)        1 2024-05-28 20:22:43.000000 turbo2csv-0.1/turbo2csv.egg-info/dependency_links.txt
--rw-r--r--   0 ziya       (501) staff       (20)       53 2024-05-28 20:22:43.000000 turbo2csv-0.1/turbo2csv.egg-info/entry_points.txt
--rw-r--r--   0 ziya       (501) staff       (20)        9 2024-05-28 20:22:43.000000 turbo2csv-0.1/turbo2csv.egg-info/requires.txt
--rw-r--r--   0 ziya       (501) staff       (20)       10 2024-05-28 20:22:43.000000 turbo2csv-0.1/turbo2csv.egg-info/top_level.txt
+drwxr-xr-x   0 ziya       (501) staff       (20)        0 2024-05-28 20:24:42.811900 turbo2csv-1.1.0/
+-rw-r--r--   0 ziya       (501) staff       (20)     1070 2024-05-28 19:44:18.000000 turbo2csv-1.1.0/LICENSE
+-rw-r--r--   0 ziya       (501) staff       (20)     2099 2024-05-28 20:24:42.811674 turbo2csv-1.1.0/PKG-INFO
+-rw-r--r--   0 ziya       (501) staff       (20)     1324 2024-05-28 20:10:42.000000 turbo2csv-1.1.0/README.md
+-rw-r--r--   0 ziya       (501) staff       (20)       38 2024-05-28 20:24:42.811959 turbo2csv-1.1.0/setup.cfg
+-rw-r--r--   0 ziya       (501) staff       (20)      970 2024-05-28 20:24:26.000000 turbo2csv-1.1.0/setup.py
+drwxr-xr-x   0 ziya       (501) staff       (20)        0 2024-05-28 20:24:42.809926 turbo2csv-1.1.0/tests/
+-rw-r--r--   0 ziya       (501) staff       (20)      665 2024-05-28 20:03:55.000000 turbo2csv-1.1.0/tests/test_scrape.py
+drwxr-xr-x   0 ziya       (501) staff       (20)        0 2024-05-28 20:24:42.810330 turbo2csv-1.1.0/turbo2csv/
+-rw-r--r--   0 ziya       (501) staff       (20)        0 2024-05-28 20:04:06.000000 turbo2csv-1.1.0/turbo2csv/__init__.py
+-rw-r--r--   0 ziya       (501) staff       (20)     2827 2024-05-28 20:00:09.000000 turbo2csv-1.1.0/turbo2csv/scraper.py
+drwxr-xr-x   0 ziya       (501) staff       (20)        0 2024-05-28 20:24:42.811373 turbo2csv-1.1.0/turbo2csv.egg-info/
+-rw-r--r--   0 ziya       (501) staff       (20)     2099 2024-05-28 20:24:42.000000 turbo2csv-1.1.0/turbo2csv.egg-info/PKG-INFO
+-rw-r--r--   0 ziya       (501) staff       (20)      254 2024-05-28 20:24:42.000000 turbo2csv-1.1.0/turbo2csv.egg-info/SOURCES.txt
+-rw-r--r--   0 ziya       (501) staff       (20)        1 2024-05-28 20:24:42.000000 turbo2csv-1.1.0/turbo2csv.egg-info/dependency_links.txt
+-rw-r--r--   0 ziya       (501) staff       (20)        9 2024-05-28 20:24:42.000000 turbo2csv-1.1.0/turbo2csv.egg-info/requires.txt
+-rw-r--r--   0 ziya       (501) staff       (20)       10 2024-05-28 20:24:42.000000 turbo2csv-1.1.0/turbo2csv.egg-info/top_level.txt
```

### Comparing `turbo2csv-0.1/LICENSE` & `turbo2csv-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `turbo2csv-0.1/README.md` & `turbo2csv-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `turbo2csv-0.1/tests/test_scrape.py` & `turbo2csv-1.1.0/tests/test_scrape.py`

 * *Files identical despite different names*

### Comparing `turbo2csv-0.1/turbo2csv/scraper.py` & `turbo2csv-1.1.0/turbo2csv/scraper.py`

 * *Files identical despite different names*

