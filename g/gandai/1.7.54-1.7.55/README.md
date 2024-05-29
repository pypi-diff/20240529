# Comparing `tmp/gandai-1.7.54.tar.gz` & `tmp/gandai-1.7.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.54.tar", last modified: Fri May 24 07:19:12 2024, max compression
+gzip compressed data, was "gandai-1.7.55.tar", last modified: Tue May 28 14:24:10 2024, max compression
```

## Comparing `gandai-1.7.54.tar` & `gandai-1.7.55.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:19:12.746815 gandai-1.7.54/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.54/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 07:19:12.746620 gandai-1.7.54/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:19:12.736649 gandai-1.7.54/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.54/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:19:12.743361 gandai-1.7.54/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.54/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.54/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.54/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.54/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2600 2024-05-24 00:47:47.000000 gandai-1.7.54/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.54/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.54/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.54/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7037 2024-05-23 23:56:05.000000 gandai-1.7.54/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.54/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-24 05:31:06.000000 gandai-1.7.54/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    15990 2024-05-24 06:59:26.000000 gandai-1.7.54/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.54/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    42429 2024-05-24 06:59:56.000000 gandai-1.7.54/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.54/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.54/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.54/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1550 2024-05-24 07:18:42.000000 gandai-1.7.54/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.54/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1674 2024-05-24 00:47:46.000000 gandai-1.7.54/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.54/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.54/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)     6395 2024-05-23 23:56:03.000000 gandai-1.7.54/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.54/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-24 05:31:04.000000 gandai-1.7.54/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    11376 2024-05-24 06:59:24.000000 gandai-1.7.54/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:19:12.744084 gandai-1.7.54/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.54/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:19:12.744435 gandai-1.7.54/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.54/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.54/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.54/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.54/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.54/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:19:12.746148 gandai-1.7.54/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.54/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.54/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.54/gandai/migrations/sql/240523-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.54/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.54/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    28739 2024-05-24 06:59:54.000000 gandai-1.7.54/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.54/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1057 2024-05-24 07:18:39.000000 gandai-1.7.54/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:19:12.746422 gandai-1.7.54/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 07:19:12.000000 gandai-1.7.54/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-24 07:19:12.000000 gandai-1.7.54/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-24 07:19:12.000000 gandai-1.7.54/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-24 07:19:12.000000 gandai-1.7.54/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-24 07:19:06.000000 gandai-1.7.54/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-24 07:19:12.746850 gandai-1.7.54/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.54/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-28 14:24:10.457664 gandai-1.7.55/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.55/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-28 14:24:10.457467 gandai-1.7.55/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-28 14:24:10.448326 gandai-1.7.55/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.55/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-28 14:24:10.453961 gandai-1.7.55/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.55/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.55/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.55/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.55/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2600 2024-05-24 00:47:47.000000 gandai-1.7.55/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.55/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.55/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.55/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7037 2024-05-24 15:09:38.000000 gandai-1.7.55/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.55/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-24 15:09:39.000000 gandai-1.7.55/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    15990 2024-05-24 15:09:39.000000 gandai-1.7.55/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10401 2024-05-24 15:29:10.000000 gandai-1.7.55/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    42438 2024-05-28 14:21:54.000000 gandai-1.7.55/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.55/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.55/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.55/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1697 2024-05-24 15:09:39.000000 gandai-1.7.55/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.55/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1674 2024-05-24 00:47:46.000000 gandai-1.7.55/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.55/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.55/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)     6395 2024-05-24 15:09:36.000000 gandai-1.7.55/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.55/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-24 15:09:36.000000 gandai-1.7.55/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    11376 2024-05-24 15:09:36.000000 gandai-1.7.55/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-28 14:24:10.455052 gandai-1.7.55/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.55/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-28 14:24:10.455469 gandai-1.7.55/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.55/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.55/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.55/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.55/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.55/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-28 14:24:10.456994 gandai-1.7.55/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.55/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.55/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-24 15:09:36.000000 gandai-1.7.55/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3021 2024-05-28 14:16:49.000000 gandai-1.7.55/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-24 15:29:09.000000 gandai-1.7.55/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    29338 2024-05-28 14:17:20.000000 gandai-1.7.55/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.55/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1081 2024-05-24 15:09:36.000000 gandai-1.7.55/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-28 14:24:10.457284 gandai-1.7.55/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-28 14:24:10.000000 gandai-1.7.55/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-28 14:24:10.000000 gandai-1.7.55/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-28 14:24:10.000000 gandai-1.7.55/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-28 14:24:10.000000 gandai-1.7.55/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-28 14:23:59.000000 gandai-1.7.55/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-28 14:24:10.457703 gandai-1.7.55/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.55/setup.py
```

### Comparing `gandai-1.7.54/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x93d74f66 (Thu May 23 23:56:03 2024 UTC)
+moddate:  0xb0ad5066 (Fri May 24 15:09:36 2024 UTC)
 files sz: 6395
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `gandai-1.7.54/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x18265066 (Fri May 24 05:31:04 2024 UTC)
+moddate:  0xb0ad5066 (Fri May 24 15:09:36 2024 UTC)
 files sz: 1283
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `gandai-1.7.54/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xcc3a5066 (Fri May 24 06:59:24 2024 UTC)
+moddate:  0xb0ad5066 (Fri May 24 15:09:36 2024 UTC)
 files sz: 11376
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `gandai-1.7.54/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/models.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd29a4f66 (Thu May 23 19:36:50 2024 UTC)
+moddate:  0x45b25066 (Fri May 24 15:29:09 2024 UTC)
 files sz: 4501
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
@@ -1416,23 +1416,21 @@
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006505650464023c
             000000020065066507ac03a6010000ab0100000000000000005a08650765
-            0464043c000000020065066509ac03a6010000ab0100000000000000005a
-            0a6509650464053c000000650b64066505660264078404a6000000ab0000
-            000000000000005a0c650b64066505660264088404a6000000ab00000000
-            00000000005a0d650b64066505660264098404a6000000ab000000000000
-            0000005a0e650b640665056602640a8404a6000000ab0000000000000000
-            005a0f650b640665056602640b8404a6000000ab0000000000000000005a
-            10650b640665056602640c8404a6000000ab0000000000000000005a1165
-            0b640665056602640d8404a6000000ab0000000000000000005a12640e53
-            00
+            0464043c000000650964056505660264068404a6000000ab000000000000
+            0000005a0a650964056505660264078404a6000000ab0000000000000000
+            005a0b650964056505660264088404a6000000ab0000000000000000005a
+            0c650964056505660264098404a6000000ab0000000000000000005a0d65
+            09640565056602640a8404a6000000ab0000000000000000005a0e650964
+            0565056602640b8404a6000000ab0000000000000000005a0f6509640565
+            056602640c8404a6000000ab0000000000000000005a10640d5300
          138           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Search')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
@@ -1454,125 +1452,112 @@
                       44 CALL                     1
                       54 STORE_NAME               8 (meta)
                       56 LOAD_NAME                7 (dict)
                       58 LOAD_NAME                4 (__annotations__)
                       60 LOAD_CONST               4 ('meta')
                       62 STORE_SUBSCR
          
-         143          66 PUSH_NULL
-                      68 LOAD_NAME                6 (field)
-                      70 LOAD_NAME                9 (Criteria)
-                      72 KW_NAMES                 3
-                      74 PRECALL                  1
-                      78 CALL                     1
-                      88 STORE_NAME              10 (criteria)
-                      90 LOAD_NAME                9 (Criteria)
-                      92 LOAD_NAME                4 (__annotations__)
-                      94 LOAD_CONST               5 ('criteria')
-                      96 STORE_SUBSCR
+         147          66 LOAD_NAME                9 (property)
          
-         147         100 LOAD_NAME               11 (property)
+         148          68 LOAD_CONST               5 ('return')
+                      70 LOAD_NAME                5 (str)
+                      72 BUILD_TUPLE              2
+                      74 LOAD_CONST               6 (<code object notes, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 147>)
+                      76 MAKE_FUNCTION            4 (annotations)
          
-         148         102 LOAD_CONST               6 ('return')
-                     104 LOAD_NAME                5 (str)
-                     106 BUILD_TUPLE              2
-                     108 LOAD_CONST               7 (<code object notes, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 147>)
-                     110 MAKE_FUNCTION            4 (annotations)
+         147          78 PRECALL                  0
+                      82 CALL                     0
          
-         147         112 PRECALL                  0
-                     116 CALL                     0
+         148          92 STORE_NAME              10 (notes)
          
-         148         126 STORE_NAME              12 (notes)
+         151          94 LOAD_NAME                9 (property)
          
-         151         128 LOAD_NAME               11 (property)
+         152          96 LOAD_CONST               5 ('return')
+                      98 LOAD_NAME                5 (str)
+                     100 BUILD_TUPLE              2
+                     102 LOAD_CONST               7 (<code object type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 151>)
+                     104 MAKE_FUNCTION            4 (annotations)
          
-         152         130 LOAD_CONST               6 ('return')
-                     132 LOAD_NAME                5 (str)
-                     134 BUILD_TUPLE              2
-                     136 LOAD_CONST               8 (<code object type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 151>)
-                     138 MAKE_FUNCTION            4 (annotations)
+         151         106 PRECALL                  0
+                     110 CALL                     0
          
-         151         140 PRECALL                  0
-                     144 CALL                     0
+         152         120 STORE_NAME              11 (type)
          
-         152         154 STORE_NAME              13 (type)
+         155         122 LOAD_NAME                9 (property)
          
-         155         156 LOAD_NAME               11 (property)
+         156         124 LOAD_CONST               5 ('return')
+                     126 LOAD_NAME                5 (str)
+                     128 BUILD_TUPLE              2
+                     130 LOAD_CONST               8 (<code object prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 155>)
+                     132 MAKE_FUNCTION            4 (annotations)
          
-         156         158 LOAD_CONST               6 ('return')
-                     160 LOAD_NAME                5 (str)
-                     162 BUILD_TUPLE              2
-                     164 LOAD_CONST               9 (<code object prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 155>)
-                     166 MAKE_FUNCTION            4 (annotations)
-         
-         155         168 PRECALL                  0
-                     172 CALL                     0
+         155         134 PRECALL                  0
+                     138 CALL                     0
          
-         156         182 STORE_NAME              14 (prompt)
+         156         148 STORE_NAME              12 (prompt)
          
-         159         184 LOAD_NAME               11 (property)
+         159         150 LOAD_NAME                9 (property)
          
-         160         186 LOAD_CONST               6 ('return')
-                     188 LOAD_NAME                5 (str)
-                     190 BUILD_TUPLE              2
-                     192 LOAD_CONST              10 (<code object products, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 159>)
-                     194 MAKE_FUNCTION            4 (annotations)
+         160         152 LOAD_CONST               5 ('return')
+                     154 LOAD_NAME                5 (str)
+                     156 BUILD_TUPLE              2
+                     158 LOAD_CONST               9 (<code object products, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 159>)
+                     160 MAKE_FUNCTION            4 (annotations)
          
-         159         196 PRECALL                  0
-                     200 CALL                     0
+         159         162 PRECALL                  0
+                     166 CALL                     0
          
-         160         210 STORE_NAME              15 (products)
+         160         176 STORE_NAME              13 (products)
          
-         164         212 LOAD_NAME               11 (property)
+         164         178 LOAD_NAME                9 (property)
          
-         165         214 LOAD_CONST               6 ('return')
-                     216 LOAD_NAME                5 (str)
-                     218 BUILD_TUPLE              2
-                     220 LOAD_CONST              11 (<code object services, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 164>)
-                     222 MAKE_FUNCTION            4 (annotations)
+         165         180 LOAD_CONST               5 ('return')
+                     182 LOAD_NAME                5 (str)
+                     184 BUILD_TUPLE              2
+                     186 LOAD_CONST              10 (<code object services, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 164>)
+                     188 MAKE_FUNCTION            4 (annotations)
          
-         164         224 PRECALL                  0
-                     228 CALL                     0
+         164         190 PRECALL                  0
+                     194 CALL                     0
          
-         165         238 STORE_NAME              16 (services)
+         165         204 STORE_NAME              14 (services)
          
-         169         240 LOAD_NAME               11 (property)
+         169         206 LOAD_NAME                9 (property)
          
-         170         242 LOAD_CONST               6 ('return')
-                     244 LOAD_NAME                5 (str)
-                     246 BUILD_TUPLE              2
-                     248 LOAD_CONST              12 (<code object customers, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 169>)
-                     250 MAKE_FUNCTION            4 (annotations)
+         170         208 LOAD_CONST               5 ('return')
+                     210 LOAD_NAME                5 (str)
+                     212 BUILD_TUPLE              2
+                     214 LOAD_CONST              11 (<code object customers, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 169>)
+                     216 MAKE_FUNCTION            4 (annotations)
          
-         169         252 PRECALL                  0
-                     256 CALL                     0
+         169         218 PRECALL                  0
+                     222 CALL                     0
          
-         170         266 STORE_NAME              17 (customers)
+         170         232 STORE_NAME              15 (customers)
          
-         174         268 LOAD_NAME               11 (property)
+         174         234 LOAD_NAME                9 (property)
          
-         175         270 LOAD_CONST               6 ('return')
-                     272 LOAD_NAME                5 (str)
-                     274 BUILD_TUPLE              2
-                     276 LOAD_CONST              13 (<code object token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 174>)
-                     278 MAKE_FUNCTION            4 (annotations)
+         175         236 LOAD_CONST               5 ('return')
+                     238 LOAD_NAME                5 (str)
+                     240 BUILD_TUPLE              2
+                     242 LOAD_CONST              12 (<code object token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 174>)
+                     244 MAKE_FUNCTION            4 (annotations)
          
-         174         280 PRECALL                  0
-                     284 CALL                     0
+         174         246 PRECALL                  0
+                     250 CALL                     0
          
-         175         294 STORE_NAME              18 (token)
-                     296 LOAD_CONST              14 (None)
-                     298 RETURN_VALUE
+         175         260 STORE_NAME              16 (token)
+                     262 LOAD_CONST              13 (None)
+                     264 RETURN_VALUE
          consts
             'Search'
             'uid'
             'label'
             ('default_factory',)
             'meta'
-            'criteria'
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
@@ -1783,25 +1768,25 @@
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'token'
                firstlineno 174
                lnotab 0x0203
             None
-         names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'field', 'dict', 'meta', 'Criteria', 'criteria', 'property', 'notes', 'type', 'prompt', 'products', 'services', 'customers', 'token')
+         names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'field', 'dict', 'meta', 'property', 'notes', 'type', 'prompt', 'products', 'services', 'customers', 'token')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Search'
          firstlineno 138
          lnotab
-            0x0c020a010a012201220402010aff0e01020302010aff0e01020302010a
-            ff0e01020302010aff0e01020402010aff0e01020402010aff0e01020402
-            010aff0e01
+            0x0c020a010a01220502010aff0e01020302010aff0e01020302010aff0e
+            01020302010aff0e01020402010aff0e01020402010aff0e01020402010a
+            ff0e01
       'Search'
    names      ('hashlib', 'dataclasses', 'asdict', 'dataclass', 'field', 'enum', 'Enum', 'auto', 'typing', 'Any', 'List', 'Optional', 'Actor', 'Company', 'str', 'EventType', 'Event', 'Comment', 'Rating', 'Inclusion', 'Exclusion', 'Criteria', 'Maps', 'Search')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
    name       '<module>'
```

