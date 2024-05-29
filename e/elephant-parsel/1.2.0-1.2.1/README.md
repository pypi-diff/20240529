# Comparing `tmp/elephant_parsel-1.2.0.tar.gz` & `tmp/elephant_parsel-1.2.1.tar.gz`

## Comparing `elephant_parsel-1.2.0.tar` & `elephant_parsel-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 elephant_parsel-1.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 elephant_parsel-1.2.0/requirements.txt
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 elephant_parsel-1.2.0/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 elephant_parsel-1.2.0/docs/Makefile
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 elephant_parsel-1.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 elephant_parsel-1.2.0/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elephant_parsel-1.2.0/src/elephant_parsel/__init__.py
--rw-r--r--   0        0        0    14680 2020-02-02 00:00:00.000000 elephant_parsel-1.2.0/src/elephant_parsel/postgres_db.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 elephant_parsel-1.2.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 elephant_parsel-1.2.0/LICENSE
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 elephant_parsel-1.2.0/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 elephant_parsel-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 elephant_parsel-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 elephant_parsel-1.2.1/.readthedocs.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 elephant_parsel-1.2.1/requirements.txt
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 elephant_parsel-1.2.1/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 elephant_parsel-1.2.1/docs/Makefile
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 elephant_parsel-1.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 elephant_parsel-1.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elephant_parsel-1.2.1/src/elephant_parsel/__init__.py
+-rw-r--r--   0        0        0    14676 2020-02-02 00:00:00.000000 elephant_parsel-1.2.1/src/elephant_parsel/postgres_db.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 elephant_parsel-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 elephant_parsel-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 elephant_parsel-1.2.1/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 elephant_parsel-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 elephant_parsel-1.2.1/PKG-INFO
```

### Comparing `elephant_parsel-1.2.0/.readthedocs.yaml` & `elephant_parsel-1.2.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `elephant_parsel-1.2.0/.github/workflows/publish-to-test-pypi.yml` & `elephant_parsel-1.2.1/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `elephant_parsel-1.2.0/docs/Makefile` & `elephant_parsel-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `elephant_parsel-1.2.0/docs/source/conf.py` & `elephant_parsel-1.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `elephant_parsel-1.2.0/src/elephant_parsel/postgres_db.py` & `elephant_parsel-1.2.1/src/elephant_parsel/postgres_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         cur.execute(b''.join(parts))
         if fetch:
             result.extend(cur.fetchall())
 
     return result
 
 
-class PostgresDBException(BaseException):
+class PostgresDBException(Exception):
     pass
 
 
 def _format_rows(rows: list, map_row, column) -> list:
     if column:
         return [row[column] for row in rows]
     if map_row:
```

### Comparing `elephant_parsel-1.2.0/.gitignore` & `elephant_parsel-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `elephant_parsel-1.2.0/LICENSE` & `elephant_parsel-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elephant_parsel-1.2.0/README.md` & `elephant_parsel-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `elephant_parsel-1.2.0/pyproject.toml` & `elephant_parsel-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "elephant_parsel"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="betanummeric", email="40263343+betanummeric@users.noreply.github.com" },
 ]
 description = "wrapper for PostgreSQL queries with transaction and connection pooling support"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `elephant_parsel-1.2.0/PKG-INFO` & `elephant_parsel-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elephant_parsel
-Version: 1.2.0
+Version: 1.2.1
 Summary: wrapper for PostgreSQL queries with transaction and connection pooling support
 Project-URL: Homepage, https://github.com/betanummeric/elephant_parsel
 Project-URL: Bug Tracker, https://github.com/betanummeric/elephant_parsel/issues
 Project-URL: Documentation, https://elephant-parsel.readthedocs.io/en/latest/
 Author-email: betanummeric <40263343+betanummeric@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

