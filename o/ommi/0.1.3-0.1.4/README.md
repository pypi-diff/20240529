# Comparing `tmp/ommi-0.1.3.tar.gz` & `tmp/ommi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ommi-0.1.3.tar", max compression
+gzip compressed data, was "ommi-0.1.4.tar", max compression
```

## Comparing `ommi-0.1.3.tar` & `ommi-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1076 2024-05-23 15:31:01.150359 ommi-0.1.3/LICENSE
--rw-r--r--   0        0        0     4001 2024-05-23 15:31:01.150359 ommi-0.1.3/README.md
--rw-r--r--   0        0        0      195 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/__init__.py
--rw-r--r--   0        0        0      943 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/contextual_method.py
--rw-r--r--   0        0        0      677 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/driver_context.py
--rw-r--r--   0        0        0     4676 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/drivers.py
--rw-r--r--   0        0        0     6148 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/ext/.DS_Store
--rw-r--r--   0        0        0     8295 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/ext/drivers/mongodb.py
--rw-r--r--   0        0        0    13214 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/ext/drivers/postgresql.py
--rw-r--r--   0        0        0    12398 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/ext/drivers/sqlite.py
--rw-r--r--   0        0        0     4605 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/field_metadata.py
--rw-r--r--   0        0        0      350 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/model_collections.py
--rw-r--r--   0        0        0     8755 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/models.py
--rw-r--r--   0        0        0     9955 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/query_ast.py
--rw-r--r--   0        0        0     1279 2024-05-23 15:31:01.154359 ommi-0.1.3/ommi/statuses.py
--rw-r--r--   0        0        0      170 2024-05-23 15:31:01.154359 ommi-0.1.3/ommi/utils/get_first.py
--rw-r--r--   0        0        0      837 2024-05-23 15:31:18.422281 ommi-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4813 1970-01-01 00:00:00.000000 ommi-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-29 00:17:53.997303 ommi-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4187 2024-05-29 00:17:53.997303 ommi-0.1.4/README.md
+-rw-r--r--   0        0        0      195 2024-05-29 00:17:53.997303 ommi-0.1.4/ommi/__init__.py
+-rw-r--r--   0        0        0      943 2024-05-29 00:17:53.997303 ommi-0.1.4/ommi/contextual_method.py
+-rw-r--r--   0        0        0      677 2024-05-29 00:17:53.997303 ommi-0.1.4/ommi/driver_context.py
+-rw-r--r--   0        0        0     6623 2024-05-29 00:17:53.997303 ommi-0.1.4/ommi/drivers.py
+-rw-r--r--   0        0        0     6148 2024-05-29 00:17:53.997303 ommi-0.1.4/ommi/ext/.DS_Store
+-rw-r--r--   0        0        0    13121 2024-05-29 00:17:53.997303 ommi-0.1.4/ommi/ext/drivers/mongodb.py
+-rw-r--r--   0        0        0    12707 2024-05-29 00:17:53.997303 ommi-0.1.4/ommi/ext/drivers/postgresql.py
+-rw-r--r--   0        0        0    11594 2024-05-29 00:17:53.997303 ommi-0.1.4/ommi/ext/drivers/sqlite.py
+-rw-r--r--   0        0        0     4605 2024-05-29 00:17:54.001303 ommi-0.1.4/ommi/field_metadata.py
+-rw-r--r--   0        0        0      350 2024-05-29 00:17:54.001303 ommi-0.1.4/ommi/model_collections.py
+-rw-r--r--   0        0        0     9217 2024-05-29 00:17:54.001303 ommi-0.1.4/ommi/models.py
+-rw-r--r--   0        0        0    10003 2024-05-29 00:17:54.001303 ommi-0.1.4/ommi/query_ast.py
+-rw-r--r--   0        0        0     1279 2024-05-29 00:17:54.001303 ommi-0.1.4/ommi/statuses.py
+-rw-r--r--   0        0        0      170 2024-05-29 00:17:54.001303 ommi-0.1.4/ommi/utils/get_first.py
+-rw-r--r--   0        0        0      837 2024-05-29 00:18:10.373529 ommi-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4999 1970-01-01 00:00:00.000000 ommi-0.1.4/PKG-INFO
```

### Comparing `ommi-0.1.3/LICENSE` & `ommi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ommi-0.1.3/README.md` & `ommi-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 ### Connecting
 
 ```python
 from ommi.ext.drivers.sqlite import SQLiteDriver, SQLiteConfig
 
 
 async def example():
-    async with SQLiteDriver(SQLiteConfig(filename=":memory:")) as db:
+    async with SQLiteDriver.from_config(SQLiteConfig(filename=":memory:")) as db:
         ...
 ```
 
 ### Database Actions
 
 The database drivers provide `add`, `count`, delete`, `fetch`, `sync_schema`, and `update` methods. These methods should
 be wrapped in an `ommi.drivers.DatabaseAction`. The database action will capture the return and wrap it in a
@@ -134,13 +134,18 @@
 
 ```python
 await db.sync_schema().or_raise()
 ```
 
 #### Update
 
-Update takes any number of model instances and syncs their changes to the database.
+Update takes any number of predicates and fields to set as keyword arguments. The predicates will be ANDed together.
 
 ```python
