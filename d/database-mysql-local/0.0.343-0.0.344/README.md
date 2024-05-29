# Comparing `tmp/database_mysql_local-0.0.343.tar.gz` & `tmp/database_mysql_local-0.0.344.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.343.tar", last modified: Wed May 29 12:32:00 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.344.tar", last modified: Wed May 29 15:18:16 2024, max compression
```

## Comparing `database_mysql_local-0.0.343.tar` & `database_mysql_local-0.0.344.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:32:00.564662 database_mysql_local-0.0.343/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-29 12:32:00.564662 database_mysql_local-0.0.343/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:32:00.552662 database_mysql_local-0.0.343/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:32:00.564662 database_mysql_local-0.0.343/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    58562 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31606 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   652104 2024-05-29 12:31:28.000000 database_mysql_local-0.0.343/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:32:00.564662 database_mysql_local-0.0.343/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-29 12:32:00.000000 database_mysql_local-0.0.343/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-29 12:32:00.000000 database_mysql_local-0.0.343/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:32:00.000000 database_mysql_local-0.0.343/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-29 12:32:00.000000 database_mysql_local-0.0.343/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 12:32:00.000000 database_mysql_local-0.0.343/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-29 12:31:12.000000 database_mysql_local-0.0.343/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:32:00.564662 database_mysql_local-0.0.343/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-29 12:31:04.000000 database_mysql_local-0.0.343/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:18:16.683164 database_mysql_local-0.0.344/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-29 15:18:16.683164 database_mysql_local-0.0.344/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:18:16.679165 database_mysql_local-0.0.344/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:18:16.683164 database_mysql_local-0.0.344/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58562 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31606 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   246093 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   652104 2024-05-29 15:17:41.000000 database_mysql_local-0.0.344/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:18:16.683164 database_mysql_local-0.0.344/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-29 15:18:16.000000 database_mysql_local-0.0.344/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-29 15:18:16.000000 database_mysql_local-0.0.344/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:18:16.000000 database_mysql_local-0.0.344/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-29 15:18:16.000000 database_mysql_local-0.0.344/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 15:18:16.000000 database_mysql_local-0.0.344/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-29 15:17:21.000000 database_mysql_local-0.0.344/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:18:16.683164 database_mysql_local-0.0.344/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-29 15:17:13.000000 database_mysql_local-0.0.344/setup.py
```

### Comparing `database_mysql_local-0.0.343/PKG-INFO` & `database_mysql_local-0.0.344/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.343
+Version: 0.0.344
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.343/README.md` & `database_mysql_local-0.0.344/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.344/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.344/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.344/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/generate_table_columns.py` & `database_mysql_local-0.0.344/database_mysql_local/src/generate_table_columns.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
+import os
 
 from database_mysql_local.connector import Connector
 
