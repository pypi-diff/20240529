# Comparing `tmp/gandai-1.7.57.tar.gz` & `tmp/gandai-1.7.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.57.tar", last modified: Wed May 29 03:55:58 2024, max compression
+gzip compressed data, was "gandai-1.7.58.tar", last modified: Wed May 29 13:11:02 2024, max compression
```

## Comparing `gandai-1.7.57.tar` & `gandai-1.7.58.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.158005 gandai-1.7.57/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.57/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 03:55:58.157795 gandai-1.7.57/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.148541 gandai-1.7.57/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.57/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.154660 gandai-1.7.57/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.57/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.57/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.57/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.57/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2623 2024-05-29 02:35:57.000000 gandai-1.7.57/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.57/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.57/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.57/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17446 2024-05-29 00:40:29.000000 gandai-1.7.57/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1673 2024-05-29 02:22:28.000000 gandai-1.7.57/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-29 00:06:01.000000 gandai-1.7.57/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17768 2024-05-29 03:54:02.000000 gandai-1.7.57/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10401 2024-05-29 00:06:00.000000 gandai-1.7.57/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    45062 2024-05-29 03:54:47.000000 gandai-1.7.57/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.57/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.57/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.57/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1697 2024-05-24 15:09:39.000000 gandai-1.7.57/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.57/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1700 2024-05-29 02:35:57.000000 gandai-1.7.57/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.57/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.57/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)    16797 2024-05-29 00:40:27.000000 gandai-1.7.57/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     4127 2024-05-29 02:22:25.000000 gandai-1.7.57/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-29 00:05:27.000000 gandai-1.7.57/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    13122 2024-05-29 03:53:59.000000 gandai-1.7.57/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.155449 gandai-1.7.57/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.57/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.155823 gandai-1.7.57/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.57/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.57/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.57/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.57/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.57/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.157280 gandai-1.7.57/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.57/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.57/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-24 15:09:36.000000 gandai-1.7.57/gandai/migrations/sql/240523-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3021 2024-05-28 15:04:19.000000 gandai-1.7.57/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-29 00:05:27.000000 gandai-1.7.57/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    31209 2024-05-29 03:54:45.000000 gandai-1.7.57/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.57/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1081 2024-05-24 15:09:36.000000 gandai-1.7.57/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 03:55:58.157562 gandai-1.7.57/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 03:55:58.000000 gandai-1.7.57/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-29 03:55:58.000000 gandai-1.7.57/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-29 03:55:58.000000 gandai-1.7.57/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-29 03:55:58.000000 gandai-1.7.57/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-29 03:55:48.000000 gandai-1.7.57/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-29 03:55:58.158040 gandai-1.7.57/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.57/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.262579 gandai-1.7.58/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.58/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 13:11:02.262356 gandai-1.7.58/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.253052 gandai-1.7.58/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.58/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.258992 gandai-1.7.58/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.58/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.58/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.58/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.58/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2623 2024-05-29 02:35:57.000000 gandai-1.7.58/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.58/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.58/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.58/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17445 2024-05-29 12:27:02.000000 gandai-1.7.58/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1673 2024-05-29 02:22:28.000000 gandai-1.7.58/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-29 00:06:01.000000 gandai-1.7.58/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17789 2024-05-29 13:10:26.000000 gandai-1.7.58/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10401 2024-05-29 00:06:00.000000 gandai-1.7.58/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    45331 2024-05-29 13:10:08.000000 gandai-1.7.58/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.58/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.58/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.58/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1697 2024-05-24 15:09:39.000000 gandai-1.7.58/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.58/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1700 2024-05-29 02:35:57.000000 gandai-1.7.58/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.58/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.58/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)    16796 2024-05-29 12:26:59.000000 gandai-1.7.58/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     4127 2024-05-29 02:22:25.000000 gandai-1.7.58/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-29 00:05:27.000000 gandai-1.7.58/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    13149 2024-05-29 13:10:23.000000 gandai-1.7.58/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.259820 gandai-1.7.58/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.58/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.260358 gandai-1.7.58/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.58/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.58/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.58/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.58/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.58/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.261726 gandai-1.7.58/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.58/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.58/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-24 15:09:36.000000 gandai-1.7.58/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3021 2024-05-28 15:04:19.000000 gandai-1.7.58/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-29 00:05:27.000000 gandai-1.7.58/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    30959 2024-05-29 13:10:05.000000 gandai-1.7.58/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.58/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1081 2024-05-24 15:09:36.000000 gandai-1.7.58/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 13:11:02.262076 gandai-1.7.58/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 13:11:02.000000 gandai-1.7.58/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-29 13:11:02.000000 gandai-1.7.58/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-29 13:11:02.000000 gandai-1.7.58/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-29 13:11:02.000000 gandai-1.7.58/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-29 13:10:37.000000 gandai-1.7.58/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-29 13:11:02.262616 gandai-1.7.58/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.58/setup.py
```

### Comparing `gandai-1.7.57/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x7b795666 (Wed May 29 00:40:27 2024 UTC)
-files sz: 16797
+moddate:  0x131f5766 (Wed May 29 12:26:59 2024 UTC)
+files sz: 16796
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a02640064026c016d035a0301
@@ -77,15 +77,15 @@
    
    158         128 LOAD_CONST              14 ('\nTo move a target to a different stage you will create an event with the targets domain \nand the stage you want to move it to.\n\ndomain should include domain only, no subdomain or protocol\n\n// example Event\n{\n    "search_uid": 19696114,\n    "domain": "acme.com",\n    "actor_key": "5558248581",\n    "type": "send",\n    "data": {"key": "value"},\n}\n\n\nHere are the stages along with their labels:\nThe only valid event types are the labelMap.keys()\nconst labelMap = {\n    "land": "Landing",\n    "create": "Inbox",\n    "advance": "Review",\n    "validate": "Validated",\n    "send": "Client Inbox",\n    "client_approve": "Client Approved",\n    "sync": "Synced",\n    "reject": "Reject",\n    "conflict": "Conflict",\n    "client_conflict": "Client Conflict",\n    "client_reject": "Client Reject"\n}\n')
                130 STORE_NAME              14 (HOW_TO_TRANSITION)
    
    191         132 LOAD_CONST              15 ('\n\nTo search Google, you will create an Event object.\n\n@dataclass\nclass Google(Event):\n    search_uid: int  # fk # add index\n    actor_key: str  # fk\n    type: str  \n    data: dict = field(default_factory=dict)\n    id: int = field(default=None)  # pk\n    # created: int = field(init=False)\n\nList[Event] examples asdict:\n\n[{\n  \'search_uid\': 200,\n  \'domain\': null,\n  \'actor_key\': \'3125740050\',\n  \'type\': \'google\',\n  \'data\': {\'q\': \'"golf cart" AND audio\'},\n  \'created\': 1697813193},\n{\n  \'search_uid\': 5255570,\n  \'domain\': null,\n  \'actor_key\': \'3102835279\',\n  \'type\': \'google\',\n  \'data\': {\'q\': \'"commercial" AND "door" AND ("repair" OR "maintenance" OR "replacement") AND "new York City"\'},\n  \'created\': 1697814555}]\n\nThe type is \'google\'\nYou will not set the id or created fields.\nThe default count is 10\n\n')
                134 STORE_NAME              15 (HOW_TO_GOOGLE)
    
-   228         136 LOAD_CONST              16 ('\n\nSearch\nPOST\nhttps://search.grata.com\n/api/v1.3/search/\nReturns Grata-powered search results based on an input search query. If you\'re using any the filters in the UI that are not presented below, the results may differ.\n\nRequest\nHeaders\nAuthorization\nstring\nrequired\nToken\n\nContent-Type\nstring\napplication/json\n\nBody\n\napplication/json\n\napplication/json\nSearch input criteria for company search.\n\nCriteria inputs for company search query.\n\ninclude\narray[string]\nString used for keyword search. This is an array of keywords\n\nExample:\n["CRM, proptech"]\nexclude\narray[string]\nKeywords to exclude from the search.\n\nop\nstring\nThe operation performed on the keywords (any or all). \'Any\' indicates that any of the specified keywords can be included within a company\'s website. \'All\' indicates that all of the specified keywords should be included within a company\'s website.\n\nAllowed values:\nany\nall\nExample:\nany\npage_token\nstring\nString used for pagination. The initial response body for a given search will contain a page_token that can be used for additional results. Insert the page token string into the request body.\n\nlists\narray[string]\nGrata list IDs to search within.\n\nindustry_classifications\nobject\nIndustry classification code for the company. Pass the industry NAICS code or Grata\'s specific software industry code listed in the mapping doc - https://grata.stoplight.io/docs/grata/branches/v1.3/42ptq2xej8i5j-software-industry-code-mapping\n\ninclude\narray[number]\nexclude\narray[number]\nend_customer\narray[string]\nEnd vertical that the company sells to.\n\nAllowed values:\nb2b\nb2c\ninformation_technology\nprofessional_services\nelectronics\ncommercial_and_residential_services\nhospitality_and_leisure\nmedia\nfinance\nindustrials\ntransportation\neducation\nagriculture\nhealthcare\ngovernment\nconsumer_product_and_retail\nownership\narray[string]\nOwnership types to search and sort on.\n\nAllowed values:\nbootstrapped\ninvestor_backed\npublic\npublic_subsidiary\nprivate_subsidiary\nprivate_equity\nprivate_equity_add_on\nbusiness_models\narray[string]\nBusiness models to search on.\n\nAllowed values:\nsoftware\nsoftware_enabled\nservices\nhardware\ncontent_and_publishing\ninvestment_banks_and_business_brokers\neducation\ndirectory\njob_site\nstaffing_and_recruiting\nprivate_equity_and_venture_capital\nprivate_schools\nretailer\nmanufacturer\ndistributor\nproducer\nmarketplace\nhospitals_and_medical_centers\ncolleges_and_universities\ngovernment\nus_federal_agencies\nnonprofit_and_associations\nreligious_institutions\nis_funded\nboolean\nIndicates whether or not the company has received outside funding.\n\nfunding_size\narray[number]\nRange of funding the company has received in USD. Ranges can only start and begin with the following values: 0, 5000000, 10000000, 20000000, 50000000, 100000000, 200000000, 500000000, 500000001. 500000001 equates to maximum.\n\n>= 2 items\n<= 2 items\nfunding_stage\narray[string]\nAllowed values:\nearly_stage_funding\nlate_stage_funding\nprivate_equity_backed\nother_funding\npre_ipo_funding\nemployees_change_time\nstring\nThe interval for employee growth rate.\n\nAllowed values:\nmonth\nquarter\nsix_month\nannual\ngrata_employees_estimates_range\narray[number]\nThe range of employee counts based on Grata Employee estimates. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_on_professional_networks_range\narray[number]\nThe range of employee counts listed on professional networks. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_change\narray[number]\nRange of % employee growth.\n\nyear_founded\narray[number]\nRange of founding years.\n\nheadquarters\nobject\nHeadquarter locations supports all countries and US city/states. State cannot be left blank if city is populated. Country cannot be other than United States if searching for city/state.\n\ninclude\narray[object]\nexclude\narray[object]\nResponses\n200\n400\n401\n404\n405\n429\n500\nOK\n\nBody\n\napplication/json\n\napplication/json\ncompanies\narray[object]\nname\nstring\nName of the company.\n\ncompany_uid\nstring\nUnique alphanumeric Grata ID for the company (case-sensitive).\n\nurl\nstring\nURL to the company\'s Grata profile.\n\ndomain\nstring\nDomain of the company.\n\ndescription\nstring\nDescription of the company.\n\ncompany-basic\nExport\ncompanies\narray[object]\nname\nstring\nName of the company.\n\ncompany_uid\nstring\nUnique alphanumeric Grata ID for the company (case-sensitive).\n\nurl\nstring\nURL to the company\'s Grata profile.\n\ndomain\nstring\nDomain of the company.\n\ndescription\nstring\nDescription of the company.\n\n{\n  "companies": [\n    {\n      "name": "Slack",\n      "company_uid": "7W46XUJT",\n      "url": "https://search.gratadata.com/search?c=MDKZCCG3",\n      "domain": "slack.com",\n      "description": "Slack is a global collaboration hub that makes people’s working lives simpler, more pleasant and more productive. From global Fortune 100 companies to corner markets, businesses and teams of every kind use Slack to bring the right people together with all the right information. Slack is headquartered in San Francisco California and has nine offices around the world. Slack is where work flows. It\'s where the people you need, the information you share, and the tools you use come together to get things done."\n    }\n  ]\n}\n\nsearch-filters\nExport\nCriteria inputs for company search query.\n\nheadquarters\n.\nexclude[]\ninclude\narray[string]\nString used for keyword search. This is an array of keywords\n\nExample:\n["CRM, proptech"]\nexclude\narray[string]\nKeywords to exclude from the search.\n\nop\nstring\nThe operation performed on the keywords (any or all). \'Any\' indicates that any of the specified keywords can be included within a company\'s website. \'All\' indicates that all of the specified keywords should be included within a company\'s website.\n\nAllowed values:\nany\nall\nExample:\nany\npage_token\nstring\nString used for pagination. The initial response body for a given search will contain a page_token that can be used for additional results. Insert the page token string into the request body.\n\nlists\narray[string]\nGrata list IDs to search within.\n\nindustry_classifications\nobject\nIndustry classification code for the company. Pass the industry NAICS code or Grata\'s specific software industry code listed in the mapping doc - https://grata.stoplight.io/docs/grata/branches/v1.3/42ptq2xej8i5j-software-industry-code-mapping\n\ninclude\narray[number]\nexclude\narray[number]\nend_customer\narray[string]\nEnd vertical that the company sells to.\n\nAllowed values:\nb2b\nb2c\ninformation_technology\nprofessional_services\nelectronics\ncommercial_and_residential_services\nhospitality_and_leisure\nmedia\nfinance\nindustrials\ntransportation\neducation\nagriculture\nhealthcare\ngovernment\nconsumer_product_and_retail\nownership\narray[string]\nOwnership types to search and sort on.\n\nAllowed values:\nbootstrapped\ninvestor_backed\npublic\npublic_subsidiary\nprivate_subsidiary\nprivate_equity\nprivate_equity_add_on\nbusiness_models\narray[string]\nBusiness models to search on.\n\nAllowed values:\nsoftware\nsoftware_enabled\nservices\nhardware\ncontent_and_publishing\ninvestment_banks_and_business_brokers\neducation\ndirectory\njob_site\nstaffing_and_recruiting\nprivate_equity_and_venture_capital\nprivate_schools\nretailer\nmanufacturer\ndistributor\nproducer\nmarketplace\nhospitals_and_medical_centers\ncolleges_and_universities\ngovernment\nus_federal_agencies\nnonprofit_and_associations\nreligious_institutions\nis_funded\nboolean\nIndicates whether or not the company has received outside funding.\n\nfunding_size\narray[number]\nRange of funding the company has received in USD. Ranges can only start and begin with the following values: 0, 5000000, 10000000, 20000000, 50000000, 100000000, 200000000, 500000000, 500000001. 500000001 equates to maximum.\n\n>= 2 items\n<= 2 items\nfunding_stage\narray[string]\nAllowed values:\nearly_stage_funding\nlate_stage_funding\nprivate_equity_backed\nother_funding\npre_ipo_funding\nemployees_change_time\nstring\nThe interval for employee growth rate.\n\nAllowed values:\nmonth\nquarter\nsix_month\nannual\ngrata_employees_estimates_range\narray[number]\nThe range of employee counts based on Grata Employee estimates. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_on_professional_networks_range\narray[number]\nThe range of employee counts listed on professional networks. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_change\narray[number]\nRange of % employee growth.\n\nyear_founded\narray[number]\nRange of founding years.\n\nheadquarters\nobject\nHeadquarter locations supports all countries and US city/states. State cannot be left blank if city is populated. Country cannot be other than United States if searching for city/state.\n\ninclude\narray[object]\ncity\nstring or null\nExample:\nLos Angeles\nstate\nstring or null\nExample:\nCalifornia\ncountry\nstring\nExample:\nUnited States\nexclude\narray[object]\ncity\nstring or null\nExample:\nNew York\nstate\nstring or null\nExample:\nNew York\ncountry\nstring\nExample:\nUnited States\n\nimport requests\n\nimport gandai as ts\nfrom gandai import secrets\n\nHEADERS = {\n    "Authorization": secrets.access_secret_version("GRATA_API_TOKEN"),\n    "Content-Type": "application/json",\n}\n\n\n\nmessages = [\n        {\n            "role": "system",\n            "content": HOW_TO_SEARCH_GRATA_API\n        },\n        \n        {\n            "role": "user",\n            "content": "Find me private hvac companies in Alabama",\n        },\n    ]\n\napi_filters: dict = ts.gpt.ask_gpt4(messages)\nprint(api_filters)\n\nresponse = requests.post(\n    "https://search.grata.com/api/v1.3/search/",\n    headers=HEADERS,\n    json={\n        "include": api_filters["include"],\n        "exclude": api_filters["exclude"],\n        "grata_employees_estimates_range": api_filters["grata_employees_estimates_range"],  \n        "headquarters": {\n            "include": api_filters["headquarters"]["include"],\n            "exclude": api_filters["headquarters"]["exclude"],\n        }\n    },\n)\n\n\nresponse\n\n\nYou will respond with the API filters for searching Grata API as a JSON object.\n\n\n')
+   228         136 LOAD_CONST              16 ('\n\nSearch\nPOST\nhttps://search.grata.com\n/api/v1.3/search/\nReturns Grata-powered search results based on an input search query. If you\'re using any the filters in the UI that are not presented below, the results may differ.\n\nRequest\nHeaders\nAuthorization\nstring\nrequired\nToken\n\nContent-Type\nstring\napplication/json\n\nBody\n\napplication/json\n\napplication/json\nSearch input criteria for company search.\n\nCriteria inputs for company search query.\n\ninclude\narray[string]\nString used for keyword search. This is an array of keywords\n\nExample:\n["CRM, proptech"]\nexclude\narray[string]\nKeywords to exclude from the search.\n\nop\nstring\nThe operation performed on the keywords (any or all). \'Any\' indicates that any of the specified keywords can be included within a company\'s website. \'All\' indicates that all of the specified keywords should be included within a company\'s website.\n\nAllowed values:\nany\nall\nExample:\nany\npage_token\nstring\nString used for pagination. The initial response body for a given search will contain a page_token that can be used for additional results. Insert the page token string into the request body.\n\nlists\narray[string]\nGrata list IDs to search within.\n\nindustry_classifications\nobject\nIndustry classification code for the company. Pass the industry NAICS code or Grata\'s specific software industry code listed in the mapping doc - https://grata.stoplight.io/docs/grata/branches/v1.3/42ptq2xej8i5j-software-industry-code-mapping\n\ninclude\narray[number]\nexclude\narray[number]\nend_customer\narray[string]\nEnd vertical that the company sells to.\n\nAllowed values:\nb2b\nb2c\ninformation_technology\nprofessional_services\nelectronics\ncommercial_and_residential_services\nhospitality_and_leisure\nmedia\nfinance\nindustrials\ntransportation\neducation\nagriculture\nhealthcare\ngovernment\nconsumer_product_and_retail\nownership\narray[string]\nOwnership types to search and sort on.\n\nAllowed values:\nbootstrapped\ninvestor_backed\npublic\npublic_subsidiary\nprivate_subsidiary\nprivate_equity\nprivate_equity_add_on\nbusiness_models\narray[string]\nBusiness models to search on.\n\nAllowed values:\nsoftware\nsoftware_enabled\nservices\nhardware\ncontent_and_publishing\ninvestment_banks_and_business_brokers\neducation\ndirectory\njob_site\nstaffing_and_recruiting\nprivate_equity_and_venture_capital\nprivate_schools\nretailer\nmanufacturer\ndistributor\nproducer\nmarketplace\nhospitals_and_medical_centers\ncolleges_and_universities\ngovernment\nus_federal_agencies\nnonprofit_and_associations\nreligious_institutions\nis_funded\nboolean\nIndicates whether or not the company has received outside funding.\n\nfunding_size\narray[number]\nRange of funding the company has received in USD. Ranges can only start and begin with the following values: 0, 5000000, 10000000, 20000000, 50000000, 100000000, 200000000, 500000000, 500000001. 500000001 equates to maximum.\n\n>= 2 items\n<= 2 items\nfunding_stage\narray[string]\nAllowed values:\nearly_stage_funding\nlate_stage_funding\nprivate_equity_backed\nother_funding\npre_ipo_funding\nemployees_change_time\nstring\nThe interval for employee growth rate.\n\nAllowed values:\nmonth\nquarter\nsix_month\nannual\ngrata_employees_estimates_range\narray[number]\nThe range of employee counts based on Grata Employee estimates. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_on_professional_networks_range\narray[number]\nThe range of employee counts listed on professional networks. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_change\narray[number]\nRange of % employee growth.\n\nyear_founded\narray[number]\nRange of founding years.\n\nheadquarters\nobject\nHeadquarter locations supports all countries and US city/states. State cannot be left blank if city is populated. Country cannot be other than United States if searching for city/state.\n\ninclude\narray[object]\nexclude\narray[object]\nResponses\n200\n400\n401\n404\n405\n429\n500\nOK\n\nBody\n\napplication/json\n\napplication/json\ncompanies\narray[object]\nname\nstring\nName of the company.\n\ncompany_uid\nstring\nUnique alphanumeric Grata ID for the company (case-sensitive).\n\nurl\nstring\nURL to the company\'s Grata profile.\n\ndomain\nstring\nDomain of the company.\n\ndescription\nstring\nDescription of the company.\n\ncompany-basic\nExport\ncompanies\narray[object]\nname\nstring\nName of the company.\n\ncompany_uid\nstring\nUnique alphanumeric Grata ID for the company (case-sensitive).\n\nurl\nstring\nURL to the company\'s Grata profile.\n\ndomain\nstring\nDomain of the company.\n\ndescription\nstring\nDescription of the company.\n\n{\n  "companies": [\n    {\n      "name": "Slack",\n      "company_uid": "7W46XUJT",\n      "url": "https://search.gratadata.com/search?c=MDKZCCG3",\n      "domain": "slack.com",\n      "description": "Slack is a global collaboration hub that makes people’s working lives simpler, more pleasant and more productive. From global Fortune 100 companies to corner markets, businesses and teams of every kind use Slack to bring the right people together with all the right information. Slack is headquartered in San Francisco California and has nine offices around the world. Slack is where work flows. It\'s where the people you need, the information you share, and the tools you use come together to get things done."\n    }\n  ]\n}\n\nsearch-filters\nExport\nCriteria inputs for company search query.\n\nheadquarters\n.\nexclude[]\ninclude\narray[string]\nString used for keyword search. This is an array of keywords\n\nExample:\n["CRM, proptech"]\nexclude\narray[string]\nKeywords to exclude from the search.\n\nop\nstring\nThe operation performed on the keywords (any or all). \'Any\' indicates that any of the specified keywords can be included within a company\'s website. \'All\' indicates that all of the specified keywords should be included within a company\'s website.\n\nAllowed values:\nany\nall\nExample:\nany\npage_token\nstring\nString used for pagination. The initial response body for a given search will contain a page_token that can be used for additional results. Insert the page token string into the request body.\n\nlists\narray[string]\nGrata list IDs to search within.\n\nindustry_classifications\nobject\nIndustry classification code for the company. Pass the industry NAICS code or Grata\'s specific software industry code listed in the mapping doc - https://grata.stoplight.io/docs/grata/branches/v1.3/42ptq2xej8i5j-software-industry-code-mapping\n\ninclude\narray[number]\nexclude\narray[number]\nend_customer\narray[string]\nEnd vertical that the company sells to.\n\nAllowed values:\nb2b\nb2c\ninformation_technology\nprofessional_services\nelectronics\ncommercial_and_residential_services\nhospitality_and_leisure\nmedia\nfinance\nindustrials\ntransportation\neducation\nagriculture\nhealthcare\ngovernment\nconsumer_product_and_retail\nownership\narray[string]\nOwnership types to search and sort on.\n\nAllowed values:\nbootstrapped\ninvestor_backed\npublic\npublic_subsidiary\nprivate_subsidiary\nprivate_equity\nprivate_equity_add_on\nbusiness_models\narray[string]\nBusiness models to search on.\n\nAllowed values:\nsoftware\nsoftware_enabled\nservices\nhardware\ncontent_and_publishing\ninvestment_banks_and_business_brokers\neducation\ndirectory\njob_site\nstaffing_and_recruiting\nprivate_equity_and_venture_capital\nprivate_schools\nretailer\nmanufacturer\ndistributor\nproducer\nmarketplace\nhospitals_and_medical_centers\ncolleges_and_universities\ngovernment\nus_federal_agencies\nnonprofit_and_associations\nreligious_institutions\nis_funded\nboolean\nIndicates whether or not the company has received outside funding.\n\nfunding_size\narray[number]\nRange of funding the company has received in USD. Ranges can only start and begin with the following values: 0, 5000000, 10000000, 20000000, 50000000, 100000000, 200000000, 500000000, 500000001. 500000001 equates to maximum.\n\n>= 2 items\n<= 2 items\nfunding_stage\narray[string]\nAllowed values:\nearly_stage_funding\nlate_stage_funding\nprivate_equity_backed\nother_funding\npre_ipo_funding\nemployees_change_time\nstring\nThe interval for employee growth rate.\n\nAllowed values:\nmonth\nquarter\nsix_month\nannual\ngrata_employees_estimates_range\narray[number]\nThe range of employee counts based on Grata Employee estimates. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_on_professional_networks_range\narray[number]\nThe range of employee counts listed on professional networks. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_change\narray[number]\nRange of % employee growth.\n\nyear_founded\narray[number]\nRange of founding years.\n\nheadquarters\nobject\nHeadquarter locations supports all countries and US city/states. State cannot be left blank if city is populated. Country cannot be other than United States if searching for city/state.\n\ninclude\narray[object]\ncity\nstring or null\nExample:\nLos Angeles\nstate\nstring or null\nExample:\nCalifornia\ncountry\nstring\nExample:\nUnited States\nexclude\narray[object]\ncity\nstring or null\nExample:\nNew York\nstate\nstring or null\nExample:\nNew York\ncountry\nstring\nExample:\nUnited States\n\nimport requests\n\nimport gandai as ts\nfrom gandai import secrets\n\nHEADERS = {\n    "Authorization": secrets.access_secret_version("GRATA_API_TOKEN"),\n    "Content-Type": "application/json",\n}\n\n\nmessages = [\n        {\n            "role": "system",\n            "content": HOW_TO_SEARCH_GRATA_API\n        },\n        \n        {\n            "role": "user",\n            "content": "Find me private hvac companies in Alabama",\n        },\n    ]\n\napi_filters: dict = ts.gpt.ask_gpt4(messages)\nprint(api_filters)\n\nresponse = requests.post(\n    "https://search.grata.com/api/v1.3/search/",\n    headers=HEADERS,\n    json={\n        "include": api_filters["include"],\n        "exclude": api_filters["exclude"],\n        "grata_employees_estimates_range": api_filters["grata_employees_estimates_range"],  \n        "headquarters": {\n            "include": api_filters["headquarters"]["include"],\n            "exclude": api_filters["headquarters"]["exclude"],\n        }\n    },\n)\n\n\nresponse\n\n\nYou will respond with the API filters for searching Grata API as a JSON object.\n\n\n')
                138 STORE_NAME              16 (HOW_TO_SEARCH_GRATA_API)
                140 LOAD_CONST               1 (None)
                142 RETURN_VALUE
    consts
       0
       None
       ('secrets',)
@@ -165,15 +165,15 @@
          lnotab 0x0201360102010202020106fb12082801
       '\nTo update an attribute for a company you will create an event with the company\'s domain\nof type "update". This will update that company\'s meta field \n\nhere is an example update event\n\n{\n    "domain": "lol.com",\n    "actor_key": "chatgpt",\n    "type": "update",\n    "data": {\n        "contact_name": "Bob"\n    }\n}\n\nHere are all the fields you can use for event[\'data\']\n\nc.data->>\'gpt_description\' as gpt_description, -- a description of the company for use by private equity research analyst to understand the company.\n\nYou will fill out the description field with a description of the company. \nThe description will be a comprehensive description of the company for use \nby private equity research analyst to understand the company.\n\nc.data->>\'employees\' as employees, -- the INTEGER number of employees at the company. prefer the grata estimate. this is an integer.\nc.data->>\'ownership\' as ownership, -- one of ["bootstrapped","investor_backed","public","public_subsidiary","private_subsidiary","private_equity","private_equity_add_on"] \nc.data->>\'headquarters\' as headquarters,\nc.data->>\'city\' as city,\nc.data->>\'state\' as state,\nc.data->>\'designation\' as designation,\nc.data->>\'products\' as products, -- products are physical goods sold by the company. do not list services here. A brand is not a product, do not list brands here.\nc.data->>\'services\' as services, -- services are intangible goods offered by the company. do not list products here.\nc.data->>\'end_customer\' as end_customer, -- what types of customers does the company serve. If commercial, what industry(s). do not list specific customers here.\nc.data->>\'geographies\' as geographies, -- geographies are the areas where the company does business. \nc.data->>\'year_founded\' as year_founded,\nc.data->>\'linkedin\' as linkedin, -- linkedinUrl \nc.data->>\'linkedin_range\' as linkedin_range,\nc.data->>\'industry\' as industry,\nc.data->>\'revenue_estimates\' as revenue_estimates,\nc.data->>\'location_count\' as location_count,\nc.data->>\'business_models\' as business_models,\nc.data->>\'facility_size\' as facility_size,\nc.data->>\'contact_name\' as contact_name,\nc.data->>\'contact_title\' as contact_title,\nc.data->>\'contact_email\' as contact_email,\nc.data->>\'contact_phone\' as contact_phone,\nc.data->>\'contact_address\' as contact_address,\n\nFor fields that are lists, you will use a csv string \nFor these lists, such as products or services, try to stick to top 5 or less areas of focus.\n\n\nIf you are unsure, just leave that key out of the response data\n\n'
       '\nYou will respond with an JSON object that looks like this:\n{\n    "events": List[Event],\n}\n'
       '\nTo search the Google Maps Places API\nYou will respond with this\n{"events": List[asdict(Event)]}\n\nUnless otherwise directed you will return 10 centroids\n\nThere are 20 results per centroid\nSo if the user asks for 100 results you will return the count divided by 20\n\nGive me the query strings you would use to search for \nEach query string should be small enough for a Google Maps search\n\nFor example to search throughout Dallas you might use:\ndentists in Dallas, TX\ndentists in Highland Park, TX\ndentists in Grapevine, TX\ndentists in Plano, TX\n\nNow give me the queries that you would use\n\nHere\'s some Event examples:\n[{\n    "type": "maps",\n    "search_uid": 1700,\n    "actor_key": "7138248581",\n    "data": {\n        "query": "dentists in Dallas, TX"\n    }\n}]\n\n'
       '\n// example Import(Event)\n{\n    "search_uid": 19696114,\n    "domain": null,\n    "actor_key": "4805705555",\n    "type": "import",\n    "data": {\n        "stage": "advance",\n        "domains": [\n            "buybits.com",\n            "lidoradio.com",\n            "rocklandcustomproducts.com",\n            "sigmasafety.ca",\n        ],\n    },\n}\n\nHere are the stages along with their labels:\nThe only valid stages are labelMap.keys()\nconst labelMap = {\n    "land": "Landing",\n    "create": "Inbox",\n    "advance": "Review",\n    "validate": "Validated",\n    "send": "Client Inbox",\n    "client_approve": "Client Approved",\n    "sync": "Synced",\n    "reject": "Reject",\n    "conflict": "Conflict",\n    "client_conflict": "Client Conflict",\n    "client_reject": "Client Reject"\n}\n'
       '\nTo move a target to a different stage you will create an event with the targets domain \nand the stage you want to move it to.\n\ndomain should include domain only, no subdomain or protocol\n\n// example Event\n{\n    "search_uid": 19696114,\n    "domain": "acme.com",\n    "actor_key": "5558248581",\n    "type": "send",\n    "data": {"key": "value"},\n}\n\n\nHere are the stages along with their labels:\nThe only valid event types are the labelMap.keys()\nconst labelMap = {\n    "land": "Landing",\n    "create": "Inbox",\n    "advance": "Review",\n    "validate": "Validated",\n    "send": "Client Inbox",\n    "client_approve": "Client Approved",\n    "sync": "Synced",\n    "reject": "Reject",\n    "conflict": "Conflict",\n    "client_conflict": "Client Conflict",\n    "client_reject": "Client Reject"\n}\n'
       '\n\nTo search Google, you will create an Event object.\n\n@dataclass\nclass Google(Event):\n    search_uid: int  # fk # add index\n    actor_key: str  # fk\n    type: str  \n    data: dict = field(default_factory=dict)\n    id: int = field(default=None)  # pk\n    # created: int = field(init=False)\n\nList[Event] examples asdict:\n\n[{\n  \'search_uid\': 200,\n  \'domain\': null,\n  \'actor_key\': \'3125740050\',\n  \'type\': \'google\',\n  \'data\': {\'q\': \'"golf cart" AND audio\'},\n  \'created\': 1697813193},\n{\n  \'search_uid\': 5255570,\n  \'domain\': null,\n  \'actor_key\': \'3102835279\',\n  \'type\': \'google\',\n  \'data\': {\'q\': \'"commercial" AND "door" AND ("repair" OR "maintenance" OR "replacement") AND "new York City"\'},\n  \'created\': 1697814555}]\n\nThe type is \'google\'\nYou will not set the id or created fields.\nThe default count is 10\n\n'