-user.name = "Bob"
-await db.update(user).or_raise()
+await db.update(User.id == 20, name="Bob").or_raise()
+```
+
+Additionally, models provide a `sync` method that does an `update` querying the model's key.
+
+```python
+await user.sync().or_raise()
 ```
```

### Comparing `ommi-0.1.3/ommi/contextual_method.py` & `ommi-0.1.4/ommi/contextual_method.py`

 * *Files identical despite different names*

### Comparing `ommi-0.1.3/ommi/driver_context.py` & `ommi-0.1.4/ommi/driver_context.py`

 * *Files identical despite different names*

### Comparing `ommi-0.1.3/ommi/ext/.DS_Store` & `ommi-0.1.4/ommi/ext/.DS_Store`

 * *Files identical despite different names*

### Comparing `ommi-0.1.3/ommi/ext/drivers/postgresql.py` & `ommi-0.1.4/ommi/ext/drivers/postgresql.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,31 @@
 import psycopg
 from dataclasses import dataclass, field as dc_field
 from datetime import datetime, date
-from typing import Type, Any, TypeVar, Callable, get_origin, Generator, Sequence
+from typing import (
+    Type,
+    Any,
+    TypeVar,
+    Callable,
+    get_origin,
+    Generator,
+    Sequence,
+    Protocol,
+    runtime_checkable,
+)
 
 from tramp.results import Result
 
