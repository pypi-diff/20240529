# Comparing `tmp/surrealist-0.5.1.tar.gz` & `tmp/surrealist-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surrealist-0.5.1.tar", last modified: Sun May 19 16:07:06 2024, max compression
+gzip compressed data, was "surrealist-0.5.2.tar", last modified: Wed May 29 11:42:21 2024, max compression
```

## Comparing `surrealist-0.5.1.tar` & `surrealist-0.5.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.366100 surrealist-0.5.1/
--rw-rw-rw-   0        0        0     1091 2024-02-04 05:55:53.000000 surrealist-0.5.1/LICENSE
--rw-rw-rw-   0        0        0    31133 2024-05-19 16:07:06.365100 surrealist-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    29123 2024-05-19 16:06:48.000000 surrealist-0.5.1/README.md
--rw-rw-rw-   0        0        0      905 2024-05-19 16:06:48.000000 surrealist-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-19 16:07:06.366100 surrealist-0.5.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.315129 surrealist-0.5.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.324100 surrealist-0.5.1/src/surrealist/
--rw-rw-rw-   0        0        0      849 2024-04-20 09:05:50.000000 surrealist-0.5.1/src/surrealist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.331100 surrealist-0.5.1/src/surrealist/clients/
--rw-rw-rw-   0        0        0      124 2024-02-04 05:55:53.000000 surrealist-0.5.1/src/surrealist/clients/__init__.py
--rw-rw-rw-   0        0        0     5044 2024-02-16 16:27:45.000000 surrealist-0.5.1/src/surrealist/clients/http_client.py
--rw-rw-rw-   0        0        0     8117 2024-02-16 16:26:19.000000 surrealist-0.5.1/src/surrealist/clients/ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.337100 surrealist-0.5.1/src/surrealist/connections/
--rw-rw-rw-   0        0        0      198 2024-02-04 05:55:53.000000 surrealist-0.5.1/src/surrealist/connections/__init__.py
--rw-rw-rw-   0        0        0    19339 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/connections/connection.py
--rw-rw-rw-   0        0        0    27023 2024-03-14 16:05:03.000000 surrealist-0.5.1/src/surrealist/connections/http_connection.py
--rw-rw-rw-   0        0        0     8023 2024-04-14 06:04:00.000000 surrealist-0.5.1/src/surrealist/connections/pool.py
--rw-rw-rw-   0        0        0    29659 2024-04-14 06:04:00.000000 surrealist-0.5.1/src/surrealist/connections/ws_connection.py
--rw-rw-rw-   0        0        0     2439 2024-03-14 15:59:51.000000 surrealist-0.5.1/src/surrealist/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.341100 surrealist-0.5.1/src/surrealist/ql/
--rw-rw-rw-   0        0        0      231 2024-03-02 11:31:18.000000 surrealist-0.5.1/src/surrealist/ql/__init__.py
--rw-rw-rw-   0        0        0    16349 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/database.py
--rw-rw-rw-   0        0        0     3135 2024-03-02 11:31:18.000000 surrealist-0.5.1/src/surrealist/ql/pool_database.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.363100 surrealist-0.5.1/src/surrealist/ql/statements/
--rw-rw-rw-   0        0        0      530 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/statements/__init__.py
--rw-rw-rw-   0        0        0     2909 2024-02-11 13:05:41.000000 surrealist-0.5.1/src/surrealist/ql/statements/common_statements.py
--rw-rw-rw-   0        0        0     1518 2024-02-12 10:41:24.000000 surrealist-0.5.1/src/surrealist/ql/statements/create.py
--rw-rw-rw-   0        0        0     1282 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/statements/create_statements.py
--rw-rw-rw-   0        0        0    15489 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/define.py
--rw-rw-rw-   0        0        0    14628 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/define_index_statements.py
--rw-rw-rw-   0        0        0     1213 2024-02-19 06:12:19.000000 surrealist-0.5.1/src/surrealist/ql/statements/delete.py
--rw-rw-rw-   0        0        0     2409 2024-02-19 06:14:54.000000 surrealist-0.5.1/src/surrealist/ql/statements/insert.py
--rw-rw-rw-   0        0        0      937 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/insert_statements.py
--rw-rw-rw-   0        0        0     3297 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/live.py
--rw-rw-rw-   0        0        0     1951 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/live_statements.py
--rw-rw-rw-   0        0        0     1967 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/permissions.py
--rw-rw-rw-   0        0        0      962 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/statements/rebuild_index.py
--rw-rw-rw-   0        0        0     1377 2024-02-12 10:41:24.000000 surrealist-0.5.1/src/surrealist/ql/statements/relate.py
--rw-rw-rw-   0        0        0     2025 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/remove.py
--rw-rw-rw-   0        0        0      825 2024-02-12 10:41:24.000000 surrealist-0.5.1/src/surrealist/ql/statements/returns.py
--rw-rw-rw-   0        0        0     3190 2024-02-19 06:14:54.000000 surrealist-0.5.1/src/surrealist/ql/statements/select.py
--rw-rw-rw-   0        0        0     8006 2024-02-11 12:57:39.000000 surrealist-0.5.1/src/surrealist/ql/statements/select_statements.py
--rw-rw-rw-   0        0        0     2167 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/statements/show.py
--rw-rw-rw-   0        0        0     1457 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/statements/simple_statements.py
--rw-rw-rw-   0        0        0     3436 2024-02-16 16:23:17.000000 surrealist-0.5.1/src/surrealist/ql/statements/statement.py
--rw-rw-rw-   0        0        0      924 2024-02-19 06:12:19.000000 surrealist-0.5.1/src/surrealist/ql/statements/transaction.py
--rw-rw-rw-   0        0        0     1273 2024-02-19 06:12:19.000000 surrealist-0.5.1/src/surrealist/ql/statements/update.py
--rw-rw-rw-   0        0        0     3667 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/update_statements.py
--rw-rw-rw-   0        0        0      621 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/statements/utils.py
--rw-rw-rw-   0        0        0     9582 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/table.py
--rw-rw-rw-   0        0        0     8695 2024-04-14 06:04:00.000000 surrealist-0.5.1/src/surrealist/result.py
--rw-rw-rw-   0        0        0     9831 2024-05-19 12:47:50.000000 surrealist-0.5.1/src/surrealist/surreal.py
--rw-rw-rw-   0        0        0     2221 2024-04-20 09:05:50.000000 surrealist-0.5.1/src/surrealist/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.364100 surrealist-0.5.1/src/surrealist.egg-info/
--rw-rw-rw-   0        0        0    31133 2024-05-19 16:07:06.000000 surrealist-0.5.1/src/surrealist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1869 2024-05-19 16:07:06.000000 surrealist-0.5.1/src/surrealist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 16:07:06.000000 surrealist-0.5.1/src/surrealist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-19 16:07:06.000000 surrealist-0.5.1/src/surrealist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-19 16:07:06.000000 surrealist-0.5.1/src/surrealist.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 11:42:21.648305 surrealist-0.5.2/
+-rw-rw-rw-   0        0        0     1091 2024-02-04 05:55:53.000000 surrealist-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0    31626 2024-05-29 11:42:21.647305 surrealist-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    29616 2024-05-29 11:41:30.000000 surrealist-0.5.2/README.md
+-rw-rw-rw-   0        0        0      905 2024-05-29 11:41:30.000000 surrealist-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:42:21.648305 surrealist-0.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 11:42:21.590154 surrealist-0.5.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 11:42:21.601184 surrealist-0.5.2/src/surrealist/
+-rw-rw-rw-   0        0        0      875 2024-05-29 11:41:30.000000 surrealist-0.5.2/src/surrealist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:42:21.609154 surrealist-0.5.2/src/surrealist/clients/
+-rw-rw-rw-   0        0        0      124 2024-02-04 05:55:53.000000 surrealist-0.5.2/src/surrealist/clients/__init__.py
+-rw-rw-rw-   0        0        0     5056 2024-05-29 11:41:30.000000 surrealist-0.5.2/src/surrealist/clients/http_client.py
+-rw-rw-rw-   0        0        0     8129 2024-05-29 11:41:30.000000 surrealist-0.5.2/src/surrealist/clients/ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:42:21.615185 surrealist-0.5.2/src/surrealist/connections/
+-rw-rw-rw-   0        0        0      198 2024-02-04 05:55:53.000000 surrealist-0.5.2/src/surrealist/connections/__init__.py
+-rw-rw-rw-   0        0        0    19350 2024-05-29 11:41:30.000000 surrealist-0.5.2/src/surrealist/connections/connection.py
+-rw-rw-rw-   0        0        0    27035 2024-05-29 11:41:30.000000 surrealist-0.5.2/src/surrealist/connections/http_connection.py
+-rw-rw-rw-   0        0        0     7995 2024-05-29 11:41:30.000000 surrealist-0.5.2/src/surrealist/connections/pool.py
+-rw-rw-rw-   0        0        0    29671 2024-05-29 11:41:30.000000 surrealist-0.5.2/src/surrealist/connections/ws_connection.py
+-rw-rw-rw-   0        0        0     2439 2024-03-14 15:59:51.000000 surrealist-0.5.2/src/surrealist/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:42:21.619183 surrealist-0.5.2/src/surrealist/ql/
+-rw-rw-rw-   0        0        0      231 2024-03-02 11:31:18.000000 surrealist-0.5.2/src/surrealist/ql/__init__.py
+-rw-rw-rw-   0        0        0    16323 2024-05-29 11:41:30.000000 surrealist-0.5.2/src/surrealist/ql/database.py
+-rw-rw-rw-   0        0        0     3072 2024-05-29 11:41:30.000000 surrealist-0.5.2/src/surrealist/ql/pool_database.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:42:21.645305 surrealist-0.5.2/src/surrealist/ql/statements/
+-rw-rw-rw-   0        0        0      530 2024-05-15 11:06:07.000000 surrealist-0.5.2/src/surrealist/ql/statements/__init__.py
+-rw-rw-rw-   0        0        0     2909 2024-02-11 13:05:41.000000 surrealist-0.5.2/src/surrealist/ql/statements/common_statements.py
+-rw-rw-rw-   0        0        0     1518 2024-02-12 10:41:24.000000 surrealist-0.5.2/src/surrealist/ql/statements/create.py
+-rw-rw-rw-   0        0        0     1282 2024-05-15 11:06:07.000000 surrealist-0.5.2/src/surrealist/ql/statements/create_statements.py
+-rw-rw-rw-   0        0        0    15489 2024-05-19 16:06:48.000000 surrealist-0.5.2/src/surrealist/ql/statements/define.py
+-rw-rw-rw-   0        0        0    14628 2024-05-19 16:06:48.000000 surrealist-0.5.2/src/surrealist/ql/statements/define_index_statements.py
+-rw-rw-rw-   0        0        0     1213 2024-02-19 06:12:19.000000 surrealist-0.5.2/src/surrealist/ql/statements/delete.py
+-rw-rw-rw-   0        0        0     2409 2024-02-19 06:14:54.000000 surrealist-0.5.2/src/surrealist/ql/statements/insert.py
+-rw-rw-rw-   0        0        0      937 2024-05-19 16:06:48.000000 surrealist-0.5.2/src/surrealist/ql/statements/insert_statements.py
+-rw-rw-rw-   0        0        0     3297 2024-05-19 16:06:48.000000 surrealist-0.5.2/src/surrealist/ql/statements/live.py
+-rw-rw-rw-   0        0        0     1951 2024-05-19 16:06:48.000000 surrealist-0.5.2/src/surrealist/ql/statements/live_statements.py
+-rw-rw-rw-   0        0        0     1967 2024-05-19 16:06:48.000000 surrealist-0.5.2/src/surrealist/ql/statements/permissions.py
+-rw-rw-rw-   0        0        0      962 2024-05-15 11:06:07.000000 surrealist-0.5.2/src/surrealist/ql/statements/rebuild_index.py
+-rw-rw-rw-   0        0        0     1377 2024-02-12 10:41:24.000000 surrealist-0.5.2/src/surrealist/ql/statements/relate.py
+-rw-rw-rw-   0        0        0     2025 2024-05-19 16:06:48.000000 surrealist-0.5.2/src/surrealist/ql/statements/remove.py
+-rw-rw-rw-   0        0        0      825 2024-02-12 10:41:24.000000 surrealist-0.5.2/src/surrealist/ql/statements/returns.py
+-rw-rw-rw-   0        0        0     3190 2024-02-19 06:14:54.000000 surrealist-0.5.2/src/surrealist/ql/statements/select.py
+-rw-rw-rw-   0        0        0     8006 2024-02-11 12:57:39.000000 surrealist-0.5.2/src/surrealist/ql/statements/select_statements.py
+-rw-rw-rw-   0        0        0     2167 2024-05-15 11:06:07.000000 surrealist-0.5.2/src/surrealist/ql/statements/show.py
+-rw-rw-rw-   0        0        0     1457 2024-05-15 11:06:07.000000 surrealist-0.5.2/src/surrealist/ql/statements/simple_statements.py
+-rw-rw-rw-   0        0        0     3436 2024-02-16 16:23:17.000000 surrealist-0.5.2/src/surrealist/ql/statements/statement.py
+-rw-rw-rw-   0        0        0      924 2024-02-19 06:12:19.000000 surrealist-0.5.2/src/surrealist/ql/statements/transaction.py
+-rw-rw-rw-   0        0        0     1273 2024-02-19 06:12:19.000000 surrealist-0.5.2/src/surrealist/ql/statements/update.py
+-rw-rw-rw-   0        0        0     3667 2024-05-19 16:06:48.000000 surrealist-0.5.2/src/surrealist/ql/statements/update_statements.py
+-rw-rw-rw-   0        0        0      621 2024-05-15 11:06:07.000000 surrealist-0.5.2/src/surrealist/ql/statements/utils.py
+-rw-rw-rw-   0        0        0     9582 2024-05-15 11:06:07.000000 surrealist-0.5.2/src/surrealist/ql/table.py
+-rw-rw-rw-   0        0        0     8696 2024-05-29 11:41:30.000000 surrealist-0.5.2/src/surrealist/result.py
+-rw-rw-rw-   0        0        0     8173 2024-05-29 11:41:30.000000 surrealist-0.5.2/src/surrealist/surreal.py
+-rw-rw-rw-   0        0        0     2326 2024-05-29 11:41:30.000000 surrealist-0.5.2/src/surrealist/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:42:21.646305 surrealist-0.5.2/src/surrealist.egg-info/
+-rw-rw-rw-   0        0        0    31626 2024-05-29 11:42:21.000000 surrealist-0.5.2/src/surrealist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1869 2024-05-29 11:42:21.000000 surrealist-0.5.2/src/surrealist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:42:21.000000 surrealist-0.5.2/src/surrealist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-29 11:42:21.000000 surrealist-0.5.2/src/surrealist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 11:42:21.000000 surrealist-0.5.2/src/surrealist.egg-info/top_level.txt
```

### Comparing `surrealist-0.5.1/LICENSE` & `surrealist-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/PKG-INFO` & `surrealist-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surrealist
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python client for SurrealDB, latest SurrealDB version compatible, all features supported
 Author-email: kotolex <farofwell@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,27 +34,27 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: websocket-client
 
 # README #
 
