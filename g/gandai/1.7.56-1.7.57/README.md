# Comparing `tmp/gandai-1.7.56.tar.gz` & `tmp/gandai-1.7.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.56.tar", last modified: Wed May 29 03:05:17 2024, max compression
+gzip compressed data, was "gandai-1.7.57.tar", last modified: Wed May 29 03:55:58 2024, max compression
```

## Comparing `gandai-1.7.56.tar` & `gandai-1.7.57.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:05:17.013809 gandai-1.7.56/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.56/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 03:05:17.013560 gandai-1.7.56/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:05:17.004368 gandai-1.7.56/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.56/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:05:17.010493 gandai-1.7.56/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.56/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.56/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.56/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.56/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2623 2024-05-29 02:35:57.000000 gandai-1.7.56/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.56/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.56/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.56/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17446 2024-05-29 00:40:29.000000 gandai-1.7.56/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1673 2024-05-29 02:22:28.000000 gandai-1.7.56/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-29 00:06:01.000000 gandai-1.7.56/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17147 2024-05-29 02:56:12.000000 gandai-1.7.56/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10401 2024-05-29 00:06:00.000000 gandai-1.7.56/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    42475 2024-05-29 02:32:12.000000 gandai-1.7.56/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.56/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.56/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.56/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1697 2024-05-24 15:09:39.000000 gandai-1.7.56/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.56/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1700 2024-05-29 02:35:57.000000 gandai-1.7.56/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.56/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.56/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)    16797 2024-05-29 00:40:27.000000 gandai-1.7.56/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     4127 2024-05-29 02:22:25.000000 gandai-1.7.56/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-29 00:05:27.000000 gandai-1.7.56/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    12983 2024-05-29 02:56:09.000000 gandai-1.7.56/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:05:17.011275 gandai-1.7.56/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.56/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:05:17.011702 gandai-1.7.56/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.56/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.56/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.56/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.56/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.56/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:05:17.012999 gandai-1.7.56/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.56/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.56/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-24 15:09:36.000000 gandai-1.7.56/gandai/migrations/sql/240523-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3021 2024-05-28 15:04:19.000000 gandai-1.7.56/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-29 00:05:27.000000 gandai-1.7.56/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    29361 2024-05-29 02:32:09.000000 gandai-1.7.56/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.56/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1081 2024-05-24 15:09:36.000000 gandai-1.7.56/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:05:17.013296 gandai-1.7.56/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 03:05:16.000000 gandai-1.7.56/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-29 03:05:16.000000 gandai-1.7.56/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-29 03:05:16.000000 gandai-1.7.56/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-29 03:05:16.000000 gandai-1.7.56/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-29 03:05:08.000000 gandai-1.7.56/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-29 03:05:17.013889 gandai-1.7.56/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.56/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.158005 gandai-1.7.57/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.57/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 03:55:58.157795 gandai-1.7.57/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.148541 gandai-1.7.57/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.57/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.154660 gandai-1.7.57/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.57/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.57/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.57/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.57/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2623 2024-05-29 02:35:57.000000 gandai-1.7.57/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.57/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.57/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.57/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17446 2024-05-29 00:40:29.000000 gandai-1.7.57/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1673 2024-05-29 02:22:28.000000 gandai-1.7.57/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-29 00:06:01.000000 gandai-1.7.57/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17768 2024-05-29 03:54:02.000000 gandai-1.7.57/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10401 2024-05-29 00:06:00.000000 gandai-1.7.57/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    45062 2024-05-29 03:54:47.000000 gandai-1.7.57/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.57/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.57/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.57/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1697 2024-05-24 15:09:39.000000 gandai-1.7.57/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.57/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1700 2024-05-29 02:35:57.000000 gandai-1.7.57/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.57/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.57/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)    16797 2024-05-29 00:40:27.000000 gandai-1.7.57/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     4127 2024-05-29 02:22:25.000000 gandai-1.7.57/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-29 00:05:27.000000 gandai-1.7.57/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    13122 2024-05-29 03:53:59.000000 gandai-1.7.57/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.155449 gandai-1.7.57/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.57/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.155823 gandai-1.7.57/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.57/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.57/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.57/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.57/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.57/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.157280 gandai-1.7.57/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.57/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.57/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-24 15:09:36.000000 gandai-1.7.57/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3021 2024-05-28 15:04:19.000000 gandai-1.7.57/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-29 00:05:27.000000 gandai-1.7.57/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    31209 2024-05-29 03:54:45.000000 gandai-1.7.57/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.57/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1081 2024-05-24 15:09:36.000000 gandai-1.7.57/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.157562 gandai-1.7.57/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 03:55:58.000000 gandai-1.7.57/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-29 03:55:58.000000 gandai-1.7.57/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-29 03:55:58.000000 gandai-1.7.57/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-29 03:55:58.000000 gandai-1.7.57/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-29 03:55:48.000000 gandai-1.7.57/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-29 03:55:58.158040 gandai-1.7.57/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.57/setup.py
```

### Comparing `gandai-1.7.56/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x49995666 (Wed May 29 02:56:09 2024 UTC)
-files sz: 12983
+moddate:  0xd7a65666 (Wed May 29 03:53:59 2024 UTC)
+files sz: 13122
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d025a020100640064
@@ -134,42 +134,42 @@
                322 LOAD_CONST               9 ('return')
                324 LOAD_CONST               3 (None)
                326 BUILD_TUPLE              4
                328 LOAD_CONST              15 (<code object handle_prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 173>)
                330 MAKE_FUNCTION            4 (annotations)
                332 STORE_NAME              18 (handle_prompt)
    
-   221         334 LOAD_CONST              16 ('company')
+   223         334 LOAD_CONST              16 ('company')
                336 LOAD_NAME                4 (ts)
                338 LOAD_ATTR               11 (models)
                348 LOAD_ATTR               19 (Company)
                358 LOAD_CONST               9 ('return')
                360 LOAD_CONST               3 (None)
                362 BUILD_TUPLE              4
-               364 LOAD_CONST              17 (<code object enrich_with_gpt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 221>)
+               364 LOAD_CONST              17 (<code object enrich_with_gpt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 223>)
                366 MAKE_FUNCTION            4 (annotations)
                368 STORE_NAME              20 (enrich_with_gpt)
    
-   260         370 LOAD_CONST              11 ('event')
+   262         370 LOAD_CONST              11 ('event')
                372 LOAD_NAME                4 (ts)
                374 LOAD_ATTR               11 (models)
                384 LOAD_ATTR               14 (Event)
                394 LOAD_CONST               9 ('return')
                396 LOAD_CONST               3 (None)
                398 BUILD_TUPLE              4
-               400 LOAD_CONST              18 (<code object run_enrichment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 260>)
+               400 LOAD_CONST              18 (<code object run_enrichment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 262>)
                402 MAKE_FUNCTION            4 (annotations)
                404 STORE_NAME              21 (run_enrichment)
    
-   279         406 LOAD_CONST              19 ('event_id')
+   281         406 LOAD_CONST              19 ('event_id')
                408 LOAD_NAME               22 (int)
                410 LOAD_CONST               9 ('return')
                412 LOAD_CONST               3 (None)
                414 BUILD_TUPLE              4
-               416 LOAD_CONST              20 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 279>)
+               416 LOAD_CONST              20 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 281>)
                418 MAKE_FUNCTION            4 (annotations)
                420 STORE_NAME              23 (process_event)
                422 LOAD_CONST               3 (None)
                424 RETURN_VALUE
    consts
       0
       ('asdict',)
@@ -1043,38 +1043,41 @@
          firstlineno 133
          lnotab
             0x0202260102fe06062602020118fe04fe040842021601020102020e010e
             01020102ff0a041a011afe04fa04fd120f28012c010e010c01020102fc
       code
          argcount  : 1
          nlocals   : 5
-         stacksize : 9
+         stacksize : 11
          flags     : 3
          code
             0x970074010000000000000000000064017c00a6020000ab020000000000
             000000010064027402000000000000000000006a0200000000000000006a
             03000000000000000064039c0264027402000000000000000000006a0200
             000000000000006a04000000000000000064039c02640274020000000000
             00000000006a0200000000000000006a05000000000000000064039c0264
             027402000000000000000000006a0200000000000000006a060000000000
-            00000064039c02640264047c006a0700000000000000009b009d0264039c
-            02640264057c006a0800000000000000009b009d0264039c0264067c006a
-            09000000000000000064071900000000000000000064039c0267077d0174
-            02000000000000000000006a020000000000000000a00a00000000000000
-            000000000000000000000000007c01a6010000ab0100000000000000007d
-            027401000000000000000000007c02a6010000ab01000000000000000001
-            007c0264081900000000000000000044005d747d03740100000000000000
-            00000064097c03a6020000ab020000000000000000010074170000000000
-            00000000007402000000000000000000006a0c00000000000000006a0d00
-            000000000000007c03a6020000ab0200000000000000007d047401000000
-            000000000000007c04a6010000ab01000000000000000001007c006a0900
-            000000000000006407190000000000000000007c046a0900000000000000
-            0064073c0000007402000000000000000000006a0e0000000000000000a0
-            0f00000000000000000000000000000000000000007c04a6010000ab0100
-            0000000000000001008c7564005300
+            00000064039c0264027402000000000000000000006a0200000000000000
+            006a07000000000000000064039c0264027402000000000000000000006a
+            0200000000000000006a08000000000000000064039c02640264047c006a
+            0900000000000000009b009d0264039c02640264057c006a0a0000000000
+            0000009b009d0264039c0264067c006a0b00000000000000006407190000
+            0000000000000064039c0267097d017402000000000000000000006a0200
+            00000000000000a00c00000000000000000000000000000000000000007c
+            01a6010000ab0100000000000000007d027401000000000000000000007c
+            02a6010000ab01000000000000000001007c026408190000000000000000
+            0044005d7e7d0374010000000000000000000064097c03a6020000ab0200
+            0000000000000001007c006a0900000000000000007c03640a3c00000074
+            1b000000000000000000007402000000000000000000006a0e0000000000
+            0000006a0f00000000000000007c03a6020000ab0200000000000000007d
+            047401000000000000000000007c04a6010000ab01000000000000000001
+            007c006a0b00000000000000006407190000000000000000007c046a0b00
+            0000000000000064073c0000007402000000000000000000006a10000000
+            0000000000a01100000000000000000000000000000000000000007c04a6
+            010000ab01000000000000000001008c7f64005300
          173           0 RESUME                   0
          
          174           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('prompt event:')
                       16 LOAD_FAST                0 (event)
                       18 PRECALL                  2
                       22 CALL                     2
@@ -1103,141 +1106,166 @@
          186         112 LOAD_GLOBAL              2 (ts)
                      124 LOAD_ATTR                2 (gpt)
                      134 LOAD_ATTR                5 (HOW_TO_TRANSITION)
          
          184         144 LOAD_CONST               3 (('role', 'content'))
                      146 BUILD_CONST_KEY_MAP      2
          
-         197         148 LOAD_CONST               2 ('system')
+         189         148 LOAD_CONST               2 ('system')
          
-         198         150 LOAD_GLOBAL              2 (ts)
+         190         150 LOAD_GLOBAL              2 (ts)
                      162 LOAD_ATTR                2 (gpt)
-                     172 LOAD_ATTR                6 (HOW_TO_SEARCH_GRATA_API)
+                     172 LOAD_ATTR                6 (HOW_TO_GOOGLE)
          
-         196         182 LOAD_CONST               3 (('role', 'content'))
+         188         182 LOAD_CONST               3 (('role', 'content'))
                      184 BUILD_CONST_KEY_MAP      2
          
-         201         186 LOAD_CONST               2 ('system')
+         193         186 LOAD_CONST               2 ('system')
+         
+         194         188 LOAD_GLOBAL              2 (ts)
+                     200 LOAD_ATTR                2 (gpt)
+                     210 LOAD_ATTR                7 (HOW_TO_GOOGLE_MAPS)
+         
+         192         220 LOAD_CONST               3 (('role', 'content'))
+                     222 BUILD_CONST_KEY_MAP      2
+         
+         197         224 LOAD_CONST               2 ('system')
+         
+         198         226 LOAD_GLOBAL              2 (ts)
+                     238 LOAD_ATTR                2 (gpt)
+                     248 LOAD_ATTR                8 (HOW_TO_SEARCH_GRATA_API)
+         
+         196         258 LOAD_CONST               3 (('role', 'content'))
+                     260 BUILD_CONST_KEY_MAP      2
+         
+         201         262 LOAD_CONST               2 ('system')
+         
+         202         264 LOAD_CONST               4 ('the search_uid is ')
+                     266 LOAD_FAST                0 (event)
+                     268 LOAD_ATTR                9 (search_uid)
+                     278 FORMAT_VALUE             0
+                     280 BUILD_STRING             2
          
-         202         188 LOAD_CONST               4 ('the search_uid is ')
-                     190 LOAD_FAST                0 (event)
-                     192 LOAD_ATTR                7 (search_uid)
-                     202 FORMAT_VALUE             0
-                     204 BUILD_STRING             2
-         
-         200         206 LOAD_CONST               3 (('role', 'content'))
-                     208 BUILD_CONST_KEY_MAP      2
-         
-         205         210 LOAD_CONST               2 ('system')
-         
-         206         212 LOAD_CONST               5 ('the actor_key is ')
-                     214 LOAD_FAST                0 (event)
-                     216 LOAD_ATTR                8 (actor_key)
-                     226 FORMAT_VALUE             0
-                     228 BUILD_STRING             2
-         
-         204         230 LOAD_CONST               3 (('role', 'content'))
-                     232 BUILD_CONST_KEY_MAP      2
-         
-         208         234 LOAD_CONST               6 ('user')
-                     236 LOAD_FAST                0 (event)
-                     238 LOAD_ATTR                9 (data)
-                     248 LOAD_CONST               7 ('prompt')
-                     250 BINARY_SUBSCR
-                     260 LOAD_CONST               3 (('role', 'content'))
-                     262 BUILD_CONST_KEY_MAP      2
-         
-         175         264 BUILD_LIST               7
-                     266 STORE_FAST               1 (messages)
-         
-         210         268 LOAD_GLOBAL              2 (ts)
-                     280 LOAD_ATTR                2 (gpt)
-                     290 LOAD_METHOD             10 (ask_gpt4)
-                     312 LOAD_FAST                1 (messages)
-                     314 PRECALL                  1
-                     318 CALL                     1
-                     328 STORE_FAST               2 (resp)
-         
-         212         330 LOAD_GLOBAL              1 (NULL + print)
-                     342 LOAD_FAST                2 (resp)
-                     344 PRECALL                  1
-                     348 CALL                     1
-                     358 POP_TOP
-         
-         213         360 LOAD_FAST                2 (resp)
-                     362 LOAD_CONST               8 ('events')
-                     364 BINARY_SUBSCR
-                     374 GET_ITER
-                 >>  376 FOR_ITER               116 (to 610)
-                     378 STORE_FAST               3 (new_event)
-         
-         214         380 LOAD_GLOBAL              1 (NULL + print)
-                     392 LOAD_CONST               9 ('new event:')
-                     394 LOAD_FAST                3 (new_event)
-                     396 PRECALL                  2
-                     400 CALL                     2
-                     410 POP_TOP
-         
-         215         412 LOAD_GLOBAL             23 (NULL + from_dict)
-                     424 LOAD_GLOBAL              2 (ts)
-                     436 LOAD_ATTR               12 (models)
-                     446 LOAD_ATTR               13 (Event)
-                     456 LOAD_FAST                3 (new_event)
-                     458 PRECALL                  2
-                     462 CALL                     2
-                     472 STORE_FAST               4 (e)
-         
-         216         474 LOAD_GLOBAL              1 (NULL + print)
-                     486 LOAD_FAST                4 (e)
-                     488 PRECALL                  1
-                     492 CALL                     1
-                     502 POP_TOP
-         
-         217         504 LOAD_FAST                0 (event)
-                     506 LOAD_ATTR                9 (data)
-                     516 LOAD_CONST               7 ('prompt')
-                     518 BINARY_SUBSCR
-                     528 LOAD_FAST                4 (e)
-                     530 LOAD_ATTR                9 (data)
-                     540 LOAD_CONST               7 ('prompt')
-                     542 STORE_SUBSCR
-         
-         218         546 LOAD_GLOBAL              2 (ts)
-                     558 LOAD_ATTR               14 (query)
-                     568 LOAD_METHOD             15 (insert_event)
-                     590 LOAD_FAST                4 (e)
-                     592 PRECALL                  1
-                     596 CALL                     1
-                     606 POP_TOP
-                     608 JUMP_BACKWARD          117 (to 376)
+         200         282 LOAD_CONST               3 (('role', 'content'))
+                     284 BUILD_CONST_KEY_MAP      2
          
-         213     >>  610 LOAD_CONST               0 (None)
-                     612 RETURN_VALUE
+         205         286 LOAD_CONST               2 ('system')
+         
+         206         288 LOAD_CONST               5 ('the actor_key is ')
+                     290 LOAD_FAST                0 (event)
+                     292 LOAD_ATTR               10 (actor_key)
+                     302 FORMAT_VALUE             0
+                     304 BUILD_STRING             2
+         
+         204         306 LOAD_CONST               3 (('role', 'content'))
+                     308 BUILD_CONST_KEY_MAP      2
+         
+         208         310 LOAD_CONST               6 ('user')
+                     312 LOAD_FAST                0 (event)
+                     314 LOAD_ATTR               11 (data)
+                     324 LOAD_CONST               7 ('prompt')
+                     326 BINARY_SUBSCR
+                     336 LOAD_CONST               3 (('role', 'content'))
+                     338 BUILD_CONST_KEY_MAP      2
+         
+         175         340 BUILD_LIST               9
+                     342 STORE_FAST               1 (messages)
+         
+         210         344 LOAD_GLOBAL              2 (ts)
+                     356 LOAD_ATTR                2 (gpt)
+                     366 LOAD_METHOD             12 (ask_gpt4)
+                     388 LOAD_FAST                1 (messages)
+                     390 PRECALL                  1
+                     394 CALL                     1
+                     404 STORE_FAST               2 (resp)
+         
+         212         406 LOAD_GLOBAL              1 (NULL + print)
+                     418 LOAD_FAST                2 (resp)
+                     420 PRECALL                  1
+                     424 CALL                     1
+                     434 POP_TOP
+         
+         213         436 LOAD_FAST                2 (resp)
+                     438 LOAD_CONST               8 ('events')
+                     440 BINARY_SUBSCR
+                     450 GET_ITER
+                 >>  452 FOR_ITER               126 (to 706)
+                     454 STORE_FAST               3 (new_event)
+         
+         214         456 LOAD_GLOBAL              1 (NULL + print)
+                     468 LOAD_CONST               9 ('new event:')
+                     470 LOAD_FAST                3 (new_event)
+                     472 PRECALL                  2
+                     476 CALL                     2
+                     486 POP_TOP
+         
+         215         488 LOAD_FAST                0 (event)
+                     490 LOAD_ATTR                9 (search_uid)
+                     500 LOAD_FAST                3 (new_event)
+                     502 LOAD_CONST              10 ('search_uid')
+                     504 STORE_SUBSCR
+         
+         216         508 LOAD_GLOBAL             27 (NULL + from_dict)
+                     520 LOAD_GLOBAL              2 (ts)
+                     532 LOAD_ATTR               14 (models)
+                     542 LOAD_ATTR               15 (Event)
+                     552 LOAD_FAST                3 (new_event)
+                     554 PRECALL                  2
+                     558 CALL                     2
+                     568 STORE_FAST               4 (e)
+         
+         217         570 LOAD_GLOBAL              1 (NULL + print)
+                     582 LOAD_FAST                4 (e)
+                     584 PRECALL                  1
+                     588 CALL                     1
+                     598 POP_TOP
+         
+         219         600 LOAD_FAST                0 (event)
+                     602 LOAD_ATTR               11 (data)
+                     612 LOAD_CONST               7 ('prompt')
+                     614 BINARY_SUBSCR
+                     624 LOAD_FAST                4 (e)
+                     626 LOAD_ATTR               11 (data)
+                     636 LOAD_CONST               7 ('prompt')
+                     638 STORE_SUBSCR
+         
+         220         642 LOAD_GLOBAL              2 (ts)
+                     654 LOAD_ATTR               16 (query)
+                     664 LOAD_METHOD             17 (insert_event)
+                     686 LOAD_FAST                4 (e)
+                     688 PRECALL                  1
+                     692 CALL                     1
+                     702 POP_TOP
+                     704 JUMP_BACKWARD          127 (to 452)
+         
+         213     >>  706 LOAD_CONST               0 (None)
+                     708 RETURN_VALUE
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
-         names      ('print', 'ts', 'gpt', 'HOW_TO_RESPOND', 'HOW_TO_IMPORT', 'HOW_TO_TRANSITION', 'HOW_TO_SEARCH_GRATA_API', 'search_uid', 'actor_key', 'data', 'ask_gpt4', 'from_dict', 'models', 'Event', 'query', 'insert_event')
+            'search_uid'
+         names      ('print', 'ts', 'gpt', 'HOW_TO_RESPOND', 'HOW_TO_IMPORT', 'HOW_TO_TRANSITION', 'HOW_TO_GOOGLE', 'HOW_TO_GOOGLE_MAPS', 'HOW_TO_SEARCH_GRATA_API', 'search_uid', 'actor_key', 'data', 'ask_gpt4', 'from_dict', 'models', 'Event', 'query', 'insert_event')
          varnames   ('event', 'messages', 'resp', 'new_event', 'e')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'handle_prompt'
          firstlineno 173
          lnotab
-            0x02012003020120fe0405020120fe0405020120fe040d020120fe040502
-            0112fe0405020112fe04041edf04233e021e01140120013e011e012a0140
-            fb
+            0x02012003020120fe0405020120fe0405020120fe0405020120fe040502
+            0120fe0405020120fe0405020112fe0405020112fe04041edf04233e021e
+            011401200114013e011e022a0140f9
       'company'
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -1259,165 +1287,165 @@
             00000000007c055f040000000000000000741d0000000000000000000074
             1f00000000000000000000a6000000ab000000000000000000a6010000ab
             0100000000000000007c056a100000000000000000640b3c000000740100
             0000000000000000007c05a6010000ab0100000000000000000100740200
             0000000000000000006a110000000000000000a012000000000000000000
             00000000000000000000007c05a6010000ab01000000000000000001007c
             045300
-         221           0 RESUME                   0
+         223           0 RESUME                   0
          
-         222           2 LOAD_GLOBAL              1 (NULL + print)
+         224           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('enriching with gpt...')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-         223          32 NOP
+         225          32 NOP
          
-         224          34 LOAD_GLOBAL              2 (ts)
+         226          34 LOAD_GLOBAL              2 (ts)
                       46 LOAD_ATTR                2 (helpers)
                       56 LOAD_METHOD              3 (get_homepage_text)
                       78 LOAD_FAST                0 (company)
                       80 LOAD_ATTR                4 (domain)
                       90 PRECALL                  1
                       94 CALL                     1
                      104 STORE_FAST               1 (homepage_text)
                      106 JUMP_FORWARD            40 (to 188)
                  >>  108 PUSH_EXC_INFO
          
-         225         110 LOAD_GLOBAL             10 (Exception)
+         227         110 LOAD_GLOBAL             10 (Exception)
                      122 CHECK_EXC_MATCH
                      124 POP_JUMP_FORWARD_IF_FALSE    27 (to 180)
                      126 STORE_FAST               2 (e)
          
-         226         128 LOAD_GLOBAL              1 (NULL + print)
+         228         128 LOAD_GLOBAL              1 (NULL + print)
                      140 LOAD_FAST                2 (e)
                      142 PRECALL                  1
                      146 CALL                     1
                      156 POP_TOP
          
-         227         158 LOAD_CONST               2 ('<could not fetch homepage>')
+         229         158 LOAD_CONST               2 ('<could not fetch homepage>')
                      160 STORE_FAST               1 (homepage_text)
                      162 POP_EXCEPT
                      164 LOAD_CONST               0 (None)
                      166 STORE_FAST               2 (e)
                      168 DELETE_FAST              2 (e)
                      170 JUMP_FORWARD             8 (to 188)
                  >>  172 LOAD_CONST               0 (None)
                      174 STORE_FAST               2 (e)
                      176 DELETE_FAST              2 (e)
                      178 RERAISE                  1
          
-         225     >>  180 RERAISE                  0
+         227     >>  180 RERAISE                  0
                  >>  182 COPY                     3
                      184 POP_EXCEPT
                      186 RERAISE                  1
          
-         230     >>  188 LOAD_CONST               3 ('system')
+         232     >>  188 LOAD_CONST               3 ('system')
          
-         231         190 LOAD_CONST               4 ('You will help us evaluate ')
+         233         190 LOAD_CONST               4 ('You will help us evaluate ')
                      192 LOAD_FAST                0 (company)
                      194 LOAD_ATTR                6 (name)
                      204 FORMAT_VALUE             0
                      206 LOAD_CONST               5 (' for acquisition.')
                      208 BUILD_STRING             3
          
-         229         210 LOAD_CONST               6 (('role', 'content'))
+         231         210 LOAD_CONST               6 (('role', 'content'))
                      212 BUILD_CONST_KEY_MAP      2
          
-         234         214 LOAD_CONST               3 ('system')
+         236         214 LOAD_CONST               3 ('system')
          
-         235         216 LOAD_CONST               7 ('You will consider this existing information: ')
+         237         216 LOAD_CONST               7 ('You will consider this existing information: ')
                      218 LOAD_GLOBAL             15 (NULL + asdict)
                      230 LOAD_FAST                0 (company)
                      232 PRECALL                  1
                      236 CALL                     1
                      246 FORMAT_VALUE             0
                      248 BUILD_STRING             2
          
-         233         250 LOAD_CONST               6 (('role', 'content'))
+         235         250 LOAD_CONST               6 (('role', 'content'))
                      252 BUILD_CONST_KEY_MAP      2
          
-         238         254 LOAD_CONST               3 ('system')
+         240         254 LOAD_CONST               3 ('system')
          
-         239         256 LOAD_CONST               8 ('You will consider this copy from the company homepage as the most up to date. homepage_text: ')
+         241         256 LOAD_CONST               8 ('You will consider this copy from the company homepage as the most up to date. homepage_text: ')
                      258 LOAD_FAST                1 (homepage_text)
                      260 FORMAT_VALUE             0
                      262 BUILD_STRING             2
          
-         237         264 LOAD_CONST               6 (('role', 'content'))
+         239         264 LOAD_CONST               6 (('role', 'content'))
                      266 BUILD_CONST_KEY_MAP      2
          
-         242         268 LOAD_CONST               3 ('system')
+         244         268 LOAD_CONST               3 ('system')
          
-         243         270 LOAD_CONST               9 ('You will respond with only the JSON object.')
+         245         270 LOAD_CONST               9 ('You will respond with only the JSON object.')
          
-         241         272 LOAD_CONST               6 (('role', 'content'))
+         243         272 LOAD_CONST               6 (('role', 'content'))
                      274 BUILD_CONST_KEY_MAP      2
          
-         246         276 LOAD_CONST              10 ('user')
+         248         276 LOAD_CONST              10 ('user')
          
-         247         278 LOAD_GLOBAL              2 (ts)
+         249         278 LOAD_GLOBAL              2 (ts)
                      290 LOAD_ATTR                8 (gpt)
                      300 LOAD_ATTR                9 (HOW_TO_ENRICH)
          
-         245         310 LOAD_CONST               6 (('role', 'content'))
+         247         310 LOAD_CONST               6 (('role', 'content'))
                      312 BUILD_CONST_KEY_MAP      2
          
-         228         314 BUILD_LIST               5
+         230         314 BUILD_LIST               5
                      316 STORE_FAST               3 (messages)
          
-         251         318 LOAD_GLOBAL              2 (ts)
+         253         318 LOAD_GLOBAL              2 (ts)
                      330 LOAD_ATTR                8 (gpt)
                      340 LOAD_METHOD             10 (ask_gpt4)
                      362 LOAD_FAST                3 (messages)
                      364 PRECALL                  1
                      368 CALL                     1
                      378 STORE_FAST               4 (resp)
          
-         252         380 LOAD_GLOBAL             23 (NULL + from_dict)
+         254         380 LOAD_GLOBAL             23 (NULL + from_dict)
                      392 LOAD_GLOBAL              2 (ts)
                      404 LOAD_ATTR               12 (models)
                      414 LOAD_ATTR               13 (Event)
                      424 LOAD_FAST                4 (resp)
                      426 PRECALL                  2
                      430 CALL                     2
                      440 STORE_FAST               5 (update_event)
          
-         253         442 LOAD_FAST                0 (company)
+         255         442 LOAD_FAST                0 (company)
                      444 LOAD_ATTR                4 (domain)
                      454 LOAD_FAST                5 (update_event)
                      456 STORE_ATTR               4 (domain)
          
-         254         466 LOAD_GLOBAL             29 (NULL + int)
+         256         466 LOAD_GLOBAL             29 (NULL + int)
                      478 LOAD_GLOBAL             31 (NULL + time)
                      490 PRECALL                  0
                      494 CALL                     0
                      504 PRECALL                  1
                      508 CALL                     1
                      518 LOAD_FAST                5 (update_event)
                      520 LOAD_ATTR               16 (data)
                      530 LOAD_CONST              11 ('gpt')
                      532 STORE_SUBSCR
          
-         255         536 LOAD_GLOBAL              1 (NULL + print)
+         257         536 LOAD_GLOBAL              1 (NULL + print)
                      548 LOAD_FAST                5 (update_event)
                      550 PRECALL                  1
                      554 CALL                     1
                      564 POP_TOP
          
-         256         566 LOAD_GLOBAL              2 (ts)
+         258         566 LOAD_GLOBAL              2 (ts)
                      578 LOAD_ATTR               17 (query)
                      588 LOAD_METHOD             18 (insert_event)
                      610 LOAD_FAST                5 (update_event)
                      612 PRECALL                  1
                      616 CALL                     1
                      626 POP_TOP
          
-         257         628 LOAD_FAST                4 (resp)
+         259         628 LOAD_FAST                4 (resp)
                      630 RETURN_VALUE
          ExceptionTable:
            34 to 104 -> 108 [0]
            108 to 126 -> 182 [1] lasti
            128 to 160 -> 172 [1] lasti
            172 to 180 -> 182 [1] lasti
          consts
@@ -1435,15 +1463,15 @@
             'gpt'
          names      ('print', 'ts', 'helpers', 'get_homepage_text', 'domain', 'Exception', 'name', 'asdict', 'gpt', 'HOW_TO_ENRICH', 'ask_gpt4', 'from_dict', 'models', 'Event', 'int', 'time', 'data', 'query', 'insert_event')
          varnames   ('company', 'homepage_text', 'e', 'messages', 'resp', 'update_event')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'enrich_with_gpt'
