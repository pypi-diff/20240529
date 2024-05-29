# Comparing `tmp/gandai-1.7.58.tar.gz` & `tmp/gandai-1.7.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.58.tar", last modified: Wed May 29 13:11:02 2024, max compression
+gzip compressed data, was "gandai-1.7.60.tar", last modified: Wed May 29 13:43:56 2024, max compression
```

## Comparing `gandai-1.7.58.tar` & `gandai-1.7.60.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.262579 gandai-1.7.58/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.58/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 13:11:02.262356 gandai-1.7.58/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.253052 gandai-1.7.58/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.58/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.258992 gandai-1.7.58/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.58/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.58/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.58/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.58/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2623 2024-05-29 02:35:57.000000 gandai-1.7.58/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.58/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.58/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.58/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17445 2024-05-29 12:27:02.000000 gandai-1.7.58/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1673 2024-05-29 02:22:28.000000 gandai-1.7.58/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-29 00:06:01.000000 gandai-1.7.58/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17789 2024-05-29 13:10:26.000000 gandai-1.7.58/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10401 2024-05-29 00:06:00.000000 gandai-1.7.58/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    45331 2024-05-29 13:10:08.000000 gandai-1.7.58/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.58/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.58/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.58/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1697 2024-05-24 15:09:39.000000 gandai-1.7.58/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.58/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1700 2024-05-29 02:35:57.000000 gandai-1.7.58/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.58/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.58/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)    16796 2024-05-29 12:26:59.000000 gandai-1.7.58/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     4127 2024-05-29 02:22:25.000000 gandai-1.7.58/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-29 00:05:27.000000 gandai-1.7.58/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    13149 2024-05-29 13:10:23.000000 gandai-1.7.58/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.259820 gandai-1.7.58/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.58/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.260358 gandai-1.7.58/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.58/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.58/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.58/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.58/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.58/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.261726 gandai-1.7.58/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.58/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.58/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-24 15:09:36.000000 gandai-1.7.58/gandai/migrations/sql/240523-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3021 2024-05-28 15:04:19.000000 gandai-1.7.58/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-29 00:05:27.000000 gandai-1.7.58/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    30959 2024-05-29 13:10:05.000000 gandai-1.7.58/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.58/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1081 2024-05-24 15:09:36.000000 gandai-1.7.58/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.262076 gandai-1.7.58/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 13:11:02.000000 gandai-1.7.58/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-29 13:11:02.000000 gandai-1.7.58/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-29 13:11:02.000000 gandai-1.7.58/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-29 13:11:02.000000 gandai-1.7.58/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-29 13:10:37.000000 gandai-1.7.58/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-29 13:11:02.262616 gandai-1.7.58/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.58/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.097789 gandai-1.7.60/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.60/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 13:43:56.097598 gandai-1.7.60/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.088102 gandai-1.7.60/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.60/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.094834 gandai-1.7.60/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.60/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.60/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.60/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.60/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2623 2024-05-29 02:35:57.000000 gandai-1.7.60/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.60/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.60/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.60/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17445 2024-05-29 12:27:02.000000 gandai-1.7.60/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1673 2024-05-29 02:22:28.000000 gandai-1.7.60/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-29 00:06:01.000000 gandai-1.7.60/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17723 2024-05-29 13:23:39.000000 gandai-1.7.60/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10401 2024-05-29 00:06:00.000000 gandai-1.7.60/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    45533 2024-05-29 13:35:24.000000 gandai-1.7.60/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.60/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.60/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.60/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1697 2024-05-24 15:09:39.000000 gandai-1.7.60/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.60/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1700 2024-05-29 02:35:57.000000 gandai-1.7.60/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.60/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.60/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)    16796 2024-05-29 12:26:59.000000 gandai-1.7.60/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     4127 2024-05-29 02:22:25.000000 gandai-1.7.60/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-29 00:05:27.000000 gandai-1.7.60/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    13157 2024-05-29 13:23:36.000000 gandai-1.7.60/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.095594 gandai-1.7.60/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.60/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.095968 gandai-1.7.60/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.60/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.60/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.60/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.60/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.60/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.097079 gandai-1.7.60/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.60/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.60/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-24 15:09:36.000000 gandai-1.7.60/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3021 2024-05-28 15:04:19.000000 gandai-1.7.60/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-29 00:05:27.000000 gandai-1.7.60/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    31009 2024-05-29 13:35:22.000000 gandai-1.7.60/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.60/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1081 2024-05-24 15:09:36.000000 gandai-1.7.60/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.097389 gandai-1.7.60/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 13:43:56.000000 gandai-1.7.60/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-29 13:43:56.000000 gandai-1.7.60/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-29 13:43:56.000000 gandai-1.7.60/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-29 13:43:56.000000 gandai-1.7.60/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-29 13:43:48.000000 gandai-1.7.60/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-29 13:43:56.097827 gandai-1.7.60/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.60/setup.py
```

### Comparing `gandai-1.7.58/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f295766 (Wed May 29 13:10:23 2024 UTC)
-files sz: 13149
+moddate:  0x582c5766 (Wed May 29 13:23:36 2024 UTC)
+files sz: 13157
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d025a020100640064
@@ -1043,41 +1043,40 @@
          firstlineno 133
          lnotab
             0x0202260102fe06062602020118fe04fe040842021601020102020e010e
             01020102ff0a041a011afe04fa04fd120f28012c010e010c01020102fc
       code
          argcount  : 1
          nlocals   : 5
