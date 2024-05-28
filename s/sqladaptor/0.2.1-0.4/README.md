# Comparing `tmp/sqladaptor-0.2.1.tar.gz` & `tmp/sqladaptor-0.4.tar.gz`

## Comparing `sqladaptor-0.2.1.tar` & `sqladaptor-0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/.python-version
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/.idea/.gitignore
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/.idea/modules.xml
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/.idea/ruff.xml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/.idea/sqladaptor.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/.idea/vcs.xml
--rw-r--r--   0        0        0    10253 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/.idea/workspace.xml
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/example/db.sqlite
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/example/quick_run.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/src/sqladaptor/__init__.py
--rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/src/sqladaptor/sqlite.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/test/test_sqlite_adaptor.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/.gitignore
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/README.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 sqladaptor-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sqladaptor-0.4/.python-version
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 sqladaptor-0.4/.idea/.gitignore
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sqladaptor-0.4/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sqladaptor-0.4/.idea/modules.xml
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 sqladaptor-0.4/.idea/ruff.xml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 sqladaptor-0.4/.idea/sqladaptor.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sqladaptor-0.4/.idea/vcs.xml
+-rw-r--r--   0        0        0    10650 2020-02-02 00:00:00.000000 sqladaptor-0.4/.idea/workspace.xml
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 sqladaptor-0.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sqladaptor-0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 sqladaptor-0.4/example/db.sqlite
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 sqladaptor-0.4/example/quick_run.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 sqladaptor-0.4/src/sqladaptor/__init__.py
+-rw-r--r--   0        0        0     8693 2020-02-02 00:00:00.000000 sqladaptor-0.4/src/sqladaptor/sqlite.py
+-rw-r--r--   0        0        0     5495 2020-02-02 00:00:00.000000 sqladaptor-0.4/test/test_sqlite_adaptor.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqladaptor-0.4/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 sqladaptor-0.4/LICENSE
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 sqladaptor-0.4/README.md
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 sqladaptor-0.4/pyproject.toml
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 sqladaptor-0.4/PKG-INFO
```

### Comparing `sqladaptor-0.2.1/.idea/sqladaptor.iml` & `sqladaptor-0.4/.idea/sqladaptor.iml`

 * *Files identical despite different names*

### Comparing `sqladaptor-0.2.1/.idea/workspace.xml` & `sqladaptor-0.4/.idea/workspace.xml`

 * *Files 6% similar despite different names*

#### Comparing `sqladaptor-0.2.1/.idea/workspace.xml` & `sqladaptor-0.4/.idea/workspace.xml`

```diff
@@ -1,15 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="f543d5ca-4570-440d-bf15-99b5763dd321" name="Changes" comment="">
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/sqladaptor/sqlite.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/sqladaptor/sqlite.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
@@ -156,15 +158,17 @@
       <workItem from="1716504580504" duration="637000"/>
       <workItem from="1716514704262" duration="1528000"/>
       <workItem from="1716516241964" duration="8805000"/>
       <workItem from="1716531741803" duration="4040000"/>
       <workItem from="1716538104718" duration="1121000"/>
       <workItem from="1716539517401" duration="430000"/>
       <workItem from="1716539990504" duration="1321000"/>
-      <workItem from="1716547503531" duration="87000"/>
+      <workItem from="1716547503531" duration="155000"/>
+      <workItem from="1716721499547" duration="64000"/>
+      <workItem from="1716721602120" duration="1528000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
```

### Comparing `sqladaptor-0.2.1/.idea/inspectionProfiles/Project_Default.xml` & `sqladaptor-0.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `sqladaptor-0.2.1/example/db.sqlite` & `sqladaptor-0.4/example/db.sqlite`

 * *Files identical despite different names*

### Comparing `sqladaptor-0.2.1/example/quick_run.py` & `sqladaptor-0.4/example/quick_run.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 
 entries = [
     {"description": "this", "value": 1},
     {"description": "that", "value": 2},
 ]
 db.set_from_df("data1", pandas.DataFrame(entries))
 