-         firstlineno 221
+         firstlineno 223
          lnotab
             0x02011e0102014c0112011e0116fe0805020114fe0405020122fe040502
             0108fe0405020102fe0405020120fe04ef04173e013e01180146011e013e
             01
       code
          argcount  : 1
          nlocals   : 4
@@ -1465,105 +1493,105 @@
             00000000000000a5017c03a5017c025f0400000000000000007402000000
             000000000000006a020000000000000000a00b0000000000000000000000
             0000000000000000007c02a6010000ab01000000000000000001007c026a
             040000000000000000a00500000000000000000000000000000000000000
             006405a6010000ab0100000000000000007211740d000000000000000000
             006406a6010000ab01000000000000000001006400530074190000000000
             00000000007c02ac07a6010000ab010000000000000000010064005300
-         260           0 RESUME                   0
+         262           0 RESUME                   0
          
-         261           2 LOAD_FAST                0 (event)
+         263           2 LOAD_FAST                0 (event)
                        4 LOAD_ATTR                0 (domain)
                       14 STORE_FAST               1 (domain)
          
-         263          16 LOAD_GLOBAL              2 (ts)
+         265          16 LOAD_GLOBAL              2 (ts)
                       28 LOAD_ATTR                2 (query)
                       38 LOAD_METHOD              3 (find_company_by_domain)
                       60 LOAD_FAST                1 (domain)
                       62 PRECALL                  1
                       66 CALL                     1
                       76 STORE_FAST               2 (company)
          
-         264          78 LOAD_FAST                2 (company)
+         266          78 LOAD_FAST                2 (company)
                       80 LOAD_ATTR                4 (meta)
                       90 LOAD_METHOD              5 (get)
                      112 LOAD_CONST               1 ('company_uid')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_JUMP_FORWARD_IF_FALSE    16 (to 162)
          
-         265         130 LOAD_GLOBAL             13 (NULL + print)
+         267         130 LOAD_GLOBAL             13 (NULL + print)
                      142 LOAD_CONST               2 ('company already exists. skipping enrichment...')
                      144 PRECALL                  1
                      148 CALL                     1
                      158 POP_TOP
                      160 JUMP_FORWARD           142 (to 446)
          
-         267     >>  162 LOAD_GLOBAL              2 (ts)
+         269     >>  162 LOAD_GLOBAL              2 (ts)
                      174 LOAD_ATTR                7 (grata)
                      184 LOAD_METHOD              8 (enrich)
                      206 LOAD_FAST                2 (company)
                      208 LOAD_ATTR                0 (domain)
                      218 PRECALL                  1
                      222 CALL                     1
                      232 STORE_FAST               3 (resp)
          
-         268         234 LOAD_FAST                2 (company)
+         270         234 LOAD_FAST                2 (company)
                      236 LOAD_ATTR                9 (name)
                      246 JUMP_IF_TRUE_OR_POP     20 (to 288)
                      248 LOAD_FAST                3 (resp)
                      250 LOAD_METHOD              5 (get)
                      272 LOAD_CONST               3 ('name')
                      274 PRECALL                  1
                      278 CALL                     1
                  >>  288 LOAD_FAST                2 (company)
                      290 STORE_ATTR               9 (name)
          
-         269         300 LOAD_FAST                3 (resp)
+         271         300 LOAD_FAST                3 (resp)
                      302 LOAD_METHOD              5 (get)
                      324 LOAD_CONST               4 ('description')
                      326 PRECALL                  1
                      330 CALL                     1
                      340 LOAD_FAST                2 (company)
                      342 STORE_ATTR              10 (description)
          
-         270         352 BUILD_MAP                0
+         272         352 BUILD_MAP                0
                      354 LOAD_FAST                2 (company)
                      356 LOAD_ATTR                4 (meta)
                      366 DICT_UPDATE              1
                      368 LOAD_FAST                3 (resp)
                      370 DICT_UPDATE              1
                      372 LOAD_FAST                2 (company)
                      374 STORE_ATTR               4 (meta)
          
-         271         384 LOAD_GLOBAL              2 (ts)
+         273         384 LOAD_GLOBAL              2 (ts)
                      396 LOAD_ATTR                2 (query)
                      406 LOAD_METHOD             11 (update_company)
                      428 LOAD_FAST                2 (company)
                      430 PRECALL                  1
                      434 CALL                     1
                      444 POP_TOP
          
-         273     >>  446 LOAD_FAST                2 (company)
+         275     >>  446 LOAD_FAST                2 (company)
                      448 LOAD_ATTR                4 (meta)
                      458 LOAD_METHOD              5 (get)
                      480 LOAD_CONST               5 ('gpt_description')
                      482 PRECALL                  1
                      486 CALL                     1
                      496 POP_JUMP_FORWARD_IF_FALSE    17 (to 532)
          
-         274         498 LOAD_GLOBAL             13 (NULL + print)
+         276         498 LOAD_GLOBAL             13 (NULL + print)
                      510 LOAD_CONST               6 ('company already enriched with gpt. skipping...')
                      512 PRECALL                  1
                      516 CALL                     1
                      526 POP_TOP
                      528 LOAD_CONST               0 (None)
                      530 RETURN_VALUE
          
-         276     >>  532 LOAD_GLOBAL             25 (NULL + enrich_with_gpt)
+         278     >>  532 LOAD_GLOBAL             25 (NULL + enrich_with_gpt)
                      544 LOAD_FAST                2 (company)
                      546 KW_NAMES                 7
                      548 PRECALL                  1
                      552 CALL                     1
                      562 POP_TOP
                      564 LOAD_CONST               0 (None)
                      566 RETURN_VALUE
@@ -1578,20 +1606,20 @@
             ('company',)
          names      ('domain', 'ts', 'query', 'find_company_by_domain', 'meta', 'get', 'print', 'grata', 'enrich', 'name', 'description', 'update_company', 'enrich_with_gpt')
          varnames   ('event', 'domain', 'company', 'resp')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_enrichment'
-         firstlineno 260
+         firstlineno 262
          lnotab 0x02010e023e013401200248014201340120013e0234012202
       'event_id'
       code
          argcount  : 1
-         nlocals   : 7
+         nlocals   : 9
          stacksize : 9
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             0001007402000000000000000000006a020000000000000000a003000000
             00000000000000000000000000000000007c00a6010000ab010000000000
             0000007d0174010000000000000000000064027c00a6020000ab02000000
@@ -1631,655 +1659,700 @@
             166b02000000007213741b000000000000000000007c027c01ac15a60200
             00ab0200000000000000000100640053007c016a07000000000000000064
             176b02000000007213741b000000000000000000007c027c01ac15a60200
             00ab0200000000000000000100640053007c016a07000000000000000064
             186b020000000072227402000000000000000000006a0200000000000000
             00a00e00000000000000000000000000000000000000007c01ac05a60100
             00ab0100000000000000000100640053007c016a07000000000000000064
-            196b02000000007236740100000000000000000000641aa6010000ab0100
-            0000000000000001007402000000000000000000006a0200000000000000
-            00a00f00000000000000000000000000000000000000007c026a10000000
-            0000000000ac1ba6010000ab0100000000000000000100640053007c016a
-            070000000000000000641c6b02000000009001721f740100000000000000
-            0000007c01a6010000ab01000000000000000001007c016a110000000000
-            000000641c190000000000000000007d047c016a11000000000000000064
-            1d190000000000000000007d057c04641e6b0200000000724c7402000000
-            000000000000006a020000000000000000a0120000000000000000000000
-            0000000000000000007402000000000000000000006a1300000000000000
-            00a01400000000000000000000000000000000000000007c026a10000000
-            0000000000640e7c037c016a150000000000000000ac1fa6040000ab0400
-            00000000000000a6010000ab0100000000000000000100640053007c0464
-            206b0200000000724c7402000000000000000000006a0200000000000000
-            00a012000000000000000000000000000000000000000074020000000000
-            00000000006a130000000000000000a01400000000000000000000000000
-            000000000000007c026a10000000000000000064217c037c016a15000000
-            0000000000ac1fa6040000ab040000000000000000a6010000ab01000000
-            00000000000100640053007c0564227600724c7402000000000000000000
-            006a020000000000000000a0120000000000000000000000000000000000
-            0000007402000000000000000000006a130000000000000000a014000000
-            00000000000000000000000000000000007c026a10000000000000000064
-            097c037c016a150000000000000000ac1fa6040000ab0400000000000000
-            00a6010000ab010000000000000000010064005300640053007c016a0700
-            0000000000000064236b020000000072b97c037281740200000000000000
-            0000006a020000000000000000a016000000000000000000000000000000
-            00000000007c03a6010000ab0100000000000000007d067c016a11000000
-            0000000000a01700000000000000000000000000000000000000006424a6
-            010000ab01000000000000000072127c016a110000000000000000642419
-            0000000000000000007c065f18000000000000000069007c066a19000000
-            0000000000a5017c016a110000000000000000a5017c065f190000000000
-            0000007402000000000000000000006a020000000000000000a01a000000
-            00000000000000000000000000000000007c06a6010000ab010000000000
-            00000001006400530069007c026a190000000000000000a5017c016a1100
-            00000000000000a5017c025f190000000000000000740200000000000000
-            0000006a020000000000000000a01b000000000000000000000000000000
-            00000000007c02a6010000ab0100000000000000000100640053007c016a
-            07000000000000000064256b020000000072757c016a1100000000000000
-            0064261900000000000000000044005d697d037401000000000000000000
-            0064277c03a6020000ab0200000000000000000100740200000000000000
-            0000006a020000000000000000a012000000000000000000000000000000
-            00000000007402000000000000000000006a130000000000000000a01400
-            000000000000000000000000000000000000007c026a1000000000000000
-            007c037c016a1100000000000000006428190000000000000000007c016a
-            150000000000000000ac29a6040000ab040000000000000000a6010000ab
-            01000000000000000001008c686400530064005300
-         279           0 RESUME                   0
+            196b020000000072537c016a0f0000000000000000641a19000000000000
+            00000044005d437d047402000000000000000000006a0200000000000000
+            00a01000000000000000000000000000000000000000007c04ac1ba60100
+            00ab0100000000000000007d057402000000000000000000006a02000000
+            0000000000a01100000000000000000000000000000000000000007c057c
+            02ac1ca6020000ab02000000000000000001008c44640053007c016a0700
+            00000000000000641d6b0200000000723674010000000000000000000064
+            1ea6010000ab01000000000000000001007402000000000000000000006a
+            020000000000000000a01200000000000000000000000000000000000000
+            007c026a130000000000000000ac1fa6010000ab01000000000000000001
+            00640053007c016a07000000000000000064206b02000000009001721f74
+            01000000000000000000007c01a6010000ab01000000000000000001007c
+            016a0f00000000000000006420190000000000000000007d067c016a0f00
+            000000000000006421190000000000000000007d077c0664226b02000000
+            00724c7402000000000000000000006a020000000000000000a014000000
+            00000000000000000000000000000000007402000000000000000000006a
+            150000000000000000a01600000000000000000000000000000000000000
+            007c026a130000000000000000640e7c037c016a170000000000000000ac
+            23a6040000ab040000000000000000a6010000ab01000000000000000001
+            00640053007c0664246b0200000000724c7402000000000000000000006a
+            020000000000000000a01400000000000000000000000000000000000000
+            007402000000000000000000006a150000000000000000a0160000000000
+            0000000000000000000000000000007c026a13000000000000000064257c
+            037c016a170000000000000000ac23a6040000ab040000000000000000a6
+            010000ab0100000000000000000100640053007c0764267600724c740200
+            0000000000000000006a020000000000000000a014000000000000000000
+            00000000000000000000007402000000000000000000006a150000000000
+            000000a01600000000000000000000000000000000000000007c026a1300
+            0000000000000064097c037c016a170000000000000000ac23a6040000ab
+            040000000000000000a6010000ab01000000000000000001006400530064
+            0053007c016a07000000000000000064276b020000000072b97c03728174
+            02000000000000000000006a020000000000000000a01800000000000000
+            000000000000000000000000007c03a6010000ab0100000000000000007d
+            087c016a0f0000000000000000a019000000000000000000000000000000
+            00000000006428a6010000ab01000000000000000072127c016a0f000000
+            00000000006428190000000000000000007c085f1a000000000000000069
+            007c086a1b0000000000000000a5017c016a0f0000000000000000a5017c
+            085f1b00000000000000007402000000000000000000006a020000000000
+            000000a01c00000000000000000000000000000000000000007c08a60100
+            00ab01000000000000000001006400530069007c026a1b00000000000000
+            00a5017c016a0f0000000000000000a5017c025f1b000000000000000074
+            02000000000000000000006a020000000000000000a01d00000000000000
+            000000000000000000000000007c02a6010000ab01000000000000000001
+            00640053007c016a07000000000000000064296b020000000072757c016a
+            0f0000000000000000642a1900000000000000000044005d697d03740100
+            000000000000000000642b7c03a6020000ab020000000000000000010074
+            02000000000000000000006a020000000000000000a01400000000000000
+            000000000000000000000000007402000000000000000000006a15000000
+            0000000000a01600000000000000000000000000000000000000007c026a
+            1300000000000000007c037c016a0f0000000000000000642c1900000000
+            00000000007c016a170000000000000000ac2da6040000ab040000000000
+            000000a6010000ab01000000000000000001008c686400530064005300
+         281           0 RESUME                   0
          
-         280           2 LOAD_GLOBAL              1 (NULL + print)
+         282           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('processing event...')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-         281          32 LOAD_GLOBAL              2 (ts)
+         283          32 LOAD_GLOBAL              2 (ts)
                       44 LOAD_ATTR                2 (query)
                       54 LOAD_METHOD              3 (find_event_by_id)
                       76 LOAD_FAST                0 (event_id)
                       78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               1 (event)
          
-         282          94 LOAD_GLOBAL              1 (NULL + print)
+         284          94 LOAD_GLOBAL              1 (NULL + print)
                      106 LOAD_CONST               2 ('event_id')
                      108 LOAD_FAST                0 (event_id)
                      110 PRECALL                  2
                      114 CALL                     2
                      124 POP_TOP
          
-         283         126 LOAD_GLOBAL              1 (NULL + print)
+         285         126 LOAD_GLOBAL              1 (NULL + print)
                      138 LOAD_FAST                1 (event)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 POP_TOP
          
-         284         156 LOAD_GLOBAL              2 (ts)
+         286         156 LOAD_GLOBAL              2 (ts)
                      168 LOAD_ATTR                2 (query)
                      178 LOAD_METHOD              4 (find_search)
                      200 LOAD_FAST                1 (event)
                      202 LOAD_ATTR                5 (search_uid)
                      212 KW_NAMES                 3
                      214 PRECALL                  1
                      218 CALL                     1
                      228 STORE_FAST               2 (search)
          
-         285         230 LOAD_FAST                1 (event)
+         287         230 LOAD_FAST                1 (event)
                      232 LOAD_ATTR                6 (domain)
                      242 STORE_FAST               3 (domain)
          
-         286         244 LOAD_FAST                1 (event)
+         288         244 LOAD_FAST                1 (event)
                      246 LOAD_ATTR                7 (type)
                      256 LOAD_CONST               4 ('land')
                      258 COMPARE_OP               2 (==)
                      264 POP_JUMP_FORWARD_IF_FALSE    18 (to 302)
          
-         287         266 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         289         266 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      278 LOAD_FAST                1 (event)
                      280 KW_NAMES                 5
                      282 PRECALL                  1
                      286 CALL                     1
                      296 POP_TOP
                      298 LOAD_CONST               0 (None)
                      300 RETURN_VALUE
          
-         288     >>  302 LOAD_FAST                1 (event)
+         290     >>  302 LOAD_FAST                1 (event)
                      304 LOAD_ATTR                7 (type)
                      314 LOAD_CONST               6 ('create')
                      316 COMPARE_OP               2 (==)
                      322 POP_JUMP_FORWARD_IF_FALSE    18 (to 360)
          
-         289         324 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         291         324 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      336 LOAD_FAST                1 (event)
                      338 KW_NAMES                 5
                      340 PRECALL                  1
                      344 CALL                     1
                      354 POP_TOP
                      356 LOAD_CONST               0 (None)
                      358 RETURN_VALUE
          
-         290     >>  360 LOAD_FAST                1 (event)
+         292     >>  360 LOAD_FAST                1 (event)
                      362 LOAD_ATTR                7 (type)
                      372 LOAD_CONST               7 ('similar')
                      374 COMPARE_OP               2 (==)
                      380 POP_JUMP_FORWARD_IF_FALSE    18 (to 418)
          
-         291         382 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         293         382 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      394 LOAD_FAST                1 (event)
                      396 KW_NAMES                 5
                      398 PRECALL                  1
                      402 CALL                     1
                      412 POP_TOP
                      414 LOAD_CONST               0 (None)
                      416 RETURN_VALUE
          
-         292     >>  418 LOAD_FAST                1 (event)
+         294     >>  418 LOAD_FAST                1 (event)
                      420 LOAD_ATTR                7 (type)
                      430 LOAD_CONST               8 ('advance')
                      432 COMPARE_OP               2 (==)
                      438 POP_JUMP_FORWARD_IF_FALSE    18 (to 476)
          
-         293         440 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         295         440 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      452 LOAD_FAST                1 (event)
                      454 KW_NAMES                 5
                      456 PRECALL                  1
                      460 CALL                     1
                      470 POP_TOP
                      472 LOAD_CONST               0 (None)
                      474 RETURN_VALUE
          
-         294     >>  476 LOAD_FAST                1 (event)
+         296     >>  476 LOAD_FAST                1 (event)
                      478 LOAD_ATTR                7 (type)
                      488 LOAD_CONST               9 ('validate')
                      490 COMPARE_OP               2 (==)
                      496 POP_JUMP_FORWARD_IF_FALSE    51 (to 600)
          
-         295         498 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         297         498 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      510 LOAD_FAST                1 (event)
                      512 KW_NAMES                 5
                      514 PRECALL                  1
                      518 CALL                     1
                      528 POP_TOP
          
-         296         530 LOAD_GLOBAL             19 (NULL + run_acquired_check)
+         298         530 LOAD_GLOBAL             19 (NULL + run_acquired_check)
                      542 LOAD_FAST                3 (domain)
                      544 KW_NAMES                10
                      546 PRECALL                  1
                      550 CALL                     1
                      560 POP_TOP
          
-         297         562 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         299         562 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      574 LOAD_FAST                2 (search)
                      576 LOAD_FAST                3 (domain)
                      578 KW_NAMES                11
                      580 PRECALL                  2
                      584 CALL                     2
                      594 POP_TOP
                      596 LOAD_CONST               0 (None)
                      598 RETURN_VALUE
          
-         298     >>  600 LOAD_FAST                1 (event)
+         300     >>  600 LOAD_FAST                1 (event)
                      602 LOAD_ATTR                7 (type)
                      612 LOAD_CONST              12 ('send')
                      614 COMPARE_OP               2 (==)
                      620 POP_JUMP_FORWARD_IF_FALSE    18 (to 658)
          
-         299         622 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         301         622 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      634 LOAD_FAST                1 (event)
                      636 KW_NAMES                 5
                      638 PRECALL                  1
                      642 CALL                     1
                      652 POP_TOP
                      654 LOAD_CONST               0 (None)
                      656 RETURN_VALUE
          
-         300     >>  658 LOAD_FAST                1 (event)
+         302     >>  658 LOAD_FAST                1 (event)
                      660 LOAD_ATTR                7 (type)
                      670 LOAD_CONST              13 ('client_approve')
                      672 COMPARE_OP               2 (==)
                      678 POP_JUMP_FORWARD_IF_FALSE    35 (to 750)
          
-         301         680 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         303         680 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      692 LOAD_FAST                1 (event)
                      694 KW_NAMES                 5
                      696 PRECALL                  1
                      700 CALL                     1
                      710 POP_TOP
          
-         302         712 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         304         712 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      724 LOAD_FAST                2 (search)
                      726 LOAD_FAST                3 (domain)
                      728 KW_NAMES                11
                      730 PRECALL                  2
                      734 CALL                     2
                      744 POP_TOP
                      746 LOAD_CONST               0 (None)
                      748 RETURN_VALUE
          
-         303     >>  750 LOAD_FAST                1 (event)
+         305     >>  750 LOAD_FAST                1 (event)
                      752 LOAD_ATTR                7 (type)
                      762 LOAD_CONST              14 ('reject')
                      764 COMPARE_OP               2 (==)
                      770 POP_JUMP_FORWARD_IF_FALSE     2 (to 776)
          
-         304         772 LOAD_CONST               0 (None)
+         306         772 LOAD_CONST               0 (None)
                      774 RETURN_VALUE
          
-         305     >>  776 LOAD_FAST                1 (event)
+         307     >>  776 LOAD_FAST                1 (event)
                      778 LOAD_ATTR                7 (type)
                      788 LOAD_CONST              15 ('client_reject')
                      790 COMPARE_OP               2 (==)
                      796 POP_JUMP_FORWARD_IF_FALSE     2 (to 802)
          
-         306         798 LOAD_CONST               0 (None)
+         308         798 LOAD_CONST               0 (None)
                      800 RETURN_VALUE
          
-         307     >>  802 LOAD_FAST                1 (event)
+         309     >>  802 LOAD_FAST                1 (event)
                      804 LOAD_ATTR                7 (type)
                      814 LOAD_CONST              16 ('conflict')
                      816 COMPARE_OP               2 (==)
                      822 POP_JUMP_FORWARD_IF_FALSE    35 (to 894)
          
-         308         824 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         310         824 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      836 LOAD_FAST                1 (event)
                      838 KW_NAMES                 5
                      840 PRECALL                  1
                      844 CALL                     1
                      854 POP_TOP
          
-         309         856 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         311         856 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      868 LOAD_FAST                2 (search)
                      870 LOAD_FAST                3 (domain)
                      872 KW_NAMES                11
                      874 PRECALL                  2
                      878 CALL                     2
                      888 POP_TOP
                      890 LOAD_CONST               0 (None)
                      892 RETURN_VALUE
          
-         310     >>  894 LOAD_FAST                1 (event)
+         312     >>  894 LOAD_FAST                1 (event)
                      896 LOAD_ATTR                7 (type)
                      906 LOAD_CONST              17 ('client_conflict')
                      908 COMPARE_OP               2 (==)
                      914 POP_JUMP_FORWARD_IF_FALSE     2 (to 920)
          
-         311         916 LOAD_CONST               0 (None)
+         313         916 LOAD_CONST               0 (None)
                      918 RETURN_VALUE
          
-         313     >>  920 LOAD_FAST                1 (event)
+         315     >>  920 LOAD_FAST                1 (event)
                      922 LOAD_ATTR                7 (type)
                      932 LOAD_CONST              18 ('enrich')
                      934 COMPARE_OP               2 (==)
                      940 POP_JUMP_FORWARD_IF_FALSE    18 (to 978)
          
-         314         942 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         316         942 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      954 LOAD_FAST                1 (event)
                      956 KW_NAMES                 5
                      958 PRECALL                  1
                      962 CALL                     1
                      972 POP_TOP
                      974 LOAD_CONST               0 (None)
                      976 RETURN_VALUE
          
-         316     >>  978 LOAD_FAST                1 (event)
+         318     >>  978 LOAD_FAST                1 (event)
                      980 LOAD_ATTR                7 (type)
                      990 LOAD_CONST              19 ('prompt')
                      992 COMPARE_OP               2 (==)
                      998 POP_JUMP_FORWARD_IF_FALSE    18 (to 1036)
          
-         317        1000 LOAD_GLOBAL             23 (NULL + handle_prompt)
+         319        1000 LOAD_GLOBAL             23 (NULL + handle_prompt)
                     1012 LOAD_FAST                1 (event)
                     1014 KW_NAMES                 5
                     1016 PRECALL                  1
                     1020 CALL                     1
                     1030 POP_TOP
                     1032 LOAD_CONST               0 (None)
                     1034 RETURN_VALUE
          
-         321     >> 1036 LOAD_FAST                1 (event)
+         323     >> 1036 LOAD_FAST                1 (event)
                     1038 LOAD_ATTR                7 (type)
                     1048 LOAD_CONST              20 ('maps')
                     1050 COMPARE_OP               2 (==)
                     1056 POP_JUMP_FORWARD_IF_FALSE    19 (to 1096)
          
-         322        1058 LOAD_GLOBAL             25 (NULL + run_maps_search)
+         324        1058 LOAD_GLOBAL             25 (NULL + run_maps_search)
                     1070 LOAD_FAST                2 (search)
                     1072 LOAD_FAST                1 (event)
                     1074 KW_NAMES                21
                     1076 PRECALL                  2
                     1080 CALL                     2
                     1090 POP_TOP
                     1092 LOAD_CONST               0 (None)
                     1094 RETURN_VALUE
          
-         323     >> 1096 LOAD_FAST                1 (event)
+         325     >> 1096 LOAD_FAST                1 (event)
                     1098 LOAD_ATTR                7 (type)
                     1108 LOAD_CONST              22 ('google')
                     1110 COMPARE_OP               2 (==)
                     1116 POP_JUMP_FORWARD_IF_FALSE    19 (to 1156)
          
-         324        1118 LOAD_GLOBAL             27 (NULL + run_google_search)
+         326        1118 LOAD_GLOBAL             27 (NULL + run_google_search)
                     1130 LOAD_FAST                2 (search)
                     1132 LOAD_FAST                1 (event)
                     1134 KW_NAMES                21
                     1136 PRECALL                  2
                     1140 CALL                     2
                     1150 POP_TOP
                     1152 LOAD_CONST               0 (None)
                     1154 RETURN_VALUE
          
-         326     >> 1156 LOAD_FAST                1 (event)
+         328     >> 1156 LOAD_FAST                1 (event)
                     1158 LOAD_ATTR                7 (type)
                     1168 LOAD_CONST              23 ('grata_search')
                     1170 COMPARE_OP               2 (==)
                     1176 POP_JUMP_FORWARD_IF_FALSE    19 (to 1216)
          
-         327        1178 LOAD_GLOBAL             27 (NULL + run_google_search)
+         329        1178 LOAD_GLOBAL             27 (NULL + run_google_search)
                     1190 LOAD_FAST                2 (search)
                     1192 LOAD_FAST                1 (event)
                     1194 KW_NAMES                21
                     1196 PRECALL                  2
                     1200 CALL                     2
                     1210 POP_TOP
                     1212 LOAD_CONST               0 (None)
                     1214 RETURN_VALUE
          
-         329     >> 1216 LOAD_FAST                1 (event)
+         331     >> 1216 LOAD_FAST                1 (event)
                     1218 LOAD_ATTR                7 (type)
                     1228 LOAD_CONST              24 ('import')
                     1230 COMPARE_OP               2 (==)
                     1236 POP_JUMP_FORWARD_IF_FALSE    34 (to 1306)
          
-         330        1238 LOAD_GLOBAL              2 (ts)
+         332        1238 LOAD_GLOBAL              2 (ts)
                     1250 LOAD_ATTR                2 (query)
                     1260 LOAD_METHOD             14 (important_targets_from_event)
                     1282 LOAD_FAST                1 (event)
                     1284 KW_NAMES                 5
                     1286 PRECALL                  1
                     1290 CALL                     1
                     1300 POP_TOP
                     1302 LOAD_CONST               0 (None)
                     1304 RETURN_VALUE
          
-         332     >> 1306 LOAD_FAST                1 (event)
+         334     >> 1306 LOAD_FAST                1 (event)
                     1308 LOAD_ATTR                7 (type)
-                    1318 LOAD_CONST              25 ('reset')
+                    1318 LOAD_CONST              25 ('import_searches')
                     1320 COMPARE_OP               2 (==)
-                    1326 POP_JUMP_FORWARD_IF_FALSE    54 (to 1436)
+                    1326 POP_JUMP_FORWARD_IF_FALSE    83 (to 1494)
          
-         333        1328 LOAD_GLOBAL              1 (NULL + print)
-                    1340 LOAD_CONST              26 ('💣 Resetting Inbox...')
-                    1342 PRECALL                  1
-                    1346 CALL                     1
-                    1356 POP_TOP
+         335        1328 LOAD_FAST                1 (event)
+                    1330 LOAD_ATTR               15 (data)
+                    1340 LOAD_CONST              26 ('searches')
+                    1342 BINARY_SUBSCR
+                    1352 GET_ITER
+                 >> 1354 FOR_ITER                67 (to 1490)
+                    1356 STORE_FAST               4 (label)
          
-         334        1358 LOAD_GLOBAL              2 (ts)
+         336        1358 LOAD_GLOBAL              2 (ts)
                     1370 LOAD_ATTR                2 (query)