-         stacksize : 11
+         stacksize : 10
          flags     : 3
          code
             0x970074010000000000000000000064017c00a6020000ab020000000000
             000000010064027402000000000000000000006a0200000000000000006a
             03000000000000000064039c0264027402000000000000000000006a0200
             000000000000006a04000000000000000064039c02640274020000000000
             00000000006a0200000000000000006a05000000000000000064039c0264
             027402000000000000000000006a0200000000000000006a060000000000
             00000064039c0264027402000000000000000000006a0200000000000000
-            006a07000000000000000064039c0264027402000000000000000000006a
-            0200000000000000006a08000000000000000064039c02640264047c006a
-            0900000000000000009b009d0264039c02640264057c006a0a0000000000
-            0000009b009d0264039c0264067c006a0b00000000000000006407190000
-            0000000000000064039c0267097d017402000000000000000000006a0200
-            00000000000000a00c00000000000000000000000000000000000000007c
-            01a6010000ab0100000000000000007d027401000000000000000000007c
-            02a6010000ab01000000000000000001007c026408190000000000000000
-            0044005d7e7d0374010000000000000000000064097c03a6020000ab0200
-            0000000000000001007c006a0900000000000000007c03640a3c00000074
-            1b000000000000000000007402000000000000000000006a0e0000000000
-            0000006a0f00000000000000007c03a6020000ab0200000000000000007d
-            047401000000000000000000007c04a6010000ab01000000000000000001
-            007c006a0b00000000000000006407190000000000000000007c046a0b00
-            0000000000000064073c0000007402000000000000000000006a10000000
-            0000000000a01100000000000000000000000000000000000000007c04a6
-            010000ab01000000000000000001008c7f64005300
+            006a07000000000000000064039c02640264047c006a0800000000000000
+            009b009d0264039c02640264057c006a0900000000000000009b009d0264
+            039c0264067c006a0a000000000000000064071900000000000000000064
+            039c0267087d017402000000000000000000006a020000000000000000a0
+            0b00000000000000000000000000000000000000007c01a6010000ab0100
+            000000000000007d027401000000000000000000007c02a6010000ab0100
+            0000000000000001007c0264081900000000000000000044005d7e7d0374
+            010000000000000000000064097c03a6020000ab02000000000000000001
+            007c006a0800000000000000007c03640a3c000000741900000000000000
+            0000007402000000000000000000006a0d00000000000000006a0e000000
+            00000000007c03a6020000ab0200000000000000007d0474010000000000
+            00000000007c04a6010000ab01000000000000000001007c006a0a000000
+            00000000006407190000000000000000007c046a0a000000000000000064
+            073c0000007402000000000000000000006a0f0000000000000000a01000
+            000000000000000000000000000000000000007c04a6010000ab01000000
+            000000000001008c7f64005300
          173           0 RESUME                   0
          
          174           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('prompt event:')
                       16 LOAD_FAST                0 (event)
                       18 PRECALL                  2
                       22 CALL                     2
@@ -1124,148 +1123,139 @@
          194         188 LOAD_GLOBAL              2 (ts)
                      200 LOAD_ATTR                2 (gpt)
                      210 LOAD_ATTR                7 (HOW_TO_GOOGLE_MAPS)
          
          192         220 LOAD_CONST               3 (('role', 'content'))
                      222 BUILD_CONST_KEY_MAP      2
          
-         197         224 LOAD_CONST               2 ('system')
-         
-         198         226 LOAD_GLOBAL              2 (ts)
-                     238 LOAD_ATTR                2 (gpt)
-                     248 LOAD_ATTR                8 (HOW_TO_SEARCH_GRATA_API)
-         
-         196         258 LOAD_CONST               3 (('role', 'content'))
-                     260 BUILD_CONST_KEY_MAP      2
-         
-         201         262 LOAD_CONST               2 ('system')
-         
-         202         264 LOAD_CONST               4 ('the search_uid is ')
-                     266 LOAD_FAST                0 (event)
-                     268 LOAD_ATTR                9 (search_uid)
-                     278 FORMAT_VALUE             0
-                     280 BUILD_STRING             2
-         
-         200         282 LOAD_CONST               3 (('role', 'content'))
-                     284 BUILD_CONST_KEY_MAP      2
-         
-         205         286 LOAD_CONST               2 ('system')
-         
-         206         288 LOAD_CONST               5 ('the actor_key is ')
-                     290 LOAD_FAST                0 (event)
-                     292 LOAD_ATTR               10 (actor_key)
-                     302 FORMAT_VALUE             0
-                     304 BUILD_STRING             2
-         
-         204         306 LOAD_CONST               3 (('role', 'content'))
-                     308 BUILD_CONST_KEY_MAP      2
-         
-         208         310 LOAD_CONST               6 ('user')
-                     312 LOAD_FAST                0 (event)
-                     314 LOAD_ATTR               11 (data)
-                     324 LOAD_CONST               7 ('prompt')
-                     326 BINARY_SUBSCR
-                     336 LOAD_CONST               3 (('role', 'content'))
-                     338 BUILD_CONST_KEY_MAP      2
-         
-         175         340 BUILD_LIST               9
-                     342 STORE_FAST               1 (messages)
-         
-         210         344 LOAD_GLOBAL              2 (ts)
-                     356 LOAD_ATTR                2 (gpt)
-                     366 LOAD_METHOD             12 (ask_gpt4)
-                     388 LOAD_FAST                1 (messages)
-                     390 PRECALL                  1
-                     394 CALL                     1
-                     404 STORE_FAST               2 (resp)
-         
-         212         406 LOAD_GLOBAL              1 (NULL + print)
-                     418 LOAD_FAST                2 (resp)
-                     420 PRECALL                  1
-                     424 CALL                     1
-                     434 POP_TOP
-         
-         213         436 LOAD_FAST                2 (resp)
-                     438 LOAD_CONST               8 ('events')
-                     440 BINARY_SUBSCR
-                     450 GET_ITER
-                 >>  452 FOR_ITER               126 (to 706)
-                     454 STORE_FAST               3 (new_event)
-         
-         214         456 LOAD_GLOBAL              1 (NULL + print)
-                     468 LOAD_CONST               9 ('new event:')
-                     470 LOAD_FAST                3 (new_event)
-                     472 PRECALL                  2
-                     476 CALL                     2
-                     486 POP_TOP
+         201         224 LOAD_CONST               2 ('system')
          