-      '\n\nSearch\nPOST\nhttps://search.grata.com\n/api/v1.3/search/\nReturns Grata-powered search results based on an input search query. If you\'re using any the filters in the UI that are not presented below, the results may differ.\n\nRequest\nHeaders\nAuthorization\nstring\nrequired\nToken\n\nContent-Type\nstring\napplication/json\n\nBody\n\napplication/json\n\napplication/json\nSearch input criteria for company search.\n\nCriteria inputs for company search query.\n\ninclude\narray[string]\nString used for keyword search. This is an array of keywords\n\nExample:\n["CRM, proptech"]\nexclude\narray[string]\nKeywords to exclude from the search.\n\nop\nstring\nThe operation performed on the keywords (any or all). \'Any\' indicates that any of the specified keywords can be included within a company\'s website. \'All\' indicates that all of the specified keywords should be included within a company\'s website.\n\nAllowed values:\nany\nall\nExample:\nany\npage_token\nstring\nString used for pagination. The initial response body for a given search will contain a page_token that can be used for additional results. Insert the page token string into the request body.\n\nlists\narray[string]\nGrata list IDs to search within.\n\nindustry_classifications\nobject\nIndustry classification code for the company. Pass the industry NAICS code or Grata\'s specific software industry code listed in the mapping doc - https://grata.stoplight.io/docs/grata/branches/v1.3/42ptq2xej8i5j-software-industry-code-mapping\n\ninclude\narray[number]\nexclude\narray[number]\nend_customer\narray[string]\nEnd vertical that the company sells to.\n\nAllowed values:\nb2b\nb2c\ninformation_technology\nprofessional_services\nelectronics\ncommercial_and_residential_services\nhospitality_and_leisure\nmedia\nfinance\nindustrials\ntransportation\neducation\nagriculture\nhealthcare\ngovernment\nconsumer_product_and_retail\nownership\narray[string]\nOwnership types to search and sort on.\n\nAllowed values:\nbootstrapped\ninvestor_backed\npublic\npublic_subsidiary\nprivate_subsidiary\nprivate_equity\nprivate_equity_add_on\nbusiness_models\narray[string]\nBusiness models to search on.\n\nAllowed values:\nsoftware\nsoftware_enabled\nservices\nhardware\ncontent_and_publishing\ninvestment_banks_and_business_brokers\neducation\ndirectory\njob_site\nstaffing_and_recruiting\nprivate_equity_and_venture_capital\nprivate_schools\nretailer\nmanufacturer\ndistributor\nproducer\nmarketplace\nhospitals_and_medical_centers\ncolleges_and_universities\ngovernment\nus_federal_agencies\nnonprofit_and_associations\nreligious_institutions\nis_funded\nboolean\nIndicates whether or not the company has received outside funding.\n\nfunding_size\narray[number]\nRange of funding the company has received in USD. Ranges can only start and begin with the following values: 0, 5000000, 10000000, 20000000, 50000000, 100000000, 200000000, 500000000, 500000001. 500000001 equates to maximum.\n\n>= 2 items\n<= 2 items\nfunding_stage\narray[string]\nAllowed values:\nearly_stage_funding\nlate_stage_funding\nprivate_equity_backed\nother_funding\npre_ipo_funding\nemployees_change_time\nstring\nThe interval for employee growth rate.\n\nAllowed values:\nmonth\nquarter\nsix_month\nannual\ngrata_employees_estimates_range\narray[number]\nThe range of employee counts based on Grata Employee estimates. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_on_professional_networks_range\narray[number]\nThe range of employee counts listed on professional networks. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_change\narray[number]\nRange of % employee growth.\n\nyear_founded\narray[number]\nRange of founding years.\n\nheadquarters\nobject\nHeadquarter locations supports all countries and US city/states. State cannot be left blank if city is populated. Country cannot be other than United States if searching for city/state.\n\ninclude\narray[object]\nexclude\narray[object]\nResponses\n200\n400\n401\n404\n405\n429\n500\nOK\n\nBody\n\napplication/json\n\napplication/json\ncompanies\narray[object]\nname\nstring\nName of the company.\n\ncompany_uid\nstring\nUnique alphanumeric Grata ID for the company (case-sensitive).\n\nurl\nstring\nURL to the company\'s Grata profile.\n\ndomain\nstring\nDomain of the company.\n\ndescription\nstring\nDescription of the company.\n\ncompany-basic\nExport\ncompanies\narray[object]\nname\nstring\nName of the company.\n\ncompany_uid\nstring\nUnique alphanumeric Grata ID for the company (case-sensitive).\n\nurl\nstring\nURL to the company\'s Grata profile.\n\ndomain\nstring\nDomain of the company.\n\ndescription\nstring\nDescription of the company.\n\n{\n  "companies": [\n    {\n      "name": "Slack",\n      "company_uid": "7W46XUJT",\n      "url": "https://search.gratadata.com/search?c=MDKZCCG3",\n      "domain": "slack.com",\n      "description": "Slack is a global collaboration hub that makes people’s working lives simpler, more pleasant and more productive. From global Fortune 100 companies to corner markets, businesses and teams of every kind use Slack to bring the right people together with all the right information. Slack is headquartered in San Francisco California and has nine offices around the world. Slack is where work flows. It\'s where the people you need, the information you share, and the tools you use come together to get things done."\n    }\n  ]\n}\n\nsearch-filters\nExport\nCriteria inputs for company search query.\n\nheadquarters\n.\nexclude[]\ninclude\narray[string]\nString used for keyword search. This is an array of keywords\n\nExample:\n["CRM, proptech"]\nexclude\narray[string]\nKeywords to exclude from the search.\n\nop\nstring\nThe operation performed on the keywords (any or all). \'Any\' indicates that any of the specified keywords can be included within a company\'s website. \'All\' indicates that all of the specified keywords should be included within a company\'s website.\n\nAllowed values:\nany\nall\nExample:\nany\npage_token\nstring\nString used for pagination. The initial response body for a given search will contain a page_token that can be used for additional results. Insert the page token string into the request body.\n\nlists\narray[string]\nGrata list IDs to search within.\n\nindustry_classifications\nobject\nIndustry classification code for the company. Pass the industry NAICS code or Grata\'s specific software industry code listed in the mapping doc - https://grata.stoplight.io/docs/grata/branches/v1.3/42ptq2xej8i5j-software-industry-code-mapping\n\ninclude\narray[number]\nexclude\narray[number]\nend_customer\narray[string]\nEnd vertical that the company sells to.\n\nAllowed values:\nb2b\nb2c\ninformation_technology\nprofessional_services\nelectronics\ncommercial_and_residential_services\nhospitality_and_leisure\nmedia\nfinance\nindustrials\ntransportation\neducation\nagriculture\nhealthcare\ngovernment\nconsumer_product_and_retail\nownership\narray[string]\nOwnership types to search and sort on.\n\nAllowed values:\nbootstrapped\ninvestor_backed\npublic\npublic_subsidiary\nprivate_subsidiary\nprivate_equity\nprivate_equity_add_on\nbusiness_models\narray[string]\nBusiness models to search on.\n\nAllowed values:\nsoftware\nsoftware_enabled\nservices\nhardware\ncontent_and_publishing\ninvestment_banks_and_business_brokers\neducation\ndirectory\njob_site\nstaffing_and_recruiting\nprivate_equity_and_venture_capital\nprivate_schools\nretailer\nmanufacturer\ndistributor\nproducer\nmarketplace\nhospitals_and_medical_centers\ncolleges_and_universities\ngovernment\nus_federal_agencies\nnonprofit_and_associations\nreligious_institutions\nis_funded\nboolean\nIndicates whether or not the company has received outside funding.\n\nfunding_size\narray[number]\nRange of funding the company has received in USD. Ranges can only start and begin with the following values: 0, 5000000, 10000000, 20000000, 50000000, 100000000, 200000000, 500000000, 500000001. 500000001 equates to maximum.\n\n>= 2 items\n<= 2 items\nfunding_stage\narray[string]\nAllowed values:\nearly_stage_funding\nlate_stage_funding\nprivate_equity_backed\nother_funding\npre_ipo_funding\nemployees_change_time\nstring\nThe interval for employee growth rate.\n\nAllowed values:\nmonth\nquarter\nsix_month\nannual\ngrata_employees_estimates_range\narray[number]\nThe range of employee counts based on Grata Employee estimates. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_on_professional_networks_range\narray[number]\nThe range of employee counts listed on professional networks. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_change\narray[number]\nRange of % employee growth.\n\nyear_founded\narray[number]\nRange of founding years.\n\nheadquarters\nobject\nHeadquarter locations supports all countries and US city/states. State cannot be left blank if city is populated. Country cannot be other than United States if searching for city/state.\n\ninclude\narray[object]\ncity\nstring or null\nExample:\nLos Angeles\nstate\nstring or null\nExample:\nCalifornia\ncountry\nstring\nExample:\nUnited States\nexclude\narray[object]\ncity\nstring or null\nExample:\nNew York\nstate\nstring or null\nExample:\nNew York\ncountry\nstring\nExample:\nUnited States\n\nimport requests\n\nimport gandai as ts\nfrom gandai import secrets\n\nHEADERS = {\n    "Authorization": secrets.access_secret_version("GRATA_API_TOKEN"),\n    "Content-Type": "application/json",\n}\n\n\n\nmessages = [\n        {\n            "role": "system",\n            "content": HOW_TO_SEARCH_GRATA_API\n        },\n        \n        {\n            "role": "user",\n            "content": "Find me private hvac companies in Alabama",\n        },\n    ]\n\napi_filters: dict = ts.gpt.ask_gpt4(messages)\nprint(api_filters)\n\nresponse = requests.post(\n    "https://search.grata.com/api/v1.3/search/",\n    headers=HEADERS,\n    json={\n        "include": api_filters["include"],\n        "exclude": api_filters["exclude"],\n        "grata_employees_estimates_range": api_filters["grata_employees_estimates_range"],  \n        "headquarters": {\n            "include": api_filters["headquarters"]["include"],\n            "exclude": api_filters["headquarters"]["exclude"],\n        }\n    },\n)\n\n\nresponse\n\n\nYou will respond with the API filters for searching Grata API as a JSON object.\n\n\n'
+      '\n\nSearch\nPOST\nhttps://search.grata.com\n/api/v1.3/search/\nReturns Grata-powered search results based on an input search query. If you\'re using any the filters in the UI that are not presented below, the results may differ.\n\nRequest\nHeaders\nAuthorization\nstring\nrequired\nToken\n\nContent-Type\nstring\napplication/json\n\nBody\n\napplication/json\n\napplication/json\nSearch input criteria for company search.\n\nCriteria inputs for company search query.\n\ninclude\narray[string]\nString used for keyword search. This is an array of keywords\n\nExample:\n["CRM, proptech"]\nexclude\narray[string]\nKeywords to exclude from the search.\n\nop\nstring\nThe operation performed on the keywords (any or all). \'Any\' indicates that any of the specified keywords can be included within a company\'s website. \'All\' indicates that all of the specified keywords should be included within a company\'s website.\n\nAllowed values:\nany\nall\nExample:\nany\npage_token\nstring\nString used for pagination. The initial response body for a given search will contain a page_token that can be used for additional results. Insert the page token string into the request body.\n\nlists\narray[string]\nGrata list IDs to search within.\n\nindustry_classifications\nobject\nIndustry classification code for the company. Pass the industry NAICS code or Grata\'s specific software industry code listed in the mapping doc - https://grata.stoplight.io/docs/grata/branches/v1.3/42ptq2xej8i5j-software-industry-code-mapping\n\ninclude\narray[number]\nexclude\narray[number]\nend_customer\narray[string]\nEnd vertical that the company sells to.\n\nAllowed values:\nb2b\nb2c\ninformation_technology\nprofessional_services\nelectronics\ncommercial_and_residential_services\nhospitality_and_leisure\nmedia\nfinance\nindustrials\ntransportation\neducation\nagriculture\nhealthcare\ngovernment\nconsumer_product_and_retail\nownership\narray[string]\nOwnership types to search and sort on.\n\nAllowed values:\nbootstrapped\ninvestor_backed\npublic\npublic_subsidiary\nprivate_subsidiary\nprivate_equity\nprivate_equity_add_on\nbusiness_models\narray[string]\nBusiness models to search on.\n\nAllowed values:\nsoftware\nsoftware_enabled\nservices\nhardware\ncontent_and_publishing\ninvestment_banks_and_business_brokers\neducation\ndirectory\njob_site\nstaffing_and_recruiting\nprivate_equity_and_venture_capital\nprivate_schools\nretailer\nmanufacturer\ndistributor\nproducer\nmarketplace\nhospitals_and_medical_centers\ncolleges_and_universities\ngovernment\nus_federal_agencies\nnonprofit_and_associations\nreligious_institutions\nis_funded\nboolean\nIndicates whether or not the company has received outside funding.\n\nfunding_size\narray[number]\nRange of funding the company has received in USD. Ranges can only start and begin with the following values: 0, 5000000, 10000000, 20000000, 50000000, 100000000, 200000000, 500000000, 500000001. 500000001 equates to maximum.\n\n>= 2 items\n<= 2 items\nfunding_stage\narray[string]\nAllowed values:\nearly_stage_funding\nlate_stage_funding\nprivate_equity_backed\nother_funding\npre_ipo_funding\nemployees_change_time\nstring\nThe interval for employee growth rate.\n\nAllowed values:\nmonth\nquarter\nsix_month\nannual\ngrata_employees_estimates_range\narray[number]\nThe range of employee counts based on Grata Employee estimates. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_on_professional_networks_range\narray[number]\nThe range of employee counts listed on professional networks. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_change\narray[number]\nRange of % employee growth.\n\nyear_founded\narray[number]\nRange of founding years.\n\nheadquarters\nobject\nHeadquarter locations supports all countries and US city/states. State cannot be left blank if city is populated. Country cannot be other than United States if searching for city/state.\n\ninclude\narray[object]\nexclude\narray[object]\nResponses\n200\n400\n401\n404\n405\n429\n500\nOK\n\nBody\n\napplication/json\n\napplication/json\ncompanies\narray[object]\nname\nstring\nName of the company.\n\ncompany_uid\nstring\nUnique alphanumeric Grata ID for the company (case-sensitive).\n\nurl\nstring\nURL to the company\'s Grata profile.\n\ndomain\nstring\nDomain of the company.\n\ndescription\nstring\nDescription of the company.\n\ncompany-basic\nExport\ncompanies\narray[object]\nname\nstring\nName of the company.\n\ncompany_uid\nstring\nUnique alphanumeric Grata ID for the company (case-sensitive).\n\nurl\nstring\nURL to the company\'s Grata profile.\n\ndomain\nstring\nDomain of the company.\n\ndescription\nstring\nDescription of the company.\n\n{\n  "companies": [\n    {\n      "name": "Slack",\n      "company_uid": "7W46XUJT",\n      "url": "https://search.gratadata.com/search?c=MDKZCCG3",\n      "domain": "slack.com",\n      "description": "Slack is a global collaboration hub that makes people’s working lives simpler, more pleasant and more productive. From global Fortune 100 companies to corner markets, businesses and teams of every kind use Slack to bring the right people together with all the right information. Slack is headquartered in San Francisco California and has nine offices around the world. Slack is where work flows. It\'s where the people you need, the information you share, and the tools you use come together to get things done."\n    }\n  ]\n}\n\nsearch-filters\nExport\nCriteria inputs for company search query.\n\nheadquarters\n.\nexclude[]\ninclude\narray[string]\nString used for keyword search. This is an array of keywords\n\nExample:\n["CRM, proptech"]\nexclude\narray[string]\nKeywords to exclude from the search.\n\nop\nstring\nThe operation performed on the keywords (any or all). \'Any\' indicates that any of the specified keywords can be included within a company\'s website. \'All\' indicates that all of the specified keywords should be included within a company\'s website.\n\nAllowed values:\nany\nall\nExample:\nany\npage_token\nstring\nString used for pagination. The initial response body for a given search will contain a page_token that can be used for additional results. Insert the page token string into the request body.\n\nlists\narray[string]\nGrata list IDs to search within.\n\nindustry_classifications\nobject\nIndustry classification code for the company. Pass the industry NAICS code or Grata\'s specific software industry code listed in the mapping doc - https://grata.stoplight.io/docs/grata/branches/v1.3/42ptq2xej8i5j-software-industry-code-mapping\n\ninclude\narray[number]\nexclude\narray[number]\nend_customer\narray[string]\nEnd vertical that the company sells to.\n\nAllowed values:\nb2b\nb2c\ninformation_technology\nprofessional_services\nelectronics\ncommercial_and_residential_services\nhospitality_and_leisure\nmedia\nfinance\nindustrials\ntransportation\neducation\nagriculture\nhealthcare\ngovernment\nconsumer_product_and_retail\nownership\narray[string]\nOwnership types to search and sort on.\n\nAllowed values:\nbootstrapped\ninvestor_backed\npublic\npublic_subsidiary\nprivate_subsidiary\nprivate_equity\nprivate_equity_add_on\nbusiness_models\narray[string]\nBusiness models to search on.\n\nAllowed values:\nsoftware\nsoftware_enabled\nservices\nhardware\ncontent_and_publishing\ninvestment_banks_and_business_brokers\neducation\ndirectory\njob_site\nstaffing_and_recruiting\nprivate_equity_and_venture_capital\nprivate_schools\nretailer\nmanufacturer\ndistributor\nproducer\nmarketplace\nhospitals_and_medical_centers\ncolleges_and_universities\ngovernment\nus_federal_agencies\nnonprofit_and_associations\nreligious_institutions\nis_funded\nboolean\nIndicates whether or not the company has received outside funding.\n\nfunding_size\narray[number]\nRange of funding the company has received in USD. Ranges can only start and begin with the following values: 0, 5000000, 10000000, 20000000, 50000000, 100000000, 200000000, 500000000, 500000001. 500000001 equates to maximum.\n\n>= 2 items\n<= 2 items\nfunding_stage\narray[string]\nAllowed values:\nearly_stage_funding\nlate_stage_funding\nprivate_equity_backed\nother_funding\npre_ipo_funding\nemployees_change_time\nstring\nThe interval for employee growth rate.\n\nAllowed values:\nmonth\nquarter\nsix_month\nannual\ngrata_employees_estimates_range\narray[number]\nThe range of employee counts based on Grata Employee estimates. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_on_professional_networks_range\narray[number]\nThe range of employee counts listed on professional networks. Inputting 100,001 as the maximum value will search for all employee sizes above the minimum. [100,100001] will search for all companies with 100 or more employees\n\nemployees_change\narray[number]\nRange of % employee growth.\n\nyear_founded\narray[number]\nRange of founding years.\n\nheadquarters\nobject\nHeadquarter locations supports all countries and US city/states. State cannot be left blank if city is populated. Country cannot be other than United States if searching for city/state.\n\ninclude\narray[object]\ncity\nstring or null\nExample:\nLos Angeles\nstate\nstring or null\nExample:\nCalifornia\ncountry\nstring\nExample:\nUnited States\nexclude\narray[object]\ncity\nstring or null\nExample:\nNew York\nstate\nstring or null\nExample:\nNew York\ncountry\nstring\nExample:\nUnited States\n\nimport requests\n\nimport gandai as ts\nfrom gandai import secrets\n\nHEADERS = {\n    "Authorization": secrets.access_secret_version("GRATA_API_TOKEN"),\n    "Content-Type": "application/json",\n}\n\n\nmessages = [\n        {\n            "role": "system",\n            "content": HOW_TO_SEARCH_GRATA_API\n        },\n        \n        {\n            "role": "user",\n            "content": "Find me private hvac companies in Alabama",\n        },\n    ]\n\napi_filters: dict = ts.gpt.ask_gpt4(messages)\nprint(api_filters)\n\nresponse = requests.post(\n    "https://search.grata.com/api/v1.3/search/",\n    headers=HEADERS,\n    json={\n        "include": api_filters["include"],\n        "exclude": api_filters["exclude"],\n        "grata_employees_estimates_range": api_filters["grata_employees_estimates_range"],  \n        "headquarters": {\n            "include": api_filters["headquarters"]["include"],\n            "exclude": api_filters["headquarters"]["exclude"],\n        }\n    },\n)\n\n\nresponse\n\n\nYou will respond with the API filters for searching Grata API as a JSON object.\n\n\n'
       (0.0,)
    names      ('json', 'gandai', 'ts', 'secrets', 'openai', 'OpenAI', 'access_secret_version', 'client', 'list', 'ask_gpt4', 'HOW_TO_ENRICH', 'HOW_TO_RESPOND', 'HOW_TO_GOOGLE_MAPS', 'HOW_TO_IMPORT', 'HOW_TO_TRANSITION', 'HOW_TO_GOOGLE', 'HOW_TO_SEARCH_GRATA_API')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py'
    name       '<module>'
```

### Comparing `gandai-1.7.57/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xd7a65666 (Wed May 29 03:53:59 2024 UTC)
-files sz: 13122
+moddate:  0x3f295766 (Wed May 29 13:10:23 2024 UTC)
+files sz: 13149
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d025a020100640064
@@ -1659,66 +1659,67 @@
             166b02000000007213741b000000000000000000007c027c01ac15a60200
             00ab0200000000000000000100640053007c016a07000000000000000064
             176b02000000007213741b000000000000000000007c027c01ac15a60200
             00ab0200000000000000000100640053007c016a07000000000000000064
             186b020000000072227402000000000000000000006a0200000000000000
             00a00e00000000000000000000000000000000000000007c01ac05a60100
             00ab0100000000000000000100640053007c016a07000000000000000064
-            196b020000000072537c016a0f0000000000000000641a19000000000000
-            00000044005d437d047402000000000000000000006a0200000000000000
+            196b020000000072597c016a0f0000000000000000641a19000000000000
+            00000044005d497d047402000000000000000000006a0200000000000000
             00a01000000000000000000000000000000000000000007c04ac1ba60100
             00ab0100000000000000007d057402000000000000000000006a02000000
             0000000000a01100000000000000000000000000000000000000007c057c
-            02ac1ca6020000ab02000000000000000001008c44640053007c016a0700
-            00000000000000641d6b0200000000723674010000000000000000000064
-            1ea6010000ab01000000000000000001007402000000000000000000006a
-            020000000000000000a01200000000000000000000000000000000000000
-            007c026a130000000000000000ac1fa6010000ab01000000000000000001
-            00640053007c016a07000000000000000064206b02000000009001721f74
-            01000000000000000000007c01a6010000ab01000000000000000001007c
-            016a0f00000000000000006420190000000000000000007d067c016a0f00
-            000000000000006421190000000000000000007d077c0664226b02000000
-            00724c7402000000000000000000006a020000000000000000a014000000
-            00000000000000000000000000000000007402000000000000000000006a
-            150000000000000000a01600000000000000000000000000000000000000
-            007c026a130000000000000000640e7c037c016a170000000000000000ac
-            23a6040000ab040000000000000000a6010000ab01000000000000000001
-            00640053007c0664246b0200000000724c7402000000000000000000006a
-            020000000000000000a01400000000000000000000000000000000000000
-            007402000000000000000000006a150000000000000000a0160000000000
-            0000000000000000000000000000007c026a13000000000000000064257c
-            037c016a170000000000000000ac23a6040000ab040000000000000000a6
-            010000ab0100000000000000000100640053007c0764267600724c740200
-            0000000000000000006a020000000000000000a014000000000000000000
-            00000000000000000000007402000000000000000000006a150000000000
-            000000a01600000000000000000000000000000000000000007c026a1300
-            0000000000000064097c037c016a170000000000000000ac23a6040000ab
-            040000000000000000a6010000ab01000000000000000001006400530064
-            0053007c016a07000000000000000064276b020000000072b97c03728174
-            02000000000000000000006a020000000000000000a01800000000000000
-            000000000000000000000000007c03a6010000ab0100000000000000007d
-            087c016a0f0000000000000000a019000000000000000000000000000000
-            00000000006428a6010000ab01000000000000000072127c016a0f000000
-            00000000006428190000000000000000007c085f1a000000000000000069
-            007c086a1b0000000000000000a5017c016a0f0000000000000000a5017c
-            085f1b00000000000000007402000000000000000000006a020000000000
-            000000a01c00000000000000000000000000000000000000007c08a60100
-            00ab01000000000000000001006400530069007c026a1b00000000000000
-            00a5017c016a0f0000000000000000a5017c025f1b000000000000000074
-            02000000000000000000006a020000000000000000a01d00000000000000
-            000000000000000000000000007c02a6010000ab01000000000000000001
-            00640053007c016a07000000000000000064296b020000000072757c016a
-            0f0000000000000000642a1900000000000000000044005d697d03740100
-            000000000000000000642b7c03a6020000ab020000000000000000010074
-            02000000000000000000006a020000000000000000a01400000000000000
-            000000000000000000000000007402000000000000000000006a15000000
-            0000000000a01600000000000000000000000000000000000000007c026a
-            1300000000000000007c037c016a0f0000000000000000642c1900000000
-            00000000007c016a170000000000000000ac2da6040000ab040000000000
-            000000a6010000ab01000000000000000001008c686400530064005300
+            027c016a120000000000000000ac1ca6030000ab03000000000000000001
+            008c4a640053007c016a070000000000000000641d6b0200000000723674
+            0100000000000000000000641ea6010000ab010000000000000000010074
+            02000000000000000000006a020000000000000000a01300000000000000
+            000000000000000000000000007c026a140000000000000000ac1fa60100
+            00ab0100000000000000000100640053007c016a07000000000000000064
+            206b02000000009001721f7401000000000000000000007c01a6010000ab
+            01000000000000000001007c016a0f000000000000000064201900000000
+            00000000007d067c016a0f00000000000000006421190000000000000000
+            007d077c0664226b0200000000724c7402000000000000000000006a0200
+            00000000000000a015000000000000000000000000000000000000000074
+            02000000000000000000006a160000000000000000a01700000000000000
+            000000000000000000000000007c026a140000000000000000640e7c037c
+            016a120000000000000000ac23a6040000ab040000000000000000a60100
+            00ab0100000000000000000100640053007c0664246b0200000000724c74
+            02000000000000000000006a020000000000000000a01500000000000000
+            000000000000000000000000007402000000000000000000006a16000000
+            0000000000a01700000000000000000000000000000000000000007c026a
+            14000000000000000064257c037c016a120000000000000000ac23a60400
+            00ab040000000000000000a6010000ab0100000000000000000100640053
+            007c0764267600724c7402000000000000000000006a0200000000000000
+            00a015000000000000000000000000000000000000000074020000000000
+            00000000006a160000000000000000a01700000000000000000000000000
+            000000000000007c026a14000000000000000064097c037c016a12000000
+            0000000000ac23a6040000ab040000000000000000a6010000ab01000000
+            0000000000010064005300640053007c016a07000000000000000064276b
+            020000000072b97c0372817402000000000000000000006a020000000000
+            000000a01800000000000000000000000000000000000000007c03a60100
+            00ab0100000000000000007d087c016a0f0000000000000000a019000000
+            00000000000000000000000000000000006428a6010000ab010000000000
+            00000072127c016a0f00000000000000006428190000000000000000007c
+            085f1a000000000000000069007c086a1b0000000000000000a5017c016a
+            0f0000000000000000a5017c085f1b000000000000000074020000000000
+            00000000006a020000000000000000a01c00000000000000000000000000
+            000000000000007c08a6010000ab01000000000000000001006400530069
+            007c026a1b0000000000000000a5017c016a0f0000000000000000a5017c
+            025f1b00000000000000007402000000000000000000006a020000000000
+            000000a01d00000000000000000000000000000000000000007c02a60100
+            00ab0100000000000000000100640053007c016a07000000000000000064
+            296b020000000072757c016a0f0000000000000000642a19000000000000
+            00000044005d697d03740100000000000000000000642b7c03a6020000ab
+            02000000000000000001007402000000000000000000006a020000000000
+            000000a01500000000000000000000000000000000000000007402000000
+            000000000000006a160000000000000000a0170000000000000000000000
+            0000000000000000007c026a1400000000000000007c037c016a0f000000
+            0000000000642c190000000000000000007c016a120000000000000000ac
+            2da6040000ab040000000000000000a6010000ab01000000000000000001
+            008c686400530064005300
          281           0 RESUME                   0
          
          282           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('processing event...')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
@@ -2031,22 +2032,22 @@
                     1302 LOAD_CONST               0 (None)
                     1304 RETURN_VALUE
          
          334     >> 1306 LOAD_FAST                1 (event)
                     1308 LOAD_ATTR                7 (type)
                     1318 LOAD_CONST              25 ('import_searches')
                     1320 COMPARE_OP               2 (==)