### Comparing `gandai-1.7.54/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xea3a5066 (Fri May 24 06:59:54 2024 UTC)
-files sz: 28739
+moddate:  0x70e75566 (Tue May 28 14:17:20 2024 UTC)
+files sz: 29338
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -248,168 +248,168 @@
                420 MAKE_FUNCTION            0
                422 STORE_NAME              41 (searches_comment_counts)
    
    375         424 LOAD_CONST              31 (<code object enriched_searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 375>)
                426 MAKE_FUNCTION            0
                428 STORE_NAME              42 (enriched_searches_query)
    
-   402         430 LOAD_CONST              11 ('return')
+   395         430 LOAD_CONST              11 ('return')
                432 LOAD_NAME                9 (pd)
                434 LOAD_ATTR               37 (DataFrame)
                444 BUILD_TUPLE              2
-               446 LOAD_CONST              32 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 402>)
+               446 LOAD_CONST              32 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 395>)
                448 MAKE_FUNCTION            4 (annotations)
                450 STORE_NAME              43 (actor)
    
-   416         452 LOAD_CONST              11 ('return')
+   409         452 LOAD_CONST              11 ('return')
                454 LOAD_NAME                9 (pd)
                456 LOAD_ATTR               37 (DataFrame)
                466 BUILD_TUPLE              2
-               468 LOAD_CONST              33 (<code object buyer, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 416>)
+               468 LOAD_CONST              33 (<code object buyer, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 409>)
                470 MAKE_FUNCTION            4 (annotations)
                472 STORE_NAME              44 (buyer)
    
-   478         474 LOAD_CONST              22 ('search_uid')
+   506         474 LOAD_CONST              22 ('search_uid')
                476 LOAD_NAME               33 (int)
                478 BUILD_TUPLE              2
-               480 LOAD_CONST              34 (<code object search_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 478>)
+               480 LOAD_CONST              34 (<code object search_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 506>)
                482 MAKE_FUNCTION            4 (annotations)
                484 STORE_NAME              45 (search_targets)
    
-   612         486 LOAD_CONST              22 ('search_uid')
+   640         486 LOAD_CONST              22 ('search_uid')
                488 LOAD_NAME               33 (int)
                490 LOAD_CONST              11 ('return')
                492 LOAD_NAME                9 (pd)
                494 LOAD_ATTR               37 (DataFrame)
                504 BUILD_TUPLE              4
-               506 LOAD_CONST              35 (<code object search_comments, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 612>)
+               506 LOAD_CONST              35 (<code object search_comments, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 640>)
                508 MAKE_FUNCTION            4 (annotations)
                510 STORE_NAME              46 (search_comments)
    
-   634         512 LOAD_CONST              22 ('search_uid')
+   662         512 LOAD_CONST              22 ('search_uid')
                514 LOAD_NAME               33 (int)
                516 LOAD_CONST              11 ('return')
                518 LOAD_NAME                9 (pd)
                520 LOAD_ATTR               37 (DataFrame)
                530 BUILD_TUPLE              4
-               532 LOAD_CONST              36 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 634>)
+               532 LOAD_CONST              36 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 662>)
                534 MAKE_FUNCTION            4 (annotations)
                536 STORE_NAME              47 (event)
    
-   646         538 LOAD_CONST              22 ('search_uid')
+   674         538 LOAD_CONST              22 ('search_uid')
                540 LOAD_NAME               33 (int)
                542 LOAD_CONST              11 ('return')
                544 LOAD_NAME                9 (pd)
                546 LOAD_ATTR               37 (DataFrame)
                556 BUILD_TUPLE              4
-               558 LOAD_CONST              37 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 646>)
+               558 LOAD_CONST              37 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 674>)
                560 MAKE_FUNCTION            4 (annotations)
                562 STORE_NAME              48 (event_history)
    
-   676         564 LOAD_CONST              22 ('search_uid')
+   704         564 LOAD_CONST              22 ('search_uid')
                566 LOAD_NAME               33 (int)
                568 LOAD_CONST              11 ('return')
                570 LOAD_NAME                9 (pd)
                572 LOAD_ATTR               37 (DataFrame)
                582 BUILD_TUPLE              4
-               584 LOAD_CONST              38 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 676>)
+               584 LOAD_CONST              38 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 704>)
                586 MAKE_FUNCTION            4 (annotations)
                588 STORE_NAME              49 (search_criteria_history)
    
-   705         590 LOAD_CONST              39 ('uid')
+   733         590 LOAD_CONST              39 ('uid')
                592 LOAD_NAME               33 (int)
                594 LOAD_CONST              11 ('return')
                596 LOAD_NAME               16 (ts)
                598 LOAD_ATTR               28 (models)
                608 LOAD_ATTR               25 (Search)
                618 BUILD_TUPLE              4
-               620 LOAD_CONST              40 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 705>)
+               620 LOAD_CONST              40 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 733>)
                622 MAKE_FUNCTION            4 (annotations)
                624 STORE_NAME              50 (find_search)
    
-   733         626 LOAD_CONST              41 ('searchToken')
+   761         626 LOAD_CONST              41 ('searchToken')
                628 LOAD_NAME               34 (str)
                630 LOAD_CONST              11 ('return')
                632 LOAD_NAME               16 (ts)
                634 LOAD_ATTR               28 (models)
                644 LOAD_ATTR               25 (Search)
                654 BUILD_TUPLE              4
-               656 LOAD_CONST              42 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 733>)
+               656 LOAD_CONST              42 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 761>)
                658 MAKE_FUNCTION            4 (annotations)
                660 STORE_NAME              51 (find_search_by_token)
    
-   742         662 LOAD_CONST              43 ('domain')
+   770         662 LOAD_CONST              43 ('domain')
                664 LOAD_NAME               34 (str)
                666 LOAD_CONST              11 ('return')
                668 LOAD_NAME               22 (Company)
                670 BUILD_TUPLE              4