-         215         488 LOAD_FAST                0 (event)
-                     490 LOAD_ATTR                9 (search_uid)
-                     500 LOAD_FAST                3 (new_event)
-                     502 LOAD_CONST              10 ('search_uid')
-                     504 STORE_SUBSCR
-         
-         216         508 LOAD_GLOBAL             27 (NULL + from_dict)
-                     520 LOAD_GLOBAL              2 (ts)
-                     532 LOAD_ATTR               14 (models)
-                     542 LOAD_ATTR               15 (Event)
-                     552 LOAD_FAST                3 (new_event)
-                     554 PRECALL                  2
-                     558 CALL                     2
-                     568 STORE_FAST               4 (e)
-         
-         217         570 LOAD_GLOBAL              1 (NULL + print)
-                     582 LOAD_FAST                4 (e)
-                     584 PRECALL                  1
-                     588 CALL                     1
-                     598 POP_TOP
-         
-         219         600 LOAD_FAST                0 (event)
-                     602 LOAD_ATTR               11 (data)
-                     612 LOAD_CONST               7 ('prompt')
-                     614 BINARY_SUBSCR
-                     624 LOAD_FAST                4 (e)
-                     626 LOAD_ATTR               11 (data)
-                     636 LOAD_CONST               7 ('prompt')
-                     638 STORE_SUBSCR
-         
-         220         642 LOAD_GLOBAL              2 (ts)
-                     654 LOAD_ATTR               16 (query)
-                     664 LOAD_METHOD             17 (insert_event)
-                     686 LOAD_FAST                4 (e)
-                     688 PRECALL                  1
-                     692 CALL                     1
-                     702 POP_TOP
-                     704 JUMP_BACKWARD          127 (to 452)
+         202         226 LOAD_CONST               4 ('the search_uid is ')
+                     228 LOAD_FAST                0 (event)
+                     230 LOAD_ATTR                8 (search_uid)
+                     240 FORMAT_VALUE             0
+                     242 BUILD_STRING             2
+         
+         200         244 LOAD_CONST               3 (('role', 'content'))
+                     246 BUILD_CONST_KEY_MAP      2
+         
+         205         248 LOAD_CONST               2 ('system')
+         
+         206         250 LOAD_CONST               5 ('the actor_key is ')
+                     252 LOAD_FAST                0 (event)
+                     254 LOAD_ATTR                9 (actor_key)
+                     264 FORMAT_VALUE             0
+                     266 BUILD_STRING             2
+         
+         204         268 LOAD_CONST               3 (('role', 'content'))
+                     270 BUILD_CONST_KEY_MAP      2
+         
+         208         272 LOAD_CONST               6 ('user')
+                     274 LOAD_FAST                0 (event)
+                     276 LOAD_ATTR               10 (data)
+                     286 LOAD_CONST               7 ('prompt')
+                     288 BINARY_SUBSCR
+                     298 LOAD_CONST               3 (('role', 'content'))
+                     300 BUILD_CONST_KEY_MAP      2
+         
+         175         302 BUILD_LIST               8
+                     304 STORE_FAST               1 (messages)
+         
+         210         306 LOAD_GLOBAL              2 (ts)
+                     318 LOAD_ATTR                2 (gpt)
+                     328 LOAD_METHOD             11 (ask_gpt4)
+                     350 LOAD_FAST                1 (messages)
+                     352 PRECALL                  1
+                     356 CALL                     1
+                     366 STORE_FAST               2 (resp)
+         
+         212         368 LOAD_GLOBAL              1 (NULL + print)
+                     380 LOAD_FAST                2 (resp)
+                     382 PRECALL                  1
+                     386 CALL                     1
+                     396 POP_TOP
+         
+         213         398 LOAD_FAST                2 (resp)
+                     400 LOAD_CONST               8 ('events')
+                     402 BINARY_SUBSCR
+                     412 GET_ITER
+                 >>  414 FOR_ITER               126 (to 668)
+                     416 STORE_FAST               3 (new_event)
+         
+         214         418 LOAD_GLOBAL              1 (NULL + print)
+                     430 LOAD_CONST               9 ('new event:')
+                     432 LOAD_FAST                3 (new_event)
+                     434 PRECALL                  2
+                     438 CALL                     2
+                     448 POP_TOP
+         
+         215         450 LOAD_FAST                0 (event)
+                     452 LOAD_ATTR                8 (search_uid)
+                     462 LOAD_FAST                3 (new_event)
+                     464 LOAD_CONST              10 ('search_uid')
+                     466 STORE_SUBSCR
+         
+         216         470 LOAD_GLOBAL             25 (NULL + from_dict)
+                     482 LOAD_GLOBAL              2 (ts)
+                     494 LOAD_ATTR               13 (models)
+                     504 LOAD_ATTR               14 (Event)
+                     514 LOAD_FAST                3 (new_event)
+                     516 PRECALL                  2
+                     520 CALL                     2
+                     530 STORE_FAST               4 (e)
+         
+         217         532 LOAD_GLOBAL              1 (NULL + print)
+                     544 LOAD_FAST                4 (e)
+                     546 PRECALL                  1
+                     550 CALL                     1
+                     560 POP_TOP
+         
+         219         562 LOAD_FAST                0 (event)
+                     564 LOAD_ATTR               10 (data)
+                     574 LOAD_CONST               7 ('prompt')
+                     576 BINARY_SUBSCR
+                     586 LOAD_FAST                4 (e)
+                     588 LOAD_ATTR               10 (data)
+                     598 LOAD_CONST               7 ('prompt')
+                     600 STORE_SUBSCR
+         
+         220         604 LOAD_GLOBAL              2 (ts)
+                     616 LOAD_ATTR               15 (query)
+                     626 LOAD_METHOD             16 (insert_event)
+                     648 LOAD_FAST                4 (e)
+                     650 PRECALL                  1
+                     654 CALL                     1
+                     664 POP_TOP
+                     666 JUMP_BACKWARD          127 (to 414)
          