-                    1380 LOAD_METHOD             15 (reset_inbox)
-                    1402 LOAD_FAST                2 (search)
-                    1404 LOAD_ATTR               16 (uid)
-                    1414 KW_NAMES                27
-                    1416 PRECALL                  1
-                    1420 CALL                     1
-                    1430 POP_TOP
-                    1432 LOAD_CONST               0 (None)
-                    1434 RETURN_VALUE
-         
-         336     >> 1436 LOAD_FAST                1 (event)
-                    1438 LOAD_ATTR                7 (type)
-                    1448 LOAD_CONST              28 ('rating')
-                    1450 COMPARE_OP               2 (==)
-                    1456 EXTENDED_ARG             1
-                    1458 POP_JUMP_FORWARD_IF_FALSE   287 (to 2034)
-         
-         338        1460 LOAD_GLOBAL              1 (NULL + print)
-                    1472 LOAD_FAST                1 (event)
-                    1474 PRECALL                  1
-                    1478 CALL                     1
-                    1488 POP_TOP
-         
-         339        1490 LOAD_FAST                1 (event)
-                    1492 LOAD_ATTR               17 (data)
-                    1502 LOAD_CONST              28 ('rating')
-                    1504 BINARY_SUBSCR
-                    1514 STORE_FAST               4 (rating)
-         
-         340        1516 LOAD_FAST                1 (event)
-                    1518 LOAD_ATTR               17 (data)
-                    1528 LOAD_CONST              29 ('currentView')
-                    1530 BINARY_SUBSCR
-                    1540 STORE_FAST               5 (from_stage)
-         
-         341        1542 LOAD_FAST                4 (rating)
-                    1544 LOAD_CONST              30 (1)
-                    1546 COMPARE_OP               2 (==)
-                    1552 POP_JUMP_FORWARD_IF_FALSE    76 (to 1706)
-         
-         342        1554 LOAD_GLOBAL              2 (ts)
-                    1566 LOAD_ATTR                2 (query)
-                    1576 LOAD_METHOD             18 (insert_event)
-         
-         343        1598 LOAD_GLOBAL              2 (ts)
-                    1610 LOAD_ATTR               19 (models)
-                    1620 LOAD_METHOD             20 (Event)
-         
-         344        1642 LOAD_FAST                2 (search)
-                    1644 LOAD_ATTR               16 (uid)
-         
-         345        1654 LOAD_CONST              14 ('reject')
-         
-         346        1656 LOAD_FAST                3 (domain)
-         
-         347        1658 LOAD_FAST                1 (event)
-                    1660 LOAD_ATTR               21 (actor_key)
-         
-         343        1670 KW_NAMES                31
-                    1672 PRECALL                  4
-                    1676 CALL                     4
-         
-         342        1686 PRECALL                  1
-                    1690 CALL                     1
-                    1700 POP_TOP
-                    1702 LOAD_CONST               0 (None)
-                    1704 RETURN_VALUE
-         
-         350     >> 1706 LOAD_FAST                4 (rating)
-                    1708 LOAD_CONST              32 (2)
-                    1710 COMPARE_OP               2 (==)
-                    1716 POP_JUMP_FORWARD_IF_FALSE    76 (to 1870)
-         
-         351        1718 LOAD_GLOBAL              2 (ts)
-                    1730 LOAD_ATTR                2 (query)
-                    1740 LOAD_METHOD             18 (insert_event)
-         
-         352        1762 LOAD_GLOBAL              2 (ts)
-                    1774 LOAD_ATTR               19 (models)
-                    1784 LOAD_METHOD             20 (Event)
-         
-         353        1806 LOAD_FAST                2 (search)
-                    1808 LOAD_ATTR               16 (uid)
-         
-         354        1818 LOAD_CONST              33 ('hold')
-         
-         355        1820 LOAD_FAST                3 (domain)
-         
-         356        1822 LOAD_FAST                1 (event)
-                    1824 LOAD_ATTR               21 (actor_key)
-         
-         352        1834 KW_NAMES                31
-                    1836 PRECALL                  4
-                    1840 CALL                     4
-         
-         351        1850 PRECALL                  1
-                    1854 CALL                     1
-                    1864 POP_TOP
-                    1866 LOAD_CONST               0 (None)
-                    1868 RETURN_VALUE
-         
-         359     >> 1870 LOAD_FAST                5 (from_stage)
-                    1872 LOAD_CONST              34 (('land', 'create', 'advance', 'hold', 'similar'))
-                    1874 CONTAINS_OP              0
-                    1876 POP_JUMP_FORWARD_IF_FALSE    76 (to 2030)
-         
-         360        1878 LOAD_GLOBAL              2 (ts)
-                    1890 LOAD_ATTR                2 (query)
-                    1900 LOAD_METHOD             18 (insert_event)
-         
-         361        1922 LOAD_GLOBAL              2 (ts)
-                    1934 LOAD_ATTR               19 (models)
-                    1944 LOAD_METHOD             20 (Event)
-         
-         362        1966 LOAD_FAST                2 (search)
-                    1968 LOAD_ATTR               16 (uid)
-         
-         363        1978 LOAD_CONST               9 ('validate')
-         
-         364        1980 LOAD_FAST                3 (domain)
-         
-         365        1982 LOAD_FAST                1 (event)
-                    1984 LOAD_ATTR               21 (actor_key)
-         
-         361        1994 KW_NAMES                31
-                    1996 PRECALL                  4
-                    2000 CALL                     4
-         
-         360        2010 PRECALL                  1
-                    2014 CALL                     1
-                    2024 POP_TOP
-                    2026 LOAD_CONST               0 (None)
-                    2028 RETURN_VALUE
-         
-         359     >> 2030 LOAD_CONST               0 (None)
-                    2032 RETURN_VALUE
-         
-         369     >> 2034 LOAD_FAST                1 (event)
-                    2036 LOAD_ATTR                7 (type)
-                    2046 LOAD_CONST              35 ('update')
-                    2048 COMPARE_OP               2 (==)
-                    2054 POP_JUMP_FORWARD_IF_FALSE   185 (to 2426)
-         
-         370        2056 LOAD_FAST                3 (domain)
-                    2058 POP_JUMP_FORWARD_IF_FALSE   129 (to 2318)
-         
-         371        2060 LOAD_GLOBAL              2 (ts)
-                    2072 LOAD_ATTR                2 (query)
-                    2082 LOAD_METHOD             22 (find_company_by_domain)
-                    2104 LOAD_FAST                3 (domain)
-                    2106 PRECALL                  1
-                    2110 CALL                     1
-                    2120 STORE_FAST               6 (company)
-         
-         372        2122 LOAD_FAST                1 (event)
-                    2124 LOAD_ATTR               17 (data)
-                    2134 LOAD_METHOD             23 (get)
-                    2156 LOAD_CONST              36 ('name')
-                    2158 PRECALL                  1
-                    2162 CALL                     1
-                    2172 POP_JUMP_FORWARD_IF_FALSE    18 (to 2210)
-         
-         373        2174 LOAD_FAST                1 (event)
-                    2176 LOAD_ATTR               17 (data)
-                    2186 LOAD_CONST              36 ('name')
-                    2188 BINARY_SUBSCR
-                    2198 LOAD_FAST                6 (company)
-                    2200 STORE_ATTR              24 (name)
-         
-         379     >> 2210 BUILD_MAP                0
-                    2212 LOAD_FAST                6 (company)
-                    2214 LOAD_ATTR               25 (meta)
-                    2224 DICT_UPDATE              1
-                    2226 LOAD_FAST                1 (event)
-                    2228 LOAD_ATTR               17 (data)
-                    2238 DICT_UPDATE              1
-                    2240 LOAD_FAST                6 (company)
-                    2242 STORE_ATTR              25 (meta)
-         
-         380        2252 LOAD_GLOBAL              2 (ts)
-                    2264 LOAD_ATTR                2 (query)
-                    2274 LOAD_METHOD             26 (update_company)
-                    2296 LOAD_FAST                6 (company)
-                    2298 PRECALL                  1
-                    2302 CALL                     1
-                    2312 POP_TOP
-                    2314 LOAD_CONST               0 (None)
-                    2316 RETURN_VALUE
-         
-         382     >> 2318 BUILD_MAP                0
-                    2320 LOAD_FAST                2 (search)
-                    2322 LOAD_ATTR               25 (meta)
-                    2332 DICT_UPDATE              1
-                    2334 LOAD_FAST                1 (event)
-                    2336 LOAD_ATTR               17 (data)
-                    2346 DICT_UPDATE              1
-                    2348 LOAD_FAST                2 (search)
-                    2350 STORE_ATTR              25 (meta)
-         
-         383        2360 LOAD_GLOBAL              2 (ts)
-                    2372 LOAD_ATTR                2 (query)
-                    2382 LOAD_METHOD             27 (update_search)
-                    2404 LOAD_FAST                2 (search)
-                    2406 PRECALL                  1
-                    2410 CALL                     1
-                    2420 POP_TOP
-                    2422 LOAD_CONST               0 (None)
-                    2424 RETURN_VALUE
-         
-         385     >> 2426 LOAD_FAST                1 (event)
-                    2428 LOAD_ATTR                7 (type)
-                    2438 LOAD_CONST              37 ('move')
-                    2440 COMPARE_OP               2 (==)
-                    2446 POP_JUMP_FORWARD_IF_FALSE   117 (to 2682)
-         
-         387        2448 LOAD_FAST                1 (event)
-                    2450 LOAD_ATTR               17 (data)
-                    2460 LOAD_CONST              38 ('domains')
-                    2462 BINARY_SUBSCR
-                    2472 GET_ITER
-                 >> 2474 FOR_ITER               105 (to 2686)
-                    2476 STORE_FAST               3 (domain)
-         
-         388        2478 LOAD_GLOBAL              1 (NULL + print)
-                    2490 LOAD_CONST              39 ('moving domain:')
-                    2492 LOAD_FAST                3 (domain)
-                    2494 PRECALL                  2
-                    2498 CALL                     2
-                    2508 POP_TOP
-         
-         389        2510 LOAD_GLOBAL              2 (ts)
-                    2522 LOAD_ATTR                2 (query)
-                    2532 LOAD_METHOD             18 (insert_event)
-         
-         390        2554 LOAD_GLOBAL              2 (ts)
-                    2566 LOAD_ATTR               19 (models)
-                    2576 LOAD_METHOD             20 (Event)
-         
-         391        2598 LOAD_FAST                2 (search)
-                    2600 LOAD_ATTR               16 (uid)
-         
-         392        2610 LOAD_FAST                3 (domain)
-         
-         393        2612 LOAD_FAST                1 (event)
-                    2614 LOAD_ATTR               17 (data)
-                    2624 LOAD_CONST              40 ('stage')
-                    2626 BINARY_SUBSCR
-         
-         394        2636 LOAD_FAST                1 (event)
-                    2638 LOAD_ATTR               21 (actor_key)
-         
-         390        2648 KW_NAMES                41
-                    2650 PRECALL                  4
-                    2654 CALL                     4
-         
-         389        2664 PRECALL                  1
-                    2668 CALL                     1
-                    2678 POP_TOP
-                    2680 JUMP_BACKWARD          104 (to 2474)
+                    1380 LOAD_METHOD             16 (find_search_by_label)
+                    1402 LOAD_FAST                4 (label)
+                    1404 KW_NAMES                27
+                    1406 PRECALL                  1
+                    1410 CALL                     1
+                    1420 STORE_FAST               5 (from_search)
+         
+         337        1422 LOAD_GLOBAL              2 (ts)
+                    1434 LOAD_ATTR                2 (query)
+                    1444 LOAD_METHOD             17 (important_targets_from_search)
+         
+         338        1466 LOAD_FAST                5 (from_search)
+                    1468 LOAD_FAST                2 (search)
+         
+         337        1470 KW_NAMES                28
+                    1472 PRECALL                  2
+                    1476 CALL                     2
+                    1486 POP_TOP
+                    1488 JUMP_BACKWARD           68 (to 1354)
+         
+         335     >> 1490 LOAD_CONST               0 (None)
+                    1492 RETURN_VALUE
+         
+         341     >> 1494 LOAD_FAST                1 (event)
+                    1496 LOAD_ATTR                7 (type)
+                    1506 LOAD_CONST              29 ('reset')
+                    1508 COMPARE_OP               2 (==)
+                    1514 POP_JUMP_FORWARD_IF_FALSE    54 (to 1624)
+         
+         342        1516 LOAD_GLOBAL              1 (NULL + print)
+                    1528 LOAD_CONST              30 ('💣 Resetting Inbox...')
+                    1530 PRECALL                  1
+                    1534 CALL                     1
+                    1544 POP_TOP
+         
+         343        1546 LOAD_GLOBAL              2 (ts)
+                    1558 LOAD_ATTR                2 (query)
+                    1568 LOAD_METHOD             18 (reset_inbox)
+                    1590 LOAD_FAST                2 (search)
+                    1592 LOAD_ATTR               19 (uid)
+                    1602 KW_NAMES                31
+                    1604 PRECALL                  1
+                    1608 CALL                     1
+                    1618 POP_TOP
+                    1620 LOAD_CONST               0 (None)
+                    1622 RETURN_VALUE
+         
+         345     >> 1624 LOAD_FAST                1 (event)
+                    1626 LOAD_ATTR                7 (type)
+                    1636 LOAD_CONST              32 ('rating')
+                    1638 COMPARE_OP               2 (==)
+                    1644 EXTENDED_ARG             1
+                    1646 POP_JUMP_FORWARD_IF_FALSE   287 (to 2222)
+         
+         347        1648 LOAD_GLOBAL              1 (NULL + print)
+                    1660 LOAD_FAST                1 (event)
+                    1662 PRECALL                  1
+                    1666 CALL                     1
+                    1676 POP_TOP
+         
+         348        1678 LOAD_FAST                1 (event)
+                    1680 LOAD_ATTR               15 (data)
+                    1690 LOAD_CONST              32 ('rating')
+                    1692 BINARY_SUBSCR
+                    1702 STORE_FAST               6 (rating)
+         
+         349        1704 LOAD_FAST                1 (event)
+                    1706 LOAD_ATTR               15 (data)
+                    1716 LOAD_CONST              33 ('currentView')
+                    1718 BINARY_SUBSCR
+                    1728 STORE_FAST               7 (from_stage)
+         
+         350        1730 LOAD_FAST                6 (rating)
+                    1732 LOAD_CONST              34 (1)
+                    1734 COMPARE_OP               2 (==)
+                    1740 POP_JUMP_FORWARD_IF_FALSE    76 (to 1894)
+         
+         351        1742 LOAD_GLOBAL              2 (ts)
+                    1754 LOAD_ATTR                2 (query)
+                    1764 LOAD_METHOD             20 (insert_event)
+         
+         352        1786 LOAD_GLOBAL              2 (ts)
+                    1798 LOAD_ATTR               21 (models)
+                    1808 LOAD_METHOD             22 (Event)
+         
+         353        1830 LOAD_FAST                2 (search)
+                    1832 LOAD_ATTR               19 (uid)
+         
+         354        1842 LOAD_CONST              14 ('reject')
+         
+         355        1844 LOAD_FAST                3 (domain)
+         
+         356        1846 LOAD_FAST                1 (event)
+                    1848 LOAD_ATTR               23 (actor_key)
+         
+         352        1858 KW_NAMES                35
+                    1860 PRECALL                  4
+                    1864 CALL                     4
+         
+         351        1874 PRECALL                  1
+                    1878 CALL                     1
+                    1888 POP_TOP
+                    1890 LOAD_CONST               0 (None)
+                    1892 RETURN_VALUE
+         
+         359     >> 1894 LOAD_FAST                6 (rating)
+                    1896 LOAD_CONST              36 (2)
+                    1898 COMPARE_OP               2 (==)
+                    1904 POP_JUMP_FORWARD_IF_FALSE    76 (to 2058)
+         
+         360        1906 LOAD_GLOBAL              2 (ts)
+                    1918 LOAD_ATTR                2 (query)
+                    1928 LOAD_METHOD             20 (insert_event)
+         
+         361        1950 LOAD_GLOBAL              2 (ts)
+                    1962 LOAD_ATTR               21 (models)
+                    1972 LOAD_METHOD             22 (Event)
+         
+         362        1994 LOAD_FAST                2 (search)
+                    1996 LOAD_ATTR               19 (uid)
+         
+         363        2006 LOAD_CONST              37 ('hold')
+         
+         364        2008 LOAD_FAST                3 (domain)
+         
+         365        2010 LOAD_FAST                1 (event)
+                    2012 LOAD_ATTR               23 (actor_key)
+         
+         361        2022 KW_NAMES                35
+                    2024 PRECALL                  4
+                    2028 CALL                     4
+         
+         360        2038 PRECALL                  1
+                    2042 CALL                     1
+                    2052 POP_TOP
+                    2054 LOAD_CONST               0 (None)
+                    2056 RETURN_VALUE
+         
+         368     >> 2058 LOAD_FAST                7 (from_stage)
+                    2060 LOAD_CONST              38 (('land', 'create', 'advance', 'hold', 'similar'))
+                    2062 CONTAINS_OP              0
+                    2064 POP_JUMP_FORWARD_IF_FALSE    76 (to 2218)
+         
+         369        2066 LOAD_GLOBAL              2 (ts)
+                    2078 LOAD_ATTR                2 (query)
+                    2088 LOAD_METHOD             20 (insert_event)
+         
+         370        2110 LOAD_GLOBAL              2 (ts)
+                    2122 LOAD_ATTR               21 (models)
+                    2132 LOAD_METHOD             22 (Event)
+         
+         371        2154 LOAD_FAST                2 (search)
+                    2156 LOAD_ATTR               19 (uid)
+         
+         372        2166 LOAD_CONST               9 ('validate')
+         
+         373        2168 LOAD_FAST                3 (domain)
+         
+         374        2170 LOAD_FAST                1 (event)
+                    2172 LOAD_ATTR               23 (actor_key)
+         
+         370        2182 KW_NAMES                35
+                    2184 PRECALL                  4
+                    2188 CALL                     4
+         
+         369        2198 PRECALL                  1
+                    2202 CALL                     1
+                    2212 POP_TOP
+                    2214 LOAD_CONST               0 (None)
+                    2216 RETURN_VALUE
+         
+         368     >> 2218 LOAD_CONST               0 (None)
+                    2220 RETURN_VALUE
+         
+         378     >> 2222 LOAD_FAST                1 (event)
+                    2224 LOAD_ATTR                7 (type)
+                    2234 LOAD_CONST              39 ('update')
+                    2236 COMPARE_OP               2 (==)
+                    2242 POP_JUMP_FORWARD_IF_FALSE   185 (to 2614)
+         
+         379        2244 LOAD_FAST                3 (domain)
+                    2246 POP_JUMP_FORWARD_IF_FALSE   129 (to 2506)
+         
+         380        2248 LOAD_GLOBAL              2 (ts)
+                    2260 LOAD_ATTR                2 (query)
+                    2270 LOAD_METHOD             24 (find_company_by_domain)
+                    2292 LOAD_FAST                3 (domain)
+                    2294 PRECALL                  1
+                    2298 CALL                     1
+                    2308 STORE_FAST               8 (company)
+         
+         381        2310 LOAD_FAST                1 (event)
+                    2312 LOAD_ATTR               15 (data)
+                    2322 LOAD_METHOD             25 (get)
+                    2344 LOAD_CONST              40 ('name')
+                    2346 PRECALL                  1
+                    2350 CALL                     1
+                    2360 POP_JUMP_FORWARD_IF_FALSE    18 (to 2398)
+         
+         382        2362 LOAD_FAST                1 (event)
+                    2364 LOAD_ATTR               15 (data)
+                    2374 LOAD_CONST              40 ('name')
+                    2376 BINARY_SUBSCR
+                    2386 LOAD_FAST                8 (company)
+                    2388 STORE_ATTR              26 (name)
+         
+         383     >> 2398 BUILD_MAP                0
+                    2400 LOAD_FAST                8 (company)
+                    2402 LOAD_ATTR               27 (meta)
+                    2412 DICT_UPDATE              1
+                    2414 LOAD_FAST                1 (event)
+                    2416 LOAD_ATTR               15 (data)
+                    2426 DICT_UPDATE              1
+                    2428 LOAD_FAST                8 (company)
+                    2430 STORE_ATTR              27 (meta)
+         
+         384        2440 LOAD_GLOBAL              2 (ts)
+                    2452 LOAD_ATTR                2 (query)
+                    2462 LOAD_METHOD             28 (update_company)
+                    2484 LOAD_FAST                8 (company)
+                    2486 PRECALL                  1
+                    2490 CALL                     1
+                    2500 POP_TOP
+                    2502 LOAD_CONST               0 (None)
+                    2504 RETURN_VALUE
+         
+         386     >> 2506 BUILD_MAP                0
+                    2508 LOAD_FAST                2 (search)
+                    2510 LOAD_ATTR               27 (meta)
+                    2520 DICT_UPDATE              1
+                    2522 LOAD_FAST                1 (event)
+                    2524 LOAD_ATTR               15 (data)
+                    2534 DICT_UPDATE              1
+                    2536 LOAD_FAST                2 (search)
+                    2538 STORE_ATTR              27 (meta)
+         
+         387        2548 LOAD_GLOBAL              2 (ts)
+                    2560 LOAD_ATTR                2 (query)
+                    2570 LOAD_METHOD             29 (update_search)
+                    2592 LOAD_FAST                2 (search)
+                    2594 PRECALL                  1
+                    2598 CALL                     1
+                    2608 POP_TOP
+                    2610 LOAD_CONST               0 (None)
+                    2612 RETURN_VALUE
+         
+         389     >> 2614 LOAD_FAST                1 (event)
+                    2616 LOAD_ATTR                7 (type)
+                    2626 LOAD_CONST              41 ('move')
+                    2628 COMPARE_OP               2 (==)
+                    2634 POP_JUMP_FORWARD_IF_FALSE   117 (to 2870)
+         
+         391        2636 LOAD_FAST                1 (event)
+                    2638 LOAD_ATTR               15 (data)
+                    2648 LOAD_CONST              42 ('domains')
+                    2650 BINARY_SUBSCR
+                    2660 GET_ITER
+                 >> 2662 FOR_ITER               105 (to 2874)
+                    2664 STORE_FAST               3 (domain)
+         
+         392        2666 LOAD_GLOBAL              1 (NULL + print)
+                    2678 LOAD_CONST              43 ('moving domain:')
+                    2680 LOAD_FAST                3 (domain)
+                    2682 PRECALL                  2
+                    2686 CALL                     2
+                    2696 POP_TOP
+         
+         393        2698 LOAD_GLOBAL              2 (ts)
+                    2710 LOAD_ATTR                2 (query)
+                    2720 LOAD_METHOD             20 (insert_event)
+         
+         394        2742 LOAD_GLOBAL              2 (ts)
+                    2754 LOAD_ATTR               21 (models)
+                    2764 LOAD_METHOD             22 (Event)
+         
+         395        2786 LOAD_FAST                2 (search)
+                    2788 LOAD_ATTR               19 (uid)
+         
+         396        2798 LOAD_FAST                3 (domain)
+         
+         397        2800 LOAD_FAST                1 (event)
+                    2802 LOAD_ATTR               15 (data)
+                    2812 LOAD_CONST              44 ('stage')
+                    2814 BINARY_SUBSCR
+         
+         398        2824 LOAD_FAST                1 (event)
+                    2826 LOAD_ATTR               23 (actor_key)
+         
+         394        2836 KW_NAMES                45
+                    2838 PRECALL                  4
+                    2842 CALL                     4
+         
+         393        2852 PRECALL                  1
+                    2856 CALL                     1
+                    2866 POP_TOP
+                    2868 JUMP_BACKWARD          104 (to 2662)
          
-         385     >> 2682 LOAD_CONST               0 (None)
-                    2684 RETURN_VALUE
+         389     >> 2870 LOAD_CONST               0 (None)
+                    2872 RETURN_VALUE
          
-         387     >> 2686 LOAD_CONST               0 (None)
-                    2688 RETURN_VALUE
+         391     >> 2874 LOAD_CONST               0 (None)
+                    2876 RETURN_VALUE
          consts
             None
             'processing event...'
             'event_id'
             ('uid',)
             'land'
             ('event',)
@@ -2298,14 +2371,18 @@
             'enrich'
             'prompt'
             'maps'
             ('search', 'event')
             'google'
             'grata_search'
             'import'
+            'import_searches'
+            'searches'
+            ('label',)
+            ('from_search', 'to_search')
             'reset'
             '💣 Resetting Inbox...'
             ('search_uid',)
             'rating'
             'currentView'
             1
             ('search_uid', 'type', 'domain', 'actor_key')
@@ -2315,32 +2392,33 @@
             'update'
             'name'
             'move'
             'domains'
             'moving domain:'
             'stage'
             ('search_uid', 'domain', 'type', 'actor_key')
-         names      ('print', 'ts', 'query', 'find_event_by_id', 'find_search', 'search_uid', 'domain', 'type', 'run_enrichment', 'run_acquired_check', 'run_similarity_search', 'handle_prompt', 'run_maps_search', 'run_google_search', 'important_targets_from_event', 'reset_inbox', 'uid', 'data', 'insert_event', 'models', 'Event', 'actor_key', 'find_company_by_domain', 'get', 'name', 'meta', 'update_company', 'update_search')
-         varnames   ('event_id', 'event', 'search', 'domain', 'rating', 'from_stage', 'company')
+         names      ('print', 'ts', 'query', 'find_event_by_id', 'find_search', 'search_uid', 'domain', 'type', 'run_enrichment', 'run_acquired_check', 'run_similarity_search', 'handle_prompt', 'run_maps_search', 'run_google_search', 'important_targets_from_event', 'data', 'find_search_by_label', 'important_targets_from_search', 'reset_inbox', 'uid', 'insert_event', 'models', 'Event', 'actor_key', 'find_company_by_domain', 'get', 'name', 'meta', 'update_company', 'update_search')
+         varnames   ('event_id', 'event', 'search', 'domain', 'label', 'from_search', 'rating', 'from_stage', 'company')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'process_event'
-         firstlineno 279
+         firstlineno 281
          lnotab
             0x02011e013e0120011e014a010e01160124011601240116012401160124
             011601200120012601160124011601200126011601040116010401160120
             012601160104021601240216012404160126011601260216012602160144
-            0216011e014e0218021e011a011a010c012c012c010c01020102010cfc10
-            ff14080c012c012c010c01020102010cfc10ff140808012c012c010c0102
-            0102010cfc10ff14ff040a160104013e01340124062a0142022a01420216
-            021e0120012c012c010c01020118010cfc10ff12fc0402
+            0216011e0140012c0104ff14fe040616011e014e0218021e011a011a010c
+            012c012c010c01020102010cfc10ff14080c012c012c010c01020102010c
+            fc10ff140808012c012c010c01020102010cfc10ff14ff040a160104013e
+            01340124012a0142022a01420216021e0120012c012c010c01020118010c
+            fc10ff12fc0402
    names      ('dataclasses', 'asdict', 'time', 'gandai', 'ts', 'requests', 'dacite', 'from_dict', 'secrets', 'str', 'run_acquired_check', 'models', 'Search', 'run_similarity_search', 'Event', 'run_maps_search', 'run_google_search', 'run_gpt_grata_search', 'handle_prompt', 'Company', 'enrich_with_gpt', 'run_enrichment', 'int', 'process_event')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c02080108010c010c030c2628193c2d3c0f3c28243024
+      0x00ff02010c010c02080108010c010c030c2628193c2d3c0f3c28243224
       272413
```

### Comparing `gandai-1.7.56/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa9935666 (Wed May 29 02:32:09 2024 UTC)
-files sz: 29361
+moddate:  0x05a75666 (Wed May 29 03:54:45 2024 UTC)
+files sz: 31209
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 15
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -12,32 +12,35 @@
       0064016c085a09640064016c0a5a0a640064056c0b6d0c5a0c0100640064
       066c0d6d0e5a0e01000200650ea6000000ab000000000000000000010064
       0064016c0f5a10640064076c0f6d115a110100640064086c126d135a1301
       00640064096c146d155a156d165a166d175a176d185a186d195a19010002
       006513a6000000ab0000000000000000005a1a640a6517640b6517660464
       0c84045a1b640d6516640b65106a1c00000000000000006a160000000000
       0000006604640e84045a1d640f6515640b65156604641084045a1e641165
-      19640b65196604641284045a1f640a65106a1c00000000000000006a1700
-      00000000000000640b64016604641384045a200900090009006439641665
-      07650619000000000000000000641765216418652264196523641a652264
-      1b6522640b6401660e641c84055a24640b65096a25000000000000000066
-      02641d84045a26641e84005a27640b65096a250000000000000000660264
-      1f84045a28642084005a29642184005a2a640b65096a2500000000000000
-      006602642284045a2b640b65096a2500000000000000006602642384045a
-      2c641765216602642484045a2d64176521640b65096a2500000000000000
-      006604642584045a2e64176521640b65096a250000000000000000660464
-      2684045a2f64176521640b65096a2500000000000000006604642784045a
-      3064176521640b65096a2500000000000000006604642884045a31642965
-      21640b65106a1c00000000000000006a1900000000000000006604642a84
-      045a32642b6522640b65106a1c00000000000000006a1900000000000000
-      006604642c84045a33642d6522640b65166604642e84045a34642f652264
-      0b65166604643084045a3564316521640b65176604643284045a36640d65
-      16640b64016604643384045a3764116519640b64016604643484045a3864
-      316521640b64016604643584045a3964366521640b64016604643784045a
-      3a64176521640b64016604643884045a3b64015300
+      19640b65196604641284045a1f641365106a1c00000000000000006a1900
+      00000000000000641465106a1c00000000000000006a1900000000000000
+      00640b64016606641584045a20640a65106a1c00000000000000006a1700
+      00000000000000640b64016604641684045a21090009000900643e641965
+      07650619000000000000000000641a6522641b6523641c6524641d652364
+      1e6523640b6401660e641f84055a25640b65096a26000000000000000066
+      02642084045a27642184005a28640b65096a260000000000000000660264
+      2284045a29642384005a2a642484005a2b640b65096a2600000000000000
+      006602642584045a2c640b65096a2600000000000000006602642684045a
+      2d641a65226602642784045a2e641a6522640b65096a2600000000000000
+      006604642884045a2f641a6522640b65096a260000000000000000660464
+      2984045a30641a6522640b65096a2600000000000000006604642a84045a
+      31641a6522640b65096a2600000000000000006604642b84045a32642c65
+      22640b65106a1c00000000000000006a1900000000000000006604642d84
+      045a33642e6523640b65106a1c00000000000000006a1900000000000000
+      006604642f84045a3464306523640b65106a1c00000000000000006a1900
+      000000000000006604643184045a3564326523640b65166604643384045a
+      3664346523640b65166604643584045a3764366522640b65176604643784
+      045a38640d6516640b64016604643884045a3964116519640b6401660464
+      3984045a3a64366522640b64016604643a84045a3b643b6522640b640166
+      04643c84045a3c641a6522640b64016604643d84045a3d64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (hashlib)
                  8 STORE_NAME               0 (hashlib)
    
@@ -173,253 +176,285 @@
                270 LOAD_CONST              11 ('return')
                272 LOAD_NAME               25 (Search)
                274 BUILD_TUPLE              4
                276 LOAD_CONST              18 (<code object insert_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 84>)
                278 MAKE_FUNCTION            4 (annotations)
                280 STORE_NAME              31 (insert_search)
    
-   100         282 LOAD_CONST              10 ('event')
-               284 LOAD_NAME               16 (ts)
+   100         282 LOAD_CONST              19 ('from_search')
+   
+   101         284 LOAD_NAME               16 (ts)
                286 LOAD_ATTR               28 (models)
-               296 LOAD_ATTR               23 (Event)
-               306 LOAD_CONST              11 ('return')
-               308 LOAD_CONST               1 (None)
-               310 BUILD_TUPLE              4
-               312 LOAD_CONST              19 (<code object important_targets_from_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 100>)
-               314 MAKE_FUNCTION            4 (annotations)
-               316 STORE_NAME              32 (important_targets_from_event)
+               296 LOAD_ATTR               25 (Search)
+   
+   100         306 LOAD_CONST              20 ('to_search')
+   
+   101         308 LOAD_NAME               16 (ts)
+               310 LOAD_ATTR               28 (models)
+               320 LOAD_ATTR               25 (Search)
+   
+   100         330 LOAD_CONST              11 ('return')
    
-   176         318 NOP
+   102         332 LOAD_CONST               1 (None)
    