-               672 LOAD_CONST              44 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 742>)
+               672 LOAD_CONST              44 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 770>)
                674 MAKE_FUNCTION            4 (annotations)
                676 STORE_NAME              52 (find_company_by_domain)
    
-   758         678 LOAD_CONST              45 ('email')
+   786         678 LOAD_CONST              45 ('email')
                680 LOAD_NAME               34 (str)
                682 LOAD_CONST              11 ('return')
                684 LOAD_NAME               22 (Company)
                686 BUILD_TUPLE              4
-               688 LOAD_CONST              46 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 758>)
+               688 LOAD_CONST              46 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 786>)
                690 MAKE_FUNCTION            4 (annotations)
                692 STORE_NAME              53 (find_actor_by_email)
    
-   774         694 LOAD_CONST              47 ('event_id')
+   802         694 LOAD_CONST              47 ('event_id')
                696 LOAD_NAME               33 (int)
                698 LOAD_CONST              11 ('return')
                700 LOAD_NAME               23 (Event)
                702 BUILD_TUPLE              4
-               704 LOAD_CONST              48 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 774>)
+               704 LOAD_CONST              48 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 802>)
                706 MAKE_FUNCTION            4 (annotations)
                708 STORE_NAME              54 (find_event_by_id)
    
-   793         710 LOAD_CONST              13 ('company')
+   821         710 LOAD_CONST              13 ('company')
                712 LOAD_NAME               22 (Company)
                714 LOAD_CONST              11 ('return')
                716 LOAD_CONST               1 (None)
                718 BUILD_TUPLE              4
-               720 LOAD_CONST              49 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 793>)
+               720 LOAD_CONST              49 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 821>)
                722 MAKE_FUNCTION            4 (annotations)
                724 STORE_NAME              55 (update_company)
    
-   822         726 LOAD_CONST              17 ('search')
+   850         726 LOAD_CONST              17 ('search')
                728 LOAD_NAME               25 (Search)
                730 LOAD_CONST              11 ('return')
                732 LOAD_CONST               1 (None)
                734 BUILD_TUPLE              4
-               736 LOAD_CONST              50 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 822>)
+               736 LOAD_CONST              50 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 850>)
                738 MAKE_FUNCTION            4 (annotations)
                740 STORE_NAME              56 (update_search)
    
-   845         742 LOAD_CONST              47 ('event_id')
+   873         742 LOAD_CONST              47 ('event_id')
                744 LOAD_NAME               33 (int)
                746 LOAD_CONST              11 ('return')
                748 LOAD_CONST               1 (None)
                750 BUILD_TUPLE              4
-               752 LOAD_CONST              51 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 845>)
+               752 LOAD_CONST              51 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 873>)
                754 MAKE_FUNCTION            4 (annotations)
                756 STORE_NAME              57 (mute_event)
    
-   868         758 LOAD_CONST              52 ('comment_id')
+   896         758 LOAD_CONST              52 ('comment_id')
                760 LOAD_NAME               33 (int)
                762 LOAD_CONST              11 ('return')
                764 LOAD_CONST               1 (None)
                766 BUILD_TUPLE              4
-               768 LOAD_CONST              53 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 868>)
+               768 LOAD_CONST              53 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 896>)
                770 MAKE_FUNCTION            4 (annotations)
                772 STORE_NAME              58 (delete_comment)
    
-   879         774 LOAD_CONST              22 ('search_uid')
+   907         774 LOAD_CONST              22 ('search_uid')
                776 LOAD_NAME               33 (int)
                778 LOAD_CONST              11 ('return')
                780 LOAD_CONST               1 (None)
                782 BUILD_TUPLE              4
-               784 LOAD_CONST              54 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 879>)
+               784 LOAD_CONST              54 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 907>)
                786 MAKE_FUNCTION            4 (annotations)
                788 STORE_NAME              59 (reset_inbox)
                790 LOAD_CONST               1 (None)
                792 RETURN_VALUE
    consts
       0
       None
@@ -2265,15 +2265,15 @@
                      456 LOAD_CONST               6 (0)
                      458 PRECALL                  1
                      462 CALL                     1
                      472 LOAD_FAST                2 (df)
                      474 LOAD_CONST              11 ('comment_count')
                      476 STORE_SUBSCR
          
-         399         480 LOAD_FAST                2 (df)
+         392         480 LOAD_FAST                2 (df)
                      482 RETURN_VALUE
          consts
             None
             'uid'
             'search_uid'
             'left'
             ('left_on', 'right_on', 'how')
@@ -2287,15 +2287,15 @@
          names      ('searches_query', 'validation_history', 'merge', 'fillna', 'searches_comment_counts')
          varnames   ('searches', 'recent_event_count', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'enriched_searches_query'
          firstlineno 375
-         lnotab 0x02011c021c02180108ff12043c013c013c013c0248013c09
+         lnotab 0x02011c021c02180108ff12043c013c013c013c0248013c02
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
@@ -2306,66 +2306,66 @@
             00000000007c01a0070000000000000000000000000000000000000000a6
             000000ab0000000000000000007c01a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000ac02a6020000ab0200
             000000000000007d027c02a0090000000000000000000000000000000000
             00000067006403a201ac02a6010000ab0100000000000000007d027c0263
             02640064006400a6020000ab020000000000000000010053002300310073
             047702780359007701010059000100010064005300
-         402           0 RESUME                   0
+         395           0 RESUME                   0
          
-         403           2 LOAD_GLOBAL              0 (db)
+         396           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         404          54 LOAD_FAST                0 (conn)
+         397          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         405          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         398          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         406         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
+         399         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
          
-         405         102 PRECALL                  1
+         398         102 PRECALL                  1
                      106 CALL                     1
          
-         404         116 PRECALL                  1
+         397         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         411         132 LOAD_GLOBAL             11 (NULL + pd)
+         404         132 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         412         248 LOAD_FAST                2 (df)
+         405         248 LOAD_FAST                2 (df)
                      250 LOAD_METHOD              9 (drop)
                      272 BUILD_LIST               0
                      274 LOAD_CONST               3 (('id', 'created', 'updated'))
                      276 LIST_EXTEND              1
                      278 KW_NAMES                 2
                      280 PRECALL                  1
                      284 CALL                     1
                      294 STORE_FAST               2 (df)
          
-         413         296 LOAD_FAST                2 (df)
+         406         296 LOAD_FAST                2 (df)
          
-         403         298 SWAP                     2
+         396         298 SWAP                     2
                      300 LOAD_CONST               0 (None)
                      302 LOAD_CONST               0 (None)
                      304 LOAD_CONST               0 (None)
                      306 PRECALL                  2
                      310 CALL                     2
                      320 POP_TOP
                      322 RETURN_VALUE
@@ -2393,15 +2393,15 @@
             ('id', 'created', 'updated')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'drop')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'actor'
-         firstlineno 402
+         firstlineno 395
          lnotab 0x020134011801160102ff0eff10077401300102f6
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -2414,54 +2414,54 @@
             000000ab0000000000000000007c01a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000ac02a6020000ab0200
             000000000000007d02640064006400a6020000ab02000000000000000001
             006e0b23003100730477027803590077010100590001000100640384007d
             037c02640419000000000000000000a00900000000000000000000000000
             000000000000007c03a6010000ab0100000000000000007c0264053c0000
             007c025300
-         416           0 RESUME                   0
+         409           0 RESUME                   0
          
-         417           2 LOAD_GLOBAL              0 (db)
+         410           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         418          54 LOAD_FAST                0 (conn)
+         411          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         419          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         412          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         420         100 LOAD_CONST               1 ("\n                SELECT \n                    e.id,\n                    e.domain,\n                    e.created as updated,\n                    a.name as updated_by, \n                    to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n                    c.name, \n                    c.description,\n                    c.source,\n                    c.meta->>'ownership' as ownership, \n                    c.meta->>'headquarters' as headquarters,\n                    c.meta->>'city' as city,\n                    c.meta->>'state' as state,\n                    c.meta->>'designation' as designation,\n                    c.meta->>'products' as products,\n                    c.meta->>'services' as services,\n                    c.meta->>'end_customer' as end_customer,\n                    c.meta->>'geographies' as geographies,\n                    c.meta->>'was_acquired' as was_acquired,\n                    c.meta->>'justification' as justification,\n                    c.meta->>'year_founded' as year_founded,\n                    c.meta->>'linkedin' as linkedin,\n                    c.meta->>'linkedin_range' as linkedin_range,\n                    c.meta->>'primary_contact' as primary_contact,\n                    c.meta->>'industry' as industry,\n                    c.meta->>'revenue_estimates' as revenue_estimates,\n                    c.meta->>'location_count' as location_count,\n                    c.meta->>'business_models' as business_models,\n                    c.meta->>'facility_size' as facility_size,\n                    c.meta,\n                    COALESCE(co.comments, '[]'::jsonb) as comments\n                FROM event e\n                LEFT JOIN actor a ON e.actor_key = a.key\n                LEFT JOIN company c ON e.domain = c.domain\n                LEFT JOIN comment co ON e.domain = co.domain\n                WHERE e.type = 'buyer'\n                ")
+         413         100 LOAD_CONST               1 ("\n                SELECT \n                    e.id,\n                    e.domain,\n                    e.created as updated,\n                    a.name as updated_by, \n                    to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n                    c.name, \n                    c.description,\n                    c.source,\n                    c.meta->>'ownership' as ownership, \n                    c.meta->>'headquarters' as headquarters,\n                    c.meta->>'city' as city,\n                    c.meta->>'state' as state,\n                    c.meta->>'designation' as designation,\n                    c.meta->>'products' as products,\n                    c.meta->>'services' as services,\n                    c.meta->>'end_customer' as end_customer,\n                    c.meta->>'geographies' as geographies,\n                    c.meta->>'was_acquired' as was_acquired,\n                    c.meta->>'justification' as justification,\n                    c.meta->>'year_founded' as year_founded,\n                    c.meta->>'linkedin' as linkedin,\n                    c.meta->>'linkedin_range' as linkedin_range,\n                    c.meta->>'primary_contact' as primary_contact,\n                    c.meta->>'industry' as industry,\n                    c.meta->>'revenue_estimates' as revenue_estimates,\n                    c.meta->>'location_count' as location_count,\n                    c.meta->>'business_models' as business_models,\n                    c.meta->>'facility_size' as facility_size,\n                    c.meta,\n                    COALESCE(co.comments, '[]'::jsonb) as comments\n                FROM event e\n                LEFT JOIN actor a ON e.actor_key = a.key\n                LEFT JOIN company c ON e.domain = c.domain\n                LEFT JOIN comment co ON e.domain = co.domain\n                WHERE e.type = 'buyer'\n                ")
          
-         419         102 PRECALL                  1
+         412         102 PRECALL                  1
                      106 CALL                     1
          