-                    1326 POP_JUMP_FORWARD_IF_FALSE    83 (to 1494)
+                    1326 POP_JUMP_FORWARD_IF_FALSE    89 (to 1506)
          
          335        1328 LOAD_FAST                1 (event)
                     1330 LOAD_ATTR               15 (data)
                     1340 LOAD_CONST              26 ('searches')
                     1342 BINARY_SUBSCR
                     1352 GET_ITER
-                 >> 1354 FOR_ITER                67 (to 1490)
+                 >> 1354 FOR_ITER                73 (to 1502)
                     1356 STORE_FAST               4 (label)
          
          336        1358 LOAD_GLOBAL              2 (ts)
                     1370 LOAD_ATTR                2 (query)
                     1380 LOAD_METHOD             16 (find_search_by_label)
                     1402 LOAD_FAST                4 (label)
                     1404 KW_NAMES                27
@@ -2056,303 +2057,305 @@
          
          337        1422 LOAD_GLOBAL              2 (ts)
                     1434 LOAD_ATTR                2 (query)
                     1444 LOAD_METHOD             17 (important_targets_from_search)
          
          338        1466 LOAD_FAST                5 (from_search)
                     1468 LOAD_FAST                2 (search)
+                    1470 LOAD_FAST                1 (event)
+                    1472 LOAD_ATTR               18 (actor_key)
          
-         337        1470 KW_NAMES                28
-                    1472 PRECALL                  2
-                    1476 CALL                     2
-                    1486 POP_TOP
-                    1488 JUMP_BACKWARD           68 (to 1354)
-         
-         335     >> 1490 LOAD_CONST               0 (None)
-                    1492 RETURN_VALUE
-         
-         341     >> 1494 LOAD_FAST                1 (event)
-                    1496 LOAD_ATTR                7 (type)
-                    1506 LOAD_CONST              29 ('reset')
-                    1508 COMPARE_OP               2 (==)
-                    1514 POP_JUMP_FORWARD_IF_FALSE    54 (to 1624)
-         
-         342        1516 LOAD_GLOBAL              1 (NULL + print)
-                    1528 LOAD_CONST              30 ('💣 Resetting Inbox...')
-                    1530 PRECALL                  1
-                    1534 CALL                     1
-                    1544 POP_TOP
-         
-         343        1546 LOAD_GLOBAL              2 (ts)
-                    1558 LOAD_ATTR                2 (query)
-                    1568 LOAD_METHOD             18 (reset_inbox)
-                    1590 LOAD_FAST                2 (search)
-                    1592 LOAD_ATTR               19 (uid)
-                    1602 KW_NAMES                31
-                    1604 PRECALL                  1
-                    1608 CALL                     1
-                    1618 POP_TOP
-                    1620 LOAD_CONST               0 (None)
-                    1622 RETURN_VALUE
-         
-         345     >> 1624 LOAD_FAST                1 (event)
-                    1626 LOAD_ATTR                7 (type)
-                    1636 LOAD_CONST              32 ('rating')
-                    1638 COMPARE_OP               2 (==)
-                    1644 EXTENDED_ARG             1
-                    1646 POP_JUMP_FORWARD_IF_FALSE   287 (to 2222)
-         
-         347        1648 LOAD_GLOBAL              1 (NULL + print)
-                    1660 LOAD_FAST                1 (event)
-                    1662 PRECALL                  1
-                    1666 CALL                     1
-                    1676 POP_TOP
-         
-         348        1678 LOAD_FAST                1 (event)
-                    1680 LOAD_ATTR               15 (data)
-                    1690 LOAD_CONST              32 ('rating')
-                    1692 BINARY_SUBSCR
-                    1702 STORE_FAST               6 (rating)
-         
-         349        1704 LOAD_FAST                1 (event)
-                    1706 LOAD_ATTR               15 (data)
-                    1716 LOAD_CONST              33 ('currentView')
-                    1718 BINARY_SUBSCR
-                    1728 STORE_FAST               7 (from_stage)
-         
-         350        1730 LOAD_FAST                6 (rating)
-                    1732 LOAD_CONST              34 (1)
-                    1734 COMPARE_OP               2 (==)
-                    1740 POP_JUMP_FORWARD_IF_FALSE    76 (to 1894)
-         
-         351        1742 LOAD_GLOBAL              2 (ts)
-                    1754 LOAD_ATTR                2 (query)
-                    1764 LOAD_METHOD             20 (insert_event)
-         
-         352        1786 LOAD_GLOBAL              2 (ts)
-                    1798 LOAD_ATTR               21 (models)
-                    1808 LOAD_METHOD             22 (Event)
-         
-         353        1830 LOAD_FAST                2 (search)
-                    1832 LOAD_ATTR               19 (uid)
-         
-         354        1842 LOAD_CONST              14 ('reject')
-         
-         355        1844 LOAD_FAST                3 (domain)
-         
-         356        1846 LOAD_FAST                1 (event)
-                    1848 LOAD_ATTR               23 (actor_key)
-         
-         352        1858 KW_NAMES                35
-                    1860 PRECALL                  4
-                    1864 CALL                     4
-         
-         351        1874 PRECALL                  1
-                    1878 CALL                     1
-                    1888 POP_TOP
-                    1890 LOAD_CONST               0 (None)
-                    1892 RETURN_VALUE
-         
-         359     >> 1894 LOAD_FAST                6 (rating)
-                    1896 LOAD_CONST              36 (2)
-                    1898 COMPARE_OP               2 (==)
-                    1904 POP_JUMP_FORWARD_IF_FALSE    76 (to 2058)
-         
-         360        1906 LOAD_GLOBAL              2 (ts)
-                    1918 LOAD_ATTR                2 (query)
-                    1928 LOAD_METHOD             20 (insert_event)
-         
-         361        1950 LOAD_GLOBAL              2 (ts)
-                    1962 LOAD_ATTR               21 (models)
-                    1972 LOAD_METHOD             22 (Event)
-         
-         362        1994 LOAD_FAST                2 (search)
-                    1996 LOAD_ATTR               19 (uid)
-         
-         363        2006 LOAD_CONST              37 ('hold')
-         
-         364        2008 LOAD_FAST                3 (domain)
-         
-         365        2010 LOAD_FAST                1 (event)
-                    2012 LOAD_ATTR               23 (actor_key)
-         
-         361        2022 KW_NAMES                35
-                    2024 PRECALL                  4
-                    2028 CALL                     4
-         
-         360        2038 PRECALL                  1
-                    2042 CALL                     1
-                    2052 POP_TOP
-                    2054 LOAD_CONST               0 (None)
-                    2056 RETURN_VALUE
-         
-         368     >> 2058 LOAD_FAST                7 (from_stage)
-                    2060 LOAD_CONST              38 (('land', 'create', 'advance', 'hold', 'similar'))
-                    2062 CONTAINS_OP              0
-                    2064 POP_JUMP_FORWARD_IF_FALSE    76 (to 2218)
-         
-         369        2066 LOAD_GLOBAL              2 (ts)
-                    2078 LOAD_ATTR                2 (query)
-                    2088 LOAD_METHOD             20 (insert_event)
-         
-         370        2110 LOAD_GLOBAL              2 (ts)
-                    2122 LOAD_ATTR               21 (models)
-                    2132 LOAD_METHOD             22 (Event)
-         
-         371        2154 LOAD_FAST                2 (search)
-                    2156 LOAD_ATTR               19 (uid)
-         
-         372        2166 LOAD_CONST               9 ('validate')
-         
-         373        2168 LOAD_FAST                3 (domain)
-         
-         374        2170 LOAD_FAST                1 (event)
-                    2172 LOAD_ATTR               23 (actor_key)
-         
-         370        2182 KW_NAMES                35
-                    2184 PRECALL                  4
-                    2188 CALL                     4
-         
-         369        2198 PRECALL                  1
-                    2202 CALL                     1
-                    2212 POP_TOP
-                    2214 LOAD_CONST               0 (None)
-                    2216 RETURN_VALUE
-         
-         368     >> 2218 LOAD_CONST               0 (None)
-                    2220 RETURN_VALUE
-         
-         378     >> 2222 LOAD_FAST                1 (event)
-                    2224 LOAD_ATTR                7 (type)
-                    2234 LOAD_CONST              39 ('update')
-                    2236 COMPARE_OP               2 (==)
-                    2242 POP_JUMP_FORWARD_IF_FALSE   185 (to 2614)
-         
-         379        2244 LOAD_FAST                3 (domain)
-                    2246 POP_JUMP_FORWARD_IF_FALSE   129 (to 2506)
-         
-         380        2248 LOAD_GLOBAL              2 (ts)
-                    2260 LOAD_ATTR                2 (query)
-                    2270 LOAD_METHOD             24 (find_company_by_domain)
-                    2292 LOAD_FAST                3 (domain)
-                    2294 PRECALL                  1
-                    2298 CALL                     1
-                    2308 STORE_FAST               8 (company)
-         
-         381        2310 LOAD_FAST                1 (event)
-                    2312 LOAD_ATTR               15 (data)
-                    2322 LOAD_METHOD             25 (get)
-                    2344 LOAD_CONST              40 ('name')
-                    2346 PRECALL                  1
-                    2350 CALL                     1
-                    2360 POP_JUMP_FORWARD_IF_FALSE    18 (to 2398)
-         
-         382        2362 LOAD_FAST                1 (event)
-                    2364 LOAD_ATTR               15 (data)
-                    2374 LOAD_CONST              40 ('name')
-                    2376 BINARY_SUBSCR
-                    2386 LOAD_FAST                8 (company)
-                    2388 STORE_ATTR              26 (name)
-         
-         383     >> 2398 BUILD_MAP                0
-                    2400 LOAD_FAST                8 (company)
-                    2402 LOAD_ATTR               27 (meta)
-                    2412 DICT_UPDATE              1
-                    2414 LOAD_FAST                1 (event)
-                    2416 LOAD_ATTR               15 (data)
-                    2426 DICT_UPDATE              1
-                    2428 LOAD_FAST                8 (company)
-                    2430 STORE_ATTR              27 (meta)
-         
-         384        2440 LOAD_GLOBAL              2 (ts)
-                    2452 LOAD_ATTR                2 (query)
-                    2462 LOAD_METHOD             28 (update_company)
-                    2484 LOAD_FAST                8 (company)
-                    2486 PRECALL                  1
-                    2490 CALL                     1
-                    2500 POP_TOP
-                    2502 LOAD_CONST               0 (None)
-                    2504 RETURN_VALUE
-         
-         386     >> 2506 BUILD_MAP                0
-                    2508 LOAD_FAST                2 (search)
-                    2510 LOAD_ATTR               27 (meta)
-                    2520 DICT_UPDATE              1
-                    2522 LOAD_FAST                1 (event)
-                    2524 LOAD_ATTR               15 (data)
-                    2534 DICT_UPDATE              1
-                    2536 LOAD_FAST                2 (search)
-                    2538 STORE_ATTR              27 (meta)
-         
-         387        2548 LOAD_GLOBAL              2 (ts)
-                    2560 LOAD_ATTR                2 (query)
-                    2570 LOAD_METHOD             29 (update_search)
-                    2592 LOAD_FAST                2 (search)
-                    2594 PRECALL                  1
-                    2598 CALL                     1
-                    2608 POP_TOP
-                    2610 LOAD_CONST               0 (None)
-                    2612 RETURN_VALUE
-         
-         389     >> 2614 LOAD_FAST                1 (event)
-                    2616 LOAD_ATTR                7 (type)
-                    2626 LOAD_CONST              41 ('move')
-                    2628 COMPARE_OP               2 (==)
-                    2634 POP_JUMP_FORWARD_IF_FALSE   117 (to 2870)
-         
-         391        2636 LOAD_FAST                1 (event)
-                    2638 LOAD_ATTR               15 (data)
-                    2648 LOAD_CONST              42 ('domains')
-                    2650 BINARY_SUBSCR
-                    2660 GET_ITER
-                 >> 2662 FOR_ITER               105 (to 2874)
-                    2664 STORE_FAST               3 (domain)
-         
-         392        2666 LOAD_GLOBAL              1 (NULL + print)
-                    2678 LOAD_CONST              43 ('moving domain:')
-                    2680 LOAD_FAST                3 (domain)
-                    2682 PRECALL                  2
-                    2686 CALL                     2
-                    2696 POP_TOP
-         
-         393        2698 LOAD_GLOBAL              2 (ts)
-                    2710 LOAD_ATTR                2 (query)
-                    2720 LOAD_METHOD             20 (insert_event)
-         
-         394        2742 LOAD_GLOBAL              2 (ts)
-                    2754 LOAD_ATTR               21 (models)
-                    2764 LOAD_METHOD             22 (Event)
-         
-         395        2786 LOAD_FAST                2 (search)
-                    2788 LOAD_ATTR               19 (uid)
-         
-         396        2798 LOAD_FAST                3 (domain)
-         
-         397        2800 LOAD_FAST                1 (event)
-                    2802 LOAD_ATTR               15 (data)
-                    2812 LOAD_CONST              44 ('stage')
-                    2814 BINARY_SUBSCR
-         
-         398        2824 LOAD_FAST                1 (event)
-                    2826 LOAD_ATTR               23 (actor_key)
-         
-         394        2836 KW_NAMES                45
-                    2838 PRECALL                  4
-                    2842 CALL                     4
-         
-         393        2852 PRECALL                  1
-                    2856 CALL                     1
-                    2866 POP_TOP
-                    2868 JUMP_BACKWARD          104 (to 2662)
+         337        1482 KW_NAMES                28
+                    1484 PRECALL                  3
+                    1488 CALL                     3
+                    1498 POP_TOP
+                    1500 JUMP_BACKWARD           74 (to 1354)
+         
+         335     >> 1502 LOAD_CONST               0 (None)
+                    1504 RETURN_VALUE
+         
+         341     >> 1506 LOAD_FAST                1 (event)
+                    1508 LOAD_ATTR                7 (type)
+                    1518 LOAD_CONST              29 ('reset')
+                    1520 COMPARE_OP               2 (==)
+                    1526 POP_JUMP_FORWARD_IF_FALSE    54 (to 1636)
+         
+         342        1528 LOAD_GLOBAL              1 (NULL + print)
+                    1540 LOAD_CONST              30 ('💣 Resetting Inbox...')
+                    1542 PRECALL                  1
+                    1546 CALL                     1
+                    1556 POP_TOP
+         
+         343        1558 LOAD_GLOBAL              2 (ts)
+                    1570 LOAD_ATTR                2 (query)
+                    1580 LOAD_METHOD             19 (reset_inbox)
+                    1602 LOAD_FAST                2 (search)
+                    1604 LOAD_ATTR               20 (uid)
+                    1614 KW_NAMES                31
+                    1616 PRECALL                  1
+                    1620 CALL                     1
+                    1630 POP_TOP
+                    1632 LOAD_CONST               0 (None)
+                    1634 RETURN_VALUE
+         
+         345     >> 1636 LOAD_FAST                1 (event)
+                    1638 LOAD_ATTR                7 (type)
+                    1648 LOAD_CONST              32 ('rating')
+                    1650 COMPARE_OP               2 (==)
+                    1656 EXTENDED_ARG             1
+                    1658 POP_JUMP_FORWARD_IF_FALSE   287 (to 2234)
+         
+         347        1660 LOAD_GLOBAL              1 (NULL + print)
+                    1672 LOAD_FAST                1 (event)
+                    1674 PRECALL                  1
+                    1678 CALL                     1
+                    1688 POP_TOP
+         
+         348        1690 LOAD_FAST                1 (event)
+                    1692 LOAD_ATTR               15 (data)
+                    1702 LOAD_CONST              32 ('rating')
+                    1704 BINARY_SUBSCR
+                    1714 STORE_FAST               6 (rating)
+         
+         349        1716 LOAD_FAST                1 (event)
+                    1718 LOAD_ATTR               15 (data)
+                    1728 LOAD_CONST              33 ('currentView')
+                    1730 BINARY_SUBSCR
+                    1740 STORE_FAST               7 (from_stage)
+         
+         350        1742 LOAD_FAST                6 (rating)
+                    1744 LOAD_CONST              34 (1)
+                    1746 COMPARE_OP               2 (==)
+                    1752 POP_JUMP_FORWARD_IF_FALSE    76 (to 1906)
+         
+         351        1754 LOAD_GLOBAL              2 (ts)
+                    1766 LOAD_ATTR                2 (query)
+                    1776 LOAD_METHOD             21 (insert_event)
+         
+         352        1798 LOAD_GLOBAL              2 (ts)
+                    1810 LOAD_ATTR               22 (models)
+                    1820 LOAD_METHOD             23 (Event)
+         
+         353        1842 LOAD_FAST                2 (search)
+                    1844 LOAD_ATTR               20 (uid)
+         
+         354        1854 LOAD_CONST              14 ('reject')
+         
+         355        1856 LOAD_FAST                3 (domain)
+         
+         356        1858 LOAD_FAST                1 (event)
+                    1860 LOAD_ATTR               18 (actor_key)
+         
+         352        1870 KW_NAMES                35
+                    1872 PRECALL                  4
+                    1876 CALL                     4
+         
+         351        1886 PRECALL                  1
+                    1890 CALL                     1
+                    1900 POP_TOP
+                    1902 LOAD_CONST               0 (None)
+                    1904 RETURN_VALUE
+         
+         359     >> 1906 LOAD_FAST                6 (rating)
+                    1908 LOAD_CONST              36 (2)
+                    1910 COMPARE_OP               2 (==)
+                    1916 POP_JUMP_FORWARD_IF_FALSE    76 (to 2070)
+         
+         360        1918 LOAD_GLOBAL              2 (ts)
+                    1930 LOAD_ATTR                2 (query)
+                    1940 LOAD_METHOD             21 (insert_event)
+         
+         361        1962 LOAD_GLOBAL              2 (ts)
+                    1974 LOAD_ATTR               22 (models)
+                    1984 LOAD_METHOD             23 (Event)
+         
+         362        2006 LOAD_FAST                2 (search)
+                    2008 LOAD_ATTR               20 (uid)
+         
+         363        2018 LOAD_CONST              37 ('hold')
+         
+         364        2020 LOAD_FAST                3 (domain)
+         
+         365        2022 LOAD_FAST                1 (event)
+                    2024 LOAD_ATTR               18 (actor_key)
+         
+         361        2034 KW_NAMES                35
+                    2036 PRECALL                  4
+                    2040 CALL                     4
+         
+         360        2050 PRECALL                  1
+                    2054 CALL                     1
+                    2064 POP_TOP
+                    2066 LOAD_CONST               0 (None)
+                    2068 RETURN_VALUE
+         
+         368     >> 2070 LOAD_FAST                7 (from_stage)
+                    2072 LOAD_CONST              38 (('land', 'create', 'advance', 'hold', 'similar'))
+                    2074 CONTAINS_OP              0
+                    2076 POP_JUMP_FORWARD_IF_FALSE    76 (to 2230)
+         
+         369        2078 LOAD_GLOBAL              2 (ts)
+                    2090 LOAD_ATTR                2 (query)
+                    2100 LOAD_METHOD             21 (insert_event)
+         
+         370        2122 LOAD_GLOBAL              2 (ts)
+                    2134 LOAD_ATTR               22 (models)
+                    2144 LOAD_METHOD             23 (Event)
+         
+         371        2166 LOAD_FAST                2 (search)
+                    2168 LOAD_ATTR               20 (uid)
+         
+         372        2178 LOAD_CONST               9 ('validate')
+         
+         373        2180 LOAD_FAST                3 (domain)
+         
+         374        2182 LOAD_FAST                1 (event)
+                    2184 LOAD_ATTR               18 (actor_key)
+         
+         370        2194 KW_NAMES                35
+                    2196 PRECALL                  4
+                    2200 CALL                     4
+         
+         369        2210 PRECALL                  1
+                    2214 CALL                     1
+                    2224 POP_TOP
+                    2226 LOAD_CONST               0 (None)
+                    2228 RETURN_VALUE
+         
+         368     >> 2230 LOAD_CONST               0 (None)
+                    2232 RETURN_VALUE
+         
+         378     >> 2234 LOAD_FAST                1 (event)
+                    2236 LOAD_ATTR                7 (type)
+                    2246 LOAD_CONST              39 ('update')
+                    2248 COMPARE_OP               2 (==)
+                    2254 POP_JUMP_FORWARD_IF_FALSE   185 (to 2626)
+         
+         379        2256 LOAD_FAST                3 (domain)
+                    2258 POP_JUMP_FORWARD_IF_FALSE   129 (to 2518)
+         
+         380        2260 LOAD_GLOBAL              2 (ts)
+                    2272 LOAD_ATTR                2 (query)
+                    2282 LOAD_METHOD             24 (find_company_by_domain)
+                    2304 LOAD_FAST                3 (domain)
+                    2306 PRECALL                  1
+                    2310 CALL                     1
+                    2320 STORE_FAST               8 (company)
+         
+         381        2322 LOAD_FAST                1 (event)
+                    2324 LOAD_ATTR               15 (data)
+                    2334 LOAD_METHOD             25 (get)
+                    2356 LOAD_CONST              40 ('name')
+                    2358 PRECALL                  1
+                    2362 CALL                     1
+                    2372 POP_JUMP_FORWARD_IF_FALSE    18 (to 2410)
+         
+         382        2374 LOAD_FAST                1 (event)
+                    2376 LOAD_ATTR               15 (data)
+                    2386 LOAD_CONST              40 ('name')
+                    2388 BINARY_SUBSCR
+                    2398 LOAD_FAST                8 (company)
+                    2400 STORE_ATTR              26 (name)
+         
+         383     >> 2410 BUILD_MAP                0
+                    2412 LOAD_FAST                8 (company)
+                    2414 LOAD_ATTR               27 (meta)
+                    2424 DICT_UPDATE              1
+                    2426 LOAD_FAST                1 (event)
+                    2428 LOAD_ATTR               15 (data)
+                    2438 DICT_UPDATE              1
+                    2440 LOAD_FAST                8 (company)
+                    2442 STORE_ATTR              27 (meta)
+         
+         384        2452 LOAD_GLOBAL              2 (ts)
+                    2464 LOAD_ATTR                2 (query)
+                    2474 LOAD_METHOD             28 (update_company)
+                    2496 LOAD_FAST                8 (company)
+                    2498 PRECALL                  1
+                    2502 CALL                     1
+                    2512 POP_TOP
+                    2514 LOAD_CONST               0 (None)
+                    2516 RETURN_VALUE
+         
+         386     >> 2518 BUILD_MAP                0
+                    2520 LOAD_FAST                2 (search)
+                    2522 LOAD_ATTR               27 (meta)
+                    2532 DICT_UPDATE              1
+                    2534 LOAD_FAST                1 (event)
+                    2536 LOAD_ATTR               15 (data)
+                    2546 DICT_UPDATE              1
+                    2548 LOAD_FAST                2 (search)
+                    2550 STORE_ATTR              27 (meta)
+         
+         387        2560 LOAD_GLOBAL              2 (ts)
+                    2572 LOAD_ATTR                2 (query)
+                    2582 LOAD_METHOD             29 (update_search)
+                    2604 LOAD_FAST                2 (search)
+                    2606 PRECALL                  1
+                    2610 CALL                     1
+                    2620 POP_TOP
+                    2622 LOAD_CONST               0 (None)
+                    2624 RETURN_VALUE
+         
+         389     >> 2626 LOAD_FAST                1 (event)
+                    2628 LOAD_ATTR                7 (type)
+                    2638 LOAD_CONST              41 ('move')
+                    2640 COMPARE_OP               2 (==)
+                    2646 POP_JUMP_FORWARD_IF_FALSE   117 (to 2882)
+         
+         391        2648 LOAD_FAST                1 (event)
+                    2650 LOAD_ATTR               15 (data)
+                    2660 LOAD_CONST              42 ('domains')
+                    2662 BINARY_SUBSCR
+                    2672 GET_ITER
+                 >> 2674 FOR_ITER               105 (to 2886)
+                    2676 STORE_FAST               3 (domain)
+         
+         392        2678 LOAD_GLOBAL              1 (NULL + print)
+                    2690 LOAD_CONST              43 ('moving domain:')
+                    2692 LOAD_FAST                3 (domain)
+                    2694 PRECALL                  2
+                    2698 CALL                     2
+                    2708 POP_TOP
+         
+         393        2710 LOAD_GLOBAL              2 (ts)
+                    2722 LOAD_ATTR                2 (query)
+                    2732 LOAD_METHOD             21 (insert_event)
+         
+         394        2754 LOAD_GLOBAL              2 (ts)
+                    2766 LOAD_ATTR               22 (models)
+                    2776 LOAD_METHOD             23 (Event)
+         
+         395        2798 LOAD_FAST                2 (search)
+                    2800 LOAD_ATTR               20 (uid)
+         
+         396        2810 LOAD_FAST                3 (domain)
+         
+         397        2812 LOAD_FAST                1 (event)
+                    2814 LOAD_ATTR               15 (data)
+                    2824 LOAD_CONST              44 ('stage')
+                    2826 BINARY_SUBSCR
+         
+         398        2836 LOAD_FAST                1 (event)
+                    2838 LOAD_ATTR               18 (actor_key)
+         
+         394        2848 KW_NAMES                45
+                    2850 PRECALL                  4
+                    2854 CALL                     4
+         
+         393        2864 PRECALL                  1
+                    2868 CALL                     1
+                    2878 POP_TOP
+                    2880 JUMP_BACKWARD          104 (to 2674)
          
-         389     >> 2870 LOAD_CONST               0 (None)
-                    2872 RETURN_VALUE
+         389     >> 2882 LOAD_CONST               0 (None)
+                    2884 RETURN_VALUE
          
-         391     >> 2874 LOAD_CONST               0 (None)
-                    2876 RETURN_VALUE
+         391     >> 2886 LOAD_CONST               0 (None)
+                    2888 RETURN_VALUE
          consts
             None
             'processing event...'
             'event_id'
             ('uid',)
             'land'
             ('event',)
@@ -2374,15 +2377,15 @@
             ('search', 'event')
             'google'
             'grata_search'
             'import'
             'import_searches'
             'searches'
             ('label',)
-            ('from_search', 'to_search')
+            ('from_search', 'to_search', 'actor_key')
             'reset'
             '💣 Resetting Inbox...'
             ('search_uid',)
             'rating'
             'currentView'
             1
             ('search_uid', 'type', 'domain', 'actor_key')
@@ -2392,26 +2395,26 @@
             'update'
             'name'
             'move'
             'domains'
             'moving domain:'
             'stage'
             ('search_uid', 'domain', 'type', 'actor_key')
-         names      ('print', 'ts', 'query', 'find_event_by_id', 'find_search', 'search_uid', 'domain', 'type', 'run_enrichment', 'run_acquired_check', 'run_similarity_search', 'handle_prompt', 'run_maps_search', 'run_google_search', 'important_targets_from_event', 'data', 'find_search_by_label', 'important_targets_from_search', 'reset_inbox', 'uid', 'insert_event', 'models', 'Event', 'actor_key', 'find_company_by_domain', 'get', 'name', 'meta', 'update_company', 'update_search')
+         names      ('print', 'ts', 'query', 'find_event_by_id', 'find_search', 'search_uid', 'domain', 'type', 'run_enrichment', 'run_acquired_check', 'run_similarity_search', 'handle_prompt', 'run_maps_search', 'run_google_search', 'important_targets_from_event', 'data', 'find_search_by_label', 'important_targets_from_search', 'actor_key', 'reset_inbox', 'uid', 'insert_event', 'models', 'Event', 'find_company_by_domain', 'get', 'name', 'meta', 'update_company', 'update_search')
          varnames   ('event_id', 'event', 'search', 'domain', 'label', 'from_search', 'rating', 'from_stage', 'company')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'process_event'
          firstlineno 281
          lnotab
             0x02011e013e0120011e014a010e01160124011601240116012401160124
             011601200120012601160124011601200126011601040116010401160120
             012601160104021601240216012404160126011601260216012602160144
-            0216011e0140012c0104ff14fe040616011e014e0218021e011a011a010c
+            0216011e0140012c0110ff14fe040616011e014e0218021e011a011a010c
             012c012c010c01020102010cfc10ff14080c012c012c010c01020102010c
             fc10ff140808012c012c010c01020102010cfc10ff14ff040a160104013e
             01340124012a0142022a01420216021e0120012c012c010c01020118010c
             fc10ff12fc0402
    names      ('dataclasses', 'asdict', 'time', 'gandai', 'ts', 'requests', 'dacite', 'from_dict', 'secrets', 'str', 'run_acquired_check', 'models', 'Search', 'run_similarity_search', 'Event', 'run_maps_search', 'run_google_search', 'run_gpt_grata_search', 'handle_prompt', 'Company', 'enrich_with_gpt', 'run_enrichment', 'int', 'process_event')
    varnames   ()
    freevars   ()
```

### Comparing `gandai-1.7.57/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x05a75666 (Wed May 29 03:54:45 2024 UTC)
-files sz: 31209
+moddate:  0x2d295766 (Wed May 29 13:10:05 2024 UTC)
+files sz: 30959
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 15
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -14,33 +14,34 @@
       0064016c0f5a10640064076c0f6d115a110100640064086c126d135a1301
       00640064096c146d155a156d165a166d175a176d185a186d195a19010002
       006513a6000000ab0000000000000000005a1a640a6517640b6517660464
       0c84045a1b640d6516640b65106a1c00000000000000006a160000000000
       0000006604640e84045a1d640f6515640b65156604641084045a1e641165
       19640b65196604641284045a1f641365106a1c00000000000000006a1900
       00000000000000641465106a1c00000000000000006a1900000000000000
-      00640b64016606641584045a20640a65106a1c00000000000000006a1700
-      00000000000000640b64016604641684045a21090009000900643e641965
-      07650619000000000000000000641a6522641b6523641c6524641d652364
-      1e6523640b6401660e641f84055a25640b65096a26000000000000000066
-      02642084045a27642184005a28640b65096a260000000000000000660264
-      2284045a29642384005a2a642484005a2b640b65096a2600000000000000
-      006602642584045a2c640b65096a2600000000000000006602642684045a
-      2d641a65226602642784045a2e641a6522640b65096a2600000000000000
-      006604642884045a2f641a6522640b65096a260000000000000000660464
-      2984045a30641a6522640b65096a2600000000000000006604642a84045a
-      31641a6522640b65096a2600000000000000006604642b84045a32642c65
-      22640b65106a1c00000000000000006a1900000000000000006604642d84
-      045a33642e6523640b65106a1c00000000000000006a1900000000000000
-      006604642f84045a3464306523640b65106a1c00000000000000006a1900
-      000000000000006604643184045a3564326523640b65166604643384045a
-      3664346523640b65166604643584045a3764366522640b65176604643784
-      045a38640d6516640b64016604643884045a3964116519640b6401660464
-      3984045a3a64366522640b64016604643a84045a3b643b6522640b640166
-      04643c84045a3c641a6522640b64016604643d84045a3d64015300
+      0064156520640b64016608641684045a21640a65106a1c00000000000000
+      006a170000000000000000640b64016604641784045a2209000900090064
+      3e641a6507650619000000000000000000641b652364156520641c652464
+      1d6520641e6520640b6401660e641f84055a25640b65096a260000000000
+      0000006602642084045a27642184005a28640b65096a2600000000000000
+      006602642284045a29642384005a2a642484005a2b640b65096a26000000
+      00000000006602642584045a2c640b65096a260000000000000000660264
+      2684045a2d641b65236602642784045a2e641b6523640b65096a26000000
+      00000000006604642884045a2f641b6523640b65096a2600000000000000
+      006604642984045a30641b6523640b65096a260000000000000000660464
+      2a84045a31641b6523640b65096a2600000000000000006604642b84045a
+      32642c6523640b65106a1c00000000000000006a19000000000000000066
+      04642d84045a33642e6520640b65106a1c00000000000000006a19000000
+      00000000006604642f84045a3464306520640b65106a1c00000000000000
+      006a1900000000000000006604643184045a3564326520640b6516660464
+      3384045a3664346520640b65166604643584045a3764366523640b651766
+      04643784045a38640d6516640b64016604643884045a3964116519640b64
+      016604643984045a3a64366523640b64016604643a84045a3b643b652364
+      0b64016604643c84045a3c641b6523640b64016604643d84045a3d640153
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (hashlib)
                  8 STORE_NAME               0 (hashlib)
    