-from ommi.drivers import DatabaseDriver, DriverConfig, database_action
+from ommi.drivers import (
+    DatabaseDriver,
+    DriverConfig,
+    database_action,
+    enforce_connection_protocol,
+    connection_context_manager,
+)
 from ommi.model_collections import ModelCollection
 from ommi.models import OmmiField, OmmiModel, get_collection
 from ommi.query_ast import (
     ASTGroupNode,
     when,
     ASTReferenceNode,
     ASTLiteralNode,
@@ -42,17 +58,31 @@
     username: str
     password: str
 
     def to_uri(self) -> str:
         return f"postgresql://{self.username}:{self.password}@{self.host}:{self.port}/{self.database_name}"
 
 
-class PostgreSQLDriver(DatabaseDriver, driver_name="postgresql", nice_name="PostgreSQL"):
-    config: PostgreSQLConfig
+@runtime_checkable
+class PostgreSQLConnection(Protocol):
+    def cursor(self) -> psycopg.AsyncCursor: ...
+
+    def close(self) -> None: ...
+
+    async def commit(self) -> None: ...
 
+    async def rollback(self) -> None: ...
+
+
+@enforce_connection_protocol
+class PostgreSQLDriver(
+    DatabaseDriver[PostgreSQLConnection],
+    driver_name="postgresql",
+    nice_name="PostgreSQL",
+):
     logical_operator_mapping = {
         ASTLogicalOperatorNode.AND: "AND",
         ASTLogicalOperatorNode.OR: "OR",
     }
 
     operator_mapping = {
         ASTOperatorNode.EQUALS: "=",
@@ -71,131 +101,95 @@
     type_mapping = {
         int: "INTEGER",
         str: "TEXT",
         float: "REAL",
         bool: "INTEGER",
     }
 
-    def __init__(self, *args):
-        super().__init__(*args)
-        self._connected = False
-        self._db: psycopg.AsyncConnection | None = None
-
-    @property
-    def connected(self) -> bool:
-        return self._connected
-
-    @database_action
-    async def connect(self) -> "PostgreSQLDriver":
-        if not self._connected:
-            self._db = await psycopg.AsyncConnection.connect(self.config.to_uri())
-            self._connected = True
-
-        return self
+    def __init__(self, connection: PostgreSQLConnection):
+        super().__init__(connection)
 
     @database_action
     async def disconnect(self) -> "PostgreSQLDriver":
-        await self._db.close()
+        await self.connection.close()
         self._connected = False
         return self
 
     @database_action
     async def add(self, *items: OmmiModel) -> "PostgreSQLDriver":
-        session = self._db.cursor()
+        session = self._connection.cursor()
         try:
             await self._insert(items, session, type(items[0]))
 
         except:
-            await self._db.rollback()
+            await self._connection.rollback()
             raise
 
         else:
             return self
 
         finally:
             await session.close()
 
     @database_action
     async def count(self, *predicates: ASTGroupNode | Type[OmmiModel]) -> int:
         ast = when(*predicates)
-        session = self._db.cursor()
+        session = self._connection.cursor()
         return await self._count(ast, session)
 
     @database_action
-    async def delete(self, *items: OmmiModel) -> "PostgreSQLDriver":
-        models = {}
-        for item in items:
-            models.setdefault(type(item), []).append(item)
-
-        session = self._db.cursor()
-        try:
-            for model, items in models.items():
-                await self._delete_rows(model, items, session)
-
-        except:
-            await self._db.rollback()
-            raise
-
-        else:
-            return self
-
-        finally:
-            await session.close()
+    async def delete(self, *predicates: ASTGroupNode | Type[OmmiModel]) -> "PostgreSQLDriver":
+        ast = when(*predicates)
+        session = self._connection.cursor()
+        await self._delete(ast, session)
+        return self
 
     @database_action
     async def fetch(
         self, *predicates: ASTGroupNode | Type[OmmiModel]
     ) -> list[OmmiModel]:
         ast = when(*predicates)
-        session = self._db.cursor()
+        session = self._connection.cursor()
         result = await self._select(ast, session)
         return result
 
     @database_action
     async def sync_schema(
         self, collection: ModelCollection | None = None
     ) -> "PostgreSQLDriver":
-        session = self._db.cursor()
+        session = self._connection.cursor()
         models = get_collection(
             Result.Value(collection) if collection else Result.Nothing
         ).models
         try:
             for model in models:
                 await self._create_table(model, session)
 
         except:
-            await self._db.rollback()
+            await self._connection.rollback()
             raise
 
         else:
             return self
 
         finally:
             await session.close()
 
     @database_action
-    async def update(self, *items: OmmiModel) -> "PostgreSQLDriver":
-        models = {}
-        for item in items:
-            models.setdefault(type(item), []).append(item)
-
-        session = self._db.cursor()
-        try:
-            for model, items in models.items():
-                await self._update_rows(model, items, session)
-
-        except:
-            await self._db.rollback()
-            raise
+    async def update(self, *predicates: ASTGroupNode | Type[OmmiModel], **kwargs) -> "PostgreSQLDriver":
+        ast = when(*predicates)
+        session = self._connection.cursor()
+        await self._update(ast, kwargs, session)
+        return self
 
-        else:
-            return self
-
-        finally:
-            await session.close()
+    @classmethod
+    @connection_context_manager
+    async def from_config(cls, config: PostgreSQLConfig) -> "PostgreSQLDriver":
+        connection = await psycopg.AsyncConnection.connect(config.to_uri())
+        return cls(connection)
 
     def _build_column(self, field: OmmiField, pk: bool) -> str:
         column = [
             field.get("store_as"),
             self._get_postgresql_type(field.get("field_type"), pk),
         ]
         if pk:
@@ -270,90 +264,89 @@
             self._build_column(field, field == pk)
             for field in model.__ommi_metadata__.fields.values()
         )
         await session.execute(
             f"CREATE TABLE IF NOT EXISTS {model.__ommi_metadata__.model_name} ({columns});"
         )
 
-    async def _insert(self, items: Sequence[OmmiModel], session: psycopg.AsyncCursor, model: Type[OmmiModel]):
+    async def _insert(
+        self,
+        items: Sequence[OmmiModel],
+        session: psycopg.AsyncCursor,
+        model: Type[OmmiModel],
+    ):
         query = [f"INSERT INTO {model.__ommi_metadata__.model_name}"]
 
         fields = list(model.__ommi_metadata__.fields.values())
         pk = model.get_primary_key_field()
         columns = [field.get("store_as") for field in fields if field != pk]
         query.append(f"({','.join(columns)})")
 
         values = []
         inserts = []
         for item in items:
             qs = ",".join(["%s"] * len(columns))
             inserts.append(f"({qs})")
-            values.extend(getattr(item, field.get("field_name")) for field in fields if field != pk)
+            values.extend(
+                getattr(item, field.get("field_name"))
+                for field in fields
+                if field != pk
+            )
 
         query.append(f"VALUES {','.join(inserts)}")
         query.append(f"RETURNING {pk.get('store_as')};")
 
         result = await session.execute(" ".join(query).encode(), values)
 
         # Update the primary key field of the models that were inserted if the primary key is an auto-incrementing field
         item_stack = iter(items)
         async for record in result:
             item = next(item_stack)
             setattr(item, pk.get("field_name"), record[0])
 
-    async def _update_rows(
+    async def _update(
         self,
-        model: Type[OmmiModel],
-        items: list[OmmiModel],
+        ast: ASTGroupNode,
+        set_fields: dict[str, Any],
         session: psycopg.AsyncCursor,
     ):
-        pk = model.get_primary_key_field().get("store_as")
-        fields = list(model.__ommi_metadata__.fields.values())
-        for item in items:
-            values = (
-                getattr(item, field.get("field_name"))
-                for field in fields
-                if field.get("store_as") != pk
-            )
-            assignments = ", ".join(
-                f"{field.get('store_as')} = %s"
-                for field in fields
-                if field.get("store_as") != pk
-            )
-            await session.execute(
-                f"UPDATE {model.__ommi_metadata__.model_name} SET {assignments} WHERE {pk} = %s;",
-                (*values, getattr(item, pk)),
-            )
+        query = self._process_ast(ast)
+        fields = query.model.__ommi_metadata__.fields
+        assignments = ", ".join(f"{fields[name].get('store_as')} = %s" for name in set_fields.keys())
+        await session.execute(
+            f"UPDATE {query.model.__ommi_metadata__.model_name} SET {assignments} WHERE {query.where};",
+            (*set_fields.values(), *query.values),
+        )
 
-    async def _delete_rows(
+    async def _delete(
         self,
-        model: Type[OmmiModel],
-        items: list[OmmiModel],
+        ast: ASTGroupNode,
         session: psycopg.AsyncCursor,
     ):
-        pk = model.get_primary_key_field().get("store_as")
-        keys = [getattr(item, pk) for item in items]
-        qs = ", ".join(["%s"] * len(items))
+        query = self._process_ast(ast)
         await session.execute(
-            f"DELETE FROM {model.__ommi_metadata__.model_name} WHERE {pk} IN ({qs});",
-            keys,
+            f"DELETE FROM {query.model.__ommi_metadata__.model_name} WHERE {query.where};",
+            query.values,
         )
 
     async def _select(self, predicates: ASTGroupNode, session: psycopg.AsyncCursor):
         query = self._process_ast(predicates)
         query_str = self._build_select_query(query)
-        result = await session.execute(query_str, query.values)
+        result = await session.execute(query_str.encode(), query.values)
         return [
-            query.model(*self._validate_row_values(query.model, row)) async for row in result
+            query.model(*self._validate_row_values(query.model, row))
+            async for row in result
         ]
 
     async def _count(self, predicates: ASTGroupNode, session: psycopg.AsyncCursor):
         query = self._process_ast(predicates)
         query_str = self._build_count_query(query)
-        result = await (await session.execute(query_str.encode(), query.values)).fetchone()
+        result = await (
+            await session.execute(query_str.encode(), query.values)
+        ).fetchone()
         return result[0]
 
     def _validate_row_values(
         self, model: Type[OmmiModel], row: tuple[Any]
     ) -> Generator[Any, None, None]:
         for field, value in zip(model.__ommi_metadata__.fields.values(), row):
             if validator := self._find_type_validator(field.get("field_type", value)):
```

### Comparing `ommi-0.1.3/ommi/ext/drivers/sqlite.py` & `ommi-0.1.4/ommi/ext/drivers/sqlite.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 import sqlite3
 from dataclasses import dataclass, field as dc_field
 from datetime import datetime, date
-from typing import Type, Any, TypeVar, Callable, get_origin, Generator
+from typing import (
+    Type,
+    Any,
+    TypeVar,
+    Callable,
+    get_origin,
+    Generator,
+    Protocol,
+    runtime_checkable,
+)
 
 from tramp.results import Result
 
-from ommi.drivers import DatabaseDriver, DriverConfig, database_action
+from ommi.drivers import (
+    DatabaseDriver,
+    DriverConfig,
+    database_action,
+    enforce_connection_protocol,
+    connection_context_manager,
+)
 from ommi.model_collections import ModelCollection
 from ommi.models import OmmiField, OmmiModel, get_collection
 from ommi.query_ast import (
     ASTGroupNode,
     when,
     ASTReferenceNode,
     ASTLiteralNode,
@@ -35,17 +50,27 @@
 
 
 @dataclass
 class SQLiteConfig(DriverConfig):
     filename: str
 
 
-class SQLiteDriver(DatabaseDriver, driver_name="sqlite", nice_name="SQLite"):
-    config: SQLiteConfig
+@runtime_checkable
+class SQLiteConnection(Protocol):
+    def close(self) -> None: ...
+
+    def cursor(self) -> sqlite3.Cursor: ...
 
+    def rollback(self) -> None: ...
+
+
+@enforce_connection_protocol
+class SQLiteDriver(
+    DatabaseDriver[SQLiteConnection], driver_name="sqlite", nice_name="SQLite"
+):
     logical_operator_mapping = {
         ASTLogicalOperatorNode.AND: "AND",
         ASTLogicalOperatorNode.OR: "OR",
     }
 
     operator_mapping = {
         ASTOperatorNode.EQUALS: "=",
@@ -64,133 +89,93 @@
     type_mapping = {
         int: "INTEGER",
         str: "TEXT",
         float: "REAL",
         bool: "INTEGER",
     }
 
-    def __init__(self, *args):
-        super().__init__(*args)
-        self._connected = False
-        self._db: sqlite3.Connection | None = None
-
-    @property
-    def connected(self) -> bool:
-        return self._connected
-
-    @database_action
-    async def connect(self) -> "SQLiteDriver":
-        if not self._connected:
-            self._db = sqlite3.connect(self.config.filename)
-            self._connected = True
-
-        return self
-
     @database_action
     async def disconnect(self) -> "SQLiteDriver":
-        self._db.close()
+        self._connection.close()
         self._connected = False
         return self
 
     @database_action
     async def add(self, *items: OmmiModel) -> "SQLiteDriver":
-        session = self._db.cursor()
+        session = self._connection.cursor()
         try:
             for item in items:
                 self._insert(item, session)
                 self._sync_with_last_inserted(item, session)
 
         except:
-            self._db.rollback()
+            self._connection.rollback()
             raise
 
         else:
             return self
 
         finally:
             session.close()
 
     @database_action
     async def count(self, *predicates: ASTGroupNode | Type[OmmiModel]) -> int:
         ast = when(*predicates)
-        session = self._db.cursor()
+        session = self._connection.cursor()
         return self._count(ast, session)
 
     @database_action
-    async def delete(self, *items: OmmiModel) -> "SQLiteDriver":
-        models = {}
-        for item in items:
-            models.setdefault(type(item), []).append(item)
-
-        session = self._db.cursor()
-        try:
-            for model, items in models.items():
-                self._delete_rows(model, items, session)
-
-        except:
-            self._db.rollback()
-            raise
-
-        else:
-            return self
-
-        finally:
-            session.close()
+    async def delete(self, *predicates: ASTGroupNode | Type[OmmiModel]) -> "SQLiteDriver":
+        ast = when(*predicates)
+        session = self._connection.cursor()
+        self._delete(ast, session)
+        return self
 
     @database_action
     async def fetch(
         self, *predicates: ASTGroupNode | Type[OmmiModel]
     ) -> list[OmmiModel]:
         ast = when(*predicates)
-        session = self._db.cursor()
+        session = self._connection.cursor()
         result = self._select(ast, session)
         return result
 
     @database_action
     async def sync_schema(
         self, collection: ModelCollection | None = None
     ) -> "SQLiteDriver":
-        session = self._db.cursor()
+        session = self._connection.cursor()
         models = get_collection(
             Result.Value(collection) if collection else Result.Nothing
         ).models
         try:
             for model in models:
                 self._create_table(model, session)
 
         except:
-            self._db.rollback()
+            self._connection.rollback()
             raise
 
         else:
             return self
 
         finally:
             session.close()
 
     @database_action
-    async def update(self, *items: OmmiModel) -> "SQLiteDriver":
-        models = {}
-        for item in items:
-            models.setdefault(type(item), []).append(item)
-
-        session = self._db.cursor()
-        try:
-            for model, items in models.items():
-                self._update_rows(model, items, session)
-
-        except:
-            self._db.rollback()
-            raise
-
-        else:
-            return self
+    async def update(self, *predicates: ASTGroupNode | Type[OmmiModel], **kwargs) -> "SQLiteDriver":
+        ast = when(*predicates)
+        session = self._connection.cursor()
+        self._update(ast, kwargs, session)
+        return self
 
-        finally:
-            session.close()
+    @classmethod
+    @connection_context_manager
+    async def from_config(cls, config: SQLiteConfig) -> "SQLiteDriver":
+        return cls(sqlite3.connect(config.filename))
 
     def _build_column(self, field: OmmiField, pk: bool) -> str:
         column = [
             field.get("store_as"),
             self._get_sqlite_type(field.get("field_type")),
         ]
         if pk:
@@ -279,50 +264,37 @@
         columns = ", ".join(data.keys())
         values = tuple(data.values())
         session.execute(
             f"INSERT INTO {item.__ommi_metadata__.model_name} ({columns}) VALUES ({qs});",
             values,
         )
 
-    def _update_rows(
-        self,
-        model: Type[OmmiModel],
-        items: list[OmmiModel],
-        session: sqlite3.Cursor,
+    def _update(
+            self,
+            ast: ASTGroupNode,
+            set_fields: dict[str, Any],
+            session: sqlite3.Cursor,
     ):
-        pk = model.get_primary_key_field().get("store_as")
-        fields = list(model.__ommi_metadata__.fields.values())
-        for item in items:
-            values = (
-                getattr(item, field.get("field_name"))
-                for field in fields
-                if field.get("store_as") != pk
-            )
-            assignments = ", ".join(
-                f"{field.get('store_as')} = ?"
-                for field in fields
-                if field.get("store_as") != pk
-            )
-            session.execute(
-                f"UPDATE {model.__ommi_metadata__.model_name} SET {assignments} WHERE {pk} = ?;",
-                (*values, getattr(item, pk)),
-            )
+        query = self._process_ast(ast)
+        fields = query.model.__ommi_metadata__.fields
+        assignments = ", ".join(f"{fields[name].get('store_as')} = ?" for name in set_fields.keys())
+        session.execute(
+            f"UPDATE {query.model.__ommi_metadata__.model_name} SET {assignments} WHERE {query.where};",
+            (*set_fields.values(), *query.values),
+        )
 
-    def _delete_rows(
+    def _delete(
         self,
-        model: Type[OmmiModel],
-        items: list[OmmiModel],
+        ast: ASTGroupNode,
         session: sqlite3.Cursor,
     ):
-        pk = model.get_primary_key_field().get("store_as")
-        keys = [getattr(item, pk) for item in items]
-        qs = ", ".join(["?"] * len(items))
+        query = self._process_ast(ast)
         session.execute(
-            f"DELETE FROM {model.__ommi_metadata__.model_name} WHERE {pk} IN ({qs});",
-            keys,
+            f"DELETE FROM {query.model.__ommi_metadata__.model_name} WHERE {query.where};",
+            query.values,
         )
 
     def _select(self, predicates: ASTGroupNode, session: sqlite3.Cursor):
         query = self._process_ast(predicates)
         query_str = self._build_select_query(query)
         session.execute(query_str, query.values)
         result = session.fetchall()
```

### Comparing `ommi-0.1.3/ommi/field_metadata.py` & `ommi-0.1.4/ommi/field_metadata.py`

 * *Files identical despite different names*

### Comparing `ommi-0.1.3/ommi/models.py` & `ommi-0.1.4/ommi/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 import ommi.drivers as drivers
 import ommi.query_ast as query_ast
 from ommi.field_metadata import (
     FieldMetadata,
     AggregateMetadata,
     FieldType,
     StoreAs,
-    create_metadata_type, Key,
+    create_metadata_type,
+    Key,
 )
 from ommi.utils.get_first import first
 from ommi.statuses import DatabaseStatus
 from ommi.contextual_method import contextual_method
 from ommi.driver_context import active_driver
 import ommi.model_collections
 
@@ -111,15 +112,16 @@
     ) -> "drivers.DatabaseAction[DatabaseStatus[OmmiModel]] | Awaitable[DatabaseStatus[OmmiModel]]":
         return self.get_driver().add(self)
 
     @contextual_method
     def delete(
         self, driver: "drivers.DatabaseDriver | None" = None
     ) -> "drivers.DatabaseAction[DatabaseStatus[drivers.DatabaseDriver]] | Awaitable[DatabaseStatus[drivers.DatabaseDriver]]":
-        return self.get_driver(driver).delete(self)
+        pk_name = self.get_primary_key_field().get("field_name")
+        return self.get_driver(driver).delete(query_ast.when(getattr(type(self), pk_name) == getattr(self, pk_name)))
 
     @delete.classmethod
     def delete(
         cls, *items: "OmmiModel", driver: "drivers.DatabaseDriver | None" = None
     ) -> "drivers.DatabaseAction[DatabaseStatus[drivers.DatabaseDriver]] | Awaitable[DatabaseStatus[drivers.DatabaseDriver]]":
         return cls.get_driver(driver).delete(*items)
 
@@ -144,15 +146,23 @@
         return cls.get_driver(driver).fetch(
             cls, *predicates, *cls._build_column_predicates(columns)
         )
 
     def sync(
         self, driver: "drivers.DatabaseDriver | None" = None
     ) -> "drivers.DatabaseAction[DatabaseStatus[drivers.DatabaseDriver]] | Awaitable[DatabaseStatus[drivers.DatabaseDriver]]":
-        return self.get_driver(driver).update(self)
+        pk_name = self.get_primary_key_field().get("field_name")
+        return self.get_driver(driver).update(
+            query_ast.when(getattr(type(self), pk_name) == getattr(self, pk_name)),
+            **{
+                name: getattr(self, name)
+                for name in self.__ommi_metadata__.fields.keys()
+                if name != pk_name
+            },
+        )
 
     @classmethod
     def get_primary_key_field(cls) -> OmmiField:
         fields = cls.__ommi_metadata__.fields
         if not fields:
             raise Exception(f"No fields defined on {cls}")
```

### Comparing `ommi-0.1.3/ommi/query_ast.py` & `ommi-0.1.4/ommi/query_ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,19 @@
     def __init__(self, field, model, ordering=ResultOrdering.ASCENDING):
         super().__init__(ASTGroupNode())
         self._field = field
         self._model = model
         self._ordering = ordering
 
     def _eq(self, other):
-        return self.field == other.field and self.model == other.model and self.ordering == other.ordering
+        return (
+            self.field == other.field
+            and self.model == other.model
+            and self.ordering == other.ordering
+        )
 
     def __iter__(self):
         yield from (self._field, self._model)
 
     @property
     def field(self):
         return self._field
```

### Comparing `ommi-0.1.3/ommi/statuses.py` & `ommi-0.1.4/ommi/statuses.py`

 * *Files identical despite different names*

### Comparing `ommi-0.1.3/pyproject.toml` & `ommi-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ommi"
-version = "0.1.3"
+version = "0.1.4"
 description = "A portable object model mapper that can work with any database and model library (dataclasses, Attrs, Pydantic, etc.). It is designed for the general case to support the largest possible number of databases."
 authors = ["Zech Zimmerman <hi@zech.codes>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ZechCodes/Ommi"
 keywords = ["database", "orm", "object model mapper", "dataclasses", "attrs", "pydantic", "sqlite"]
```

### Comparing `ommi-0.1.3/PKG-INFO` & `ommi-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ommi
-Version: 0.1.3
+Version: 0.1.4
 Summary: A portable object model mapper that can work with any database and model library (dataclasses, Attrs, Pydantic, etc.). It is designed for the general case to support the largest possible number of databases.
 Home-page: https://github.com/ZechCodes/Ommi
 License: MIT
 Keywords: database,orm,object model mapper,dataclasses,attrs,pydantic,sqlite
 Author: Zech Zimmerman
 Author-email: hi@zech.codes
 Requires-Python: >=3.10,<4.0
@@ -95,15 +95,15 @@
 ### Connecting
 
 ```python
 from ommi.ext.drivers.sqlite import SQLiteDriver, SQLiteConfig
 
 
 async def example():
-    async with SQLiteDriver(SQLiteConfig(filename=":memory:")) as db:
+    async with SQLiteDriver.from_config(SQLiteConfig(filename=":memory:")) as db:
         ...
 ```
 
 ### Database Actions
 
 The database drivers provide `add`, `count`, delete`, `fetch`, `sync_schema`, and `update` methods. These methods should
 be wrapped in an `ommi.drivers.DatabaseAction`. The database action will capture the return and wrap it in a
@@ -152,14 +152,19 @@
 
 ```python
 await db.sync_schema().or_raise()
 ```
 
 #### Update
 
-Update takes any number of model instances and syncs their changes to the database.
+Update takes any number of predicates and fields to set as keyword arguments. The predicates will be ANDed together.
 
 ```python
-user.name = "Bob"
-await db.update(user).or_raise()
+await db.update(User.id == 20, name="Bob").or_raise()
+```
+
+Additionally, models provide a `sync` method that does an `update` querying the model's key.
+
+```python
+await user.sync().or_raise()
 ```
```