-   177         320 NOP
+   100         334 BUILD_TUPLE              6
+               336 LOAD_CONST              21 (<code object important_targets_from_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 100>)
+               338 MAKE_FUNCTION            4 (annotations)
+               340 STORE_NAME              32 (important_targets_from_search)
    
-   178         322 NOP
+   146         342 LOAD_CONST              10 ('event')
+               344 LOAD_NAME               16 (ts)
+               346 LOAD_ATTR               28 (models)
+               356 LOAD_ATTR               23 (Event)
+               366 LOAD_CONST              11 ('return')
+               368 LOAD_CONST               1 (None)
+               370 BUILD_TUPLE              4
+               372 LOAD_CONST              22 (<code object important_targets_from_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 146>)
+               374 MAKE_FUNCTION            4 (annotations)
+               376 STORE_NAME              33 (important_targets_from_event)
    
-   172         324 LOAD_CONST              57 ((True, None, 'create'))
-               326 LOAD_CONST              22 ('companies')
+   222         378 NOP
    
-   173         328 LOAD_NAME                7 (List)
-               330 LOAD_NAME                6 (Any)
-               332 BINARY_SUBSCR
+   223         380 NOP
    
-   172         342 LOAD_CONST              23 ('search_uid')
+   224         382 NOP
    
-   174         344 LOAD_NAME               33 (int)
+   218         384 LOAD_CONST              62 ((True, None, 'create'))
+               386 LOAD_CONST              25 ('companies')
    
-   172         346 LOAD_CONST              24 ('actor_key')
+   219         388 LOAD_NAME                7 (List)
+               390 LOAD_NAME                6 (Any)
+               392 BINARY_SUBSCR
    
-   175         348 LOAD_NAME               34 (str)
+   218         402 LOAD_CONST              26 ('search_uid')
    
-   172         350 LOAD_CONST              25 ('force')
+   220         404 LOAD_NAME               34 (int)
    
-   176         352 LOAD_NAME               35 (bool)
+   218         406 LOAD_CONST              27 ('actor_key')
    
-   172         354 LOAD_CONST              26 ('source')
+   221         408 LOAD_NAME               35 (str)
    
-   177         356 LOAD_NAME               34 (str)
+   218         410 LOAD_CONST              28 ('force')
    
-   172         358 LOAD_CONST              27 ('stage')
+   222         412 LOAD_NAME               36 (bool)
    
-   178         360 LOAD_NAME               34 (str)
+   218         414 LOAD_CONST              29 ('source')
    
-   172         362 LOAD_CONST              11 ('return')
+   223         416 LOAD_NAME               35 (str)
    
-   179         364 LOAD_CONST               1 (None)
+   218         418 LOAD_CONST              30 ('stage')
    
-   172         366 BUILD_TUPLE             14
-               368 LOAD_CONST              28 (<code object insert_companies_as_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 172>)
-               370 MAKE_FUNCTION            5 (defaults, annotations)
-               372 STORE_NAME              36 (insert_companies_as_targets)
+   224         420 LOAD_NAME               35 (str)
    
-   269         374 LOAD_CONST              11 ('return')
-               376 LOAD_NAME                9 (pd)
-               378 LOAD_ATTR               37 (DataFrame)
-               388 BUILD_TUPLE              2
-               390 LOAD_CONST              29 (<code object searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 269>)
-               392 MAKE_FUNCTION            4 (annotations)
-               394 STORE_NAME              38 (searches_query)
+   218         422 LOAD_CONST              11 ('return')
    
-   301         396 LOAD_CONST              30 (<code object average_rating_per_search_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 301>)
-               398 MAKE_FUNCTION            0
-               400 STORE_NAME              39 (average_rating_per_search_query)
+   225         424 LOAD_CONST               1 (None)
    
-   313         402 LOAD_CONST              11 ('return')
-               404 LOAD_NAME                9 (pd)
-               406 LOAD_ATTR               37 (DataFrame)
-               416 BUILD_TUPLE              2
-               418 LOAD_CONST              31 (<code object validation_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 313>)
-               420 MAKE_FUNCTION            4 (annotations)
-               422 STORE_NAME              40 (validation_history)
+   218         426 BUILD_TUPLE             14
+               428 LOAD_CONST              31 (<code object insert_companies_as_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 218>)
+               430 MAKE_FUNCTION            5 (defaults, annotations)
+               432 STORE_NAME              37 (insert_companies_as_targets)
    
-   356         424 LOAD_CONST              32 (<code object searches_comment_counts, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 356>)
-               426 MAKE_FUNCTION            0
-               428 STORE_NAME              41 (searches_comment_counts)
+   315         434 LOAD_CONST              11 ('return')
+               436 LOAD_NAME                9 (pd)
+               438 LOAD_ATTR               38 (DataFrame)
+               448 BUILD_TUPLE              2
+               450 LOAD_CONST              32 (<code object searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 315>)
+               452 MAKE_FUNCTION            4 (annotations)
+               454 STORE_NAME              39 (searches_query)
    
-   376         430 LOAD_CONST              33 (<code object enriched_searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 376>)
-               432 MAKE_FUNCTION            0
-               434 STORE_NAME              42 (enriched_searches_query)
+   347         456 LOAD_CONST              33 (<code object average_rating_per_search_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 347>)
+               458 MAKE_FUNCTION            0
+               460 STORE_NAME              40 (average_rating_per_search_query)
    
-   396         436 LOAD_CONST              11 ('return')
-               438 LOAD_NAME                9 (pd)
-               440 LOAD_ATTR               37 (DataFrame)
-               450 BUILD_TUPLE              2
-               452 LOAD_CONST              34 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 396>)
-               454 MAKE_FUNCTION            4 (annotations)
-               456 STORE_NAME              43 (actor)
+   359         462 LOAD_CONST              11 ('return')
+               464 LOAD_NAME                9 (pd)
+               466 LOAD_ATTR               38 (DataFrame)
+               476 BUILD_TUPLE              2
+               478 LOAD_CONST              34 (<code object validation_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 359>)
+               480 MAKE_FUNCTION            4 (annotations)
+               482 STORE_NAME              41 (validation_history)
    
-   410         458 LOAD_CONST              11 ('return')
-               460 LOAD_NAME                9 (pd)
-               462 LOAD_ATTR               37 (DataFrame)
-               472 BUILD_TUPLE              2
-               474 LOAD_CONST              35 (<code object buyer, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 410>)
-               476 MAKE_FUNCTION            4 (annotations)
-               478 STORE_NAME              44 (buyer)
+   402         484 LOAD_CONST              35 (<code object searches_comment_counts, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 402>)
+               486 MAKE_FUNCTION            0
+               488 STORE_NAME              42 (searches_comment_counts)
    
-   507         480 LOAD_CONST              23 ('search_uid')
-               482 LOAD_NAME               33 (int)
-               484 BUILD_TUPLE              2
-               486 LOAD_CONST              36 (<code object search_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 507>)
-               488 MAKE_FUNCTION            4 (annotations)
-               490 STORE_NAME              45 (search_targets)
+   422         490 LOAD_CONST              36 (<code object enriched_searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 422>)
+               492 MAKE_FUNCTION            0
+               494 STORE_NAME              43 (enriched_searches_query)
    
-   641         492 LOAD_CONST              23 ('search_uid')
-               494 LOAD_NAME               33 (int)
-               496 LOAD_CONST              11 ('return')
+   442         496 LOAD_CONST              11 ('return')
                498 LOAD_NAME                9 (pd)
-               500 LOAD_ATTR               37 (DataFrame)
-               510 BUILD_TUPLE              4
-               512 LOAD_CONST              37 (<code object search_comments, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 641>)
+               500 LOAD_ATTR               38 (DataFrame)
+               510 BUILD_TUPLE              2
+               512 LOAD_CONST              37 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 442>)
                514 MAKE_FUNCTION            4 (annotations)
-               516 STORE_NAME              46 (search_comments)
+               516 STORE_NAME              44 (actor)
    
-   663         518 LOAD_CONST              23 ('search_uid')
-               520 LOAD_NAME               33 (int)
-               522 LOAD_CONST              11 ('return')
-               524 LOAD_NAME                9 (pd)
-               526 LOAD_ATTR               37 (DataFrame)
-               536 BUILD_TUPLE              4
-               538 LOAD_CONST              38 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 663>)
-               540 MAKE_FUNCTION            4 (annotations)
-               542 STORE_NAME              47 (event)
-   
-   675         544 LOAD_CONST              23 ('search_uid')
-               546 LOAD_NAME               33 (int)
-               548 LOAD_CONST              11 ('return')
-               550 LOAD_NAME                9 (pd)
-               552 LOAD_ATTR               37 (DataFrame)
-               562 BUILD_TUPLE              4
-               564 LOAD_CONST              39 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 675>)
-               566 MAKE_FUNCTION            4 (annotations)
-               568 STORE_NAME              48 (event_history)
-   
-   705         570 LOAD_CONST              23 ('search_uid')
-               572 LOAD_NAME               33 (int)
-               574 LOAD_CONST              11 ('return')
-               576 LOAD_NAME                9 (pd)
-               578 LOAD_ATTR               37 (DataFrame)
-               588 BUILD_TUPLE              4
-               590 LOAD_CONST              40 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 705>)
-               592 MAKE_FUNCTION            4 (annotations)
-               594 STORE_NAME              49 (search_criteria_history)
-   
-   734         596 LOAD_CONST              41 ('uid')
-               598 LOAD_NAME               33 (int)
-               600 LOAD_CONST              11 ('return')
-               602 LOAD_NAME               16 (ts)
-               604 LOAD_ATTR               28 (models)
-               614 LOAD_ATTR               25 (Search)
-               624 BUILD_TUPLE              4
-               626 LOAD_CONST              42 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 734>)
-               628 MAKE_FUNCTION            4 (annotations)
-               630 STORE_NAME              50 (find_search)
-   
-   762         632 LOAD_CONST              43 ('searchToken')
-               634 LOAD_NAME               34 (str)
-               636 LOAD_CONST              11 ('return')
-               638 LOAD_NAME               16 (ts)
-               640 LOAD_ATTR               28 (models)
-               650 LOAD_ATTR               25 (Search)
-               660 BUILD_TUPLE              4
-               662 LOAD_CONST              44 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 762>)
-               664 MAKE_FUNCTION            4 (annotations)
-               666 STORE_NAME              51 (find_search_by_token)
-   
-   771         668 LOAD_CONST              45 ('domain')
-               670 LOAD_NAME               34 (str)
-               672 LOAD_CONST              11 ('return')
-               674 LOAD_NAME               22 (Company)
-               676 BUILD_TUPLE              4
-               678 LOAD_CONST              46 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 771>)
-               680 MAKE_FUNCTION            4 (annotations)
-               682 STORE_NAME              52 (find_company_by_domain)
-   
-   787         684 LOAD_CONST              47 ('email')
-               686 LOAD_NAME               34 (str)
-               688 LOAD_CONST              11 ('return')
-               690 LOAD_NAME               22 (Company)
-               692 BUILD_TUPLE              4
-               694 LOAD_CONST              48 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 787>)
-               696 MAKE_FUNCTION            4 (annotations)
-               698 STORE_NAME              53 (find_actor_by_email)
-   
-   803         700 LOAD_CONST              49 ('event_id')
-               702 LOAD_NAME               33 (int)
-               704 LOAD_CONST              11 ('return')
-               706 LOAD_NAME               23 (Event)
-               708 BUILD_TUPLE              4
-               710 LOAD_CONST              50 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 803>)
-               712 MAKE_FUNCTION            4 (annotations)
-               714 STORE_NAME              54 (find_event_by_id)
-   
-   822         716 LOAD_CONST              13 ('company')
-               718 LOAD_NAME               22 (Company)
-               720 LOAD_CONST              11 ('return')
-               722 LOAD_CONST               1 (None)
-               724 BUILD_TUPLE              4
-               726 LOAD_CONST              51 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 822>)
-               728 MAKE_FUNCTION            4 (annotations)
-               730 STORE_NAME              55 (update_company)
-   
-   851         732 LOAD_CONST              17 ('search')
-               734 LOAD_NAME               25 (Search)
-               736 LOAD_CONST              11 ('return')
-               738 LOAD_CONST               1 (None)
-               740 BUILD_TUPLE              4
-               742 LOAD_CONST              52 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 851>)
-               744 MAKE_FUNCTION            4 (annotations)
-               746 STORE_NAME              56 (update_search)
-   
-   874         748 LOAD_CONST              49 ('event_id')
-               750 LOAD_NAME               33 (int)
-               752 LOAD_CONST              11 ('return')
-               754 LOAD_CONST               1 (None)
+   456         518 LOAD_CONST              11 ('return')
+               520 LOAD_NAME                9 (pd)
+               522 LOAD_ATTR               38 (DataFrame)
+               532 BUILD_TUPLE              2
+               534 LOAD_CONST              38 (<code object buyer, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 456>)
+               536 MAKE_FUNCTION            4 (annotations)
+               538 STORE_NAME              45 (buyer)
+   
+   553         540 LOAD_CONST              26 ('search_uid')
+               542 LOAD_NAME               34 (int)
+               544 BUILD_TUPLE              2
+               546 LOAD_CONST              39 (<code object search_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 553>)
+               548 MAKE_FUNCTION            4 (annotations)
+               550 STORE_NAME              46 (search_targets)
+   
+   687         552 LOAD_CONST              26 ('search_uid')
+               554 LOAD_NAME               34 (int)
+               556 LOAD_CONST              11 ('return')
+               558 LOAD_NAME                9 (pd)
+               560 LOAD_ATTR               38 (DataFrame)
+               570 BUILD_TUPLE              4
+               572 LOAD_CONST              40 (<code object search_comments, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 687>)
+               574 MAKE_FUNCTION            4 (annotations)
+               576 STORE_NAME              47 (search_comments)
+   
+   709         578 LOAD_CONST              26 ('search_uid')
+               580 LOAD_NAME               34 (int)
+               582 LOAD_CONST              11 ('return')
+               584 LOAD_NAME                9 (pd)
+               586 LOAD_ATTR               38 (DataFrame)
+               596 BUILD_TUPLE              4
+               598 LOAD_CONST              41 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 709>)
+               600 MAKE_FUNCTION            4 (annotations)
+               602 STORE_NAME              48 (event)
+   
+   721         604 LOAD_CONST              26 ('search_uid')
+               606 LOAD_NAME               34 (int)
+               608 LOAD_CONST              11 ('return')
+               610 LOAD_NAME                9 (pd)
+               612 LOAD_ATTR               38 (DataFrame)
+               622 BUILD_TUPLE              4
+               624 LOAD_CONST              42 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 721>)
+               626 MAKE_FUNCTION            4 (annotations)
+               628 STORE_NAME              49 (event_history)
+   
+   751         630 LOAD_CONST              26 ('search_uid')
+               632 LOAD_NAME               34 (int)
+               634 LOAD_CONST              11 ('return')
+               636 LOAD_NAME                9 (pd)
+               638 LOAD_ATTR               38 (DataFrame)
+               648 BUILD_TUPLE              4
+               650 LOAD_CONST              43 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 751>)
+               652 MAKE_FUNCTION            4 (annotations)
+               654 STORE_NAME              50 (search_criteria_history)
+   
+   780         656 LOAD_CONST              44 ('uid')
+               658 LOAD_NAME               34 (int)
+               660 LOAD_CONST              11 ('return')
+               662 LOAD_NAME               16 (ts)
+               664 LOAD_ATTR               28 (models)
+               674 LOAD_ATTR               25 (Search)
+               684 BUILD_TUPLE              4
+               686 LOAD_CONST              45 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 780>)
+               688 MAKE_FUNCTION            4 (annotations)
+               690 STORE_NAME              51 (find_search)
+   
+   804         692 LOAD_CONST              46 ('label')
+               694 LOAD_NAME               35 (str)
+               696 LOAD_CONST              11 ('return')
+               698 LOAD_NAME               16 (ts)
+               700 LOAD_ATTR               28 (models)
+               710 LOAD_ATTR               25 (Search)
+               720 BUILD_TUPLE              4
+               722 LOAD_CONST              47 (<code object find_search_by_label, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 804>)
+               724 MAKE_FUNCTION            4 (annotations)
+               726 STORE_NAME              52 (find_search_by_label)
+   
+   828         728 LOAD_CONST              48 ('searchToken')
+               730 LOAD_NAME               35 (str)
+               732 LOAD_CONST              11 ('return')
+               734 LOAD_NAME               16 (ts)
+               736 LOAD_ATTR               28 (models)
+               746 LOAD_ATTR               25 (Search)
                756 BUILD_TUPLE              4
-               758 LOAD_CONST              53 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 874>)
+               758 LOAD_CONST              49 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 828>)
                760 MAKE_FUNCTION            4 (annotations)
-               762 STORE_NAME              57 (mute_event)
+               762 STORE_NAME              53 (find_search_by_token)
    
-   897         764 LOAD_CONST              54 ('comment_id')
-               766 LOAD_NAME               33 (int)
+   837         764 LOAD_CONST              50 ('domain')
+               766 LOAD_NAME               35 (str)
                768 LOAD_CONST              11 ('return')
-               770 LOAD_CONST               1 (None)
+               770 LOAD_NAME               22 (Company)
                772 BUILD_TUPLE              4
-               774 LOAD_CONST              55 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 897>)
+               774 LOAD_CONST              51 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 837>)
                776 MAKE_FUNCTION            4 (annotations)
-               778 STORE_NAME              58 (delete_comment)
+               778 STORE_NAME              54 (find_company_by_domain)
    
-   908         780 LOAD_CONST              23 ('search_uid')
-               782 LOAD_NAME               33 (int)
+   853         780 LOAD_CONST              52 ('email')
+               782 LOAD_NAME               35 (str)
                784 LOAD_CONST              11 ('return')
-               786 LOAD_CONST               1 (None)
+               786 LOAD_NAME               22 (Company)
                788 BUILD_TUPLE              4
-               790 LOAD_CONST              56 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 908>)
+               790 LOAD_CONST              53 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 853>)
                792 MAKE_FUNCTION            4 (annotations)
-               794 STORE_NAME              59 (reset_inbox)
-               796 LOAD_CONST               1 (None)
-               798 RETURN_VALUE
+               794 STORE_NAME              55 (find_actor_by_email)
+   
+   869         796 LOAD_CONST              54 ('event_id')
+               798 LOAD_NAME               34 (int)
+               800 LOAD_CONST              11 ('return')
+               802 LOAD_NAME               23 (Event)
+               804 BUILD_TUPLE              4
+               806 LOAD_CONST              55 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 869>)
+               808 MAKE_FUNCTION            4 (annotations)
+               810 STORE_NAME              56 (find_event_by_id)
+   
+   888         812 LOAD_CONST              13 ('company')
+               814 LOAD_NAME               22 (Company)
+               816 LOAD_CONST              11 ('return')
+               818 LOAD_CONST               1 (None)
+               820 BUILD_TUPLE              4
+               822 LOAD_CONST              56 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 888>)
+               824 MAKE_FUNCTION            4 (annotations)
+               826 STORE_NAME              57 (update_company)
+   
+   917         828 LOAD_CONST              17 ('search')
+               830 LOAD_NAME               25 (Search)
+               832 LOAD_CONST              11 ('return')
+               834 LOAD_CONST               1 (None)
+               836 BUILD_TUPLE              4
+               838 LOAD_CONST              57 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 917>)
+               840 MAKE_FUNCTION            4 (annotations)
+               842 STORE_NAME              58 (update_search)
+   
+   940         844 LOAD_CONST              54 ('event_id')
+               846 LOAD_NAME               34 (int)
+               848 LOAD_CONST              11 ('return')
+               850 LOAD_CONST               1 (None)
+               852 BUILD_TUPLE              4
+               854 LOAD_CONST              58 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 940>)
+               856 MAKE_FUNCTION            4 (annotations)
+               858 STORE_NAME              59 (mute_event)
+   
+   963         860 LOAD_CONST              59 ('comment_id')
+               862 LOAD_NAME               34 (int)
+               864 LOAD_CONST              11 ('return')
+               866 LOAD_CONST               1 (None)
+               868 BUILD_TUPLE              4
+               870 LOAD_CONST              60 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 963>)
+               872 MAKE_FUNCTION            4 (annotations)
+               874 STORE_NAME              60 (delete_comment)
+   
+   974         876 LOAD_CONST              26 ('search_uid')
+               878 LOAD_NAME               34 (int)
+               880 LOAD_CONST              11 ('return')
+               882 LOAD_CONST               1 (None)
+               884 BUILD_TUPLE              4
+               886 LOAD_CONST              61 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 974>)
+               888 MAKE_FUNCTION            4 (annotations)
+               890 STORE_NAME              61 (reset_inbox)
+               892 LOAD_CONST               1 (None)
+               894 RETURN_VALUE
    consts
       0
       None
       ('asdict',)
       ('time',)
       ('Any', 'List')
       ('from_dict',)