-         418         116 PRECALL                  1
+         411         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         460         132 LOAD_GLOBAL             11 (NULL + pd)
+         453         132 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         417         248 LOAD_CONST               0 (None)
+         410         248 LOAD_CONST               0 (None)
                      250 LOAD_CONST               0 (None)
                      252 LOAD_CONST               0 (None)
                      254 PRECALL                  2
                      258 CALL                     2
                      268 POP_TOP
                      270 JUMP_FORWARD            11 (to 294)
                  >>  272 PUSH_EXC_INFO
@@ -2472,30 +2472,30 @@
                      282 POP_EXCEPT
                      284 RERAISE                  1
                  >>  286 POP_TOP
                      288 POP_EXCEPT
                      290 POP_TOP
                      292 POP_TOP
          
-         462     >>  294 LOAD_CONST               3 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 462>)
+         455     >>  294 LOAD_CONST               3 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 455>)
                      296 MAKE_FUNCTION            0
                      298 STORE_FAST               3 (get_employees)
          
-         474         300 LOAD_FAST                2 (df)
+         467         300 LOAD_FAST                2 (df)
                      302 LOAD_CONST               4 ('meta')
                      304 BINARY_SUBSCR
                      314 LOAD_METHOD              9 (apply)
                      336 LOAD_FAST                3 (get_employees)
                      338 PRECALL                  1
                      342 CALL                     1
                      352 LOAD_FAST                2 (df)
                      354 LOAD_CONST               5 ('employees')
                      356 STORE_SUBSCR
          
-         475         360 LOAD_FAST                2 (df)
+         468         360 LOAD_FAST                2 (df)
                      362 RETURN_VALUE
          ExceptionTable:
            52 to 246 -> 272 [1] lasti
            272 to 278 -> 280 [3] lasti
            286 to 286 -> 280 [3] lasti
          consts
             None
@@ -2510,60 +2510,60 @@
                   0x97007c00a00000000000000000000000000000000000000000006401a6
                   010000ab010000000000000000721e09007403000000000000000000007c
                   00640119000000000000000000a6010000ab010000000000000000530023
                   0001005900640053007803590077017c00a0000000000000000000000000
                   0000000000000000006402a6010000ab010000000000000000721b7c0064
                   0219000000000000000000a0000000000000000000000000000000000000
                   0000006403a6010000ab010000000000000000530064005300
-               462           0 RESUME                   0
+               455           0 RESUME                   0
                
-               463           2 LOAD_FAST                0 (meta)
+               456           2 LOAD_FAST                0 (meta)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('employees')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE    30 (to 104)
                
-               465          44 NOP
+               458          44 NOP
                
-               466          46 LOAD_GLOBAL              3 (NULL + int)
+               459          46 LOAD_GLOBAL              3 (NULL + int)
                             58 LOAD_FAST                0 (meta)
                             60 LOAD_CONST               1 ('employees')
                             62 BINARY_SUBSCR
                             72 PRECALL                  1
                             76 CALL                     1
                             86 RETURN_VALUE
                        >>   88 PUSH_EXC_INFO
                
-               467          90 POP_TOP
+               460          90 POP_TOP
                
-               468          92 POP_EXCEPT
+               461          92 POP_EXCEPT
                             94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                        >>   98 COPY                     3
                            100 POP_EXCEPT
                            102 RERAISE                  1
                
-               469     >>  104 LOAD_FAST                0 (meta)
+               462     >>  104 LOAD_FAST                0 (meta)
                            106 LOAD_METHOD              0 (get)
                            128 LOAD_CONST               2 ('grata_employee_estimates')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 POP_JUMP_FORWARD_IF_FALSE    27 (to 200)
                
-               470         146 LOAD_FAST                0 (meta)
+               463         146 LOAD_FAST                0 (meta)
                            148 LOAD_CONST               2 ('grata_employee_estimates')
                            150 BINARY_SUBSCR
                            160 LOAD_METHOD              0 (get)
                            182 LOAD_CONST               3 ('count')
                            184 PRECALL                  1
                            188 CALL                     1
                            198 RETURN_VALUE
                
-               472     >>  200 LOAD_CONST               0 (None)
+               465     >>  200 LOAD_CONST               0 (None)
                            202 RETURN_VALUE
                ExceptionTable:
                  46 to 84 -> 88 [0]
                  88 to 90 -> 98 [1] lasti
                consts
                   None
                   'employees'
@@ -2571,25 +2571,25 @@
                   'count'
                names      ('get', 'int')
                varnames   ('meta',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_employees'
-               firstlineno 462
+               firstlineno 455
                lnotab 0x02012a0202012c0102010c012a013602
             'meta'
             'employees'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'apply')
          varnames   ('conn', 'result', 'df', 'get_employees')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'buyer'
-         firstlineno 416
+         firstlineno 409
          lnotab 0x020134011801160102ff0eff102a74d52e2d060c3c01
       code
          argcount  : 1
          nlocals   : 10
          stacksize : 6
          flags     : 3
          code
@@ -2611,59 +2611,59 @@
             010000ab0100000000000000007c04640c3c0000007c04640d1900000000
             0000000000a00a00000000000000000000000000000000000000007c07a6
             010000ab0100000000000000007c04640d3c0000007c04a00a0000000000
             0000000000000000000000000000007c08640eac0fa6020000ab02000000
             00000000007c0464103c0000007c04a00a00000000000000000000000000
             000000000000007c09640eac0fa6020000ab0200000000000000007c0464
             113c0000007c045300
-         478           0 RESUME                   0
+         506           0 RESUME                   0
          
-         481           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute','enrich')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        -- c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n        AND e.domain != ''\n    ;\n    ")
+         509           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute','enrich')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        -- c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n        AND e.domain != ''\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
-         545           6 LOAD_GLOBAL              0 (db)
+         573           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         546          58 LOAD_FAST                2 (conn)
+         574          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         547          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         575          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         548         120 LOAD_CONST               2 ('search_uid')
+         576         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         546         126 PRECALL                  2
+         574         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         550         142 LOAD_GLOBAL             11 (NULL + pd)
+         578         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         545         258 LOAD_CONST               0 (None)
+         573         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2674,93 +2674,93 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         552     >>  304 LOAD_CONST               4 ('return')
+         580     >>  304 LOAD_CONST               4 ('return')
                      306 LOAD_GLOBAL             18 (str)
                      318 BUILD_TUPLE              2
-                     320 LOAD_CONST               5 (<code object list_to_csv, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 552>)
+                     320 LOAD_CONST               5 (<code object list_to_csv, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 580>)
                      322 MAKE_FUNCTION            4 (annotations)
                      324 STORE_FAST               5 (list_to_csv)
          
-         564         326 LOAD_CONST               6 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 564>)
+         592         326 LOAD_CONST               6 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 592>)
                      328 MAKE_FUNCTION            0
                      330 STORE_FAST               6 (get_employees)
          
-         576         332 LOAD_CONST               7 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 576>)
+         604         332 LOAD_CONST               7 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 604>)
                      334 MAKE_FUNCTION            0
                      336 STORE_FAST               7 (get_ownership)
          
-         584         338 LOAD_CONST               8 (<code object get_state, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 584>)
+         612         338 LOAD_CONST               8 (<code object get_state, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 612>)
                      340 MAKE_FUNCTION            0
                      342 STORE_FAST               8 (get_state)
          
-         594         344 LOAD_CONST               9 (<code object get_city, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 594>)
+         622         344 LOAD_CONST               9 (<code object get_city, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 622>)
                      346 MAKE_FUNCTION            0
                      348 STORE_FAST               9 (get_city)
          
-         603         350 LOAD_FAST                4 (df)
+         631         350 LOAD_FAST                4 (df)
                      352 LOAD_CONST              10 ('end_customer')
                      354 BINARY_SUBSCR
                      364 LOAD_METHOD             10 (apply)
                      386 LOAD_FAST                5 (list_to_csv)
                      388 PRECALL                  1
                      392 CALL                     1
                      402 LOAD_FAST                4 (df)
                      404 LOAD_CONST              10 ('end_customer')
                      406 STORE_SUBSCR
          
-         604         410 LOAD_FAST                4 (df)
+         632         410 LOAD_FAST                4 (df)
                      412 LOAD_CONST              11 ('meta')
                      414 BINARY_SUBSCR
                      424 LOAD_METHOD             10 (apply)
                      446 LOAD_FAST                6 (get_employees)
                      448 PRECALL                  1
                      452 CALL                     1
                      462 LOAD_FAST                4 (df)
                      464 LOAD_CONST              12 ('employees')
                      466 STORE_SUBSCR
          
-         605         470 LOAD_FAST                4 (df)
+         633         470 LOAD_FAST                4 (df)
                      472 LOAD_CONST              13 ('ownership')
                      474 BINARY_SUBSCR
                      484 LOAD_METHOD             10 (apply)
                      506 LOAD_FAST                7 (get_ownership)
                      508 PRECALL                  1
                      512 CALL                     1
                      522 LOAD_FAST                4 (df)
                      524 LOAD_CONST              13 ('ownership')
                      526 STORE_SUBSCR
          
-         606         530 LOAD_FAST                4 (df)
+         634         530 LOAD_FAST                4 (df)
                      532 LOAD_METHOD             10 (apply)
                      554 LOAD_FAST                8 (get_state)
                      556 LOAD_CONST              14 (1)
                      558 KW_NAMES                15
                      560 PRECALL                  2
                      564 CALL                     2
                      574 LOAD_FAST                4 (df)
                      576 LOAD_CONST              16 ('state')
                      578 STORE_SUBSCR
          
-         607         582 LOAD_FAST                4 (df)
+         635         582 LOAD_FAST                4 (df)
                      584 LOAD_METHOD             10 (apply)
                      606 LOAD_FAST                9 (get_city)
                      608 LOAD_CONST              14 (1)
                      610 KW_NAMES                15
                      612 PRECALL                  2
                      616 CALL                     2
                      626 LOAD_FAST                4 (df)
                      628 LOAD_CONST              17 ('city')
                      630 STORE_SUBSCR
          
-         609         634 LOAD_FAST                4 (df)
+         637         634 LOAD_FAST                4 (df)
                      636 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2774,39 +2774,39 @@
                stacksize : 4
                flags     : 19
                code
                   0x970009007401000000000000000000006a0100000000000000007c00a6
                   010000ab0100000000000000007d016401a0020000000000000000000000
                   0000000000000000007c01a6010000ab0100000000000000007d027c0253
                   0023000100590064025300780359007701
-               552           0 RESUME                   0
+               580           0 RESUME                   0
                
-               554           2 NOP
+               582           2 NOP
                