-# TODO Why can't we use Sql2Code? - If needed to improve Sql2Code. We prefer only Sql2Code to generate those structures.
+# TODO improve Sql2Code. We prefer only Sql2Code to generate those structures.
 
 connection = Connector.connect(schema_name="test")
 try:
     tables_and_columns = {}
     cursor = connection.cursor()
     query = """SELECT TABLE_NAME, COLUMN_NAME 
                 FROM INFORMATION_SCHEMA.COLUMNS 
@@ -16,14 +17,14 @@
     cursor.execute(query)
     result = cursor.fetchall()
 
     # Process the results and group by table name
     for row in result:
         table_name, column_name = row
         if table_name not in tables_and_columns:
-            tables_and_columns[table_name] = tuple()
-        tables_and_columns[table_name] += (column_name, )
+            tables_and_columns[table_name] = []
+        tables_and_columns[table_name].append(column_name)
     table_columns_json = json.dumps(tables_and_columns, indent=4).replace("[", "(").replace("]", ")")
     with open("table_columns.py", "w") as f:
-        f.write(f"table_columns = {json.dumps(tables_and_columns, indent=4)}")
+        f.write(f"table_columns = {table_columns_json}")
 finally:
-    connection.close()
+    connection.close()
```

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.344/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.344/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.344/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/point.py` & `database_mysql_local-0.0.344/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.344/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.344/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.344/database_mysql_local/src/table_columns.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# TODO: generate with sql2code once ready
+# Generated locally
 table_columns = {
     "action_table": (
         "action_id",
         "name",
         "description",
         "is_queue_action",
         "is_smartlink_action",
@@ -1707,14 +1707,32 @@
         "created_effective_user_id",
         "created_effective_profile_id",
         "updated_timestamp",
         "updated_real_user_id",
         "updated_effective_user_id",
         "updated_effective_profile_id"
     ),
+    "criteria_set_profile_view": (
+        "criteria_set_profile_id",
+        "number",
+        "identifier",
+        "batch_timestamp",
+        "criteria_set_id",
+        "profile_id",
+        "visibility_id",
+        "is_test_data",
+        "created_timestamp",
+        "created_real_user_id",
+        "created_effective_user_id",
+        "created_effective_profile_id",
+        "updated_timestamp",
+        "updated_real_user_id",
+        "updated_effective_user_id",
+        "updated_effective_profile_id"
+    ),
     "criteria_promotional_message_to_person_table": (
         "criteria_promotional_message_to_person_id",
         "criteria_id",
         "multiply_from_yesterday",
         "promotional_message_to_person_id",
         "created_timestamp",
         "created_user_id",
@@ -2230,14 +2248,40 @@
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
         "profile_id_old"
     ),
+    "email_address_profile_general_view": (
+        "email_address_profile_id",
+        "email_address_id",
+        "profile_id",
+        "is_main",
+        "is_sure",
+        "start_timestamp",
+        "end_timestamp",
+        "created_timestamp",
+        "created_user_id",
+        "created_real_user_id",
+        "created_effective_user_id",
+        "created_effective_profile_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "updated_real_user_id",
+        "updated_effective_user_id",
+        "updated_effective_profile_id",
+        "email_address_of_profile",
+        "person_id",
+        "email_address_person_id",
+        "email_address_of_person",
+        "contact_id",
+        "contact_email_address_id",
+        "email_address_of_contact"
+    ),
     "email_address_profile_table": (
         "email_address_profile_id",
         "email_address_id",
         "profile_id",
         "is_main",
         "is_sure",
         "start_timestamp",
@@ -2906,14 +2950,15 @@
         "max_message_template"
     ),
     "form_table": (
         "form_id",
         "number",
         "identifier",
         "name",
+        "form_type_id",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "created_real_user_id",
         "created_effective_user_id",
@@ -2922,14 +2967,15 @@
         "updated_user_id",
         "updated_real_user_id",
         "updated_effective_user_id",
         "updated_effective_profile_id"
     ),
     "form_type_table": (
         "form_type_table_id",
+        "name",
         "version",
         "channel_type_id"
     ),
     "form_transaction_table": (
         "form_transaction_id",
         "form_id",
         "previous_form_id",
@@ -4012,15 +4058,15 @@
     ),
     "city_ml_table": (
         "city_ml_id",
         "city_id",
         "lang_code",
         "is_main",
         "title",
-        "title_approved",
+        "is_title_approved",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
         "is_test_data"
@@ -4052,14 +4098,34 @@
         "country_id_old",
         "is_test_data",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id"
     ),
+    "country_general_view": (
+        "country_id",
+        "identifier",
+        "coordinate",
+        "iso",
+        "name",
+        "nicename",
+        "iso3",
+        "numcode",
+        "phonecode",
+        "group_id",
+        "is_test_data",
+        "created_timestamp",
+        "created_user_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "title",
+        "group.name",
+        "group.title"
+    ),
     "country_ml_table": (
         "country_ml_id",
         "number",
         "identifier",
         "country_id",
         "country_id_old",
         "lang_code",
@@ -4092,15 +4158,31 @@
         "phonecode",
         "lang_code",
         "title",
         "is_title_approved"
     ),
     "country_table": (
         "country_id",
-        "country_id_old",
+        "identifier",
+        "coordinate",
+        "iso",
+        "name",
+        "nicename",
+        "iso3",
+        "numcode",
+        "phonecode",
+        "group_id",
+        "is_test_data",
+        "created_timestamp",
+        "created_user_id",
+        "updated_timestamp",
+        "updated_user_id"
+    ),
+    "country_view": (
+        "country_id",
         "identifier",
         "coordinate",
         "iso",
         "name",
         "nicename",
         "iso3",
         "numcode",
@@ -4236,27 +4318,32 @@
         "neighborhood_id",
         "city_id",
         "county_id",
         "region_id",
         "state_id",
         "country_id",
         "postal_code",
-        "plus_code",
+        "phonecode",
         "is_approved",
         "is_test_data",
         "is_community_active",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
         "start_timestamp",
         "end_timestamp",
+        "location_ml.title",
+        "location.is_title_approved",
         "country_name",
-        "state_name",
-        "city_name"
+        "country_ml.is_title_approved",
+        "state_ml.title",
+        "state_ml.is_title_approved",
+        "city_ml.title",
+        "city_ml.is_title_approved"
     ),
     "location_list_member_table": (
         "location_list_member_id",
         "location_list_id",
         "location_id",
         "created_timestamp",
         "created_user_id",
@@ -4276,15 +4363,27 @@
         "end_timestamp"
     ),
     "location_ml_table": (
         "location_ml_id",
         "location_id",
         "lang_code",
         "title",
-        "title_approved",
+        "is_title_approved",
+        "created_timestamp",
+        "created_user_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "is_test_data"
+    ),
+    "location_ml_view": (
+        "location_ml_id",
+        "location_id",
+        "lang_code",
+        "title",
+        "is_title_approved",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
         "is_test_data"
     ),
     "location_table": (
@@ -4298,15 +4397,15 @@
         "neighborhood_id",
         "county_id",
         "city_id",
         "region_id",
         "state_id",
         "country_id",
         "postal_code",
-        "plus_code",
+        "phonecode",
         "is_approved",
         "is_community_active",
         "group_id",
         "visibility_id",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
@@ -4366,15 +4465,15 @@
         "neighborhood_id",
         "county_id",
         "city_id",
         "region_id",
         "state_id",
         "country_id",
         "postal_code",
-        "plus_code",
+        "phonecode",
         "is_approved",
         "is_community_active",
         "group_id",
         "visibility_id",
         "created_timestamp",
         "created_user_id",
         "created_real_user_id",
@@ -4393,45 +4492,49 @@
     ),
     "neighborhood_ml_table": (
         "neighborhood_ml_id",
         "neighborhood_id",
         "lang_code",
         "is_main",
         "title",
-        "title_approved",
+        "is_title_approved",
+        "is_test_data",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
-        "updated_user_id",
-        "is_test_data"
+        "updated_user_id"
     ),
     "neighborhood_ml_view": (
         "neighborhood_id",
         "city_id",
+        "name",
+        "neighborhood.end_timestamp",
         "lang_code",
         "title",
-        "end_timestamp"
+        "group_id",
+        "group.name"
     ),
     "neighborhood_ml_with_deleted_and_test_data_view": (
         "neighborhood_ml_id",
         "neighborhood_id",
         "lang_code",
         "is_main",
         "title",
-        "title_approved",
+        "is_title_approved",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
         "is_test_data",
         "city_id"
     ),
     "neighborhood_table": (
         "neighborhood_id",
         "number",
+        "name",
         "city_id",
         "coordinate",
         "group_id",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
@@ -4452,70 +4555,81 @@
         "updated_user_id"
     ),
     "region_ml_table": (
         "region_ml_id",
         "region_id",
         "lang_code",
         "title",
-        "title_approved",
+        "is_title_approved",
+        "is_test_data",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
-        "is_test_data"
+        "end_timestamp"
     ),
     "region_ml_view": (
         "region_id",
         "country_id",
+        "group_id",
+        "is_test_data",
         "lang_code",
-        "title"
+        "title",
+        "is_title_approved",
+        "group.name"
     ),
     "region_ml_with_deleted_and_test_data_view": (
         "region_ml_id",
         "region_id",
         "lang_code",
         "title",
-        "title_approved",
+        "is_title_approved",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
         "is_test_data",
-        "country_id"
+        "country_id",
+        "group_id",
+        "region.end_timestamp",
+        "region_ml.end_timestamp"
     ),
     "region_table": (
         "region_id",
+        "number",
+        "name",
         "country_id",
         "coordinate",
         "group_id",
+        "is_test_data",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
-        "number",
-        "is_test_data"
+        "end_timestamp"
     ),
     "state_ml_table": (
         "state_ml_id",
         "state_id",
         "lang_code",
-        "state_name",
-        "state_name_approved",
+        "title",
+        "is_title_approved",
         "state_abbr",
         "state_abbr_approved",
         "is_test_data",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id"
     ),
     "state_ml_view": (
         "state_id",
         "lang_code",
-        "state_name"
+        "title",
+        "is_title_approved"
     ),
     "state_table": (
         "state_id",
         "name",
         "number",
         "country_id",
         "coordinate",
@@ -4538,15 +4652,15 @@
         "neighborhood_id",
         "county_id",
         "city_id",
         "region_id",
         "state_id",
         "country_id",
         "postal_code",
-        "plus_code",
+        "phonecode",
         "is_approved",
         "is_community_active",
         "group_id",
         "visibility_id",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
@@ -4573,15 +4687,15 @@
         "neighborhood_id",
         "county_id",
         "city_id",
         "region_id",
         "state_id",
         "country_id",
         "postal_code",
-        "plus_code",
+        "phonecode",
         "is_approved",
         "is_community_active",
         "group_id",
         "visibility_id",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
@@ -5833,19 +5947,19 @@
         "bcc_profile_list_id",
         "bcc_email",
         "group_list_id",
         "occurrence_id",
         "location_id",
         "message_channel_id",
         "message_type_id",
-        "push_notification",
+        "is_push_notification",
         "group_id",
         "session_id",
         "visibility_id",
-        "pin",
+        "is_pin",
         "mailbox_id",
         "is_gen_ai",
         "machine_learning_model_id",
         "is_require_moderator",
         "moderator_profile_id",
         "moderator_feedback_type",
         "moderator_feedback_text",
@@ -5911,14 +6025,15 @@
     "message_type_table": (
         "message_type_table_id",
         "version",
         "channel_type_id"
     ),
     "message_view": (
         "message_id",
+        "number",
         "identifier",
         "parent_message_id",
         "message_message_relationship_id",
         "sender_profile_id",
         "sender_email",
         "to_profile_id",
         "to_profile_list_id",
@@ -5930,19 +6045,19 @@
         "bcc_profile_list_id",
         "bcc_email",
         "group_list_id",
         "occurrence_id",
         "location_id",
         "message_channel_id",
         "message_type_id",
-        "push_notification",
+        "is_push_notification",
         "group_id",
         "session_id",
         "visibility_id",
-        "pin",
+        "is_pin",
         "mailbox_id",
         "is_gen_ai",
         "machine_learning_model_id",
         "is_require_moderator",
         "moderator_profile_id",
         "moderator_feedback_type",
         "moderator_feedback_text",
@@ -5963,32 +6078,37 @@
         "class_parameters_json",
         "function_parameters_json",
         "action_id",
         "campaign_id",
         "requested_channel_id",
         "actual_channel_id",
         "provider_id",
+        "email_message_id",
+        "body",
+        "subject",
+        "compound_message",
+        "compound_message_json_version",
+        "compound_message_json",
+        "session",
         "is_test_data",
         "request_to_send_timestamp",
         "scheduled_sent_timestamp",
         "actual_sent_timestamp",
+        "start_timestamp",
+        "end_timestamp",
         "created_timestamp",
         "created_user_id",
+        "created_real_user_id",
+        "created_effective_user_id",
+        "created_effective_profile_id",
         "updated_timestamp",
         "updated_user_id",
-        "start_timestamp",
-        "end_timestamp",
-        "email_message_id",
-        "body",
-        "subject",
-        "number",
-        "compound_message",
-        "compound_message_json_version",
-        "compound_message_json",
-        "session"
+        "updated_real_user_id",
+        "updated_effective_user_id",
+        "updated_effective_profile_id"
     ),
     "message_profile_table": (
         "message_profile_id",
         "number",
         "identifier",
         "message_id",
         "profile_id",
@@ -6028,14 +6148,15 @@
         "message_template_id",
         "message_template_name",
         "message_template_text_block.criteria_id",
         "message_template_text_block.criteria.name",
         "message_template_text_block_id",
         "message_template_text_block_name",
         "message_template_text_block_is_visible",
+        "message_template_text_block.criteria_set_id",
         "message_template_text_block_seq",
         "question_id",
         "default_question_possible_answer_id",
         "question_is_required",
         "message_template_text_block_ml_lang_code",
         "default_subject_template",
         "default_body_template",
@@ -6113,14 +6234,15 @@
         "lang_code",
         "default_subject_template",
         "default_body_template",
         "sms_body_template",
         "email_subject_template",
         "email_body_html_template",
         "whatsapp_body_template",
+        "smartlink_type_id",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "created_real_user_id",
         "created_effective_user_id",
@@ -6745,61 +6867,40 @@
         "contact_person_type_id",
         "contact_person_type_name",
         "contact_id",
         "contact_first_name",
         "contact_email_address1",
         "contact_created_timestamp"
     ),
-    "person_general_view": (
-        "person_id",
-        "first_name",
-        "last_name",
-        "main_email_person",
-        "person_is_test_data",
-        "person_created_timestamp",
-        "person_end_timestamp",
-        "person_profile_end_timestamp",
-        "person_birthday_date",
-        "profile_id",
-        "profile_main_email_address",
-        "profile_name",
-        "user_id",
-        "profile_main_email",
-        "profile_is_test_data",
-        "profile_end_timestamp",
-        "number_of_contacts",
-        "number_of_profiles",
-        "number_of_phones"
-    ),
     "person_in_all_table_view": (
         "COUNT(person_id)"
     ),
     "person_kid_table": (
         "person_kids_id",
         "person_id",
         "number_of_kids"
     ),
     "person_ml_table": (
         "person_ml_id",
         "person_id",
         "lang_code",
         "first_name",
-        "first_name_approved",
+        "is_first_name_approved",
         "last_name",
-        "last_name_approved",
+        "is_last_name_approved",
         "is_test_data"
     ),
     "person_ml_view": (
         "person_ml_id",
         "person_id",
         "lang_code",
         "first_name",
-        "first_name_approved",
+        "is_first_name_approved",
         "last_name",
-        "last_name_approved",
+        "is_last_name_approved",
         "is_test_data"
     ),
     "person_phone_general_view": (
         "person_id",
         "person.is_test_data",
         "person_phone_id",
         "phone_id",
@@ -6811,29 +6912,14 @@
     "person_probably_test_data_view": (
         "person_id",
         "first_name",
         "last_name",
         "main_email_person",
         "is_test_data"
     ),
-    "person_profile_general_view": (
-        "person_id",
-        "first_name",
-        "last_name",
-        "main_email_person",
-        "person_end_timestamp",
-        "person_profile_end_timestamp",
-        "profile_id",
-        "profile_main_email_address",
-        "profile_name",
-        "user_id",
-        "profile_main_email",
-        "profile_is_test_data",
-        "profile_end_timestamp"
-    ),
     "person_table": (
         "person_id",
         "number",
         "identifier",
         "name",
         "is_approved",
         "is_identity_confirmed",
@@ -6847,14 +6933,17 @@
         "gender_id",
         "first_name",
         "is_first_name_approved",
         "nickname",
         "is_nickname_approved",
         "father_name",
         "last_name",
+        "is_last_name_approved",
+        "is_last_name_sure",
+        "is_last_name_auto_generated",
         "main_email_person",
         "main_full_number_normalized",
         "last_coordinate",
         "last_location_id",
         "location_id",
         "is_rip",
         "visibility_id",
@@ -6868,30 +6957,53 @@
         "created_effective_profile_id",
         "updated_timestamp",
         "updated_user_id",
         "updated_real_user_id",
         "updated_effective_user_id",
         "updated_effective_profile_id"
     ),
-    "person_user_profile_view": (
+    "person_view": (
         "person_id",
-        "person_first_name",
-        "person_is_approve",
-        "user_id",
-        "user_created_timestamp",
+        "number",
+        "identifier",
+        "is_approved",
+        "is_identity_confirmed",
+        "birthday_original",
+        "birthday_timestamp",
+        "birthday_date",
+        "day",
+        "month",
+        "year",
+        "year_cira",
+        "gender_id",
         "first_name",
-        "main_email",
+        "is_first_name_approved",
+        "nickname",
+        "is_nickname_approved",
+        "father_name",
         "last_name",
-        "user stars",
-        "profile_id",
-        "is_main",
-        "profile_preferred_lang_code",
-        "profile stars",
-        "brand_id",
-        "login_timestamp"
+        "main_email_person",
+        "last_coordinate",
+        "last_location_id",
+        "location_id",
+        "is_rip",
+        "is_test_data",
+        "start_timestamp",
+        "end_timestamp",
+        "created_timestamp",
+        "created_user_id",
+        "created_real_user_id",
+        "created_effective_user_id",
+        "created_effective_profile_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "updated_real_user_id",
+        "updated_effective_user_id",
+        "updated_effective_profile_id",
+        "visibility_id"
     ),
     "person_profile_table": (
         "person_profile_id",
         "number",
         "identifier",
         "person_id",
         "profile_id",
@@ -7152,28 +7264,30 @@
         "updated_real_user_id",
         "updated_effective_user_id",
         "updated_effective_profile_id"
     ),
     "profile_approved_en_main_view": (
         "profile_id",
         "number",
-        "user_id",
+        "main_user_id",
+        "main_person_id",
         "is_main",
         "visibility_id",
         "is_approved",
         "profile_type_id",
         "preferred_lang_code",
         "experience_years_min",
         "is_rip",
         "last_dialog_workflow_state_id"
     ),
     "profile_approved_en_view": (
         "id_profile",
         "number",
-        "user_id",
+        "main_user_id",
+        "main_person_id",
         "is_main",
         "visibility_id",
         "is_approved",
         "profile_type_id",
         "preferred_lang_code",
         "experience_years_min",
         "is_rip",
@@ -7211,54 +7325,55 @@
         "updated_real_user_id",
         "updated_effective_user_id",
         "updated_effective_profile_id"
     ),
     "profile_en_view": (
         "id_profile",
         "number",
-        "user_id",
+        "main_user_id",
+        "main_person_id",
         "is_main",
         "visibility_id",
         "is_approved",
         "profile_type_id",
         "preferred_lang_code",
         "experience_years_min",
         "is_rip",
         "last_dialog_workflow_state_id"
     ),
     "profile_general_view": (
         "profile_id",
         "number",
         "profile_name",
-        "user_id",
-        "person_id",
+        "main_user_id",
+        "main_person_id",
         "is_main",
         "visibility_id",
         "is_approved",
         "profile_type_id",
         "preferred_lang_code",
         "experience_years_min",
         "main_phone_id",
         "profile_main_email",
         "is_rip",
-        "profile_gender_id",
+        "profile.gender_id",
         "stars",
         "last_dialog_workflow_state_id",
         "is_system",
         "internal_description",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
         "title",
         "profile_ml.title",
-        "person_id_in_profile_table",
+        "main_person_id_in_profile_table",
         "person_id_in_person_table",
         "person_first_name",
         "person_last_name"
     ),
     "profile_history_table": (
         "profile_history_id",
         "profile_id",
@@ -7317,14 +7432,50 @@
         "updated_user_id",
         "updated_real_user_id",
         "updated_effective_user_id",
         "updated_effective_profile_id",
         "start_timestamp",
         "end_timestamp"
     ),
+    "profile_mailbox_general_view": (
+        "profile_id",
+        "number",
+        "profile_name",
+        "main_user_id",
+        "main_person_id",
+        "is_main",
+        "visibility_id",
+        "is_approved",
+        "profile_type_id",
+        "preferred_lang_code",
+        "experience_years_min",
+        "main_phone_id",
+        "profile_main_email",
+        "is_rip",
+        "gender_id",
+        "stars",
+        "last_dialog_workflow_state_id",
+        "is_system",
+        "internal_description",
+        "is_test_data",
+        "start_timestamp",
+        "end_timestamp",
+        "created_timestamp",
+        "created_user_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "title",
+        "profile_ml.title",
+        "main_person_id_in_profile_table",
+        "person_id_in_person_table",
+        "person_first_name",
+        "person_last_name",
+        "mailbox_profile_id",
+        "mailbox_profile_name"
+    ),
     "profile_media_ml_table": (
         "profile_media_ml_id",
         "profile_media_id",
         "lang_code",
         "title",
         "description",
         "start_timestamp",
@@ -7355,54 +7506,14 @@
         "created_real_user_id",
         "created_effective_user_id",
         "updated_timestamp",
         "updated_user_id",
         "updated_real_user_id",
         "updated_effective_user_id"
     ),
-    "profile_ml_approved_en_view": (
-        "profile_id",
-        "number",
-        "user_id",
-        "is_main",
-        "visibility_id",
-        "is_approved",
-        "profile_type_id",
-        "preferred_lang_code",
-        "experience_years_min",
-        "is_rip",
-        "last_dialog_workflow_state_id"
-    ),
-    "profile_ml_approved_view": (
-        "profile_id",
-        "number",
-        "user_id",
-        "is_main",
-        "visibility_id",
-        "is_approved",
-        "profile_type_id",
-        "preferred_lang_code",
-        "experience_years_min",
-        "is_rip",
-        "last_dialog_workflow_state_id"
-    ),
-    "profile_ml_en_view": (
-        "profile_id",
-        "number",
-        "user_id",
-        "is_main",
-        "visibility_id",
-        "is_approved",
-        "profile_type_id",
-        "preferred_lang_code",
-        "experience_years_min",
-        "is_rip",
-        "last_dialog_workflow_state_id",
-        "title"
-    ),
     "profile_ml_table": (
         "profile_ml_id",
         "profile_id",
         "lang_code",
         "is_main",
         "title",
         "title_approved",
@@ -7421,16 +7532,16 @@
         "title"
     ),
     "profile_table": (
         "profile_id",
         "number",
         "identifier",
         "name",
-        "user_id",
-        "person_id",
+        "main_user_id",
+        "main_person_id",
         "is_main",
         "visibility_id",
         "is_approved",
         "profile_type_id",
         "preferred_lang_code",
         "experience_years_min",
         "main_phone_id",
@@ -7502,31 +7613,26 @@
         "updated_timestamp",
         "updated_user_id",
         "updated_real_user_id",
         "updated_effective_user_id",
         "updated_effective_profile_id",
         "is_test_data"
     ),
-    "profile_user_field_view": (
-        "profile_id",
-        "name",
-        "user_id"
-    ),
     "profile_user_table_view": (
         "profile_id",
         "profile_user_id",
         "user_id"
     ),
     "profile_view": (
         "profile_id",
         "number",
         "identifier",
         "name",
-        "user_id",
-        "person_id",
+        "main_user_id",
+        "main_person_id",
         "is_main",
         "is_approved",
         "profile_type_id",
         "preferred_lang_code",
         "experience_years_min",
         "main_phone_id",
         "profile_main_email",
@@ -8821,14 +8927,15 @@
         "system_id",
         "system_entity_id",
         "text_block_type_id",
         "fields_extracted_json",
         "url",
         "visibility_id",
         "is_test_data",
+        "effective_timestamp",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "created_real_user_id",
         "created_effective_user_id",
         "created_effective_profile_id",
```

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.344/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.344/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.344/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.344/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.343
+Version: 0.0.344
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.343/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.344/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.343/pyproject.toml` & `database_mysql_local-0.0.344/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.343" # https://pypi.org/project/database-mysql-local
+version = "0.0.345" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.343/setup.py` & `database_mysql_local-0.0.344/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.343',
+    version='0.0.344',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