@@ -911,14 +946,243 @@
          varnames   ('search', 'con', 'statement', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_search'
          firstlineno 84
          lnotab 0x02013401160102ff10071e013a012c0128f52e0c
+      'from_search'
+      'to_search'
+      code
+         argcount  : 2
+         nlocals   : 10
+         stacksize : 11
+         flags     : 3
+         code
+            0x97007401000000000000000000007c006a010000000000000000ac01a6
+            010000ab0100000000000000007d027c027c026402190000000000000000
+            0064036b0300000000190000000000000000007d027c0264041900000000
+            0000000000a0020000000000000000000000000000000000000000a60000
+            00ab0000000000000000007d037407000000000000000000007409000000
+            000000000000007c03a6010000ab010000000000000000a6010000ab0100
+            00000000000000010067007d04740a00000000000000000000a006000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            0035007d057c05a0070000000000000000000000000000000000000000a6
+            000000ab000000000000000000350001007c0344005d7e7d067410000000
+            000000000000006a090000000000000000a00a0000000000000000000000
+            0000000000000000007c06a6010000ab0100000000000000007d067c05a0
+            0b0000000000000000000000000000000000000000741900000000000000
+            0000006a0d00000000000000006405a6010000ab0100000000000000007c
+            016a01000000000000000064067c06640764089c04a6020000ab02000000
+            00000000007d077c07a00e00000000000000000000000000000000000000
+            00a6000000ab0000000000000000007d087c0881157c04a00f0000000000
+            0000000000000000000000000000007c08a6010000ab0100000000000000
+            0001008c7f0900640064006400a6020000ab02000000000000000001006e
+            0b23003100730477027803590077010100590001000100640064006400a6
+            020000ab02000000000000000001006e0b23003100730477027803590077
+            0101005900010001007c0444005d177d097411000000000000000000006a
+            1000000000000000007c09ac09a6010000ab01000000000000000001008c
+            1864005300
+         100           0 RESUME                   0
+         
+         107           2 LOAD_GLOBAL              1 (NULL + search_targets)
+                      14 LOAD_FAST                0 (from_search)
+                      16 LOAD_ATTR                1 (uid)
+                      26 KW_NAMES                 1
+                      28 PRECALL                  1
+                      32 CALL                     1
+                      42 STORE_FAST               2 (targets)
+         
+         108          44 LOAD_FAST                2 (targets)
+                      46 LOAD_FAST                2 (targets)
+                      48 LOAD_CONST               2 ('stage')
+                      50 BINARY_SUBSCR
+                      60 LOAD_CONST               3 ('reject')
+                      62 COMPARE_OP               3 (!=)
+                      68 BINARY_SUBSCR
+                      78 STORE_FAST               2 (targets)
+         
+         109          80 LOAD_FAST                2 (targets)
+                      82 LOAD_CONST               4 ('domain')
+                      84 BINARY_SUBSCR
+                      94 LOAD_METHOD              2 (tolist)
+                     116 PRECALL                  0
+                     120 CALL                     0
+                     130 STORE_FAST               3 (domains)
+         
+         110         132 LOAD_GLOBAL              7 (NULL + print)
+                     144 LOAD_GLOBAL              9 (NULL + len)
+                     156 LOAD_FAST                3 (domains)
+                     158 PRECALL                  1
+                     162 CALL                     1
+                     172 PRECALL                  1
+                     176 CALL                     1
+                     186 POP_TOP
+         
+         114         188 BUILD_LIST               0
+                     190 STORE_FAST               4 (new_event_ids)
+         
+         115         192 LOAD_GLOBAL             10 (db)
+                     204 LOAD_METHOD              6 (connect)
+                     226 PRECALL                  0
+                     230 CALL                     0
+                     240 BEFORE_WITH
+                     242 STORE_FAST               5 (con)
+         
+         116         244 LOAD_FAST                5 (con)
+                     246 LOAD_METHOD              7 (begin)
+                     268 PRECALL                  0
+                     272 CALL                     0
+                     282 BEFORE_WITH
+                     284 POP_TOP
+         
+         117         286 LOAD_FAST                3 (domains)
+                     288 GET_ITER
+                 >>  290 FOR_ITER               126 (to 544)
+                     292 STORE_FAST               6 (domain)
+         
+         119         294 LOAD_GLOBAL             16 (ts)
+                     306 LOAD_ATTR                9 (helpers)
+                     316 LOAD_METHOD             10 (clean_domain)
+                     338 LOAD_FAST                6 (domain)
+                     340 PRECALL                  1
+                     344 CALL                     1
+                     354 STORE_FAST               6 (domain)
+         
+         121         356 LOAD_FAST                5 (con)
+                     358 LOAD_METHOD             11 (execute)
+         
+         122         380 LOAD_GLOBAL             25 (NULL + sqlalchemy)
+                     392 LOAD_ATTR               13 (text)
+         
+         123         402 LOAD_CONST               5 ('\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        ')
+         
+         122         404 PRECALL                  1
+                     408 CALL                     1
+         
+         131         418 LOAD_FAST                1 (to_search)
+                     420 LOAD_ATTR                1 (uid)
+         
+         132         430 LOAD_CONST               6 ('chatgpt')
+         
+         133         432 LOAD_FAST                6 (domain)
+         
+         134         434 LOAD_CONST               7 ('land')
+         
+         130         436 LOAD_CONST               8 (('search_uid', 'actor_key', 'domain', 'type'))
+                     438 BUILD_CONST_KEY_MAP      4
+         
+         121         440 PRECALL                  2
+                     444 CALL                     2
+                     454 STORE_FAST               7 (result)
+         
+         138         456 LOAD_FAST                7 (result)
+                     458 LOAD_METHOD             14 (scalar_one)
+                     480 PRECALL                  0
+                     484 CALL                     0
+                     494 STORE_FAST               8 (new_event_id)
+         
+         139         496 LOAD_FAST                8 (new_event_id)
+                     498 POP_JUMP_FORWARD_IF_NONE    21 (to 542)
+         
+         140         500 LOAD_FAST                4 (new_event_ids)
+                     502 LOAD_METHOD             15 (append)
+                     524 LOAD_FAST                8 (new_event_id)
+                     526 PRECALL                  1
+                     530 CALL                     1
+                     540 POP_TOP
+                 >>  542 JUMP_BACKWARD          127 (to 290)
+         
+         117     >>  544 NOP
+         
+         116         546 LOAD_CONST               0 (None)
+                     548 LOAD_CONST               0 (None)
+                     550 LOAD_CONST               0 (None)
+                     552 PRECALL                  2
+                     556 CALL                     2
+                     566 POP_TOP
+                     568 JUMP_FORWARD            11 (to 592)
+                 >>  570 PUSH_EXC_INFO
+                     572 WITH_EXCEPT_START
+                     574 POP_JUMP_FORWARD_IF_TRUE     4 (to 584)
+                     576 RERAISE                  2
+                 >>  578 COPY                     3
+                     580 POP_EXCEPT
+                     582 RERAISE                  1
+                 >>  584 POP_TOP
+                     586 POP_EXCEPT
+                     588 POP_TOP
+                     590 POP_TOP
+         
+         115     >>  592 LOAD_CONST               0 (None)
+                     594 LOAD_CONST               0 (None)
+                     596 LOAD_CONST               0 (None)
+                     598 PRECALL                  2
+                     602 CALL                     2
+                     612 POP_TOP
+                     614 JUMP_FORWARD            11 (to 638)
+                 >>  616 PUSH_EXC_INFO
+                     618 WITH_EXCEPT_START
+                     620 POP_JUMP_FORWARD_IF_TRUE     4 (to 630)
+                     622 RERAISE                  2
+                 >>  624 COPY                     3
+                     626 POP_EXCEPT
+                     628 RERAISE                  1
+                 >>  630 POP_TOP
+                     632 POP_EXCEPT
+                     634 POP_TOP
+                     636 POP_TOP
+         
+         142     >>  638 LOAD_FAST                4 (new_event_ids)
+                     640 GET_ITER
+                 >>  642 FOR_ITER                23 (to 690)
+                     644 STORE_FAST               9 (event_id)
+         
+         143         646 LOAD_GLOBAL             17 (NULL + ts)
+                     658 LOAD_ATTR               16 (trigger_process_event)
+                     668 LOAD_FAST                9 (event_id)
+                     670 KW_NAMES                 9
+                     672 PRECALL                  1
+                     676 CALL                     1
+                     686 POP_TOP
+                     688 JUMP_BACKWARD           24 (to 642)
+         
+         142     >>  690 LOAD_CONST               0 (None)
+                     692 RETURN_VALUE
+         ExceptionTable:
+           242 to 282 -> 616 [1] lasti
+           284 to 542 -> 570 [2] lasti
+           546 to 568 -> 616 [1] lasti
+           570 to 576 -> 578 [4] lasti
+           578 to 582 -> 616 [1] lasti
+           584 to 584 -> 578 [4] lasti
+           586 to 590 -> 616 [1] lasti
+           616 to 622 -> 624 [3] lasti
+           630 to 630 -> 624 [3] lasti
+         consts
+            None
+            ('search_uid',)
+            'stage'
+            'reject'
+            'domain'
+            '\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        '
+            'chatgpt'
+            'land'
+            ('search_uid', 'actor_key', 'domain', 'type')
+            ('event_id',)
+         names      ('search_targets', 'uid', 'tolist', 'print', 'len', 'db', 'connect', 'begin', 'ts', 'helpers', 'clean_domain', 'execute', 'sqlalchemy', 'text', 'scalar_one', 'append', 'trigger_process_event')
+         varnames   ('from_search', 'to_search', 'targets', 'domains', 'new_event_ids', 'con', 'domain', 'result', 'new_event_id', 'event_id')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
+         name       'important_targets_from_search'
+         firstlineno 100
+         lnotab
+            0x02072a01240134013804040134012a0108023e021801160102ff0e090c
+            010201020102fc04f71011280104012ce902ff2eff2e1b08012cff
       code
          argcount  : 1
          nlocals   : 12
          stacksize : 16
          flags     : 3
          code
             0x870c97007c006a000000000000000000a0010000000000000000000000
@@ -959,179 +1223,179 @@
             00640064006400a6020000ab02000000000000000001006e0b2300310073
             0477027803590077010100590001000100640064006400a6020000ab0200
             0000000000000001006e0b23003100730477027803590077010100590001
             0001007c0544005d177d0b7413000000000000000000006a180000000000
             0000007c0bac0fa6010000ab01000000000000000001008c1864005300
                        0 MAKE_CELL               12 (stage_dict)
          
-         100           2 RESUME                   0
+         146           2 RESUME                   0
          
-         102           4 LOAD_FAST                0 (event)
+         148           4 LOAD_FAST                0 (event)
                        6 LOAD_ATTR                0 (data)
                       16 LOAD_METHOD              1 (get)
                       38 LOAD_CONST               1 ('source')
                       40 PRECALL                  1
                       44 CALL                     1
                       54 STORE_FAST               1 (source)
          
-         103          56 LOAD_GLOBAL              5 (NULL + search_targets)
+         149          56 LOAD_GLOBAL              5 (NULL + search_targets)
                       68 LOAD_FAST                0 (event)
                       70 LOAD_ATTR                3 (search_uid)
                       80 KW_NAMES                 2
                       82 PRECALL                  1
                       86 CALL                     1
                       96 STORE_FAST               2 (targets)
          
-         104          98 LOAD_FAST                2 (targets)
+         150          98 LOAD_FAST                2 (targets)
                      100 LOAD_METHOD              4 (set_index)
                      122 LOAD_CONST               3 ('domain')
                      124 PRECALL                  1
                      128 CALL                     1
                      138 LOAD_CONST               4 ('stage')
                      140 BINARY_SUBSCR
                      150 LOAD_METHOD              5 (to_dict)
                      172 PRECALL                  0
                      176 CALL                     0
                      186 STORE_DEREF             12 (stage_dict)
          
-         106         188 LOAD_CLOSURE            12 (stage_dict)
+         152         188 LOAD_CLOSURE            12 (stage_dict)
                      190 BUILD_TUPLE              1
-                     192 LOAD_CONST               5 (<code object get_stage, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 106>)
+                     192 LOAD_CONST               5 (<code object get_stage, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 152>)
                      194 MAKE_FUNCTION            8 (closure)
                      196 STORE_FAST               3 (get_stage)
          
-         110         198 LOAD_FAST                0 (event)
+         156         198 LOAD_FAST                0 (event)
                      200 LOAD_ATTR                0 (data)
                      210 LOAD_CONST               6 ('domains')
                      212 BINARY_SUBSCR
                      222 STORE_FAST               4 (domains)
          
-         112         224 BUILD_LIST               0
+         158         224 BUILD_LIST               0
                      226 STORE_FAST               5 (new_event_ids)
          
-         113         228 LOAD_GLOBAL             12 (db)
+         159         228 LOAD_GLOBAL             12 (db)
                      240 LOAD_METHOD              7 (connect)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 BEFORE_WITH
                      278 STORE_FAST               6 (con)
          
-         114         280 LOAD_FAST                6 (con)
+         160         280 LOAD_FAST                6 (con)
                      282 LOAD_METHOD              8 (begin)
                      304 PRECALL                  0
                      308 CALL                     0
                      318 BEFORE_WITH
                      320 POP_TOP
          
-         115         322 LOAD_FAST                4 (domains)
+         161         322 LOAD_FAST                4 (domains)
                      324 GET_ITER
                  >>  326 EXTENDED_ARG             1
                      328 FOR_ITER               359 (to 1048)
                      330 STORE_FAST               7 (domain)
          
-         117         332 LOAD_GLOBAL             18 (ts)
+         163         332 LOAD_GLOBAL             18 (ts)
                      344 LOAD_ATTR               10 (helpers)
                      354 LOAD_METHOD             11 (clean_domain)
                      376 LOAD_FAST                7 (domain)
                      378 PRECALL                  1
                      382 CALL                     1
                      392 STORE_FAST               7 (domain)
          
-         118         394 LOAD_FAST                6 (con)
+         164         394 LOAD_FAST                6 (con)
                      396 LOAD_METHOD             12 (execute)
          
-         119         418 LOAD_GLOBAL             27 (NULL + sqlalchemy)
+         165         418 LOAD_GLOBAL             27 (NULL + sqlalchemy)
                      430 LOAD_ATTR               14 (text)
          
-         120         440 LOAD_CONST               7 ('\n                        INSERT INTO company (domain, source) \n                        VALUES(:domain, :source)\n                        ON CONFLICT DO NOTHING\n                        ')
+         166         440 LOAD_CONST               7 ('\n                        INSERT INTO company (domain, source) \n                        VALUES(:domain, :source)\n                        ON CONFLICT DO NOTHING\n                        ')
          
-         119         442 PRECALL                  1
+         165         442 PRECALL                  1
                      446 CALL                     1
          
-         126         456 LOAD_FAST                7 (domain)
+         172         456 LOAD_FAST                7 (domain)
                      458 LOAD_FAST                1 (source)
                      460 LOAD_CONST               8 (('domain', 'source'))
                      462 BUILD_CONST_KEY_MAP      2
          
-         118         464 PRECALL                  2
+         164         464 PRECALL                  2
                      468 CALL                     2
                      478 POP_TOP
          
-         129         480 LOAD_FAST                6 (con)
+         175         480 LOAD_FAST                6 (con)
                      482 LOAD_METHOD             12 (execute)
          
-         130         504 LOAD_GLOBAL             27 (NULL + sqlalchemy)
+         176         504 LOAD_GLOBAL             27 (NULL + sqlalchemy)
                      516 LOAD_ATTR               14 (text)
          
-         131         526 LOAD_CONST               9 ('\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        ')
+         177         526 LOAD_CONST               9 ('\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        ')
          
-         130         528 PRECALL                  1
+         176         528 PRECALL                  1
                      532 CALL                     1
          
-         139         542 LOAD_FAST                0 (event)
+         185         542 LOAD_FAST                0 (event)
                      544 LOAD_ATTR                3 (search_uid)
          
-         140         554 LOAD_FAST                0 (event)
+         186         554 LOAD_FAST                0 (event)
                      556 LOAD_ATTR               15 (actor_key)
          
-         141         566 LOAD_FAST                7 (domain)
+         187         566 LOAD_FAST                7 (domain)
          
-         142         568 LOAD_FAST                0 (event)
+         188         568 LOAD_FAST                0 (event)
                      570 LOAD_ATTR                0 (data)
                      580 LOAD_METHOD              1 (get)
                      602 LOAD_CONST               4 ('stage')
                      604 LOAD_CONST              10 ('create')
                      606 PRECALL                  2
                      610 CALL                     2
          
-         138         620 LOAD_CONST              11 (('search_uid', 'actor_key', 'domain', 'type'))
+         184         620 LOAD_CONST              11 (('search_uid', 'actor_key', 'domain', 'type'))
                      622 BUILD_CONST_KEY_MAP      4
          
-         129         624 PRECALL                  2
+         175         624 PRECALL                  2
                      628 CALL                     2
                      638 STORE_FAST               8 (result)
          
-         146         640 LOAD_FAST                8 (result)
+         192         640 LOAD_FAST                8 (result)
                      642 LOAD_METHOD             16 (scalar_one)
                      664 PRECALL                  0
                      668 CALL                     0
                      678 STORE_FAST               9 (new_event_id)
          
-         147         680 LOAD_FAST                9 (new_event_id)
+         193         680 LOAD_FAST                9 (new_event_id)
                      682 POP_JUMP_FORWARD_IF_NONE    21 (to 726)
          
-         148         684 LOAD_FAST                5 (new_event_ids)
+         194         684 LOAD_FAST                5 (new_event_ids)
                      686 LOAD_METHOD             17 (append)
                      708 LOAD_FAST                9 (new_event_id)
                      710 PRECALL                  1
                      714 CALL                     1
                      724 POP_TOP
          
-         150     >>  726 LOAD_DEREF              12 (stage_dict)
+         196     >>  726 LOAD_DEREF              12 (stage_dict)
                      728 LOAD_METHOD              1 (get)
                      750 LOAD_FAST                7 (domain)
                      752 PRECALL                  1
                      756 CALL                     1
                      766 POP_JUMP_FORWARD_IF_NONE   138 (to 1044)
          
-         151         768 LOAD_GLOBAL             18 (ts)
+         197         768 LOAD_GLOBAL             18 (ts)
                      780 LOAD_ATTR               18 (models)
                      790 LOAD_METHOD             19 (Event)
          
-         152         812 LOAD_FAST                0 (event)
+         198         812 LOAD_FAST                0 (event)
                      814 LOAD_ATTR                3 (search_uid)
          
-         153         824 LOAD_FAST                0 (event)
+         199         824 LOAD_FAST                0 (event)
                      826 LOAD_ATTR               15 (actor_key)
          
-         154         836 LOAD_FAST                7 (domain)
+         200         836 LOAD_FAST                7 (domain)
          
-         155         838 LOAD_CONST              12 ('comment')
+         201         838 LOAD_CONST              12 ('comment')
          
-         157         840 LOAD_CONST              12 ('comment')
+         203         840 LOAD_CONST              12 ('comment')
                      842 PUSH_NULL
                      844 LOAD_FAST                3 (get_stage)
                      846 LOAD_FAST                7 (domain)
                      848 PRECALL                  1
                      852 CALL                     1
                      862 FORMAT_VALUE             0
                      864 LOAD_CONST              13 (' → ')
@@ -1144,34 +1408,34 @@
                      932 LOAD_CONST               4 ('stage')
                      934 PRECALL                  1
                      938 CALL                     1
                      948 BINARY_SUBSCR
                      958 FORMAT_VALUE             0
                      960 BUILD_STRING             3
          
-         156         962 BUILD_MAP                1
+         202         962 BUILD_MAP                1
          
-         151         964 KW_NAMES                14
+         197         964 KW_NAMES                14
                      966 PRECALL                  5
                      970 CALL                     5
                      980 STORE_FAST              10 (comment)
          
-         160         982 LOAD_GLOBAL             18 (ts)
+         206         982 LOAD_GLOBAL             18 (ts)
                      994 LOAD_ATTR               22 (query)
                     1004 LOAD_METHOD             23 (insert_event)
                     1026 LOAD_FAST               10 (comment)
                     1028 PRECALL                  1
                     1032 CALL                     1
                     1042 POP_TOP
                  >> 1044 EXTENDED_ARG             1
                     1046 JUMP_BACKWARD          361 (to 326)
          
-         115     >> 1048 NOP
+         161     >> 1048 NOP
          
-         114        1050 LOAD_CONST               0 (None)
+         160        1050 LOAD_CONST               0 (None)
                     1052 LOAD_CONST               0 (None)
                     1054 LOAD_CONST               0 (None)
                     1056 PRECALL                  2
                     1060 CALL                     2
                     1070 POP_TOP
                     1072 JUMP_FORWARD            11 (to 1096)
                  >> 1074 PUSH_EXC_INFO
@@ -1182,15 +1446,15 @@
                     1084 POP_EXCEPT
                     1086 RERAISE                  1
                  >> 1088 POP_TOP
                     1090 POP_EXCEPT
                     1092 POP_TOP
                     1094 POP_TOP
          
-         113     >> 1096 LOAD_CONST               0 (None)
+         159     >> 1096 LOAD_CONST               0 (None)
                     1098 LOAD_CONST               0 (None)
                     1100 LOAD_CONST               0 (None)
                     1102 PRECALL                  2
                     1106 CALL                     2
                     1116 POP_TOP
                     1118 JUMP_FORWARD            11 (to 1142)
                  >> 1120 PUSH_EXC_INFO
@@ -1201,29 +1465,29 @@
                     1130 POP_EXCEPT
                     1132 RERAISE                  1
                  >> 1134 POP_TOP
                     1136 POP_EXCEPT
                     1138 POP_TOP
                     1140 POP_TOP
          
-         162     >> 1142 LOAD_FAST                5 (new_event_ids)
+         208     >> 1142 LOAD_FAST                5 (new_event_ids)
                     1144 GET_ITER
                  >> 1146 FOR_ITER                23 (to 1194)
                     1148 STORE_FAST              11 (event_id)
          
-         163        1150 LOAD_GLOBAL             19 (NULL + ts)
+         209        1150 LOAD_GLOBAL             19 (NULL + ts)
                     1162 LOAD_ATTR               24 (trigger_process_event)
                     1172 LOAD_FAST               11 (event_id)
                     1174 KW_NAMES                15
                     1176 PRECALL                  1
                     1180 CALL                     1
                     1190 POP_TOP
                     1192 JUMP_BACKWARD           24 (to 1146)
          
-         162     >> 1194 LOAD_CONST               0 (None)
+         208     >> 1194 LOAD_CONST               0 (None)
                     1196 RETURN_VALUE
          ExceptionTable:
            278 to 318 -> 1120 [1] lasti
            320 to 1046 -> 1074 [2] lasti
            1050 to 1072 -> 1120 [1] lasti
            1074 to 1080 -> 1082 [4] lasti
            1082 to 1086 -> 1120 [1] lasti
@@ -1246,25 +1510,25 @@
                   0x950197008902a00000000000000000000000000000000000000000007c
                   006401a6020000ab0200000000000000007d017402000000000000000000
                   006a0200000000000000006a030000000000000000a00000000000000000
                   000000000000000000000000007c016401a6020000ab0200000000000000
                   005300
                              0 COPY_FREE_VARS           1
                
-               106           2 RESUME                   0
+               152           2 RESUME                   0
                
-               107           4 LOAD_DEREF               2 (stage_dict)
+               153           4 LOAD_DEREF               2 (stage_dict)
                              6 LOAD_METHOD              0 (get)
                             28 LOAD_FAST                0 (domain)
                             30 LOAD_CONST               1 ('Unknown')
                             32 PRECALL                  2
                             36 CALL                     2
                             46 STORE_FAST               1 (stage_key)
                
-               108          48 LOAD_GLOBAL              2 (ts)
+               154          48 LOAD_GLOBAL              2 (ts)
                             60 LOAD_ATTR                2 (constants)
                             70 LOAD_ATTR                3 (LABEL_MAP)
                             80 LOAD_METHOD              0 (get)
                            102 LOAD_FAST                1 (stage_key)
                            104 LOAD_CONST               1 ('Unknown')
                            106 PRECALL                  2
                            110 CALL                     2
@@ -1274,15 +1538,15 @@
                   'Unknown'
                names      ('get', 'ts', 'constants', 'LABEL_MAP')
                varnames   ('domain', 'stage_key')
                freevars   ('stage_dict',)
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_stage'
-               firstlineno 106
+               firstlineno 152
                lnotab 0x04012c01
             'domains'
             '\n                        INSERT INTO company (domain, source) \n                        VALUES(:domain, :source)\n                        ON CONFLICT DO NOTHING\n                        '
             ('domain', 'source')
             '\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        '
             'create'
             ('search_uid', 'actor_key', 'domain', 'type')
@@ -1292,15 +1556,15 @@
             ('event_id',)
          names      ('data', 'get', 'search_targets', 'search_uid', 'set_index', 'to_dict', 'db', 'connect', 'begin', 'ts', 'helpers', 'clean_domain', 'execute', 'sqlalchemy', 'text', 'actor_key', 'scalar_one', 'append', 'models', 'Event', 'constants', 'LABEL_MAP', 'query', 'insert_event', 'trigger_process_event')
          varnames   ('event', 'source', 'targets', 'get_stage', 'domains', 'new_event_ids', 'con', 'domain', 'result', 'new_event_id', 'comment', 'event_id')
          freevars   ()
          cellvars   ('stage_dict',)
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'important_targets_from_event'
-         firstlineno 100
+         firstlineno 146
          lnotab
             0x040234012a015a020a041a02040134012a010a023e011801160102ff0e
             0708f8100b1801160102ff0e090c010c01020134fc04f71011280104012a
             022a012c010c010c01020102027aff02fb120942d302ff2eff2e3108012c
             ff
       True
       'create'
@@ -1360,253 +1624,253 @@
             0278035900770101005900010001007401000000000000000000007c0ba6
             010000ab01000000000000000001007c0b44005d177d1174230000000000
             00000000006a1200000000000000007c11ac12a6010000ab010000000000
             00000001008c1874010000000000000000000064137c089b0064147c099b
             006415740900000000000000000000a6000000ab0000000000000000007c
             0a7a0a00009b0064169d07a6010000ab0100000000000000000100640053
             00
-         172           0 RESUME                   0
+         218           0 RESUME                   0
          
-         180           2 LOAD_GLOBAL              1 (NULL + print)
+         226           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('Inserting ')
                       16 LOAD_GLOBAL              3 (NULL + len)
                       28 LOAD_FAST                0 (companies)
                       30 PRECALL                  1
                       34 CALL                     1
                       44 FORMAT_VALUE             0
                       46 LOAD_CONST               2 (' companies as targets...')
                       48 BUILD_STRING             3
                       50 PRECALL                  1
                       54 CALL                     1
                       64 POP_TOP
          
-         182          66 LOAD_GLOBAL              5 (NULL + search_targets)
+         228          66 LOAD_GLOBAL              5 (NULL + search_targets)
                       78 LOAD_FAST                1 (search_uid)
                       80 KW_NAMES                 3
                       82 PRECALL                  1
                       86 CALL                     1
                       96 STORE_FAST               6 (targets)
          
-         184          98 LOAD_FAST                3 (force)
+         230          98 LOAD_FAST                3 (force)
                      100 POP_JUMP_FORWARD_IF_FALSE    45 (to 192)
          
-         187         102 LOAD_FAST                6 (targets)
+         233         102 LOAD_FAST                6 (targets)
                      104 LOAD_FAST                6 (targets)
                      106 LOAD_CONST               4 ('stage')
                      108 BINARY_SUBSCR
                      118 LOAD_CONST               5 ('reject')
                      120 COMPARE_OP               3 (!=)
                      126 BINARY_SUBSCR
                      136 STORE_FAST               6 (targets)
          
-         188         138 LOAD_FAST                6 (targets)
+         234         138 LOAD_FAST                6 (targets)
                      140 LOAD_CONST               6 ('domain')
                      142 BINARY_SUBSCR
                      152 LOAD_METHOD              3 (tolist)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 STORE_FAST               7 (protected_domains)
                      190 JUMP_FORWARD            26 (to 244)
          
-         190     >>  192 LOAD_FAST                6 (targets)
+         236     >>  192 LOAD_FAST                6 (targets)
                      194 LOAD_CONST               6 ('domain')
                      196 BINARY_SUBSCR
                      206 LOAD_METHOD              3 (tolist)
                      228 PRECALL                  0
                      232 CALL                     0
                      242 STORE_FAST               7 (protected_domains)
          
-         194     >>  244 LOAD_CONST               7 (0)
+         240     >>  244 LOAD_CONST               7 (0)
                      246 STORE_FAST               8 (inserted)
          
-         195         248 LOAD_CONST               7 (0)
+         241         248 LOAD_CONST               7 (0)
                      250 STORE_FAST               9 (skipped)
          
-         196         252 LOAD_GLOBAL              9 (NULL + time)
+         242         252 LOAD_GLOBAL              9 (NULL + time)
                      264 PRECALL                  0
                      268 CALL                     0
                      278 STORE_FAST              10 (start)
          
-         198         280 BUILD_LIST               0
+         244         280 BUILD_LIST               0
                      282 STORE_FAST              11 (new_event_ids)
          
-         199         284 LOAD_GLOBAL             10 (db)
+         245         284 LOAD_GLOBAL             10 (db)
                      296 LOAD_METHOD              6 (connect)
                      318 PRECALL                  0
                      322 CALL                     0
                      332 BEFORE_WITH
                      334 STORE_FAST              12 (con)
          
-         200         336 LOAD_FAST               12 (con)
+         246         336 LOAD_FAST               12 (con)
                      338 LOAD_METHOD              7 (begin)
                      360 PRECALL                  0
                      364 CALL                     0
                      374 BEFORE_WITH
                      376 POP_TOP
          
-         201         378 LOAD_FAST                0 (companies)
+         247         378 LOAD_FAST                0 (companies)
                      380 GET_ITER
                  >>  382 EXTENDED_ARG             1
                      384 FOR_ITER               382 (to 1150)
                      386 STORE_FAST              13 (company)
          
-         202         388 LOAD_GLOBAL              1 (NULL + print)
+         248         388 LOAD_GLOBAL              1 (NULL + print)
                      400 LOAD_FAST               13 (company)
                      402 PRECALL                  1
                      406 CALL                     1
                      416 POP_TOP
          
-         203         418 LOAD_GLOBAL             17 (NULL + helpers)
+         249         418 LOAD_GLOBAL             17 (NULL + helpers)
                      430 LOAD_ATTR                9 (domain_is_none)
                      440 LOAD_FAST               13 (company)
                      442 LOAD_METHOD             10 (get)
                      464 LOAD_CONST               6 ('domain')
                      466 PRECALL                  1
                      470 CALL                     1
                      480 PRECALL                  1
                      484 CALL                     1
                      494 POP_JUMP_FORWARD_IF_FALSE    20 (to 536)
          
-         204         496 LOAD_GLOBAL              1 (NULL + print)
+         250         496 LOAD_GLOBAL              1 (NULL + print)
                      508 LOAD_CONST               8 ('Missing domain: ')
                      510 LOAD_FAST               13 (company)
                      512 FORMAT_VALUE             0
                      514 LOAD_CONST               9 ('. Skipping')
                      516 BUILD_STRING             3
                      518 PRECALL                  1
                      522 CALL                     1
                      532 POP_TOP
          
-         205         534 JUMP_BACKWARD           77 (to 382)
+         251         534 JUMP_BACKWARD           77 (to 382)
          
-         207     >>  536 LOAD_FAST               13 (company)
+         253     >>  536 LOAD_FAST               13 (company)
                      538 LOAD_CONST               6 ('domain')
                      540 BINARY_SUBSCR
                      550 LOAD_FAST                7 (protected_domains)
                      552 CONTAINS_OP              0
                      554 POP_JUMP_FORWARD_IF_FALSE     6 (to 568)
          
-         209         556 LOAD_FAST                9 (skipped)
+         255         556 LOAD_FAST                9 (skipped)
                      558 LOAD_CONST              10 (1)
                      560 BINARY_OP               13 (+=)
                      564 STORE_FAST               9 (skipped)
          
-         210         566 JUMP_BACKWARD           93 (to 382)
+         256         566 JUMP_BACKWARD           93 (to 382)
          
-         212     >>  568 LOAD_FAST                8 (inserted)
+         258     >>  568 LOAD_FAST                8 (inserted)
                      570 LOAD_CONST              10 (1)
                      572 BINARY_OP               13 (+=)
                      576 STORE_FAST               8 (inserted)
          
-         215         578 LOAD_FAST               12 (con)
+         261         578 LOAD_FAST               12 (con)
                      580 LOAD_METHOD             11 (execute)
          
-         216         602 LOAD_GLOBAL             25 (NULL + sqlalchemy)
+         262         602 LOAD_GLOBAL             25 (NULL + sqlalchemy)
                      614 LOAD_ATTR               13 (text)
          
-         217         624 LOAD_CONST              11 ('\n                        INSERT INTO company (domain, name, description, source) \n                        VALUES(:domain, :name, :description, :source)\n                        ON CONFLICT DO NOTHING\n                        ')
+         263         624 LOAD_CONST              11 ('\n                        INSERT INTO company (domain, name, description, source) \n                        VALUES(:domain, :name, :description, :source)\n                        ON CONFLICT DO NOTHING\n                        ')
          
-         216         626 PRECALL                  1
+         262         626 PRECALL                  1
                      630 CALL                     1
          
-         224         640 LOAD_FAST               13 (company)
+         270         640 LOAD_FAST               13 (company)
                      642 LOAD_METHOD             10 (get)
                      664 LOAD_CONST               6 ('domain')
                      666 PRECALL                  1
                      670 CALL                     1
          
-         225         680 LOAD_FAST               13 (company)
+         271         680 LOAD_FAST               13 (company)
                      682 LOAD_METHOD             10 (get)
                      704 LOAD_CONST              12 ('name')
                      706 PRECALL                  1
                      710 CALL                     1
          
-         226         720 LOAD_FAST               13 (company)
+         272         720 LOAD_FAST               13 (company)
                      722 LOAD_METHOD             10 (get)
                      744 LOAD_CONST              13 ('description')
                      746 PRECALL                  1
                      750 CALL                     1
          
-         227         760 LOAD_FAST               13 (company)
+         273         760 LOAD_FAST               13 (company)
                      762 LOAD_METHOD             10 (get)
                      784 LOAD_CONST              14 ('source')
                      786 LOAD_FAST                4 (source)
                      788 PRECALL                  2
                      792 CALL                     2
          
-         223         802 LOAD_CONST              15 (('domain', 'name', 'description', 'source'))
+         269         802 LOAD_CONST              15 (('domain', 'name', 'description', 'source'))
                      804 BUILD_CONST_KEY_MAP      4
          
-         215         806 PRECALL                  2
+         261         806 PRECALL                  2
                      810 CALL                     2
                      820 POP_TOP
          
-         231         822 LOAD_FAST               12 (con)
+         277         822 LOAD_FAST               12 (con)
                      824 LOAD_METHOD             11 (execute)
          
-         232         846 LOAD_GLOBAL             25 (NULL + sqlalchemy)
+         278         846 LOAD_GLOBAL             25 (NULL + sqlalchemy)
                      858 LOAD_ATTR               13 (text)
          
-         233         868 LOAD_CONST              16 ('\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        ')
+         279         868 LOAD_CONST              16 ('\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        ')
          
-         232         870 PRECALL                  1
+         278         870 PRECALL                  1
                      874 CALL                     1
          
-         241         884 LOAD_FAST                1 (search_uid)
+         287         884 LOAD_FAST                1 (search_uid)
          
-         242         886 LOAD_FAST                2 (actor_key)
+         288         886 LOAD_FAST                2 (actor_key)
          
-         243         888 LOAD_FAST               13 (company)
+         289         888 LOAD_FAST               13 (company)
                      890 LOAD_METHOD             10 (get)
                      912 LOAD_CONST               6 ('domain')
                      914 PRECALL                  1
                      918 CALL                     1
          
-         244         928 LOAD_FAST                5 (stage)
+         290         928 LOAD_FAST                5 (stage)
          
-         240         930 LOAD_CONST              17 (('search_uid', 'actor_key', 'domain', 'type'))
+         286         930 LOAD_CONST              17 (('search_uid', 'actor_key', 'domain', 'type'))
                      932 BUILD_CONST_KEY_MAP      4
          
-         231         934 PRECALL                  2
+         277         934 PRECALL                  2
                      938 CALL                     2
                      948 STORE_FAST              14 (result)
          
-         251         950 LOAD_GLOBAL              1 (NULL + print)
+         297         950 LOAD_GLOBAL              1 (NULL + print)
                      962 LOAD_FAST               14 (result)
                      964 PRECALL                  1
                      968 CALL                     1
                      978 POP_TOP
          
-         252         980 NOP
+         298         980 NOP
          
-         253         982 LOAD_FAST               14 (result)
+         299         982 LOAD_FAST               14 (result)
                      984 LOAD_METHOD             14 (scalar_one)
                     1006 PRECALL                  0
                     1010 CALL                     0
                     1020 STORE_FAST              15 (new_event_id)
          
-         254        1022 LOAD_FAST               15 (new_event_id)
+         300        1022 LOAD_FAST               15 (new_event_id)
                     1024 POP_JUMP_FORWARD_IF_NONE    21 (to 1068)
          
-         255        1026 LOAD_FAST               11 (new_event_ids)
+         301        1026 LOAD_FAST               11 (new_event_ids)
                     1028 LOAD_METHOD             15 (append)
                     1050 LOAD_FAST               15 (new_event_id)
                     1052 PRECALL                  1
                     1056 CALL                     1
                     1066 POP_TOP
                  >> 1068 EXTENDED_ARG             1
                     1070 JUMP_BACKWARD          345 (to 382)
                  >> 1072 PUSH_EXC_INFO
          
-         256        1074 LOAD_GLOBAL             32 (Exception)
+         302        1074 LOAD_GLOBAL             32 (Exception)
                     1086 CHECK_EXC_MATCH
                     1088 POP_JUMP_FORWARD_IF_FALSE    26 (to 1142)
                     1090 STORE_FAST              16 (e)
          
-         257        1092 LOAD_GLOBAL              1 (NULL + print)
+         303        1092 LOAD_GLOBAL              1 (NULL + print)
                     1104 LOAD_FAST               16 (e)
                     1106 PRECALL                  1
                     1110 CALL                     1
                     1120 POP_TOP
                     1122 POP_EXCEPT
                     1124 LOAD_CONST               0 (None)
                     1126 STORE_FAST              16 (e)
@@ -1614,22 +1878,22 @@
                     1130 EXTENDED_ARG             1
                     1132 JUMP_BACKWARD          376 (to 382)
                  >> 1134 LOAD_CONST               0 (None)
                     1136 STORE_FAST              16 (e)
                     1138 DELETE_FAST             16 (e)
                     1140 RERAISE                  1
          
-         256     >> 1142 RERAISE                  0
+         302     >> 1142 RERAISE                  0
                  >> 1144 COPY                     3
                     1146 POP_EXCEPT
                     1148 RERAISE                  1
          
-         201     >> 1150 NOP
+         247     >> 1150 NOP
          
-         200        1152 LOAD_CONST               0 (None)
+         246        1152 LOAD_CONST               0 (None)
                     1154 LOAD_CONST               0 (None)
                     1156 LOAD_CONST               0 (None)
                     1158 PRECALL                  2
                     1162 CALL                     2
                     1172 POP_TOP
                     1174 JUMP_FORWARD            11 (to 1198)
                  >> 1176 PUSH_EXC_INFO
@@ -1640,15 +1904,15 @@
                     1186 POP_EXCEPT
                     1188 RERAISE                  1
                  >> 1190 POP_TOP
                     1192 POP_EXCEPT
                     1194 POP_TOP
                     1196 POP_TOP
          
-         199     >> 1198 LOAD_CONST               0 (None)
+         245     >> 1198 LOAD_CONST               0 (None)
                     1200 LOAD_CONST               0 (None)
                     1202 LOAD_CONST               0 (None)
                     1204 PRECALL                  2
                     1208 CALL                     2
                     1218 POP_TOP
                     1220 JUMP_FORWARD            11 (to 1244)
                  >> 1222 PUSH_EXC_INFO
@@ -1659,35 +1923,35 @@
                     1232 POP_EXCEPT
                     1234 RERAISE                  1
                  >> 1236 POP_TOP
                     1238 POP_EXCEPT
                     1240 POP_TOP
                     1242 POP_TOP
          
-         259     >> 1244 LOAD_GLOBAL              1 (NULL + print)
+         305     >> 1244 LOAD_GLOBAL              1 (NULL + print)
                     1256 LOAD_FAST               11 (new_event_ids)
                     1258 PRECALL                  1
                     1262 CALL                     1
                     1272 POP_TOP
          
-         260        1274 LOAD_FAST               11 (new_event_ids)
+         306        1274 LOAD_FAST               11 (new_event_ids)
                     1276 GET_ITER
                  >> 1278 FOR_ITER                23 (to 1326)
                     1280 STORE_FAST              17 (event_id)
          
-         261        1282 LOAD_GLOBAL             35 (NULL + ts)
+         307        1282 LOAD_GLOBAL             35 (NULL + ts)
                     1294 LOAD_ATTR               18 (trigger_process_event)
                     1304 LOAD_FAST               17 (event_id)
                     1306 KW_NAMES                18
                     1308 PRECALL                  1
                     1312 CALL                     1
                     1322 POP_TOP
                     1324 JUMP_BACKWARD           24 (to 1278)
          
-         262     >> 1326 LOAD_GLOBAL              1 (NULL + print)
+         308     >> 1326 LOAD_GLOBAL              1 (NULL + print)
                     1338 LOAD_CONST              19 ('Inserted ')
                     1340 LOAD_FAST                8 (inserted)
                     1342 FORMAT_VALUE             0
                     1344 LOAD_CONST              20 ('. Skipped ')
                     1346 LOAD_FAST                9 (skipped)
                     1348 FORMAT_VALUE             0
                     1350 LOAD_CONST              21 ('. Took ')
@@ -1747,15 +2011,15 @@
             ' seconds'
          names      ('print', 'len', 'search_targets', 'tolist', 'time', 'db', 'connect', 'begin', 'helpers', 'domain_is_none', 'get', 'execute', 'sqlalchemy', 'text', 'scalar_one', 'append', 'Exception', 'ts', 'trigger_process_event')
          varnames   ('companies', 'search_uid', 'actor_key', 'force', 'source', 'stage', 'targets', 'protected_domains', 'inserted', 'skipped', 'start', 'new_event_ids', 'con', 'company', 'result', 'new_event_id', 'e', 'event_id')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_companies_as_targets'
-         firstlineno 172
+         firstlineno 218
          lnotab
             0x0208400220020403240136023404040104011c02040134012a010a011e
             014e012601020214020a0102020a031801160102ff0e082801280128012a
             fc04f810101801160102ff0e0902010201280102fc04f710141e01020128
             0104013001120132ff08c902ff2eff2e3c1e0108012c01
       code
          argcount  : 0
@@ -1775,53 +2039,53 @@
             00000001006e0b230031007304770278035900770101005900010001007c
             036403190000000000000000006a090000000000000000a00a0000000000
             0000000000000000000000000000006404a6010000ab0100000000000000
             006a0900000000000000006405190000000000000000007c0364063c0000
             007c03640719000000000000000000a00b00000000000000000000000000
             0000000000000064088400a6010000ab0100000000000000007c0364093c
             0000007c035300
-         269           0 RESUME                   0
+         315           0 RESUME                   0
          
-         270           2 LOAD_CONST               1 ("\n    SELECT \n        s.uid,\n        s.label,\n        s.updated,\n        s.meta->>'type' as type,\n        s.meta->>'notes' as notes,\n        s.meta->>'products' as products,\n        s.meta->>'services' as services,\n        s.meta->>'customers' as customers,\n        s.meta->>'end_customer' as end_customer,\n        s.meta->>'last_list' as last_list,\n        s.meta->>'next_due_date' as next_due_date,\n        s.meta->>'geographies' as geographies,\n        s.meta->>'week' as week,\n        s.meta->>'day' as day,\n\n        COALESCE(s.meta->>'search_status', 'active') as search_status\n    FROM search s\n    ORDER BY updated\n    ")
+         316           2 LOAD_CONST               1 ("\n    SELECT \n        s.uid,\n        s.label,\n        s.updated,\n        s.meta->>'type' as type,\n        s.meta->>'notes' as notes,\n        s.meta->>'products' as products,\n        s.meta->>'services' as services,\n        s.meta->>'customers' as customers,\n        s.meta->>'end_customer' as end_customer,\n        s.meta->>'last_list' as last_list,\n        s.meta->>'next_due_date' as next_due_date,\n        s.meta->>'geographies' as geographies,\n        s.meta->>'week' as week,\n        s.meta->>'day' as day,\n\n        COALESCE(s.meta->>'search_status', 'active') as search_status\n    FROM search s\n    ORDER BY updated\n    ")
                        4 STORE_FAST               0 (statement)
          
-         291           6 LOAD_GLOBAL              0 (db)
+         337           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               1 (conn)
          
-         292          58 LOAD_FAST                1 (conn)
+         338          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                0 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         293         136 LOAD_GLOBAL             11 (NULL + pd)
+         339         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         291         252 LOAD_CONST               0 (None)
+         337         252 LOAD_CONST               0 (None)
                      254 LOAD_CONST               0 (None)
                      256 LOAD_CONST               0 (None)
                      258 PRECALL                  2
                      262 CALL                     2
                      272 POP_TOP
                      274 JUMP_FORWARD            11 (to 298)
                  >>  276 PUSH_EXC_INFO
@@ -1832,44 +2096,44 @@
                      286 POP_EXCEPT
                      288 RERAISE                  1
                  >>  290 POP_TOP
                      292 POP_EXCEPT
                      294 POP_TOP
                      296 POP_TOP
          
-         294     >>  298 LOAD_FAST                3 (df)
+         340     >>  298 LOAD_FAST                3 (df)
                      300 LOAD_CONST               3 ('label')
                      302 BINARY_SUBSCR
                      312 LOAD_ATTR                9 (str)
                      322 LOAD_METHOD             10 (split)
                      344 LOAD_CONST               4 (' - ')
                      346 PRECALL                  1
                      350 CALL                     1
                      360 LOAD_ATTR                9 (str)
                      370 LOAD_CONST               5 (0)
                      372 BINARY_SUBSCR
                      382 LOAD_FAST                3 (df)
                      384 LOAD_CONST               6 ('client')
                      386 STORE_SUBSCR
          
-         295         390 LOAD_FAST                3 (df)
+         341         390 LOAD_FAST                3 (df)
                      392 LOAD_CONST               7 ('uid')
                      394 BINARY_SUBSCR
                      404 LOAD_METHOD             11 (apply)
          
-         296         426 LOAD_CONST               8 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 296>)
+         342         426 LOAD_CONST               8 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 342>)
                      428 MAKE_FUNCTION            0
          