-               555           4 LOAD_GLOBAL              1 (NULL + json)
+               583           4 LOAD_GLOBAL              1 (NULL + json)
                             16 LOAD_ATTR                1 (loads)
                             26 LOAD_FAST                0 (list_str)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 STORE_FAST               1 (list_data)
                
-               558          44 LOAD_CONST               1 (', ')
+               586          44 LOAD_CONST               1 (', ')
                             46 LOAD_METHOD              2 (join)
                             68 LOAD_FAST                1 (list_data)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 STORE_FAST               2 (csv_str)
                
-               560          86 LOAD_FAST                2 (csv_str)
+               588          86 LOAD_FAST                2 (csv_str)
                             88 RETURN_VALUE
                        >>   90 PUSH_EXC_INFO
                
-               561          92 POP_TOP
+               589          92 POP_TOP
                
-               562          94 POP_EXCEPT
+               590          94 POP_EXCEPT
                             96 LOAD_CONST               2 ('')
                             98 RETURN_VALUE
                        >>  100 COPY                     3
                            102 POP_EXCEPT
                            104 RERAISE                  1
                ExceptionTable:
                  4 to 86 -> 90 [0]
@@ -2817,75 +2817,75 @@
                   ''
                names      ('json', 'loads', 'join')
                varnames   ('list_str', 'list_data', 'csv_str')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'list_to_csv'
-               firstlineno 552
+               firstlineno 580
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
-               564           0 RESUME                   0
+               592           0 RESUME                   0
                
-               565           2 LOAD_FAST                0 (meta)
+               593           2 LOAD_FAST                0 (meta)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('employees')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE    30 (to 104)
                
-               567          44 NOP
+               595          44 NOP
                
-               568          46 LOAD_GLOBAL              3 (NULL + int)
+               596          46 LOAD_GLOBAL              3 (NULL + int)
                             58 LOAD_FAST                0 (meta)
                             60 LOAD_CONST               1 ('employees')
                             62 BINARY_SUBSCR
                             72 PRECALL                  1
                             76 CALL                     1
                             86 RETURN_VALUE
                        >>   88 PUSH_EXC_INFO
                
-               569          90 POP_TOP
+               597          90 POP_TOP
                
-               570          92 POP_EXCEPT
+               598          92 POP_EXCEPT
                             94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                        >>   98 COPY                     3
                            100 POP_EXCEPT
                            102 RERAISE                  1
                
-               571     >>  104 LOAD_FAST                0 (meta)
+               599     >>  104 LOAD_FAST                0 (meta)
                            106 LOAD_METHOD              0 (get)
                            128 LOAD_CONST               2 ('grata_employee_estimates')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 POP_JUMP_FORWARD_IF_FALSE    27 (to 200)
                
-               572         146 LOAD_FAST                0 (meta)
+               600         146 LOAD_FAST                0 (meta)
                            148 LOAD_CONST               2 ('grata_employee_estimates')
                            150 BINARY_SUBSCR
                            160 LOAD_METHOD              0 (get)
                            182 LOAD_CONST               3 ('count')
                            184 PRECALL                  1
                            188 CALL                     1
                            198 RETURN_VALUE
                
-               574     >>  200 LOAD_CONST               0 (None)
+               602     >>  200 LOAD_CONST               0 (None)
                            202 RETURN_VALUE
                ExceptionTable:
                  46 to 84 -> 88 [0]
                  88 to 90 -> 98 [1] lasti
                consts
                   None
                   'employees'
@@ -2893,57 +2893,57 @@
                   'count'
                names      ('get', 'int')
                varnames   ('meta',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_employees'
-               firstlineno 564
+               firstlineno 592
                lnotab 0x02012a0202012c0102010c012a013602
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 19
                code
                   0x97007c0064016b02000000007202640253007c0064036b020000000072
                   02640453007c005300
-               576           0 RESUME                   0
+               604           0 RESUME                   0
                
-               577           2 LOAD_FAST                0 (ownership)
+               605           2 LOAD_FAST                0 (ownership)
                              4 LOAD_CONST               1 ('Bootstrapped')
                              6 COMPARE_OP               2 (==)
                             12 POP_JUMP_FORWARD_IF_FALSE     2 (to 18)
                
-               578          14 LOAD_CONST               2 ('Private')
+               606          14 LOAD_CONST               2 ('Private')
                             16 RETURN_VALUE
                
-               579     >>   18 LOAD_FAST                0 (ownership)
+               607     >>   18 LOAD_FAST                0 (ownership)
                             20 LOAD_CONST               3 ('Investor Backed')
                             22 COMPARE_OP               2 (==)
                             28 POP_JUMP_FORWARD_IF_FALSE     2 (to 34)
                
-               580          30 LOAD_CONST               4 ('Venture Capital')
+               608          30 LOAD_CONST               4 ('Venture Capital')
                             32 RETURN_VALUE
                
-               582     >>   34 LOAD_FAST                0 (ownership)
+               610     >>   34 LOAD_FAST                0 (ownership)
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
-               firstlineno 576
+               firstlineno 604
                lnotab 0x02010c0104010c010402
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 19
                code
@@ -2953,78 +2953,78 @@
                   00ab010000000000000000725a7c00640219000000000000000000a00100
                   000000000000000000000000000000000000006403a6010000ab01000000
                   0000000000640419000000000000000000a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d017406000000
                   000000000000006a0400000000000000006a050000000000000000a00000
                   000000000000000000000000000000000000007c016405a6020000ab0200
                   000000000000007d027c02530064005300
-               584           0 RESUME                   0
+               612           0 RESUME                   0
                
-               585           2 LOAD_FAST                0 (row)
+               613           2 LOAD_FAST                0 (row)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('state')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE     8 (to 60)
                
-               586          44 LOAD_FAST                0 (row)
+               614          44 LOAD_FAST                0 (row)
                             46 LOAD_CONST               1 ('state')
                             48 BINARY_SUBSCR
                             58 RETURN_VALUE
                
-               587     >>   60 LOAD_FAST                0 (row)
+               615     >>   60 LOAD_FAST                0 (row)
                             62 LOAD_METHOD              0 (get)
                             84 LOAD_CONST               2 ('headquarters')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_JUMP_FORWARD_IF_FALSE    90 (to 282)
                
-               588         102 LOAD_FAST                0 (row)
+               616         102 LOAD_FAST                0 (row)
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
                
-               589         204 LOAD_GLOBAL              6 (ts)
+               617         204 LOAD_GLOBAL              6 (ts)
                            216 LOAD_ATTR                4 (constants)
                            226 LOAD_ATTR                5 (STATE_NAMES)
                            236 LOAD_METHOD              0 (get)
                            258 LOAD_FAST                1 (state_name)
                            260 LOAD_CONST               5 ('')
                            262 PRECALL                  2
                            266 CALL                     2
                            276 STORE_FAST               2 (state_code)
                
-               590         278 LOAD_FAST                2 (state_code)
+               618         278 LOAD_FAST                2 (state_code)
                            280 RETURN_VALUE
                
-               592     >>  282 LOAD_CONST               0 (None)
+               620     >>  282 LOAD_CONST               0 (None)
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
-               firstlineno 584
+               firstlineno 612
                lnotab 0x02012a0110012a0166014a010402
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
@@ -3032,67 +3032,67 @@
                   010000ab01000000000000000072087c0064011900000000000000000053
                   007c00a00000000000000000000000000000000000000000006402a60100
                   00ab01000000000000000072357c00640219000000000000000000a00100
                   000000000000000000000000000000000000006403a6010000ab01000000
                   0000000000640419000000000000000000a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d017c01530064
                   005300
-               594           0 RESUME                   0
+               622           0 RESUME                   0
                
-               595           2 LOAD_FAST                0 (row)
+               623           2 LOAD_FAST                0 (row)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('city')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE     8 (to 60)
                
-               596          44 LOAD_FAST                0 (row)
+               624          44 LOAD_FAST                0 (row)
                             46 LOAD_CONST               1 ('city')
                             48 BINARY_SUBSCR
                             58 RETURN_VALUE
                
-               597     >>   60 LOAD_FAST                0 (row)
+               625     >>   60 LOAD_FAST                0 (row)
                             62 LOAD_METHOD              0 (get)
                             84 LOAD_CONST               2 ('headquarters')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_JUMP_FORWARD_IF_FALSE    53 (to 208)
                
-               598         102 LOAD_FAST                0 (row)
+               626         102 LOAD_FAST                0 (row)
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
                
-               599         204 LOAD_FAST                1 (city_name)
+               627         204 LOAD_FAST                1 (city_name)
                            206 RETURN_VALUE
                
-               601     >>  208 LOAD_CONST               0 (None)
+               629     >>  208 LOAD_CONST               0 (None)
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
-               firstlineno 594
+               firstlineno 622
                lnotab 0x02012a0110012a0166010402
             'end_customer'
             'meta'
             'employees'
             'ownership'
             1
             ('axis',)
@@ -3100,15 +3100,15 @@
             'city'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'str', 'apply')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df', 'list_to_csv', 'get_employees', 'get_ownership', 'get_state', 'get_city')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_targets'
-         firstlineno 478
+         firstlineno 506
          lnotab
             0x0203044034011801260106fe100474fb2e07160c060c0608060a06093c
             013c013c0134013402
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
@@ -3121,59 +3121,59 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         612           0 RESUME                   0
+         640           0 RESUME                   0
          
-         613           2 LOAD_CONST               1 ("\n    SELECT \n        e.*,\n        a.name as author\n    FROM event e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    WHERE\n        e.type = 'comment'\n        AND e.domain is null\n        AND search_uid = :search_uid\n    ")
+         641           2 LOAD_CONST               1 ("\n    SELECT \n        e.*,\n        a.name as author\n    FROM event e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    WHERE\n        e.type = 'comment'\n        AND e.domain is null\n        AND search_uid = :search_uid\n    ")
                        4 STORE_FAST               1 (statement)
          
-         625           6 LOAD_GLOBAL              0 (db)
+         653           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         626          58 LOAD_FAST                2 (conn)
+         654          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         627          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         655          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         628         120 LOAD_CONST               2 ('search_uid')
+         656         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         626         126 PRECALL                  2
+         654         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         630         142 LOAD_GLOBAL             11 (NULL + pd)
+         658         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         625         258 LOAD_CONST               0 (None)
+         653         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3184,15 +3184,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         631     >>  304 LOAD_FAST                4 (df)
+         659     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3201,15 +3201,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_comments'
-         firstlineno 612
+         firstlineno 640
          lnotab 0x0201040c34011801260106fe100474fb2e06
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3220,56 +3220,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         634           0 RESUME                   0
+         662           0 RESUME                   0
          
-         635           2 LOAD_GLOBAL              0 (db)
+         663           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         636          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         664          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         641          58 LOAD_FAST                1 (conn)
+         669          58 LOAD_FAST                1 (conn)
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
          