-entries = db.get_dicts("data1")
+entries = db.read_dicts("data1")
 pprint(entries)
 
-schema = db.get_table_schema("test_table")
+schema = db.read_table_schema("test_table")
 validator = fastjsonschema.compile(schema)
 for entry in entries:
     print("validate: ", end="")
     pprint(validator(entry))
 
-entries = db.get_dicts("data1", {"description": "this"})
+entries = db.read_dicts("data1", {"description": "this"})
 pprint(entries)
 
-df = db.get_df("data1", {"value": 2})
+df = db.read_df("data1", {"value": 2})
 pprint(df)
 
 db.update("data1", {"value": 2}, {"description": "altered"})
-entries = db.get_dicts("data1", {"value": 2})
+entries = db.read_dicts("data1", {"value": 2})
 pprint(entries)
 
-rows = db.get_rows("data1")
+rows = db.read_rows("data1")
 pprint(rows)
 
 schema = {
     "type": "object",
     "properties": {
         "description": {"type": "string"},
         "value": {"type": "integer"},
```

### Comparing `sqladaptor-0.2.1/src/sqladaptor/sqlite.py` & `sqladaptor-0.4/src/sqladaptor/sqlite.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import re
 import sqlite3
-from typing import Optional, Union
+from typing import Optional, Union, Literal
 
 import pandas
 from pydash import py_
 
 __doc__ = """
 Interface to an SQLite3 database for storage, with accessor methods to both ingest
 and generate Pandas dataframes or JSON dict lists 
@@ -52,73 +52,118 @@
 
     def close(self):
         self.conn.close()
 
     def execute(self, *args):
         return self.cursor.execute(*args)
 
-    def get_tables(self):
+    def read_tables(self):
         rows = self.execute("SELECT name FROM sqlite_master").fetchall()
         return [r[0] for r in rows]
 
-    def get_table_schema(self, table: str) -> dict:
+    def read_table_schema(self, table: str) -> dict:
+        """
+        Reads the table schema as a json schema of an object. AdditionalProperties
+        are set to False so that json-schema can be used to validate incoming dict.
+
+        :param schema: dict - e.g. {
+            "type": "object",
+            "properties": {
+                "row_id": {"type": "integer"},
+                "description": {"type": "string"},
+                "amount": {"type": "number"},
+                "category": {"type": "string"},
+            },
+            "additionalProperties": False,
+        }
+        """
         queries = self.execute(f"PRAGMA table_info('{table}')").fetchall()
         props = {}
         for query in queries:
             name = query[1]
             data_type = json_type_from_sql_type[query[2]]
             props[name] = {"type": data_type}
-        return {"type": "object", "properties": props}
+        return {"type": "object", "properties": props, "additionalProperties": False}
 
     def create_table(self, table: str, schema: dict):
+        """
+        Creates table with json schema of an object representing table keys.
+        Required properties are interpreted as primary keys.
+
+        :param schema: dict - e.g. {
+            "type": "object",
+            "properties": {
+                "row_id": {"type": "integer"},
+                "description": {"type": "string"},
+                "amount": {"type": "number"},
+                "category": {"type": "string"},
+            },
+            "required": ["row_id"],
+        }
+        """
         columns = []
         for col, props in schema["properties"].items():
             if check_key_characters(col):
                 sql_type = sql_type_from_json_type[props["type"].lower()]
                 s = f"  {col} {sql_type} "
                 if col in schema.get("required", []):
                     s += " PRIMARY KEY"
                 columns.append(s)
         columns_sql = ",".join(columns)
         self.execute(f"CREATE TABLE IF NOT EXISTS {table} (\n{columns_sql}\n)\n")
         self.commit()
 
+    def add_columns(self, table: str, schema: dict):
+        """
+        Adds columns described in a schema to a table.
+
+        :param schema: dict - e.g.
+        {
+            type: "object",
+            "properties": {
+                "column_text_a": { "type": "string" }
+                "column_float_b": { "type": "number" }
+            }
+        }
+        """
+        for name, props in schema["properties"].items():
+            if check_key_characters(name):
+                sqlite_type = sql_type_from_json_type[props["type"].lower()]
+                self.execute(f"ALTER TABLE {table} ADD '{name}' '{sqlite_type}'")
+        self.commit()
+
     def drop_table(self, table: str):
-        if table in self.get_tables():
+        if table in self.read_tables():
             self.execute(f"DROP TABLE {table}")
             self.commit()
 
     def rename_table(self, table: str, new_table: str):
-        if table in self.get_tables():
+        if table in self.read_tables():
             new_table = py_.snake_case(new_table)
             self.execute(f"ALTER TABLE {table} RENAME to {new_table}")
             self.commit()
 
-    def add_column(self, table: str, name: str, col_type: str):
-        self.execute(f"ALTER TABLE {table} ADD COLUMN '{name}' '{col_type}'")
-        self.commit()
-
     def execute_to_df(self, sql: str, params=None):
         return pandas.read_sql_query(sql, self.conn, params=params)
 
     def set_from_df(
-        self, table: str, df: pandas.DataFrame, index=False, if_exists="append"
+            self, table: str, df: pandas.DataFrame, index=False,
+            if_exists: Literal["fail", "append", "replace"] = "append"
     ):
         """
         :param df: pandas.Dataframe
-        :param if_exists: ["fail", "append", "replace"]
         """
         df.to_sql(con=self.conn, name=table, index=index, if_exists=if_exists)
         self.commit()
 
     def replace_with_df(self, table: str, df: pandas.DataFrame, index=False):
         self.set_from_df(table, df, index=index, if_exists="replace")
 
-    def build_condition_sql_params(
-        self, value_by_key: OptionalValueDict, head="WHERE", separator=" AND "
+    def build_condition_sql_and_params(
+            self, value_by_key: OptionalValueDict, head="WHERE", separator=" AND "
     ):
         sql = ""
         params = []
         if value_by_key:
             lines = []
             for k, v in value_by_key.items():
                 if check_key_characters(k):
@@ -126,43 +171,43 @@
                     params.append(str(v))
             if len(lines):
                 column_str = separator.join(lines)
                 sql += f"{head} {column_str} "
         return sql, params
 
     def build_select_sql_and_params(self, table: str, where: OptionalValueDict):
-        where_sql, where_params = self.build_condition_sql_params(where)
+        where_sql, where_params = self.build_condition_sql_and_params(where)
         return f"SELECT * FROM {table} " + where_sql, where_params
 
-    def get_rows(self, table: str, where: OptionalValueDict = None) -> [tuple]:
+    def read_rows(self, table: str, where: OptionalValueDict = None) -> [tuple]:
         sql, params = self.build_select_sql_and_params(table, where)
         return list(self.execute(sql, params))
 
-    def get_one_row(self, table: str, where: OptionalValueDict = None) -> tuple:
+    def read_one_row(self, table: str, where: OptionalValueDict = None) -> tuple:
         sql, params = self.build_select_sql_and_params(table, where)
         return self.execute(sql, params).fetchone()
 
-    def get_df(self, table: str, where: OptionalValueDict = None) -> pandas.DataFrame:
+    def read_df(self, table: str, where: OptionalValueDict = None) -> pandas.DataFrame:
         sql, params = self.build_select_sql_and_params(table, where)
         return pandas.read_sql_query(sql, self.conn, params=params)
 
-    def get_dicts(self, table: str, where: OptionalValueDict = None) -> [dict]:
-        return self.get_df(table, where).to_dict(orient="records")
+    def read_dicts(self, table: str, where: OptionalValueDict = None) -> [dict]:
+        return self.read_df(table, where).to_dict(orient="records")
 
-    def get_one_dict(self, table: str, where: OptionalValueDict = None) -> dict:
+    def read_one_dict(self, table: str, where: OptionalValueDict = None) -> dict:
         sql, params = self.build_select_sql_and_params(table, where)
         df = pandas.read_sql_query(sql + " LIMIT 1", self.conn, params=params)
         entries = df.to_dict(orient="records")
         if len(entries):
             return entries[0]
         else:
             return {}
 
-    def get_csv(self, table: str) -> str:
-        return self.get_df(table).to_csv(index=False)
+    def read_csv(self, table: str) -> str:
+        return self.read_df(table).to_csv(index=False)
 
     def insert(self, table: str, vals):
         """
         :param vals:
             <k>: <v>
         """
         params = []
@@ -187,27 +232,27 @@
         """
         :param vals:
             <k>: <v>
         """
         sql = f"UPDATE {table} "
         params = []
         if vals:
-            set_sql, set_params = self.build_condition_sql_params(
+            set_sql, set_params = self.build_condition_sql_and_params(
                 vals, separator=", ", head="SET"
             )
             params.extend(set_params)
             sql += set_sql + " "
         if where:
-            where_sql, where_params = self.build_condition_sql_params(where)
+            where_sql, where_params = self.build_condition_sql_and_params(where)
             params.extend(where_params)
             sql += where_sql
         self.execute(sql, params)
         self.commit()
 
     def delete(self, table: str, where: OptionalValueDict):
         """
         :param vals:
             <k>: <v>
         """
-        where_sql, params = self.build_condition_sql_params(where)
+        where_sql, params = self.build_condition_sql_and_params(where)
         self.execute(f"DELETE FROM {table} " + where_sql, params)
         self.commit()
```

### Comparing `sqladaptor-0.2.1/test/test_sqlite_adaptor.py` & `sqladaptor-0.4/test/test_sqlite_adaptor.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,23 @@
 import pandas
 import pytest
 from path import Path
 from pydash import py_
 
 from sqladaptor.sqlite import SqliteAdaptor, var_name_regex
 
+
+def test_var_names():
+    assert var_name_regex.fullmatch("__ha__")
+    assert not var_name_regex.fullmatch("1__ha__")
+    assert not var_name_regex.fullmatch("__ ha__")
+    assert not var_name_regex.fullmatch("var#")
+    assert not var_name_regex.fullmatch("v;ar")
+
+
 schema = {
     "type": "object",
     "properties": {
         "row_id": {"type": "integer"},
         "description": {"type": "string"},
         "amount": {"type": "number"},
         "category": {"type": "string"},
@@ -33,89 +42,154 @@
     db.close()
     db_fname.remove_p()
 
 
 def test_get_schema(test_db):
     this_schema = deepcopy(schema)
     del this_schema["required"]
-    return_schmea = test_db.get_table_schema("test_table")
-    assert return_schmea == this_schema
+    return_schmea = test_db.read_table_schema("test_table")
+    del return_schmea["additionalProperties"]
+    assert this_schema == return_schmea
 
 
 def test_insert_row(test_db):
     entry = dict(description="haha", amount=2)
     test_db.insert("test_table", entry)
-    saved_entries = test_db.get_df("test_table").to_dict(orient="records")
+    saved_entries = test_db.read_df("test_table").to_dict(orient="records")
     assert py_.find(saved_entries, entry)
 
 
+def test_insert_df(test_db):
+    entries = [
+        dict(description="haha", amount=2),
+        dict(description="hoho", amount=1),
+        dict(description="hihi", amount=3),
+    ]
+    test_db.set_from_df("test_table", pandas.DataFrame(entries))
+    saved_entries = test_db.read_df("test_table").to_dict(orient="records")
+    for entry in entries:
+        assert py_.find(saved_entries, entry)
+
+
+def test_fail_insert_too_big_df(test_db):
+    entries = [
+        dict(description="haha", amount=2, extra="bad"),
+        dict(description="hoho", amount=1, extra="bad"),
+        dict(description="hihi", amount=3, extra="bad"),
+    ]
+    with pytest.raises(Exception):
+        test_db.set_from_df("test_table", pandas.DataFrame(entries))
+
+
+def test_fail_when_insert_too_much(test_db):
+    entry = dict(description="haha", amount=2, extra_field="haha")
+    with pytest.raises(Exception):
+        test_db.insert("test_table", entry)
+
+
 def test_update_row(test_db):
     test_db.insert("test_table", dict(description="haha", amount=2))
 
-    entries = test_db.get_df("test_table").to_dict(orient="records")
+    entries = test_db.read_df("test_table").to_dict(orient="records")
     where = {"row_id": entries[0]["row_id"]}
 
     vals = {"category": "X"}
     test_db.update("test_table", where, vals)
 
-    entries = test_db.get_df("test_table").to_dict(orient="records")
+    entries = test_db.read_df("test_table").to_dict(orient="records")
     assert py_.find(entries, {**vals, **where})
 
 
 def test_delete_row(test_db):
     test_db.insert("test_table", dict(description="haha", amount=2))
-    entries = test_db.get_df("test_table").to_dict(orient="records")
+    entries = test_db.read_df("test_table").to_dict(orient="records")
     where = {"row_id": entries[0]["row_id"]}
     test_db.delete("test_table", where)
-    entries = test_db.get_df("test_table").to_dict(orient="records")
+    entries = test_db.read_df("test_table").to_dict(orient="records")
     assert not py_.find(entries, where)
 
 
 def test_get_rows(test_db):
     entry = dict(description="haha", amount=2)
     test_db.insert("test_table", entry)
-    rows = test_db.get_rows("test_table")
+    rows = test_db.read_rows("test_table")
     assert len(rows) == 1
     row = rows[0]
     for val in entry.values():
         assert val in row
 
 
 def test_get_one_row(test_db):
     entry = dict(description="haha", amount=2)
     test_db.insert("test_table", entry)
-    row = test_db.get_one_row("test_table")
+    row = test_db.read_one_row("test_table")
     for val in entry.values():
         assert val in row
 
 
 def test_get_dicts(test_db):
     entries = [
         dict(description="haha", amount=2),
         dict(description="dodo", amount=3),
     ]
     test_db.set_from_df("test_table", pandas.DataFrame(entries))
-    return_entries = test_db.get_dicts("test_table")
+    return_entries = test_db.read_dicts("test_table")
     for entry in return_entries:
         assert py_.find(return_entries, entry)
 
 
 def test_get_one_dict(test_db):
     entries = [
         dict(description="haha", amount=2),
         dict(description="dodo", amount=3),
     ]
     test_db.set_from_df("test_table", pandas.DataFrame(entries))
-    return_entry = test_db.get_one_dict("test_table")
+    return_entry = test_db.read_one_dict("test_table")
     is_found = False
     for entry in entries:
         if entry.items() < return_entry.items():
             is_found = True
     assert is_found
 
 
-def test_var_names():
-    assert var_name_regex.fullmatch("__ha__")
-    assert not var_name_regex.fullmatch("1__ha__")
-    assert not var_name_regex.fullmatch("__ ha__")
-    assert not var_name_regex.fullmatch("var#")
-    assert not var_name_regex.fullmatch("v;ar")
+@pytest.fixture(scope="function")
+def empty_db():
+    db_fname = Path(__file__).parent / "test.sqlite3"
+    db_fname.remove_p()
+
+    db = SqliteAdaptor(db_fname)
+    db.commit()
+
+    yield db
+
+    db.close()
+    db_fname.remove_p()
+
+
+def test_build_table(empty_db):
+    first_schema = {
+        "type": "object",
+        "properties": {
+            "row_id": {"type": "integer"},
+            "description": {"type": "string"},
+        },
+        "required": ["row_id"],
+    }
+
+    second_schema = {
+        "type": "object",
+        "properties": {
+            "amount": {"type": "number"},
+            "category": {"type": "string"},
+        },
+    }
+
+    def col_names(schema):
+        return list(schema["properties"].keys())
+
+    empty_db.create_table("test_table", first_schema)
+    return_schema = empty_db.read_table_schema("test_table")
+    assert col_names(return_schema) == col_names(first_schema)
+
+    empty_db.add_columns("test_table", second_schema)
+    return_schema = empty_db.read_table_schema("test_table")
+    assert col_names(return_schema) == col_names(first_schema) + col_names(second_schema)
```

### Comparing `sqladaptor-0.2.1/README.md` & `sqladaptor-0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -32,24 +32,31 @@
     {"description": "this", "value": 1},
     {"description": "that", "value": 2}
 ]
 
 db = SqliteAdaptor('db.sqlite')
 db.set_from_df('data1', pandas.DataFrame(entries))
 
-entries = db.get_dicts('data1')
+entries = db.read_dicts('data1')
 # [
 #   {'description': 'this', 'value': 1}, 
 #   {'description': 'that', 'value': 2}
 # ]
 
-return_entries = db.get_dicts('data1', {"description": "this"})
+return_entries = db.read_dicts('data1', {"description": "this"})
 # [{'description': 'this', 'value': 1}]
 
-df = db.get_df("data1", {"value": 2})
+df = db.read_df("data1", {"value": 2})
 #   description  value
 # 0        that      2
 
 db.update("data1", {"value": 2}, {"description": "altered"})
-return_entries2 = db.get_dicts('data1', {"value": 2})
+return_entries2 = db.read_dicts('data1', {"value": 2})
 # [{'description': 'altered', 'value': 2}]
 ```
+
+## The API
+
+The key idea is to provide a JSON-like API for an SQL database. This will get provide
+a simple way of moving JSON lists into a database. With the API, JSON lists are easily
+returned. This is to simplify the transition of a good prototype into a production 
+database.
```

### Comparing `sqladaptor-0.2.1/pyproject.toml` & `sqladaptor-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sqladaptor"
-version = "0.2.1"
+version = "0.4"
 description = "Starting adaptor for JSON/Pandas to SQL db"
 authors = [
     { name = "Bosco Ho", email = "apposite@gmail.com" }
 ]
 dependencies = [
     "path>=16.14.0",
     "pydash>=8.0.1",
```

### Comparing `sqladaptor-0.2.1/PKG-INFO` & `sqladaptor-0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.3
 Name: sqladaptor
-Version: 0.2.1
+Version: 0.4
 Summary: Starting adaptor for JSON/Pandas to SQL db
 Author-email: Bosco Ho <apposite@gmail.com>
+License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: fastjsonschema>=2.19.1
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: path>=16.14.0
 Requires-Dist: pydash>=8.0.1
 Requires-Dist: pytest>=8.2.1
 Requires-Dist: rich>=13.7.1
@@ -48,24 +49,31 @@
     {"description": "this", "value": 1},
     {"description": "that", "value": 2}
 ]
 
 db = SqliteAdaptor('db.sqlite')
 db.set_from_df('data1', pandas.DataFrame(entries))
 
-entries = db.get_dicts('data1')
+entries = db.read_dicts('data1')
 # [
 #   {'description': 'this', 'value': 1}, 
 #   {'description': 'that', 'value': 2}
 # ]
 
-return_entries = db.get_dicts('data1', {"description": "this"})
+return_entries = db.read_dicts('data1', {"description": "this"})
 # [{'description': 'this', 'value': 1}]
 
-df = db.get_df("data1", {"value": 2})
+df = db.read_df("data1", {"value": 2})
 #   description  value
 # 0        that      2
 
 db.update("data1", {"value": 2}, {"description": "altered"})
-return_entries2 = db.get_dicts('data1', {"value": 2})
+return_entries2 = db.read_dicts('data1', {"value": 2})
 # [{'description': 'altered', 'value': 2}]
 ```
+
+## The API
+
+The key idea is to provide a JSON-like API for an SQL database. This will get provide
+a simple way of moving JSON lists into a database. With the API, JSON lists are easily
+returned. This is to simplify the transition of a good prototype into a production 
+database.
```