-         213     >>  706 LOAD_CONST               0 (None)
-                     708 RETURN_VALUE
+         213     >>  668 LOAD_CONST               0 (None)
+                     670 RETURN_VALUE
          consts
             None
             'prompt event:'
             'system'
             ('role', 'content')
             'the search_uid is '
             'the actor_key is '
             'user'
             'prompt'
             'events'
             'new event:'
             'search_uid'
-         names      ('print', 'ts', 'gpt', 'HOW_TO_RESPOND', 'HOW_TO_IMPORT', 'HOW_TO_TRANSITION', 'HOW_TO_GOOGLE', 'HOW_TO_GOOGLE_MAPS', 'HOW_TO_SEARCH_GRATA_API', 'search_uid', 'actor_key', 'data', 'ask_gpt4', 'from_dict', 'models', 'Event', 'query', 'insert_event')
+         names      ('print', 'ts', 'gpt', 'HOW_TO_RESPOND', 'HOW_TO_IMPORT', 'HOW_TO_TRANSITION', 'HOW_TO_GOOGLE', 'HOW_TO_GOOGLE_MAPS', 'search_uid', 'actor_key', 'data', 'ask_gpt4', 'from_dict', 'models', 'Event', 'query', 'insert_event')
          varnames   ('event', 'messages', 'resp', 'new_event', 'e')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'handle_prompt'
          firstlineno 173
          lnotab
             0x02012003020120fe0405020120fe0405020120fe0405020120fe040502
-            0120fe0405020120fe0405020112fe0405020112fe04041edf04233e021e
-            011401200114013e011e022a0140f9
+            0120fe0409020112fe0405020112fe04041edf04233e021e011401200114
+            013e011e022a0140f9
       'company'
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
```

### Comparing `gandai-1.7.58/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x2d295766 (Wed May 29 13:10:05 2024 UTC)
-files sz: 30959
+moddate:  0x1a2f5766 (Wed May 29 13:35:22 2024 UTC)
+files sz: 31009
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 15
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -956,185 +956,211 @@
          firstlineno 84
          lnotab 0x02013401160102ff10071e013a012c0128f52e0c
       'from_search'
       'to_search'
       'actor_key'
       code
          argcount  : 3
-         nlocals   : 8
+         nlocals   : 9
          stacksize : 7
          flags     : 3
          code
