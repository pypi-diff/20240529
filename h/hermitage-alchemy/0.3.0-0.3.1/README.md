# Comparing `tmp/hermitage_alchemy-0.3.0.tar.gz` & `tmp/hermitage_alchemy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage_alchemy-0.3.0.tar", max compression
+gzip compressed data, was "hermitage_alchemy-0.3.1.tar", max compression
```

## Comparing `hermitage_alchemy-0.3.0.tar` & `hermitage_alchemy-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.3.0/README.md
--rw-r--r--   0        0        0      504 2024-05-25 14:24:50.954908 hermitage_alchemy-0.3.0/hermitage_alchemy/__init__.py
--rw-r--r--   0        0        0    10393 2024-05-28 08:51:26.557813 hermitage_alchemy-0.3.0/hermitage_alchemy/assembling.py
--rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.3.0/hermitage_alchemy/bootstraping.py
--rw-r--r--   0        0        0     7409 2024-05-27 18:32:27.541366 hermitage_alchemy-0.3.0/hermitage_alchemy/configuration.py
--rw-r--r--   0        0        0       24 2024-05-25 14:24:50.956586 hermitage_alchemy-0.3.0/hermitage_alchemy/definition/__init__.py
--rw-r--r--   0        0        0      718 2024-05-26 13:12:45.022518 hermitage_alchemy-0.3.0/hermitage_alchemy/definition/contracts.py
--rw-r--r--   0        0        0       60 2024-05-25 14:24:50.957143 hermitage_alchemy-0.3.0/hermitage_alchemy/execution/__init__.py
--rw-r--r--   0        0        0     6987 2024-05-28 08:51:26.552502 hermitage_alchemy-0.3.0/hermitage_alchemy/execution/read.py
--rw-r--r--   0        0        0     1840 2024-05-27 17:39:40.830848 hermitage_alchemy-0.3.0/hermitage_alchemy/execution/write.py
--rw-r--r--   0        0        0      415 2024-05-28 08:31:33.385070 hermitage_alchemy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 hermitage_alchemy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.3.1/README.md
+-rw-r--r--   0        0        0      524 2024-05-28 09:17:37.633261 hermitage_alchemy-0.3.1/hermitage_alchemy/__init__.py
+-rw-r--r--   0        0        0    10393 2024-05-28 08:51:26.557813 hermitage_alchemy-0.3.1/hermitage_alchemy/assembling.py
+-rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.3.1/hermitage_alchemy/bootstraping.py
+-rw-r--r--   0        0        0     7409 2024-05-27 18:32:27.541366 hermitage_alchemy-0.3.1/hermitage_alchemy/configuration.py
+-rw-r--r--   0        0        0       24 2024-05-25 14:24:50.956586 hermitage_alchemy-0.3.1/hermitage_alchemy/definition/__init__.py
+-rw-r--r--   0        0        0      718 2024-05-26 13:12:45.022518 hermitage_alchemy-0.3.1/hermitage_alchemy/definition/contracts.py
+-rw-r--r--   0        0        0       60 2024-05-25 14:24:50.957143 hermitage_alchemy-0.3.1/hermitage_alchemy/execution/__init__.py
+-rw-r--r--   0        0        0     6987 2024-05-28 08:51:26.552502 hermitage_alchemy-0.3.1/hermitage_alchemy/execution/read.py
+-rw-r--r--   0        0        0     1840 2024-05-27 17:39:40.830848 hermitage_alchemy-0.3.1/hermitage_alchemy/execution/write.py
+-rw-r--r--   0        0        0       20 2024-05-28 09:17:37.627547 hermitage_alchemy-0.3.1/hermitage_alchemy/types/__init__.py
+-rw-r--r--   0        0        0       58 2024-01-11 09:14:13.699423 hermitage_alchemy-0.3.1/hermitage_alchemy/types/jsonb/__init__.py
+-rw-r--r--   0        0        0      538 2024-01-11 09:14:13.699814 hermitage_alchemy-0.3.1/hermitage_alchemy/types/jsonb/decoding.py
+-rw-r--r--   0        0        0      631 2024-05-28 09:17:37.603101 hermitage_alchemy-0.3.1/hermitage_alchemy/types/jsonb/encoding.py
+-rw-r--r--   0        0        0      415 2024-05-28 09:19:53.351453 hermitage_alchemy-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 hermitage_alchemy-0.3.1/PKG-INFO
```

### Comparing `hermitage_alchemy-0.3.0/hermitage_alchemy/assembling.py` & `hermitage_alchemy-0.3.1/hermitage_alchemy/assembling.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.3.0/hermitage_alchemy/bootstraping.py` & `hermitage_alchemy-0.3.1/hermitage_alchemy/bootstraping.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.3.0/hermitage_alchemy/configuration.py` & `hermitage_alchemy-0.3.1/hermitage_alchemy/configuration.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.3.0/hermitage_alchemy/definition/contracts.py` & `hermitage_alchemy-0.3.1/hermitage_alchemy/definition/contracts.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.3.0/hermitage_alchemy/execution/read.py` & `hermitage_alchemy-0.3.1/hermitage_alchemy/execution/read.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.3.0/hermitage_alchemy/execution/write.py` & `hermitage_alchemy-0.3.1/hermitage_alchemy/execution/write.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.3.0/PKG-INFO` & `hermitage_alchemy-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermitage-alchemy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Implementation of hermitage contracts for sqlalchemy engine
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