-         295         430 PRECALL                  1
+         341         430 PRECALL                  1
                      434 CALL                     1
                      444 LOAD_FAST                3 (df)
                      446 LOAD_CONST               9 ('searchToken')
                      448 STORE_SUBSCR
          
-         298         452 LOAD_FAST                3 (df)
+         344         452 LOAD_FAST                3 (df)
                      454 RETURN_VALUE
          ExceptionTable:
            56 to 250 -> 276 [1] lasti
            276 to 282 -> 284 [3] lasti
            290 to 290 -> 284 [3] lasti
          consts
             None
@@ -1887,15 +2151,15 @@
                flags     : 19
                code
                   0x97007401000000000000000000006a0100000000000000007405000000
                   000000000000007c00a6010000ab010000000000000000a0030000000000
                   0000000000000000000000000000006401a6010000ab0100000000000000
                   00a6010000ab010000000000000000a00400000000000000000000000000
                   00000000000000a6000000ab0000000000000000005300
-               296           0 RESUME                   0
+               342           0 RESUME                   0
                              2 LOAD_GLOBAL              1 (NULL + hashlib)
                             14 LOAD_ATTR                1 (md5)
                             24 LOAD_GLOBAL              5 (NULL + str)
                             36 LOAD_FAST                0 (x)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              3 (encode)
@@ -1913,39 +2177,39 @@
                   'utf-8'
                names      ('hashlib', 'md5', 'str', 'encode', 'hexdigest')
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '<lambda>'
-               firstlineno 296
+               firstlineno 342
                lnotab 0x
             'searchToken'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'str', 'split', 'apply')
          varnames   ('statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'searches_query'
-         firstlineno 269
+         firstlineno 315
          lnotab 0x0201041534014e0174fe2e035c01240104ff1603
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x970064017d007401000000000000000000006a0100000000000000007c
             00740400000000000000000000a6020000ab0200000000000000005300
-         301           0 RESUME                   0
+         347           0 RESUME                   0
          
-         302           2 LOAD_CONST               1 ('\n       SELECT\n        search_uid,\n        AVG(rating::int) AS rating_avg,\n        COUNT(rating) as rating_count\n    FROM rating \n    GROUP BY search_uid\n    ')
+         348           2 LOAD_CONST               1 ('\n       SELECT\n        search_uid,\n        AVG(rating::int) AS rating_avg,\n        COUNT(rating) as rating_count\n    FROM rating \n    GROUP BY search_uid\n    ')
                        4 STORE_FAST               0 (query)
          
-         310           6 LOAD_GLOBAL              1 (NULL + pd)
+         356           6 LOAD_GLOBAL              1 (NULL + pd)
                       18 LOAD_ATTR                1 (read_sql)
                       28 LOAD_FAST                0 (query)
                       30 LOAD_GLOBAL              4 (db)
                       42 PRECALL                  2
                       46 CALL                     2
                       56 RETURN_VALUE
          consts
@@ -1953,15 +2217,15 @@
             '\n       SELECT\n        search_uid,\n        AVG(rating::int) AS rating_avg,\n        COUNT(rating) as rating_count\n    FROM rating \n    GROUP BY search_uid\n    '
          names      ('pd', 'read_sql', 'db')
          varnames   ('query',)
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'average_rating_per_search_query'
-         firstlineno 301
+         firstlineno 347
          lnotab 0x02010408
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -1973,66 +2237,66 @@
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d037413000000000000000000007c03640319
             00000000000000000064047a0b00006405a6020000ab0200000000000000
             007c0364063c000000640064006400a6020000ab02000000000000000001
             006e0b230031007304770278035900770101005900010001007c035300
-         313           0 RESUME                   0
+         359           0 RESUME                   0
          
-         314           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT\n            e.search_uid,\n            a.name as analyst,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 1 * 86400 THEN 1 ELSE 0 END) AS last_1_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 7 * 86400 THEN 1 ELSE 0 END) AS last_7_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400 THEN 1 ELSE 0 END) AS last_30_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) AS last_90_days,\n            SUM(CASE WHEN e.type = 'validate' THEN 1 ELSE 0 END) AS total_validations,\n            RANK() OVER (PARTITION BY e.search_uid ORDER BY SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) DESC) as rank\n        FROM\n            event e\n        LEFT JOIN\n            actor a ON a.key = e.actor_key\n        WHERE\n            e.type = 'validate'\n        GROUP BY\n            e.search_uid, analyst\n    )\n    SELECT\n        search_uid,\n        analyst,\n        last_1_days,\n        last_7_days,\n        last_30_days,\n        last_90_days,\n        total_validations\n    FROM\n        RankedEvents\n    WHERE\n        rank = 1\n        AND last_90_days > 0\n    ;\n    ")
+         360           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT\n            e.search_uid,\n            a.name as analyst,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 1 * 86400 THEN 1 ELSE 0 END) AS last_1_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 7 * 86400 THEN 1 ELSE 0 END) AS last_7_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400 THEN 1 ELSE 0 END) AS last_30_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) AS last_90_days,\n            SUM(CASE WHEN e.type = 'validate' THEN 1 ELSE 0 END) AS total_validations,\n            RANK() OVER (PARTITION BY e.search_uid ORDER BY SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) DESC) as rank\n        FROM\n            event e\n        LEFT JOIN\n            actor a ON a.key = e.actor_key\n        WHERE\n            e.type = 'validate'\n        GROUP BY\n            e.search_uid, analyst\n    )\n    SELECT\n        search_uid,\n        analyst,\n        last_1_days,\n        last_7_days,\n        last_30_days,\n        last_90_days,\n        total_validations\n    FROM\n        RankedEvents\n    WHERE\n        rank = 1\n        AND last_90_days > 0\n    ;\n    ")
                        4 STORE_FAST               0 (stmt)
          
-         349           6 LOAD_GLOBAL              0 (db)
+         395           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               1 (conn)
          
-         350          58 LOAD_FAST                1 (conn)
+         396          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                0 (stmt)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         351         136 LOAD_GLOBAL             11 (NULL + pd)
+         397         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         352         252 LOAD_GLOBAL             19 (NULL + round)
+         398         252 LOAD_GLOBAL             19 (NULL + round)
                      264 LOAD_FAST                3 (df)
                      266 LOAD_CONST               3 ('total_validations')
                      268 BINARY_SUBSCR
                      278 LOAD_CONST               4 (300)
                      280 BINARY_OP               11 (/)
                      284 LOAD_CONST               5 (2)
                      286 PRECALL                  2
                      290 CALL                     2
                      300 LOAD_FAST                3 (df)
                      302 LOAD_CONST               6 ('total_validations_pct')
                      304 STORE_SUBSCR
          
-         349         308 LOAD_CONST               0 (None)
+         395         308 LOAD_CONST               0 (None)
                      310 LOAD_CONST               0 (None)
                      312 LOAD_CONST               0 (None)
                      314 PRECALL                  2
                      318 CALL                     2
                      328 POP_TOP
                      330 JUMP_FORWARD            11 (to 354)
                  >>  332 PUSH_EXC_INFO
@@ -2043,15 +2307,15 @@
                      342 POP_EXCEPT
                      344 RERAISE                  1
                  >>  346 POP_TOP
                      348 POP_EXCEPT
                      350 POP_TOP
                      352 POP_TOP
          
-         353     >>  354 LOAD_FAST                3 (df)
+         399     >>  354 LOAD_FAST                3 (df)
                      356 RETURN_VALUE
          ExceptionTable:
            56 to 306 -> 332 [1] lasti
            332 to 338 -> 340 [3] lasti
            346 to 346 -> 340 [3] lasti
          consts
             None
@@ -2063,15 +2327,15 @@
             'total_validations_pct'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'round')
          varnames   ('stmt', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'validation_history'
-         firstlineno 313
+         firstlineno 359
          lnotab 0x0201042334014e01740138fd2e04
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -2082,53 +2346,53 @@
             00a6010000ab0100000000000000007d02740b000000000000000000006a
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d03640064006400a6020000ab020000000000
             00000001006e0b230031007304770278035900770101005900010001007c
             035300
-         356           0 RESUME                   0
+         402           0 RESUME                   0
          
-         357           2 LOAD_CONST               1 ("\n        SELECT \n            e.search_uid as uid,\n            COUNT(*) as comment_count\n        FROM event e\n        WHERE \n            e.type = 'comment'\n            AND e.domain is null\n            -- last 30 days\n            AND e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400\n        GROUP BY e.search_uid\n        ")
+         403           2 LOAD_CONST               1 ("\n        SELECT \n            e.search_uid as uid,\n            COUNT(*) as comment_count\n        FROM event e\n        WHERE \n            e.type = 'comment'\n            AND e.domain is null\n            -- last 30 days\n            AND e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400\n        GROUP BY e.search_uid\n        ")
                        4 STORE_FAST               0 (statement)
          
-         369           6 LOAD_GLOBAL              0 (db)
+         415           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               1 (conn)
          
-         370          58 LOAD_FAST                1 (conn)
+         416          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                0 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         371         136 LOAD_GLOBAL             11 (NULL + pd)
+         417         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         369         252 LOAD_CONST               0 (None)
+         415         252 LOAD_CONST               0 (None)
                      254 LOAD_CONST               0 (None)
                      256 LOAD_CONST               0 (None)
                      258 PRECALL                  2
                      262 CALL                     2
                      272 POP_TOP
                      274 JUMP_FORWARD            11 (to 298)
                  >>  276 PUSH_EXC_INFO
@@ -2139,15 +2403,15 @@
                      286 POP_EXCEPT
                      288 RERAISE                  1
                  >>  290 POP_TOP
                      292 POP_EXCEPT
                      294 POP_TOP
                      296 POP_TOP
          
-         373     >>  298 LOAD_FAST                3 (df)
+         419     >>  298 LOAD_FAST                3 (df)
                      300 RETURN_VALUE
          ExceptionTable:
            56 to 250 -> 276 [1] lasti
            276 to 282 -> 284 [3] lasti
            290 to 290 -> 284 [3] lasti
          consts
             None
@@ -2155,15 +2419,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'searches_comment_counts'
-         firstlineno 356
+         firstlineno 402
          lnotab 0x0201040c34014e0174fe2e04
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
@@ -2180,107 +2444,107 @@
             000000a00300000000000000000000000000000000000000006406a60100
             00ab0100000000000000007c0264093c0000007c02a00200000000000000
             00000000000000000000000000740900000000000000000000a6000000ab
             00000000000000000064016403ac0aa6030000ab0300000000000000007d
             027c02640b19000000000000000000a00300000000000000000000000000
             000000000000006406a6010000ab0100000000000000007c02640b3c0000
             007c025300
-         376           0 RESUME                   0
+         422           0 RESUME                   0
          
-         377           2 LOAD_GLOBAL              1 (NULL + searches_query)
+         423           2 LOAD_GLOBAL              1 (NULL + searches_query)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               0 (searches)
          
-         379          30 LOAD_GLOBAL              3 (NULL + validation_history)
+         425          30 LOAD_GLOBAL              3 (NULL + validation_history)
                       42 PRECALL                  0
                       46 CALL                     0
                       56 STORE_FAST               1 (recent_event_count)
          
-         381          58 LOAD_FAST                0 (searches)
+         427          58 LOAD_FAST                0 (searches)
                       60 LOAD_METHOD              2 (merge)
          
-         382          82 LOAD_FAST                1 (recent_event_count)
+         428          82 LOAD_FAST                1 (recent_event_count)
                       84 LOAD_CONST               1 ('uid')
                       86 LOAD_CONST               2 ('search_uid')
                       88 LOAD_CONST               3 ('left')
          
-         381          90 KW_NAMES                 4
+         427          90 KW_NAMES                 4
                       92 PRECALL                  4
                       96 CALL                     4
                      106 STORE_FAST               2 (df)
          
-         385         108 LOAD_FAST                2 (df)
+         431         108 LOAD_FAST                2 (df)
                      110 LOAD_CONST               5 ('last_1_days')
                      112 BINARY_SUBSCR
                      122 LOAD_METHOD              3 (fillna)
                      144 LOAD_CONST               6 (0)
                      146 PRECALL                  1
                      150 CALL                     1
                      160 LOAD_FAST                2 (df)
                      162 LOAD_CONST               5 ('last_1_days')
                      164 STORE_SUBSCR
          
-         386         168 LOAD_FAST                2 (df)
+         432         168 LOAD_FAST                2 (df)
                      170 LOAD_CONST               7 ('last_7_days')
                      172 BINARY_SUBSCR
                      182 LOAD_METHOD              3 (fillna)
                      204 LOAD_CONST               6 (0)
                      206 PRECALL                  1
                      210 CALL                     1
                      220 LOAD_FAST                2 (df)
                      222 LOAD_CONST               7 ('last_7_days')
                      224 STORE_SUBSCR
          
-         387         228 LOAD_FAST                2 (df)
+         433         228 LOAD_FAST                2 (df)
                      230 LOAD_CONST               8 ('last_30_days')
                      232 BINARY_SUBSCR
                      242 LOAD_METHOD              3 (fillna)
                      264 LOAD_CONST               6 (0)
                      266 PRECALL                  1
                      270 CALL                     1
                      280 LOAD_FAST                2 (df)
                      282 LOAD_CONST               8 ('last_30_days')
                      284 STORE_SUBSCR
          
-         388         288 LOAD_FAST                2 (df)
+         434         288 LOAD_FAST                2 (df)
                      290 LOAD_CONST               9 ('last_90_days')
                      292 BINARY_SUBSCR
                      302 LOAD_METHOD              3 (fillna)
                      324 LOAD_CONST               6 (0)
                      326 PRECALL                  1
                      330 CALL                     1
                      340 LOAD_FAST                2 (df)
                      342 LOAD_CONST               9 ('last_90_days')
                      344 STORE_SUBSCR
          
-         390         348 LOAD_FAST                2 (df)
+         436         348 LOAD_FAST                2 (df)
                      350 LOAD_METHOD              2 (merge)
                      372 LOAD_GLOBAL              9 (NULL + searches_comment_counts)
                      384 PRECALL                  0
                      388 CALL                     0
                      398 LOAD_CONST               1 ('uid')
                      400 LOAD_CONST               3 ('left')
                      402 KW_NAMES                10
                      404 PRECALL                  3
                      408 CALL                     3
                      418 STORE_FAST               2 (df)
          
-         391         420 LOAD_FAST                2 (df)
+         437         420 LOAD_FAST                2 (df)
                      422 LOAD_CONST              11 ('comment_count')
                      424 BINARY_SUBSCR
                      434 LOAD_METHOD              3 (fillna)
                      456 LOAD_CONST               6 (0)
                      458 PRECALL                  1
                      462 CALL                     1
                      472 LOAD_FAST                2 (df)
                      474 LOAD_CONST              11 ('comment_count')
                      476 STORE_SUBSCR
          
-         393         480 LOAD_FAST                2 (df)
+         439         480 LOAD_FAST                2 (df)
                      482 RETURN_VALUE
          consts
             None
             'uid'
             'search_uid'
             'left'
             ('left_on', 'right_on', 'how')
@@ -2293,15 +2557,15 @@
             'comment_count'
          names      ('searches_query', 'validation_history', 'merge', 'fillna', 'searches_comment_counts')
          varnames   ('searches', 'recent_event_count', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'enriched_searches_query'
-         firstlineno 376
+         firstlineno 422
          lnotab 0x02011c021c02180108ff12043c013c013c013c0248013c02
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
@@ -2313,66 +2577,66 @@
             00000000007c01a0070000000000000000000000000000000000000000a6
             000000ab0000000000000000007c01a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000ac02a6020000ab0200
             000000000000007d027c02a0090000000000000000000000000000000000
             00000067006403a201ac02a6010000ab0100000000000000007d027c0263
             02640064006400a6020000ab020000000000000000010053002300310073
             047702780359007701010059000100010064005300
-         396           0 RESUME                   0
+         442           0 RESUME                   0
          
-         397           2 LOAD_GLOBAL              0 (db)
+         443           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         398          54 LOAD_FAST                0 (conn)
+         444          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         399          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         445          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         400         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
+         446         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
          
-         399         102 PRECALL                  1
+         445         102 PRECALL                  1
                      106 CALL                     1
          
-         398         116 PRECALL                  1
+         444         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         405         132 LOAD_GLOBAL             11 (NULL + pd)
+         451         132 LOAD_GLOBAL             11 (NULL + pd)
                      144 LOAD_ATTR                6 (DataFrame)
                      154 LOAD_FAST                1 (result)
                      156 LOAD_METHOD              7 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                1 (result)
                      194 LOAD_METHOD              8 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 2
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               2 (df)
          
-         406         248 LOAD_FAST                2 (df)
+         452         248 LOAD_FAST                2 (df)
                      250 LOAD_METHOD              9 (drop)
                      272 BUILD_LIST               0
                      274 LOAD_CONST               3 (('id', 'created', 'updated'))
                      276 LIST_EXTEND              1
                      278 KW_NAMES                 2
                      280 PRECALL                  1
                      284 CALL                     1
                      294 STORE_FAST               2 (df)
          
-         407         296 LOAD_FAST                2 (df)
+         453         296 LOAD_FAST                2 (df)
          
-         397         298 SWAP                     2
+         443         298 SWAP                     2
                      300 LOAD_CONST               0 (None)
                      302 LOAD_CONST               0 (None)
                      304 LOAD_CONST               0 (None)
                      306 PRECALL                  2
                      310 CALL                     2
                      320 POP_TOP
                      322 RETURN_VALUE
@@ -2400,15 +2664,15 @@
             ('id', 'created', 'updated')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'drop')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'actor'
-         firstlineno 396
+         firstlineno 442
          lnotab 0x020134011801160102ff0eff10077401300102f6
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -2421,54 +2685,54 @@
             000000ab0000000000000000007c01a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000ac02a6020000ab0200
             000000000000007d02640064006400a6020000ab02000000000000000001
             006e0b23003100730477027803590077010100590001000100640384007d
             037c02640419000000000000000000a00900000000000000000000000000
             000000000000007c03a6010000ab0100000000000000007c0264053c0000
             007c025300
-         410           0 RESUME                   0
+         456           0 RESUME                   0
          
-         411           2 LOAD_GLOBAL              0 (db)
+         457           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         412          54 LOAD_FAST                0 (conn)
+         458          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         413          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         459          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         414         100 LOAD_CONST               1 ("\n                SELECT \n                    e.id,\n                    e.domain,\n                    e.created as updated,\n                    a.name as updated_by, \n                    to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n                    c.name, \n                    c.description,\n                    c.source,\n                    c.meta->>'ownership' as ownership, \n                    c.meta->>'headquarters' as headquarters,\n                    c.meta->>'city' as city,\n                    c.meta->>'state' as state,\n                    c.meta->>'designation' as designation,\n                    c.meta->>'products' as products,\n                    c.meta->>'services' as services,\n                    c.meta->>'end_customer' as end_customer,\n                    c.meta->>'geographies' as geographies,\n                    c.meta->>'was_acquired' as was_acquired,\n                    c.meta->>'justification' as justification,\n                    c.meta->>'year_founded' as year_founded,\n                    c.meta->>'linkedin' as linkedin,\n                    c.meta->>'linkedin_range' as linkedin_range,\n                    c.meta->>'primary_contact' as primary_contact,\n                    c.meta->>'industry' as industry,\n                    c.meta->>'revenue_estimates' as revenue_estimates,\n                    c.meta->>'location_count' as location_count,\n                    c.meta->>'business_models' as business_models,\n                    c.meta->>'facility_size' as facility_size,\n                    c.meta,\n                    COALESCE(co.comments, '[]'::jsonb) as comments\n                FROM event e\n                LEFT JOIN actor a ON e.actor_key = a.key\n                LEFT JOIN company c ON e.domain = c.domain\n                LEFT JOIN comment co ON e.domain = co.domain\n                WHERE e.type = 'buyer'\n                ")
+         460         100 LOAD_CONST               1 ("\n                SELECT \n                    e.id,\n                    e.domain,\n                    e.created as updated,\n                    a.name as updated_by, \n                    to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n                    c.name, \n                    c.description,\n                    c.source,\n                    c.meta->>'ownership' as ownership, \n                    c.meta->>'headquarters' as headquarters,\n                    c.meta->>'city' as city,\n                    c.meta->>'state' as state,\n                    c.meta->>'designation' as designation,\n                    c.meta->>'products' as products,\n                    c.meta->>'services' as services,\n                    c.meta->>'end_customer' as end_customer,\n                    c.meta->>'geographies' as geographies,\n                    c.meta->>'was_acquired' as was_acquired,\n                    c.meta->>'justification' as justification,\n                    c.meta->>'year_founded' as year_founded,\n                    c.meta->>'linkedin' as linkedin,\n                    c.meta->>'linkedin_range' as linkedin_range,\n                    c.meta->>'primary_contact' as primary_contact,\n                    c.meta->>'industry' as industry,\n                    c.meta->>'revenue_estimates' as revenue_estimates,\n                    c.meta->>'location_count' as location_count,\n                    c.meta->>'business_models' as business_models,\n                    c.meta->>'facility_size' as facility_size,\n                    c.meta,\n                    COALESCE(co.comments, '[]'::jsonb) as comments\n                FROM event e\n                LEFT JOIN actor a ON e.actor_key = a.key\n                LEFT JOIN company c ON e.domain = c.domain\n                LEFT JOIN comment co ON e.domain = co.domain\n                WHERE e.type = 'buyer'\n                ")
          
-         413         102 PRECALL                  1
+         459         102 PRECALL                  1
                      106 CALL                     1
          
-         412         116 PRECALL                  1
+         458         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         454         132 LOAD_GLOBAL             11 (NULL + pd)
+         500         132 LOAD_GLOBAL             11 (NULL + pd)
                      144 LOAD_ATTR                6 (DataFrame)
                      154 LOAD_FAST                1 (result)
                      156 LOAD_METHOD              7 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                1 (result)
                      194 LOAD_METHOD              8 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 2
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               2 (df)
          
-         411         248 LOAD_CONST               0 (None)
+         457         248 LOAD_CONST               0 (None)
                      250 LOAD_CONST               0 (None)
                      252 LOAD_CONST               0 (None)
                      254 PRECALL                  2
                      258 CALL                     2
                      268 POP_TOP
                      270 JUMP_FORWARD            11 (to 294)
                  >>  272 PUSH_EXC_INFO
@@ -2479,30 +2743,30 @@
                      282 POP_EXCEPT
                      284 RERAISE                  1
                  >>  286 POP_TOP
                      288 POP_EXCEPT
                      290 POP_TOP
                      292 POP_TOP
          
-         456     >>  294 LOAD_CONST               3 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 456>)
+         502     >>  294 LOAD_CONST               3 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 502>)
                      296 MAKE_FUNCTION            0
                      298 STORE_FAST               3 (get_employees)
          
-         468         300 LOAD_FAST                2 (df)
+         514         300 LOAD_FAST                2 (df)
                      302 LOAD_CONST               4 ('meta')
                      304 BINARY_SUBSCR
                      314 LOAD_METHOD              9 (apply)
                      336 LOAD_FAST                3 (get_employees)
                      338 PRECALL                  1
                      342 CALL                     1
                      352 LOAD_FAST                2 (df)
                      354 LOAD_CONST               5 ('employees')
                      356 STORE_SUBSCR
          
-         469         360 LOAD_FAST                2 (df)
+         515         360 LOAD_FAST                2 (df)
                      362 RETURN_VALUE
          ExceptionTable:
            52 to 246 -> 272 [1] lasti
            272 to 278 -> 280 [3] lasti
            286 to 286 -> 280 [3] lasti
          consts
             None
@@ -2517,60 +2781,60 @@
                   0x97007c00a00000000000000000000000000000000000000000006401a6
                   010000ab010000000000000000721e09007403000000000000000000007c
                   00640119000000000000000000a6010000ab010000000000000000530023
                   0001005900640053007803590077017c00a0000000000000000000000000
                   0000000000000000006402a6010000ab010000000000000000721b7c0064
                   0219000000000000000000a0000000000000000000000000000000000000
                   0000006403a6010000ab010000000000000000530064005300
-               456           0 RESUME                   0
+               502           0 RESUME                   0
                