-            0x8701870297007401000000000000000000007c006a0100000000000000
-            00ac01a6010000ab0100000000000000007d037c037c0364021900000000
-            000000000064036b0300000000190000000000000000007d037c037c0364
-            021900000000000000000064046b0300000000190000000000000000007d
-            037405000000000000000000007c03a6010000ab01000000000000000001
-            007c03640519000000000000000000a00300000000000000000000000000
-            00000000000000a6000000ab0000000000000000007d0474050000000000
-            00000000007409000000000000000000007c04a6010000ab010000000000
-            000000a6010000ab0100000000000000000100740a000000000000000000
-            00a0060000000000000000000000000000000000000000a6000000ab0000
-            0000000000000035007d057c05a007000000000000000000000000000000
-            0000000000a6000000ab0000000000000000003500010088028801660264
-            0684087c044400a6000000ab0000000000000000007d067c05a008000000
-            00000000000000000000000000000000007413000000000000000000006a
-            0a00000000000000006407a6010000ab0100000000000000007c06a60200
-            00ab0200000000000000007d07640064006400a6020000ab020000000000
-            00000001006e0b2300310073047702780359007701010059000100010064
-            0064006400a6020000ab0200000000000000000100640053002300310073
-            047702780359007701010059000100010064005300
+            0x870187029700740100000000000000000000a6000000ab000000000000
+            0000007d037403000000000000000000007c006a020000000000000000ac
+            01a6010000ab0100000000000000007d047c047c04640219000000000000
+            00000064036b0300000000190000000000000000007d047c047c04640219
+            00000000000000000064046b0300000000190000000000000000007d0474
+            07000000000000000000007c04a6010000ab01000000000000000001007c
+            04640519000000000000000000a004000000000000000000000000000000
+            0000000000a6000000ab0000000000000000007d05740700000000000000
+            000000740b000000000000000000007c05a6010000ab0100000000000000
+            00a6010000ab0100000000000000000100740c00000000000000000000a0
+            070000000000000000000000000000000000000000a6000000ab00000000
+            000000000035007d067c06a0080000000000000000000000000000000000
+            000000a6000000ab00000000000000000035000100880288016602640684
+            087c054400a6000000ab0000000000000000007d077c06a0090000000000
+            0000000000000000000000000000007415000000000000000000006a0b00
+            000000000000006407a6010000ab0100000000000000007c07a6020000ab
+            0200000000000000007d08640064006400a6020000ab0200000000000000
+            0001006e0b23003100730477027803590077010100590001000100640064
+            006400a6020000ab02000000000000000001006e0b230031007304770278
+            0359007701010059000100010074070000000000000000000064087c086a
+            0c00000000000000009b006409740100000000000000000000a6000000ab
+            0000000000000000007c037a0a00009b00640a9d05a6010000ab01000000
+            0000000000010064005300
                        0 MAKE_CELL                1 (to_search)
                        2 MAKE_CELL                2 (actor_key)
          
          100           4 RESUME                   0
          
