# Comparing `tmp/database_mysql_local-0.0.342.tar.gz` & `tmp/database_mysql_local-0.0.343.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.342.tar", last modified: Tue May 28 17:09:10 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.343.tar", last modified: Wed May 29 12:32:00 2024, max compression
```

## Comparing `database_mysql_local-0.0.342.tar` & `database_mysql_local-0.0.343.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:09:10.879692 database_mysql_local-0.0.342/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-28 17:09:10.879692 database_mysql_local-0.0.342/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:09:10.871692 database_mysql_local-0.0.342/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:09:10.879692 database_mysql_local-0.0.342/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    58532 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31229 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   652104 2024-05-28 17:08:35.000000 database_mysql_local-0.0.342/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:09:10.879692 database_mysql_local-0.0.342/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-28 17:09:10.000000 database_mysql_local-0.0.342/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-28 17:09:10.000000 database_mysql_local-0.0.342/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:09:10.000000 database_mysql_local-0.0.342/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 17:09:10.000000 database_mysql_local-0.0.342/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 17:09:10.000000 database_mysql_local-0.0.342/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 17:08:16.000000 database_mysql_local-0.0.342/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:09:10.879692 database_mysql_local-0.0.342/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-28 17:08:08.000000 database_mysql_local-0.0.342/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:32:00.564662 database_mysql_local-0.0.343/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-29 12:32:00.564662 database_mysql_local-0.0.343/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:32:00.552662 database_mysql_local-0.0.343/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:32:00.564662 database_mysql_local-0.0.343/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58562 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31606 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   652104 2024-05-29 12:31:28.000000 database_mysql_local-0.0.343/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:32:00.564662 database_mysql_local-0.0.343/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-29 12:32:00.000000 database_mysql_local-0.0.343/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-29 12:32:00.000000 database_mysql_local-0.0.343/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:32:00.000000 database_mysql_local-0.0.343/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-29 12:32:00.000000 database_mysql_local-0.0.343/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 12:32:00.000000 database_mysql_local-0.0.343/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-29 12:31:12.000000 database_mysql_local-0.0.343/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:32:00.564662 database_mysql_local-0.0.343/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/setup.py
```

### Comparing `database_mysql_local-0.0.342/PKG-INFO` & `database_mysql_local-0.0.343/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.342
+Version: 0.0.343
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.342/README.md` & `database_mysql_local-0.0.343/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.343/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.343/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.343/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/generate_table_columns.py` & `database_mysql_local-0.0.343/database_mysql_local/src/generate_table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.343/database_mysql_local/src/generic_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
 
     def __get_existing_duplicate_id_with_timestamp(
             self, schema_name: str, table_name: str, duplicate_column_name: str,
             duplicate_value: Any, column_name: str) -> int or None:
         select_query = (
             f"SELECT {column_name}, end_timestamp "
             f"FROM `{schema_name}`.`{table_name}` "
-            f"WHERE {duplicate_column_name} = %s LIMIT 1;"
+            f"WHERE {duplicate_column_name} = %s AND end_timestamp IS NOT NULL LIMIT 1;"
         )
         self.connection.commit()
         self.cursor.execute(select_query, (duplicate_value,))
         row = self.cursor.fetchone()
         if row is None:
             existing_duplicate_id = None
             return existing_duplicate_id
```

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.343/database_mysql_local/src/generic_crud_ml.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # is_main in data_ml_dict
 # table_definition_table.is_main_column
 # I'm not sure we need additional parameter.
 class GenericCRUDML(GenericCRUD, metaclass=MetaLogger, object=LOGGER_CRUD_ML_CODE_OBJECT):
     """A class that provides generic CRUD functionality for tables with multi-language support."""
 
     # TODO: allow overiding all default values in all methods
+    # TODO Shall we add same_entity method as parameter?
     def __init__(self, default_schema_name: str,
                  default_table_name: str = None, default_view_table_name: str = None,
                  default_ml_table_name: str = None, default_ml_view_table_name: str = None,
                  default_view_with_deleted_and_test_data: str = None,
                  default_column_name: str = None, default_id_column_name: str = None,
                  is_main_column_name: str = IS_MAIN_COLUMN_NAME, is_test_data: bool = False) -> None:
         """Initializes the GenericCRUDML class. If connection is not provided,
@@ -127,14 +128,15 @@
             self.connection.rollback()
             raise e
         finally:
             self.cursor.close()
             self.cursor = old_cursor
         return table_id, ml_table_id
 
+    # TODO add parameter if_same_even_deleted_return_existing_id=true - When inserting a deleted entity (all entities except person and tables of codes i.e. country, state, county, city, neighbourhood, street ...) and table_definition.insert_is_undelete=false, we should null all the unique fields of the deleted entity
     def add_value_if_not_exist(
             self, *, data_dict: dict = None, data_ml_dict: dict = None, data_json: dict = None,
             data_ml_json: dict = None, table_id: int = None, lang_code: LangCode = None,
             is_main: bool = False, table_name: str = None, ml_table_name: str = None, schema_name: str = None,
             order_by: str = None) -> (int, int):
         # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
         if not data_ml_dict and not data_ml_json:
```

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.343/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/point.py` & `database_mysql_local-0.0.343/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.343/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.343/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.343/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.343/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.343/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.343/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.343/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.342
+Version: 0.0.343
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.342/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.343/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/pyproject.toml` & `database_mysql_local-0.0.343/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.342/setup.py` & `database_mysql_local-0.0.343/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.342',
+    version='0.0.343',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