@@ -188,273 +189,277 @@
    
    100         306 LOAD_CONST              20 ('to_search')
    
    101         308 LOAD_NAME               16 (ts)
                310 LOAD_ATTR               28 (models)
                320 LOAD_ATTR               25 (Search)
    
-   100         330 LOAD_CONST              11 ('return')
+   100         330 LOAD_CONST              21 ('actor_key')
    
-   102         332 LOAD_CONST               1 (None)
+   101         332 LOAD_NAME               32 (str)
    
-   100         334 BUILD_TUPLE              6
-               336 LOAD_CONST              21 (<code object important_targets_from_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 100>)
-               338 MAKE_FUNCTION            4 (annotations)
-               340 STORE_NAME              32 (important_targets_from_search)
-   
-   146         342 LOAD_CONST              10 ('event')
-               344 LOAD_NAME               16 (ts)
-               346 LOAD_ATTR               28 (models)
-               356 LOAD_ATTR               23 (Event)
-               366 LOAD_CONST              11 ('return')
-               368 LOAD_CONST               1 (None)
-               370 BUILD_TUPLE              4
-               372 LOAD_CONST              22 (<code object important_targets_from_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 146>)
-               374 MAKE_FUNCTION            4 (annotations)
-               376 STORE_NAME              33 (important_targets_from_event)
-   
-   222         378 NOP
-   
-   223         380 NOP
-   
-   224         382 NOP
-   
-   218         384 LOAD_CONST              62 ((True, None, 'create'))
-               386 LOAD_CONST              25 ('companies')
-   
-   219         388 LOAD_NAME                7 (List)
-               390 LOAD_NAME                6 (Any)
-               392 BINARY_SUBSCR
-   
-   218         402 LOAD_CONST              26 ('search_uid')
-   
-   220         404 LOAD_NAME               34 (int)
-   
-   218         406 LOAD_CONST              27 ('actor_key')
-   
-   221         408 LOAD_NAME               35 (str)
-   
-   218         410 LOAD_CONST              28 ('force')
-   
-   222         412 LOAD_NAME               36 (bool)
-   
-   218         414 LOAD_CONST              29 ('source')
-   
-   223         416 LOAD_NAME               35 (str)
-   
-   218         418 LOAD_CONST              30 ('stage')
-   
-   224         420 LOAD_NAME               35 (str)
-   
-   218         422 LOAD_CONST              11 ('return')
-   
-   225         424 LOAD_CONST               1 (None)
-   
-   218         426 BUILD_TUPLE             14
-               428 LOAD_CONST              31 (<code object insert_companies_as_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 218>)
-               430 MAKE_FUNCTION            5 (defaults, annotations)
-               432 STORE_NAME              37 (insert_companies_as_targets)
-   
-   315         434 LOAD_CONST              11 ('return')
-               436 LOAD_NAME                9 (pd)
-               438 LOAD_ATTR               38 (DataFrame)
-               448 BUILD_TUPLE              2
-               450 LOAD_CONST              32 (<code object searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 315>)
-               452 MAKE_FUNCTION            4 (annotations)
-               454 STORE_NAME              39 (searches_query)
-   
-   347         456 LOAD_CONST              33 (<code object average_rating_per_search_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 347>)
-               458 MAKE_FUNCTION            0
-               460 STORE_NAME              40 (average_rating_per_search_query)
-   
-   359         462 LOAD_CONST              11 ('return')
-               464 LOAD_NAME                9 (pd)
-               466 LOAD_ATTR               38 (DataFrame)
-               476 BUILD_TUPLE              2
-               478 LOAD_CONST              34 (<code object validation_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 359>)
-               480 MAKE_FUNCTION            4 (annotations)
-               482 STORE_NAME              41 (validation_history)
-   
-   402         484 LOAD_CONST              35 (<code object searches_comment_counts, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 402>)
-               486 MAKE_FUNCTION            0
-               488 STORE_NAME              42 (searches_comment_counts)
-   
-   422         490 LOAD_CONST              36 (<code object enriched_searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 422>)
-               492 MAKE_FUNCTION            0
-               494 STORE_NAME              43 (enriched_searches_query)
-   
-   442         496 LOAD_CONST              11 ('return')
-               498 LOAD_NAME                9 (pd)
-               500 LOAD_ATTR               38 (DataFrame)
-               510 BUILD_TUPLE              2
-               512 LOAD_CONST              37 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 442>)
-               514 MAKE_FUNCTION            4 (annotations)
-               516 STORE_NAME              44 (actor)
-   
-   456         518 LOAD_CONST              11 ('return')
-               520 LOAD_NAME                9 (pd)
-               522 LOAD_ATTR               38 (DataFrame)
-               532 BUILD_TUPLE              2
-               534 LOAD_CONST              38 (<code object buyer, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 456>)
-               536 MAKE_FUNCTION            4 (annotations)
-               538 STORE_NAME              45 (buyer)
-   
-   553         540 LOAD_CONST              26 ('search_uid')
-               542 LOAD_NAME               34 (int)
-               544 BUILD_TUPLE              2
-               546 LOAD_CONST              39 (<code object search_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 553>)
-               548 MAKE_FUNCTION            4 (annotations)
-               550 STORE_NAME              46 (search_targets)
-   
-   687         552 LOAD_CONST              26 ('search_uid')
-               554 LOAD_NAME               34 (int)
-               556 LOAD_CONST              11 ('return')
-               558 LOAD_NAME                9 (pd)
-               560 LOAD_ATTR               38 (DataFrame)
-               570 BUILD_TUPLE              4
-               572 LOAD_CONST              40 (<code object search_comments, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 687>)
-               574 MAKE_FUNCTION            4 (annotations)
-               576 STORE_NAME              47 (search_comments)
-   
-   709         578 LOAD_CONST              26 ('search_uid')
-               580 LOAD_NAME               34 (int)
-               582 LOAD_CONST              11 ('return')
-               584 LOAD_NAME                9 (pd)
-               586 LOAD_ATTR               38 (DataFrame)
-               596 BUILD_TUPLE              4
-               598 LOAD_CONST              41 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 709>)
-               600 MAKE_FUNCTION            4 (annotations)
-               602 STORE_NAME              48 (event)
-   
-   721         604 LOAD_CONST              26 ('search_uid')
-               606 LOAD_NAME               34 (int)
-               608 LOAD_CONST              11 ('return')
-               610 LOAD_NAME                9 (pd)
-               612 LOAD_ATTR               38 (DataFrame)
-               622 BUILD_TUPLE              4
-               624 LOAD_CONST              42 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 721>)
-               626 MAKE_FUNCTION            4 (annotations)
-               628 STORE_NAME              49 (event_history)
-   
-   751         630 LOAD_CONST              26 ('search_uid')
-               632 LOAD_NAME               34 (int)
-               634 LOAD_CONST              11 ('return')
-               636 LOAD_NAME                9 (pd)
-               638 LOAD_ATTR               38 (DataFrame)
-               648 BUILD_TUPLE              4
-               650 LOAD_CONST              43 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 751>)
-               652 MAKE_FUNCTION            4 (annotations)
-               654 STORE_NAME              50 (search_criteria_history)
-   
-   780         656 LOAD_CONST              44 ('uid')
-               658 LOAD_NAME               34 (int)
-               660 LOAD_CONST              11 ('return')
-               662 LOAD_NAME               16 (ts)
-               664 LOAD_ATTR               28 (models)
-               674 LOAD_ATTR               25 (Search)
-               684 BUILD_TUPLE              4
-               686 LOAD_CONST              45 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 780>)
-               688 MAKE_FUNCTION            4 (annotations)
-               690 STORE_NAME              51 (find_search)
-   
-   804         692 LOAD_CONST              46 ('label')
-               694 LOAD_NAME               35 (str)
-               696 LOAD_CONST              11 ('return')
-               698 LOAD_NAME               16 (ts)
-               700 LOAD_ATTR               28 (models)
-               710 LOAD_ATTR               25 (Search)
-               720 BUILD_TUPLE              4
-               722 LOAD_CONST              47 (<code object find_search_by_label, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 804>)
-               724 MAKE_FUNCTION            4 (annotations)
-               726 STORE_NAME              52 (find_search_by_label)
-   
-   828         728 LOAD_CONST              48 ('searchToken')
-               730 LOAD_NAME               35 (str)
-               732 LOAD_CONST              11 ('return')
-               734 LOAD_NAME               16 (ts)
-               736 LOAD_ATTR               28 (models)
-               746 LOAD_ATTR               25 (Search)
-               756 BUILD_TUPLE              4
-               758 LOAD_CONST              49 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 828>)
-               760 MAKE_FUNCTION            4 (annotations)
-               762 STORE_NAME              53 (find_search_by_token)
-   
-   837         764 LOAD_CONST              50 ('domain')
-               766 LOAD_NAME               35 (str)
-               768 LOAD_CONST              11 ('return')
-               770 LOAD_NAME               22 (Company)
-               772 BUILD_TUPLE              4
-               774 LOAD_CONST              51 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 837>)
-               776 MAKE_FUNCTION            4 (annotations)
-               778 STORE_NAME              54 (find_company_by_domain)
-   
-   853         780 LOAD_CONST              52 ('email')
-               782 LOAD_NAME               35 (str)
-               784 LOAD_CONST              11 ('return')
-               786 LOAD_NAME               22 (Company)
-               788 BUILD_TUPLE              4
-               790 LOAD_CONST              53 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 853>)
-               792 MAKE_FUNCTION            4 (annotations)
-               794 STORE_NAME              55 (find_actor_by_email)
-   
-   869         796 LOAD_CONST              54 ('event_id')
-               798 LOAD_NAME               34 (int)
-               800 LOAD_CONST              11 ('return')
-               802 LOAD_NAME               23 (Event)
-               804 BUILD_TUPLE              4
-               806 LOAD_CONST              55 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 869>)
-               808 MAKE_FUNCTION            4 (annotations)
-               810 STORE_NAME              56 (find_event_by_id)
-   
-   888         812 LOAD_CONST              13 ('company')
-               814 LOAD_NAME               22 (Company)
-               816 LOAD_CONST              11 ('return')
-               818 LOAD_CONST               1 (None)
-               820 BUILD_TUPLE              4
-               822 LOAD_CONST              56 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 888>)
-               824 MAKE_FUNCTION            4 (annotations)
-               826 STORE_NAME              57 (update_company)
-   
-   917         828 LOAD_CONST              17 ('search')
-               830 LOAD_NAME               25 (Search)
-               832 LOAD_CONST              11 ('return')
-               834 LOAD_CONST               1 (None)
-               836 BUILD_TUPLE              4
-               838 LOAD_CONST              57 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 917>)
-               840 MAKE_FUNCTION            4 (annotations)
-               842 STORE_NAME              58 (update_search)
-   
-   940         844 LOAD_CONST              54 ('event_id')
-               846 LOAD_NAME               34 (int)
-               848 LOAD_CONST              11 ('return')
-               850 LOAD_CONST               1 (None)
-               852 BUILD_TUPLE              4
-               854 LOAD_CONST              58 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 940>)
-               856 MAKE_FUNCTION            4 (annotations)
-               858 STORE_NAME              59 (mute_event)
-   
-   963         860 LOAD_CONST              59 ('comment_id')
-               862 LOAD_NAME               34 (int)
-               864 LOAD_CONST              11 ('return')
-               866 LOAD_CONST               1 (None)
-               868 BUILD_TUPLE              4
-               870 LOAD_CONST              60 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 963>)
-               872 MAKE_FUNCTION            4 (annotations)
-               874 STORE_NAME              60 (delete_comment)
-   
-   974         876 LOAD_CONST              26 ('search_uid')
-               878 LOAD_NAME               34 (int)
-               880 LOAD_CONST              11 ('return')
-               882 LOAD_CONST               1 (None)
-               884 BUILD_TUPLE              4
-               886 LOAD_CONST              61 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 974>)
-               888 MAKE_FUNCTION            4 (annotations)
-               890 STORE_NAME              61 (reset_inbox)
-               892 LOAD_CONST               1 (None)
-               894 RETURN_VALUE
+   100         334 LOAD_CONST              11 ('return')
+   
+   102         336 LOAD_CONST               1 (None)
+   
+   100         338 BUILD_TUPLE              8
+               340 LOAD_CONST              22 (<code object important_targets_from_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 100>)
+               342 MAKE_FUNCTION            4 (annotations)
+               344 STORE_NAME              33 (important_targets_from_search)
+   
+   139         346 LOAD_CONST              10 ('event')
+               348 LOAD_NAME               16 (ts)
+               350 LOAD_ATTR               28 (models)
+               360 LOAD_ATTR               23 (Event)
+               370 LOAD_CONST              11 ('return')
+               372 LOAD_CONST               1 (None)
+               374 BUILD_TUPLE              4
+               376 LOAD_CONST              23 (<code object important_targets_from_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 139>)
+               378 MAKE_FUNCTION            4 (annotations)
+               380 STORE_NAME              34 (important_targets_from_event)
+   
+   215         382 NOP
+   
+   216         384 NOP
+   
+   217         386 NOP
+   
+   211         388 LOAD_CONST              62 ((True, None, 'create'))
+               390 LOAD_CONST              26 ('companies')
+   
+   212         392 LOAD_NAME                7 (List)
+               394 LOAD_NAME                6 (Any)
+               396 BINARY_SUBSCR
+   
+   211         406 LOAD_CONST              27 ('search_uid')
+   
+   213         408 LOAD_NAME               35 (int)
+   
+   211         410 LOAD_CONST              21 ('actor_key')
+   
+   214         412 LOAD_NAME               32 (str)
+   
+   211         414 LOAD_CONST              28 ('force')
+   
+   215         416 LOAD_NAME               36 (bool)
+   
+   211         418 LOAD_CONST              29 ('source')
+   
+   216         420 LOAD_NAME               32 (str)
+   
+   211         422 LOAD_CONST              30 ('stage')
+   
+   217         424 LOAD_NAME               32 (str)
+   
+   211         426 LOAD_CONST              11 ('return')
+   
+   218         428 LOAD_CONST               1 (None)
+   
+   211         430 BUILD_TUPLE             14
+               432 LOAD_CONST              31 (<code object insert_companies_as_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 211>)
+               434 MAKE_FUNCTION            5 (defaults, annotations)
+               436 STORE_NAME              37 (insert_companies_as_targets)
+   
+   308         438 LOAD_CONST              11 ('return')
+               440 LOAD_NAME                9 (pd)
+               442 LOAD_ATTR               38 (DataFrame)
+               452 BUILD_TUPLE              2
+               454 LOAD_CONST              32 (<code object searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 308>)
+               456 MAKE_FUNCTION            4 (annotations)
+               458 STORE_NAME              39 (searches_query)
+   
+   340         460 LOAD_CONST              33 (<code object average_rating_per_search_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 340>)
+               462 MAKE_FUNCTION            0
+               464 STORE_NAME              40 (average_rating_per_search_query)
+   
+   352         466 LOAD_CONST              11 ('return')
+               468 LOAD_NAME                9 (pd)
+               470 LOAD_ATTR               38 (DataFrame)
+               480 BUILD_TUPLE              2
+               482 LOAD_CONST              34 (<code object validation_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 352>)
+               484 MAKE_FUNCTION            4 (annotations)
+               486 STORE_NAME              41 (validation_history)
+   
+   395         488 LOAD_CONST              35 (<code object searches_comment_counts, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 395>)
+               490 MAKE_FUNCTION            0
+               492 STORE_NAME              42 (searches_comment_counts)
+   
+   415         494 LOAD_CONST              36 (<code object enriched_searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 415>)
+               496 MAKE_FUNCTION            0
+               498 STORE_NAME              43 (enriched_searches_query)
+   
+   435         500 LOAD_CONST              11 ('return')
+               502 LOAD_NAME                9 (pd)
+               504 LOAD_ATTR               38 (DataFrame)
+               514 BUILD_TUPLE              2
+               516 LOAD_CONST              37 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 435>)
+               518 MAKE_FUNCTION            4 (annotations)
+               520 STORE_NAME              44 (actor)
+   
+   449         522 LOAD_CONST              11 ('return')
+               524 LOAD_NAME                9 (pd)
+               526 LOAD_ATTR               38 (DataFrame)
+               536 BUILD_TUPLE              2
+               538 LOAD_CONST              38 (<code object buyer, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 449>)
+               540 MAKE_FUNCTION            4 (annotations)
+               542 STORE_NAME              45 (buyer)
+   
+   546         544 LOAD_CONST              27 ('search_uid')
+               546 LOAD_NAME               35 (int)
+               548 BUILD_TUPLE              2
+               550 LOAD_CONST              39 (<code object search_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 546>)
+               552 MAKE_FUNCTION            4 (annotations)
+               554 STORE_NAME              46 (search_targets)
+   
+   680         556 LOAD_CONST              27 ('search_uid')
+               558 LOAD_NAME               35 (int)
+               560 LOAD_CONST              11 ('return')
+               562 LOAD_NAME                9 (pd)
+               564 LOAD_ATTR               38 (DataFrame)
+               574 BUILD_TUPLE              4
+               576 LOAD_CONST              40 (<code object search_comments, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 680>)
+               578 MAKE_FUNCTION            4 (annotations)
+               580 STORE_NAME              47 (search_comments)
+   
+   702         582 LOAD_CONST              27 ('search_uid')
+               584 LOAD_NAME               35 (int)
+               586 LOAD_CONST              11 ('return')
+               588 LOAD_NAME                9 (pd)
+               590 LOAD_ATTR               38 (DataFrame)
+               600 BUILD_TUPLE              4
+               602 LOAD_CONST              41 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 702>)
+               604 MAKE_FUNCTION            4 (annotations)
+               606 STORE_NAME              48 (event)
+   
+   714         608 LOAD_CONST              27 ('search_uid')
+               610 LOAD_NAME               35 (int)
+               612 LOAD_CONST              11 ('return')
+               614 LOAD_NAME                9 (pd)
+               616 LOAD_ATTR               38 (DataFrame)
+               626 BUILD_TUPLE              4
+               628 LOAD_CONST              42 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 714>)
+               630 MAKE_FUNCTION            4 (annotations)
+               632 STORE_NAME              49 (event_history)
+   
+   744         634 LOAD_CONST              27 ('search_uid')
+               636 LOAD_NAME               35 (int)
+               638 LOAD_CONST              11 ('return')
+               640 LOAD_NAME                9 (pd)
+               642 LOAD_ATTR               38 (DataFrame)
+               652 BUILD_TUPLE              4
+               654 LOAD_CONST              43 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 744>)
+               656 MAKE_FUNCTION            4 (annotations)
+               658 STORE_NAME              50 (search_criteria_history)
+   
+   773         660 LOAD_CONST              44 ('uid')
+               662 LOAD_NAME               35 (int)
+               664 LOAD_CONST              11 ('return')
+               666 LOAD_NAME               16 (ts)
+               668 LOAD_ATTR               28 (models)
+               678 LOAD_ATTR               25 (Search)
+               688 BUILD_TUPLE              4
+               690 LOAD_CONST              45 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 773>)
+               692 MAKE_FUNCTION            4 (annotations)
+               694 STORE_NAME              51 (find_search)
+   
+   797         696 LOAD_CONST              46 ('label')
+               698 LOAD_NAME               32 (str)
+               700 LOAD_CONST              11 ('return')
+               702 LOAD_NAME               16 (ts)
+               704 LOAD_ATTR               28 (models)
+               714 LOAD_ATTR               25 (Search)
+               724 BUILD_TUPLE              4
+               726 LOAD_CONST              47 (<code object find_search_by_label, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 797>)
+               728 MAKE_FUNCTION            4 (annotations)
+               730 STORE_NAME              52 (find_search_by_label)
+   
+   821         732 LOAD_CONST              48 ('searchToken')
+               734 LOAD_NAME               32 (str)
+               736 LOAD_CONST              11 ('return')
+               738 LOAD_NAME               16 (ts)
+               740 LOAD_ATTR               28 (models)
+               750 LOAD_ATTR               25 (Search)
+               760 BUILD_TUPLE              4
+               762 LOAD_CONST              49 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 821>)
+               764 MAKE_FUNCTION            4 (annotations)
+               766 STORE_NAME              53 (find_search_by_token)
+   
+   830         768 LOAD_CONST              50 ('domain')
+               770 LOAD_NAME               32 (str)
+               772 LOAD_CONST              11 ('return')
+               774 LOAD_NAME               22 (Company)
+               776 BUILD_TUPLE              4
+               778 LOAD_CONST              51 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 830>)
+               780 MAKE_FUNCTION            4 (annotations)
+               782 STORE_NAME              54 (find_company_by_domain)
+   
+   846         784 LOAD_CONST              52 ('email')
+               786 LOAD_NAME               32 (str)
+               788 LOAD_CONST              11 ('return')
+               790 LOAD_NAME               22 (Company)
+               792 BUILD_TUPLE              4
+               794 LOAD_CONST              53 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 846>)
+               796 MAKE_FUNCTION            4 (annotations)
+               798 STORE_NAME              55 (find_actor_by_email)
+   
+   862         800 LOAD_CONST              54 ('event_id')
+               802 LOAD_NAME               35 (int)
+               804 LOAD_CONST              11 ('return')
+               806 LOAD_NAME               23 (Event)
+               808 BUILD_TUPLE              4
+               810 LOAD_CONST              55 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 862>)
+               812 MAKE_FUNCTION            4 (annotations)
+               814 STORE_NAME              56 (find_event_by_id)
+   
+   881         816 LOAD_CONST              13 ('company')
+               818 LOAD_NAME               22 (Company)
+               820 LOAD_CONST              11 ('return')
+               822 LOAD_CONST               1 (None)
+               824 BUILD_TUPLE              4
+               826 LOAD_CONST              56 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 881>)
+               828 MAKE_FUNCTION            4 (annotations)
+               830 STORE_NAME              57 (update_company)
+   
+   910         832 LOAD_CONST              17 ('search')
+               834 LOAD_NAME               25 (Search)
+               836 LOAD_CONST              11 ('return')
+               838 LOAD_CONST               1 (None)
+               840 BUILD_TUPLE              4
+               842 LOAD_CONST              57 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 910>)
+               844 MAKE_FUNCTION            4 (annotations)
+               846 STORE_NAME              58 (update_search)
+   
+   933         848 LOAD_CONST              54 ('event_id')
+               850 LOAD_NAME               35 (int)
+               852 LOAD_CONST              11 ('return')
+               854 LOAD_CONST               1 (None)
+               856 BUILD_TUPLE              4
+               858 LOAD_CONST              58 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 933>)
+               860 MAKE_FUNCTION            4 (annotations)
+               862 STORE_NAME              59 (mute_event)
+   
+   956         864 LOAD_CONST              59 ('comment_id')
+               866 LOAD_NAME               35 (int)
+               868 LOAD_CONST              11 ('return')
+               870 LOAD_CONST               1 (None)
+               872 BUILD_TUPLE              4
+               874 LOAD_CONST              60 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 956>)
+               876 MAKE_FUNCTION            4 (annotations)
+               878 STORE_NAME              60 (delete_comment)
+   
+   967         880 LOAD_CONST              27 ('search_uid')
+               882 LOAD_NAME               35 (int)
+               884 LOAD_CONST              11 ('return')
+               886 LOAD_CONST               1 (None)
+               888 BUILD_TUPLE              4
+               890 LOAD_CONST              61 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 967>)
+               892 MAKE_FUNCTION            4 (annotations)
+               894 STORE_NAME              61 (reset_inbox)
+               896 LOAD_CONST               1 (None)
+               898 RETURN_VALUE
    consts
       0
       None
       ('asdict',)
       ('time',)
       ('Any', 'List')
       ('from_dict',)
@@ -948,241 +953,249 @@
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_search'
          firstlineno 84
          lnotab 0x02013401160102ff10071e013a012c0128f52e0c
       'from_search'
       'to_search'
+      'actor_key'
       code
-         argcount  : 2
-         nlocals   : 10
-         stacksize : 11
+         argcount  : 3
+         nlocals   : 8
+         stacksize : 7
          flags     : 3
          code
-            0x97007401000000000000000000007c006a010000000000000000ac01a6
-            010000ab0100000000000000007d027c027c026402190000000000000000
-            0064036b0300000000190000000000000000007d027c0264041900000000
-            0000000000a0020000000000000000000000000000000000000000a60000
-            00ab0000000000000000007d037407000000000000000000007409000000
-            000000000000007c03a6010000ab010000000000000000a6010000ab0100
-            00000000000000010067007d04740a00000000000000000000a006000000
-            0000000000000000000000000000000000a6000000ab0000000000000000
-            0035007d057c05a0070000000000000000000000000000000000000000a6
-            000000ab000000000000000000350001007c0344005d7e7d067410000000
-            000000000000006a090000000000000000a00a0000000000000000000000
-            0000000000000000007c06a6010000ab0100000000000000007d067c05a0
-            0b0000000000000000000000000000000000000000741900000000000000
-            0000006a0d00000000000000006405a6010000ab0100000000000000007c
-            016a01000000000000000064067c06640764089c04a6020000ab02000000
-            00000000007d077c07a00e00000000000000000000000000000000000000
-            00a6000000ab0000000000000000007d087c0881157c04a00f0000000000
-            0000000000000000000000000000007c08a6010000ab0100000000000000
-            0001008c7f0900640064006400a6020000ab02000000000000000001006e
-            0b23003100730477027803590077010100590001000100640064006400a6
-            020000ab02000000000000000001006e0b23003100730477027803590077
-            0101005900010001007c0444005d177d097411000000000000000000006a
-            1000000000000000007c09ac09a6010000ab01000000000000000001008c
-            1864005300
-         100           0 RESUME                   0
-         
-         107           2 LOAD_GLOBAL              1 (NULL + search_targets)
-                      14 LOAD_FAST                0 (from_search)
-                      16 LOAD_ATTR                1 (uid)
-                      26 KW_NAMES                 1
-                      28 PRECALL                  1
-                      32 CALL                     1
-                      42 STORE_FAST               2 (targets)
-         
-         108          44 LOAD_FAST                2 (targets)
-                      46 LOAD_FAST                2 (targets)
-                      48 LOAD_CONST               2 ('stage')
-                      50 BINARY_SUBSCR
-                      60 LOAD_CONST               3 ('reject')
-                      62 COMPARE_OP               3 (!=)
-                      68 BINARY_SUBSCR
-                      78 STORE_FAST               2 (targets)
-         
-         109          80 LOAD_FAST                2 (targets)
-                      82 LOAD_CONST               4 ('domain')
-                      84 BINARY_SUBSCR
-                      94 LOAD_METHOD              2 (tolist)
-                     116 PRECALL                  0
-                     120 CALL                     0
-                     130 STORE_FAST               3 (domains)
-         
-         110         132 LOAD_GLOBAL              7 (NULL + print)
-                     144 LOAD_GLOBAL              9 (NULL + len)
-                     156 LOAD_FAST                3 (domains)
-                     158 PRECALL                  1
-                     162 CALL                     1
-                     172 PRECALL                  1
-                     176 CALL                     1
-                     186 POP_TOP
+            0x8701870297007401000000000000000000007c006a0100000000000000
+            00ac01a6010000ab0100000000000000007d037c037c0364021900000000
+            000000000064036b0300000000190000000000000000007d037c037c0364
+            021900000000000000000064046b0300000000190000000000000000007d
+            037405000000000000000000007c03a6010000ab01000000000000000001
+            007c03640519000000000000000000a00300000000000000000000000000
+            00000000000000a6000000ab0000000000000000007d0474050000000000
+            00000000007409000000000000000000007c04a6010000ab010000000000
+            000000a6010000ab0100000000000000000100740a000000000000000000
+            00a0060000000000000000000000000000000000000000a6000000ab0000
+            0000000000000035007d057c05a007000000000000000000000000000000
+            0000000000a6000000ab0000000000000000003500010088028801660264
+            0684087c044400a6000000ab0000000000000000007d067c05a008000000
+            00000000000000000000000000000000007413000000000000000000006a
+            0a00000000000000006407a6010000ab0100000000000000007c06a60200
+            00ab0200000000000000007d07640064006400a6020000ab020000000000
+            00000001006e0b2300310073047702780359007701010059000100010064
+            0064006400a6020000ab0200000000000000000100640053002300310073
+            047702780359007701010059000100010064005300
+                       0 MAKE_CELL                1 (to_search)
+                       2 MAKE_CELL                2 (actor_key)
          
-         114         188 BUILD_LIST               0
-                     190 STORE_FAST               4 (new_event_ids)
+         100           4 RESUME                   0
          
-         115         192 LOAD_GLOBAL             10 (db)
-                     204 LOAD_METHOD              6 (connect)
-                     226 PRECALL                  0
-                     230 CALL                     0
-                     240 BEFORE_WITH
-                     242 STORE_FAST               5 (con)
+         107           6 LOAD_GLOBAL              1 (NULL + search_targets)
+                      18 LOAD_FAST                0 (from_search)
+                      20 LOAD_ATTR                1 (uid)
+                      30 KW_NAMES                 1
+                      32 PRECALL                  1
+                      36 CALL                     1
+                      46 STORE_FAST               3 (targets)
+         
+         108          48 LOAD_FAST                3 (targets)
+                      50 LOAD_FAST                3 (targets)
+                      52 LOAD_CONST               2 ('stage')
+                      54 BINARY_SUBSCR
+                      64 LOAD_CONST               3 ('reject')
+                      66 COMPARE_OP               3 (!=)
+                      72 BINARY_SUBSCR
+                      82 STORE_FAST               3 (targets)
+         
+         109          84 LOAD_FAST                3 (targets)
+                      86 LOAD_FAST                3 (targets)
+                      88 LOAD_CONST               2 ('stage')
+                      90 BINARY_SUBSCR
+                     100 LOAD_CONST               4 ('create')
+                     102 COMPARE_OP               3 (!=)
+                     108 BINARY_SUBSCR
+                     118 STORE_FAST               3 (targets)
          
