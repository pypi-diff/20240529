# Comparing `tmp/sqlalchemy_altibase7-0.0.2.tar.gz` & `tmp/sqlalchemy_altibase7-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_altibase7-0.0.2.tar", last modified: Sun May 26 10:12:29 2024, max compression
+gzip compressed data, was "sqlalchemy_altibase7-0.0.3.tar", last modified: Wed May 29 03:51:54 2024, max compression
```

## Comparing `sqlalchemy_altibase7-0.0.2.tar` & `sqlalchemy_altibase7-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 hess      (1000) hess      (1000)        0 2024-05-26 10:12:29.215192 sqlalchemy_altibase7-0.0.2/
--rw-r--r--   0 hess      (1000) hess      (1000)     2885 2024-05-26 10:12:29.215192 sqlalchemy_altibase7-0.0.2/PKG-INFO
--rw-rw-r--   0 hess      (1000) hess      (1000)     1895 2024-05-26 10:06:48.000000 sqlalchemy_altibase7-0.0.2/README.md
--rw-rw-r--   0 hess      (1000) hess      (1000)     1699 2024-05-26 10:11:14.000000 sqlalchemy_altibase7-0.0.2/pyproject.toml
--rw-rw-r--   0 hess      (1000) hess      (1000)       38 2024-05-26 10:12:29.215192 sqlalchemy_altibase7-0.0.2/setup.cfg
-drwxrwxr-x   0 hess      (1000) hess      (1000)        0 2024-05-26 10:12:29.211192 sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7/
--rw-r--r--   0 hess      (1000) hess      (1000)      849 2024-05-26 06:06:54.000000 sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7/__init__.py
--rw-r--r--   0 hess      (1000) hess      (1000)    25580 2024-05-26 06:19:21.000000 sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7/base.py
--rw-r--r--   0 hess      (1000) hess      (1000)     5472 2024-05-26 06:19:12.000000 sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7/pyodbc.py
--rw-r--r--   0 hess      (1000) hess      (1000)     2422 2024-02-02 01:25:59.000000 sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7/requirements.py
-drwxrwxr-x   0 hess      (1000) hess      (1000)        0 2024-05-26 10:12:29.211192 sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7.egg-info/
--rw-r--r--   0 hess      (1000) hess      (1000)     2885 2024-05-26 10:12:29.000000 sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7.egg-info/PKG-INFO
--rw-rw-r--   0 hess      (1000) hess      (1000)      508 2024-05-26 10:12:29.000000 sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7.egg-info/SOURCES.txt
--rw-rw-r--   0 hess      (1000) hess      (1000)        1 2024-05-26 10:12:29.000000 sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7.egg-info/dependency_links.txt
--rw-rw-r--   0 hess      (1000) hess      (1000)       91 2024-05-26 10:12:29.000000 sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7.egg-info/entry_points.txt
--rw-rw-r--   0 hess      (1000) hess      (1000)      112 2024-05-26 10:12:29.000000 sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7.egg-info/requires.txt
--rw-rw-r--   0 hess      (1000) hess      (1000)       21 2024-05-26 10:12:29.000000 sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7.egg-info/top_level.txt
-drwxrwxr-x   0 hess      (1000) hess      (1000)        0 2024-05-26 10:12:29.211192 sqlalchemy_altibase7-0.0.2/test/
--rw-r--r--   0 hess      (1000) hess      (1000)     2075 2024-05-26 06:04:06.000000 sqlalchemy_altibase7-0.0.2/test/test_altibase_specific.py
--rw-r--r--   0 hess      (1000) hess      (1000)     1999 2024-02-02 01:25:59.000000 sqlalchemy_altibase7-0.0.2/test/test_suite_alembic.py
--rw-r--r--   0 hess      (1000) hess      (1000)     6706 2024-02-02 01:25:59.000000 sqlalchemy_altibase7-0.0.2/test/test_suite_sqlalchemy.py
+drwxrwxr-x   0 hess      (1000) hess      (1000)        0 2024-05-29 03:51:54.435722 sqlalchemy_altibase7-0.0.3/
+-rw-r--r--   0 hess      (1000) hess      (1000)     2489 2024-05-29 03:51:54.435722 sqlalchemy_altibase7-0.0.3/PKG-INFO
+-rw-rw-r--   0 hess      (1000) hess      (1000)     1502 2024-05-29 03:51:01.000000 sqlalchemy_altibase7-0.0.3/README.md
+-rw-rw-r--   0 hess      (1000) hess      (1000)     1695 2024-05-27 03:23:19.000000 sqlalchemy_altibase7-0.0.3/pyproject.toml
+-rw-rw-r--   0 hess      (1000) hess      (1000)       38 2024-05-29 03:51:54.435722 sqlalchemy_altibase7-0.0.3/setup.cfg
+drwxrwxr-x   0 hess      (1000) hess      (1000)        0 2024-05-29 03:51:54.431722 sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7/
+-rw-r--r--   0 hess      (1000) hess      (1000)      849 2024-05-26 06:06:54.000000 sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7/__init__.py
+-rw-r--r--   0 hess      (1000) hess      (1000)    26004 2024-05-29 00:34:12.000000 sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7/base.py
+-rw-r--r--   0 hess      (1000) hess      (1000)     5472 2024-05-26 06:19:12.000000 sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7/pyodbc.py
+-rw-r--r--   0 hess      (1000) hess      (1000)     2422 2024-02-02 01:25:59.000000 sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7/requirements.py
+drwxrwxr-x   0 hess      (1000) hess      (1000)        0 2024-05-29 03:51:54.435722 sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7.egg-info/
+-rw-r--r--   0 hess      (1000) hess      (1000)     2489 2024-05-29 03:51:54.000000 sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7.egg-info/PKG-INFO
+-rw-rw-r--   0 hess      (1000) hess      (1000)      508 2024-05-29 03:51:54.000000 sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7.egg-info/SOURCES.txt
+-rw-rw-r--   0 hess      (1000) hess      (1000)        1 2024-05-29 03:51:54.000000 sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7.egg-info/dependency_links.txt
+-rw-rw-r--   0 hess      (1000) hess      (1000)       91 2024-05-29 03:51:54.000000 sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7.egg-info/entry_points.txt
+-rw-rw-r--   0 hess      (1000) hess      (1000)      109 2024-05-29 03:51:54.000000 sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7.egg-info/requires.txt
+-rw-rw-r--   0 hess      (1000) hess      (1000)       21 2024-05-29 03:51:54.000000 sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7.egg-info/top_level.txt
+drwxrwxr-x   0 hess      (1000) hess      (1000)        0 2024-05-29 03:51:54.435722 sqlalchemy_altibase7-0.0.3/test/
+-rw-r--r--   0 hess      (1000) hess      (1000)     2075 2024-05-26 06:04:06.000000 sqlalchemy_altibase7-0.0.3/test/test_altibase_specific.py
+-rw-r--r--   0 hess      (1000) hess      (1000)     1999 2024-02-02 01:25:59.000000 sqlalchemy_altibase7-0.0.3/test/test_suite_alembic.py
+-rw-r--r--   0 hess      (1000) hess      (1000)     6706 2024-02-02 01:25:59.000000 sqlalchemy_altibase7-0.0.3/test/test_suite_sqlalchemy.py
```

### Comparing `sqlalchemy_altibase7-0.0.2/pyproject.toml` & `sqlalchemy_altibase7-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 [project]
 name = "sqlalchemy_altibase7"
 description ="Altibase for SQLAlchemy"
 authors = [{name = "Hess Lee", email = "hess.lee@altibase.com"}]
 license = {text = "MIT"}
 readme = "README.md"
 keywords=["SQLAlchemy Altibase"]
