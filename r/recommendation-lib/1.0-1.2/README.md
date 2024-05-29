# Comparing `tmp/recommendation_lib-1.0.tar.gz` & `tmp/recommendation_lib-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recommendation_lib-1.0.tar", last modified: Wed May 29 07:29:54 2024, max compression
+gzip compressed data, was "recommendation_lib-1.2.tar", last modified: Wed May 29 08:15:36 2024, max compression
```

## Comparing `recommendation_lib-1.0.tar` & `recommendation_lib-1.2.tar`

### file list

```diff
@@ -1,23 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 07:29:54.460148 recommendation_lib-1.0/
--rw-rw-rw-   0        0        0      214 2024-05-29 07:29:54.454616 recommendation_lib-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-29 07:29:54.343422 recommendation_lib-1.0/general_tools/
--rw-rw-rw-   0        0        0        0 2024-05-27 22:28:14.000000 recommendation_lib-1.0/general_tools/__init__.py
--rw-rw-rw-   0        0        0      785 2024-05-26 13:37:53.000000 recommendation_lib-1.0/general_tools/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-29 07:29:54.362111 recommendation_lib-1.0/postgres/
--rw-rw-rw-   0        0        0        0 2024-05-27 22:28:25.000000 recommendation_lib-1.0/postgres/__init__.py
--rw-rw-rw-   0        0        0     3801 2024-05-29 00:09:54.000000 recommendation_lib-1.0/postgres/functions.py
--rw-rw-rw-   0        0        0     1436 2024-05-28 17:21:25.000000 recommendation_lib-1.0/postgres/table_class.py
-drwxrwxrwx   0        0        0        0 2024-05-29 07:29:54.373111 recommendation_lib-1.0/preprocessing/
--rw-rw-rw-   0        0        0        0 2024-05-27 22:28:34.000000 recommendation_lib-1.0/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2941 2024-05-28 22:05:36.000000 recommendation_lib-1.0/preprocessing/preprocess.py
-drwxrwxrwx   0        0        0        0 2024-05-29 07:29:54.384344 recommendation_lib-1.0/recommendation/
--rw-rw-rw-   0        0        0        0 2024-05-27 22:33:29.000000 recommendation_lib-1.0/recommendation/__init__.py
--rw-rw-rw-   0        0        0     1520 2024-05-28 23:44:52.000000 recommendation_lib-1.0/recommendation/recommendation.py
-drwxrwxrwx   0        0        0        0 2024-05-29 07:29:54.447972 recommendation_lib-1.0/recommendation_lib.egg-info/
--rw-rw-rw-   0        0        0      214 2024-05-29 07:29:54.000000 recommendation_lib-1.0/recommendation_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2024-05-29 07:29:54.000000 recommendation_lib-1.0/recommendation_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 07:29:54.000000 recommendation_lib-1.0/recommendation_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-29 07:29:54.000000 recommendation_lib-1.0/recommendation_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       52 2024-05-29 07:29:54.000000 recommendation_lib-1.0/recommendation_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 07:29:54.461126 recommendation_lib-1.0/setup.cfg
--rw-rw-rw-   0        0        0      336 2024-05-27 22:30:30.000000 recommendation_lib-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:15:36.542785 recommendation_lib-1.2/
+-rw-rw-rw-   0        0        0      883 2024-05-29 01:06:20.000000 recommendation_lib-1.2/Dockerfile
+-rw-rw-rw-   0        0        0       97 2024-05-29 08:10:19.000000 recommendation_lib-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      302 2024-05-29 08:15:36.538787 recommendation_lib-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-29 08:09:33.000000 recommendation_lib-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 08:15:36.397801 recommendation_lib-1.2/app/
+-rw-rw-rw-   0        0        0        0 2024-05-29 00:52:06.000000 recommendation_lib-1.2/app/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:15:36.407144 recommendation_lib-1.2/app/core/
+-rw-rw-rw-   0        0        0        0 2024-05-29 07:59:28.000000 recommendation_lib-1.2/app/core/__init__.py
+-rw-rw-rw-   0        0        0     2974 2024-05-29 08:05:28.000000 recommendation_lib-1.2/app/core/main.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:15:36.441995 recommendation_lib-1.2/app/data/
+-rw-rw-rw-   0        0        0        0 2024-05-29 07:54:55.000000 recommendation_lib-1.2/app/data/__init__.py
+-rw-rw-rw-   0        0        0  4540272 2024-05-29 00:57:54.000000 recommendation_lib-1.2/app/data/content_owns.csv
+-rw-rw-rw-   0        0        0  4715753 2024-05-26 12:29:21.000000 recommendation_lib-1.2/app/data/machine_ratings.csv
+-rw-rw-rw-   0        0        0   422045 2024-05-26 12:29:25.000000 recommendation_lib-1.2/app/data/machines.csv
+drwxrwxrwx   0        0        0        0 2024-05-29 08:15:36.453460 recommendation_lib-1.2/app/general_tools/
+-rw-rw-rw-   0        0        0        0 2024-05-27 22:28:14.000000 recommendation_lib-1.2/app/general_tools/__init__.py
+-rw-rw-rw-   0        0        0      785 2024-05-26 13:37:53.000000 recommendation_lib-1.2/app/general_tools/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:15:36.468352 recommendation_lib-1.2/app/postgres/
+-rw-rw-rw-   0        0        0        0 2024-05-27 22:28:25.000000 recommendation_lib-1.2/app/postgres/__init__.py
+-rw-rw-rw-   0        0        0     3805 2024-05-29 08:04:57.000000 recommendation_lib-1.2/app/postgres/functions.py
+-rw-rw-rw-   0        0        0     1436 2024-05-28 17:21:25.000000 recommendation_lib-1.2/app/postgres/table_class.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:15:36.478484 recommendation_lib-1.2/app/preprocessing/
+-rw-rw-rw-   0        0        0        0 2024-05-27 22:28:34.000000 recommendation_lib-1.2/app/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2941 2024-05-28 22:05:36.000000 recommendation_lib-1.2/app/preprocessing/preprocess.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:15:36.488311 recommendation_lib-1.2/app/recommendation/
+-rw-rw-rw-   0        0        0        0 2024-05-27 22:33:29.000000 recommendation_lib-1.2/app/recommendation/__init__.py
+-rw-rw-rw-   0        0        0     1520 2024-05-28 23:44:52.000000 recommendation_lib-1.2/app/recommendation/recommendation.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:15:36.532078 recommendation_lib-1.2/recommendation_lib.egg-info/
+-rw-rw-rw-   0        0        0      302 2024-05-29 08:15:36.000000 recommendation_lib-1.2/recommendation_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2024-05-29 08:15:36.000000 recommendation_lib-1.2/recommendation_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:15:36.000000 recommendation_lib-1.2/recommendation_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-05-29 08:15:36.000000 recommendation_lib-1.2/recommendation_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      135 2024-05-29 07:45:12.000000 recommendation_lib-1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:15:36.543785 recommendation_lib-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      546 2024-05-29 08:15:10.000000 recommendation_lib-1.2/setup.py
```

### Comparing `recommendation_lib-1.0/general_tools/logger.py` & `recommendation_lib-1.2/app/general_tools/logger.py`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.0/postgres/functions.py` & `recommendation_lib-1.2/app/postgres/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import psycopg2
-from general_tools.logger import logger
+from app.general_tools.logger import logger
 import pandas as pd
 from sqlalchemy import text
 from psycopg2 import sql
 import csv
```

### Comparing `recommendation_lib-1.0/postgres/table_class.py` & `recommendation_lib-1.2/app/postgres/table_class.py`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.0/preprocessing/preprocess.py` & `recommendation_lib-1.2/app/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.0/recommendation/recommendation.py` & `recommendation_lib-1.2/app/recommendation/recommendation.py`

 * *Files identical despite different names*