-         116         244 LOAD_FAST                5 (con)
-                     246 LOAD_METHOD              7 (begin)
-                     268 PRECALL                  0
-                     272 CALL                     0
-                     282 BEFORE_WITH
-                     284 POP_TOP
-         
-         117         286 LOAD_FAST                3 (domains)
-                     288 GET_ITER
-                 >>  290 FOR_ITER               126 (to 544)
-                     292 STORE_FAST               6 (domain)
-         
-         119         294 LOAD_GLOBAL             16 (ts)
-                     306 LOAD_ATTR                9 (helpers)
-                     316 LOAD_METHOD             10 (clean_domain)
-                     338 LOAD_FAST                6 (domain)
-                     340 PRECALL                  1
-                     344 CALL                     1
-                     354 STORE_FAST               6 (domain)
-         
-         121         356 LOAD_FAST                5 (con)
-                     358 LOAD_METHOD             11 (execute)
-         
-         122         380 LOAD_GLOBAL             25 (NULL + sqlalchemy)
-                     392 LOAD_ATTR               13 (text)
-         
-         123         402 LOAD_CONST               5 ('\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        ')
-         
-         122         404 PRECALL                  1
-                     408 CALL                     1
-         
-         131         418 LOAD_FAST                1 (to_search)
-                     420 LOAD_ATTR                1 (uid)
-         
-         132         430 LOAD_CONST               6 ('chatgpt')
-         
-         133         432 LOAD_FAST                6 (domain)
-         
-         134         434 LOAD_CONST               7 ('land')
-         
-         130         436 LOAD_CONST               8 (('search_uid', 'actor_key', 'domain', 'type'))
-                     438 BUILD_CONST_KEY_MAP      4
-         
-         121         440 PRECALL                  2
-                     444 CALL                     2
-                     454 STORE_FAST               7 (result)
-         
-         138         456 LOAD_FAST                7 (result)
-                     458 LOAD_METHOD             14 (scalar_one)
-                     480 PRECALL                  0
-                     484 CALL                     0
-                     494 STORE_FAST               8 (new_event_id)
-         
-         139         496 LOAD_FAST                8 (new_event_id)
-                     498 POP_JUMP_FORWARD_IF_NONE    21 (to 542)
-         
-         140         500 LOAD_FAST                4 (new_event_ids)
-                     502 LOAD_METHOD             15 (append)
-                     524 LOAD_FAST                8 (new_event_id)
-                     526 PRECALL                  1
-                     530 CALL                     1
-                     540 POP_TOP
-                 >>  542 JUMP_BACKWARD          127 (to 290)
-         
-         117     >>  544 NOP
-         
-         116         546 LOAD_CONST               0 (None)
-                     548 LOAD_CONST               0 (None)
-                     550 LOAD_CONST               0 (None)
-                     552 PRECALL                  2
-                     556 CALL                     2
-                     566 POP_TOP
-                     568 JUMP_FORWARD            11 (to 592)
-                 >>  570 PUSH_EXC_INFO
-                     572 WITH_EXCEPT_START
-                     574 POP_JUMP_FORWARD_IF_TRUE     4 (to 584)
-                     576 RERAISE                  2
-                 >>  578 COPY                     3
-                     580 POP_EXCEPT
-                     582 RERAISE                  1
-                 >>  584 POP_TOP
-                     586 POP_EXCEPT
-                     588 POP_TOP
-                     590 POP_TOP
-         
-         115     >>  592 LOAD_CONST               0 (None)
-                     594 LOAD_CONST               0 (None)
-                     596 LOAD_CONST               0 (None)
-                     598 PRECALL                  2
-                     602 CALL                     2
-                     612 POP_TOP
-                     614 JUMP_FORWARD            11 (to 638)
-                 >>  616 PUSH_EXC_INFO
-                     618 WITH_EXCEPT_START
-                     620 POP_JUMP_FORWARD_IF_TRUE     4 (to 630)
-                     622 RERAISE                  2
-                 >>  624 COPY                     3
-                     626 POP_EXCEPT
-                     628 RERAISE                  1
-                 >>  630 POP_TOP
-                     632 POP_EXCEPT
-                     634 POP_TOP
-                     636 POP_TOP
-         
-         142     >>  638 LOAD_FAST                4 (new_event_ids)
-                     640 GET_ITER
-                 >>  642 FOR_ITER                23 (to 690)
-                     644 STORE_FAST               9 (event_id)
-         
-         143         646 LOAD_GLOBAL             17 (NULL + ts)
-                     658 LOAD_ATTR               16 (trigger_process_event)
-                     668 LOAD_FAST                9 (event_id)
-                     670 KW_NAMES                 9
-                     672 PRECALL                  1
-                     676 CALL                     1
-                     686 POP_TOP
-                     688 JUMP_BACKWARD           24 (to 642)
+         110         120 LOAD_GLOBAL              5 (NULL + print)
+                     132 LOAD_FAST                3 (targets)
+                     134 PRECALL                  1
+                     138 CALL                     1
+                     148 POP_TOP
+         
+         111         150 LOAD_FAST                3 (targets)
+                     152 LOAD_CONST               5 ('domain')
+                     154 BINARY_SUBSCR
+                     164 LOAD_METHOD              3 (tolist)
+                     186 PRECALL                  0
+                     190 CALL                     0
+                     200 STORE_FAST               4 (domains)
+         
+         112         202 LOAD_GLOBAL              5 (NULL + print)
+                     214 LOAD_GLOBAL              9 (NULL + len)
+                     226 LOAD_FAST                4 (domains)
+                     228 PRECALL                  1
+                     232 CALL                     1
+                     242 PRECALL                  1
+                     246 CALL                     1
+                     256 POP_TOP
+         
+         114         258 LOAD_GLOBAL             10 (db)
+                     270 LOAD_METHOD              6 (connect)
+                     292 PRECALL                  0
+                     296 CALL                     0
+                     306 BEFORE_WITH
+                     308 STORE_FAST               5 (con)
+         
+         115         310 LOAD_FAST                5 (con)
+                     312 LOAD_METHOD              7 (begin)
+                     334 PRECALL                  0
+                     338 CALL                     0
+                     348 BEFORE_WITH
+                     350 POP_TOP
+         
+         116         352 LOAD_CLOSURE             2 (actor_key)
+                     354 LOAD_CLOSURE             1 (to_search)
+                     356 BUILD_TUPLE              2
+                     358 LOAD_CONST               6 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 116>)
+                     360 MAKE_FUNCTION            8 (closure)
+         
+         123         362 LOAD_FAST                4 (domains)
+         
+         116         364 GET_ITER
+                     366 PRECALL                  0
+                     370 CALL                     0
+                     380 STORE_FAST               6 (events)
+         
+         126         382 LOAD_FAST                5 (con)
+                     384 LOAD_METHOD              8 (execute)
+         
+         127         406 LOAD_GLOBAL             19 (NULL + sqlalchemy)
+                     418 LOAD_ATTR               10 (text)
          
-         142     >>  690 LOAD_CONST               0 (None)
-                     692 RETURN_VALUE
+         128         428 LOAD_CONST               7 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES (:search_uid, :domain, :actor_key, :type)\n                    ON CONFLICT DO NOTHING\n                    RETURNING id\n                    ')
+         
+         127         430 PRECALL                  1
+                     434 CALL                     1
+         
+         135         444 LOAD_FAST                6 (events)
+         
+         126         446 PRECALL                  2
+                     450 CALL                     2
+                     460 STORE_FAST               7 (result)
+         
+         115         462 LOAD_CONST               0 (None)
+                     464 LOAD_CONST               0 (None)
+                     466 LOAD_CONST               0 (None)
+                     468 PRECALL                  2
+                     472 CALL                     2
+                     482 POP_TOP
+                     484 JUMP_FORWARD            11 (to 508)
+                 >>  486 PUSH_EXC_INFO
+                     488 WITH_EXCEPT_START
+                     490 POP_JUMP_FORWARD_IF_TRUE     4 (to 500)
+                     492 RERAISE                  2
+                 >>  494 COPY                     3
+                     496 POP_EXCEPT
+                     498 RERAISE                  1
+                 >>  500 POP_TOP
+                     502 POP_EXCEPT
+                     504 POP_TOP
+                     506 POP_TOP
+         
+         114     >>  508 LOAD_CONST               0 (None)
+                     510 LOAD_CONST               0 (None)
+                     512 LOAD_CONST               0 (None)
+                     514 PRECALL                  2
+                     518 CALL                     2
+                     528 POP_TOP
+                     530 LOAD_CONST               0 (None)
+                     532 RETURN_VALUE
+                 >>  534 PUSH_EXC_INFO
+                     536 WITH_EXCEPT_START
+                     538 POP_JUMP_FORWARD_IF_TRUE     4 (to 548)
+                     540 RERAISE                  2
+                 >>  542 COPY                     3
+                     544 POP_EXCEPT
+                     546 RERAISE                  1
+                 >>  548 POP_TOP
+                     550 POP_EXCEPT
+                     552 POP_TOP
+                     554 POP_TOP
+                     556 LOAD_CONST               0 (None)
+                     558 RETURN_VALUE
          ExceptionTable:
-           242 to 282 -> 616 [1] lasti
-           284 to 542 -> 570 [2] lasti
-           546 to 568 -> 616 [1] lasti
-           570 to 576 -> 578 [4] lasti
-           578 to 582 -> 616 [1] lasti
-           584 to 584 -> 578 [4] lasti
-           586 to 590 -> 616 [1] lasti
-           616 to 622 -> 624 [3] lasti
-           630 to 630 -> 624 [3] lasti
+           308 to 348 -> 534 [1] lasti
+           350 to 460 -> 486 [2] lasti
+           462 to 484 -> 534 [1] lasti
+           486 to 492 -> 494 [4] lasti
+           494 to 498 -> 534 [1] lasti
+           500 to 500 -> 494 [4] lasti
+           502 to 506 -> 534 [1] lasti
+           534 to 540 -> 542 [3] lasti
+           548 to 548 -> 542 [3] lasti
          consts
             None
             ('search_uid',)
             'stage'
             'reject'
+            'create'
             'domain'
-            '\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        '
-            'chatgpt'
-            'land'
-            ('search_uid', 'actor_key', 'domain', 'type')
-            ('event_id',)
-         names      ('search_targets', 'uid', 'tolist', 'print', 'len', 'db', 'connect', 'begin', 'ts', 'helpers', 'clean_domain', 'execute', 'sqlalchemy', 'text', 'scalar_one', 'append', 'trigger_process_event')
-         varnames   ('from_search', 'to_search', 'targets', 'domains', 'new_event_ids', 'con', 'domain', 'result', 'new_event_id', 'event_id')
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 7
+               flags     : 19
+               code
+                  0x9502970067007c005d0e7d0189036a0000000000000000007c01890264
+                  0064019c0491028c0f5300
+                             0 COPY_FREE_VARS           2
+               
+               116           2 RESUME                   0
+                             4 BUILD_LIST               0
+                             6 LOAD_FAST                0 (.0)
+                       >>    8 FOR_ITER                14 (to 38)
+               
+               123          10 STORE_FAST               1 (domain)
+               
+               118          12 LOAD_DEREF               3 (to_search)
+                            14 LOAD_ATTR                0 (uid)
+               
+               119          24 LOAD_FAST                1 (domain)
+               
+               120          26 LOAD_DEREF               2 (actor_key)
+               
+               121          28 LOAD_CONST               0 ('land')
+               
+               117          30 LOAD_CONST               1 (('search_uid', 'domain', 'actor_key', 'type'))
+                            32 BUILD_CONST_KEY_MAP      4
+               
+               116          34 LIST_APPEND              2
+                            36 JUMP_BACKWARD           15 (to 8)
+                       >>   38 RETURN_VALUE
+               consts
+                  'land'
+                  ('search_uid', 'domain', 'actor_key', 'type')
+               names      ('uid',)
+               varnames   ('.0', 'domain')
+               freevars   ('actor_key', 'to_search')
+               cellvars   ()
+               filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
+               name       '<listcomp>'
+               firstlineno 116
+               lnotab 0x0a0702fb0c010201020102fc04ff
+            '\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES (:search_uid, :domain, :actor_key, :type)\n                    ON CONFLICT DO NOTHING\n                    RETURNING id\n                    '
+         names      ('search_targets', 'uid', 'print', 'tolist', 'len', 'db', 'connect', 'begin', 'execute', 'sqlalchemy', 'text')
+         varnames   ('from_search', 'to_search', 'actor_key', 'targets', 'domains', 'con', 'events', 'result')
          freevars   ()
-         cellvars   ()
+         cellvars   ('to_search', 'actor_key')
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'important_targets_from_search'
          firstlineno 100
          lnotab
-            0x02072a01240134013804040134012a0108023e021801160102ff0e090c
-            010201020102fc04f71011280104012ce902ff2eff2e1b08012cff
+            0x06072a01240124011e013401380234012a010a0702f9120a1801160102
+            ff0e0802f710f52eff
       code
          argcount  : 1
          nlocals   : 12
          stacksize : 16
          flags     : 3
          code
             0x870c97007c006a000000000000000000a0010000000000000000000000
@@ -1223,179 +1236,179 @@
             00640064006400a6020000ab02000000000000000001006e0b2300310073
             0477027803590077010100590001000100640064006400a6020000ab0200
             0000000000000001006e0b23003100730477027803590077010100590001
             0001007c0544005d177d0b7413000000000000000000006a180000000000
             0000007c0bac0fa6010000ab01000000000000000001008c1864005300
                        0 MAKE_CELL               12 (stage_dict)
          
-         146           2 RESUME                   0
+         139           2 RESUME                   0
          
-         148           4 LOAD_FAST                0 (event)
+         141           4 LOAD_FAST                0 (event)
                        6 LOAD_ATTR                0 (data)
                       16 LOAD_METHOD              1 (get)
                       38 LOAD_CONST               1 ('source')
                       40 PRECALL                  1
                       44 CALL                     1
                       54 STORE_FAST               1 (source)
          
-         149          56 LOAD_GLOBAL              5 (NULL + search_targets)
+         142          56 LOAD_GLOBAL              5 (NULL + search_targets)
                       68 LOAD_FAST                0 (event)
                       70 LOAD_ATTR                3 (search_uid)
                       80 KW_NAMES                 2
                       82 PRECALL                  1
                       86 CALL                     1
                       96 STORE_FAST               2 (targets)
          
-         150          98 LOAD_FAST                2 (targets)
+         143          98 LOAD_FAST                2 (targets)
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
          
-         152         188 LOAD_CLOSURE            12 (stage_dict)
+         145         188 LOAD_CLOSURE            12 (stage_dict)
                      190 BUILD_TUPLE              1
-                     192 LOAD_CONST               5 (<code object get_stage, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 152>)
+                     192 LOAD_CONST               5 (<code object get_stage, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 145>)
                      194 MAKE_FUNCTION            8 (closure)
                      196 STORE_FAST               3 (get_stage)
          
-         156         198 LOAD_FAST                0 (event)
+         149         198 LOAD_FAST                0 (event)
                      200 LOAD_ATTR                0 (data)
                      210 LOAD_CONST               6 ('domains')
                      212 BINARY_SUBSCR
                      222 STORE_FAST               4 (domains)
          
-         158         224 BUILD_LIST               0
+         151         224 BUILD_LIST               0
                      226 STORE_FAST               5 (new_event_ids)
          
-         159         228 LOAD_GLOBAL             12 (db)
+         152         228 LOAD_GLOBAL             12 (db)
                      240 LOAD_METHOD              7 (connect)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 BEFORE_WITH
                      278 STORE_FAST               6 (con)
          
-         160         280 LOAD_FAST                6 (con)
+         153         280 LOAD_FAST                6 (con)
                      282 LOAD_METHOD              8 (begin)
                      304 PRECALL                  0
                      308 CALL                     0
                      318 BEFORE_WITH
                      320 POP_TOP
          
-         161         322 LOAD_FAST                4 (domains)
+         154         322 LOAD_FAST                4 (domains)
                      324 GET_ITER
                  >>  326 EXTENDED_ARG             1
                      328 FOR_ITER               359 (to 1048)
                      330 STORE_FAST               7 (domain)
          
-         163         332 LOAD_GLOBAL             18 (ts)
+         156         332 LOAD_GLOBAL             18 (ts)
                      344 LOAD_ATTR               10 (helpers)
                      354 LOAD_METHOD             11 (clean_domain)
                      376 LOAD_FAST                7 (domain)
                      378 PRECALL                  1
                      382 CALL                     1
                      392 STORE_FAST               7 (domain)
          
-         164         394 LOAD_FAST                6 (con)
+         157         394 LOAD_FAST                6 (con)
                      396 LOAD_METHOD             12 (execute)
          
-         165         418 LOAD_GLOBAL             27 (NULL + sqlalchemy)
+         158         418 LOAD_GLOBAL             27 (NULL + sqlalchemy)
                      430 LOAD_ATTR               14 (text)
          
-         166         440 LOAD_CONST               7 ('\n                        INSERT INTO company (domain, source) \n                        VALUES(:domain, :source)\n                        ON CONFLICT DO NOTHING\n                        ')
+         159         440 LOAD_CONST               7 ('\n                        INSERT INTO company (domain, source) \n                        VALUES(:domain, :source)\n                        ON CONFLICT DO NOTHING\n                        ')
          
-         165         442 PRECALL                  1
+         158         442 PRECALL                  1
                      446 CALL                     1
          
-         172         456 LOAD_FAST                7 (domain)
+         165         456 LOAD_FAST                7 (domain)
                      458 LOAD_FAST                1 (source)
                      460 LOAD_CONST               8 (('domain', 'source'))
                      462 BUILD_CONST_KEY_MAP      2
          
-         164         464 PRECALL                  2
+         157         464 PRECALL                  2
                      468 CALL                     2
                      478 POP_TOP
          
-         175         480 LOAD_FAST                6 (con)
+         168         480 LOAD_FAST                6 (con)
                      482 LOAD_METHOD             12 (execute)
          
-         176         504 LOAD_GLOBAL             27 (NULL + sqlalchemy)
+         169         504 LOAD_GLOBAL             27 (NULL + sqlalchemy)
                      516 LOAD_ATTR               14 (text)
          
-         177         526 LOAD_CONST               9 ('\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        ')
+         170         526 LOAD_CONST               9 ('\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        ')
          
-         176         528 PRECALL                  1
+         169         528 PRECALL                  1
                      532 CALL                     1
          
-         185         542 LOAD_FAST                0 (event)
+         178         542 LOAD_FAST                0 (event)
                      544 LOAD_ATTR                3 (search_uid)
          
-         186         554 LOAD_FAST                0 (event)
+         179         554 LOAD_FAST                0 (event)
                      556 LOAD_ATTR               15 (actor_key)
          
-         187         566 LOAD_FAST                7 (domain)
+         180         566 LOAD_FAST                7 (domain)
          
-         188         568 LOAD_FAST                0 (event)
+         181         568 LOAD_FAST                0 (event)
                      570 LOAD_ATTR                0 (data)
                      580 LOAD_METHOD              1 (get)
                      602 LOAD_CONST               4 ('stage')
                      604 LOAD_CONST              10 ('create')
                      606 PRECALL                  2
                      610 CALL                     2
          
-         184         620 LOAD_CONST              11 (('search_uid', 'actor_key', 'domain', 'type'))
+         177         620 LOAD_CONST              11 (('search_uid', 'actor_key', 'domain', 'type'))
                      622 BUILD_CONST_KEY_MAP      4
          
-         175         624 PRECALL                  2
+         168         624 PRECALL                  2
                      628 CALL                     2
                      638 STORE_FAST               8 (result)
          
-         192         640 LOAD_FAST                8 (result)
+         185         640 LOAD_FAST                8 (result)
                      642 LOAD_METHOD             16 (scalar_one)
                      664 PRECALL                  0
                      668 CALL                     0
                      678 STORE_FAST               9 (new_event_id)
          
-         193         680 LOAD_FAST                9 (new_event_id)
+         186         680 LOAD_FAST                9 (new_event_id)
                      682 POP_JUMP_FORWARD_IF_NONE    21 (to 726)
          
-         194         684 LOAD_FAST                5 (new_event_ids)
+         187         684 LOAD_FAST                5 (new_event_ids)
                      686 LOAD_METHOD             17 (append)
                      708 LOAD_FAST                9 (new_event_id)
                      710 PRECALL                  1
                      714 CALL                     1
                      724 POP_TOP
          
-         196     >>  726 LOAD_DEREF              12 (stage_dict)
+         189     >>  726 LOAD_DEREF              12 (stage_dict)
                      728 LOAD_METHOD              1 (get)
                      750 LOAD_FAST                7 (domain)
                      752 PRECALL                  1
                      756 CALL                     1
                      766 POP_JUMP_FORWARD_IF_NONE   138 (to 1044)
          
-         197         768 LOAD_GLOBAL             18 (ts)
+         190         768 LOAD_GLOBAL             18 (ts)
                      780 LOAD_ATTR               18 (models)
                      790 LOAD_METHOD             19 (Event)
          
-         198         812 LOAD_FAST                0 (event)
+         191         812 LOAD_FAST                0 (event)
                      814 LOAD_ATTR                3 (search_uid)
          
-         199         824 LOAD_FAST                0 (event)
+         192         824 LOAD_FAST                0 (event)
                      826 LOAD_ATTR               15 (actor_key)
          
-         200         836 LOAD_FAST                7 (domain)
+         193         836 LOAD_FAST                7 (domain)
          
-         201         838 LOAD_CONST              12 ('comment')
+         194         838 LOAD_CONST              12 ('comment')
          
-         203         840 LOAD_CONST              12 ('comment')
+         196         840 LOAD_CONST              12 ('comment')
                      842 PUSH_NULL
                      844 LOAD_FAST                3 (get_stage)
                      846 LOAD_FAST                7 (domain)
                      848 PRECALL                  1
                      852 CALL                     1
                      862 FORMAT_VALUE             0
                      864 LOAD_CONST              13 (' → ')
@@ -1408,34 +1421,34 @@
                      932 LOAD_CONST               4 ('stage')
                      934 PRECALL                  1
                      938 CALL                     1
                      948 BINARY_SUBSCR
                      958 FORMAT_VALUE             0
                      960 BUILD_STRING             3
          
-         202         962 BUILD_MAP                1
+         195         962 BUILD_MAP                1
          
-         197         964 KW_NAMES                14
+         190         964 KW_NAMES                14
                      966 PRECALL                  5
                      970 CALL                     5
                      980 STORE_FAST              10 (comment)
          
-         206         982 LOAD_GLOBAL             18 (ts)
+         199         982 LOAD_GLOBAL             18 (ts)
                      994 LOAD_ATTR               22 (query)
                     1004 LOAD_METHOD             23 (insert_event)
                     1026 LOAD_FAST               10 (comment)
                     1028 PRECALL                  1
                     1032 CALL                     1
                     1042 POP_TOP
                  >> 1044 EXTENDED_ARG             1
                     1046 JUMP_BACKWARD          361 (to 326)
          
-         161     >> 1048 NOP
+         154     >> 1048 NOP
          
-         160        1050 LOAD_CONST               0 (None)
+         153        1050 LOAD_CONST               0 (None)
                     1052 LOAD_CONST               0 (None)
                     1054 LOAD_CONST               0 (None)
                     1056 PRECALL                  2
                     1060 CALL                     2
                     1070 POP_TOP
                     1072 JUMP_FORWARD            11 (to 1096)
                  >> 1074 PUSH_EXC_INFO
@@ -1446,15 +1459,15 @@
                     1084 POP_EXCEPT
                     1086 RERAISE                  1
                  >> 1088 POP_TOP
                     1090 POP_EXCEPT
                     1092 POP_TOP
                     1094 POP_TOP
          
-         159     >> 1096 LOAD_CONST               0 (None)
+         152     >> 1096 LOAD_CONST               0 (None)
                     1098 LOAD_CONST               0 (None)
                     1100 LOAD_CONST               0 (None)
                     1102 PRECALL                  2
                     1106 CALL                     2
                     1116 POP_TOP
                     1118 JUMP_FORWARD            11 (to 1142)
                  >> 1120 PUSH_EXC_INFO
@@ -1465,29 +1478,29 @@
                     1130 POP_EXCEPT
                     1132 RERAISE                  1
                  >> 1134 POP_TOP
                     1136 POP_EXCEPT
                     1138 POP_TOP
                     1140 POP_TOP
          
-         208     >> 1142 LOAD_FAST                5 (new_event_ids)
+         201     >> 1142 LOAD_FAST                5 (new_event_ids)
                     1144 GET_ITER
                  >> 1146 FOR_ITER                23 (to 1194)
                     1148 STORE_FAST              11 (event_id)
          
-         209        1150 LOAD_GLOBAL             19 (NULL + ts)
+         202        1150 LOAD_GLOBAL             19 (NULL + ts)
                     1162 LOAD_ATTR               24 (trigger_process_event)
                     1172 LOAD_FAST               11 (event_id)
                     1174 KW_NAMES                15
                     1176 PRECALL                  1
                     1180 CALL                     1
                     1190 POP_TOP
                     1192 JUMP_BACKWARD           24 (to 1146)
          
-         208     >> 1194 LOAD_CONST               0 (None)
+         201     >> 1194 LOAD_CONST               0 (None)
                     1196 RETURN_VALUE
          ExceptionTable:
            278 to 318 -> 1120 [1] lasti
            320 to 1046 -> 1074 [2] lasti
            1050 to 1072 -> 1120 [1] lasti
            1074 to 1080 -> 1082 [4] lasti
            1082 to 1086 -> 1120 [1] lasti
@@ -1510,25 +1523,25 @@
                   0x950197008902a00000000000000000000000000000000000000000007c
                   006401a6020000ab0200000000000000007d017402000000000000000000
                   006a0200000000000000006a030000000000000000a00000000000000000
                   000000000000000000000000007c016401a6020000ab0200000000000000
                   005300
                              0 COPY_FREE_VARS           1
                
-               152           2 RESUME                   0
+               145           2 RESUME                   0
                
-               153           4 LOAD_DEREF               2 (stage_dict)
+               146           4 LOAD_DEREF               2 (stage_dict)
                              6 LOAD_METHOD              0 (get)
                             28 LOAD_FAST                0 (domain)
                             30 LOAD_CONST               1 ('Unknown')
                             32 PRECALL                  2
                             36 CALL                     2
                             46 STORE_FAST               1 (stage_key)
                
-               154          48 LOAD_GLOBAL              2 (ts)
+               147          48 LOAD_GLOBAL              2 (ts)
                             60 LOAD_ATTR                2 (constants)
                             70 LOAD_ATTR                3 (LABEL_MAP)
                             80 LOAD_METHOD              0 (get)
                            102 LOAD_FAST                1 (stage_key)
                            104 LOAD_CONST               1 ('Unknown')
                            106 PRECALL                  2
                            110 CALL                     2
@@ -1538,15 +1551,15 @@
                   'Unknown'
                names      ('get', 'ts', 'constants', 'LABEL_MAP')
                varnames   ('domain', 'stage_key')
                freevars   ('stage_dict',)
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_stage'
-               firstlineno 152
+               firstlineno 145
                lnotab 0x04012c01
             'domains'
             '\n                        INSERT INTO company (domain, source) \n                        VALUES(:domain, :source)\n                        ON CONFLICT DO NOTHING\n                        '
             ('domain', 'source')
             '\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        '
             'create'
             ('search_uid', 'actor_key', 'domain', 'type')
@@ -1556,25 +1569,24 @@
             ('event_id',)
          names      ('data', 'get', 'search_targets', 'search_uid', 'set_index', 'to_dict', 'db', 'connect', 'begin', 'ts', 'helpers', 'clean_domain', 'execute', 'sqlalchemy', 'text', 'actor_key', 'scalar_one', 'append', 'models', 'Event', 'constants', 'LABEL_MAP', 'query', 'insert_event', 'trigger_process_event')
          varnames   ('event', 'source', 'targets', 'get_stage', 'domains', 'new_event_ids', 'con', 'domain', 'result', 'new_event_id', 'comment', 'event_id')
          freevars   ()
          cellvars   ('stage_dict',)
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'important_targets_from_event'
-         firstlineno 146
+         firstlineno 139
          lnotab
             0x040234012a015a020a041a02040134012a010a023e011801160102ff0e
             0708f8100b1801160102ff0e090c010c01020134fc04f71011280104012a
             022a012c010c010c01020102027aff02fb120942d302ff2eff2e3108012c
             ff
       True
       'create'
       'companies'
       'search_uid'
-      'actor_key'
       'force'
       'source'
       'stage'
       code
          argcount  : 6
          nlocals   : 18
          stacksize : 13
@@ -1624,253 +1636,253 @@
             0278035900770101005900010001007401000000000000000000007c0ba6
             010000ab01000000000000000001007c0b44005d177d1174230000000000
             00000000006a1200000000000000007c11ac12a6010000ab010000000000
             00000001008c1874010000000000000000000064137c089b0064147c099b
             006415740900000000000000000000a6000000ab0000000000000000007c
             0a7a0a00009b0064169d07a6010000ab0100000000000000000100640053
             00
-         218           0 RESUME                   0
+         211           0 RESUME                   0
          
-         226           2 LOAD_GLOBAL              1 (NULL + print)
+         219           2 LOAD_GLOBAL              1 (NULL + print)
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
          
-         228          66 LOAD_GLOBAL              5 (NULL + search_targets)
+         221          66 LOAD_GLOBAL              5 (NULL + search_targets)
                       78 LOAD_FAST                1 (search_uid)
                       80 KW_NAMES                 3
                       82 PRECALL                  1
                       86 CALL                     1
                       96 STORE_FAST               6 (targets)
          
-         230          98 LOAD_FAST                3 (force)
+         223          98 LOAD_FAST                3 (force)
                      100 POP_JUMP_FORWARD_IF_FALSE    45 (to 192)
          
-         233         102 LOAD_FAST                6 (targets)
+         226         102 LOAD_FAST                6 (targets)
                      104 LOAD_FAST                6 (targets)
                      106 LOAD_CONST               4 ('stage')
                      108 BINARY_SUBSCR
                      118 LOAD_CONST               5 ('reject')
                      120 COMPARE_OP               3 (!=)
                      126 BINARY_SUBSCR
                      136 STORE_FAST               6 (targets)
          
-         234         138 LOAD_FAST                6 (targets)
+         227         138 LOAD_FAST                6 (targets)
                      140 LOAD_CONST               6 ('domain')
                      142 BINARY_SUBSCR
                      152 LOAD_METHOD              3 (tolist)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 STORE_FAST               7 (protected_domains)
                      190 JUMP_FORWARD            26 (to 244)
          
-         236     >>  192 LOAD_FAST                6 (targets)
+         229     >>  192 LOAD_FAST                6 (targets)
                      194 LOAD_CONST               6 ('domain')
                      196 BINARY_SUBSCR
                      206 LOAD_METHOD              3 (tolist)
                      228 PRECALL                  0
                      232 CALL                     0
                      242 STORE_FAST               7 (protected_domains)
          
