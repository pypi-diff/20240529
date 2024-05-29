# Comparing `tmp/csle_base-0.6.1.tar.gz` & `tmp/csle_base-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_base-0.6.1.tar", last modified: Thu May 23 18:34:57 2024, max compression
+gzip compressed data, was "csle_base-0.6.2.tar", last modified: Tue May 28 16:30:04 2024, max compression
```

## Comparing `csle_base-0.6.1.tar` & `csle_base-0.6.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:34:57.506679 csle_base-0.6.1/
--rw-r--r--   0 kim        (501) staff       (20)      653 2024-05-23 18:34:57.506720 csle_base-0.6.1/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     3716 2024-02-13 12:24:16.000000 csle_base-0.6.1/README.md
--rw-r--r--   0 kim        (501) staff       (20)      670 2023-08-15 10:44:03.000000 csle_base-0.6.1/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     1671 2024-05-23 18:34:57.506948 csle_base-0.6.1/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_base-0.6.1/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:34:57.504815 csle_base-0.6.1/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:34:57.505727 csle_base-0.6.1/src/csle_base/
--rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_base-0.6.1/src/csle_base/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 18:34:56.000000 csle_base-0.6.1/src/csle_base/__version__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:34:57.506587 csle_base-0.6.1/src/csle_base/encoding/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-14 08:14:52.000000 csle_base-0.6.1/src/csle_base/encoding/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)      571 2023-09-14 08:14:52.000000 csle_base-0.6.1/src/csle_base/encoding/np_encoder.py
--rw-r--r--   0 kim        (501) staff       (20)      574 2023-08-15 10:44:03.000000 csle_base-0.6.1/src/csle_base/grpc_serializable.py
--rw-r--r--   0 kim        (501) staff       (20)     2017 2023-09-14 08:14:52.000000 csle_base-0.6.1/src/csle_base/json_serializable.py
--rw-r--r--   0 kim        (501) staff       (20)      713 2023-08-15 10:44:03.000000 csle_base-0.6.1/src/csle_base/kafka_serializable.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:34:57.506419 csle_base-0.6.1/src/csle_base.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      653 2024-05-23 18:34:57.000000 csle_base-0.6.1/src/csle_base.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)      496 2024-05-23 18:34:57.000000 csle_base-0.6.1/src/csle_base.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 18:34:57.000000 csle_base-0.6.1/src/csle_base.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:18.000000 csle_base-0.6.1/src/csle_base.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      439 2024-05-23 18:34:57.000000 csle_base-0.6.1/src/csle_base.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)       10 2024-05-23 18:34:57.000000 csle_base-0.6.1/src/csle_base.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:04.702633 csle_base-0.6.2/
+-rw-r--r--   0 kim        (501) staff       (20)      653 2024-05-28 16:30:04.702674 csle_base-0.6.2/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     3716 2024-02-13 12:24:16.000000 csle_base-0.6.2/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      670 2023-08-15 10:44:03.000000 csle_base-0.6.2/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1671 2024-05-28 16:30:04.702909 csle_base-0.6.2/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_base-0.6.2/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:04.699722 csle_base-0.6.2/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:04.701394 csle_base-0.6.2/src/csle_base/
+-rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_base-0.6.2/src/csle_base/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-28 16:30:03.000000 csle_base-0.6.2/src/csle_base/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:04.702366 csle_base-0.6.2/src/csle_base/encoding/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-14 08:14:52.000000 csle_base-0.6.2/src/csle_base/encoding/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)      571 2023-09-14 08:14:52.000000 csle_base-0.6.2/src/csle_base/encoding/np_encoder.py
+-rw-r--r--   0 kim        (501) staff       (20)      574 2023-08-15 10:44:03.000000 csle_base-0.6.2/src/csle_base/grpc_serializable.py
+-rw-r--r--   0 kim        (501) staff       (20)     2017 2023-09-14 08:14:52.000000 csle_base-0.6.2/src/csle_base/json_serializable.py
+-rw-r--r--   0 kim        (501) staff       (20)      713 2023-08-15 10:44:03.000000 csle_base-0.6.2/src/csle_base/kafka_serializable.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:04.702170 csle_base-0.6.2/src/csle_base.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      653 2024-05-28 16:30:04.000000 csle_base-0.6.2/src/csle_base.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      496 2024-05-28 16:30:04.000000 csle_base-0.6.2/src/csle_base.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-28 16:30:04.000000 csle_base-0.6.2/src/csle_base.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:18.000000 csle_base-0.6.2/src/csle_base.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      439 2024-05-28 16:30:04.000000 csle_base-0.6.2/src/csle_base.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       10 2024-05-28 16:30:04.000000 csle_base-0.6.2/src/csle_base.egg-info/top_level.txt
```

### Comparing `csle_base-0.6.1/PKG-INFO` & `csle_base-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_base
-Version: 0.6.1
+Version: 0.6.2
 Summary: Library with base classes and definitions for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_base-0.6.1/README.md` & `csle_base-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `csle_base-0.6.1/pyproject.toml` & `csle_base-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_base-0.6.1/setup.cfg` & `csle_base-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `csle_base-0.6.1/src/csle_base/encoding/np_encoder.py` & `csle_base-0.6.2/src/csle_base/encoding/np_encoder.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.6.1/src/csle_base/grpc_serializable.py` & `csle_base-0.6.2/src/csle_base/grpc_serializable.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.6.1/src/csle_base/json_serializable.py` & `csle_base-0.6.2/src/csle_base/json_serializable.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.6.1/src/csle_base/kafka_serializable.py` & `csle_base-0.6.2/src/csle_base/kafka_serializable.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.6.1/src/csle_base.egg-info/PKG-INFO` & `csle_base-0.6.2/src/csle_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-base
-Version: 0.6.1
+Version: 0.6.2
 Summary: Library with base classes and definitions for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