-         642         142 LOAD_GLOBAL             11 (NULL + pd)
+         670         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         635         258 LOAD_CONST               0 (None)
+         663         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3280,15 +3280,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         643     >>  304 LOAD_FAST                4 (df)
+         671     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3297,15 +3297,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event'
-         firstlineno 634
+         firstlineno 662
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3317,65 +3317,65 @@
             007c01a6010000ab01000000000000000064027c006901a6020000ab0200
             000000000000007d03740f000000000000000000006a0800000000000000
             007c03a0090000000000000000000000000000000000000000a6000000ab
             0000000000000000007c03a00a0000000000000000000000000000000000
             000000a6000000ab000000000000000000ac03a6020000ab020000000000
             0000007d04640064006400a6020000ab02000000000000000001006e0b23
             0031007304770278035900770101005900010001007c045300
-         646           0 RESUME                   0
+         674           0 RESUME                   0
          
-         647           2 LOAD_GLOBAL              1 (NULL + isinstance)
+         675           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (search_uid)
                       16 LOAD_GLOBAL              2 (int)
                       28 PRECALL                  2
                       32 CALL                     2
                       42 POP_JUMP_FORWARD_IF_TRUE     2 (to 48)
                       44 LOAD_ASSERTION_ERROR
                       46 RAISE_VARARGS            1
          
-         648     >>   48 LOAD_CONST               1 ("\n    SELECT \n        e.id,\n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.domain,\n        e.data,\n        a.type as actor_type,\n        a.key as actor_key,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type != 'mute'\n    ORDER BY created DESC\n    ;\n\n    ")
+         676     >>   48 LOAD_CONST               1 ("\n    SELECT \n        e.id,\n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.domain,\n        e.data,\n        a.type as actor_type,\n        a.key as actor_key,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type != 'mute'\n    ORDER BY created DESC\n    ;\n\n    ")
                       50 STORE_FAST               1 (statement)
          
-         670          52 LOAD_GLOBAL              4 (db)
+         698          52 LOAD_GLOBAL              4 (db)
                       64 LOAD_METHOD              3 (connect)
                       86 PRECALL                  0
                       90 CALL                     0
                      100 BEFORE_WITH
                      102 STORE_FAST               2 (conn)
          
-         671         104 LOAD_FAST                2 (conn)
+         699         104 LOAD_FAST                2 (conn)
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
          
-         672         188 LOAD_GLOBAL             15 (NULL + pd)
+         700         188 LOAD_GLOBAL             15 (NULL + pd)
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
          
-         670         304 LOAD_CONST               0 (None)
+         698         304 LOAD_CONST               0 (None)
                      306 LOAD_CONST               0 (None)
                      308 LOAD_CONST               0 (None)
                      310 PRECALL                  2
                      314 CALL                     2
                      324 POP_TOP
                      326 JUMP_FORWARD            11 (to 350)
                  >>  328 PUSH_EXC_INFO
@@ -3386,15 +3386,15 @@
                      338 POP_EXCEPT
                      340 RERAISE                  1
                  >>  342 POP_TOP
                      344 POP_EXCEPT
                      346 POP_TOP
                      348 POP_TOP
          
-         673     >>  350 LOAD_FAST                4 (df)
+         701     >>  350 LOAD_FAST                4 (df)
                      352 RETURN_VALUE
          ExceptionTable:
            102 to 302 -> 328 [1] lasti
            328 to 334 -> 336 [3] lasti
            342 to 342 -> 336 [3] lasti
          consts
             None
@@ -3403,15 +3403,15 @@
             ('columns',)
          names      ('isinstance', 'int', 'db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event_history'
-         firstlineno 646
+         firstlineno 674
          lnotab 0x02012e0104163401540174fe2e03
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3422,56 +3422,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         676           0 RESUME                   0
+         704           0 RESUME                   0
          
-         678           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
+         706           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
-         696           6 LOAD_GLOBAL              0 (db)
+         724           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         697          58 LOAD_FAST                2 (conn)
+         725          58 LOAD_FAST                2 (conn)
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
          
-         698         142 LOAD_GLOBAL             11 (NULL + pd)
+         726         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         696         258 LOAD_CONST               0 (None)
+         724         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3482,15 +3482,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         699     >>  304 LOAD_FAST                4 (df)
+         727     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3499,15 +3499,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_criteria_history'
-         firstlineno 676
+         firstlineno 704
          lnotab 0x020204123401540174fe2e03
       'uid'
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 7
          flags     : 3
@@ -3525,96 +3525,96 @@
             000000000000007d05741300000000000000000000741400000000000000
             0000006a0b00000000000000006a0c00000000000000007c05a6020000ab
             0200000000000000007d067c066a0d0000000000000000a00e0000000000
             0000000000000000000000000000006403a6010000ab0100000000000000
             006404190000000000000000007c066a0f000000000000000064053c0000
             00640064006400a6020000ab02000000000000000001006e0b2300310073
             04770278035900770101005900010001007c065300
-         705           0 RESUME                   0
+         733           0 RESUME                   0
          
-         706           2 LOAD_GLOBAL              0 (db)
+         734           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         707          54 LOAD_CONST               1 ("\n            SELECT \n                uid, \n                label, \n                meta, \n                meta->>'next_due_date' as next_due_date,\n                meta->>'notes' as notes,\n                COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            ")
+         735          54 LOAD_CONST               1 ("\n            SELECT \n                uid, \n                label, \n                meta \n                -- meta->>'next_due_date' as next_due_date,\n                -- meta->>'notes' as notes,\n                -- COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            -- LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            ")
                       56 STORE_FAST               2 (statement)
          
-         720          58 LOAD_FAST                1 (conn)
+         748          58 LOAD_FAST                1 (conn)
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
          
-         722         142 LOAD_FAST                3 (result)
+         750         142 LOAD_FAST                3 (result)
                      144 LOAD_METHOD              5 (fetchone)
                      166 PRECALL                  0
                      170 CALL                     0
                      180 STORE_FAST               4 (row)
          
-         723         182 LOAD_FAST                4 (row)
+         751         182 LOAD_FAST                4 (row)
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 214)
          
-         724         186 NOP
+         752         186 NOP
          
-         706         188 LOAD_CONST               0 (None)
+         734         188 LOAD_CONST               0 (None)
                      190 LOAD_CONST               0 (None)
                      192 LOAD_CONST               0 (None)
                      194 PRECALL                  2
                      198 CALL                     2
                      208 POP_TOP
                      210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         726     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         754     >>  214 LOAD_GLOBAL             13 (NULL + dict)
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
          
-         727         308 LOAD_GLOBAL             19 (NULL + from_dict)
+         755         308 LOAD_GLOBAL             19 (NULL + from_dict)
                      320 LOAD_GLOBAL             20 (ts)
                      332 LOAD_ATTR               11 (models)
                      342 LOAD_ATTR               12 (Search)
                      352 LOAD_FAST                5 (obj)
                      354 PRECALL                  2
                      358 CALL                     2
                      368 STORE_FAST               6 (search)
          
-         728         370 LOAD_FAST                6 (search)
+         756         370 LOAD_FAST                6 (search)
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
          
-         706         450 LOAD_CONST               0 (None)
+         734         450 LOAD_CONST               0 (None)
                      452 LOAD_CONST               0 (None)
                      454 LOAD_CONST               0 (None)
                      456 PRECALL                  2
                      460 CALL                     2
                      470 POP_TOP
                      472 JUMP_FORWARD            11 (to 496)
                  >>  474 PUSH_EXC_INFO
@@ -3625,72 +3625,72 @@
                      484 POP_EXCEPT
                      486 RERAISE                  1
                  >>  488 POP_TOP
                      490 POP_EXCEPT
                      492 POP_TOP
                      494 POP_TOP
          
-         730     >>  496 LOAD_FAST                6 (search)
+         758     >>  496 LOAD_FAST                6 (search)
                      498 RETURN_VALUE
          ExceptionTable:
            52 to 186 -> 474 [1] lasti
            214 to 448 -> 474 [1] lasti
            474 to 480 -> 482 [3] lasti
            488 to 488 -> 482 [3] lasti
          consts
             None
-            "\n            SELECT \n                uid, \n                label, \n                meta, \n                meta->>'next_due_date' as next_due_date,\n                meta->>'notes' as notes,\n                COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            "
+            "\n            SELECT \n                uid, \n                label, \n                meta \n                -- meta->>'next_due_date' as next_due_date,\n                -- meta->>'notes' as notes,\n                -- COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            -- LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            "
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
-         firstlineno 705
+         firstlineno 733
          lnotab 0x02013401040d54022801040102ee1a145e013e0150ea2e18
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
-         733           0 RESUME                   0
+         761           0 RESUME                   0
          
-         734           2 LOAD_GLOBAL              1 (NULL + searches_query)
+         762           2 LOAD_GLOBAL              1 (NULL + searches_query)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               1 (searches)
          
-         735          30 LOAD_FAST                1 (searches)
+         763          30 LOAD_FAST                1 (searches)
                       32 LOAD_FAST                1 (searches)
                       34 LOAD_CONST               1 ('searchToken')
                       36 BINARY_SUBSCR
                       46 LOAD_FAST                0 (searchToken)
                       48 COMPARE_OP               2 (==)
                       54 BINARY_SUBSCR
                       64 STORE_FAST               2 (search)
          
-         736          66 LOAD_FAST                2 (search)
+         764          66 LOAD_FAST                2 (search)
                       68 LOAD_ATTR                1 (empty)
                       78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
          
-         737          80 LOAD_CONST               0 (None)
+         765          80 LOAD_CONST               0 (None)
                       82 RETURN_VALUE
          
-         739     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
+         767     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
                       96 LOAD_FAST                2 (search)
                       98 LOAD_ATTR                3 (iloc)
                      108 LOAD_CONST               2 (0)
                      110 BINARY_SUBSCR
                      120 LOAD_CONST               3 ('uid')
                      122 BINARY_SUBSCR
                      132 PRECALL                  1
@@ -3703,15 +3703,15 @@
             'uid'
          names      ('searches_query', 'empty', 'find_search', 'iloc')
          varnames   ('searchToken', 'searches', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_token'
-         firstlineno 733
+         firstlineno 761
          lnotab 0x02011c0124010e010402
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3725,41 +3725,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         742           0 RESUME                   0
+         770           0 RESUME                   0
          
-         743           2 LOAD_GLOBAL              0 (db)
+         771           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         744          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         772          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         749          58 LOAD_FAST                1 (conn)
+         777          58 LOAD_FAST                1 (conn)
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
          
-         743         142 LOAD_CONST               0 (None)
+         771         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3770,24 +3770,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         751     >>  188 LOAD_FAST                3 (result)
+         779     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         752         210 LOAD_CONST               0 (None)
+         780         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         754     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         782     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3795,15 +3795,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         755         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         783         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Company)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3816,15 +3816,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 742
+         firstlineno 770
          lnotab 0x02013401040554fa2e08160104028201
       'email'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3839,41 +3839,41 @@
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000006a0c00000000000000006a0d00000000000000007c
             04a6020000ab0200000000000000005300
