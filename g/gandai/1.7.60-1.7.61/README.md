# Comparing `tmp/gandai-1.7.60.tar.gz` & `tmp/gandai-1.7.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.60.tar", last modified: Wed May 29 13:43:56 2024, max compression
+gzip compressed data, was "gandai-1.7.61.tar", last modified: Wed May 29 14:26:53 2024, max compression
```

## Comparing `gandai-1.7.60.tar` & `gandai-1.7.61.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.097789 gandai-1.7.60/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.60/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 13:43:56.097598 gandai-1.7.60/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.088102 gandai-1.7.60/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.60/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.094834 gandai-1.7.60/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.60/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.60/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.60/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.60/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2623 2024-05-29 02:35:57.000000 gandai-1.7.60/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.60/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.60/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.60/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17445 2024-05-29 12:27:02.000000 gandai-1.7.60/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1673 2024-05-29 02:22:28.000000 gandai-1.7.60/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-29 00:06:01.000000 gandai-1.7.60/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17723 2024-05-29 13:23:39.000000 gandai-1.7.60/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10401 2024-05-29 00:06:00.000000 gandai-1.7.60/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    45533 2024-05-29 13:35:24.000000 gandai-1.7.60/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.60/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.60/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.60/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1697 2024-05-24 15:09:39.000000 gandai-1.7.60/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.60/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1700 2024-05-29 02:35:57.000000 gandai-1.7.60/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.60/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.60/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)    16796 2024-05-29 12:26:59.000000 gandai-1.7.60/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     4127 2024-05-29 02:22:25.000000 gandai-1.7.60/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-29 00:05:27.000000 gandai-1.7.60/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    13157 2024-05-29 13:23:36.000000 gandai-1.7.60/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.095594 gandai-1.7.60/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.60/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.095968 gandai-1.7.60/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.60/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.60/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.60/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.60/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.60/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.097079 gandai-1.7.60/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.60/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.60/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-24 15:09:36.000000 gandai-1.7.60/gandai/migrations/sql/240523-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3021 2024-05-28 15:04:19.000000 gandai-1.7.60/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-29 00:05:27.000000 gandai-1.7.60/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    31009 2024-05-29 13:35:22.000000 gandai-1.7.60/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.60/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1081 2024-05-24 15:09:36.000000 gandai-1.7.60/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:43:56.097389 gandai-1.7.60/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 13:43:56.000000 gandai-1.7.60/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-29 13:43:56.000000 gandai-1.7.60/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-29 13:43:56.000000 gandai-1.7.60/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-29 13:43:56.000000 gandai-1.7.60/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-29 13:43:48.000000 gandai-1.7.60/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-29 13:43:56.097827 gandai-1.7.60/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.60/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 14:26:53.098849 gandai-1.7.61/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.61/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 14:26:53.098609 gandai-1.7.61/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 14:26:53.088833 gandai-1.7.61/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.61/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 14:26:53.095516 gandai-1.7.61/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.61/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.61/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.61/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.61/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2623 2024-05-29 02:35:57.000000 gandai-1.7.61/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.61/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.61/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.61/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17445 2024-05-29 12:27:02.000000 gandai-1.7.61/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1673 2024-05-29 02:22:28.000000 gandai-1.7.61/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-29 00:06:01.000000 gandai-1.7.61/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17723 2024-05-29 13:23:39.000000 gandai-1.7.61/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10401 2024-05-29 00:06:00.000000 gandai-1.7.61/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    45551 2024-05-29 13:58:01.000000 gandai-1.7.61/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.61/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.61/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.61/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1697 2024-05-24 15:09:39.000000 gandai-1.7.61/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.61/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1700 2024-05-29 02:35:57.000000 gandai-1.7.61/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.61/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.61/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)    16796 2024-05-29 12:26:59.000000 gandai-1.7.61/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     4127 2024-05-29 02:22:25.000000 gandai-1.7.61/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-29 00:05:27.000000 gandai-1.7.61/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    13157 2024-05-29 13:23:36.000000 gandai-1.7.61/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 14:26:53.096327 gandai-1.7.61/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.61/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 14:26:53.096722 gandai-1.7.61/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.61/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.61/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.61/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.61/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.61/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 14:26:53.098032 gandai-1.7.61/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.61/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.61/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-24 15:09:36.000000 gandai-1.7.61/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3021 2024-05-28 15:04:19.000000 gandai-1.7.61/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-29 00:05:27.000000 gandai-1.7.61/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    31027 2024-05-29 13:57:59.000000 gandai-1.7.61/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.61/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1081 2024-05-24 15:09:36.000000 gandai-1.7.61/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 14:26:53.098360 gandai-1.7.61/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 14:26:53.000000 gandai-1.7.61/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-29 14:26:53.000000 gandai-1.7.61/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-29 14:26:53.000000 gandai-1.7.61/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-29 14:26:53.000000 gandai-1.7.61/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-29 14:26:44.000000 gandai-1.7.61/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-29 14:26:53.098939 gandai-1.7.61/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.61/setup.py
```

### Comparing `gandai-1.7.60/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x1a2f5766 (Wed May 29 13:35:22 2024 UTC)
-files sz: 31009
+moddate:  0x67345766 (Wed May 29 13:57:59 2024 UTC)
+files sz: 31027
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 15
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -3736,15 +3736,15 @@
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
          744           0 RESUME                   0
          
-         746           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
+         746           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps','import_searches')\n    ORDER BY created DESC\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
          764           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
@@ -3802,15 +3802,15 @@
                      306 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
-            "\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    "
+            "\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps','import_searches')\n    ORDER BY created DESC\n    ;\n    "
             'search_uid'
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
```

### Comparing `gandai-1.7.60/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/__pycache__/tasks.cpython-311.pyc` & `gandai-1.7.61/gandai/__pycache__/tasks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/analytics.py` & `gandai-1.7.61/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/constants.py` & `gandai-1.7.61/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/db.py` & `gandai-1.7.61/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/google.py` & `gandai-1.7.61/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/gpt.py` & `gandai-1.7.61/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/grata.py` & `gandai-1.7.61/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/helpers.py` & `gandai-1.7.61/gandai/helpers.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/main.py` & `gandai-1.7.61/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.61/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/migrations/db_seed.py` & `gandai-1.7.61/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/migrations/dealcloud.py` & `gandai-1.7.61/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.61/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/migrations/sql/schema.sql` & `gandai-1.7.61/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/models.py` & `gandai-1.7.61/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/query.py` & `gandai-1.7.61/gandai/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -753,15 +753,15 @@
         a.name,
         to_timestamp(e.created) as created 
     FROM event e
     JOIN actor a on e.actor_key = a.key
     JOIN search s on e.search_uid = s.uid
     WHERE 
         e.search_uid = :search_uid
-        AND e.type in ('import', 'criteria','google','google_maps')
+        AND e.type in ('import', 'criteria','google','google_maps','import_searches')
     ORDER BY created DESC
     ;
     """
     with db.connect() as conn:
         result = conn.execute(sqlalchemy.text(statement), {"search_uid": search_uid})
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
     return df
```

### Comparing `gandai-1.7.60/gandai/secrets.py` & `gandai-1.7.61/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai/tasks.py` & `gandai-1.7.61/gandai/tasks.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.60/gandai.egg-info/SOURCES.txt` & `gandai-1.7.61/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