-         240     >>  244 LOAD_CONST               7 (0)
+         233     >>  244 LOAD_CONST               7 (0)
                      246 STORE_FAST               8 (inserted)
          
-         241         248 LOAD_CONST               7 (0)
+         234         248 LOAD_CONST               7 (0)
                      250 STORE_FAST               9 (skipped)
          
-         242         252 LOAD_GLOBAL              9 (NULL + time)
+         235         252 LOAD_GLOBAL              9 (NULL + time)
                      264 PRECALL                  0
                      268 CALL                     0
                      278 STORE_FAST              10 (start)
          
-         244         280 BUILD_LIST               0
+         237         280 BUILD_LIST               0
                      282 STORE_FAST              11 (new_event_ids)
          
-         245         284 LOAD_GLOBAL             10 (db)
+         238         284 LOAD_GLOBAL             10 (db)
                      296 LOAD_METHOD              6 (connect)
                      318 PRECALL                  0
                      322 CALL                     0
                      332 BEFORE_WITH
                      334 STORE_FAST              12 (con)
          
-         246         336 LOAD_FAST               12 (con)
+         239         336 LOAD_FAST               12 (con)
                      338 LOAD_METHOD              7 (begin)
                      360 PRECALL                  0
                      364 CALL                     0
                      374 BEFORE_WITH
                      376 POP_TOP
          
-         247         378 LOAD_FAST                0 (companies)
+         240         378 LOAD_FAST                0 (companies)
                      380 GET_ITER
                  >>  382 EXTENDED_ARG             1
                      384 FOR_ITER               382 (to 1150)
                      386 STORE_FAST              13 (company)
          
-         248         388 LOAD_GLOBAL              1 (NULL + print)
+         241         388 LOAD_GLOBAL              1 (NULL + print)
                      400 LOAD_FAST               13 (company)
                      402 PRECALL                  1
                      406 CALL                     1
                      416 POP_TOP
          
-         249         418 LOAD_GLOBAL             17 (NULL + helpers)
+         242         418 LOAD_GLOBAL             17 (NULL + helpers)
                      430 LOAD_ATTR                9 (domain_is_none)
                      440 LOAD_FAST               13 (company)
                      442 LOAD_METHOD             10 (get)
                      464 LOAD_CONST               6 ('domain')
                      466 PRECALL                  1
                      470 CALL                     1
                      480 PRECALL                  1
                      484 CALL                     1
                      494 POP_JUMP_FORWARD_IF_FALSE    20 (to 536)
          
-         250         496 LOAD_GLOBAL              1 (NULL + print)
+         243         496 LOAD_GLOBAL              1 (NULL + print)
                      508 LOAD_CONST               8 ('Missing domain: ')
                      510 LOAD_FAST               13 (company)
                      512 FORMAT_VALUE             0
                      514 LOAD_CONST               9 ('. Skipping')
                      516 BUILD_STRING             3
                      518 PRECALL                  1
                      522 CALL                     1
                      532 POP_TOP
          
-         251         534 JUMP_BACKWARD           77 (to 382)
+         244         534 JUMP_BACKWARD           77 (to 382)
          
-         253     >>  536 LOAD_FAST               13 (company)
+         246     >>  536 LOAD_FAST               13 (company)
                      538 LOAD_CONST               6 ('domain')
                      540 BINARY_SUBSCR
                      550 LOAD_FAST                7 (protected_domains)
                      552 CONTAINS_OP              0
                      554 POP_JUMP_FORWARD_IF_FALSE     6 (to 568)
          
-         255         556 LOAD_FAST                9 (skipped)
+         248         556 LOAD_FAST                9 (skipped)
                      558 LOAD_CONST              10 (1)
                      560 BINARY_OP               13 (+=)
                      564 STORE_FAST               9 (skipped)
          
-         256         566 JUMP_BACKWARD           93 (to 382)
+         249         566 JUMP_BACKWARD           93 (to 382)
          
-         258     >>  568 LOAD_FAST                8 (inserted)
+         251     >>  568 LOAD_FAST                8 (inserted)
                      570 LOAD_CONST              10 (1)
                      572 BINARY_OP               13 (+=)
                      576 STORE_FAST               8 (inserted)
          
-         261         578 LOAD_FAST               12 (con)
+         254         578 LOAD_FAST               12 (con)
                      580 LOAD_METHOD             11 (execute)
          
-         262         602 LOAD_GLOBAL             25 (NULL + sqlalchemy)
+         255         602 LOAD_GLOBAL             25 (NULL + sqlalchemy)
                      614 LOAD_ATTR               13 (text)
          
-         263         624 LOAD_CONST              11 ('\n                        INSERT INTO company (domain, name, description, source) \n                        VALUES(:domain, :name, :description, :source)\n                        ON CONFLICT DO NOTHING\n                        ')
+         256         624 LOAD_CONST              11 ('\n                        INSERT INTO company (domain, name, description, source) \n                        VALUES(:domain, :name, :description, :source)\n                        ON CONFLICT DO NOTHING\n                        ')
          
-         262         626 PRECALL                  1
+         255         626 PRECALL                  1
                      630 CALL                     1
          
-         270         640 LOAD_FAST               13 (company)
+         263         640 LOAD_FAST               13 (company)
                      642 LOAD_METHOD             10 (get)
                      664 LOAD_CONST               6 ('domain')
                      666 PRECALL                  1
                      670 CALL                     1
          
-         271         680 LOAD_FAST               13 (company)
+         264         680 LOAD_FAST               13 (company)
                      682 LOAD_METHOD             10 (get)
                      704 LOAD_CONST              12 ('name')
                      706 PRECALL                  1
                      710 CALL                     1
          
-         272         720 LOAD_FAST               13 (company)
+         265         720 LOAD_FAST               13 (company)
                      722 LOAD_METHOD             10 (get)
                      744 LOAD_CONST              13 ('description')
                      746 PRECALL                  1
                      750 CALL                     1
          
-         273         760 LOAD_FAST               13 (company)
+         266         760 LOAD_FAST               13 (company)
                      762 LOAD_METHOD             10 (get)
                      784 LOAD_CONST              14 ('source')
                      786 LOAD_FAST                4 (source)
                      788 PRECALL                  2
                      792 CALL                     2
          
-         269         802 LOAD_CONST              15 (('domain', 'name', 'description', 'source'))
+         262         802 LOAD_CONST              15 (('domain', 'name', 'description', 'source'))
                      804 BUILD_CONST_KEY_MAP      4
          
-         261         806 PRECALL                  2
+         254         806 PRECALL                  2
                      810 CALL                     2
                      820 POP_TOP
          
-         277         822 LOAD_FAST               12 (con)
+         270         822 LOAD_FAST               12 (con)
                      824 LOAD_METHOD             11 (execute)
          
-         278         846 LOAD_GLOBAL             25 (NULL + sqlalchemy)
+         271         846 LOAD_GLOBAL             25 (NULL + sqlalchemy)
                      858 LOAD_ATTR               13 (text)
          
-         279         868 LOAD_CONST              16 ('\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        ')
+         272         868 LOAD_CONST              16 ('\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        ')
          
-         278         870 PRECALL                  1
+         271         870 PRECALL                  1
                      874 CALL                     1
          
-         287         884 LOAD_FAST                1 (search_uid)
+         280         884 LOAD_FAST                1 (search_uid)
          
-         288         886 LOAD_FAST                2 (actor_key)
+         281         886 LOAD_FAST                2 (actor_key)
          
-         289         888 LOAD_FAST               13 (company)
+         282         888 LOAD_FAST               13 (company)
                      890 LOAD_METHOD             10 (get)
                      912 LOAD_CONST               6 ('domain')
                      914 PRECALL                  1
                      918 CALL                     1
          
-         290         928 LOAD_FAST                5 (stage)
+         283         928 LOAD_FAST                5 (stage)
          
-         286         930 LOAD_CONST              17 (('search_uid', 'actor_key', 'domain', 'type'))
+         279         930 LOAD_CONST              17 (('search_uid', 'actor_key', 'domain', 'type'))
                      932 BUILD_CONST_KEY_MAP      4
          
-         277         934 PRECALL                  2
+         270         934 PRECALL                  2
                      938 CALL                     2
                      948 STORE_FAST              14 (result)
          
-         297         950 LOAD_GLOBAL              1 (NULL + print)
+         290         950 LOAD_GLOBAL              1 (NULL + print)
                      962 LOAD_FAST               14 (result)
                      964 PRECALL                  1
                      968 CALL                     1
                      978 POP_TOP
          
-         298         980 NOP
+         291         980 NOP
          
-         299         982 LOAD_FAST               14 (result)
+         292         982 LOAD_FAST               14 (result)
                      984 LOAD_METHOD             14 (scalar_one)
                     1006 PRECALL                  0
                     1010 CALL                     0
                     1020 STORE_FAST              15 (new_event_id)
          
-         300        1022 LOAD_FAST               15 (new_event_id)
+         293        1022 LOAD_FAST               15 (new_event_id)
                     1024 POP_JUMP_FORWARD_IF_NONE    21 (to 1068)
          
-         301        1026 LOAD_FAST               11 (new_event_ids)
+         294        1026 LOAD_FAST               11 (new_event_ids)
                     1028 LOAD_METHOD             15 (append)
                     1050 LOAD_FAST               15 (new_event_id)
                     1052 PRECALL                  1
                     1056 CALL                     1
                     1066 POP_TOP
                  >> 1068 EXTENDED_ARG             1
                     1070 JUMP_BACKWARD          345 (to 382)
                  >> 1072 PUSH_EXC_INFO
          
-         302        1074 LOAD_GLOBAL             32 (Exception)
+         295        1074 LOAD_GLOBAL             32 (Exception)
                     1086 CHECK_EXC_MATCH
                     1088 POP_JUMP_FORWARD_IF_FALSE    26 (to 1142)
                     1090 STORE_FAST              16 (e)
          
-         303        1092 LOAD_GLOBAL              1 (NULL + print)
+         296        1092 LOAD_GLOBAL              1 (NULL + print)
                     1104 LOAD_FAST               16 (e)
                     1106 PRECALL                  1
                     1110 CALL                     1
                     1120 POP_TOP
                     1122 POP_EXCEPT
                     1124 LOAD_CONST               0 (None)
                     1126 STORE_FAST              16 (e)
@@ -1878,22 +1890,22 @@
                     1130 EXTENDED_ARG             1
                     1132 JUMP_BACKWARD          376 (to 382)
                  >> 1134 LOAD_CONST               0 (None)
                     1136 STORE_FAST              16 (e)
                     1138 DELETE_FAST             16 (e)
                     1140 RERAISE                  1
          
-         302     >> 1142 RERAISE                  0
+         295     >> 1142 RERAISE                  0
                  >> 1144 COPY                     3
                     1146 POP_EXCEPT
                     1148 RERAISE                  1
          
-         247     >> 1150 NOP
+         240     >> 1150 NOP
          
-         246        1152 LOAD_CONST               0 (None)
+         239        1152 LOAD_CONST               0 (None)
                     1154 LOAD_CONST               0 (None)
                     1156 LOAD_CONST               0 (None)
                     1158 PRECALL                  2
                     1162 CALL                     2
                     1172 POP_TOP
                     1174 JUMP_FORWARD            11 (to 1198)
                  >> 1176 PUSH_EXC_INFO
@@ -1904,15 +1916,15 @@
                     1186 POP_EXCEPT
                     1188 RERAISE                  1
                  >> 1190 POP_TOP
                     1192 POP_EXCEPT
                     1194 POP_TOP
                     1196 POP_TOP
          
-         245     >> 1198 LOAD_CONST               0 (None)
+         238     >> 1198 LOAD_CONST               0 (None)
                     1200 LOAD_CONST               0 (None)
                     1202 LOAD_CONST               0 (None)
                     1204 PRECALL                  2
                     1208 CALL                     2
                     1218 POP_TOP
                     1220 JUMP_FORWARD            11 (to 1244)
                  >> 1222 PUSH_EXC_INFO
@@ -1923,35 +1935,35 @@
                     1232 POP_EXCEPT
                     1234 RERAISE                  1
                  >> 1236 POP_TOP
                     1238 POP_EXCEPT
                     1240 POP_TOP
                     1242 POP_TOP
          
-         305     >> 1244 LOAD_GLOBAL              1 (NULL + print)
+         298     >> 1244 LOAD_GLOBAL              1 (NULL + print)
                     1256 LOAD_FAST               11 (new_event_ids)
                     1258 PRECALL                  1
                     1262 CALL                     1
                     1272 POP_TOP
          
-         306        1274 LOAD_FAST               11 (new_event_ids)
+         299        1274 LOAD_FAST               11 (new_event_ids)
                     1276 GET_ITER
                  >> 1278 FOR_ITER                23 (to 1326)
                     1280 STORE_FAST              17 (event_id)
          
-         307        1282 LOAD_GLOBAL             35 (NULL + ts)
+         300        1282 LOAD_GLOBAL             35 (NULL + ts)
                     1294 LOAD_ATTR               18 (trigger_process_event)
                     1304 LOAD_FAST               17 (event_id)
                     1306 KW_NAMES                18
                     1308 PRECALL                  1
                     1312 CALL                     1
                     1322 POP_TOP
                     1324 JUMP_BACKWARD           24 (to 1278)
          
-         308     >> 1326 LOAD_GLOBAL              1 (NULL + print)
+         301     >> 1326 LOAD_GLOBAL              1 (NULL + print)
                     1338 LOAD_CONST              19 ('Inserted ')
                     1340 LOAD_FAST                8 (inserted)
                     1342 FORMAT_VALUE             0
                     1344 LOAD_CONST              20 ('. Skipped ')
                     1346 LOAD_FAST                9 (skipped)
                     1348 FORMAT_VALUE             0
                     1350 LOAD_CONST              21 ('. Took ')
@@ -2011,15 +2023,15 @@
             ' seconds'
          names      ('print', 'len', 'search_targets', 'tolist', 'time', 'db', 'connect', 'begin', 'helpers', 'domain_is_none', 'get', 'execute', 'sqlalchemy', 'text', 'scalar_one', 'append', 'Exception', 'ts', 'trigger_process_event')
          varnames   ('companies', 'search_uid', 'actor_key', 'force', 'source', 'stage', 'targets', 'protected_domains', 'inserted', 'skipped', 'start', 'new_event_ids', 'con', 'company', 'result', 'new_event_id', 'e', 'event_id')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_companies_as_targets'
-         firstlineno 218
+         firstlineno 211
          lnotab
             0x0208400220020403240136023404040104011c02040134012a010a011e
             014e012601020214020a0102020a031801160102ff0e082801280128012a
             fc04f810101801160102ff0e0902010201280102fc04f710141e01020128
             0104013001120132ff08c902ff2eff2e3c1e0108012c01
       code
          argcount  : 0
@@ -2039,53 +2051,53 @@
             00000001006e0b230031007304770278035900770101005900010001007c
             036403190000000000000000006a090000000000000000a00a0000000000
             0000000000000000000000000000006404a6010000ab0100000000000000
             006a0900000000000000006405190000000000000000007c0364063c0000
             007c03640719000000000000000000a00b00000000000000000000000000
             0000000000000064088400a6010000ab0100000000000000007c0364093c
             0000007c035300
-         315           0 RESUME                   0
+         308           0 RESUME                   0
          
-         316           2 LOAD_CONST               1 ("\n    SELECT \n        s.uid,\n        s.label,\n        s.updated,\n        s.meta->>'type' as type,\n        s.meta->>'notes' as notes,\n        s.meta->>'products' as products,\n        s.meta->>'services' as services,\n        s.meta->>'customers' as customers,\n        s.meta->>'end_customer' as end_customer,\n        s.meta->>'last_list' as last_list,\n        s.meta->>'next_due_date' as next_due_date,\n        s.meta->>'geographies' as geographies,\n        s.meta->>'week' as week,\n        s.meta->>'day' as day,\n\n        COALESCE(s.meta->>'search_status', 'active') as search_status\n    FROM search s\n    ORDER BY updated\n    ")
+         309           2 LOAD_CONST               1 ("\n    SELECT \n        s.uid,\n        s.label,\n        s.updated,\n        s.meta->>'type' as type,\n        s.meta->>'notes' as notes,\n        s.meta->>'products' as products,\n        s.meta->>'services' as services,\n        s.meta->>'customers' as customers,\n        s.meta->>'end_customer' as end_customer,\n        s.meta->>'last_list' as last_list,\n        s.meta->>'next_due_date' as next_due_date,\n        s.meta->>'geographies' as geographies,\n        s.meta->>'week' as week,\n        s.meta->>'day' as day,\n\n        COALESCE(s.meta->>'search_status', 'active') as search_status\n    FROM search s\n    ORDER BY updated\n    ")
                        4 STORE_FAST               0 (statement)
          
-         337           6 LOAD_GLOBAL              0 (db)
+         330           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               1 (conn)
          
-         338          58 LOAD_FAST                1 (conn)
+         331          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                0 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         339         136 LOAD_GLOBAL             11 (NULL + pd)
+         332         136 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         337         252 LOAD_CONST               0 (None)
+         330         252 LOAD_CONST               0 (None)
                      254 LOAD_CONST               0 (None)
                      256 LOAD_CONST               0 (None)
                      258 PRECALL                  2
                      262 CALL                     2
                      272 POP_TOP
                      274 JUMP_FORWARD            11 (to 298)
                  >>  276 PUSH_EXC_INFO
@@ -2096,44 +2108,44 @@
                      286 POP_EXCEPT
                      288 RERAISE                  1
                  >>  290 POP_TOP
                      292 POP_EXCEPT
                      294 POP_TOP
                      296 POP_TOP
          
-         340     >>  298 LOAD_FAST                3 (df)
+         333     >>  298 LOAD_FAST                3 (df)
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
          
-         341         390 LOAD_FAST                3 (df)
+         334         390 LOAD_FAST                3 (df)
                      392 LOAD_CONST               7 ('uid')
                      394 BINARY_SUBSCR
                      404 LOAD_METHOD             11 (apply)
          
-         342         426 LOAD_CONST               8 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 342>)
+         335         426 LOAD_CONST               8 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 335>)
                      428 MAKE_FUNCTION            0
          
-         341         430 PRECALL                  1
+         334         430 PRECALL                  1
                      434 CALL                     1
                      444 LOAD_FAST                3 (df)
                      446 LOAD_CONST               9 ('searchToken')
                      448 STORE_SUBSCR
          
-         344         452 LOAD_FAST                3 (df)
+         337         452 LOAD_FAST                3 (df)
                      454 RETURN_VALUE
          ExceptionTable:
            56 to 250 -> 276 [1] lasti
            276 to 282 -> 284 [3] lasti
            290 to 290 -> 284 [3] lasti
          consts
             None
@@ -2151,15 +2163,15 @@
                flags     : 19
                code
                   0x97007401000000000000000000006a0100000000000000007405000000
                   000000000000007c00a6010000ab010000000000000000a0030000000000
                   0000000000000000000000000000006401a6010000ab0100000000000000
                   00a6010000ab010000000000000000a00400000000000000000000000000
                   00000000000000a6000000ab0000000000000000005300
-               342           0 RESUME                   0
+               335           0 RESUME                   0
                              2 LOAD_GLOBAL              1 (NULL + hashlib)
                             14 LOAD_ATTR                1 (md5)
                             24 LOAD_GLOBAL              5 (NULL + str)
                             36 LOAD_FAST                0 (x)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              3 (encode)
@@ -2177,39 +2189,39 @@
                   'utf-8'
                names      ('hashlib', 'md5', 'str', 'encode', 'hexdigest')
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '<lambda>'
-               firstlineno 342
+               firstlineno 335
                lnotab 0x
             'searchToken'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'str', 'split', 'apply')
          varnames   ('statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'searches_query'
-         firstlineno 315
+         firstlineno 308
          lnotab 0x0201041534014e0174fe2e035c01240104ff1603
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x970064017d007401000000000000000000006a0100000000000000007c
             00740400000000000000000000a6020000ab0200000000000000005300
-         347           0 RESUME                   0
+         340           0 RESUME                   0
          
-         348           2 LOAD_CONST               1 ('\n       SELECT\n        search_uid,\n        AVG(rating::int) AS rating_avg,\n        COUNT(rating) as rating_count\n    FROM rating \n    GROUP BY search_uid\n    ')
+         341           2 LOAD_CONST               1 ('\n       SELECT\n        search_uid,\n        AVG(rating::int) AS rating_avg,\n        COUNT(rating) as rating_count\n    FROM rating \n    GROUP BY search_uid\n    ')
                        4 STORE_FAST               0 (query)
          
-         356           6 LOAD_GLOBAL              1 (NULL + pd)
+         349           6 LOAD_GLOBAL              1 (NULL + pd)
                       18 LOAD_ATTR                1 (read_sql)
                       28 LOAD_FAST                0 (query)
                       30 LOAD_GLOBAL              4 (db)
                       42 PRECALL                  2
                       46 CALL                     2
                       56 RETURN_VALUE
          consts
@@ -2217,15 +2229,15 @@
             '\n       SELECT\n        search_uid,\n        AVG(rating::int) AS rating_avg,\n        COUNT(rating) as rating_count\n    FROM rating \n    GROUP BY search_uid\n    '
          names      ('pd', 'read_sql', 'db')
          varnames   ('query',)
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'average_rating_per_search_query'
-         firstlineno 347
+         firstlineno 340
          lnotab 0x02010408
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -2237,66 +2249,66 @@
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d037413000000000000000000007c03640319
             00000000000000000064047a0b00006405a6020000ab0200000000000000
             007c0364063c000000640064006400a6020000ab02000000000000000001
             006e0b230031007304770278035900770101005900010001007c035300
-         359           0 RESUME                   0
+         352           0 RESUME                   0
          
-         360           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT\n            e.search_uid,\n            a.name as analyst,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 1 * 86400 THEN 1 ELSE 0 END) AS last_1_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 7 * 86400 THEN 1 ELSE 0 END) AS last_7_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400 THEN 1 ELSE 0 END) AS last_30_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) AS last_90_days,\n            SUM(CASE WHEN e.type = 'validate' THEN 1 ELSE 0 END) AS total_validations,\n            RANK() OVER (PARTITION BY e.search_uid ORDER BY SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) DESC) as rank\n        FROM\n            event e\n        LEFT JOIN\n            actor a ON a.key = e.actor_key\n        WHERE\n            e.type = 'validate'\n        GROUP BY\n            e.search_uid, analyst\n    )\n    SELECT\n        search_uid,\n        analyst,\n        last_1_days,\n        last_7_days,\n        last_30_days,\n        last_90_days,\n        total_validations\n    FROM\n        RankedEvents\n    WHERE\n        rank = 1\n        AND last_90_days > 0\n    ;\n    ")
+         353           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT\n            e.search_uid,\n            a.name as analyst,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 1 * 86400 THEN 1 ELSE 0 END) AS last_1_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 7 * 86400 THEN 1 ELSE 0 END) AS last_7_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400 THEN 1 ELSE 0 END) AS last_30_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) AS last_90_days,\n            SUM(CASE WHEN e.type = 'validate' THEN 1 ELSE 0 END) AS total_validations,\n            RANK() OVER (PARTITION BY e.search_uid ORDER BY SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) DESC) as rank\n        FROM\n            event e\n        LEFT JOIN\n            actor a ON a.key = e.actor_key\n        WHERE\n            e.type = 'validate'\n        GROUP BY\n            e.search_uid, analyst\n    )\n    SELECT\n        search_uid,\n        analyst,\n        last_1_days,\n        last_7_days,\n        last_30_days,\n        last_90_days,\n        total_validations\n    FROM\n        RankedEvents\n    WHERE\n        rank = 1\n        AND last_90_days > 0\n    ;\n    ")
                        4 STORE_FAST               0 (stmt)
          
-         395           6 LOAD_GLOBAL              0 (db)
+         388           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               1 (conn)
          
-         396          58 LOAD_FAST                1 (conn)
+         389          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                0 (stmt)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         397         136 LOAD_GLOBAL             11 (NULL + pd)
+         390         136 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         398         252 LOAD_GLOBAL             19 (NULL + round)
+         391         252 LOAD_GLOBAL             19 (NULL + round)
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
          
-         395         308 LOAD_CONST               0 (None)
+         388         308 LOAD_CONST               0 (None)
                      310 LOAD_CONST               0 (None)
                      312 LOAD_CONST               0 (None)
                      314 PRECALL                  2
                      318 CALL                     2
                      328 POP_TOP
                      330 JUMP_FORWARD            11 (to 354)
                  >>  332 PUSH_EXC_INFO
@@ -2307,15 +2319,15 @@
                      342 POP_EXCEPT
                      344 RERAISE                  1
                  >>  346 POP_TOP
                      348 POP_EXCEPT
                      350 POP_TOP
                      352 POP_TOP
          
-         399     >>  354 LOAD_FAST                3 (df)
+         392     >>  354 LOAD_FAST                3 (df)
                      356 RETURN_VALUE
          ExceptionTable:
            56 to 306 -> 332 [1] lasti
            332 to 338 -> 340 [3] lasti
            346 to 346 -> 340 [3] lasti
          consts
             None