-         758           0 RESUME                   0
+         786           0 RESUME                   0
          
-         759           2 LOAD_GLOBAL              0 (db)
+         787           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         760          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
+         788          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
                       56 STORE_FAST               2 (statement)
          
-         765          58 LOAD_FAST                1 (conn)
+         793          58 LOAD_FAST                1 (conn)
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
          
-         759         142 LOAD_CONST               0 (None)
+         787         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3884,24 +3884,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         767     >>  188 LOAD_FAST                3 (result)
+         795     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         768         210 LOAD_CONST               0 (None)
+         796         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         770     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         798     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3909,15 +3909,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         771         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         799         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (ts)
                      368 LOAD_ATTR               12 (models)
                      378 LOAD_ATTR               13 (Actor)
                      388 LOAD_FAST                4 (obj)
                      390 PRECALL                  2
                      394 CALL                     2
                      404 RETURN_VALUE
@@ -3932,15 +3932,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'ts', 'models', 'Actor')
          varnames   ('email', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_actor_by_email'
-         firstlineno 758
+         firstlineno 786
          lnotab 0x02013401040554fa2e08160104028201
       'event_id'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3954,41 +3954,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         774           0 RESUME                   0
+         802           0 RESUME                   0
          
-         775           2 LOAD_GLOBAL              0 (db)
+         803           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         776          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
+         804          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         781          58 LOAD_FAST                1 (conn)
+         809          58 LOAD_FAST                1 (conn)
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
          
-         775         142 LOAD_CONST               0 (None)
+         803         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3999,24 +3999,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         783     >>  188 LOAD_FAST                3 (result)
+         811     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         784         210 LOAD_CONST               0 (None)
+         812         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         786     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         814     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -4024,15 +4024,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         787         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         815         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Event)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -4045,15 +4045,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Event')
          varnames   ('event_id', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_event_by_id'
-         firstlineno 774
+         firstlineno 802
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 12
          flags     : 3
          code
@@ -4065,71 +4065,71 @@
             000000000000007c006a0800000000000000007c006a0900000000000000
             007415000000000000000000006a0b00000000000000007c006a0c000000
             0000000000a6010000ab01000000000000000064029c06a6020000ab0200
             0000000000000001007c01a00d0000000000000000000000000000000000
             000000a6000000ab0000000000000000000100640064006400a6020000ab
             020000000000000000010064005300230031007304770278035900770101
             0059000100010064005300
-         793           0 RESUME                   0
+         821           0 RESUME                   0
          
-         794           2 LOAD_GLOBAL              0 (db)
+         822           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         795          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
+         823          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         807          58 LOAD_FAST                1 (conn)
+         835          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         808          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         836          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         810         120 LOAD_FAST                0 (company)
+         838         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (uid)
          
-         811         132 LOAD_FAST                0 (company)
+         839         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (name)
          
-         812         144 LOAD_FAST                0 (company)
+         840         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (description)
          
-         813         156 LOAD_FAST                0 (company)
+         841         156 LOAD_FAST                0 (company)
                      158 LOAD_ATTR                8 (domain)
          
-         814         168 LOAD_FAST                0 (company)
+         842         168 LOAD_FAST                0 (company)
                      170 LOAD_ATTR                9 (source)
          
-         815         180 LOAD_GLOBAL             21 (NULL + json)
+         843         180 LOAD_GLOBAL             21 (NULL + json)
                      192 LOAD_ATTR               11 (dumps)
                      202 LOAD_FAST                0 (company)
                      204 LOAD_ATTR               12 (meta)
                      214 PRECALL                  1
                      218 CALL                     1
          
-         809         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
+         837         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
                      230 BUILD_CONST_KEY_MAP      6
          
-         807         232 PRECALL                  2
+         835         232 PRECALL                  2
                      236 CALL                     2
                      246 POP_TOP
          
-         819         248 LOAD_FAST                1 (conn)
+         847         248 LOAD_FAST                1 (conn)
                      250 LOAD_METHOD             13 (commit)
                      272 PRECALL                  0
                      276 CALL                     0
                      286 POP_TOP
          
-         794         288 LOAD_CONST               0 (None)
+         822         288 LOAD_CONST               0 (None)
                      290 LOAD_CONST               0 (None)
                      292 LOAD_CONST               0 (None)
                      294 PRECALL                  2
                      298 CALL                     2
                      308 POP_TOP
                      310 LOAD_CONST               0 (None)
                      312 RETURN_VALUE
@@ -4156,15 +4156,15 @@
             ('uid', 'name', 'description', 'domain', 'source', 'meta')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'uid', 'name', 'description', 'domain', 'source', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 793
+         firstlineno 821
          lnotab 0x02013401040c180126020c010c010c010c010c0130fa04fe100c28e7
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
@@ -4174,58 +4174,58 @@
             006a0400000000000000006401a6010000ab010000000000000000740b00
             0000000000000000006a0600000000000000007c006a0700000000000000
             00a6010000ab0100000000000000007c006a08000000000000000064029c
             02a6020000ab02000000000000000001007c01a009000000000000000000
             0000000000000000000000a6000000ab0000000000000000000100640064
             006400a6020000ab02000000000000000001006400530023003100730477
             02780359007701010059000100010064005300
-         822           0 RESUME                   0
+         850           0 RESUME                   0
          
-         823           2 LOAD_GLOBAL              0 (db)
+         851           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         824          54 LOAD_FAST                1 (conn)
+         852          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         825          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         853          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         826         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
+         854         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
          
-         825         102 PRECALL                  1
+         853         102 PRECALL                  1
                      106 CALL                     1
          
-         835         116 LOAD_GLOBAL             11 (NULL + json)
+         863         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (meta)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         836         164 LOAD_FAST                0 (search)
+         864         164 LOAD_FAST                0 (search)
                      166 LOAD_ATTR                8 (uid)
          
-         834         176 LOAD_CONST               2 (('meta', 'uid'))
+         862         176 LOAD_CONST               2 (('meta', 'uid'))
                      178 BUILD_CONST_KEY_MAP      2
          
-         824         180 PRECALL                  2
+         852         180 PRECALL                  2
                      184 CALL                     2
                      194 POP_TOP
          
-         839         196 LOAD_FAST                1 (conn)
+         867         196 LOAD_FAST                1 (conn)
                      198 LOAD_METHOD              9 (commit)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 POP_TOP
          
-         823         236 LOAD_CONST               0 (None)
+         851         236 LOAD_CONST               0 (None)
                      238 LOAD_CONST               0 (None)
                      240 LOAD_CONST               0 (None)
                      242 PRECALL                  2
                      246 CALL                     2
                      256 POP_TOP
                      258 LOAD_CONST               0 (None)
                      260 RETURN_VALUE
@@ -4252,15 +4252,15 @@
             ('meta', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'meta', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 822
+         firstlineno 850
          lnotab 0x020134011801160102ff0e0a30010cfe04f6100f28f0
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4271,61 +4271,61 @@
             006901a6020000ab02000000000000000001007c01a00200000000000000
             000000000000000000000000007407000000000000000000006a04000000
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00500000000000000000000000000000000000000
             00a6000000ab0000000000000000000100640064006400a6020000ab0200
             000000000000000100640053002300310073047702780359007701010059
             000100010064005300
-         845           0 RESUME                   0
+         873           0 RESUME                   0
          
-         847           2 LOAD_GLOBAL              0 (db)
+         875           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         848          54 LOAD_FAST                1 (conn)
+         876          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         849          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         877          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         850         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
+         878         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
          
-         849         102 PRECALL                  1
+         877         102 PRECALL                  1
                      106 CALL                     1
          
-         858         116 LOAD_CONST               2 ('event_id')
+         886         116 LOAD_CONST               2 ('event_id')
                      118 LOAD_FAST                0 (event_id)
          
-         857         120 BUILD_MAP                1
+         885         120 BUILD_MAP                1
          
-         848         122 PRECALL                  2
+         876         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         861         138 LOAD_FAST                1 (conn)
+         889         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         862         216 LOAD_FAST                1 (conn)
+         890         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              5 (commit)
                      240 PRECALL                  0
                      244 CALL                     0
                      254 POP_TOP
          
-         847         256 LOAD_CONST               0 (None)
+         875         256 LOAD_CONST               0 (None)
                      258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 PRECALL                  2
                      266 CALL                     2
                      276 POP_TOP
                      278 LOAD_CONST               0 (None)
                      280 RETURN_VALUE
@@ -4353,15 +4353,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('event_id', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'mute_event'
-         firstlineno 845
+         firstlineno 873
          lnotab 0x020234011801160102ff0e0904ff02f7100d4e0128f1
       'comment_id'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -4373,58 +4373,58 @@
             0064027c006901a6020000ab02000000000000000001007c01a002000000
             00000000000000000000000000000000007407000000000000000000006a
             0400000000000000006403a6010000ab010000000000000000a6010000ab
             01000000000000000001007c01a005000000000000000000000000000000
             0000000000a6000000ab0000000000000000000100640064006400a60200
             00ab02000000000000000001006400530023003100730477027803590077
             01010059000100010064005300
-         868           0 RESUME                   0
+         896           0 RESUME                   0
          
-         869           2 LOAD_GLOBAL              0 (db)
+         897           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         870          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
+         898          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         874          58 LOAD_FAST                1 (conn)
+         902          58 LOAD_FAST                1 (conn)
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
          
-         875         142 LOAD_FAST                1 (conn)
+         903         142 LOAD_FAST                1 (conn)
                      144 LOAD_METHOD              2 (execute)
                      166 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      178 LOAD_ATTR                4 (text)
                      188 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      190 PRECALL                  1
                      194 CALL                     1
                      204 PRECALL                  1
                      208 CALL                     1
                      218 POP_TOP
          
-         876         220 LOAD_FAST                1 (conn)
+         904         220 LOAD_FAST                1 (conn)
                      222 LOAD_METHOD              5 (commit)
                      244 PRECALL                  0
                      248 CALL                     0
                      258 POP_TOP
          
-         869         260 LOAD_CONST               0 (None)
+         897         260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 LOAD_CONST               0 (None)
                      266 PRECALL                  2
                      270 CALL                     2
                      280 POP_TOP
                      282 LOAD_CONST               0 (None)
                      284 RETURN_VALUE
@@ -4452,15 +4452,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('comment_id', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'delete_comment'
-         firstlineno 868
+         firstlineno 896
          lnotab 0x02013401040454014e0128f9
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4473,71 +4473,71 @@
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00200000000000000000000000000000000000000
             007407000000000000000000006a0400000000000000006404a6010000ab
             010000000000000000a6010000ab01000000000000000001007c01a00500
             00000000000000000000000000000000000000a6000000ab000000000000
             0000000100640064006400a6020000ab0200000000000000000100640053
             002300310073047702780359007701010059000100010064005300
-         879           0 RESUME                   0
+         907           0 RESUME                   0
          
-         883           2 LOAD_GLOBAL              0 (db)
+         911           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         884          54 LOAD_FAST                1 (conn)
+         912          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         885          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         913          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         886         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
+         914         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
          
-         885         102 PRECALL                  1
+         913         102 PRECALL                  1
                      106 CALL                     1
          
-         892         116 LOAD_CONST               2 ('search_uid')
+         920         116 LOAD_CONST               2 ('search_uid')
                      118 LOAD_FAST                0 (search_uid)
                      120 BUILD_MAP                1
          
-         884         122 PRECALL                  2
+         912         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         894         138 LOAD_FAST                1 (conn)
+         922         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         895         216 LOAD_FAST                1 (conn)
+         923         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              2 (execute)
                      240 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      252 LOAD_ATTR                4 (text)
                      262 LOAD_CONST               4 ('REFRESH MATERIALIZED VIEW rating')
                      264 PRECALL                  1
                      268 CALL                     1
                      278 PRECALL                  1
                      282 CALL                     1
                      292 POP_TOP
          
-         898         294 LOAD_FAST                1 (conn)
+         926         294 LOAD_FAST                1 (conn)
                      296 LOAD_METHOD              5 (commit)
                      318 PRECALL                  0
                      322 CALL                     0
                      332 POP_TOP
          
-         883         334 LOAD_CONST               0 (None)
+         911         334 LOAD_CONST               0 (None)
                      336 LOAD_CONST               0 (None)
                      338 LOAD_CONST               0 (None)
                      340 PRECALL                  2
                      344 CALL                     2
                      354 POP_TOP
                      356 LOAD_CONST               0 (None)
                      358 RETURN_VALUE
@@ -4566,22 +4566,22 @@
             'REFRESH MATERIALIZED VIEW rating'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('search_uid', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'reset_inbox'
-         firstlineno 879
+         firstlineno 907
          lnotab 0x020434011801160102ff0e0706f8100a4e014e0328f1
       (False, None)
    names      ('hashlib', 'json', 'dataclasses', 'asdict', 'time', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'gandai', 'ts', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_event', 'models', 'insert_company', 'insert_actor', 'insert_search', 'important_targets_from_event', 'int', 'str', 'bool', 'insert_companies_as_targets', 'DataFrame', 'searches_query', 'average_rating_per_search_query', 'validation_history', 'searches_comment_counts', 'enriched_searches_query', 'actor', 'buyer', 'search_targets', 'search_comments', 'event', 'event_history', 'search_criteria_history', 'find_search', 'find_search_by_token', 'find_company_by_domain', 'find_actor_by_email', 'find_event_by_id', 'update_company', 'update_search', 'mute_event', 'delete_comment', 'reset_inbox')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080108010c010c011002080108010c010c02140208010c010c
       011c021406101e240e100f1010244c020102fb04010eff020202fe020302
-      fd020402fc020502fb020602fa08601620060c162b0614061b160e163e0c
+      fd020402fc020502fb020602fa08601620060c162b06140614160e16610c
       7f00071a161a0c1a1e1a1d241c2409101010101013101d10171017100b
```

### Comparing `gandai-1.7.54/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.55/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/analytics.py` & `gandai-1.7.55/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/constants.py` & `gandai-1.7.55/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/db.py` & `gandai-1.7.55/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/google.py` & `gandai-1.7.55/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/gpt.py` & `gandai-1.7.55/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/grata.py` & `gandai-1.7.55/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/helpers.py` & `gandai-1.7.55/gandai/helpers.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/main.py` & `gandai-1.7.55/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.55/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/migrations/db_seed.py` & `gandai-1.7.55/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/migrations/dealcloud.py` & `gandai-1.7.55/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.55/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/migrations/sql/schema.sql` & `gandai-1.7.55/gandai/migrations/sql/schema.sql`

 * *Files 10% similar despite different names*

```diff
@@ -96,22 +96,7 @@
 WHERE 
     e.type = 'comment'
 GROUP BY e.search_uid, e.domain;
 
 CREATE INDEX idx_comment_search_uid_domain ON comment(search_uid, domain);
 
 
-CREATE MATERIALIZED VIEW IF NOT EXISTS criteria AS
-WITH RankedCriteria AS (
-    SELECT *,
-           ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rank
-    FROM event
-    WHERE 
-        type = 'criteria'       
-)
-SELECT 
-	search_uid, actor_key, data, created
-FROM RankedCriteria r
-WHERE 
-    rank = 1
-;
-
```

### Comparing `gandai-1.7.54/gandai/models.py` & `gandai-1.7.55/gandai/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     REJECT = auto()
     CLIENT_REJECT = auto()
     CRITERIA = auto()
 
 
 @dataclass
 class Event:
-      # fk # add index
+    # fk # add index
     actor_key: str  # fk
     type: str  # enum
     search_uid: Optional[int] = None
     domain: Optional[str] = None  # fk
     data: dict = field(default_factory=dict)
     id: int = field(default=None)  # pk
     # created: int = field(init=False)
@@ -136,15 +136,15 @@
 
 
 @dataclass
 class Search:
     uid: int  # foreign key, dealcloud id
     label: str  # maps to dealcloud engagement name
     meta: dict = field(default_factory=dict)
-    criteria: Criteria = field(default_factory=Criteria)
+    # criteria: Criteria = field(default_factory=Criteria)
     # maps: Maps = field(default_factory=Maps)
 
     # uh what are these for?
     @property
     def notes(self) -> str:
         return self.meta.get("notes", None)
```

### Comparing `gandai-1.7.54/gandai/query.py` & `gandai-1.7.55/gandai/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,36 +370,29 @@
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
 
     return df
 
 
 def enriched_searches_query():
     searches = searches_query()
-    # recent_event_count = recent_validations()
+
     recent_event_count = validation_history()
 
     df = searches.merge(
         recent_event_count, left_on="uid", right_on="search_uid", how="left"
     )
 
     df["last_1_days"] = df["last_1_days"].fillna(0)
     df["last_7_days"] = df["last_7_days"].fillna(0)
     df["last_30_days"] = df["last_30_days"].fillna(0)
     df["last_90_days"] = df["last_90_days"].fillna(0)
 
     df = df.merge(searches_comment_counts(), on="uid", how="left")
     df["comment_count"] = df["comment_count"].fillna(0)
 
-    # df = df.merge(
-    #     average_rating_per_search_query(),
-    #     left_on="uid",
-    #     right_on="search_uid",
-    #     how="left",
-    # )
-    # df["activity"] = df["activity"].fillna(0)
     return df
 
 
 def actor() -> pd.DataFrame:
     with db.connect() as conn:
         result = conn.execute(
             sqlalchemy.text(
@@ -471,14 +464,49 @@
         else:
             return None
 
     df["employees"] = df["meta"].apply(get_employees)
     return df
 
 
+# def other_searches(search_uid: int) -> pd.DataFrame:
+#     query = """
+#     SELECT
+#         t.domain,
+#         jsonb_agg(
+#             jsonb_build_object(
+#                 'search_uid', t.search_uid,
+#                 'domain', t.domain,
+#                 'stage', t.stage,
+#                 'created', t.created,
+#                 'label', t.label
+#             )
+#         ) AS searches
+#     FROM
+#         target t
+#     LEFT JOIN
+#         target tt ON tt.domain = t.domain
+#     WHERE
+#         tt.search_uid = :search_uid
+#         AND t.search_uid != :search_uid
+#         AND t.stage != 'reject'
+#     GROUP BY
+#         t.domain
+#         ;
+#     """
+
+#     with db.connect() as conn:
+#         result = conn.execute(
+#             sqlalchemy.text(query),
+#             {"search_uid": search_uid},
+#         )
+#         df = pd.DataFrame(result.fetchall(), columns=result.keys())
+#     return df
+
+
 def search_targets(search_uid: int):
     # arguably the most important query
 
     statement = """
     WITH RankedEvents AS (
         SELECT *,
             ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn
@@ -601,15 +629,15 @@
             return None
 
     df["end_customer"] = df["end_customer"].apply(list_to_csv)
     df["employees"] = df["meta"].apply(get_employees)
     df["ownership"] = df["ownership"].apply(get_ownership)
     df["state"] = df.apply(get_state, axis=1)
     df["city"] = df.apply(get_city, axis=1)
-    # df['year_founded'] = df['year_founded'].dropna().apply(lambda x: int(x))
+
     return df
 
 
 def search_comments(search_uid: int) -> pd.DataFrame:
     statement = """
     SELECT 
         e.*,
@@ -704,20 +732,20 @@
 
 def find_search(uid: int) -> ts.models.Search:
     with db.connect() as conn:
         statement = """
             SELECT 
                 uid, 
                 label, 
-                meta, 
-                meta->>'next_due_date' as next_due_date,
-                meta->>'notes' as notes,
-                COALESCE(criteria.data, '{}'::jsonb) as criteria
+                meta 
+                -- meta->>'next_due_date' as next_due_date,
+                -- meta->>'notes' as notes,
+                -- COALESCE(criteria.data, '{}'::jsonb) as criteria
             FROM search
-            LEFT JOIN criteria ON search.uid = criteria.search_uid
+            -- LEFT JOIN criteria ON search.uid = criteria.search_uid
             
             WHERE uid = :uid
             """
         result = conn.execute(sqlalchemy.text(statement), {"uid": uid})
 
         row = result.fetchone()
         if row is None:
```

### Comparing `gandai-1.7.54/gandai/secrets.py` & `gandai-1.7.55/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.54/gandai/tasks.py` & `gandai-1.7.55/gandai/tasks.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import gandai as ts
 from gandai import main
 from google.cloud import tasks_v2
 
 
 def trigger_process_event(event_id: int) -> None:
-    if False:
+    if os.getenv("TASKS") == "local":
         main.process_event(event_id=event_id)
         # Thread(target=main.process_event, kwargs={"event_id": event_id}).start()
     else:
         client = tasks_v2.CloudTasksClient()
         parent = client.queue_path(
             project=os.getenv("GOOGLE_CLOUD_PROJECT", "targetselect-staging"),
             location="us-central1",
```

### Comparing `gandai-1.7.54/gandai.egg-info/SOURCES.txt` & `gandai-1.7.55/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