-               457           2 LOAD_FAST                0 (meta)
+               503           2 LOAD_FAST                0 (meta)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('employees')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE    30 (to 104)
                
-               459          44 NOP
+               505          44 NOP
                
-               460          46 LOAD_GLOBAL              3 (NULL + int)
+               506          46 LOAD_GLOBAL              3 (NULL + int)
                             58 LOAD_FAST                0 (meta)
                             60 LOAD_CONST               1 ('employees')
                             62 BINARY_SUBSCR
                             72 PRECALL                  1
                             76 CALL                     1
                             86 RETURN_VALUE
                        >>   88 PUSH_EXC_INFO
                
-               461          90 POP_TOP
+               507          90 POP_TOP
                
-               462          92 POP_EXCEPT
+               508          92 POP_EXCEPT
                             94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                        >>   98 COPY                     3
                            100 POP_EXCEPT
                            102 RERAISE                  1
                
-               463     >>  104 LOAD_FAST                0 (meta)
+               509     >>  104 LOAD_FAST                0 (meta)
                            106 LOAD_METHOD              0 (get)
                            128 LOAD_CONST               2 ('grata_employee_estimates')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 POP_JUMP_FORWARD_IF_FALSE    27 (to 200)
                
-               464         146 LOAD_FAST                0 (meta)
+               510         146 LOAD_FAST                0 (meta)
                            148 LOAD_CONST               2 ('grata_employee_estimates')
                            150 BINARY_SUBSCR
                            160 LOAD_METHOD              0 (get)
                            182 LOAD_CONST               3 ('count')
                            184 PRECALL                  1
                            188 CALL                     1
                            198 RETURN_VALUE
                
-               466     >>  200 LOAD_CONST               0 (None)
+               512     >>  200 LOAD_CONST               0 (None)
                            202 RETURN_VALUE
                ExceptionTable:
                  46 to 84 -> 88 [0]
                  88 to 90 -> 98 [1] lasti
                consts
                   None
                   'employees'
@@ -2578,25 +2842,25 @@
                   'count'
                names      ('get', 'int')
                varnames   ('meta',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_employees'
-               firstlineno 456
+               firstlineno 502
                lnotab 0x02012a0202012c0102010c012a013602
             'meta'
             'employees'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'apply')
          varnames   ('conn', 'result', 'df', 'get_employees')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'buyer'
-         firstlineno 410
+         firstlineno 456
          lnotab 0x020134011801160102ff0eff102a74d52e2d060c3c01
       code
          argcount  : 1
          nlocals   : 10
          stacksize : 6
          flags     : 3
          code
@@ -2618,59 +2882,59 @@
             010000ab0100000000000000007c04640c3c0000007c04640d1900000000
             0000000000a00a00000000000000000000000000000000000000007c07a6
             010000ab0100000000000000007c04640d3c0000007c04a00a0000000000
             0000000000000000000000000000007c08640eac0fa6020000ab02000000
             00000000007c0464103c0000007c04a00a00000000000000000000000000
             000000000000007c09640eac0fa6020000ab0200000000000000007c0464
             113c0000007c045300
-         507           0 RESUME                   0
+         553           0 RESUME                   0
          
-         510           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute','enrich')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        -- c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n        AND e.domain != ''\n    ;\n    ")
+         556           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute','enrich')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        -- c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n        AND e.domain != ''\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
-         574           6 LOAD_GLOBAL              0 (db)
+         620           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         575          58 LOAD_FAST                2 (conn)
+         621          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         576          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         622          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         577         120 LOAD_CONST               2 ('search_uid')
+         623         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         575         126 PRECALL                  2
+         621         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         579         142 LOAD_GLOBAL             11 (NULL + pd)
+         625         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         574         258 LOAD_CONST               0 (None)
+         620         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2681,93 +2945,93 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         581     >>  304 LOAD_CONST               4 ('return')
+         627     >>  304 LOAD_CONST               4 ('return')
                      306 LOAD_GLOBAL             18 (str)
                      318 BUILD_TUPLE              2
-                     320 LOAD_CONST               5 (<code object list_to_csv, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 581>)
+                     320 LOAD_CONST               5 (<code object list_to_csv, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 627>)
                      322 MAKE_FUNCTION            4 (annotations)
                      324 STORE_FAST               5 (list_to_csv)
          
-         593         326 LOAD_CONST               6 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 593>)
+         639         326 LOAD_CONST               6 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 639>)
                      328 MAKE_FUNCTION            0
                      330 STORE_FAST               6 (get_employees)
          
-         605         332 LOAD_CONST               7 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 605>)
+         651         332 LOAD_CONST               7 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 651>)
                      334 MAKE_FUNCTION            0
                      336 STORE_FAST               7 (get_ownership)
          
-         613         338 LOAD_CONST               8 (<code object get_state, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 613>)
+         659         338 LOAD_CONST               8 (<code object get_state, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 659>)
                      340 MAKE_FUNCTION            0
                      342 STORE_FAST               8 (get_state)
          
-         623         344 LOAD_CONST               9 (<code object get_city, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 623>)
+         669         344 LOAD_CONST               9 (<code object get_city, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 669>)
                      346 MAKE_FUNCTION            0
                      348 STORE_FAST               9 (get_city)
          
-         632         350 LOAD_FAST                4 (df)
+         678         350 LOAD_FAST                4 (df)
                      352 LOAD_CONST              10 ('end_customer')
                      354 BINARY_SUBSCR
                      364 LOAD_METHOD             10 (apply)
                      386 LOAD_FAST                5 (list_to_csv)
                      388 PRECALL                  1
                      392 CALL                     1
                      402 LOAD_FAST                4 (df)
                      404 LOAD_CONST              10 ('end_customer')
                      406 STORE_SUBSCR
          
-         633         410 LOAD_FAST                4 (df)
+         679         410 LOAD_FAST                4 (df)
                      412 LOAD_CONST              11 ('meta')
                      414 BINARY_SUBSCR
                      424 LOAD_METHOD             10 (apply)
                      446 LOAD_FAST                6 (get_employees)
                      448 PRECALL                  1
                      452 CALL                     1
                      462 LOAD_FAST                4 (df)
                      464 LOAD_CONST              12 ('employees')
                      466 STORE_SUBSCR
          
-         634         470 LOAD_FAST                4 (df)
+         680         470 LOAD_FAST                4 (df)
                      472 LOAD_CONST              13 ('ownership')
                      474 BINARY_SUBSCR
                      484 LOAD_METHOD             10 (apply)
                      506 LOAD_FAST                7 (get_ownership)
                      508 PRECALL                  1
                      512 CALL                     1
                      522 LOAD_FAST                4 (df)
                      524 LOAD_CONST              13 ('ownership')
                      526 STORE_SUBSCR
          
-         635         530 LOAD_FAST                4 (df)
+         681         530 LOAD_FAST                4 (df)
                      532 LOAD_METHOD             10 (apply)
                      554 LOAD_FAST                8 (get_state)
                      556 LOAD_CONST              14 (1)
                      558 KW_NAMES                15
                      560 PRECALL                  2
                      564 CALL                     2
                      574 LOAD_FAST                4 (df)
                      576 LOAD_CONST              16 ('state')
                      578 STORE_SUBSCR
          
-         636         582 LOAD_FAST                4 (df)
+         682         582 LOAD_FAST                4 (df)
                      584 LOAD_METHOD             10 (apply)
                      606 LOAD_FAST                9 (get_city)
                      608 LOAD_CONST              14 (1)
                      610 KW_NAMES                15
                      612 PRECALL                  2
                      616 CALL                     2
                      626 LOAD_FAST                4 (df)
                      628 LOAD_CONST              17 ('city')
                      630 STORE_SUBSCR
          
-         638         634 LOAD_FAST                4 (df)
+         684         634 LOAD_FAST                4 (df)
                      636 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2781,39 +3045,39 @@
                stacksize : 4
                flags     : 19
                code
                   0x970009007401000000000000000000006a0100000000000000007c00a6
                   010000ab0100000000000000007d016401a0020000000000000000000000
                   0000000000000000007c01a6010000ab0100000000000000007d027c0253
                   0023000100590064025300780359007701
-               581           0 RESUME                   0
+               627           0 RESUME                   0
                
-               583           2 NOP
+               629           2 NOP
                
-               584           4 LOAD_GLOBAL              1 (NULL + json)
+               630           4 LOAD_GLOBAL              1 (NULL + json)
                             16 LOAD_ATTR                1 (loads)
                             26 LOAD_FAST                0 (list_str)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 STORE_FAST               1 (list_data)
                
-               587          44 LOAD_CONST               1 (', ')
+               633          44 LOAD_CONST               1 (', ')
                             46 LOAD_METHOD              2 (join)
                             68 LOAD_FAST                1 (list_data)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 STORE_FAST               2 (csv_str)
                
-               589          86 LOAD_FAST                2 (csv_str)
+               635          86 LOAD_FAST                2 (csv_str)
                             88 RETURN_VALUE
                        >>   90 PUSH_EXC_INFO
                
-               590          92 POP_TOP
+               636          92 POP_TOP
                
-               591          94 POP_EXCEPT
+               637          94 POP_EXCEPT
                             96 LOAD_CONST               2 ('')
                             98 RETURN_VALUE
                        >>  100 COPY                     3
                            102 POP_EXCEPT
                            104 RERAISE                  1
                ExceptionTable:
                  4 to 86 -> 90 [0]
@@ -2824,75 +3088,75 @@
                   ''
                names      ('json', 'loads', 'join')
                varnames   ('list_str', 'list_data', 'csv_str')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'list_to_csv'
-               firstlineno 581
+               firstlineno 627
                lnotab 0x0202020128032a0206010201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 19
                code
                   0x97007c00a00000000000000000000000000000000000000000006401a6
                   010000ab010000000000000000721e09007403000000000000000000007c
                   00640119000000000000000000a6010000ab010000000000000000530023
                   0001005900640053007803590077017c00a0000000000000000000000000
                   0000000000000000006402a6010000ab010000000000000000721b7c0064
                   0219000000000000000000a0000000000000000000000000000000000000
                   0000006403a6010000ab010000000000000000530064005300
-               593           0 RESUME                   0
+               639           0 RESUME                   0
                
-               594           2 LOAD_FAST                0 (meta)
+               640           2 LOAD_FAST                0 (meta)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('employees')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE    30 (to 104)
                
-               596          44 NOP
+               642          44 NOP
                
-               597          46 LOAD_GLOBAL              3 (NULL + int)
+               643          46 LOAD_GLOBAL              3 (NULL + int)
                             58 LOAD_FAST                0 (meta)
                             60 LOAD_CONST               1 ('employees')
                             62 BINARY_SUBSCR
                             72 PRECALL                  1
                             76 CALL                     1
                             86 RETURN_VALUE
                        >>   88 PUSH_EXC_INFO
                
-               598          90 POP_TOP
+               644          90 POP_TOP
                
-               599          92 POP_EXCEPT
+               645          92 POP_EXCEPT
                             94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                        >>   98 COPY                     3
                            100 POP_EXCEPT
                            102 RERAISE                  1
                
-               600     >>  104 LOAD_FAST                0 (meta)
+               646     >>  104 LOAD_FAST                0 (meta)
                            106 LOAD_METHOD              0 (get)
                            128 LOAD_CONST               2 ('grata_employee_estimates')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 POP_JUMP_FORWARD_IF_FALSE    27 (to 200)
                
-               601         146 LOAD_FAST                0 (meta)
+               647         146 LOAD_FAST                0 (meta)
                            148 LOAD_CONST               2 ('grata_employee_estimates')
                            150 BINARY_SUBSCR
                            160 LOAD_METHOD              0 (get)
                            182 LOAD_CONST               3 ('count')
                            184 PRECALL                  1
                            188 CALL                     1
                            198 RETURN_VALUE
                
-               603     >>  200 LOAD_CONST               0 (None)
+               649     >>  200 LOAD_CONST               0 (None)
                            202 RETURN_VALUE
                ExceptionTable:
                  46 to 84 -> 88 [0]
                  88 to 90 -> 98 [1] lasti
                consts
                   None
                   'employees'