-         107           6 LOAD_GLOBAL              1 (NULL + search_targets)
-                      18 LOAD_FAST                0 (from_search)
-                      20 LOAD_ATTR                1 (uid)
-                      30 KW_NAMES                 1
-                      32 PRECALL                  1
-                      36 CALL                     1
-                      46 STORE_FAST               3 (targets)
-         
-         108          48 LOAD_FAST                3 (targets)
-                      50 LOAD_FAST                3 (targets)
-                      52 LOAD_CONST               2 ('stage')
-                      54 BINARY_SUBSCR
-                      64 LOAD_CONST               3 ('reject')
-                      66 COMPARE_OP               3 (!=)
-                      72 BINARY_SUBSCR
-                      82 STORE_FAST               3 (targets)
-         
-         109          84 LOAD_FAST                3 (targets)
-                      86 LOAD_FAST                3 (targets)
-                      88 LOAD_CONST               2 ('stage')
-                      90 BINARY_SUBSCR
-                     100 LOAD_CONST               4 ('create')
-                     102 COMPARE_OP               3 (!=)
-                     108 BINARY_SUBSCR
-                     118 STORE_FAST               3 (targets)
-         
-         110         120 LOAD_GLOBAL              5 (NULL + print)
-                     132 LOAD_FAST                3 (targets)
-                     134 PRECALL                  1
-                     138 CALL                     1
-                     148 POP_TOP
-         
-         111         150 LOAD_FAST                3 (targets)
-                     152 LOAD_CONST               5 ('domain')
-                     154 BINARY_SUBSCR
-                     164 LOAD_METHOD              3 (tolist)
-                     186 PRECALL                  0
-                     190 CALL                     0
-                     200 STORE_FAST               4 (domains)
-         
-         112         202 LOAD_GLOBAL              5 (NULL + print)
-                     214 LOAD_GLOBAL              9 (NULL + len)
-                     226 LOAD_FAST                4 (domains)
-                     228 PRECALL                  1
-                     232 CALL                     1
-                     242 PRECALL                  1
-                     246 CALL                     1
-                     256 POP_TOP
-         
-         114         258 LOAD_GLOBAL             10 (db)
-                     270 LOAD_METHOD              6 (connect)
-                     292 PRECALL                  0
-                     296 CALL                     0
-                     306 BEFORE_WITH
-                     308 STORE_FAST               5 (con)
-         
-         115         310 LOAD_FAST                5 (con)
-                     312 LOAD_METHOD              7 (begin)
-                     334 PRECALL                  0
-                     338 CALL                     0
-                     348 BEFORE_WITH
-                     350 POP_TOP
-         
-         116         352 LOAD_CLOSURE             2 (actor_key)
-                     354 LOAD_CLOSURE             1 (to_search)
-                     356 BUILD_TUPLE              2
-                     358 LOAD_CONST               6 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 116>)
-                     360 MAKE_FUNCTION            8 (closure)
-         
-         123         362 LOAD_FAST                4 (domains)
-         
-         116         364 GET_ITER
-                     366 PRECALL                  0
-                     370 CALL                     0
-                     380 STORE_FAST               6 (events)
-         
-         126         382 LOAD_FAST                5 (con)
-                     384 LOAD_METHOD              8 (execute)
-         
-         127         406 LOAD_GLOBAL             19 (NULL + sqlalchemy)
-                     418 LOAD_ATTR               10 (text)
-         
-         128         428 LOAD_CONST               7 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES (:search_uid, :domain, :actor_key, :type)\n                    ON CONFLICT DO NOTHING\n                    RETURNING id\n                    ')
-         
-         127         430 PRECALL                  1
-                     434 CALL                     1
-         
-         135         444 LOAD_FAST                6 (events)
-         
-         126         446 PRECALL                  2
-                     450 CALL                     2
-                     460 STORE_FAST               7 (result)
-         
-         115         462 LOAD_CONST               0 (None)
-                     464 LOAD_CONST               0 (None)
-                     466 LOAD_CONST               0 (None)
-                     468 PRECALL                  2
-                     472 CALL                     2
-                     482 POP_TOP
-                     484 JUMP_FORWARD            11 (to 508)
-                 >>  486 PUSH_EXC_INFO
-                     488 WITH_EXCEPT_START
-                     490 POP_JUMP_FORWARD_IF_TRUE     4 (to 500)
-                     492 RERAISE                  2
-                 >>  494 COPY                     3
-                     496 POP_EXCEPT
-                     498 RERAISE                  1
-                 >>  500 POP_TOP
-                     502 POP_EXCEPT
-                     504 POP_TOP
-                     506 POP_TOP
-         
-         114     >>  508 LOAD_CONST               0 (None)
-                     510 LOAD_CONST               0 (None)
-                     512 LOAD_CONST               0 (None)
-                     514 PRECALL                  2
-                     518 CALL                     2
-                     528 POP_TOP
-                     530 LOAD_CONST               0 (None)
-                     532 RETURN_VALUE
-                 >>  534 PUSH_EXC_INFO
-                     536 WITH_EXCEPT_START
-                     538 POP_JUMP_FORWARD_IF_TRUE     4 (to 548)
-                     540 RERAISE                  2
-                 >>  542 COPY                     3
-                     544 POP_EXCEPT
-                     546 RERAISE                  1
-                 >>  548 POP_TOP
-                     550 POP_EXCEPT
-                     552 POP_TOP
-                     554 POP_TOP
-                     556 LOAD_CONST               0 (None)
-                     558 RETURN_VALUE
+         104           6 LOAD_GLOBAL              1 (NULL + time)
+                      18 PRECALL                  0
+                      22 CALL                     0
+                      32 STORE_FAST               3 (t0)
+         
+         105          34 LOAD_GLOBAL              3 (NULL + search_targets)
+                      46 LOAD_FAST                0 (from_search)
+                      48 LOAD_ATTR                2 (uid)
+                      58 KW_NAMES                 1
+                      60 PRECALL                  1
+                      64 CALL                     1
+                      74 STORE_FAST               4 (targets)
+         
+         106          76 LOAD_FAST                4 (targets)
+                      78 LOAD_FAST                4 (targets)
+                      80 LOAD_CONST               2 ('stage')
+                      82 BINARY_SUBSCR
+                      92 LOAD_CONST               3 ('reject')
+                      94 COMPARE_OP               3 (!=)
+                     100 BINARY_SUBSCR
+                     110 STORE_FAST               4 (targets)
+         
+         107         112 LOAD_FAST                4 (targets)
+                     114 LOAD_FAST                4 (targets)
+                     116 LOAD_CONST               2 ('stage')
+                     118 BINARY_SUBSCR
+                     128 LOAD_CONST               4 ('create')
+                     130 COMPARE_OP               3 (!=)
+                     136 BINARY_SUBSCR
+                     146 STORE_FAST               4 (targets)
+         
+         108         148 LOAD_GLOBAL              7 (NULL + print)
+                     160 LOAD_FAST                4 (targets)
+                     162 PRECALL                  1
+                     166 CALL                     1
+                     176 POP_TOP
+         
+         109         178 LOAD_FAST                4 (targets)
+                     180 LOAD_CONST               5 ('domain')
+                     182 BINARY_SUBSCR
+                     192 LOAD_METHOD              4 (tolist)
+                     214 PRECALL                  0
+                     218 CALL                     0
+                     228 STORE_FAST               5 (domains)
+         
+         110         230 LOAD_GLOBAL              7 (NULL + print)
+                     242 LOAD_GLOBAL             11 (NULL + len)
+                     254 LOAD_FAST                5 (domains)
+                     256 PRECALL                  1
+                     260 CALL                     1
+                     270 PRECALL                  1
+                     274 CALL                     1
+                     284 POP_TOP
+         
+         112         286 LOAD_GLOBAL             12 (db)
+                     298 LOAD_METHOD              7 (connect)
+                     320 PRECALL                  0
+                     324 CALL                     0
+                     334 BEFORE_WITH
+                     336 STORE_FAST               6 (con)
+         
+         113         338 LOAD_FAST                6 (con)
+                     340 LOAD_METHOD              8 (begin)
+                     362 PRECALL                  0
+                     366 CALL                     0
+                     376 BEFORE_WITH
+                     378 POP_TOP
+         
+         114         380 LOAD_CLOSURE             2 (actor_key)
+                     382 LOAD_CLOSURE             1 (to_search)
+                     384 BUILD_TUPLE              2
+                     386 LOAD_CONST               6 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 114>)
+                     388 MAKE_FUNCTION            8 (closure)
+         
+         121         390 LOAD_FAST                5 (domains)
+         
+         114         392 GET_ITER
+                     394 PRECALL                  0
+                     398 CALL                     0
+                     408 STORE_FAST               7 (events)
+         
+         124         410 LOAD_FAST                6 (con)
+                     412 LOAD_METHOD              9 (execute)
+         
+         125         434 LOAD_GLOBAL             21 (NULL + sqlalchemy)
+                     446 LOAD_ATTR               11 (text)
+         
+         126         456 LOAD_CONST               7 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES (:search_uid, :domain, :actor_key, :type)\n                    ON CONFLICT DO NOTHING\n                    RETURNING id\n                    ')
+         
+         125         458 PRECALL                  1
+                     462 CALL                     1
+         
+         133         472 LOAD_FAST                7 (events)
+         
+         124         474 PRECALL                  2
+                     478 CALL                     2
+                     488 STORE_FAST               8 (result)
+         
+         113         490 LOAD_CONST               0 (None)
+                     492 LOAD_CONST               0 (None)
+                     494 LOAD_CONST               0 (None)
+                     496 PRECALL                  2
+                     500 CALL                     2
+                     510 POP_TOP
+                     512 JUMP_FORWARD            11 (to 536)
+                 >>  514 PUSH_EXC_INFO
+                     516 WITH_EXCEPT_START
+                     518 POP_JUMP_FORWARD_IF_TRUE     4 (to 528)
+                     520 RERAISE                  2
+                 >>  522 COPY                     3
+                     524 POP_EXCEPT
+                     526 RERAISE                  1
+                 >>  528 POP_TOP
+                     530 POP_EXCEPT
+                     532 POP_TOP
+                     534 POP_TOP
+         
+         112     >>  536 LOAD_CONST               0 (None)
+                     538 LOAD_CONST               0 (None)
+                     540 LOAD_CONST               0 (None)
+                     542 PRECALL                  2
+                     546 CALL                     2
+                     556 POP_TOP
+                     558 JUMP_FORWARD            11 (to 582)
+                 >>  560 PUSH_EXC_INFO
+                     562 WITH_EXCEPT_START
+                     564 POP_JUMP_FORWARD_IF_TRUE     4 (to 574)
+                     566 RERAISE                  2
+                 >>  568 COPY                     3
+                     570 POP_EXCEPT
+                     572 RERAISE                  1
+                 >>  574 POP_TOP
+                     576 POP_EXCEPT
+                     578 POP_TOP
+                     580 POP_TOP
+         
+         136     >>  582 LOAD_GLOBAL              7 (NULL + print)
+                     594 LOAD_CONST               8 ('Inserted ')
+                     596 LOAD_FAST                8 (result)
+                     598 LOAD_ATTR               12 (rowcount)
+                     608 FORMAT_VALUE             0
+                     610 LOAD_CONST               9 (' events in ')
+                     612 LOAD_GLOBAL              1 (NULL + time)
+                     624 PRECALL                  0
+                     628 CALL                     0
+                     638 LOAD_FAST                3 (t0)
+                     640 BINARY_OP               10 (-)
+                     644 FORMAT_VALUE             0
+                     646 LOAD_CONST              10 (' seconds')
+                     648 BUILD_STRING             5
+                     650 PRECALL                  1
+                     654 CALL                     1
+                     664 POP_TOP
+                     666 LOAD_CONST               0 (None)
+                     668 RETURN_VALUE
          ExceptionTable:
-           308 to 348 -> 534 [1] lasti
-           350 to 460 -> 486 [2] lasti
-           462 to 484 -> 534 [1] lasti
-           486 to 492 -> 494 [4] lasti
-           494 to 498 -> 534 [1] lasti
-           500 to 500 -> 494 [4] lasti
-           502 to 506 -> 534 [1] lasti
-           534 to 540 -> 542 [3] lasti
-           548 to 548 -> 542 [3] lasti
+           336 to 376 -> 560 [1] lasti
+           378 to 488 -> 514 [2] lasti
+           490 to 512 -> 560 [1] lasti
+           514 to 520 -> 522 [4] lasti
+           522 to 526 -> 560 [1] lasti
+           528 to 528 -> 522 [4] lasti
+           530 to 534 -> 560 [1] lasti
+           560 to 566 -> 568 [3] lasti
+           574 to 574 -> 568 [3] lasti
          consts
             None
             ('search_uid',)
             'stage'
             'reject'
             'create'
             'domain'
@@ -1144,58 +1170,61 @@
                stacksize : 7
                flags     : 19
                code
                   0x9502970067007c005d0e7d0189036a0000000000000000007c01890264
                   0064019c0491028c0f5300
                              0 COPY_FREE_VARS           2
                
-               116           2 RESUME                   0
+               114           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                14 (to 38)
                
-               123          10 STORE_FAST               1 (domain)
+               121          10 STORE_FAST               1 (domain)
                
-               118          12 LOAD_DEREF               3 (to_search)
+               116          12 LOAD_DEREF               3 (to_search)
                             14 LOAD_ATTR                0 (uid)
                
-               119          24 LOAD_FAST                1 (domain)
+               117          24 LOAD_FAST                1 (domain)
                