-dependencies = ["odbcinst", "pyodbc", "sqlalchemy>=1.3.24, <2"]
+dependencies = ["odbcinst", "pyodbc", "sqlalchemy>=1.3.24"]
 #### dynamic = ["version"]
-version = "0.0.2"
+version = "0.0.3"
 classifiers=[
           "Development Status :: 1 - Planning",
         # "Development Status :: 2 - Pre-Alpha",
         # "Development Status :: 3 - Alpha",
         # "Development Status :: 4 - Beta",
         # "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7/__init__.py` & `sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7/base.py` & `sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,25 @@
     BIGINT,
     BLOB,
     CHAR,
     CLOB,
     DATE,
     DECIMAL,
     FLOAT,
+    NUMERIC,
+    REAL,
+    DOUBLE,
     INTEGER,
     NCHAR,
     NVARCHAR,
     SMALLINT,
     VARCHAR,
 )
 from sqlalchemy import util
-from sqlalchemy.util import py2k, warn
+from sqlalchemy.util import warn #,py2k
 from itertools import groupby
 import re
 
 RESERVED_WORDS = set(
     [
         "_PROWID",
         "FIFO",
@@ -324,18 +327,19 @@
     "CHAR": CHAR,
     "VARCHAR": VARCHAR,
     "VARCHAR2": VARCHAR,
     "NCHAR": NCHAR,
     "NVARCHAR": NVARCHAR,
     "CLOB": CLOB,
     "BLOB": BLOB,
-    "NUMBER": oracle_base.NUMBER,
+    "NUMBER": NUMERIC,  #oracle_base.NUMBER,
+    "NUMERIC": NUMERIC,
     "FLOAT": FLOAT,
-    "REAL": oracle_base.BINARY_FLOAT,
-    "DOUBLE": oracle_base.BINARY_DOUBLE,
+    "REAL": REAL,       #oracle_base.BINARY_FLOAT,
+    "DOUBLE": DOUBLE,   #oracle_base.BINARY_DOUBLE,
     "DECIMAL": DECIMAL,
     "BIGINT": BIGINT,
     "INTEGER": INTEGER,
     "SMALLINT": SMALLINT,
     "DATE": DATE,
     "BYTE": BYTE,
     "NIBBLE": NIBBLE,
@@ -346,17 +350,25 @@
 
 
 class AltibaseInspector(reflection.Inspector):
     def __init__(self, conn):
         reflection.Inspector.__init__(self, conn)
 
 
-class AltibaseExecutionContext(oracle_base.OracleExecutionContext):
-    pass
+#class AltibaseExecutionContext(oracle_base.OracleExecutionContext):
+#    pass
 
+class AltibaseExecutionContext(default.DefaultExecutionContext):
+    def fire_sequence(self, seq, type_):
+        return self._execute_scalar(
+            "SELECT "
+            + self.identifier_preparer.format_sequence(seq)
+            + ".nextval FROM DUAL",
+            type_,
+        )
 
 class AltibaseSQLCompiler(oracle_base.OracleCompiler):
     def limit_clause(self, select, **kw):
         if select._limit_clause is None and select._offset_clause is None:
             return ""
         elif select._offset_clause is not None:
             if select._limit_clause is None:
@@ -408,14 +420,15 @@
 
     supports_comments = True
 
     supports_default_values = False
     supports_default_metavalue = True
     supports_empty_insert = False
     supports_identity_columns = True
+    _supports_offset_fetch = False
 
     type_compiler = AltibaseTypeCompiler
     statement_compiler = AltibaseSQLCompiler
     ddl_compiler = AltibaseDDLCompiler
     preparer = AltibaseIdentifierPreparer
     inspector = AltibaseInspector
     oracle_dialect = oracle_base.OracleDialect
@@ -845,16 +858,16 @@
 
         params = {"view_name": self.denormalize_name(view_name)}
         params["user_name"] = self.denormalize_name(schema)
 
         rp = "".join(connection.execute(text(query), params).scalars().all())
 
         if rp:
-            if py2k:
-                rp = rp.decode(self.encoding)
+            #if py2k:
+            #    rp = rp.decode(self.encoding)
             return rp
         else:
             return None
 
 
 # If alembic is installed, register an alias in its dialect mapping.
 try:
```

### Comparing `sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7/pyodbc.py` & `sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7/pyodbc.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_altibase7-0.0.2/sqlalchemy_altibase7/requirements.py` & `sqlalchemy_altibase7-0.0.3/sqlalchemy_altibase7/requirements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_altibase7-0.0.2/test/test_altibase_specific.py` & `sqlalchemy_altibase7-0.0.3/test/test_altibase_specific.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_altibase7-0.0.2/test/test_suite_alembic.py` & `sqlalchemy_altibase7-0.0.3/test/test_suite_alembic.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_altibase7-0.0.2/test/test_suite_sqlalchemy.py` & `sqlalchemy_altibase7-0.0.3/test/test_suite_sqlalchemy.py`

 * *Files identical despite different names*