@@ -2327,15 +2339,15 @@
             'total_validations_pct'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'round')
          varnames   ('stmt', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'validation_history'
-         firstlineno 359
+         firstlineno 352
          lnotab 0x0201042334014e01740138fd2e04
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -2346,53 +2358,53 @@
             00a6010000ab0100000000000000007d02740b000000000000000000006a
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d03640064006400a6020000ab020000000000
             00000001006e0b230031007304770278035900770101005900010001007c
             035300
-         402           0 RESUME                   0
+         395           0 RESUME                   0
          
-         403           2 LOAD_CONST               1 ("\n        SELECT \n            e.search_uid as uid,\n            COUNT(*) as comment_count\n        FROM event e\n        WHERE \n            e.type = 'comment'\n            AND e.domain is null\n            -- last 30 days\n            AND e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400\n        GROUP BY e.search_uid\n        ")
+         396           2 LOAD_CONST               1 ("\n        SELECT \n            e.search_uid as uid,\n            COUNT(*) as comment_count\n        FROM event e\n        WHERE \n            e.type = 'comment'\n            AND e.domain is null\n            -- last 30 days\n            AND e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400\n        GROUP BY e.search_uid\n        ")
                        4 STORE_FAST               0 (statement)
          
-         415           6 LOAD_GLOBAL              0 (db)
+         408           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               1 (conn)
          
-         416          58 LOAD_FAST                1 (conn)
+         409          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                0 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         417         136 LOAD_GLOBAL             11 (NULL + pd)
+         410         136 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         415         252 LOAD_CONST               0 (None)
+         408         252 LOAD_CONST               0 (None)
                      254 LOAD_CONST               0 (None)
                      256 LOAD_CONST               0 (None)
                      258 PRECALL                  2
                      262 CALL                     2
                      272 POP_TOP
                      274 JUMP_FORWARD            11 (to 298)
                  >>  276 PUSH_EXC_INFO
@@ -2403,15 +2415,15 @@
                      286 POP_EXCEPT
                      288 RERAISE                  1
                  >>  290 POP_TOP
                      292 POP_EXCEPT
                      294 POP_TOP
                      296 POP_TOP
          
-         419     >>  298 LOAD_FAST                3 (df)
+         412     >>  298 LOAD_FAST                3 (df)
                      300 RETURN_VALUE
          ExceptionTable:
            56 to 250 -> 276 [1] lasti
            276 to 282 -> 284 [3] lasti
            290 to 290 -> 284 [3] lasti
          consts
             None
@@ -2419,15 +2431,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'searches_comment_counts'
-         firstlineno 402
+         firstlineno 395
          lnotab 0x0201040c34014e0174fe2e04
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
@@ -2444,107 +2456,107 @@
             000000a00300000000000000000000000000000000000000006406a60100
             00ab0100000000000000007c0264093c0000007c02a00200000000000000
             00000000000000000000000000740900000000000000000000a6000000ab
             00000000000000000064016403ac0aa6030000ab0300000000000000007d
             027c02640b19000000000000000000a00300000000000000000000000000
             000000000000006406a6010000ab0100000000000000007c02640b3c0000
             007c025300
-         422           0 RESUME                   0
+         415           0 RESUME                   0
          
-         423           2 LOAD_GLOBAL              1 (NULL + searches_query)
+         416           2 LOAD_GLOBAL              1 (NULL + searches_query)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               0 (searches)
          
-         425          30 LOAD_GLOBAL              3 (NULL + validation_history)
+         418          30 LOAD_GLOBAL              3 (NULL + validation_history)
                       42 PRECALL                  0
                       46 CALL                     0
                       56 STORE_FAST               1 (recent_event_count)
          
-         427          58 LOAD_FAST                0 (searches)
+         420          58 LOAD_FAST                0 (searches)
                       60 LOAD_METHOD              2 (merge)
          
-         428          82 LOAD_FAST                1 (recent_event_count)
+         421          82 LOAD_FAST                1 (recent_event_count)
                       84 LOAD_CONST               1 ('uid')
                       86 LOAD_CONST               2 ('search_uid')
                       88 LOAD_CONST               3 ('left')
          
-         427          90 KW_NAMES                 4
+         420          90 KW_NAMES                 4
                       92 PRECALL                  4
                       96 CALL                     4
                      106 STORE_FAST               2 (df)
          
-         431         108 LOAD_FAST                2 (df)
+         424         108 LOAD_FAST                2 (df)
                      110 LOAD_CONST               5 ('last_1_days')
                      112 BINARY_SUBSCR
                      122 LOAD_METHOD              3 (fillna)
                      144 LOAD_CONST               6 (0)
                      146 PRECALL                  1
                      150 CALL                     1
                      160 LOAD_FAST                2 (df)
                      162 LOAD_CONST               5 ('last_1_days')
                      164 STORE_SUBSCR
          
-         432         168 LOAD_FAST                2 (df)
+         425         168 LOAD_FAST                2 (df)
                      170 LOAD_CONST               7 ('last_7_days')
                      172 BINARY_SUBSCR
                      182 LOAD_METHOD              3 (fillna)
                      204 LOAD_CONST               6 (0)
                      206 PRECALL                  1
                      210 CALL                     1
                      220 LOAD_FAST                2 (df)
                      222 LOAD_CONST               7 ('last_7_days')
                      224 STORE_SUBSCR
          
-         433         228 LOAD_FAST                2 (df)
+         426         228 LOAD_FAST                2 (df)
                      230 LOAD_CONST               8 ('last_30_days')
                      232 BINARY_SUBSCR
                      242 LOAD_METHOD              3 (fillna)
                      264 LOAD_CONST               6 (0)
                      266 PRECALL                  1
                      270 CALL                     1
                      280 LOAD_FAST                2 (df)
                      282 LOAD_CONST               8 ('last_30_days')
                      284 STORE_SUBSCR
          
-         434         288 LOAD_FAST                2 (df)
+         427         288 LOAD_FAST                2 (df)
                      290 LOAD_CONST               9 ('last_90_days')
                      292 BINARY_SUBSCR
                      302 LOAD_METHOD              3 (fillna)
                      324 LOAD_CONST               6 (0)
                      326 PRECALL                  1
                      330 CALL                     1
                      340 LOAD_FAST                2 (df)
                      342 LOAD_CONST               9 ('last_90_days')
                      344 STORE_SUBSCR
          
-         436         348 LOAD_FAST                2 (df)
+         429         348 LOAD_FAST                2 (df)
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
          
-         437         420 LOAD_FAST                2 (df)
+         430         420 LOAD_FAST                2 (df)
                      422 LOAD_CONST              11 ('comment_count')
                      424 BINARY_SUBSCR
                      434 LOAD_METHOD              3 (fillna)
                      456 LOAD_CONST               6 (0)
                      458 PRECALL                  1
                      462 CALL                     1
                      472 LOAD_FAST                2 (df)
                      474 LOAD_CONST              11 ('comment_count')
                      476 STORE_SUBSCR
          
-         439         480 LOAD_FAST                2 (df)
+         432         480 LOAD_FAST                2 (df)
                      482 RETURN_VALUE
          consts
             None
             'uid'
             'search_uid'
             'left'
             ('left_on', 'right_on', 'how')
@@ -2557,15 +2569,15 @@
             'comment_count'
          names      ('searches_query', 'validation_history', 'merge', 'fillna', 'searches_comment_counts')
          varnames   ('searches', 'recent_event_count', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'enriched_searches_query'
-         firstlineno 422
+         firstlineno 415
          lnotab 0x02011c021c02180108ff12043c013c013c013c0248013c02
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
@@ -2577,66 +2589,66 @@
             00000000007c01a0070000000000000000000000000000000000000000a6
             000000ab0000000000000000007c01a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000ac02a6020000ab0200
             000000000000007d027c02a0090000000000000000000000000000000000
             00000067006403a201ac02a6010000ab0100000000000000007d027c0263
             02640064006400a6020000ab020000000000000000010053002300310073
             047702780359007701010059000100010064005300
-         442           0 RESUME                   0
+         435           0 RESUME                   0
          
-         443           2 LOAD_GLOBAL              0 (db)
+         436           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         444          54 LOAD_FAST                0 (conn)
+         437          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         445          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         438          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         446         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
+         439         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
          
-         445         102 PRECALL                  1
+         438         102 PRECALL                  1
                      106 CALL                     1
          
-         444         116 PRECALL                  1
+         437         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         451         132 LOAD_GLOBAL             11 (NULL + pd)
+         444         132 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         452         248 LOAD_FAST                2 (df)
+         445         248 LOAD_FAST                2 (df)
                      250 LOAD_METHOD              9 (drop)
                      272 BUILD_LIST               0
                      274 LOAD_CONST               3 (('id', 'created', 'updated'))
                      276 LIST_EXTEND              1
                      278 KW_NAMES                 2
                      280 PRECALL                  1
                      284 CALL                     1
                      294 STORE_FAST               2 (df)
          
-         453         296 LOAD_FAST                2 (df)
+         446         296 LOAD_FAST                2 (df)
          
-         443         298 SWAP                     2
+         436         298 SWAP                     2
                      300 LOAD_CONST               0 (None)
                      302 LOAD_CONST               0 (None)
                      304 LOAD_CONST               0 (None)
                      306 PRECALL                  2
                      310 CALL                     2
                      320 POP_TOP
                      322 RETURN_VALUE
@@ -2664,15 +2676,15 @@
             ('id', 'created', 'updated')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'drop')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'actor'
-         firstlineno 442
+         firstlineno 435
          lnotab 0x020134011801160102ff0eff10077401300102f6
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -2685,54 +2697,54 @@
             000000ab0000000000000000007c01a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000ac02a6020000ab0200
             000000000000007d02640064006400a6020000ab02000000000000000001
             006e0b23003100730477027803590077010100590001000100640384007d
             037c02640419000000000000000000a00900000000000000000000000000
             000000000000007c03a6010000ab0100000000000000007c0264053c0000
             007c025300
-         456           0 RESUME                   0
+         449           0 RESUME                   0
          
-         457           2 LOAD_GLOBAL              0 (db)
+         450           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         458          54 LOAD_FAST                0 (conn)
+         451          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         459          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         452          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         460         100 LOAD_CONST               1 ("\n                SELECT \n                    e.id,\n                    e.domain,\n                    e.created as updated,\n                    a.name as updated_by, \n                    to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n                    c.name, \n                    c.description,\n                    c.source,\n                    c.meta->>'ownership' as ownership, \n                    c.meta->>'headquarters' as headquarters,\n                    c.meta->>'city' as city,\n                    c.meta->>'state' as state,\n                    c.meta->>'designation' as designation,\n                    c.meta->>'products' as products,\n                    c.meta->>'services' as services,\n                    c.meta->>'end_customer' as end_customer,\n                    c.meta->>'geographies' as geographies,\n                    c.meta->>'was_acquired' as was_acquired,\n                    c.meta->>'justification' as justification,\n                    c.meta->>'year_founded' as year_founded,\n                    c.meta->>'linkedin' as linkedin,\n                    c.meta->>'linkedin_range' as linkedin_range,\n                    c.meta->>'primary_contact' as primary_contact,\n                    c.meta->>'industry' as industry,\n                    c.meta->>'revenue_estimates' as revenue_estimates,\n                    c.meta->>'location_count' as location_count,\n                    c.meta->>'business_models' as business_models,\n                    c.meta->>'facility_size' as facility_size,\n                    c.meta,\n                    COALESCE(co.comments, '[]'::jsonb) as comments\n                FROM event e\n                LEFT JOIN actor a ON e.actor_key = a.key\n                LEFT JOIN company c ON e.domain = c.domain\n                LEFT JOIN comment co ON e.domain = co.domain\n                WHERE e.type = 'buyer'\n                ")
+         453         100 LOAD_CONST               1 ("\n                SELECT \n                    e.id,\n                    e.domain,\n                    e.created as updated,\n                    a.name as updated_by, \n                    to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n                    c.name, \n                    c.description,\n                    c.source,\n                    c.meta->>'ownership' as ownership, \n                    c.meta->>'headquarters' as headquarters,\n                    c.meta->>'city' as city,\n                    c.meta->>'state' as state,\n                    c.meta->>'designation' as designation,\n                    c.meta->>'products' as products,\n                    c.meta->>'services' as services,\n                    c.meta->>'end_customer' as end_customer,\n                    c.meta->>'geographies' as geographies,\n                    c.meta->>'was_acquired' as was_acquired,\n                    c.meta->>'justification' as justification,\n                    c.meta->>'year_founded' as year_founded,\n                    c.meta->>'linkedin' as linkedin,\n                    c.meta->>'linkedin_range' as linkedin_range,\n                    c.meta->>'primary_contact' as primary_contact,\n                    c.meta->>'industry' as industry,\n                    c.meta->>'revenue_estimates' as revenue_estimates,\n                    c.meta->>'location_count' as location_count,\n                    c.meta->>'business_models' as business_models,\n                    c.meta->>'facility_size' as facility_size,\n                    c.meta,\n                    COALESCE(co.comments, '[]'::jsonb) as comments\n                FROM event e\n                LEFT JOIN actor a ON e.actor_key = a.key\n                LEFT JOIN company c ON e.domain = c.domain\n                LEFT JOIN comment co ON e.domain = co.domain\n                WHERE e.type = 'buyer'\n                ")
          
-         459         102 PRECALL                  1
+         452         102 PRECALL                  1
                      106 CALL                     1
          
-         458         116 PRECALL                  1
+         451         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         500         132 LOAD_GLOBAL             11 (NULL + pd)
+         493         132 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         457         248 LOAD_CONST               0 (None)
+         450         248 LOAD_CONST               0 (None)
                      250 LOAD_CONST               0 (None)
                      252 LOAD_CONST               0 (None)
                      254 PRECALL                  2
                      258 CALL                     2
                      268 POP_TOP
                      270 JUMP_FORWARD            11 (to 294)
                  >>  272 PUSH_EXC_INFO
@@ -2743,30 +2755,30 @@
                      282 POP_EXCEPT
                      284 RERAISE                  1
                  >>  286 POP_TOP
                      288 POP_EXCEPT
                      290 POP_TOP
                      292 POP_TOP
          
-         502     >>  294 LOAD_CONST               3 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 502>)
+         495     >>  294 LOAD_CONST               3 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 495>)
                      296 MAKE_FUNCTION            0
                      298 STORE_FAST               3 (get_employees)
          
-         514         300 LOAD_FAST                2 (df)
+         507         300 LOAD_FAST                2 (df)
                      302 LOAD_CONST               4 ('meta')
                      304 BINARY_SUBSCR
                      314 LOAD_METHOD              9 (apply)
                      336 LOAD_FAST                3 (get_employees)
                      338 PRECALL                  1
                      342 CALL                     1
                      352 LOAD_FAST                2 (df)
                      354 LOAD_CONST               5 ('employees')
                      356 STORE_SUBSCR
          
-         515         360 LOAD_FAST                2 (df)
+         508         360 LOAD_FAST                2 (df)
                      362 RETURN_VALUE
          ExceptionTable:
            52 to 246 -> 272 [1] lasti
            272 to 278 -> 280 [3] lasti
            286 to 286 -> 280 [3] lasti
          consts
             None
@@ -2781,60 +2793,60 @@
                   0x97007c00a00000000000000000000000000000000000000000006401a6
                   010000ab010000000000000000721e09007403000000000000000000007c
                   00640119000000000000000000a6010000ab010000000000000000530023
                   0001005900640053007803590077017c00a0000000000000000000000000
                   0000000000000000006402a6010000ab010000000000000000721b7c0064
                   0219000000000000000000a0000000000000000000000000000000000000
                   0000006403a6010000ab010000000000000000530064005300
-               502           0 RESUME                   0
+               495           0 RESUME                   0
                
-               503           2 LOAD_FAST                0 (meta)
+               496           2 LOAD_FAST                0 (meta)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('employees')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE    30 (to 104)
                
-               505          44 NOP
+               498          44 NOP
                
-               506          46 LOAD_GLOBAL              3 (NULL + int)
+               499          46 LOAD_GLOBAL              3 (NULL + int)
                             58 LOAD_FAST                0 (meta)
                             60 LOAD_CONST               1 ('employees')
                             62 BINARY_SUBSCR
                             72 PRECALL                  1
                             76 CALL                     1
                             86 RETURN_VALUE
                        >>   88 PUSH_EXC_INFO
                
-               507          90 POP_TOP
+               500          90 POP_TOP
                
-               508          92 POP_EXCEPT
+               501          92 POP_EXCEPT
                             94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                        >>   98 COPY                     3
                            100 POP_EXCEPT
                            102 RERAISE                  1
                
-               509     >>  104 LOAD_FAST                0 (meta)
+               502     >>  104 LOAD_FAST                0 (meta)
                            106 LOAD_METHOD              0 (get)
                            128 LOAD_CONST               2 ('grata_employee_estimates')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 POP_JUMP_FORWARD_IF_FALSE    27 (to 200)
                
-               510         146 LOAD_FAST                0 (meta)
+               503         146 LOAD_FAST                0 (meta)
                            148 LOAD_CONST               2 ('grata_employee_estimates')
                            150 BINARY_SUBSCR
                            160 LOAD_METHOD              0 (get)
                            182 LOAD_CONST               3 ('count')
                            184 PRECALL                  1
                            188 CALL                     1
                            198 RETURN_VALUE
                
-               512     >>  200 LOAD_CONST               0 (None)
+               505     >>  200 LOAD_CONST               0 (None)
                            202 RETURN_VALUE
                ExceptionTable:
                  46 to 84 -> 88 [0]
                  88 to 90 -> 98 [1] lasti
                consts
                   None
                   'employees'
@@ -2842,25 +2854,25 @@
                   'count'
                names      ('get', 'int')
                varnames   ('meta',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_employees'
-               firstlineno 502
+               firstlineno 495
                lnotab 0x02012a0202012c0102010c012a013602
             'meta'
             'employees'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'apply')
          varnames   ('conn', 'result', 'df', 'get_employees')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'buyer'
-         firstlineno 456
+         firstlineno 449
          lnotab 0x020134011801160102ff0eff102a74d52e2d060c3c01
       code
          argcount  : 1
          nlocals   : 10
          stacksize : 6
          flags     : 3
          code
@@ -2882,59 +2894,59 @@
             010000ab0100000000000000007c04640c3c0000007c04640d1900000000
             0000000000a00a00000000000000000000000000000000000000007c07a6
             010000ab0100000000000000007c04640d3c0000007c04a00a0000000000
             0000000000000000000000000000007c08640eac0fa6020000ab02000000
             00000000007c0464103c0000007c04a00a00000000000000000000000000
             000000000000007c09640eac0fa6020000ab0200000000000000007c0464
             113c0000007c045300
-         553           0 RESUME                   0
+         546           0 RESUME                   0
          
-         556           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute','enrich')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        -- c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n        AND e.domain != ''\n    ;\n    ")
+         549           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute','enrich')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        -- c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n        AND e.domain != ''\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
-         620           6 LOAD_GLOBAL              0 (db)
+         613           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         621          58 LOAD_FAST                2 (conn)
+         614          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         622          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         615          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         623         120 LOAD_CONST               2 ('search_uid')
+         616         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         621         126 PRECALL                  2
+         614         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         625         142 LOAD_GLOBAL             11 (NULL + pd)
+         618         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         620         258 LOAD_CONST               0 (None)
+         613         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2945,93 +2957,93 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         627     >>  304 LOAD_CONST               4 ('return')
+         620     >>  304 LOAD_CONST               4 ('return')
                      306 LOAD_GLOBAL             18 (str)
                      318 BUILD_TUPLE              2
-                     320 LOAD_CONST               5 (<code object list_to_csv, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 627>)
+                     320 LOAD_CONST               5 (<code object list_to_csv, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 620>)
                      322 MAKE_FUNCTION            4 (annotations)
                      324 STORE_FAST               5 (list_to_csv)
          
-         639         326 LOAD_CONST               6 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 639>)
+         632         326 LOAD_CONST               6 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 632>)
                      328 MAKE_FUNCTION            0
                      330 STORE_FAST               6 (get_employees)
          
-         651         332 LOAD_CONST               7 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 651>)
+         644         332 LOAD_CONST               7 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 644>)
                      334 MAKE_FUNCTION            0
                      336 STORE_FAST               7 (get_ownership)
          
-         659         338 LOAD_CONST               8 (<code object get_state, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 659>)
+         652         338 LOAD_CONST               8 (<code object get_state, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 652>)
                      340 MAKE_FUNCTION            0
                      342 STORE_FAST               8 (get_state)
          
-         669         344 LOAD_CONST               9 (<code object get_city, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 669>)
+         662         344 LOAD_CONST               9 (<code object get_city, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 662>)
                      346 MAKE_FUNCTION            0
                      348 STORE_FAST               9 (get_city)
          
-         678         350 LOAD_FAST                4 (df)
+         671         350 LOAD_FAST                4 (df)
                      352 LOAD_CONST              10 ('end_customer')
                      354 BINARY_SUBSCR
                      364 LOAD_METHOD             10 (apply)
                      386 LOAD_FAST                5 (list_to_csv)
                      388 PRECALL                  1
                      392 CALL                     1
                      402 LOAD_FAST                4 (df)
                      404 LOAD_CONST              10 ('end_customer')
                      406 STORE_SUBSCR
          
-         679         410 LOAD_FAST                4 (df)
+         672         410 LOAD_FAST                4 (df)
                      412 LOAD_CONST              11 ('meta')
                      414 BINARY_SUBSCR
                      424 LOAD_METHOD             10 (apply)
                      446 LOAD_FAST                6 (get_employees)
                      448 PRECALL                  1
                      452 CALL                     1
                      462 LOAD_FAST                4 (df)
                      464 LOAD_CONST              12 ('employees')
                      466 STORE_SUBSCR
          
-         680         470 LOAD_FAST                4 (df)
+         673         470 LOAD_FAST                4 (df)
                      472 LOAD_CONST              13 ('ownership')
                      474 BINARY_SUBSCR
                      484 LOAD_METHOD             10 (apply)
                      506 LOAD_FAST                7 (get_ownership)
                      508 PRECALL                  1
                      512 CALL                     1
                      522 LOAD_FAST                4 (df)
                      524 LOAD_CONST              13 ('ownership')
                      526 STORE_SUBSCR
          
-         681         530 LOAD_FAST                4 (df)
+         674         530 LOAD_FAST                4 (df)
                      532 LOAD_METHOD             10 (apply)
                      554 LOAD_FAST                8 (get_state)
                      556 LOAD_CONST              14 (1)
                      558 KW_NAMES                15
                      560 PRECALL                  2
                      564 CALL                     2
                      574 LOAD_FAST                4 (df)
                      576 LOAD_CONST              16 ('state')
                      578 STORE_SUBSCR
          
-         682         582 LOAD_FAST                4 (df)
+         675         582 LOAD_FAST                4 (df)
                      584 LOAD_METHOD             10 (apply)
                      606 LOAD_FAST                9 (get_city)
                      608 LOAD_CONST              14 (1)
                      610 KW_NAMES                15
                      612 PRECALL                  2
                      616 CALL                     2
                      626 LOAD_FAST                4 (df)
                      628 LOAD_CONST              17 ('city')
                      630 STORE_SUBSCR
          
-         684         634 LOAD_FAST                4 (df)
+         677         634 LOAD_FAST                4 (df)
                      636 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3045,39 +3057,39 @@
                stacksize : 4
                flags     : 19
                code
                   0x970009007401000000000000000000006a0100000000000000007c00a6
                   010000ab0100000000000000007d016401a0020000000000000000000000
                   0000000000000000007c01a6010000ab0100000000000000007d027c0253
                   0023000100590064025300780359007701
-               627           0 RESUME                   0
+               620           0 RESUME                   0
                
-               629           2 NOP
+               622           2 NOP
                
-               630           4 LOAD_GLOBAL              1 (NULL + json)
+               623           4 LOAD_GLOBAL              1 (NULL + json)
                             16 LOAD_ATTR                1 (loads)
                             26 LOAD_FAST                0 (list_str)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 STORE_FAST               1 (list_data)
                
-               633          44 LOAD_CONST               1 (', ')
+               626          44 LOAD_CONST               1 (', ')
                             46 LOAD_METHOD              2 (join)
                             68 LOAD_FAST                1 (list_data)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 STORE_FAST               2 (csv_str)
                
-               635          86 LOAD_FAST                2 (csv_str)
+               628          86 LOAD_FAST                2 (csv_str)
                             88 RETURN_VALUE
                        >>   90 PUSH_EXC_INFO
                
-               636          92 POP_TOP
+               629          92 POP_TOP
                
-               637          94 POP_EXCEPT
+               630          94 POP_EXCEPT
                             96 LOAD_CONST               2 ('')
                             98 RETURN_VALUE
                        >>  100 COPY                     3
                            102 POP_EXCEPT
                            104 RERAISE                  1
                ExceptionTable:
                  4 to 86 -> 90 [0]
@@ -3088,75 +3100,75 @@
                   ''
                names      ('json', 'loads', 'join')
                varnames   ('list_str', 'list_data', 'csv_str')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'list_to_csv'
-               firstlineno 627
+               firstlineno 620
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
-               639           0 RESUME                   0
+               632           0 RESUME                   0
                
-               640           2 LOAD_FAST                0 (meta)
+               633           2 LOAD_FAST                0 (meta)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('employees')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE    30 (to 104)
                
-               642          44 NOP
+               635          44 NOP
                
-               643          46 LOAD_GLOBAL              3 (NULL + int)
+               636          46 LOAD_GLOBAL              3 (NULL + int)
                             58 LOAD_FAST                0 (meta)
                             60 LOAD_CONST               1 ('employees')
                             62 BINARY_SUBSCR
                             72 PRECALL                  1
                             76 CALL                     1
                             86 RETURN_VALUE
                        >>   88 PUSH_EXC_INFO
                
-               644          90 POP_TOP
+               637          90 POP_TOP
                
-               645          92 POP_EXCEPT
+               638          92 POP_EXCEPT
                             94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                        >>   98 COPY                     3
                            100 POP_EXCEPT
                            102 RERAISE                  1
                
-               646     >>  104 LOAD_FAST                0 (meta)
+               639     >>  104 LOAD_FAST                0 (meta)
                            106 LOAD_METHOD              0 (get)
                            128 LOAD_CONST               2 ('grata_employee_estimates')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 POP_JUMP_FORWARD_IF_FALSE    27 (to 200)
                
-               647         146 LOAD_FAST                0 (meta)
+               640         146 LOAD_FAST                0 (meta)
                            148 LOAD_CONST               2 ('grata_employee_estimates')
                            150 BINARY_SUBSCR
                            160 LOAD_METHOD              0 (get)
                            182 LOAD_CONST               3 ('count')
                            184 PRECALL                  1
                            188 CALL                     1
                            198 RETURN_VALUE
                
-               649     >>  200 LOAD_CONST               0 (None)
+               642     >>  200 LOAD_CONST               0 (None)
                            202 RETURN_VALUE
                ExceptionTable:
                  46 to 84 -> 88 [0]
                  88 to 90 -> 98 [1] lasti
                consts
                   None
                   'employees'
@@ -3164,57 +3176,57 @@
                   'count'
                names      ('get', 'int')
                varnames   ('meta',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_employees'
-               firstlineno 639
+               firstlineno 632
                lnotab 0x02012a0202012c0102010c012a013602
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 19
                code
                   0x97007c0064016b02000000007202640253007c0064036b020000000072
                   02640453007c005300
-               651           0 RESUME                   0
+               644           0 RESUME                   0
                
-               652           2 LOAD_FAST                0 (ownership)
+               645           2 LOAD_FAST                0 (ownership)
                              4 LOAD_CONST               1 ('Bootstrapped')
                              6 COMPARE_OP               2 (==)
                             12 POP_JUMP_FORWARD_IF_FALSE     2 (to 18)
                
-               653          14 LOAD_CONST               2 ('Private')
+               646          14 LOAD_CONST               2 ('Private')
                             16 RETURN_VALUE
                
-               654     >>   18 LOAD_FAST                0 (ownership)
+               647     >>   18 LOAD_FAST                0 (ownership)
                             20 LOAD_CONST               3 ('Investor Backed')
                             22 COMPARE_OP               2 (==)
                             28 POP_JUMP_FORWARD_IF_FALSE     2 (to 34)
                
-               655          30 LOAD_CONST               4 ('Venture Capital')
+               648          30 LOAD_CONST               4 ('Venture Capital')
                             32 RETURN_VALUE
                
-               657     >>   34 LOAD_FAST                0 (ownership)
+               650     >>   34 LOAD_FAST                0 (ownership)
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
-               firstlineno 651
+               firstlineno 644
                lnotab 0x02010c0104010c010402
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 19
                code
@@ -3224,78 +3236,78 @@
                   00ab010000000000000000725a7c00640219000000000000000000a00100
                   000000000000000000000000000000000000006403a6010000ab01000000
                   0000000000640419000000000000000000a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d017406000000
                   000000000000006a0400000000000000006a050000000000000000a00000
                   000000000000000000000000000000000000007c016405a6020000ab0200
                   000000000000007d027c02530064005300
-               659           0 RESUME                   0
+               652           0 RESUME                   0
                
-               660           2 LOAD_FAST                0 (row)
+               653           2 LOAD_FAST                0 (row)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('state')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE     8 (to 60)
                
-               661          44 LOAD_FAST                0 (row)
+               654          44 LOAD_FAST                0 (row)
                             46 LOAD_CONST               1 ('state')
                             48 BINARY_SUBSCR
                             58 RETURN_VALUE
                
-               662     >>   60 LOAD_FAST                0 (row)
+               655     >>   60 LOAD_FAST                0 (row)
                             62 LOAD_METHOD              0 (get)
                             84 LOAD_CONST               2 ('headquarters')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_JUMP_FORWARD_IF_FALSE    90 (to 282)
                
-               663         102 LOAD_FAST                0 (row)
+               656         102 LOAD_FAST                0 (row)
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
                
-               664         204 LOAD_GLOBAL              6 (ts)
+               657         204 LOAD_GLOBAL              6 (ts)
                            216 LOAD_ATTR                4 (constants)
                            226 LOAD_ATTR                5 (STATE_NAMES)
                            236 LOAD_METHOD              0 (get)
                            258 LOAD_FAST                1 (state_name)
                            260 LOAD_CONST               5 ('')
                            262 PRECALL                  2
                            266 CALL                     2
                            276 STORE_FAST               2 (state_code)
                
-               665         278 LOAD_FAST                2 (state_code)
+               658         278 LOAD_FAST                2 (state_code)
                            280 RETURN_VALUE
                
-               667     >>  282 LOAD_CONST               0 (None)
+               660     >>  282 LOAD_CONST               0 (None)
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
-               firstlineno 659
+               firstlineno 652
                lnotab 0x02012a0110012a0166014a010402
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
@@ -3303,67 +3315,67 @@
                   010000ab01000000000000000072087c0064011900000000000000000053
                   007c00a00000000000000000000000000000000000000000006402a60100
                   00ab01000000000000000072357c00640219000000000000000000a00100
                   000000000000000000000000000000000000006403a6010000ab01000000
                   0000000000640419000000000000000000a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d017c01530064
                   005300
-               669           0 RESUME                   0
+               662           0 RESUME                   0
                
-               670           2 LOAD_FAST                0 (row)
+               663           2 LOAD_FAST                0 (row)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('city')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE     8 (to 60)
                
-               671          44 LOAD_FAST                0 (row)
+               664          44 LOAD_FAST                0 (row)
                             46 LOAD_CONST               1 ('city')
                             48 BINARY_SUBSCR
                             58 RETURN_VALUE
                
-               672     >>   60 LOAD_FAST                0 (row)
+               665     >>   60 LOAD_FAST                0 (row)
                             62 LOAD_METHOD              0 (get)
                             84 LOAD_CONST               2 ('headquarters')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_JUMP_FORWARD_IF_FALSE    53 (to 208)
                
-               673         102 LOAD_FAST                0 (row)
+               666         102 LOAD_FAST                0 (row)
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
                
-               674         204 LOAD_FAST                1 (city_name)
+               667         204 LOAD_FAST                1 (city_name)
                            206 RETURN_VALUE
                
-               676     >>  208 LOAD_CONST               0 (None)
+               669     >>  208 LOAD_CONST               0 (None)
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
-               firstlineno 669
+               firstlineno 662
                lnotab 0x02012a0110012a0166010402
             'end_customer'
             'meta'
             'employees'
             'ownership'
             1
             ('axis',)
@@ -3371,15 +3383,15 @@
             'city'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'str', 'apply')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df', 'list_to_csv', 'get_employees', 'get_ownership', 'get_state', 'get_city')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_targets'
-         firstlineno 553
+         firstlineno 546
          lnotab
             0x0203044034011801260106fe100474fb2e07160c060c0608060a06093c
             013c013c0134013402
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
@@ -3392,59 +3404,59 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         687           0 RESUME                   0
+         680           0 RESUME                   0
          
-         688           2 LOAD_CONST               1 ("\n    SELECT \n        e.*,\n        a.name as author\n    FROM event e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    WHERE\n        e.type = 'comment'\n        AND e.domain is null\n        AND search_uid = :search_uid\n    ")
+         681           2 LOAD_CONST               1 ("\n    SELECT \n        e.*,\n        a.name as author\n    FROM event e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    WHERE\n        e.type = 'comment'\n        AND e.domain is null\n        AND search_uid = :search_uid\n    ")
                        4 STORE_FAST               1 (statement)
          
-         700           6 LOAD_GLOBAL              0 (db)
+         693           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         701          58 LOAD_FAST                2 (conn)
+         694          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         702          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         695          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         703         120 LOAD_CONST               2 ('search_uid')
+         696         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         701         126 PRECALL                  2
+         694         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         705         142 LOAD_GLOBAL             11 (NULL + pd)
+         698         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         700         258 LOAD_CONST               0 (None)
+         693         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3455,15 +3467,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         706     >>  304 LOAD_FAST                4 (df)
+         699     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3472,15 +3484,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_comments'
-         firstlineno 687
+         firstlineno 680
          lnotab 0x0201040c34011801260106fe100474fb2e06
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3491,56 +3503,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         709           0 RESUME                   0
+         702           0 RESUME                   0
          
-         710           2 LOAD_GLOBAL              0 (db)
+         703           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         711          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         704          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         716          58 LOAD_FAST                1 (conn)
+         709          58 LOAD_FAST                1 (conn)
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
          
-         717         142 LOAD_GLOBAL             11 (NULL + pd)
+         710         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         710         258 LOAD_CONST               0 (None)
+         703         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3551,15 +3563,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         718     >>  304 LOAD_FAST                4 (df)
+         711     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3568,15 +3580,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event'
-         firstlineno 709
+         firstlineno 702
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3588,65 +3600,65 @@
             007c01a6010000ab01000000000000000064027c006901a6020000ab0200
             000000000000007d03740f000000000000000000006a0800000000000000
             007c03a0090000000000000000000000000000000000000000a6000000ab
             0000000000000000007c03a00a0000000000000000000000000000000000
             000000a6000000ab000000000000000000ac03a6020000ab020000000000
             0000007d04640064006400a6020000ab02000000000000000001006e0b23
             0031007304770278035900770101005900010001007c045300
-         721           0 RESUME                   0
+         714           0 RESUME                   0
          
-         722           2 LOAD_GLOBAL              1 (NULL + isinstance)
+         715           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (search_uid)
                       16 LOAD_GLOBAL              2 (int)
                       28 PRECALL                  2
                       32 CALL                     2
                       42 POP_JUMP_FORWARD_IF_TRUE     2 (to 48)
                       44 LOAD_ASSERTION_ERROR
                       46 RAISE_VARARGS            1
          
-         723     >>   48 LOAD_CONST               1 ("\n    SELECT \n        e.id,\n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.domain,\n        e.data,\n        a.type as actor_type,\n        a.key as actor_key,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type != 'mute'\n    ORDER BY created DESC\n    ;\n\n    ")
+         716     >>   48 LOAD_CONST               1 ("\n    SELECT \n        e.id,\n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.domain,\n        e.data,\n        a.type as actor_type,\n        a.key as actor_key,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type != 'mute'\n    ORDER BY created DESC\n    ;\n\n    ")
                       50 STORE_FAST               1 (statement)
          
-         745          52 LOAD_GLOBAL              4 (db)
+         738          52 LOAD_GLOBAL              4 (db)
                       64 LOAD_METHOD              3 (connect)
                       86 PRECALL                  0
                       90 CALL                     0
                      100 BEFORE_WITH
                      102 STORE_FAST               2 (conn)
          
-         746         104 LOAD_FAST                2 (conn)
+         739         104 LOAD_FAST                2 (conn)
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
          
-         747         188 LOAD_GLOBAL             15 (NULL + pd)
+         740         188 LOAD_GLOBAL             15 (NULL + pd)
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
          