-               120          26 LOAD_DEREF               2 (actor_key)
+               118          26 LOAD_DEREF               2 (actor_key)
                
-               121          28 LOAD_CONST               0 ('land')
+               119          28 LOAD_CONST               0 ('land')
                
-               117          30 LOAD_CONST               1 (('search_uid', 'domain', 'actor_key', 'type'))
+               115          30 LOAD_CONST               1 (('search_uid', 'domain', 'actor_key', 'type'))
                             32 BUILD_CONST_KEY_MAP      4
                
-               116          34 LIST_APPEND              2
+               114          34 LIST_APPEND              2
                             36 JUMP_BACKWARD           15 (to 8)
                        >>   38 RETURN_VALUE
                consts
                   'land'
                   ('search_uid', 'domain', 'actor_key', 'type')
                names      ('uid',)
                varnames   ('.0', 'domain')
                freevars   ('actor_key', 'to_search')
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '<listcomp>'
-               firstlineno 116
+               firstlineno 114
                lnotab 0x0a0702fb0c010201020102fc04ff
             '\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES (:search_uid, :domain, :actor_key, :type)\n                    ON CONFLICT DO NOTHING\n                    RETURNING id\n                    '
-         names      ('search_targets', 'uid', 'print', 'tolist', 'len', 'db', 'connect', 'begin', 'execute', 'sqlalchemy', 'text')
-         varnames   ('from_search', 'to_search', 'actor_key', 'targets', 'domains', 'con', 'events', 'result')
+            'Inserted '
+            ' events in '
+            ' seconds'
+         names      ('time', 'search_targets', 'uid', 'print', 'tolist', 'len', 'db', 'connect', 'begin', 'execute', 'sqlalchemy', 'text', 'rowcount')
+         varnames   ('from_search', 'to_search', 'actor_key', 't0', 'targets', 'domains', 'con', 'events', 'result')
          freevars   ()
          cellvars   ('to_search', 'actor_key')
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'important_targets_from_search'
          firstlineno 100
          lnotab
-            0x06072a01240124011e013401380234012a010a0702f9120a1801160102
-            ff0e0802f710f52eff
+            0x06041c012a01240124011e013401380234012a010a0702f9120a180116
+            0102ff0e0802f710f52eff2e18
       code
          argcount  : 1
          nlocals   : 12
          stacksize : 16
          flags     : 3
          code
             0x870c97007c006a000000000000000000a0010000000000000000000000
```

### Comparing `gandai-1.7.58/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/__pycache__/tasks.cpython-311.pyc` & `gandai-1.7.60/gandai/__pycache__/tasks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/analytics.py` & `gandai-1.7.60/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/constants.py` & `gandai-1.7.60/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/db.py` & `gandai-1.7.60/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/google.py` & `gandai-1.7.60/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/gpt.py` & `gandai-1.7.60/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/grata.py` & `gandai-1.7.60/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/helpers.py` & `gandai-1.7.60/gandai/helpers.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/main.py` & `gandai-1.7.60/gandai/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,18 +189,18 @@
             "role": "system",
             "content": ts.gpt.HOW_TO_GOOGLE,
         },
         {
             "role": "system",
             "content": ts.gpt.HOW_TO_GOOGLE_MAPS,
         },
-        {
-            "role": "system",
-            "content": ts.gpt.HOW_TO_SEARCH_GRATA_API,
-        },
+        # {
+        #     "role": "system",
+        #     "content": ts.gpt.HOW_TO_SEARCH_GRATA_API,
+        # },
         {
             "role": "system",
             "content": f"the search_uid is {event.search_uid}",
         },
         {
             "role": "system",
             "content": f"the actor_key is {event.actor_key}",
```

### Comparing `gandai-1.7.58/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.60/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/migrations/db_seed.py` & `gandai-1.7.60/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/migrations/dealcloud.py` & `gandai-1.7.60/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.60/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/migrations/sql/schema.sql` & `gandai-1.7.60/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/models.py` & `gandai-1.7.60/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/query.py` & `gandai-1.7.60/gandai/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,17 +97,15 @@
     return search
 
 
 def important_targets_from_search(
     from_search: ts.models.Search, to_search: ts.models.Search, actor_key: str
 ) -> None:
 
-    # import pdb
-
-    # pdb.set_trace()
+    t0 = time()
     targets = search_targets(search_uid=from_search.uid)
     targets = targets[targets["stage"] != "reject"]
     targets = targets[targets["stage"] != "create"]
     print(targets)
     domains: list = targets["domain"].tolist()
     print(len(domains))
 
@@ -131,14 +129,16 @@
                     ON CONFLICT DO NOTHING
                     RETURNING id
                     """
                 ),
                 events,  # Passing the list of dictionaries directly
             )
 
+    print(f"Inserted {result.rowcount} events in {time() - t0} seconds")
+
 
 def important_targets_from_event(event: ts.models.Event) -> None:
 
     source = event.data.get("source")
     targets = search_targets(search_uid=event.search_uid)
     stage_dict = targets.set_index("domain")["stage"].to_dict()
```

### Comparing `gandai-1.7.58/gandai/secrets.py` & `gandai-1.7.60/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai/tasks.py` & `gandai-1.7.60/gandai/tasks.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.58/gandai.egg-info/SOURCES.txt` & `gandai-1.7.60/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