@@ -2900,57 +3164,57 @@
                   'count'
                names      ('get', 'int')
                varnames   ('meta',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_employees'
-               firstlineno 593
+               firstlineno 639
                lnotab 0x02012a0202012c0102010c012a013602
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 19
                code
                   0x97007c0064016b02000000007202640253007c0064036b020000000072
                   02640453007c005300
-               605           0 RESUME                   0
+               651           0 RESUME                   0
                
-               606           2 LOAD_FAST                0 (ownership)
+               652           2 LOAD_FAST                0 (ownership)
                              4 LOAD_CONST               1 ('Bootstrapped')
                              6 COMPARE_OP               2 (==)
                             12 POP_JUMP_FORWARD_IF_FALSE     2 (to 18)
                
-               607          14 LOAD_CONST               2 ('Private')
+               653          14 LOAD_CONST               2 ('Private')
                             16 RETURN_VALUE
                
-               608     >>   18 LOAD_FAST                0 (ownership)
+               654     >>   18 LOAD_FAST                0 (ownership)
                             20 LOAD_CONST               3 ('Investor Backed')
                             22 COMPARE_OP               2 (==)
                             28 POP_JUMP_FORWARD_IF_FALSE     2 (to 34)
                
-               609          30 LOAD_CONST               4 ('Venture Capital')
+               655          30 LOAD_CONST               4 ('Venture Capital')
                             32 RETURN_VALUE
                
-               611     >>   34 LOAD_FAST                0 (ownership)
+               657     >>   34 LOAD_FAST                0 (ownership)
                             36 RETURN_VALUE
                consts
                   None
                   'Bootstrapped'
                   'Private'
                   'Investor Backed'
                   'Venture Capital'
                names      ()
                varnames   ('ownership',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_ownership'
-               firstlineno 605
+               firstlineno 651
                lnotab 0x02010c0104010c010402
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 19
                code
@@ -2960,78 +3224,78 @@
                   00ab010000000000000000725a7c00640219000000000000000000a00100
                   000000000000000000000000000000000000006403a6010000ab01000000
                   0000000000640419000000000000000000a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d017406000000
                   000000000000006a0400000000000000006a050000000000000000a00000
                   000000000000000000000000000000000000007c016405a6020000ab0200
                   000000000000007d027c02530064005300
-               613           0 RESUME                   0
+               659           0 RESUME                   0
                
-               614           2 LOAD_FAST                0 (row)
+               660           2 LOAD_FAST                0 (row)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('state')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE     8 (to 60)
                
-               615          44 LOAD_FAST                0 (row)
+               661          44 LOAD_FAST                0 (row)
                             46 LOAD_CONST               1 ('state')
                             48 BINARY_SUBSCR
                             58 RETURN_VALUE
                
-               616     >>   60 LOAD_FAST                0 (row)
+               662     >>   60 LOAD_FAST                0 (row)
                             62 LOAD_METHOD              0 (get)
                             84 LOAD_CONST               2 ('headquarters')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_JUMP_FORWARD_IF_FALSE    90 (to 282)
                
-               617         102 LOAD_FAST                0 (row)
+               663         102 LOAD_FAST                0 (row)
                            104 LOAD_CONST               2 ('headquarters')
                            106 BINARY_SUBSCR
                            116 LOAD_METHOD              1 (split)
                            138 LOAD_CONST               3 (',')
                            140 PRECALL                  1
                            144 CALL                     1
                            154 LOAD_CONST               4 (-1)
                            156 BINARY_SUBSCR
                            166 LOAD_METHOD              2 (strip)
                            188 PRECALL                  0
                            192 CALL                     0
                            202 STORE_FAST               1 (state_name)
                
-               618         204 LOAD_GLOBAL              6 (ts)
+               664         204 LOAD_GLOBAL              6 (ts)
                            216 LOAD_ATTR                4 (constants)
                            226 LOAD_ATTR                5 (STATE_NAMES)
                            236 LOAD_METHOD              0 (get)
                            258 LOAD_FAST                1 (state_name)
                            260 LOAD_CONST               5 ('')
                            262 PRECALL                  2
                            266 CALL                     2
                            276 STORE_FAST               2 (state_code)
                
-               619         278 LOAD_FAST                2 (state_code)
+               665         278 LOAD_FAST                2 (state_code)
                            280 RETURN_VALUE
                
-               621     >>  282 LOAD_CONST               0 (None)
+               667     >>  282 LOAD_CONST               0 (None)
                            284 RETURN_VALUE
                consts
                   None
                   'state'
                   'headquarters'
                   ','
                   -1
                   ''
                names      ('get', 'split', 'strip', 'ts', 'constants', 'STATE_NAMES')
                varnames   ('row', 'state_name', 'state_code')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_state'
-               firstlineno 613
+               firstlineno 659
                lnotab 0x02012a0110012a0166014a010402
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
@@ -3039,67 +3303,67 @@
                   010000ab01000000000000000072087c0064011900000000000000000053
                   007c00a00000000000000000000000000000000000000000006402a60100
                   00ab01000000000000000072357c00640219000000000000000000a00100
                   000000000000000000000000000000000000006403a6010000ab01000000
                   0000000000640419000000000000000000a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d017c01530064
                   005300
-               623           0 RESUME                   0
+               669           0 RESUME                   0
                
-               624           2 LOAD_FAST                0 (row)
+               670           2 LOAD_FAST                0 (row)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('city')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE     8 (to 60)
                
-               625          44 LOAD_FAST                0 (row)
+               671          44 LOAD_FAST                0 (row)
                             46 LOAD_CONST               1 ('city')
                             48 BINARY_SUBSCR
                             58 RETURN_VALUE
                
-               626     >>   60 LOAD_FAST                0 (row)
+               672     >>   60 LOAD_FAST                0 (row)
                             62 LOAD_METHOD              0 (get)
                             84 LOAD_CONST               2 ('headquarters')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_JUMP_FORWARD_IF_FALSE    53 (to 208)
                
-               627         102 LOAD_FAST                0 (row)
+               673         102 LOAD_FAST                0 (row)
                            104 LOAD_CONST               2 ('headquarters')
                            106 BINARY_SUBSCR
                            116 LOAD_METHOD              1 (split)
                            138 LOAD_CONST               3 (',')
                            140 PRECALL                  1
                            144 CALL                     1
                            154 LOAD_CONST               4 (0)
                            156 BINARY_SUBSCR
                            166 LOAD_METHOD              2 (strip)
                            188 PRECALL                  0
                            192 CALL                     0
                            202 STORE_FAST               1 (city_name)
                
-               628         204 LOAD_FAST                1 (city_name)
+               674         204 LOAD_FAST                1 (city_name)
                            206 RETURN_VALUE
                
-               630     >>  208 LOAD_CONST               0 (None)
+               676     >>  208 LOAD_CONST               0 (None)
                            210 RETURN_VALUE
                consts
                   None
                   'city'
                   'headquarters'
                   ','
                   0
                names      ('get', 'split', 'strip')
                varnames   ('row', 'city_name')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_city'
-               firstlineno 623
+               firstlineno 669
                lnotab 0x02012a0110012a0166010402
             'end_customer'
             'meta'
             'employees'
             'ownership'
             1
             ('axis',)
@@ -3107,15 +3371,15 @@
             'city'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'str', 'apply')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df', 'list_to_csv', 'get_employees', 'get_ownership', 'get_state', 'get_city')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_targets'
-         firstlineno 507
+         firstlineno 553
          lnotab
             0x0203044034011801260106fe100474fb2e07160c060c0608060a06093c
             013c013c0134013402
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
@@ -3128,59 +3392,59 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         641           0 RESUME                   0
+         687           0 RESUME                   0
          
-         642           2 LOAD_CONST               1 ("\n    SELECT \n        e.*,\n        a.name as author\n    FROM event e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    WHERE\n        e.type = 'comment'\n        AND e.domain is null\n        AND search_uid = :search_uid\n    ")
+         688           2 LOAD_CONST               1 ("\n    SELECT \n        e.*,\n        a.name as author\n    FROM event e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    WHERE\n        e.type = 'comment'\n        AND e.domain is null\n        AND search_uid = :search_uid\n    ")
                        4 STORE_FAST               1 (statement)
          
-         654           6 LOAD_GLOBAL              0 (db)
+         700           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         655          58 LOAD_FAST                2 (conn)
+         701          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         656          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         702          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         657         120 LOAD_CONST               2 ('search_uid')
+         703         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         655         126 PRECALL                  2
+         701         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         659         142 LOAD_GLOBAL             11 (NULL + pd)
+         705         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         654         258 LOAD_CONST               0 (None)
+         700         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3191,15 +3455,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         660     >>  304 LOAD_FAST                4 (df)
+         706     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3208,15 +3472,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_comments'
-         firstlineno 641
+         firstlineno 687
          lnotab 0x0201040c34011801260106fe100474fb2e06
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3227,56 +3491,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         663           0 RESUME                   0
+         709           0 RESUME                   0
          
-         664           2 LOAD_GLOBAL              0 (db)
+         710           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         665          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         711          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         670          58 LOAD_FAST                1 (conn)
+         716          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         671         142 LOAD_GLOBAL             11 (NULL + pd)
+         717         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         664         258 LOAD_CONST               0 (None)
+         710         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3287,15 +3551,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         672     >>  304 LOAD_FAST                4 (df)
+         718     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3304,15 +3568,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event'
-         firstlineno 663
+         firstlineno 709
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3324,65 +3588,65 @@
             007c01a6010000ab01000000000000000064027c006901a6020000ab0200
             000000000000007d03740f000000000000000000006a0800000000000000
             007c03a0090000000000000000000000000000000000000000a6000000ab
             0000000000000000007c03a00a0000000000000000000000000000000000
             000000a6000000ab000000000000000000ac03a6020000ab020000000000
             0000007d04640064006400a6020000ab02000000000000000001006e0b23
             0031007304770278035900770101005900010001007c045300
-         675           0 RESUME                   0
+         721           0 RESUME                   0
          
-         676           2 LOAD_GLOBAL              1 (NULL + isinstance)
+         722           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (search_uid)
                       16 LOAD_GLOBAL              2 (int)
                       28 PRECALL                  2
                       32 CALL                     2
                       42 POP_JUMP_FORWARD_IF_TRUE     2 (to 48)
                       44 LOAD_ASSERTION_ERROR
                       46 RAISE_VARARGS            1
          
-         677     >>   48 LOAD_CONST               1 ("\n    SELECT \n        e.id,\n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.domain,\n        e.data,\n        a.type as actor_type,\n        a.key as actor_key,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type != 'mute'\n    ORDER BY created DESC\n    ;\n\n    ")
+         723     >>   48 LOAD_CONST               1 ("\n    SELECT \n        e.id,\n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.domain,\n        e.data,\n        a.type as actor_type,\n        a.key as actor_key,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type != 'mute'\n    ORDER BY created DESC\n    ;\n\n    ")
                       50 STORE_FAST               1 (statement)
          
-         699          52 LOAD_GLOBAL              4 (db)
+         745          52 LOAD_GLOBAL              4 (db)
                       64 LOAD_METHOD              3 (connect)
                       86 PRECALL                  0
                       90 CALL                     0
                      100 BEFORE_WITH
                      102 STORE_FAST               2 (conn)
          
-         700         104 LOAD_FAST                2 (conn)
+         746         104 LOAD_FAST                2 (conn)
                      106 LOAD_METHOD              4 (execute)
                      128 LOAD_GLOBAL             11 (NULL + sqlalchemy)
                      140 LOAD_ATTR                6 (text)
                      150 LOAD_FAST                1 (statement)
                      152 PRECALL                  1
                      156 CALL                     1
                      166 LOAD_CONST               2 ('search_uid')
                      168 LOAD_FAST                0 (search_uid)
                      170 BUILD_MAP                1
                      172 PRECALL                  2
                      176 CALL                     2
                      186 STORE_FAST               3 (result)
          
-         701         188 LOAD_GLOBAL             15 (NULL + pd)
+         747         188 LOAD_GLOBAL             15 (NULL + pd)
                      200 LOAD_ATTR                8 (DataFrame)
                      210 LOAD_FAST                3 (result)
                      212 LOAD_METHOD              9 (fetchall)
                      234 PRECALL                  0
                      238 CALL                     0
                      248 LOAD_FAST                3 (result)
                      250 LOAD_METHOD             10 (keys)
                      272 PRECALL                  0
                      276 CALL                     0
                      286 KW_NAMES                 3
                      288 PRECALL                  2
                      292 CALL                     2
                      302 STORE_FAST               4 (df)
          
-         699         304 LOAD_CONST               0 (None)
+         745         304 LOAD_CONST               0 (None)
                      306 LOAD_CONST               0 (None)
                      308 LOAD_CONST               0 (None)
                      310 PRECALL                  2
                      314 CALL                     2
                      324 POP_TOP
                      326 JUMP_FORWARD            11 (to 350)
                  >>  328 PUSH_EXC_INFO
@@ -3393,15 +3657,15 @@
                      338 POP_EXCEPT
                      340 RERAISE                  1
                  >>  342 POP_TOP
                      344 POP_EXCEPT
                      346 POP_TOP
                      348 POP_TOP
          
-         702     >>  350 LOAD_FAST                4 (df)
+         748     >>  350 LOAD_FAST                4 (df)
                      352 RETURN_VALUE
          ExceptionTable:
            102 to 302 -> 328 [1] lasti
            328 to 334 -> 336 [3] lasti
            342 to 342 -> 336 [3] lasti
          consts
             None
@@ -3410,15 +3674,15 @@
             ('columns',)
          names      ('isinstance', 'int', 'db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event_history'
-         firstlineno 675
+         firstlineno 721
          lnotab 0x02012e0104163401540174fe2e03
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3429,56 +3693,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         705           0 RESUME                   0
+         751           0 RESUME                   0
          
-         707           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
+         753           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
-         725           6 LOAD_GLOBAL              0 (db)
+         771           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         726          58 LOAD_FAST                2 (conn)
+         772          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         727         142 LOAD_GLOBAL             11 (NULL + pd)
+         773         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         725         258 LOAD_CONST               0 (None)
+         771         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3489,15 +3753,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         728     >>  304 LOAD_FAST                4 (df)
+         774     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3506,15 +3770,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_criteria_history'
-         firstlineno 705
+         firstlineno 751
          lnotab 0x020204123401540174fe2e03
       'uid'
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 7
          flags     : 3
@@ -3532,96 +3796,96 @@
             000000000000007d05741300000000000000000000741400000000000000
             0000006a0b00000000000000006a0c00000000000000007c05a6020000ab
             0200000000000000007d067c066a0d0000000000000000a00e0000000000
             0000000000000000000000000000006403a6010000ab0100000000000000
             006404190000000000000000007c066a0f000000000000000064053c0000
             00640064006400a6020000ab02000000000000000001006e0b2300310073
             04770278035900770101005900010001007c065300
-         734           0 RESUME                   0
+         780           0 RESUME                   0
          
-         735           2 LOAD_GLOBAL              0 (db)
+         781           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         736          54 LOAD_CONST               1 ("\n            SELECT \n                uid, \n                label, \n                meta \n                -- meta->>'next_due_date' as next_due_date,\n                -- meta->>'notes' as notes,\n                -- COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            -- LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            ")
+         782          54 LOAD_CONST               1 ('\n            SELECT \n                uid, \n                label, \n                meta \n            FROM search\n            \n            WHERE uid = :uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         749          58 LOAD_FAST                1 (conn)
+         791          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('uid')
                      122 LOAD_FAST                0 (uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         751         142 LOAD_FAST                3 (result)
+         793         142 LOAD_FAST                3 (result)
                      144 LOAD_METHOD              5 (fetchone)
                      166 PRECALL                  0
                      170 CALL                     0
                      180 STORE_FAST               4 (row)
          
-         752         182 LOAD_FAST                4 (row)
+         794         182 LOAD_FAST                4 (row)
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 214)
          
-         753         186 NOP
+         795         186 NOP
          
-         735         188 LOAD_CONST               0 (None)
+         781         188 LOAD_CONST               0 (None)
                      190 LOAD_CONST               0 (None)
                      192 LOAD_CONST               0 (None)
                      194 PRECALL                  2
                      198 CALL                     2
                      208 POP_TOP
                      210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         755     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         797     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                4 (row)
                      278 PRECALL                  2
                      282 CALL                     2
                      292 PRECALL                  1
                      296 CALL                     1
                      306 STORE_FAST               5 (obj)
          
-         756         308 LOAD_GLOBAL             19 (NULL + from_dict)
+         798         308 LOAD_GLOBAL             19 (NULL + from_dict)
                      320 LOAD_GLOBAL             20 (ts)
                      332 LOAD_ATTR               11 (models)
                      342 LOAD_ATTR               12 (Search)
                      352 LOAD_FAST                5 (obj)
                      354 PRECALL                  2
                      358 CALL                     2
                      368 STORE_FAST               6 (search)
          
-         757         370 LOAD_FAST                6 (search)
+         799         370 LOAD_FAST                6 (search)
                      372 LOAD_ATTR               13 (label)
                      382 LOAD_METHOD             14 (split)
                      404 LOAD_CONST               3 (' - ')
                      406 PRECALL                  1
                      410 CALL                     1
                      420 LOAD_CONST               4 (0)
                      422 BINARY_SUBSCR
                      432 LOAD_FAST                6 (search)
                      434 LOAD_ATTR               15 (meta)
                      444 LOAD_CONST               5 ('client')
                      446 STORE_SUBSCR
          
-         735         450 LOAD_CONST               0 (None)
+         781         450 LOAD_CONST               0 (None)
                      452 LOAD_CONST               0 (None)
                      454 LOAD_CONST               0 (None)
                      456 PRECALL                  2
                      460 CALL                     2
                      470 POP_TOP
                      472 JUMP_FORWARD            11 (to 496)
                  >>  474 PUSH_EXC_INFO
@@ -3632,72 +3896,200 @@
                      484 POP_EXCEPT
                      486 RERAISE                  1
                  >>  488 POP_TOP
                      490 POP_EXCEPT
                      492 POP_TOP
                      494 POP_TOP
          
-         759     >>  496 LOAD_FAST                6 (search)
+         801     >>  496 LOAD_FAST                6 (search)
                      498 RETURN_VALUE
          ExceptionTable:
            52 to 186 -> 474 [1] lasti
            214 to 448 -> 474 [1] lasti
            474 to 480 -> 482 [3] lasti
            488 to 488 -> 482 [3] lasti
          consts
             None
-            "\n            SELECT \n                uid, \n                label, \n                meta \n                -- meta->>'next_due_date' as next_due_date,\n                -- meta->>'notes' as notes,\n                -- COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            -- LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            "
+            '\n            SELECT \n                uid, \n                label, \n                meta \n            FROM search\n            \n            WHERE uid = :uid\n            '
             'uid'
             ' - '
             0
             'client'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'fetchone', 'dict', 'zip', 'keys', 'from_dict', 'ts', 'models', 'Search', 'label', 'split', 'meta')
          varnames   ('uid', 'conn', 'statement', 'result', 'row', 'obj', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search'
-         firstlineno 734
-         lnotab 0x02013401040d54022801040102ee1a145e013e0150ea2e18
+         firstlineno 780
+         lnotab 0x02013401040954022801040102f21a105e013e0150ee2e14
+      'label'
+      code
+         argcount  : 1
+         nlocals   : 7
+         stacksize : 7
+         flags     : 3
+         code
+            0x9700740000000000000000000000a00100000000000000000000000000
+            00000000000000a6000000ab00000000000000000035007d0164017d027c
+            01a002000000000000000000000000000000000000000074070000000000
+            00000000006a0400000000000000007c02a6010000ab0100000000000000
+            0064027c006901a6020000ab0200000000000000007d037c03a005000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            007d047c04800e0900640064006400a6020000ab02000000000000000001
+            0064005300740d00000000000000000000740f000000000000000000007c
+            03a0080000000000000000000000000000000000000000a6000000ab0000
+            000000000000007c04a6020000ab020000000000000000a6010000ab0100
+            000000000000007d05741300000000000000000000741400000000000000
+            0000006a0b00000000000000006a0c00000000000000007c05a6020000ab
+            0200000000000000007d06640064006400a6020000ab0200000000000000
+            0001006e0b230031007304770278035900770101005900010001007c0653
+            00
+         804           0 RESUME                   0
+         
+         805           2 LOAD_GLOBAL              0 (db)
+                      14 LOAD_METHOD              1 (connect)
+                      36 PRECALL                  0
+                      40 CALL                     0
+                      50 BEFORE_WITH
+                      52 STORE_FAST               1 (conn)
+         
+         806          54 LOAD_CONST               1 ('\n            SELECT \n                uid, \n                label, \n                meta \n            FROM search\n            \n            WHERE label = :label\n            ')
+                      56 STORE_FAST               2 (statement)
+         
+         815          58 LOAD_FAST                1 (conn)
+                      60 LOAD_METHOD              2 (execute)
+                      82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                2 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
+                     120 LOAD_CONST               2 ('label')
+                     122 LOAD_FAST                0 (label)
+                     124 BUILD_MAP                1
+                     126 PRECALL                  2
+                     130 CALL                     2
+                     140 STORE_FAST               3 (result)
+         
+         817         142 LOAD_FAST                3 (result)
+                     144 LOAD_METHOD              5 (fetchone)
+                     166 PRECALL                  0
+                     170 CALL                     0
+                     180 STORE_FAST               4 (row)
+         
+         818         182 LOAD_FAST                4 (row)
+                     184 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 214)
+         
+         819         186 NOP
+         
+         805         188 LOAD_CONST               0 (None)
+                     190 LOAD_CONST               0 (None)
+                     192 LOAD_CONST               0 (None)
+                     194 PRECALL                  2
+                     198 CALL                     2
+                     208 POP_TOP
+                     210 LOAD_CONST               0 (None)
+                     212 RETURN_VALUE
+         
+         821     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+                     226 LOAD_GLOBAL             15 (NULL + zip)
+                     238 LOAD_FAST                3 (result)
+                     240 LOAD_METHOD              8 (keys)
+                     262 PRECALL                  0
+                     266 CALL                     0
+                     276 LOAD_FAST                4 (row)
+                     278 PRECALL                  2
+                     282 CALL                     2
+                     292 PRECALL                  1
+                     296 CALL                     1
+                     306 STORE_FAST               5 (obj)
+         
+         822         308 LOAD_GLOBAL             19 (NULL + from_dict)
+                     320 LOAD_GLOBAL             20 (ts)
+                     332 LOAD_ATTR               11 (models)
+                     342 LOAD_ATTR               12 (Search)
+                     352 LOAD_FAST                5 (obj)
+                     354 PRECALL                  2
+                     358 CALL                     2
+                     368 STORE_FAST               6 (search)
+         
+         805         370 LOAD_CONST               0 (None)
+                     372 LOAD_CONST               0 (None)
+                     374 LOAD_CONST               0 (None)
+                     376 PRECALL                  2
+                     380 CALL                     2
+                     390 POP_TOP
+                     392 JUMP_FORWARD            11 (to 416)
+                 >>  394 PUSH_EXC_INFO
+                     396 WITH_EXCEPT_START
+                     398 POP_JUMP_FORWARD_IF_TRUE     4 (to 408)
+                     400 RERAISE                  2
+                 >>  402 COPY                     3
+                     404 POP_EXCEPT
+                     406 RERAISE                  1
+                 >>  408 POP_TOP
+                     410 POP_EXCEPT
+                     412 POP_TOP
+                     414 POP_TOP
+         
+         825     >>  416 LOAD_FAST                6 (search)
+                     418 RETURN_VALUE
+         ExceptionTable:
+           52 to 186 -> 394 [1] lasti
+           214 to 368 -> 394 [1] lasti
+           394 to 400 -> 402 [3] lasti
+           408 to 408 -> 402 [3] lasti
+         consts
+            None
+            '\n            SELECT \n                uid, \n                label, \n                meta \n            FROM search\n            \n            WHERE label = :label\n            '
+            'label'
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'fetchone', 'dict', 'zip', 'keys', 'from_dict', 'ts', 'models', 'Search')
+         varnames   ('label', 'conn', 'statement', 'result', 'row', 'obj', 'search')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
+         name       'find_search_by_label'
+         firstlineno 804
+         lnotab 0x02013401040954022801040102f21a105e013eef2e14
       'searchToken'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000007d
             017c017c016401190000000000000000007c006b02000000001900000000
             00000000007d027c026a0100000000000000007202640053007405000000
             000000000000007c026a0300000000000000006402190000000000000000
             00640319000000000000000000a6010000ab0100000000000000005300
-         762           0 RESUME                   0
+         828           0 RESUME                   0
          
-         763           2 LOAD_GLOBAL              1 (NULL + searches_query)
+         829           2 LOAD_GLOBAL              1 (NULL + searches_query)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               1 (searches)
          
-         764          30 LOAD_FAST                1 (searches)
+         830          30 LOAD_FAST                1 (searches)
                       32 LOAD_FAST                1 (searches)
                       34 LOAD_CONST               1 ('searchToken')
                       36 BINARY_SUBSCR
                       46 LOAD_FAST                0 (searchToken)
                       48 COMPARE_OP               2 (==)
                       54 BINARY_SUBSCR
                       64 STORE_FAST               2 (search)
          
-         765          66 LOAD_FAST                2 (search)
+         831          66 LOAD_FAST                2 (search)
                       68 LOAD_ATTR                1 (empty)
                       78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
          
-         766          80 LOAD_CONST               0 (None)
+         832          80 LOAD_CONST               0 (None)
                       82 RETURN_VALUE
          
-         768     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
+         834     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
                       96 LOAD_FAST                2 (search)
                       98 LOAD_ATTR                3 (iloc)
                      108 LOAD_CONST               2 (0)
                      110 BINARY_SUBSCR
                      120 LOAD_CONST               3 ('uid')
                      122 BINARY_SUBSCR
                      132 PRECALL                  1
@@ -3710,15 +4102,15 @@
             'uid'
          names      ('searches_query', 'empty', 'find_search', 'iloc')
          varnames   ('searchToken', 'searches', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_token'
-         firstlineno 762
+         firstlineno 828
          lnotab 0x02011c0124010e010402
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3732,41 +4124,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         771           0 RESUME                   0
+         837           0 RESUME                   0
          
-         772           2 LOAD_GLOBAL              0 (db)
+         838           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         773          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         839          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         778          58 LOAD_FAST                1 (conn)
+         844          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('domain')
                      122 LOAD_FAST                0 (domain)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         772         142 LOAD_CONST               0 (None)
+         838         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3777,24 +4169,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         780     >>  188 LOAD_FAST                3 (result)
+         846     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         781         210 LOAD_CONST               0 (None)
+         847         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         783     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         849     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3802,15 +4194,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         784         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         850         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Company)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3823,15 +4215,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 771
+         firstlineno 837
          lnotab 0x02013401040554fa2e08160104028201
       'email'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3846,41 +4238,41 @@
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000006a0c00000000000000006a0d00000000000000007c
             04a6020000ab0200000000000000005300
-         787           0 RESUME                   0
+         853           0 RESUME                   0
          
-         788           2 LOAD_GLOBAL              0 (db)
+         854           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         789          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
+         855          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
                       56 STORE_FAST               2 (statement)
          
-         794          58 LOAD_FAST                1 (conn)
+         860          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('email')
                      122 LOAD_FAST                0 (email)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         788         142 LOAD_CONST               0 (None)
+         854         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3891,24 +4283,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         796     >>  188 LOAD_FAST                3 (result)
+         862     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         797         210 LOAD_CONST               0 (None)
+         863         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         799     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         865     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3916,15 +4308,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         800         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         866         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (ts)
                      368 LOAD_ATTR               12 (models)
                      378 LOAD_ATTR               13 (Actor)
                      388 LOAD_FAST                4 (obj)
                      390 PRECALL                  2
                      394 CALL                     2
                      404 RETURN_VALUE
@@ -3939,15 +4331,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'ts', 'models', 'Actor')
          varnames   ('email', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_actor_by_email'
-         firstlineno 787
+         firstlineno 853
          lnotab 0x02013401040554fa2e08160104028201
       'event_id'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3961,41 +4353,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         803           0 RESUME                   0
+         869           0 RESUME                   0
          
-         804           2 LOAD_GLOBAL              0 (db)
+         870           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         805          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
+         871          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         810          58 LOAD_FAST                1 (conn)
+         876          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('event_id')
                      122 LOAD_FAST                0 (event_id)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         804         142 LOAD_CONST               0 (None)
+         870         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -4006,24 +4398,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         812     >>  188 LOAD_FAST                3 (result)
+         878     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         813         210 LOAD_CONST               0 (None)
+         879         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         815     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         881     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -4031,15 +4423,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         816         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         882         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Event)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -4052,15 +4444,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Event')
          varnames   ('event_id', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_event_by_id'
-         firstlineno 803
+         firstlineno 869
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 12
          flags     : 3
          code
@@ -4072,71 +4464,71 @@
             000000000000007c006a0800000000000000007c006a0900000000000000
             007415000000000000000000006a0b00000000000000007c006a0c000000
             0000000000a6010000ab01000000000000000064029c06a6020000ab0200
             0000000000000001007c01a00d0000000000000000000000000000000000
             000000a6000000ab0000000000000000000100640064006400a6020000ab
             020000000000000000010064005300230031007304770278035900770101
             0059000100010064005300
-         822           0 RESUME                   0
+         888           0 RESUME                   0
          
-         823           2 LOAD_GLOBAL              0 (db)
+         889           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         824          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
+         890          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         836          58 LOAD_FAST                1 (conn)
+         902          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         837          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         903          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         839         120 LOAD_FAST                0 (company)
+         905         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (uid)
          
-         840         132 LOAD_FAST                0 (company)
+         906         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (name)
          
-         841         144 LOAD_FAST                0 (company)
+         907         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (description)
          
-         842         156 LOAD_FAST                0 (company)
+         908         156 LOAD_FAST                0 (company)
                      158 LOAD_ATTR                8 (domain)
          
-         843         168 LOAD_FAST                0 (company)
+         909         168 LOAD_FAST                0 (company)
                      170 LOAD_ATTR                9 (source)
          
-         844         180 LOAD_GLOBAL             21 (NULL + json)
+         910         180 LOAD_GLOBAL             21 (NULL + json)
                      192 LOAD_ATTR               11 (dumps)
                      202 LOAD_FAST                0 (company)
                      204 LOAD_ATTR               12 (meta)
                      214 PRECALL                  1
                      218 CALL                     1
          
-         838         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
+         904         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
                      230 BUILD_CONST_KEY_MAP      6
          
-         836         232 PRECALL                  2
+         902         232 PRECALL                  2
                      236 CALL                     2
                      246 POP_TOP
          
-         848         248 LOAD_FAST                1 (conn)
+         914         248 LOAD_FAST                1 (conn)
                      250 LOAD_METHOD             13 (commit)
                      272 PRECALL                  0
                      276 CALL                     0
                      286 POP_TOP
          
-         823         288 LOAD_CONST               0 (None)
+         889         288 LOAD_CONST               0 (None)
                      290 LOAD_CONST               0 (None)
                      292 LOAD_CONST               0 (None)
                      294 PRECALL                  2
                      298 CALL                     2
                      308 POP_TOP
                      310 LOAD_CONST               0 (None)
                      312 RETURN_VALUE
@@ -4163,15 +4555,15 @@
             ('uid', 'name', 'description', 'domain', 'source', 'meta')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'uid', 'name', 'description', 'domain', 'source', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 822
+         firstlineno 888
          lnotab 0x02013401040c180126020c010c010c010c010c0130fa04fe100c28e7
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
@@ -4181,58 +4573,58 @@
             006a0400000000000000006401a6010000ab010000000000000000740b00
             0000000000000000006a0600000000000000007c006a0700000000000000
             00a6010000ab0100000000000000007c006a08000000000000000064029c
             02a6020000ab02000000000000000001007c01a009000000000000000000
             0000000000000000000000a6000000ab0000000000000000000100640064
             006400a6020000ab02000000000000000001006400530023003100730477
             02780359007701010059000100010064005300
-         851           0 RESUME                   0
+         917           0 RESUME                   0
          
-         852           2 LOAD_GLOBAL              0 (db)
+         918           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         853          54 LOAD_FAST                1 (conn)
+         919          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         854          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         920          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         855         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
+         921         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
          
-         854         102 PRECALL                  1
+         920         102 PRECALL                  1
                      106 CALL                     1
          
-         864         116 LOAD_GLOBAL             11 (NULL + json)
+         930         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (meta)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         865         164 LOAD_FAST                0 (search)
+         931         164 LOAD_FAST                0 (search)
                      166 LOAD_ATTR                8 (uid)
          
-         863         176 LOAD_CONST               2 (('meta', 'uid'))
+         929         176 LOAD_CONST               2 (('meta', 'uid'))
                      178 BUILD_CONST_KEY_MAP      2
          
-         853         180 PRECALL                  2
+         919         180 PRECALL                  2
                      184 CALL                     2
                      194 POP_TOP
          
-         868         196 LOAD_FAST                1 (conn)
+         934         196 LOAD_FAST                1 (conn)
                      198 LOAD_METHOD              9 (commit)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 POP_TOP
          
-         852         236 LOAD_CONST               0 (None)
+         918         236 LOAD_CONST               0 (None)
                      238 LOAD_CONST               0 (None)
                      240 LOAD_CONST               0 (None)
                      242 PRECALL                  2
                      246 CALL                     2
                      256 POP_TOP
                      258 LOAD_CONST               0 (None)
                      260 RETURN_VALUE
@@ -4259,15 +4651,15 @@
             ('meta', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'meta', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 851
+         firstlineno 917
          lnotab 0x020134011801160102ff0e0a30010cfe04f6100f28f0
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4278,61 +4670,61 @@
             006901a6020000ab02000000000000000001007c01a00200000000000000
             000000000000000000000000007407000000000000000000006a04000000
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00500000000000000000000000000000000000000
             00a6000000ab0000000000000000000100640064006400a6020000ab0200
             000000000000000100640053002300310073047702780359007701010059
             000100010064005300
-         874           0 RESUME                   0
+         940           0 RESUME                   0
          
-         876           2 LOAD_GLOBAL              0 (db)
+         942           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         877          54 LOAD_FAST                1 (conn)
+         943          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         878          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         944          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         879         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
+         945         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
          
-         878         102 PRECALL                  1
+         944         102 PRECALL                  1
                      106 CALL                     1
          
-         887         116 LOAD_CONST               2 ('event_id')
+         953         116 LOAD_CONST               2 ('event_id')
                      118 LOAD_FAST                0 (event_id)
          
-         886         120 BUILD_MAP                1
+         952         120 BUILD_MAP                1
          
-         877         122 PRECALL                  2
+         943         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         890         138 LOAD_FAST                1 (conn)
+         956         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         891         216 LOAD_FAST                1 (conn)
+         957         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              5 (commit)
                      240 PRECALL                  0
                      244 CALL                     0
                      254 POP_TOP
          
-         876         256 LOAD_CONST               0 (None)
+         942         256 LOAD_CONST               0 (None)
                      258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 PRECALL                  2
                      266 CALL                     2
                      276 POP_TOP
                      278 LOAD_CONST               0 (None)
                      280 RETURN_VALUE
@@ -4360,15 +4752,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('event_id', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'mute_event'
-         firstlineno 874
+         firstlineno 940
          lnotab 0x020234011801160102ff0e0904ff02f7100d4e0128f1
       'comment_id'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -4380,58 +4772,58 @@
             0064027c006901a6020000ab02000000000000000001007c01a002000000
             00000000000000000000000000000000007407000000000000000000006a
             0400000000000000006403a6010000ab010000000000000000a6010000ab
             01000000000000000001007c01a005000000000000000000000000000000
             0000000000a6000000ab0000000000000000000100640064006400a60200
             00ab02000000000000000001006400530023003100730477027803590077
             01010059000100010064005300
-         897           0 RESUME                   0
+         963           0 RESUME                   0
          
-         898           2 LOAD_GLOBAL              0 (db)
+         964           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         899          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
+         965          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         903          58 LOAD_FAST                1 (conn)
+         969          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('comment_id')
                      122 LOAD_FAST                0 (comment_id)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 POP_TOP
          
-         904         142 LOAD_FAST                1 (conn)
+         970         142 LOAD_FAST                1 (conn)
                      144 LOAD_METHOD              2 (execute)
                      166 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      178 LOAD_ATTR                4 (text)
                      188 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      190 PRECALL                  1
                      194 CALL                     1
                      204 PRECALL                  1
                      208 CALL                     1
                      218 POP_TOP
          
-         905         220 LOAD_FAST                1 (conn)
+         971         220 LOAD_FAST                1 (conn)
                      222 LOAD_METHOD              5 (commit)
                      244 PRECALL                  0
                      248 CALL                     0
                      258 POP_TOP
          
-         898         260 LOAD_CONST               0 (None)
+         964         260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 LOAD_CONST               0 (None)
                      266 PRECALL                  2
                      270 CALL                     2
                      280 POP_TOP
                      282 LOAD_CONST               0 (None)
                      284 RETURN_VALUE
@@ -4459,15 +4851,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('comment_id', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'delete_comment'
-         firstlineno 897
+         firstlineno 963
          lnotab 0x02013401040454014e0128f9
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4480,71 +4872,71 @@
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00200000000000000000000000000000000000000
             007407000000000000000000006a0400000000000000006404a6010000ab
             010000000000000000a6010000ab01000000000000000001007c01a00500
             00000000000000000000000000000000000000a6000000ab000000000000
             0000000100640064006400a6020000ab0200000000000000000100640053
             002300310073047702780359007701010059000100010064005300
-         908           0 RESUME                   0
+         974           0 RESUME                   0
          
-         912           2 LOAD_GLOBAL              0 (db)
+         978           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         913          54 LOAD_FAST                1 (conn)
+         979          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         914          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         980          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         915         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
+         981         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
          
-         914         102 PRECALL                  1
+         980         102 PRECALL                  1
                      106 CALL                     1
          
-         921         116 LOAD_CONST               2 ('search_uid')
+         987         116 LOAD_CONST               2 ('search_uid')
                      118 LOAD_FAST                0 (search_uid)
                      120 BUILD_MAP                1
          
-         913         122 PRECALL                  2
+         979         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         923         138 LOAD_FAST                1 (conn)
+         989         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         924         216 LOAD_FAST                1 (conn)
+         990         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              2 (execute)
                      240 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      252 LOAD_ATTR                4 (text)
                      262 LOAD_CONST               4 ('REFRESH MATERIALIZED VIEW rating')
                      264 PRECALL                  1
                      268 CALL                     1
                      278 PRECALL                  1
                      282 CALL                     1
                      292 POP_TOP
          
-         927         294 LOAD_FAST                1 (conn)
+         993         294 LOAD_FAST                1 (conn)
                      296 LOAD_METHOD              5 (commit)
                      318 PRECALL                  0
                      322 CALL                     0
                      332 POP_TOP
          
-         912         334 LOAD_CONST               0 (None)
+         978         334 LOAD_CONST               0 (None)
                      336 LOAD_CONST               0 (None)
                      338 LOAD_CONST               0 (None)
                      340 PRECALL                  2
                      344 CALL                     2
                      354 POP_TOP
                      356 LOAD_CONST               0 (None)
                      358 RETURN_VALUE
@@ -4573,23 +4965,23 @@
             'REFRESH MATERIALIZED VIEW rating'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('search_uid', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'reset_inbox'
-         firstlineno 908
+         firstlineno 974
          lnotab 0x020434011801160102ff0e0706f8100a4e014e0328f1
       (True, None, 'create')
-   names      ('hashlib', 'json', 'dataclasses', 'asdict', 'time', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'gandai', 'ts', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_event', 'models', 'insert_company', 'insert_actor', 'insert_search', 'important_targets_from_event', 'int', 'str', 'bool', 'insert_companies_as_targets', 'DataFrame', 'searches_query', 'average_rating_per_search_query', 'validation_history', 'searches_comment_counts', 'enriched_searches_query', 'actor', 'buyer', 'search_targets', 'search_comments', 'event', 'event_history', 'search_criteria_history', 'find_search', 'find_search_by_token', 'find_company_by_domain', 'find_actor_by_email', 'find_event_by_id', 'update_company', 'update_search', 'mute_event', 'delete_comment', 'reset_inbox')
+   names      ('hashlib', 'json', 'dataclasses', 'asdict', 'time', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'gandai', 'ts', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_event', 'models', 'insert_company', 'insert_actor', 'insert_search', 'important_targets_from_search', 'important_targets_from_event', 'int', 'str', 'bool', 'insert_companies_as_targets', 'DataFrame', 'searches_query', 'average_rating_per_search_query', 'validation_history', 'searches_comment_counts', 'enriched_searches_query', 'actor', 'buyer', 'search_targets', 'search_comments', 'event', 'event_history', 'search_criteria_history', 'find_search', 'find_search_by_label', 'find_search_by_token', 'find_company_by_domain', 'find_actor_by_email', 'find_event_by_id', 'update_company', 'update_search', 'mute_event', 'delete_comment', 'reset_inbox')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080108010c010c011002080108010c010c02140208010c010c
-      011c021406101e240e100f1010244c0201020102fa04010eff020202fe02
-      0302fd020402fc020502fb020602fa020702f908611620060c162b061406
-      14160e16610c7f00071a161a0c1a1e1a1d241c2409101010101013101d10
-      171017100b
+      011c021406101e240e100f1010020116ff020116ff020202fe082e244c02
+      01020102fa04010eff020202fe020302fd020402fc020502fb020602fa02
+      0702f908611620060c162b06140614160e16610c7f00071a161a0c1a1e1a
+      1d241824182409101010101013101d10171017100b
```

### Comparing `gandai-1.7.56/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/__pycache__/tasks.cpython-311.pyc` & `gandai-1.7.57/gandai/__pycache__/tasks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/analytics.py` & `gandai-1.7.57/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/constants.py` & `gandai-1.7.57/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/db.py` & `gandai-1.7.57/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/google.py` & `gandai-1.7.57/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/gpt.py` & `gandai-1.7.57/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/grata.py` & `gandai-1.7.57/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/helpers.py` & `gandai-1.7.57/gandai/helpers.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/main.py` & `gandai-1.7.57/gandai/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,22 +181,22 @@
             "role": "system",
             "content": ts.gpt.HOW_TO_IMPORT,
         },
         {
             "role": "system",
             "content": ts.gpt.HOW_TO_TRANSITION,
         },
-        # {
-        #     "role": "system",
-        #     "content": ts.gpt.HOW_TO_GOOGLE,
-        # },
-        # {
-        #     "role": "system",
-        #     "content": ts.gpt.HOW_TO_GOOGLE_MAPS,
-        # },
+        {
+            "role": "system",
+            "content": ts.gpt.HOW_TO_GOOGLE,
+        },
+        {
+            "role": "system",
+            "content": ts.gpt.HOW_TO_GOOGLE_MAPS,
+        },
         {
             "role": "system",
             "content": ts.gpt.HOW_TO_SEARCH_GRATA_API,
         },
         {
             "role": "system",
             "content": f"the search_uid is {event.search_uid}",
@@ -208,16 +208,18 @@
         {"role": "user", "content": event.data["prompt"]},
     ]
     resp = ts.gpt.ask_gpt4(messages)
 
     print(resp)
     for new_event in resp["events"]:
         print("new event:", new_event)
+        new_event["search_uid"] = event.search_uid
         e = from_dict(ts.models.Event, new_event)
         print(e)
+
         e.data["prompt"] = event.data["prompt"]
         ts.query.insert_event(e)
 
 
 def enrich_with_gpt(company: ts.models.Company) -> None:
     print("enriching with gpt...")
     try:
@@ -325,14 +327,21 @@
 
     elif event.type == "grata_search":
         run_google_search(search=search, event=event)
 
     elif event.type == "import":
         ts.query.important_targets_from_event(event=event)
 
+    elif event.type == "import_searches":
+        for label in event.data["searches"]:
+            from_search = ts.query.find_search_by_label(label=label)
+            ts.query.important_targets_from_search(
+                from_search=from_search, to_search=search
+            )
+
     elif event.type == "reset":
         print("💣 Resetting Inbox...")
         ts.query.reset_inbox(search_uid=search.uid)
 
     elif event.type == "rating":
         # handle rating
         print(event)
@@ -367,19 +376,14 @@
             )
 
     elif event.type == "update":
         if domain:
             company = ts.query.find_company_by_domain(domain)
             if event.data.get("name"):
                 company.name = event.data["name"]
-            # if event.data.get("description"):
-            #     company.description = event.data["description"]
-            #     import pdb
-
-            #     pdb.set_trace()
             company.meta = {**company.meta, **event.data}
             ts.query.update_company(company)
         else:
             search.meta = {**search.meta, **event.data}
             ts.query.update_search(search)
 
     elif event.type == "move":
```

### Comparing `gandai-1.7.56/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.57/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/migrations/db_seed.py` & `gandai-1.7.57/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/migrations/dealcloud.py` & `gandai-1.7.57/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.57/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/migrations/sql/schema.sql` & `gandai-1.7.57/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/models.py` & `gandai-1.7.57/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/query.py` & `gandai-1.7.57/gandai/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,14 +93,60 @@
         obj = asdict(search)
         obj["meta"] = json.dumps(obj["meta"])
         con.execute(statement, obj)
         con.commit()
     return search
 
 
+def important_targets_from_search(
+    from_search: ts.models.Search, to_search: ts.models.Search
+) -> None:
+
+    # import pdb
+
+    # pdb.set_trace()
+    targets = search_targets(search_uid=from_search.uid)
+    targets = targets[targets["stage"] != "reject"]
+    domains: list = targets["domain"].tolist()
+    print(len(domains))
+
+    # stage_dict = targets.set_index("domain")["stage"].to_dict()
+
+    new_event_ids = []
+    with db.connect() as con:
+        with con.begin():
+            for domain in domains:
+                # should these be in same transaction?
+                domain = ts.helpers.clean_domain(domain)
+
+                result = con.execute(
+                    sqlalchemy.text(
+                        """
+                        INSERT INTO event (search_uid, domain, actor_key, type) 
+                        VALUES(:search_uid, :domain, :actor_key, :type)
+                        ON CONFLICT DO NOTHING
+                        RETURNING id
+                        """
+                    ),
+                    {
+                        "search_uid": to_search.uid,
+                        "actor_key": "chatgpt",
+                        "domain": domain,
+                        "type": "land",
+                    },
+                )
+
+                new_event_id = result.scalar_one()
+                if new_event_id is not None:
+                    new_event_ids.append(new_event_id)
+
+    for event_id in new_event_ids:
+        ts.trigger_process_event(event_id=event_id)
+
+
 def important_targets_from_event(event: ts.models.Event) -> None:
 
     source = event.data.get("source")
     targets = search_targets(search_uid=event.search_uid)
     stage_dict = targets.set_index("domain")["stage"].to_dict()
 
     def get_stage(domain):
@@ -179,15 +225,15 @@
 ) -> None:
     print(f"Inserting {len(companies)} companies as targets...")
 
     targets = search_targets(search_uid=search_uid)
 
     if force:
         # "New keywords should look at companies that were previously rejected"
-        # import pdb; pdb.set_trace()
+
         targets = targets[targets["stage"] != "reject"]
         protected_domains = targets["domain"].tolist()
     else:
         protected_domains = targets["domain"].tolist()
 
     ## idea, insert "search" comment for what happened
 
@@ -734,19 +780,15 @@
 def find_search(uid: int) -> ts.models.Search:
     with db.connect() as conn:
         statement = """
             SELECT 
                 uid, 
                 label, 
                 meta 
-                -- meta->>'next_due_date' as next_due_date,
-                -- meta->>'notes' as notes,
-                -- COALESCE(criteria.data, '{}'::jsonb) as criteria
             FROM search
-            -- LEFT JOIN criteria ON search.uid = criteria.search_uid
             
             WHERE uid = :uid
             """
         result = conn.execute(sqlalchemy.text(statement), {"uid": uid})
 
         row = result.fetchone()
         if row is None:
@@ -755,14 +797,38 @@
         obj = dict(zip(result.keys(), row))
         search = from_dict(ts.models.Search, obj)
         search.meta["client"] = search.label.split(" - ")[0]
 
     return search
 
 
+def find_search_by_label(label: str) -> ts.models.Search:
+    with db.connect() as conn:
+        statement = """
+            SELECT 
+                uid, 
+                label, 
+                meta 
+            FROM search
+            
+            WHERE label = :label
+            """
+        result = conn.execute(sqlalchemy.text(statement), {"label": label})
+
+        row = result.fetchone()
+        if row is None:
+            return None
+
+        obj = dict(zip(result.keys(), row))
+        search = from_dict(ts.models.Search, obj)
+        # search.meta["client"] = search.label.split(" - ")[0]
+
+    return search
+
+
 def find_search_by_token(searchToken: str) -> ts.models.Search:
     searches = searches_query()
     search = searches[searches["searchToken"] == searchToken]
     if search.empty:
         return None
     else:
         return find_search(search.iloc[0]["uid"])
```

### Comparing `gandai-1.7.56/gandai/secrets.py` & `gandai-1.7.57/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai/tasks.py` & `gandai-1.7.57/gandai/tasks.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.56/gandai.egg-info/SOURCES.txt` & `gandai-1.7.57/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