-Surrealist is a Python tool to work with awesome [SurrealDB](https://docs.surrealdb.com/docs/intro) (support for latest version 1.5.0)
+Surrealist is a Python tool to work with awesome [SurrealDB](https://docs.surrealdb.com/docs/intro) (support for latest version 1.5.1)
 
 It is **synchronous** and **unofficial**, so if you need async AND/OR official client, go [here](https://github.com/surrealdb/surrealdb.py)
 
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
  * only one small dependency (websocket-client), no need to pull a lot of libraries to your project
  * fully documented
  * well tested (on the latest Ubuntu, macOS and Windows 10)
- * fully compatible with the latest version of SurrealDB (1.5.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
- * debug mode to see all that goes in and out if you need
+ * fully compatible with the latest version of SurrealDB (1.5.1), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
+ * debug mode to see all that goes in and out if you need (using standard logging)
  * iterator to handle big select queries
  * QL-builder to explore, generate and use SurrealDB queries (explain, transaction etc.)
  * connections pool for use at a high load
  * http or websocket transport to use
  * always up to date with SurrealDB features and changes
 
 
@@ -92,17 +92,17 @@
 
 In this example, we explicitly show all parameters, but remember many of them are optional
 
 ```python
 from surrealist import Surreal
 
 # we create a surreal object, it can be used to create one or more connections with websockets (use_http=False)
-# with timeout 10 seconds and ERROR logging level
+# with timeout 10 seconds
 surreal = Surreal("http://127.0.0.1:8000", namespace="test", database="test", credentials=("root", "root"),
-                  use_http=False, timeout=10, log_level="ERROR")
+                  use_http=False, timeout=10)
 print(surreal.is_ready())  # prints True if server up and running on that url
 print(surreal.version())  # prints server version
 ```
 **Note:** create of a Surreal object does not attempt any connections or other actions, just store parameters for future use
 
 Calls of **is_ready()**, **health()** or **version()** on Surreal objects are for server checks only, these not validate or check your namespace, database or credentials.
 
@@ -121,25 +121,24 @@
 
 **credentials** - optional, pair(tuple) of username and password for SurrealDB
 
 **use_http** - optional, False by default, flag of using websockets or http transport, False mean using websocket, specify True if you want to use http transport
 
 **timeout** - optional, 5 seconds by default, it is time in seconds to wait for responses and messages, time for trying to connect to SurrealDB
 
-**log_level** - optional, "ERROR" by default, one of (DEBUG, INFO, ERROR), where ERROR - to see only errors, INFO—to see errors and operations, DEBUG—to see all, including transport requests/responses
 
 **Example 2**
 
 In this example, we do not use default(optional) parameters
 
 ```python
 from surrealist import Surreal
 
 # we create a surreal object, it can be used to create one or more connections with websockets
-# with timeout 5 seconds and ERROR logging level
+# with timeout 15 seconds
 surreal = Surreal("http://127.0.0.1:8000")
 print(surreal.is_ready())  # prints True if server up and running on that url
 print(surreal.version())  # prints server version
 ```
 ## Context managers and close ##
 You should always close created connections, when you do not need them anymore, the best way to do it is via context manager
 
@@ -276,60 +275,66 @@
 **Important note for UTF-8:** record_id can have only A-Z, a-z letters, if you want to use any other UTF-8 letters you have to use backticks "`"!
 
 **Note:** record_id parameter of methods is only concatenated with table_name and colon, so
 ws_connection.select("person", record_id="john") under the hood became
 ws_connection.select("person:john"), but no other logic performed. Do not expect we specified "`" for you.
 
 
-## Debug mode ##
-As it was said, if you need to debug something, stuck in some problem or just want to know all about data between you and SurrealDB, you can use log level.
-If you specify "INFO" level, then you will see transport operations, which methods were called, which parameters were used.
+## Logging and Debug mode ##
+As it was said, if you need to debug something, stuck in some problem or just want to know all about data between you and SurrealDB, you can use standard logging.
+All library logs will contain "surrealist" prefix in logs. You, as a developer, should choose proper handlers, formats, filters etc.
+Surrealist does not use root logger, does not use any handlers and uses only DEBUG, INFO and ERROR level for its events.
+
 For example
 
 **Example 7**
 
 ```python
-from surrealist import Surreal
+from logging import basicConfig, INFO, DEBUG
 
-surreal = Surreal("http://127.0.0.1:8000", namespace="test", database="test", credentials=("root", "root"),
-                  log_level="INFO")
+from surrealist import Surreal, LOG_FORMAT  # LOG_FORMAT is used for simplicity, you can use your own
+
+basicConfig(format=LOG_FORMAT, level=INFO)  # we specify a format and level of events to catch
+
+surreal = Surreal("http://127.0.0.1:8000", namespace="test", database="test", credentials=("root", "root"))
 with surreal.connect() as connection:
     res = connection.create("article", {"author": "John Doe", "title": "In memoriam", "text": "text"})
-
 ```
 if you run it, you get in the console:
 ```
-2024-02-02 18:31:09,419 : Thread-1 : websocket : INFO : Websocket connected
-2024-02-02 18:31:09,521 : MainThread : websocket_connection : INFO : Operation: SIGNIN. Data: {'user': 'root', 'pass': '******', 'NS': 'test', 'DB': 'test'}
-2024-02-02 18:31:09,627 : MainThread : websocket_connection : INFO : Got result: SurrealResult(id='836a2834-c6d5-416c-a840-6322a17b47cc', error=None, result='eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MDY4ODA2NjksIm5iZiI6MTcwNjg4MDY2OSwiZXhwIjoxNzA2ODg0MjY5LCJpc3MiOiJTdXJyZWFsREIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRCI6InJvb3QifQ.mrzxXkva3lCg6EihtUEx8c1yjOtuJt_EvJninTqxJ_1...
-2024-02-02 18:31:09,627 : MainThread : websocket_connection : INFO : Connected to ws://127.0.0.1:8000/rpc, params: {'NS': 'test', 'DB': 'test'}, credentials: ('root', '******'), timeout: 5
-2024-02-02 18:31:09,627 : MainThread : websocket_connection : INFO : Operation: CREATE. Path: article, data: {'author': 'John Doe', 'title': 'In memoriam', 'text': 'text'}
-2024-02-02 18:31:09,733 : MainThread : websocket_connection : INFO : Got result: SurrealResult(id='0870492e-faba-4a5f-b454-c7f7315348bd', error=None, result=[{'author': 'John Doe', 'id': 'article:pt0907zkhkhb94evjnze', 'text': 'text', 'title': 'In memoriam'}], code=None, token=None, status='OK', time='')
-2024-02-02 18:31:09,734 : MainThread : connection : INFO : Connection was closed
-```
-but if in example above (example 5) you choose "DEBUG", you will see all, including low-level clients' data:
-```
-2024-02-02 18:33:15,119 : MainThread : root : DEBUG : Log level switch to DEBUG
-2024-02-02 18:33:15,124 : Thread-1 : websocket : INFO : Websocket connected
-2024-02-02 18:33:15,223 : MainThread : websocket_client : DEBUG : Connected to ws://127.0.0.1:8000/rpc, timeout is 5 seconds
-2024-02-02 18:33:15,223 : MainThread : websocket_connection : INFO : Operation: SIGNIN. Data: {'user': 'root', 'pass': '******', 'NS': 'test', 'DB': 'test'}
-2024-02-02 18:33:15,224 : MainThread : websocket_client : DEBUG : Send data: {"id": "5a2e9c12-e03e-4879-a78a-bd360cd871b1", "method": "signin", "params": [{"user": "root", "pass": "******", "NS": "test", "DB": "test"}]}
-2024-02-02 18:33:15,281 : Thread-1 : websocket_client : DEBUG : Get message b'{"id":"5a2e9c12-e03e-4879-a78a-bd360cd871b1","result":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MDY4ODA3OTUsIm5iZiI6MTcwNjg4MDc5NSwiZXhwIjoxNzA2ODg0Mzk1LCJpc3MiOiJTdXJyZWFsREIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRCI6InJvb3QifQ.2ekRL9EyiaWOQR0Aw1qX8VE5S822Kab5SiYLHLC3YkPX3_Yu-FkWSCoP3XGoUg9w8'...
-2024-02-02 18:33:15,326 : MainThread : websocket_connection : INFO : Got result: SurrealResult(id='5a2e9c12-e03e-4879-a78a-bd360cd871b1', error=None, result='eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MDY4ODA3OTUsIm5iZiI6MTcwNjg4MDc5NSwiZXhwIjoxNzA2ODg0Mzk1LCJpc3MiOiJTdXJyZWFsREIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRCI6InJvb3QifQ.2ekRL9EyiaWOQR0Aw1qX8VE5S822Kab5SiYLHLC3YkP...
-2024-02-02 18:33:15,326 : MainThread : websocket_connection : INFO : Connected to ws://127.0.0.1:8000/rpc, params: {'NS': 'test', 'DB': 'test'}, credentials: ('root', '******'), timeout: 5
-2024-02-02 18:33:15,326 : MainThread : websocket_connection : INFO : Operation: CREATE. Path: article, data: {'author': 'John Doe', 'title': 'In memoriam', 'text': 'text'}
-2024-02-02 18:33:15,326 : MainThread : websocket_client : DEBUG : Send data: {"id": "145b2ed4-9b42-44ab-ade2-e28a27730faa", "method": "create", "params": ["article", {"author": "John Doe", "title": "In memoriam", "text": "text"}]}
-2024-02-02 18:33:15,327 : Thread-1 : websocket_client : DEBUG : Get message b'{"id":"145b2ed4-9b42-44ab-ade2-e28a27730faa","result":[{"author":"John Doe","id":"article:s0coora4gedavt2skd36","text":"text","title":"In memoriam"}]}'
-2024-02-02 18:33:15,432 : MainThread : websocket_connection : INFO : Got result: SurrealResult(id='145b2ed4-9b42-44ab-ade2-e28a27730faa', error=None, result=[{'author': 'John Doe', 'id': 'article:s0coora4gedavt2skd36', 'text': 'text', 'title': 'In memoriam'}], code=None, token=None, status='OK', time='')
-2024-02-02 18:33:15,433 : MainThread : connection : INFO : Connection was closed
-2024-02-02 18:33:15,434 : MainThread : websocket_client : DEBUG : Client is closed connection to ws://127.0.0.1:8000/rpc
+2024-05-29 15:59:41,759 : Thread-1 : websocket : INFO : Websocket connected
+2024-05-29 15:59:41,762 : MainThread : surrealist.connections.websocket : INFO : Operation: SIGNIN. Data: {'user': 'root', 'pass': '******', 'NS': 'test', 'DB': 'test'}
+2024-05-29 15:59:41,788 : MainThread : surrealist.connections.websocket : INFO : Got result: SurrealResult(id=c3fcebbc-359f-47d0-822b-a4ad8043f64b, status=OK, result=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MTY5ODAzODEsIm5iZiI6MTcxNjk4MDM4MSwiZXhwIjoxNzE2OTgzOTgxLCJpc3MiOiJTdXJyZWFsREIiLCJqdGkiOiI0YTQyNWFiNy00NGEyLTQ4OGItYjM4MS05YjUyNDQzYTI5OTQiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRC...
+2024-05-29 15:59:41,788 : MainThread : surrealist.connections.websocket : INFO : Connected to ws://127.0.0.1:8000/rpc, params: {'NS': 'test', 'DB': 'test'}, credentials: ('root', '******'), timeout: 15
+2024-05-29 15:59:41,788 : MainThread : surrealist.connections.websocket : INFO : Operation: CREATE. Path: article, data: {'author': 'John Doe', 'title': 'In memoriam', 'text': 'text'}
+2024-05-29 15:59:41,794 : MainThread : surrealist.connections.websocket : INFO : Got result: SurrealResult(id=b307d67f-b01b-4b71-a319-906fa17b8c72, status=OK, result=[{'author': 'John Doe', 'id': 'article:b44tdiiyb8jw6mcn1tzs', 'text': 'text', 'title': 'In memoriam'}], query=None, code=None, time=None, additional_info={})
+2024-05-29 15:59:41,794 : MainThread : surrealist.connection : INFO : The connection was closed
+```
+but if in the example above (example 7) you choose "DEBUG" for level, you will see all, including low-level clients' data:
+```
+2024-05-29 16:03:58,438 : MainThread : surrealist.clients.websocket : DEBUG : Connecting to ws://127.0.0.1:8000/rpc
+2024-05-29 16:03:58,445 : Thread-1 : websocket : INFO : Websocket connected
+2024-05-29 16:03:58,458 : MainThread : surrealist.clients.websocket : DEBUG : Connected to ws://127.0.0.1:8000/rpc, timeout is 15 seconds
+2024-05-29 16:03:58,458 : MainThread : surrealist.connections.websocket : INFO : Operation: SIGNIN. Data: {'user': 'root', 'pass': '******', 'NS': 'test', 'DB': 'test'}
+2024-05-29 16:03:58,458 : MainThread : surrealist.clients.websocket : DEBUG : Send data: {"id": "1d5758bb-0879-4d8d-9e14-37c9117669a3", "method": "signin", "params": [{"user": "root", "pass": "******", "NS": "test", "DB": "test"}]}
+2024-05-29 16:03:58,484 : Thread-1 : surrealist.clients.websocket : DEBUG : Get message b'{"id":"1d5758bb-0879-4d8d-9e14-37c9117669a3","result":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MTY5ODA2MzgsIm5iZiI6MTcxNjk4MDYzOCwiZXhwIjoxNzE2OTg0MjM4LCJpc3MiOiJTdXJyZWFsREIiLCJqdGkiOiIwODhhMWY0My04YzY3LTQ5NjYtYTdjNC02ZGI5NjA0MGNkYmIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRCI6InJvb3QifQ.1pSbJ'...
+2024-05-29 16:03:58,484 : MainThread : surrealist.connections.websocket : INFO : Got result: SurrealResult(id=1d5758bb-0879-4d8d-9e14-37c9117669a3, status=OK, result=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MTY5ODA2MzgsIm5iZiI6MTcxNjk4MDYzOCwiZXhwIjoxNzE2OTg0MjM4LCJpc3MiOiJTdXJyZWFsREIiLCJqdGkiOiIwODhhMWY0My04YzY3LTQ5NjYtYTdjNC02ZGI5NjA0MGNkYmIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRC...
+2024-05-29 16:03:58,484 : MainThread : surrealist.connections.websocket : INFO : Connected to ws://127.0.0.1:8000/rpc, params: {'NS': 'test', 'DB': 'test'}, credentials: ('root', '******'), timeout: 15
+2024-05-29 16:03:58,484 : MainThread : surrealist.connections.websocket : INFO : Operation: CREATE. Path: article, data: {'author': 'John Doe', 'title': 'In memoriam', 'text': 'text'}
+2024-05-29 16:03:58,484 : MainThread : surrealist.clients.websocket : DEBUG : Send data: {"id": "9bbc90d7-d6dc-4a51-ad97-b765e6b09131", "method": "create", "params": ["article", {"author": "John Doe", "title": "In memoriam", "text": "text"}]}
+2024-05-29 16:03:58,490 : Thread-1 : surrealist.clients.websocket : DEBUG : Get message b'{"id":"9bbc90d7-d6dc-4a51-ad97-b765e6b09131","result":[{"author":"John Doe","id":"article:72duj8mef1s97c67dv38","text":"text","title":"In memoriam"}]}'
+2024-05-29 16:03:58,491 : MainThread : surrealist.connections.websocket : INFO : Got result: SurrealResult(id=9bbc90d7-d6dc-4a51-ad97-b765e6b09131, status=OK, result=[{'author': 'John Doe', 'id': 'article:72duj8mef1s97c67dv38', 'text': 'text', 'title': 'In memoriam'}], query=None, code=None, time=None, additional_info={})
+2024-05-29 16:03:58,491 : MainThread : surrealist.connection : INFO : The connection was closed
+2024-05-29 16:03:58,491 : Thread-1 : surrealist.clients.websocket : DEBUG : Close connection to ws://127.0.0.1:8000/rpc
+2024-05-29 16:03:58,491 : MainThread : surrealist.clients.websocket : DEBUG : Client is closed connection to ws://127.0.0.1:8000/rpc
 ```
 
 **Note:** passwords and auth information always masked in logs. If you still see it in logs - please, report an issue
 
+
 ## Live Query ##
 Live queries let you subscribe to events of desired table when changes happen—you get notification as a simple result or in DIFF format
 
 About live query: https://surrealdb.com/products/lq
 
 Using live select: https://surrealdb.com/docs/surrealdb/surrealql/statements/live
```

### Comparing `surrealist-0.5.1/README.md` & `surrealist-0.5.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # README #
 
-Surrealist is a Python tool to work with awesome [SurrealDB](https://docs.surrealdb.com/docs/intro) (support for latest version 1.5.0)
+Surrealist is a Python tool to work with awesome [SurrealDB](https://docs.surrealdb.com/docs/intro) (support for latest version 1.5.1)
 
 It is **synchronous** and **unofficial**, so if you need async AND/OR official client, go [here](https://github.com/surrealdb/surrealdb.py)
 
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
  * only one small dependency (websocket-client), no need to pull a lot of libraries to your project
  * fully documented
  * well tested (on the latest Ubuntu, macOS and Windows 10)
- * fully compatible with the latest version of SurrealDB (1.5.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
- * debug mode to see all that goes in and out if you need
+ * fully compatible with the latest version of SurrealDB (1.5.1), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
+ * debug mode to see all that goes in and out if you need (using standard logging)
  * iterator to handle big select queries
  * QL-builder to explore, generate and use SurrealDB queries (explain, transaction etc.)
  * connections pool for use at a high load
  * http or websocket transport to use
  * always up to date with SurrealDB features and changes
 
 
@@ -54,17 +54,17 @@
 
 In this example, we explicitly show all parameters, but remember many of them are optional
 
 ```python
 from surrealist import Surreal
 
 # we create a surreal object, it can be used to create one or more connections with websockets (use_http=False)
-# with timeout 10 seconds and ERROR logging level
+# with timeout 10 seconds
 surreal = Surreal("http://127.0.0.1:8000", namespace="test", database="test", credentials=("root", "root"),
-                  use_http=False, timeout=10, log_level="ERROR")
+                  use_http=False, timeout=10)
 print(surreal.is_ready())  # prints True if server up and running on that url
 print(surreal.version())  # prints server version
 ```
 **Note:** create of a Surreal object does not attempt any connections or other actions, just store parameters for future use
 
 Calls of **is_ready()**, **health()** or **version()** on Surreal objects are for server checks only, these not validate or check your namespace, database or credentials.
 
@@ -83,25 +83,24 @@
 
 **credentials** - optional, pair(tuple) of username and password for SurrealDB
 
 **use_http** - optional, False by default, flag of using websockets or http transport, False mean using websocket, specify True if you want to use http transport
 
 **timeout** - optional, 5 seconds by default, it is time in seconds to wait for responses and messages, time for trying to connect to SurrealDB
 
-**log_level** - optional, "ERROR" by default, one of (DEBUG, INFO, ERROR), where ERROR - to see only errors, INFO—to see errors and operations, DEBUG—to see all, including transport requests/responses
 
 **Example 2**
 
 In this example, we do not use default(optional) parameters
 
 ```python
 from surrealist import Surreal
 
 # we create a surreal object, it can be used to create one or more connections with websockets
-# with timeout 5 seconds and ERROR logging level
+# with timeout 15 seconds
 surreal = Surreal("http://127.0.0.1:8000")
 print(surreal.is_ready())  # prints True if server up and running on that url
 print(surreal.version())  # prints server version
 ```
 ## Context managers and close ##
 You should always close created connections, when you do not need them anymore, the best way to do it is via context manager
 
@@ -238,60 +237,66 @@
 **Important note for UTF-8:** record_id can have only A-Z, a-z letters, if you want to use any other UTF-8 letters you have to use backticks "`"!
 
 **Note:** record_id parameter of methods is only concatenated with table_name and colon, so
 ws_connection.select("person", record_id="john") under the hood became
 ws_connection.select("person:john"), but no other logic performed. Do not expect we specified "`" for you.
 
 
-## Debug mode ##
-As it was said, if you need to debug something, stuck in some problem or just want to know all about data between you and SurrealDB, you can use log level.
-If you specify "INFO" level, then you will see transport operations, which methods were called, which parameters were used.
+## Logging and Debug mode ##
+As it was said, if you need to debug something, stuck in some problem or just want to know all about data between you and SurrealDB, you can use standard logging.
+All library logs will contain "surrealist" prefix in logs. You, as a developer, should choose proper handlers, formats, filters etc.
+Surrealist does not use root logger, does not use any handlers and uses only DEBUG, INFO and ERROR level for its events.
+
 For example
 
 **Example 7**
 
 ```python
-from surrealist import Surreal
+from logging import basicConfig, INFO, DEBUG
 
-surreal = Surreal("http://127.0.0.1:8000", namespace="test", database="test", credentials=("root", "root"),
-                  log_level="INFO")
+from surrealist import Surreal, LOG_FORMAT  # LOG_FORMAT is used for simplicity, you can use your own
+
+basicConfig(format=LOG_FORMAT, level=INFO)  # we specify a format and level of events to catch
+
+surreal = Surreal("http://127.0.0.1:8000", namespace="test", database="test", credentials=("root", "root"))
 with surreal.connect() as connection:
     res = connection.create("article", {"author": "John Doe", "title": "In memoriam", "text": "text"})
-
 ```
 if you run it, you get in the console:
 ```
-2024-02-02 18:31:09,419 : Thread-1 : websocket : INFO : Websocket connected
-2024-02-02 18:31:09,521 : MainThread : websocket_connection : INFO : Operation: SIGNIN. Data: {'user': 'root', 'pass': '******', 'NS': 'test', 'DB': 'test'}
-2024-02-02 18:31:09,627 : MainThread : websocket_connection : INFO : Got result: SurrealResult(id='836a2834-c6d5-416c-a840-6322a17b47cc', error=None, result='eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MDY4ODA2NjksIm5iZiI6MTcwNjg4MDY2OSwiZXhwIjoxNzA2ODg0MjY5LCJpc3MiOiJTdXJyZWFsREIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRCI6InJvb3QifQ.mrzxXkva3lCg6EihtUEx8c1yjOtuJt_EvJninTqxJ_1...
-2024-02-02 18:31:09,627 : MainThread : websocket_connection : INFO : Connected to ws://127.0.0.1:8000/rpc, params: {'NS': 'test', 'DB': 'test'}, credentials: ('root', '******'), timeout: 5
-2024-02-02 18:31:09,627 : MainThread : websocket_connection : INFO : Operation: CREATE. Path: article, data: {'author': 'John Doe', 'title': 'In memoriam', 'text': 'text'}
-2024-02-02 18:31:09,733 : MainThread : websocket_connection : INFO : Got result: SurrealResult(id='0870492e-faba-4a5f-b454-c7f7315348bd', error=None, result=[{'author': 'John Doe', 'id': 'article:pt0907zkhkhb94evjnze', 'text': 'text', 'title': 'In memoriam'}], code=None, token=None, status='OK', time='')
-2024-02-02 18:31:09,734 : MainThread : connection : INFO : Connection was closed
-```
-but if in example above (example 5) you choose "DEBUG", you will see all, including low-level clients' data:
-```
-2024-02-02 18:33:15,119 : MainThread : root : DEBUG : Log level switch to DEBUG
-2024-02-02 18:33:15,124 : Thread-1 : websocket : INFO : Websocket connected
-2024-02-02 18:33:15,223 : MainThread : websocket_client : DEBUG : Connected to ws://127.0.0.1:8000/rpc, timeout is 5 seconds
-2024-02-02 18:33:15,223 : MainThread : websocket_connection : INFO : Operation: SIGNIN. Data: {'user': 'root', 'pass': '******', 'NS': 'test', 'DB': 'test'}
-2024-02-02 18:33:15,224 : MainThread : websocket_client : DEBUG : Send data: {"id": "5a2e9c12-e03e-4879-a78a-bd360cd871b1", "method": "signin", "params": [{"user": "root", "pass": "******", "NS": "test", "DB": "test"}]}
-2024-02-02 18:33:15,281 : Thread-1 : websocket_client : DEBUG : Get message b'{"id":"5a2e9c12-e03e-4879-a78a-bd360cd871b1","result":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MDY4ODA3OTUsIm5iZiI6MTcwNjg4MDc5NSwiZXhwIjoxNzA2ODg0Mzk1LCJpc3MiOiJTdXJyZWFsREIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRCI6InJvb3QifQ.2ekRL9EyiaWOQR0Aw1qX8VE5S822Kab5SiYLHLC3YkPX3_Yu-FkWSCoP3XGoUg9w8'...
-2024-02-02 18:33:15,326 : MainThread : websocket_connection : INFO : Got result: SurrealResult(id='5a2e9c12-e03e-4879-a78a-bd360cd871b1', error=None, result='eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MDY4ODA3OTUsIm5iZiI6MTcwNjg4MDc5NSwiZXhwIjoxNzA2ODg0Mzk1LCJpc3MiOiJTdXJyZWFsREIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRCI6InJvb3QifQ.2ekRL9EyiaWOQR0Aw1qX8VE5S822Kab5SiYLHLC3YkP...
-2024-02-02 18:33:15,326 : MainThread : websocket_connection : INFO : Connected to ws://127.0.0.1:8000/rpc, params: {'NS': 'test', 'DB': 'test'}, credentials: ('root', '******'), timeout: 5
-2024-02-02 18:33:15,326 : MainThread : websocket_connection : INFO : Operation: CREATE. Path: article, data: {'author': 'John Doe', 'title': 'In memoriam', 'text': 'text'}
-2024-02-02 18:33:15,326 : MainThread : websocket_client : DEBUG : Send data: {"id": "145b2ed4-9b42-44ab-ade2-e28a27730faa", "method": "create", "params": ["article", {"author": "John Doe", "title": "In memoriam", "text": "text"}]}
-2024-02-02 18:33:15,327 : Thread-1 : websocket_client : DEBUG : Get message b'{"id":"145b2ed4-9b42-44ab-ade2-e28a27730faa","result":[{"author":"John Doe","id":"article:s0coora4gedavt2skd36","text":"text","title":"In memoriam"}]}'
-2024-02-02 18:33:15,432 : MainThread : websocket_connection : INFO : Got result: SurrealResult(id='145b2ed4-9b42-44ab-ade2-e28a27730faa', error=None, result=[{'author': 'John Doe', 'id': 'article:s0coora4gedavt2skd36', 'text': 'text', 'title': 'In memoriam'}], code=None, token=None, status='OK', time='')
-2024-02-02 18:33:15,433 : MainThread : connection : INFO : Connection was closed
-2024-02-02 18:33:15,434 : MainThread : websocket_client : DEBUG : Client is closed connection to ws://127.0.0.1:8000/rpc
+2024-05-29 15:59:41,759 : Thread-1 : websocket : INFO : Websocket connected
+2024-05-29 15:59:41,762 : MainThread : surrealist.connections.websocket : INFO : Operation: SIGNIN. Data: {'user': 'root', 'pass': '******', 'NS': 'test', 'DB': 'test'}
+2024-05-29 15:59:41,788 : MainThread : surrealist.connections.websocket : INFO : Got result: SurrealResult(id=c3fcebbc-359f-47d0-822b-a4ad8043f64b, status=OK, result=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MTY5ODAzODEsIm5iZiI6MTcxNjk4MDM4MSwiZXhwIjoxNzE2OTgzOTgxLCJpc3MiOiJTdXJyZWFsREIiLCJqdGkiOiI0YTQyNWFiNy00NGEyLTQ4OGItYjM4MS05YjUyNDQzYTI5OTQiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRC...
+2024-05-29 15:59:41,788 : MainThread : surrealist.connections.websocket : INFO : Connected to ws://127.0.0.1:8000/rpc, params: {'NS': 'test', 'DB': 'test'}, credentials: ('root', '******'), timeout: 15
+2024-05-29 15:59:41,788 : MainThread : surrealist.connections.websocket : INFO : Operation: CREATE. Path: article, data: {'author': 'John Doe', 'title': 'In memoriam', 'text': 'text'}
+2024-05-29 15:59:41,794 : MainThread : surrealist.connections.websocket : INFO : Got result: SurrealResult(id=b307d67f-b01b-4b71-a319-906fa17b8c72, status=OK, result=[{'author': 'John Doe', 'id': 'article:b44tdiiyb8jw6mcn1tzs', 'text': 'text', 'title': 'In memoriam'}], query=None, code=None, time=None, additional_info={})
+2024-05-29 15:59:41,794 : MainThread : surrealist.connection : INFO : The connection was closed
+```
+but if in the example above (example 7) you choose "DEBUG" for level, you will see all, including low-level clients' data:
+```
+2024-05-29 16:03:58,438 : MainThread : surrealist.clients.websocket : DEBUG : Connecting to ws://127.0.0.1:8000/rpc
+2024-05-29 16:03:58,445 : Thread-1 : websocket : INFO : Websocket connected
+2024-05-29 16:03:58,458 : MainThread : surrealist.clients.websocket : DEBUG : Connected to ws://127.0.0.1:8000/rpc, timeout is 15 seconds
+2024-05-29 16:03:58,458 : MainThread : surrealist.connections.websocket : INFO : Operation: SIGNIN. Data: {'user': 'root', 'pass': '******', 'NS': 'test', 'DB': 'test'}
+2024-05-29 16:03:58,458 : MainThread : surrealist.clients.websocket : DEBUG : Send data: {"id": "1d5758bb-0879-4d8d-9e14-37c9117669a3", "method": "signin", "params": [{"user": "root", "pass": "******", "NS": "test", "DB": "test"}]}
+2024-05-29 16:03:58,484 : Thread-1 : surrealist.clients.websocket : DEBUG : Get message b'{"id":"1d5758bb-0879-4d8d-9e14-37c9117669a3","result":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MTY5ODA2MzgsIm5iZiI6MTcxNjk4MDYzOCwiZXhwIjoxNzE2OTg0MjM4LCJpc3MiOiJTdXJyZWFsREIiLCJqdGkiOiIwODhhMWY0My04YzY3LTQ5NjYtYTdjNC02ZGI5NjA0MGNkYmIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRCI6InJvb3QifQ.1pSbJ'...
+2024-05-29 16:03:58,484 : MainThread : surrealist.connections.websocket : INFO : Got result: SurrealResult(id=1d5758bb-0879-4d8d-9e14-37c9117669a3, status=OK, result=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MTY5ODA2MzgsIm5iZiI6MTcxNjk4MDYzOCwiZXhwIjoxNzE2OTg0MjM4LCJpc3MiOiJTdXJyZWFsREIiLCJqdGkiOiIwODhhMWY0My04YzY3LTQ5NjYtYTdjNC02ZGI5NjA0MGNkYmIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRC...
+2024-05-29 16:03:58,484 : MainThread : surrealist.connections.websocket : INFO : Connected to ws://127.0.0.1:8000/rpc, params: {'NS': 'test', 'DB': 'test'}, credentials: ('root', '******'), timeout: 15
+2024-05-29 16:03:58,484 : MainThread : surrealist.connections.websocket : INFO : Operation: CREATE. Path: article, data: {'author': 'John Doe', 'title': 'In memoriam', 'text': 'text'}
+2024-05-29 16:03:58,484 : MainThread : surrealist.clients.websocket : DEBUG : Send data: {"id": "9bbc90d7-d6dc-4a51-ad97-b765e6b09131", "method": "create", "params": ["article", {"author": "John Doe", "title": "In memoriam", "text": "text"}]}
+2024-05-29 16:03:58,490 : Thread-1 : surrealist.clients.websocket : DEBUG : Get message b'{"id":"9bbc90d7-d6dc-4a51-ad97-b765e6b09131","result":[{"author":"John Doe","id":"article:72duj8mef1s97c67dv38","text":"text","title":"In memoriam"}]}'
+2024-05-29 16:03:58,491 : MainThread : surrealist.connections.websocket : INFO : Got result: SurrealResult(id=9bbc90d7-d6dc-4a51-ad97-b765e6b09131, status=OK, result=[{'author': 'John Doe', 'id': 'article:72duj8mef1s97c67dv38', 'text': 'text', 'title': 'In memoriam'}], query=None, code=None, time=None, additional_info={})
+2024-05-29 16:03:58,491 : MainThread : surrealist.connection : INFO : The connection was closed
+2024-05-29 16:03:58,491 : Thread-1 : surrealist.clients.websocket : DEBUG : Close connection to ws://127.0.0.1:8000/rpc
+2024-05-29 16:03:58,491 : MainThread : surrealist.clients.websocket : DEBUG : Client is closed connection to ws://127.0.0.1:8000/rpc
 ```
 
 **Note:** passwords and auth information always masked in logs. If you still see it in logs - please, report an issue
 
+
 ## Live Query ##
 Live queries let you subscribe to events of desired table when changes happen—you get notification as a simple result or in DIFF format
 
 About live query: https://surrealdb.com/products/lq
 
 Using live select: https://surrealdb.com/docs/surrealdb/surrealql/statements/live
```

### Comparing `surrealist-0.5.1/pyproject.toml` & `surrealist-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "surrealist"
-version = "0.5.1"
+version = "0.5.2"
 description = "Python client for SurrealDB, latest SurrealDB version compatible, all features supported"
 readme = "README.md"
 authors = [{ name = "kotolex", email = "farofwell@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
```

### Comparing `surrealist-0.5.1/src/surrealist/__init__.py` & `surrealist-0.5.2/src/surrealist/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .connections import WebSocketConnection, HttpConnection, Connection
 from .errors import *
 from .ql import Database, DatabaseConnectionsPool, Table, Where
 from .result import SurrealResult
 from .surreal import Surreal
-from .utils import DATA_LENGTH_FOR_LOGS, get_uuid, to_surreal_datetime_str, to_datetime
+from .utils import DATA_LENGTH_FOR_LOGS, get_uuid, to_surreal_datetime_str, to_datetime, LOG_FORMAT
 
 __all__ = ("Surreal", "SurrealResult", "WebSocketConnection", "HttpConnection", "PySurrealError", "HttpConnectionError",
            "HttpClientError", "SurrealConnectionError", "WebSocketConnectionError", "WebSocketConnectionClosedError",
            "ConnectionParametersError", "CompatibilityError", "OperationOnClosedConnectionError", "WrongCallError",
            "DATA_LENGTH_FOR_LOGS", "Connection", "get_uuid", "Database", "Table", "Where", "DatabaseConnectionsPool",
-           "to_surreal_datetime_str", "to_datetime")
+           "to_surreal_datetime_str", "to_datetime", "LOG_FORMAT")
```

### Comparing `surrealist-0.5.1/src/surrealist/clients/http_client.py` & `surrealist-0.5.2/src/surrealist/clients/http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from logging import getLogger
 from typing import Optional, Tuple, Dict, Union, BinaryIO
 from urllib.error import URLError, HTTPError
 
 from surrealist.errors import HttpClientError, TooManyNestedLevelsError
 from surrealist.utils import ENCODING, DEFAULT_TIMEOUT, crop_data, mask_pass
 
-logger = getLogger("http_client")
+logger = getLogger("surrealist.clients.http")
 
 
 class HttpClient:
     """
     Http-client for working with http endpoints and abilities of SurrealDB
     """
```

### Comparing `surrealist-0.5.1/src/surrealist/clients/ws_client.py` & `surrealist-0.5.2/src/surrealist/clients/ws_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import websocket
 
 from surrealist.errors import WebSocketConnectionClosedError, TooManyNestedLevelsError
 from surrealist.result import to_result, SurrealResult
 from surrealist.utils import DEFAULT_TIMEOUT, get_uuid, crop_data, mask_pass
 
-logger = getLogger("websocket_client")
+logger = getLogger("surrealist.clients.websocket")
 
 
 class WebSocketClient:
     """
     Synchronous thread-safe client to work with websockets, always wait a response for message, comparing by id (uuid).
     Every client creates at least two threads (in and out)
     """
```

### Comparing `surrealist-0.5.1/src/surrealist/connections/connection.py` & `surrealist-0.5.2/src/surrealist/connections/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from logging import getLogger
 from typing import Tuple, Dict, Optional, Union, List, Callable, Any
 
 from surrealist.errors import OperationOnClosedConnectionError, TooManyNestedLevelsError
 from surrealist.result import SurrealResult
 from surrealist.utils import DEFAULT_TIMEOUT, crop_data
 
-logger = getLogger("connection")
+logger = getLogger("surrealist.connection")
 LINK = "https://github.com/kotolex/surrealist?tab=readme-ov-file#recursion-and-json-in-python"
 
 
 def connected(func):
     """
     Decorator for methods to make sure the underlying connection is alive (connected to DB)
```

### Comparing `surrealist-0.5.1/src/surrealist/connections/http_connection.py` & `surrealist-0.5.2/src/surrealist/connections/http_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from surrealist.clients.http_client import HttpClient
 from surrealist.connections.connection import Connection, connected
 from surrealist.errors import (SurrealConnectionError, HttpClientError, CompatibilityError, HttpConnectionError)
 from surrealist.result import SurrealResult, to_result
 from surrealist.utils import (ENCODING, DEFAULT_TIMEOUT, crop_data, mask_pass, HTTP_OK)
 
-logger = getLogger("http_connection")
+logger = getLogger("surrealist.connections.http")
 
 
 class HttpConnection(Connection):
     """
     Represents http transport and abilities to work with SurrealDb. It is not a recommended connection, use websocket in 
     any doubt; this connection exists for compatibility reasons. Some features as live query are not possible on this
     transport, but import and export are.
```

### Comparing `surrealist-0.5.1/src/surrealist/connections/pool.py` & `surrealist-0.5.2/src/surrealist/connections/pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from surrealist.connections.connection import Connection
 from surrealist.errors import OperationOnClosedConnectionError
 from surrealist.result import SurrealResult
 from surrealist.surreal import Surreal
 from surrealist.utils import DEFAULT_TIMEOUT
 
 CORES_COUNT = cpu_count()
-logger = getLogger("pool")
+logger = getLogger("surrealist.connection.pool")
 
 
 def connected_and_pooled(func):
     """
     Wrapper to check if pool is connected ad delegate work to underlying connections
     :param func: function to wrap
     """
@@ -37,19 +37,19 @@
     Represents a pool of connections, which is creating a bunch of database connections on start and delegating all
     tasks to the first non-busy connection. So, if there are no nore connections in the pool, it tries to create a new
     one if the maximum is not exceeded. If the maximum of connections is reached and no more connections to work with -
     client will be blocked until the first connection finishes the task and appears at the pool.
     """
     def __init__(self, first_connection: Connection, url: str, namespace: Optional[str] = None,
                  database: Optional[str] = None, credentials: Tuple[str, str] = None, use_http: bool = False,
-                 timeout: int = DEFAULT_TIMEOUT, log_level: str = "ERROR", min_connections: int = CORES_COUNT,
+                 timeout: int = DEFAULT_TIMEOUT, min_connections: int = CORES_COUNT,
                  max_connections: int = 50):
         self._options = {
             "url": url, "namespace": namespace, "database": database, "credentials": credentials, "use_http": use_http,
-            "timeout": timeout, "log_level": log_level
+            "timeout": timeout
         }
         self._timeout = timeout
         self._url = url
         self._min = min_connections if min_connections > 1 else 2
         self._max = max_connections if max_connections <= 50 else 50
         self._main = Queue(maxsize=self._max)
         self._main.put_nowait(first_connection)
```

### Comparing `surrealist-0.5.1/src/surrealist/connections/ws_connection.py` & `surrealist-0.5.2/src/surrealist/connections/ws_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from surrealist.clients.ws_client import WebSocketClient
 from surrealist.connections.connection import Connection, connected
 from surrealist.errors import (SurrealConnectionError, WebSocketConnectionError, ConnectionParametersError,
                                WebSocketConnectionClosedError, CompatibilityError)
 from surrealist.result import SurrealResult
 from surrealist.utils import DEFAULT_TIMEOUT, crop_data, mask_pass
 
-logger = getLogger("websocket_connection")
+logger = getLogger("surrealist.connections.websocket")
 
 
 class WebSocketConnection(Connection):
     """
     Represents websocket transport and abilities to work with SurrealDb. It is a recommended connection.
 
     Refer to surrealist documentation: https://github.com/kotolex/surrealist?tab=readme-ov-file#transports
```

### Comparing `surrealist-0.5.1/src/surrealist/errors.py` & `surrealist-0.5.2/src/surrealist/errors.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/database.py` & `surrealist-0.5.2/src/surrealist/ql/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 from surrealist.ql.statements.statement import Statement
 from surrealist.ql.statements.transaction import Transaction
 from surrealist.ql.table import Table
 from surrealist.result import SurrealResult
 from surrealist.surreal import Surreal
 from surrealist.utils import DEFAULT_TIMEOUT
 
-logger = logging.getLogger("databaseQL")
+logger = logging.getLogger("surrealist.databaseQL")
 
 
 class Database:
     """
     Represents connected database(in some namespace) to operate on.
     It has features of the database level, including switch to table level. You can use DEFINE/REMOVE, query or
     transactions here, but for simple CRUD you need to switch to table level
 
     Examples: https://github.com/kotolex/surrealist/blob/master/examples/surreal_ql/database.py
     """
 
     def __init__(self, url: str, namespace: str, database: str, credentials: Optional[Tuple[str, str]],
-                 use_http: bool = False, timeout: int = DEFAULT_TIMEOUT, log_level: str = "ERROR"):
+                 use_http: bool = False, timeout: int = DEFAULT_TIMEOUT):
         self._namespace = namespace
         self._database = database
-        self._connection = Surreal(url, namespace, database, credentials, use_http, timeout, log_level).connect()
+        self._connection = Surreal(url, namespace, database, credentials, use_http, timeout).connect()
         self._connected = True
         logger.info("DatabaseQL is up")
 
     def __enter__(self):
         return self
 
     def __exit__(self, *exc_details):
```

### Comparing `surrealist-0.5.1/src/surrealist/ql/pool_database.py` & `surrealist-0.5.2/src/surrealist/ql/pool_database.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,46 +3,45 @@
 from typing import Optional, Tuple
 
 from surrealist.connections.pool import Pool
 from surrealist.ql.database import Database
 from surrealist.utils import DEFAULT_TIMEOUT
 
 CORES_COUNT = cpu_count()
-logger = logging.getLogger("pool_databaseQL")
+logger = logging.getLogger("surrealist.databaseQL.pool")
 
 
 class DatabaseConnectionsPool(Database):
     """
-    Represents a pool of connections to a database, for using in high-load multithreaded environments. As a child of
-    Database object it can be used everywhere, where Database can.
+    Represents a pool of connections to a database, for using in high-load multithreading environments. As a child of
+    Database object it can be used everywhere where Database can.
     The main difference is a number of created connections. By default, the minimum number is equal to CPU cores count
     in the system and cannot be less than 2.
 
     During work, if no more non-busy connections to use, then new connection will be created until its number not
     reaches maximum for the pool
 
     Refer to: https://github.com/kotolex/surrealist?tab=readme-ov-file#connections-pool
 
     """
 
     def __init__(self, url: str, namespace: str, database: str, credentials: Optional[Tuple[str, str]],
-                 use_http: bool = False, timeout: int = DEFAULT_TIMEOUT, log_level: str = "ERROR",
+                 use_http: bool = False, timeout: int = DEFAULT_TIMEOUT,
                  min_connections: int = CORES_COUNT, max_connections: int = 50):
         """
         All parameters are the same as for Surreal or Database object
 
         :param min_connections: minimum number of connections, it cannot be less than 2
         :param max_connections: maximum number of connections, it cannot be more than 50
         """
         self._options = {
             "url": url, "namespace": namespace, "database": database, "credentials": credentials, "use_http": use_http,
-            "timeout": timeout, "log_level": log_level, "min_connections": min_connections,
-            "max_connections": max_connections
+            "timeout": timeout, "min_connections": min_connections, "max_connections": max_connections
         }
-        super().__init__(url, namespace, database, credentials, use_http, timeout, log_level)
+        super().__init__(url, namespace, database, credentials, use_http, timeout)
         self._connection = Pool(self._connection, **self._options)
         self._connected = True
         self._min = min_connections
         self._max = max_connections
         logger.info("Pool DatabaseQL is up")
 
     @property
```

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/__init__.py` & `surrealist-0.5.2/src/surrealist/ql/statements/__init__.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/common_statements.py` & `surrealist-0.5.2/src/surrealist/ql/statements/common_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/create.py` & `surrealist-0.5.2/src/surrealist/ql/statements/create.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/create_statements.py` & `surrealist-0.5.2/src/surrealist/ql/statements/create_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/define.py` & `surrealist-0.5.2/src/surrealist/ql/statements/define.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/define_index_statements.py` & `surrealist-0.5.2/src/surrealist/ql/statements/define_index_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/delete.py` & `surrealist-0.5.2/src/surrealist/ql/statements/delete.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/insert.py` & `surrealist-0.5.2/src/surrealist/ql/statements/insert.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/insert_statements.py` & `surrealist-0.5.2/src/surrealist/ql/statements/insert_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/live.py` & `surrealist-0.5.2/src/surrealist/ql/statements/live.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/live_statements.py` & `surrealist-0.5.2/src/surrealist/ql/statements/live_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/permissions.py` & `surrealist-0.5.2/src/surrealist/ql/statements/permissions.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/rebuild_index.py` & `surrealist-0.5.2/src/surrealist/ql/statements/rebuild_index.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/relate.py` & `surrealist-0.5.2/src/surrealist/ql/statements/relate.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/remove.py` & `surrealist-0.5.2/src/surrealist/ql/statements/remove.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/returns.py` & `surrealist-0.5.2/src/surrealist/ql/statements/returns.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/select.py` & `surrealist-0.5.2/src/surrealist/ql/statements/select.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/select_statements.py` & `surrealist-0.5.2/src/surrealist/ql/statements/select_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/show.py` & `surrealist-0.5.2/src/surrealist/ql/statements/show.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/simple_statements.py` & `surrealist-0.5.2/src/surrealist/ql/statements/simple_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/statement.py` & `surrealist-0.5.2/src/surrealist/ql/statements/statement.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/transaction.py` & `surrealist-0.5.2/src/surrealist/ql/statements/transaction.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/update.py` & `surrealist-0.5.2/src/surrealist/ql/statements/update.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/update_statements.py` & `surrealist-0.5.2/src/surrealist/ql/statements/update_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/statements/utils.py` & `surrealist-0.5.2/src/surrealist/ql/statements/utils.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/ql/table.py` & `surrealist-0.5.2/src/surrealist/ql/table.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.1/src/surrealist/result.py` & `surrealist-0.5.2/src/surrealist/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from surrealist.errors import TooManyNestedLevelsError, ResultHasNoValuesError
 from surrealist.utils import OK, ERR, HTTP_OK
 
 
 class SurrealResult:
     """
     Represents a result of the request both via http or websocket.
-    Contains a few helpers to work with results of different kind: id, ids, get, is_error, is_empty
+    Contains a few helpers to work with results of different kinds: id, ids, get, is_error, is_empty
     """
 
     def __init__(self, **kwargs):
         """
         Expected fields:
         id - only from websocket requests
         result - error text or any other result of the request
```

### Comparing `surrealist-0.5.1/src/surrealist/surreal.py` & `surrealist-0.5.2/src/surrealist/surreal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 import urllib.parse
-from logging import getLogger, ERROR, DEBUG, basicConfig, INFO
+from logging import getLogger
 from typing import Tuple, Optional
 
 from surrealist.clients import HttpClient
 from surrealist.connections.connection import Connection
 from surrealist.connections.http_connection import HttpConnection
 from surrealist.connections.ws_connection import WebSocketConnection
 from surrealist.errors import HttpClientError, SurrealConnectionError
 from surrealist.utils import DEFAULT_TIMEOUT, _set_length, DATA_LENGTH_FOR_LOGS, ENCODING, OK, HTTP_OK
 
-FORMAT = '%(asctime)s : %(threadName)s : %(name)s : %(levelname)s : %(message)s'
-basicConfig(level=ERROR, format=FORMAT)
-logger = getLogger()
+logger = getLogger("surrealist")
 
 
 class Surreal:
     """
     Represents the SurrealDB client, all connections should be established via this class. By default, connection will
-    use websocket transport (recommended). This class uses log level to monitor all actions, can check a version and
+    use websocket transport (recommended). This class uses logging to monitor all actions, can check a version and
     state of the SurrealDb server.
     If you have only one SurrealDB server, you need exactly one object of this class!
 
     Refer to: https://github.com/kotolex/surrealist?tab=readme-ov-file#connect-to-surrealdb
     """
 
     def __init__(self, url: str, namespace: Optional[str] = None, database: Optional[str] = None,
-                 credentials: Tuple[str, str] = None, use_http: bool = False, timeout: int = DEFAULT_TIMEOUT,
-                 log_level: str = "ERROR"):
+                 credentials: Tuple[str, str] = None, use_http: bool = False, timeout: int = DEFAULT_TIMEOUT):
         """
         Initiating all parameters for connection, this method does not check or validates anything by itself, just save
         data for future use. To make sure your url is valid and accessible - use **is_ready** method of Surreal object.
 
-        About log_level and debug mode: https://github.com/kotolex/surrealist?tab=readme-ov-file#debug-mode
+        About debug mode: https://github.com/kotolex/surrealist?tab=readme-ov-file#logging-and-debug-mode
 
         :param url: database url, for local database http://127.0.0.1:8000/
         :param namespace: namespace to use
         :param database: a database to use, make sure to use both namespace and database or none of them
         :param credentials: pair of user and password, for example ("root", "root")
         :param use_http: boolean flag of using http transport. Will use websocket-client if False.
         It is strongly recommended to use websocket transport as it is more powerful.
         :param timeout: connection timeout in seconds
-        :param log_level: level of logging for debug purposes, one of (DEBUG, INFO, ERROR) allowed, where ERROR
-        is default, INFO - to see only operations, DEBUG - to see all, including transport requests/responses
         """
-        self._log_level = log_level
         self._log_data_length = DATA_LENGTH_FOR_LOGS
-        self.set_log_level(log_level)
         self._client = HttpConnection if use_http else WebSocketConnection
         self.db_params = {}
         if namespace:
             self.db_params["NS"] = namespace
         if database:
             self.db_params["DB"] = database
         if not self.db_params:
@@ -89,40 +82,14 @@
         SurrealDB messages.
 
         :param length: new maximum length for one string in logs
         """
         _set_length(length)
         self._log_data_length = length
 
-    def set_log_level(self, level: str):
-        """
-        Setting log level for all underlying connections of that Surreal object.
-        There are 3 options:
-        - ERROR which is default and recommended for most situations, you will see only errors
-        - INFO which is show all information about connection operations
-        - DEBUG, when you will see all logs, including requests and responses via transport level. This level is very
-        useful for debugging and finding some useful information in logs
-
-        Refer to: https://github.com/kotolex/surrealist?tab=readme-ov-file#debug-mode
-
-        Notice: authorization params and passwords can't be seen in logs at any time, if you see it, please report
-        an issue
-
-        Notice: you will see logs of this library(in and out), but not SurrealDb server logs
-
-        :param level: one of "DEBUG", "INFO", "ERROR"
-        """
-        if level not in ("DEBUG", "INFO", "ERROR"):
-            raise ValueError("Log level should be one of (DEBUG, INFO, ERROR), where ERROR is default")
-        levels = {"DEBUG": DEBUG, "INFO": INFO, "ERROR": ERROR}
-        new_level = levels[level]
-        logger.setLevel(new_level)
-        logger.debug("Log level switch to %s", level)
-        self._log_level = level
-
     def connect(self) -> Connection:
         """
         Actually connects to a database via chosen transport (websocket or http), uses specified namespace, database and
         credentials parameters, so can raise exception if connect will fail. If this method succeeded, you are
         ready to go with SurrealDB
 
         :return: connection object to work with SurrealDB
@@ -179,14 +146,17 @@
         Refer to: https://docs.surrealdb.com/docs/integration/http#version
 
         :return: version, for example, "surrealdb-1.1.1"
         :raise SurrealConnectionError: if cant connect to http-endpoint
         """
         return self.__get("version")[1]
 
+    def __repr__(self) -> str:
+        return f"Surreal(url={self._possible_url}, db_params={self.db_params}, timeout={self.timeout})"
+
     def __get(self, endpoint: str) -> Tuple[int, str]:
         try:
             with HttpClient(self._possible_url, timeout=DEFAULT_TIMEOUT).get(endpoint) as resp:
                 status, text = resp.status, resp.read().decode(ENCODING)
                 body = "is empty" if not text else text
                 logger.info("Response from /%s, status_code: %s, body: %s", endpoint, status, body)
                 if status != HTTP_OK:
```

### Comparing `surrealist-0.5.1/src/surrealist/utils.py` & `surrealist-0.5.2/src/surrealist/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 OK = "OK"
 ERR = "ERR"
 DATE_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
 DATE_FORMAT_NS = "%Y-%m-%dT%H:%M:%S.%fZ"
 HTTP_OK = 200  # status code for success
 DEFAULT_TIMEOUT = 15  # timeout in seconds for basic operations
 DATA_LENGTH_FOR_LOGS = 300  # size of data in logs, data will be cropped if bigger than that
+LOG_FORMAT = '%(asctime)s : %(threadName)s : %(name)s : %(levelname)s : %(message)s'  # use it for logs
 
 
 def _set_length(length: int):
     global DATA_LENGTH_FOR_LOGS
     DATA_LENGTH_FOR_LOGS = length
```

### Comparing `surrealist-0.5.1/src/surrealist.egg-info/PKG-INFO` & `surrealist-0.5.2/src/surrealist.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surrealist
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python client for SurrealDB, latest SurrealDB version compatible, all features supported
 Author-email: kotolex <farofwell@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,27 +34,27 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: websocket-client
 
 # README #
 
-Surrealist is a Python tool to work with awesome [SurrealDB](https://docs.surrealdb.com/docs/intro) (support for latest version 1.5.0)
+Surrealist is a Python tool to work with awesome [SurrealDB](https://docs.surrealdb.com/docs/intro) (support for latest version 1.5.1)
 
 It is **synchronous** and **unofficial**, so if you need async AND/OR official client, go [here](https://github.com/surrealdb/surrealdb.py)
 
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
  * only one small dependency (websocket-client), no need to pull a lot of libraries to your project
  * fully documented
  * well tested (on the latest Ubuntu, macOS and Windows 10)
- * fully compatible with the latest version of SurrealDB (1.5.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
- * debug mode to see all that goes in and out if you need
+ * fully compatible with the latest version of SurrealDB (1.5.1), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
+ * debug mode to see all that goes in and out if you need (using standard logging)
  * iterator to handle big select queries
  * QL-builder to explore, generate and use SurrealDB queries (explain, transaction etc.)
  * connections pool for use at a high load
  * http or websocket transport to use
  * always up to date with SurrealDB features and changes
 
 
@@ -92,17 +92,17 @@
 
 In this example, we explicitly show all parameters, but remember many of them are optional
 
 ```python
 from surrealist import Surreal
 
 # we create a surreal object, it can be used to create one or more connections with websockets (use_http=False)
-# with timeout 10 seconds and ERROR logging level
+# with timeout 10 seconds
 surreal = Surreal("http://127.0.0.1:8000", namespace="test", database="test", credentials=("root", "root"),
-                  use_http=False, timeout=10, log_level="ERROR")
+                  use_http=False, timeout=10)
 print(surreal.is_ready())  # prints True if server up and running on that url
 print(surreal.version())  # prints server version
 ```
 **Note:** create of a Surreal object does not attempt any connections or other actions, just store parameters for future use
 
 Calls of **is_ready()**, **health()** or **version()** on Surreal objects are for server checks only, these not validate or check your namespace, database or credentials.
 
@@ -121,25 +121,24 @@
 
 **credentials** - optional, pair(tuple) of username and password for SurrealDB
 
 **use_http** - optional, False by default, flag of using websockets or http transport, False mean using websocket, specify True if you want to use http transport
 
 **timeout** - optional, 5 seconds by default, it is time in seconds to wait for responses and messages, time for trying to connect to SurrealDB
 
-**log_level** - optional, "ERROR" by default, one of (DEBUG, INFO, ERROR), where ERROR - to see only errors, INFO—to see errors and operations, DEBUG—to see all, including transport requests/responses
 
 **Example 2**
 
 In this example, we do not use default(optional) parameters
 
 ```python
 from surrealist import Surreal
 
 # we create a surreal object, it can be used to create one or more connections with websockets
-# with timeout 5 seconds and ERROR logging level
+# with timeout 15 seconds
 surreal = Surreal("http://127.0.0.1:8000")
 print(surreal.is_ready())  # prints True if server up and running on that url
 print(surreal.version())  # prints server version
 ```
 ## Context managers and close ##
 You should always close created connections, when you do not need them anymore, the best way to do it is via context manager
 
@@ -276,60 +275,66 @@
 **Important note for UTF-8:** record_id can have only A-Z, a-z letters, if you want to use any other UTF-8 letters you have to use backticks "`"!
 
 **Note:** record_id parameter of methods is only concatenated with table_name and colon, so
 ws_connection.select("person", record_id="john") under the hood became
 ws_connection.select("person:john"), but no other logic performed. Do not expect we specified "`" for you.
 
 
-## Debug mode ##
-As it was said, if you need to debug something, stuck in some problem or just want to know all about data between you and SurrealDB, you can use log level.
-If you specify "INFO" level, then you will see transport operations, which methods were called, which parameters were used.
+## Logging and Debug mode ##
+As it was said, if you need to debug something, stuck in some problem or just want to know all about data between you and SurrealDB, you can use standard logging.
+All library logs will contain "surrealist" prefix in logs. You, as a developer, should choose proper handlers, formats, filters etc.
+Surrealist does not use root logger, does not use any handlers and uses only DEBUG, INFO and ERROR level for its events.
+
 For example
 
 **Example 7**
 
 ```python
-from surrealist import Surreal
+from logging import basicConfig, INFO, DEBUG
 
-surreal = Surreal("http://127.0.0.1:8000", namespace="test", database="test", credentials=("root", "root"),
-                  log_level="INFO")
+from surrealist import Surreal, LOG_FORMAT  # LOG_FORMAT is used for simplicity, you can use your own
+
+basicConfig(format=LOG_FORMAT, level=INFO)  # we specify a format and level of events to catch
+
+surreal = Surreal("http://127.0.0.1:8000", namespace="test", database="test", credentials=("root", "root"))
 with surreal.connect() as connection:
     res = connection.create("article", {"author": "John Doe", "title": "In memoriam", "text": "text"})
-
 ```
 if you run it, you get in the console:
 ```
-2024-02-02 18:31:09,419 : Thread-1 : websocket : INFO : Websocket connected
-2024-02-02 18:31:09,521 : MainThread : websocket_connection : INFO : Operation: SIGNIN. Data: {'user': 'root', 'pass': '******', 'NS': 'test', 'DB': 'test'}
-2024-02-02 18:31:09,627 : MainThread : websocket_connection : INFO : Got result: SurrealResult(id='836a2834-c6d5-416c-a840-6322a17b47cc', error=None, result='eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MDY4ODA2NjksIm5iZiI6MTcwNjg4MDY2OSwiZXhwIjoxNzA2ODg0MjY5LCJpc3MiOiJTdXJyZWFsREIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRCI6InJvb3QifQ.mrzxXkva3lCg6EihtUEx8c1yjOtuJt_EvJninTqxJ_1...
-2024-02-02 18:31:09,627 : MainThread : websocket_connection : INFO : Connected to ws://127.0.0.1:8000/rpc, params: {'NS': 'test', 'DB': 'test'}, credentials: ('root', '******'), timeout: 5
-2024-02-02 18:31:09,627 : MainThread : websocket_connection : INFO : Operation: CREATE. Path: article, data: {'author': 'John Doe', 'title': 'In memoriam', 'text': 'text'}
-2024-02-02 18:31:09,733 : MainThread : websocket_connection : INFO : Got result: SurrealResult(id='0870492e-faba-4a5f-b454-c7f7315348bd', error=None, result=[{'author': 'John Doe', 'id': 'article:pt0907zkhkhb94evjnze', 'text': 'text', 'title': 'In memoriam'}], code=None, token=None, status='OK', time='')
-2024-02-02 18:31:09,734 : MainThread : connection : INFO : Connection was closed
-```
-but if in example above (example 5) you choose "DEBUG", you will see all, including low-level clients' data:
-```
-2024-02-02 18:33:15,119 : MainThread : root : DEBUG : Log level switch to DEBUG
-2024-02-02 18:33:15,124 : Thread-1 : websocket : INFO : Websocket connected
-2024-02-02 18:33:15,223 : MainThread : websocket_client : DEBUG : Connected to ws://127.0.0.1:8000/rpc, timeout is 5 seconds
-2024-02-02 18:33:15,223 : MainThread : websocket_connection : INFO : Operation: SIGNIN. Data: {'user': 'root', 'pass': '******', 'NS': 'test', 'DB': 'test'}
-2024-02-02 18:33:15,224 : MainThread : websocket_client : DEBUG : Send data: {"id": "5a2e9c12-e03e-4879-a78a-bd360cd871b1", "method": "signin", "params": [{"user": "root", "pass": "******", "NS": "test", "DB": "test"}]}
-2024-02-02 18:33:15,281 : Thread-1 : websocket_client : DEBUG : Get message b'{"id":"5a2e9c12-e03e-4879-a78a-bd360cd871b1","result":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MDY4ODA3OTUsIm5iZiI6MTcwNjg4MDc5NSwiZXhwIjoxNzA2ODg0Mzk1LCJpc3MiOiJTdXJyZWFsREIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRCI6InJvb3QifQ.2ekRL9EyiaWOQR0Aw1qX8VE5S822Kab5SiYLHLC3YkPX3_Yu-FkWSCoP3XGoUg9w8'...
-2024-02-02 18:33:15,326 : MainThread : websocket_connection : INFO : Got result: SurrealResult(id='5a2e9c12-e03e-4879-a78a-bd360cd871b1', error=None, result='eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MDY4ODA3OTUsIm5iZiI6MTcwNjg4MDc5NSwiZXhwIjoxNzA2ODg0Mzk1LCJpc3MiOiJTdXJyZWFsREIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRCI6InJvb3QifQ.2ekRL9EyiaWOQR0Aw1qX8VE5S822Kab5SiYLHLC3YkP...
-2024-02-02 18:33:15,326 : MainThread : websocket_connection : INFO : Connected to ws://127.0.0.1:8000/rpc, params: {'NS': 'test', 'DB': 'test'}, credentials: ('root', '******'), timeout: 5
-2024-02-02 18:33:15,326 : MainThread : websocket_connection : INFO : Operation: CREATE. Path: article, data: {'author': 'John Doe', 'title': 'In memoriam', 'text': 'text'}
-2024-02-02 18:33:15,326 : MainThread : websocket_client : DEBUG : Send data: {"id": "145b2ed4-9b42-44ab-ade2-e28a27730faa", "method": "create", "params": ["article", {"author": "John Doe", "title": "In memoriam", "text": "text"}]}
-2024-02-02 18:33:15,327 : Thread-1 : websocket_client : DEBUG : Get message b'{"id":"145b2ed4-9b42-44ab-ade2-e28a27730faa","result":[{"author":"John Doe","id":"article:s0coora4gedavt2skd36","text":"text","title":"In memoriam"}]}'
-2024-02-02 18:33:15,432 : MainThread : websocket_connection : INFO : Got result: SurrealResult(id='145b2ed4-9b42-44ab-ade2-e28a27730faa', error=None, result=[{'author': 'John Doe', 'id': 'article:s0coora4gedavt2skd36', 'text': 'text', 'title': 'In memoriam'}], code=None, token=None, status='OK', time='')
-2024-02-02 18:33:15,433 : MainThread : connection : INFO : Connection was closed
-2024-02-02 18:33:15,434 : MainThread : websocket_client : DEBUG : Client is closed connection to ws://127.0.0.1:8000/rpc
+2024-05-29 15:59:41,759 : Thread-1 : websocket : INFO : Websocket connected
+2024-05-29 15:59:41,762 : MainThread : surrealist.connections.websocket : INFO : Operation: SIGNIN. Data: {'user': 'root', 'pass': '******', 'NS': 'test', 'DB': 'test'}
+2024-05-29 15:59:41,788 : MainThread : surrealist.connections.websocket : INFO : Got result: SurrealResult(id=c3fcebbc-359f-47d0-822b-a4ad8043f64b, status=OK, result=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MTY5ODAzODEsIm5iZiI6MTcxNjk4MDM4MSwiZXhwIjoxNzE2OTgzOTgxLCJpc3MiOiJTdXJyZWFsREIiLCJqdGkiOiI0YTQyNWFiNy00NGEyLTQ4OGItYjM4MS05YjUyNDQzYTI5OTQiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRC...
+2024-05-29 15:59:41,788 : MainThread : surrealist.connections.websocket : INFO : Connected to ws://127.0.0.1:8000/rpc, params: {'NS': 'test', 'DB': 'test'}, credentials: ('root', '******'), timeout: 15
+2024-05-29 15:59:41,788 : MainThread : surrealist.connections.websocket : INFO : Operation: CREATE. Path: article, data: {'author': 'John Doe', 'title': 'In memoriam', 'text': 'text'}
+2024-05-29 15:59:41,794 : MainThread : surrealist.connections.websocket : INFO : Got result: SurrealResult(id=b307d67f-b01b-4b71-a319-906fa17b8c72, status=OK, result=[{'author': 'John Doe', 'id': 'article:b44tdiiyb8jw6mcn1tzs', 'text': 'text', 'title': 'In memoriam'}], query=None, code=None, time=None, additional_info={})
+2024-05-29 15:59:41,794 : MainThread : surrealist.connection : INFO : The connection was closed
+```
+but if in the example above (example 7) you choose "DEBUG" for level, you will see all, including low-level clients' data:
+```
+2024-05-29 16:03:58,438 : MainThread : surrealist.clients.websocket : DEBUG : Connecting to ws://127.0.0.1:8000/rpc
+2024-05-29 16:03:58,445 : Thread-1 : websocket : INFO : Websocket connected
+2024-05-29 16:03:58,458 : MainThread : surrealist.clients.websocket : DEBUG : Connected to ws://127.0.0.1:8000/rpc, timeout is 15 seconds
+2024-05-29 16:03:58,458 : MainThread : surrealist.connections.websocket : INFO : Operation: SIGNIN. Data: {'user': 'root', 'pass': '******', 'NS': 'test', 'DB': 'test'}
+2024-05-29 16:03:58,458 : MainThread : surrealist.clients.websocket : DEBUG : Send data: {"id": "1d5758bb-0879-4d8d-9e14-37c9117669a3", "method": "signin", "params": [{"user": "root", "pass": "******", "NS": "test", "DB": "test"}]}
+2024-05-29 16:03:58,484 : Thread-1 : surrealist.clients.websocket : DEBUG : Get message b'{"id":"1d5758bb-0879-4d8d-9e14-37c9117669a3","result":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MTY5ODA2MzgsIm5iZiI6MTcxNjk4MDYzOCwiZXhwIjoxNzE2OTg0MjM4LCJpc3MiOiJTdXJyZWFsREIiLCJqdGkiOiIwODhhMWY0My04YzY3LTQ5NjYtYTdjNC02ZGI5NjA0MGNkYmIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRCI6InJvb3QifQ.1pSbJ'...
+2024-05-29 16:03:58,484 : MainThread : surrealist.connections.websocket : INFO : Got result: SurrealResult(id=1d5758bb-0879-4d8d-9e14-37c9117669a3, status=OK, result=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpYXQiOjE3MTY5ODA2MzgsIm5iZiI6MTcxNjk4MDYzOCwiZXhwIjoxNzE2OTg0MjM4LCJpc3MiOiJTdXJyZWFsREIiLCJqdGkiOiIwODhhMWY0My04YzY3LTQ5NjYtYTdjNC02ZGI5NjA0MGNkYmIiLCJOUyI6InRlc3QiLCJEQiI6InRlc3QiLCJJRC...
+2024-05-29 16:03:58,484 : MainThread : surrealist.connections.websocket : INFO : Connected to ws://127.0.0.1:8000/rpc, params: {'NS': 'test', 'DB': 'test'}, credentials: ('root', '******'), timeout: 15
+2024-05-29 16:03:58,484 : MainThread : surrealist.connections.websocket : INFO : Operation: CREATE. Path: article, data: {'author': 'John Doe', 'title': 'In memoriam', 'text': 'text'}
+2024-05-29 16:03:58,484 : MainThread : surrealist.clients.websocket : DEBUG : Send data: {"id": "9bbc90d7-d6dc-4a51-ad97-b765e6b09131", "method": "create", "params": ["article", {"author": "John Doe", "title": "In memoriam", "text": "text"}]}
+2024-05-29 16:03:58,490 : Thread-1 : surrealist.clients.websocket : DEBUG : Get message b'{"id":"9bbc90d7-d6dc-4a51-ad97-b765e6b09131","result":[{"author":"John Doe","id":"article:72duj8mef1s97c67dv38","text":"text","title":"In memoriam"}]}'
+2024-05-29 16:03:58,491 : MainThread : surrealist.connections.websocket : INFO : Got result: SurrealResult(id=9bbc90d7-d6dc-4a51-ad97-b765e6b09131, status=OK, result=[{'author': 'John Doe', 'id': 'article:72duj8mef1s97c67dv38', 'text': 'text', 'title': 'In memoriam'}], query=None, code=None, time=None, additional_info={})
+2024-05-29 16:03:58,491 : MainThread : surrealist.connection : INFO : The connection was closed
+2024-05-29 16:03:58,491 : Thread-1 : surrealist.clients.websocket : DEBUG : Close connection to ws://127.0.0.1:8000/rpc
+2024-05-29 16:03:58,491 : MainThread : surrealist.clients.websocket : DEBUG : Client is closed connection to ws://127.0.0.1:8000/rpc
 ```
 
 **Note:** passwords and auth information always masked in logs. If you still see it in logs - please, report an issue
 
+
 ## Live Query ##
 Live queries let you subscribe to events of desired table when changes happen—you get notification as a simple result or in DIFF format
 
 About live query: https://surrealdb.com/products/lq
 
 Using live select: https://surrealdb.com/docs/surrealdb/surrealql/statements/live
```

### Comparing `surrealist-0.5.1/src/surrealist.egg-info/SOURCES.txt` & `surrealist-0.5.2/src/surrealist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