-         745         304 LOAD_CONST               0 (None)
+         738         304 LOAD_CONST               0 (None)
                      306 LOAD_CONST               0 (None)
                      308 LOAD_CONST               0 (None)
                      310 PRECALL                  2
                      314 CALL                     2
                      324 POP_TOP
                      326 JUMP_FORWARD            11 (to 350)
                  >>  328 PUSH_EXC_INFO
@@ -3657,15 +3669,15 @@
                      338 POP_EXCEPT
                      340 RERAISE                  1
                  >>  342 POP_TOP
                      344 POP_EXCEPT
                      346 POP_TOP
                      348 POP_TOP
          
-         748     >>  350 LOAD_FAST                4 (df)
+         741     >>  350 LOAD_FAST                4 (df)
                      352 RETURN_VALUE
          ExceptionTable:
            102 to 302 -> 328 [1] lasti
            328 to 334 -> 336 [3] lasti
            342 to 342 -> 336 [3] lasti
          consts
             None
@@ -3674,15 +3686,15 @@
             ('columns',)
          names      ('isinstance', 'int', 'db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event_history'
-         firstlineno 721
+         firstlineno 714
          lnotab 0x02012e0104163401540174fe2e03
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3693,56 +3705,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         751           0 RESUME                   0
+         744           0 RESUME                   0
          
-         753           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
+         746           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
-         771           6 LOAD_GLOBAL              0 (db)
+         764           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         772          58 LOAD_FAST                2 (conn)
+         765          58 LOAD_FAST                2 (conn)
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
          
-         773         142 LOAD_GLOBAL             11 (NULL + pd)
+         766         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         771         258 LOAD_CONST               0 (None)
+         764         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3753,15 +3765,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         774     >>  304 LOAD_FAST                4 (df)
+         767     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3770,15 +3782,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_criteria_history'
-         firstlineno 751
+         firstlineno 744
          lnotab 0x020204123401540174fe2e03
       'uid'
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 7
          flags     : 3
@@ -3796,96 +3808,96 @@
             000000000000007d05741300000000000000000000741400000000000000
             0000006a0b00000000000000006a0c00000000000000007c05a6020000ab
             0200000000000000007d067c066a0d0000000000000000a00e0000000000
             0000000000000000000000000000006403a6010000ab0100000000000000
             006404190000000000000000007c066a0f000000000000000064053c0000
             00640064006400a6020000ab02000000000000000001006e0b2300310073
             04770278035900770101005900010001007c065300
-         780           0 RESUME                   0
+         773           0 RESUME                   0
          
-         781           2 LOAD_GLOBAL              0 (db)
+         774           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         782          54 LOAD_CONST               1 ('\n            SELECT \n                uid, \n                label, \n                meta \n            FROM search\n            \n            WHERE uid = :uid\n            ')
+         775          54 LOAD_CONST               1 ('\n            SELECT \n                uid, \n                label, \n                meta \n            FROM search\n            \n            WHERE uid = :uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         791          58 LOAD_FAST                1 (conn)
+         784          58 LOAD_FAST                1 (conn)
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
          
-         793         142 LOAD_FAST                3 (result)
+         786         142 LOAD_FAST                3 (result)
                      144 LOAD_METHOD              5 (fetchone)
                      166 PRECALL                  0
                      170 CALL                     0
                      180 STORE_FAST               4 (row)
          
-         794         182 LOAD_FAST                4 (row)
+         787         182 LOAD_FAST                4 (row)
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 214)
          
-         795         186 NOP
+         788         186 NOP
          
-         781         188 LOAD_CONST               0 (None)
+         774         188 LOAD_CONST               0 (None)
                      190 LOAD_CONST               0 (None)
                      192 LOAD_CONST               0 (None)
                      194 PRECALL                  2
                      198 CALL                     2
                      208 POP_TOP
                      210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         797     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         790     >>  214 LOAD_GLOBAL             13 (NULL + dict)
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
          
-         798         308 LOAD_GLOBAL             19 (NULL + from_dict)
+         791         308 LOAD_GLOBAL             19 (NULL + from_dict)
                      320 LOAD_GLOBAL             20 (ts)
                      332 LOAD_ATTR               11 (models)
                      342 LOAD_ATTR               12 (Search)
                      352 LOAD_FAST                5 (obj)
                      354 PRECALL                  2
                      358 CALL                     2
                      368 STORE_FAST               6 (search)
          
-         799         370 LOAD_FAST                6 (search)
+         792         370 LOAD_FAST                6 (search)
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
          
-         781         450 LOAD_CONST               0 (None)
+         774         450 LOAD_CONST               0 (None)
                      452 LOAD_CONST               0 (None)
                      454 LOAD_CONST               0 (None)
                      456 PRECALL                  2
                      460 CALL                     2
                      470 POP_TOP
                      472 JUMP_FORWARD            11 (to 496)
                  >>  474 PUSH_EXC_INFO
@@ -3896,15 +3908,15 @@
                      484 POP_EXCEPT
                      486 RERAISE                  1
                  >>  488 POP_TOP
                      490 POP_EXCEPT
                      492 POP_TOP
                      494 POP_TOP
          
-         801     >>  496 LOAD_FAST                6 (search)
+         794     >>  496 LOAD_FAST                6 (search)
                      498 RETURN_VALUE
          ExceptionTable:
            52 to 186 -> 474 [1] lasti
            214 to 448 -> 474 [1] lasti
            474 to 480 -> 482 [3] lasti
            488 to 488 -> 482 [3] lasti
          consts
@@ -3916,15 +3928,15 @@
             'client'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'fetchone', 'dict', 'zip', 'keys', 'from_dict', 'ts', 'models', 'Search', 'label', 'split', 'meta')
          varnames   ('uid', 'conn', 'statement', 'result', 'row', 'obj', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search'
-         firstlineno 780
+         firstlineno 773
          lnotab 0x02013401040954022801040102f21a105e013e0150ee2e14
       'label'
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 7
          flags     : 3
@@ -3940,83 +3952,83 @@
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c04a6020000ab020000000000000000a6010000ab0100
             000000000000007d05741300000000000000000000741400000000000000
             0000006a0b00000000000000006a0c00000000000000007c05a6020000ab
             0200000000000000007d06640064006400a6020000ab0200000000000000
             0001006e0b230031007304770278035900770101005900010001007c0653
             00
-         804           0 RESUME                   0
+         797           0 RESUME                   0
          
-         805           2 LOAD_GLOBAL              0 (db)
+         798           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         806          54 LOAD_CONST               1 ('\n            SELECT \n                uid, \n                label, \n                meta \n            FROM search\n            \n            WHERE label = :label\n            ')
+         799          54 LOAD_CONST               1 ('\n            SELECT \n                uid, \n                label, \n                meta \n            FROM search\n            \n            WHERE label = :label\n            ')
                       56 STORE_FAST               2 (statement)
          
-         815          58 LOAD_FAST                1 (conn)
+         808          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('label')
                      122 LOAD_FAST                0 (label)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         817         142 LOAD_FAST                3 (result)
+         810         142 LOAD_FAST                3 (result)
                      144 LOAD_METHOD              5 (fetchone)
                      166 PRECALL                  0
                      170 CALL                     0
                      180 STORE_FAST               4 (row)
          
-         818         182 LOAD_FAST                4 (row)
+         811         182 LOAD_FAST                4 (row)
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 214)
          
-         819         186 NOP
+         812         186 NOP
          
-         805         188 LOAD_CONST               0 (None)
+         798         188 LOAD_CONST               0 (None)
                      190 LOAD_CONST               0 (None)
                      192 LOAD_CONST               0 (None)
                      194 PRECALL                  2
                      198 CALL                     2
                      208 POP_TOP
                      210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         821     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         814     >>  214 LOAD_GLOBAL             13 (NULL + dict)
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
          
-         822         308 LOAD_GLOBAL             19 (NULL + from_dict)
+         815         308 LOAD_GLOBAL             19 (NULL + from_dict)
                      320 LOAD_GLOBAL             20 (ts)
                      332 LOAD_ATTR               11 (models)
                      342 LOAD_ATTR               12 (Search)
                      352 LOAD_FAST                5 (obj)
                      354 PRECALL                  2
                      358 CALL                     2
                      368 STORE_FAST               6 (search)
          
-         805         370 LOAD_CONST               0 (None)
+         798         370 LOAD_CONST               0 (None)
                      372 LOAD_CONST               0 (None)
                      374 LOAD_CONST               0 (None)
                      376 PRECALL                  2
                      380 CALL                     2
                      390 POP_TOP
                      392 JUMP_FORWARD            11 (to 416)
                  >>  394 PUSH_EXC_INFO
@@ -4027,15 +4039,15 @@
                      404 POP_EXCEPT
                      406 RERAISE                  1
                  >>  408 POP_TOP
                      410 POP_EXCEPT
                      412 POP_TOP
                      414 POP_TOP
          
-         825     >>  416 LOAD_FAST                6 (search)
+         818     >>  416 LOAD_FAST                6 (search)
                      418 RETURN_VALUE
          ExceptionTable:
            52 to 186 -> 394 [1] lasti
            214 to 368 -> 394 [1] lasti
            394 to 400 -> 402 [3] lasti
            408 to 408 -> 402 [3] lasti
          consts
@@ -4044,52 +4056,52 @@
             'label'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'fetchone', 'dict', 'zip', 'keys', 'from_dict', 'ts', 'models', 'Search')
          varnames   ('label', 'conn', 'statement', 'result', 'row', 'obj', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_label'
-         firstlineno 804
+         firstlineno 797
          lnotab 0x02013401040954022801040102f21a105e013eef2e14
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
-         828           0 RESUME                   0
+         821           0 RESUME                   0
          
-         829           2 LOAD_GLOBAL              1 (NULL + searches_query)
+         822           2 LOAD_GLOBAL              1 (NULL + searches_query)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               1 (searches)
          
-         830          30 LOAD_FAST                1 (searches)
+         823          30 LOAD_FAST                1 (searches)
                       32 LOAD_FAST                1 (searches)
                       34 LOAD_CONST               1 ('searchToken')
                       36 BINARY_SUBSCR
                       46 LOAD_FAST                0 (searchToken)
                       48 COMPARE_OP               2 (==)
                       54 BINARY_SUBSCR
                       64 STORE_FAST               2 (search)
          
-         831          66 LOAD_FAST                2 (search)
+         824          66 LOAD_FAST                2 (search)
                       68 LOAD_ATTR                1 (empty)
                       78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
          
-         832          80 LOAD_CONST               0 (None)
+         825          80 LOAD_CONST               0 (None)
                       82 RETURN_VALUE
          
-         834     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
+         827     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
                       96 LOAD_FAST                2 (search)
                       98 LOAD_ATTR                3 (iloc)
                      108 LOAD_CONST               2 (0)
                      110 BINARY_SUBSCR
                      120 LOAD_CONST               3 ('uid')
                      122 BINARY_SUBSCR
                      132 PRECALL                  1
@@ -4102,15 +4114,15 @@
             'uid'
          names      ('searches_query', 'empty', 'find_search', 'iloc')
          varnames   ('searchToken', 'searches', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_token'
-         firstlineno 828
+         firstlineno 821
          lnotab 0x02011c0124010e010402
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -4124,41 +4136,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         837           0 RESUME                   0
+         830           0 RESUME                   0
          
-         838           2 LOAD_GLOBAL              0 (db)
+         831           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         839          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         832          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         844          58 LOAD_FAST                1 (conn)
+         837          58 LOAD_FAST                1 (conn)
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
          
-         838         142 LOAD_CONST               0 (None)
+         831         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -4169,24 +4181,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         846     >>  188 LOAD_FAST                3 (result)
+         839     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         847         210 LOAD_CONST               0 (None)
+         840         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         849     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         842     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -4194,15 +4206,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         850         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         843         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Company)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -4215,15 +4227,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 837
+         firstlineno 830
          lnotab 0x02013401040554fa2e08160104028201
       'email'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -4238,41 +4250,41 @@
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000006a0c00000000000000006a0d00000000000000007c
             04a6020000ab0200000000000000005300
-         853           0 RESUME                   0
+         846           0 RESUME                   0
          
-         854           2 LOAD_GLOBAL              0 (db)
+         847           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         855          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
+         848          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
                       56 STORE_FAST               2 (statement)
          
-         860          58 LOAD_FAST                1 (conn)
+         853          58 LOAD_FAST                1 (conn)
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
          
-         854         142 LOAD_CONST               0 (None)
+         847         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -4283,24 +4295,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         862     >>  188 LOAD_FAST                3 (result)
+         855     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         863         210 LOAD_CONST               0 (None)
+         856         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         865     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         858     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -4308,15 +4320,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         866         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         859         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (ts)
                      368 LOAD_ATTR               12 (models)
                      378 LOAD_ATTR               13 (Actor)
                      388 LOAD_FAST                4 (obj)
                      390 PRECALL                  2
                      394 CALL                     2
                      404 RETURN_VALUE
@@ -4331,15 +4343,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'ts', 'models', 'Actor')
          varnames   ('email', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_actor_by_email'
-         firstlineno 853
+         firstlineno 846
          lnotab 0x02013401040554fa2e08160104028201
       'event_id'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -4353,41 +4365,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         869           0 RESUME                   0
+         862           0 RESUME                   0
          
-         870           2 LOAD_GLOBAL              0 (db)
+         863           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         871          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
+         864          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         876          58 LOAD_FAST                1 (conn)
+         869          58 LOAD_FAST                1 (conn)
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
          
-         870         142 LOAD_CONST               0 (None)
+         863         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -4398,24 +4410,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         878     >>  188 LOAD_FAST                3 (result)
+         871     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         879         210 LOAD_CONST               0 (None)
+         872         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         881     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         874     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -4423,15 +4435,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         882         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         875         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Event)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -4444,15 +4456,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Event')
          varnames   ('event_id', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_event_by_id'
-         firstlineno 869
+         firstlineno 862
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 12
          flags     : 3
          code
@@ -4464,71 +4476,71 @@
             000000000000007c006a0800000000000000007c006a0900000000000000
             007415000000000000000000006a0b00000000000000007c006a0c000000
             0000000000a6010000ab01000000000000000064029c06a6020000ab0200
             0000000000000001007c01a00d0000000000000000000000000000000000
             000000a6000000ab0000000000000000000100640064006400a6020000ab
             020000000000000000010064005300230031007304770278035900770101
             0059000100010064005300
-         888           0 RESUME                   0
+         881           0 RESUME                   0
          
-         889           2 LOAD_GLOBAL              0 (db)
+         882           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         890          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
+         883          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         902          58 LOAD_FAST                1 (conn)
+         895          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         903          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         896          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         905         120 LOAD_FAST                0 (company)
+         898         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (uid)
          
-         906         132 LOAD_FAST                0 (company)
+         899         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (name)
          
-         907         144 LOAD_FAST                0 (company)
+         900         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (description)
          
-         908         156 LOAD_FAST                0 (company)
+         901         156 LOAD_FAST                0 (company)
                      158 LOAD_ATTR                8 (domain)
          
-         909         168 LOAD_FAST                0 (company)
+         902         168 LOAD_FAST                0 (company)
                      170 LOAD_ATTR                9 (source)
          
-         910         180 LOAD_GLOBAL             21 (NULL + json)
+         903         180 LOAD_GLOBAL             21 (NULL + json)
                      192 LOAD_ATTR               11 (dumps)
                      202 LOAD_FAST                0 (company)
                      204 LOAD_ATTR               12 (meta)
                      214 PRECALL                  1
                      218 CALL                     1
          
-         904         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
+         897         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
                      230 BUILD_CONST_KEY_MAP      6
          
-         902         232 PRECALL                  2
+         895         232 PRECALL                  2
                      236 CALL                     2
                      246 POP_TOP
          
-         914         248 LOAD_FAST                1 (conn)
+         907         248 LOAD_FAST                1 (conn)
                      250 LOAD_METHOD             13 (commit)
                      272 PRECALL                  0
                      276 CALL                     0
                      286 POP_TOP
          
-         889         288 LOAD_CONST               0 (None)
+         882         288 LOAD_CONST               0 (None)
                      290 LOAD_CONST               0 (None)
                      292 LOAD_CONST               0 (None)
                      294 PRECALL                  2
                      298 CALL                     2
                      308 POP_TOP
                      310 LOAD_CONST               0 (None)
                      312 RETURN_VALUE
@@ -4555,15 +4567,15 @@
             ('uid', 'name', 'description', 'domain', 'source', 'meta')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'uid', 'name', 'description', 'domain', 'source', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 888
+         firstlineno 881
          lnotab 0x02013401040c180126020c010c010c010c010c0130fa04fe100c28e7
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
@@ -4573,58 +4585,58 @@
             006a0400000000000000006401a6010000ab010000000000000000740b00
             0000000000000000006a0600000000000000007c006a0700000000000000
             00a6010000ab0100000000000000007c006a08000000000000000064029c
             02a6020000ab02000000000000000001007c01a009000000000000000000
             0000000000000000000000a6000000ab0000000000000000000100640064
             006400a6020000ab02000000000000000001006400530023003100730477
             02780359007701010059000100010064005300
-         917           0 RESUME                   0
+         910           0 RESUME                   0
          
-         918           2 LOAD_GLOBAL              0 (db)
+         911           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         919          54 LOAD_FAST                1 (conn)
+         912          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         920          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         913          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         921         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
+         914         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
          
-         920         102 PRECALL                  1
+         913         102 PRECALL                  1
                      106 CALL                     1
          
-         930         116 LOAD_GLOBAL             11 (NULL + json)
+         923         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (meta)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         931         164 LOAD_FAST                0 (search)
+         924         164 LOAD_FAST                0 (search)
                      166 LOAD_ATTR                8 (uid)
          
-         929         176 LOAD_CONST               2 (('meta', 'uid'))
+         922         176 LOAD_CONST               2 (('meta', 'uid'))
                      178 BUILD_CONST_KEY_MAP      2
          
-         919         180 PRECALL                  2
+         912         180 PRECALL                  2
                      184 CALL                     2
                      194 POP_TOP
          
-         934         196 LOAD_FAST                1 (conn)
+         927         196 LOAD_FAST                1 (conn)
                      198 LOAD_METHOD              9 (commit)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 POP_TOP
          
-         918         236 LOAD_CONST               0 (None)
+         911         236 LOAD_CONST               0 (None)
                      238 LOAD_CONST               0 (None)
                      240 LOAD_CONST               0 (None)
                      242 PRECALL                  2
                      246 CALL                     2
                      256 POP_TOP
                      258 LOAD_CONST               0 (None)
                      260 RETURN_VALUE
@@ -4651,15 +4663,15 @@
             ('meta', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'meta', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 917
+         firstlineno 910
          lnotab 0x020134011801160102ff0e0a30010cfe04f6100f28f0
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4670,61 +4682,61 @@
             006901a6020000ab02000000000000000001007c01a00200000000000000
             000000000000000000000000007407000000000000000000006a04000000
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00500000000000000000000000000000000000000
             00a6000000ab0000000000000000000100640064006400a6020000ab0200
             000000000000000100640053002300310073047702780359007701010059
             000100010064005300
-         940           0 RESUME                   0
+         933           0 RESUME                   0
          
-         942           2 LOAD_GLOBAL              0 (db)
+         935           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         943          54 LOAD_FAST                1 (conn)
+         936          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         944          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         937          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         945         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
+         938         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
          
-         944         102 PRECALL                  1
+         937         102 PRECALL                  1
                      106 CALL                     1
          
-         953         116 LOAD_CONST               2 ('event_id')
+         946         116 LOAD_CONST               2 ('event_id')
                      118 LOAD_FAST                0 (event_id)
          
-         952         120 BUILD_MAP                1
+         945         120 BUILD_MAP                1
          
-         943         122 PRECALL                  2
+         936         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         956         138 LOAD_FAST                1 (conn)
+         949         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         957         216 LOAD_FAST                1 (conn)
+         950         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              5 (commit)
                      240 PRECALL                  0
                      244 CALL                     0
                      254 POP_TOP
          
-         942         256 LOAD_CONST               0 (None)
+         935         256 LOAD_CONST               0 (None)
                      258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 PRECALL                  2
                      266 CALL                     2
                      276 POP_TOP
                      278 LOAD_CONST               0 (None)
                      280 RETURN_VALUE
@@ -4752,15 +4764,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('event_id', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'mute_event'
-         firstlineno 940
+         firstlineno 933
          lnotab 0x020234011801160102ff0e0904ff02f7100d4e0128f1
       'comment_id'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -4772,58 +4784,58 @@
             0064027c006901a6020000ab02000000000000000001007c01a002000000
             00000000000000000000000000000000007407000000000000000000006a
             0400000000000000006403a6010000ab010000000000000000a6010000ab
             01000000000000000001007c01a005000000000000000000000000000000
             0000000000a6000000ab0000000000000000000100640064006400a60200
             00ab02000000000000000001006400530023003100730477027803590077
             01010059000100010064005300
-         963           0 RESUME                   0
+         956           0 RESUME                   0
          
-         964           2 LOAD_GLOBAL              0 (db)
+         957           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         965          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
+         958          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         969          58 LOAD_FAST                1 (conn)
+         962          58 LOAD_FAST                1 (conn)
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
          
-         970         142 LOAD_FAST                1 (conn)
+         963         142 LOAD_FAST                1 (conn)
                      144 LOAD_METHOD              2 (execute)
                      166 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      178 LOAD_ATTR                4 (text)
                      188 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      190 PRECALL                  1
                      194 CALL                     1
                      204 PRECALL                  1
                      208 CALL                     1
                      218 POP_TOP
          
-         971         220 LOAD_FAST                1 (conn)
+         964         220 LOAD_FAST                1 (conn)
                      222 LOAD_METHOD              5 (commit)
                      244 PRECALL                  0
                      248 CALL                     0
                      258 POP_TOP
          
-         964         260 LOAD_CONST               0 (None)
+         957         260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 LOAD_CONST               0 (None)
                      266 PRECALL                  2
                      270 CALL                     2
                      280 POP_TOP
                      282 LOAD_CONST               0 (None)
                      284 RETURN_VALUE
@@ -4851,15 +4863,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('comment_id', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'delete_comment'
-         firstlineno 963
+         firstlineno 956
          lnotab 0x02013401040454014e0128f9
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4872,71 +4884,71 @@
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00200000000000000000000000000000000000000
             007407000000000000000000006a0400000000000000006404a6010000ab
             010000000000000000a6010000ab01000000000000000001007c01a00500
             00000000000000000000000000000000000000a6000000ab000000000000
             0000000100640064006400a6020000ab0200000000000000000100640053
             002300310073047702780359007701010059000100010064005300
-         974           0 RESUME                   0
+         967           0 RESUME                   0
          
-         978           2 LOAD_GLOBAL              0 (db)
+         971           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         979          54 LOAD_FAST                1 (conn)
+         972          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         980          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         973          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         981         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
+         974         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
          
-         980         102 PRECALL                  1
+         973         102 PRECALL                  1
                      106 CALL                     1
          
-         987         116 LOAD_CONST               2 ('search_uid')
+         980         116 LOAD_CONST               2 ('search_uid')
                      118 LOAD_FAST                0 (search_uid)
                      120 BUILD_MAP                1
          
-         979         122 PRECALL                  2
+         972         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         989         138 LOAD_FAST                1 (conn)
+         982         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         990         216 LOAD_FAST                1 (conn)
+         983         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              2 (execute)
                      240 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      252 LOAD_ATTR                4 (text)
                      262 LOAD_CONST               4 ('REFRESH MATERIALIZED VIEW rating')
                      264 PRECALL                  1
                      268 CALL                     1
                      278 PRECALL                  1
                      282 CALL                     1
                      292 POP_TOP
          
-         993         294 LOAD_FAST                1 (conn)
+         986         294 LOAD_FAST                1 (conn)
                      296 LOAD_METHOD              5 (commit)
                      318 PRECALL                  0
                      322 CALL                     0
                      332 POP_TOP
          
-         978         334 LOAD_CONST               0 (None)
+         971         334 LOAD_CONST               0 (None)
                      336 LOAD_CONST               0 (None)
                      338 LOAD_CONST               0 (None)
                      340 PRECALL                  2
                      344 CALL                     2
                      354 POP_TOP
                      356 LOAD_CONST               0 (None)
                      358 RETURN_VALUE
@@ -4965,23 +4977,23 @@
             'REFRESH MATERIALIZED VIEW rating'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('search_uid', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'reset_inbox'
-         firstlineno 974
+         firstlineno 967
          lnotab 0x020434011801160102ff0e0706f8100a4e014e0328f1
       (True, None, 'create')
-   names      ('hashlib', 'json', 'dataclasses', 'asdict', 'time', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'gandai', 'ts', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_event', 'models', 'insert_company', 'insert_actor', 'insert_search', 'important_targets_from_search', 'important_targets_from_event', 'int', 'str', 'bool', 'insert_companies_as_targets', 'DataFrame', 'searches_query', 'average_rating_per_search_query', 'validation_history', 'searches_comment_counts', 'enriched_searches_query', 'actor', 'buyer', 'search_targets', 'search_comments', 'event', 'event_history', 'search_criteria_history', 'find_search', 'find_search_by_label', 'find_search_by_token', 'find_company_by_domain', 'find_actor_by_email', 'find_event_by_id', 'update_company', 'update_search', 'mute_event', 'delete_comment', 'reset_inbox')
+   names      ('hashlib', 'json', 'dataclasses', 'asdict', 'time', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'gandai', 'ts', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_event', 'models', 'insert_company', 'insert_actor', 'insert_search', 'str', 'important_targets_from_search', 'important_targets_from_event', 'int', 'bool', 'insert_companies_as_targets', 'DataFrame', 'searches_query', 'average_rating_per_search_query', 'validation_history', 'searches_comment_counts', 'enriched_searches_query', 'actor', 'buyer', 'search_targets', 'search_comments', 'event', 'event_history', 'search_criteria_history', 'find_search', 'find_search_by_label', 'find_search_by_token', 'find_company_by_domain', 'find_actor_by_email', 'find_event_by_id', 'update_company', 'update_search', 'mute_event', 'delete_comment', 'reset_inbox')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080108010c010c011002080108010c010c02140208010c010c
-      011c021406101e240e100f1010020116ff020116ff020202fe082e244c02
-      01020102fa04010eff020202fe020302fd020402fc020502fb020602fa02
-      0702f908611620060c162b06140614160e16610c7f00071a161a0c1a1e1a
-      1d241824182409101010101013101d10171017100b
+      011c021406101e240e100f1010020116ff020116ff020102ff020202fe08
+      27244c0201020102fa04010eff020202fe020302fd020402fc020502fb02
+      0602fa020702f908611620060c162b06140614160e16610c7f00071a161a
+      0c1a1e1a1d241824182409101010101013101d10171017100b
```

### Comparing `gandai-1.7.57/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/__pycache__/tasks.cpython-311.pyc` & `gandai-1.7.58/gandai/__pycache__/tasks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/analytics.py` & `gandai-1.7.58/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/constants.py` & `gandai-1.7.58/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/db.py` & `gandai-1.7.58/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/google.py` & `gandai-1.7.58/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/gpt.py` & `gandai-1.7.58/gandai/gpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -659,15 +659,14 @@
 
 HEADERS = {
     "Authorization": secrets.access_secret_version("GRATA_API_TOKEN"),
     "Content-Type": "application/json",
 }
 
 
-
 messages = [
         {
             "role": "system",
             "content": HOW_TO_SEARCH_GRATA_API
         },
         
         {
```

### Comparing `gandai-1.7.57/gandai/grata.py` & `gandai-1.7.58/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/helpers.py` & `gandai-1.7.58/gandai/helpers.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/main.py` & `gandai-1.7.58/gandai/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
     elif event.type == "import":
         ts.query.important_targets_from_event(event=event)
 
     elif event.type == "import_searches":
         for label in event.data["searches"]:
             from_search = ts.query.find_search_by_label(label=label)
             ts.query.important_targets_from_search(
-                from_search=from_search, to_search=search
+                from_search=from_search, to_search=search, actor_key=event.actor_key
             )
 
     elif event.type == "reset":
         print("💣 Resetting Inbox...")
         ts.query.reset_inbox(search_uid=search.uid)
 
     elif event.type == "rating":
```

### Comparing `gandai-1.7.57/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.58/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/migrations/db_seed.py` & `gandai-1.7.58/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/migrations/dealcloud.py` & `gandai-1.7.58/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.58/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/migrations/sql/schema.sql` & `gandai-1.7.58/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/models.py` & `gandai-1.7.58/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/query.py` & `gandai-1.7.58/gandai/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,57 +94,50 @@
         obj["meta"] = json.dumps(obj["meta"])
         con.execute(statement, obj)
         con.commit()
     return search
 
 
 def important_targets_from_search(
-    from_search: ts.models.Search, to_search: ts.models.Search
+    from_search: ts.models.Search, to_search: ts.models.Search, actor_key: str
 ) -> None:
 
     # import pdb
 
     # pdb.set_trace()
     targets = search_targets(search_uid=from_search.uid)
     targets = targets[targets["stage"] != "reject"]
+    targets = targets[targets["stage"] != "create"]
+    print(targets)
     domains: list = targets["domain"].tolist()
     print(len(domains))
 
-    # stage_dict = targets.set_index("domain")["stage"].to_dict()
-
-    new_event_ids = []
     with db.connect() as con:
         with con.begin():
-            for domain in domains:
-                # should these be in same transaction?
-                domain = ts.helpers.clean_domain(domain)
-
-                result = con.execute(
-                    sqlalchemy.text(
-                        """
-                        INSERT INTO event (search_uid, domain, actor_key, type) 
-                        VALUES(:search_uid, :domain, :actor_key, :type)
-                        ON CONFLICT DO NOTHING
-                        RETURNING id
-                        """
-                    ),
-                    {
-                        "search_uid": to_search.uid,
-                        "actor_key": "chatgpt",
-                        "domain": domain,
-                        "type": "land",
-                    },
-                )
-
-                new_event_id = result.scalar_one()
-                if new_event_id is not None:
-                    new_event_ids.append(new_event_id)
-
-    for event_id in new_event_ids:
-        ts.trigger_process_event(event_id=event_id)
+            events = [
+                {
+                    "search_uid": to_search.uid,
+                    "domain": domain,  # Assuming domain is cleaned and prepared before this step
+                    "actor_key": actor_key,
+                    "type": "land",
+                }
+                for domain in domains
+            ]
+
+            result = con.execute(
+                sqlalchemy.text(
+                    """
+                    INSERT INTO event (search_uid, domain, actor_key, type) 
+                    VALUES (:search_uid, :domain, :actor_key, :type)
+                    ON CONFLICT DO NOTHING
+                    RETURNING id
+                    """
+                ),
+                events,  # Passing the list of dictionaries directly
+            )
 
 
 def important_targets_from_event(event: ts.models.Event) -> None:
 
     source = event.data.get("source")
     targets = search_targets(search_uid=event.search_uid)
     stage_dict = targets.set_index("domain")["stage"].to_dict()
```

### Comparing `gandai-1.7.57/gandai/secrets.py` & `gandai-1.7.58/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai/tasks.py` & `gandai-1.7.58/gandai/tasks.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.57/gandai.egg-info/SOURCES.txt` & `gandai-1.7.58/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

