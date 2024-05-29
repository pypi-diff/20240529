# Comparing `tmp/sql_athame-0.4.0a8.tar.gz` & `tmp/sql_athame-0.4.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_athame-0.4.0a8.tar", max compression
+gzip compressed data, was "sql_athame-0.4.0a9.tar", max compression
```

## Comparing `sql_athame-0.4.0a8.tar` & `sql_athame-0.4.0a9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/LICENSE
--rw-r--r--   0        0        0    12086 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/README.md
--rw-r--r--   0        0        0     2067 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/pyproject.toml
--rw-r--r--   0        0        0       79 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/__init__.py
--rw-r--r--   0        0        0    10293 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/base.py
--rw-r--r--   0        0        0    22167 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/dataclasses.py
--rw-r--r--   0        0        0      758 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/escape.py
--rw-r--r--   0        0        0        0 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/py.typed
--rw-r--r--   0        0        0     1293 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/sqlalchemy.py
--rw-r--r--   0        0        0      475 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/types.py
--rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-29 02:28:28.950667 sql_athame-0.4.0a9/LICENSE
+-rw-r--r--   0        0        0    12086 2024-05-29 02:28:28.950667 sql_athame-0.4.0a9/README.md
+-rw-r--r--   0        0        0     2067 2024-05-29 02:28:28.950667 sql_athame-0.4.0a9/pyproject.toml
+-rw-r--r--   0        0        0       79 2024-05-29 02:28:28.950667 sql_athame-0.4.0a9/sql_athame/__init__.py
+-rw-r--r--   0        0        0    10293 2024-05-29 02:28:28.950667 sql_athame-0.4.0a9/sql_athame/base.py
+-rw-r--r--   0        0        0    23792 2024-05-29 02:28:28.950667 sql_athame-0.4.0a9/sql_athame/dataclasses.py
+-rw-r--r--   0        0        0      758 2024-05-29 02:28:28.950667 sql_athame-0.4.0a9/sql_athame/escape.py
+-rw-r--r--   0        0        0        0 2024-05-29 02:28:28.950667 sql_athame-0.4.0a9/sql_athame/py.typed
+-rw-r--r--   0        0        0     1293 2024-05-29 02:28:28.950667 sql_athame-0.4.0a9/sql_athame/sqlalchemy.py
+-rw-r--r--   0        0        0      475 2024-05-29 02:28:28.950667 sql_athame-0.4.0a9/sql_athame/types.py
+-rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a9/PKG-INFO
```

### Comparing `sql_athame-0.4.0a8/LICENSE` & `sql_athame-0.4.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a8/README.md` & `sql_athame-0.4.0a9/README.md`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a8/pyproject.toml` & `sql_athame-0.4.0a9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-athame"
-version = "0.4.0-alpha-8"
+version = "0.4.0-alpha-9"
 description = "Python tool for slicing and dicing SQL"
 authors = ["Brian Downing <bdowning@lavos.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bdowning/sql-athame"
 repository = "https://github.com/bdowning/sql-athame"
```

### Comparing `sql_athame-0.4.0a8/sql_athame/base.py` & `sql_athame-0.4.0a9/sql_athame/base.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a8/sql_athame/dataclasses.py` & `sql_athame-0.4.0a9/sql_athame/dataclasses.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import functools
+import sys
 import uuid
 from collections.abc import AsyncGenerator, Iterable, Mapping
 from dataclasses import Field, InitVar, dataclass, fields
 from typing import (
     Annotated,
     Any,
     Callable,
@@ -30,71 +31,97 @@
 
 
 @dataclass
 class ColumnInfo:
     type: Optional[str] = None
     create_type: Optional[str] = None
     nullable: Optional[bool] = None
-    _constraints: tuple[str, ...] = ()
 
+    _constraints: tuple[str, ...] = ()
     constraints: InitVar[Union[str, Iterable[str], None]] = None
 
+    serialize: Optional[Callable[[Any], Any]] = None
+    deserialize: Optional[Callable[[Any], Any]] = None
+
     def __post_init__(self, constraints: Union[str, Iterable[str], None]) -> None:
         if constraints is not None:
             if type(constraints) is str:
                 constraints = (constraints,)
             self._constraints = tuple(constraints)
 
     @staticmethod
     def merge(a: "ColumnInfo", b: "ColumnInfo") -> "ColumnInfo":
         return ColumnInfo(
             type=b.type if b.type is not None else a.type,
             create_type=b.create_type if b.create_type is not None else a.create_type,
             nullable=b.nullable if b.nullable is not None else a.nullable,
             _constraints=(*a._constraints, *b._constraints),
+            serialize=b.serialize if b.serialize is not None else a.serialize,
+            deserialize=b.deserialize if b.deserialize is not None else a.deserialize,
         )
 
 
 @dataclass
 class ConcreteColumnInfo:
+    field: Field
+    type_hint: type
     type: str
     create_type: str
     nullable: bool
     constraints: tuple[str, ...]
+    serialize: Optional[Callable[[Any], Any]] = None
+    deserialize: Optional[Callable[[Any], Any]] = None
 
     @staticmethod
-    def from_column_info(name: str, *args: ColumnInfo) -> "ConcreteColumnInfo":
+    def from_column_info(
+        field: Field, type_hint: Any, *args: ColumnInfo
+    ) -> "ConcreteColumnInfo":
         info = functools.reduce(ColumnInfo.merge, args, ColumnInfo())
         if info.create_type is None and info.type is not None:
             info.create_type = info.type
             info.type = sql_create_type_map.get(info.type.upper(), info.type)
         if type(info.type) is not str or type(info.create_type) is not str:
-            raise ValueError(f"Missing SQL type for column {name!r}")
+            raise ValueError(f"Missing SQL type for column {field.name!r}")
         return ConcreteColumnInfo(
+            field=field,
+            type_hint=type_hint,
             type=info.type,
             create_type=info.create_type,
             nullable=bool(info.nullable),
             constraints=info._constraints,
+            serialize=info.serialize,
+            deserialize=info.deserialize,
         )
 
     def create_table_string(self) -> str:
         parts = (
             self.create_type,
             *(() if self.nullable else ("NOT NULL",)),
             *self.constraints,
         )
         return " ".join(parts)
 
+    def maybe_serialize(self, value: Any) -> Any:
+        if self.serialize:
+            return self.serialize(value)
+        return value
+
+
+UNION_TYPES: tuple = (Union,)
+if sys.version_info >= (3, 10):
+    from types import UnionType
+
+    UNION_TYPES = (Union, UnionType)
 
 NULLABLE_TYPES = (type(None), Any, object)
 
 
 def split_nullable(typ: type) -> tuple[bool, type]:
     nullable = typ in NULLABLE_TYPES
-    if get_origin(typ) is Union:
+    if get_origin(typ) in UNION_TYPES:
         args = []
         for arg in get_args(typ):
             if arg in NULLABLE_TYPES:
                 nullable = True
             else:
                 args.append(arg)
         return nullable, Union[tuple(args)]  # type: ignore
@@ -104,15 +131,15 @@
 sql_create_type_map = {
     "BIGSERIAL": "BIGINT",
     "SERIAL": "INTEGER",
     "SMALLSERIAL": "SMALLINT",
 }
 
 
-sql_type_map: dict[Any, str] = {
+sql_type_map: dict[type, str] = {
     bool: "BOOLEAN",
     bytes: "BYTEA",
     datetime.date: "DATE",
     datetime.datetime: "TIMESTAMP",
     float: "DOUBLE PRECISION",
     int: "INTEGER",
     str: "TEXT",
@@ -121,20 +148,19 @@
 
 
 T = TypeVar("T", bound="ModelBase")
 U = TypeVar("U")
 
 
 class ModelBase:
-    _column_info: Optional[dict[str, ConcreteColumnInfo]]
+    _column_info: dict[str, ConcreteColumnInfo]
     _cache: dict[tuple, Any]
     table_name: str
     primary_key_names: tuple[str, ...]
     array_safe_insert: bool
-    _type_hints: dict[str, type]
 
     def __init_subclass__(
         cls,
         *,
         table_name: str,
         primary_key: Union[FieldNames, str] = (),
         insert_multiple_mode: str = "unnest",
@@ -150,73 +176,63 @@
             raise ValueError("Unknown `insert_multiple_mode`")
         if isinstance(primary_key, str):
             cls.primary_key_names = (primary_key,)
         else:
             cls.primary_key_names = tuple(primary_key)
 
     @classmethod
-    def _fields(cls):
-        # wrapper to ignore typing weirdness: 'Argument 1 to "fields"
-        # has incompatible type "..."; expected "DataclassInstance |
-        # type[DataclassInstance]"'
-        return fields(cls)  # type: ignore
-
-    @classmethod
     def _cached(cls, key: tuple, thunk: Callable[[], U]) -> U:
         try:
             return cls._cache[key]
         except KeyError:
             cls._cache[key] = thunk()
             return cls._cache[key]
 
     @classmethod
-    def type_hints(cls) -> dict[str, type]:
-        try:
-            return cls._type_hints
-        except AttributeError:
-            cls._type_hints = get_type_hints(cls, include_extras=True)
-            return cls._type_hints
-
-    @classmethod
-    def column_info_for_field(cls, field: Field) -> ConcreteColumnInfo:
-        type_info = cls.type_hints()[field.name]
-        base_type = type_info
+    def column_info_for_field(cls, field: Field, type_hint: type) -> ConcreteColumnInfo:
+        base_type = type_hint
         metadata = []
-        if get_origin(type_info) is Annotated:
-            base_type, *metadata = get_args(type_info)
+        if get_origin(type_hint) is Annotated:
+            base_type, *metadata = get_args(type_hint)
         nullable, base_type = split_nullable(base_type)
         info = [ColumnInfo(nullable=nullable)]
         if base_type in sql_type_map:
             info.append(ColumnInfo(type=sql_type_map[base_type]))
         for md in metadata:
             if isinstance(md, ColumnInfo):
                 info.append(md)
-        return ConcreteColumnInfo.from_column_info(field.name, *info)
+        return ConcreteColumnInfo.from_column_info(field, type_hint, *info)
 
     @classmethod
-    def column_info(cls, column: str) -> ConcreteColumnInfo:
+    def column_info(cls) -> dict[str, ConcreteColumnInfo]:
         try:
-            return cls._column_info[column]  # type: ignore
+            return cls._column_info
         except AttributeError:
+            type_hints = get_type_hints(cls, include_extras=True)
             cls._column_info = {
-                f.name: cls.column_info_for_field(f) for f in cls._fields()
+                f.name: cls.column_info_for_field(f, type_hints[f.name])
+                for f in fields(cls)  # type: ignore
             }
-            return cls._column_info[column]
+            return cls._column_info
 
     @classmethod
     def table_name_sql(cls, *, prefix: Optional[str] = None) -> Fragment:
         return sql.identifier(cls.table_name, prefix=prefix)
 
     @classmethod
     def primary_key_names_sql(cls, *, prefix: Optional[str] = None) -> list[Fragment]:
         return [sql.identifier(pk, prefix=prefix) for pk in cls.primary_key_names]
 
     @classmethod
     def field_names(cls, *, exclude: FieldNamesSet = ()) -> list[str]:
-        return [f.name for f in cls._fields() if f.name not in exclude]
+        return [
+            ci.field.name
+            for ci in cls.column_info().values()
+            if ci.field.name not in exclude
+        ]
 
     @classmethod
     def field_names_sql(
         cls, *, prefix: Optional[str] = None, exclude: FieldNamesSet = ()
     ) -> list[Fragment]:
         return [
             sql.identifier(f, prefix=prefix) for f in cls.field_names(exclude=exclude)
@@ -227,17 +243,21 @@
 
     @classmethod
     def _get_field_values_fn(
         cls: type[T], exclude: FieldNamesSet = ()
     ) -> Callable[[T], list[Any]]:
         env: dict[str, Any] = {}
         func = ["def get_field_values(self): return ["]
-        for f in cls._fields():
-            if f.name not in exclude:
-                func.append(f"self.{f.name},")
+        for ci in cls.column_info().values():
+            if ci.field.name not in exclude:
+                if ci.serialize:
+                    env[f"_ser_{ci.field.name}"] = ci.serialize
+                    func.append(f"_ser_{ci.field.name}(self.{ci.field.name}), ")
+                else:
+                    func.append(f"self.{ci.field.name},")
         func += ["]"]
         exec(" ".join(func), env)
         return env["get_field_values"]
 
     def field_values(self, *, exclude: FieldNamesSet = ()) -> list[Any]:
         get_field_values = self._cached(
             ("get_field_values", tuple(sorted(exclude))),
@@ -253,44 +273,54 @@
                 sql.literal("DEFAULT") if value is None else sql.value(value)
                 for value in self.field_values()
             ]
         else:
             return [sql.value(value) for value in self.field_values()]
 
     @classmethod
-    def from_tuple(
-        cls: type[T], tup: tuple, *, offset: int = 0, exclude: FieldNamesSet = ()
-    ) -> T:
-        names = (f.name for f in cls._fields() if f.name not in exclude)
-        kwargs = {name: tup[offset] for offset, name in enumerate(names, start=offset)}
-        return cls(**kwargs)
+    def _get_from_mapping_fn(cls: type[T]) -> Callable[[Mapping[str, Any]], T]:
+        env: dict[str, Any] = {"cls": cls}
+        func = ["def from_mapping(mapping):"]
+        if not any(ci.deserialize for ci in cls.column_info().values()):
+            func.append(" return cls(**mapping)")
+        else:
+            func.append(" deser_dict = dict(mapping)")
+            for ci in cls.column_info().values():
+                if ci.deserialize:
+                    env[f"_deser_{ci.field.name}"] = ci.deserialize
+                    func.append(f" if {ci.field.name!r} in deser_dict:")
+                    func.append(
+                        f"  deser_dict[{ci.field.name!r}] = _deser_{ci.field.name}(deser_dict[{ci.field.name!r}])"
+                    )
+            func.append(" return cls(**deser_dict)")
+        exec("\n".join(func), env)
+        return env["from_mapping"]
 
     @classmethod
-    def from_dict(
-        cls: type[T], dct: dict[str, Any], *, exclude: FieldNamesSet = ()
-    ) -> T:
-        names = {f.name for f in cls._fields() if f.name not in exclude}
-        kwargs = {k: v for k, v in dct.items() if k in names}
-        return cls(**kwargs)
+    def from_mapping(cls: type[T], mapping: Mapping[str, Any], /) -> T:
+        # KLUDGE nasty but... efficient?
+        from_mapping_fn = cls._get_from_mapping_fn()
+        cls.from_mapping = from_mapping_fn  # type: ignore
+        return from_mapping_fn(mapping)
 
     @classmethod
     def ensure_model(cls: type[T], row: Union[T, Mapping[str, Any]]) -> T:
         if isinstance(row, cls):
             return row
-        return cls(**row)
+        return cls.from_mapping(row)  # type: ignore
 
     @classmethod
     def create_table_sql(cls) -> Fragment:
         entries = [
             sql(
                 "{} {}",
-                sql.identifier(f.name),
-                sql.literal(cls.column_info(f.name).create_table_string()),
+                sql.identifier(ci.field.name),
+                sql.literal(ci.create_table_string()),
             )
-            for f in cls._fields()
+            for ci in cls.column_info().values()
         ]
         if cls.primary_key_names:
             entries += [sql("PRIMARY KEY ({})", sql.list(cls.primary_key_names_sql()))]
         return sql(
             "CREATE TABLE IF NOT EXISTS {table} ({entries})",
             table=cls.table_name_sql(),
             entries=sql.list(entries),
@@ -334,47 +364,50 @@
         where: Where = (),
         prefetch: int = 1000,
     ) -> AsyncGenerator[T, None]:
         async for row in connection.cursor(
             *cls.select_sql(order_by=order_by, for_update=for_update, where=where),
             prefetch=prefetch,
         ):
-            yield cls(**row)
+            yield cls.from_mapping(row)
 
     @classmethod
     async def select(
         cls: type[T],
         connection_or_pool: Union[Connection, Pool],
         order_by: Union[FieldNames, str] = (),
         for_update: bool = False,
         where: Where = (),
     ) -> list[T]:
         return [
-            cls(**row)
+            cls.from_mapping(row)
             for row in await connection_or_pool.fetch(
                 *cls.select_sql(order_by=order_by, for_update=for_update, where=where)
             )
         ]
 
     @classmethod
     def create_sql(cls: type[T], **kwargs: Any) -> Fragment:
+        column_info = cls.column_info()
         return sql(
             "INSERT INTO {table} ({fields}) VALUES ({values}) RETURNING {out_fields}",
             table=cls.table_name_sql(),
-            fields=sql.list(sql.identifier(x) for x in kwargs.keys()),
-            values=sql.list(sql.value(x) for x in kwargs.values()),
+            fields=sql.list(sql.identifier(k) for k in kwargs.keys()),
+            values=sql.list(
+                sql.value(column_info[k].maybe_serialize(v)) for k, v in kwargs.items()
+            ),
             out_fields=sql.list(cls.field_names_sql()),
         )
 
     @classmethod
     async def create(
         cls: type[T], connection_or_pool: Union[Connection, Pool], **kwargs: Any
     ) -> T:
         row = await connection_or_pool.fetchrow(*cls.create_sql(**kwargs))
-        return cls(**row)
+        return cls.from_mapping(row)
 
     def insert_sql(self, exclude: FieldNamesSet = ()) -> Fragment:
         cached = self._cached(
             ("insert_sql", tuple(sorted(exclude))),
             lambda: sql(
                 "INSERT INTO {table} ({fields}) VALUES ({values})",
                 table=self.table_name_sql(),
@@ -424,18 +457,19 @@
             ("delete_multiple_sql",),
             lambda: sql(
                 "DELETE FROM {table} WHERE ({pks}) IN (SELECT * FROM {unnest})",
                 table=cls.table_name_sql(),
                 pks=sql.list(sql.identifier(pk) for pk in cls.primary_key_names),
             ).compile(),
         )
+        column_info = cls.column_info()
         return cached(
             unnest=sql.unnest(
                 (row.primary_key() for row in rows),
-                (cls.column_info(pk).type for pk in cls.primary_key_names),
+                (column_info[pk].type for pk in cls.primary_key_names),
             ),
         )
 
     @classmethod
     async def delete_multiple(
         cls: type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
     ) -> str:
@@ -447,18 +481,19 @@
             ("insert_multiple_sql",),
             lambda: sql(
                 "INSERT INTO {table} ({fields}) SELECT * FROM {unnest}",
                 table=cls.table_name_sql(),
                 fields=sql.list(cls.field_names_sql()),
             ).compile(),
         )
+        column_info = cls.column_info()
         return cached(
             unnest=sql.unnest(
                 (row.field_values() for row in rows),
-                (cls.column_info(name).type for name in cls.field_names()),
+                (column_info[name].type for name in cls.field_names()),
             ),
         )
 
     @classmethod
     def insert_multiple_array_safe_sql(cls: type[T], rows: Iterable[T]) -> Fragment:
         return sql(
             "INSERT INTO {table} ({fields}) VALUES {values}",
@@ -541,17 +576,17 @@
 
     @classmethod
     def _get_equal_ignoring_fn(
         cls: type[T], ignore: FieldNamesSet = ()
     ) -> Callable[[T, T], bool]:
         env: dict[str, Any] = {}
         func = ["def equal_ignoring(a, b):"]
-        for f in cls._fields():
-            if f.name not in ignore:
-                func.append(f" if a.{f.name} != b.{f.name}: return False")
+        for ci in cls.column_info().values():
+            if ci.field.name not in ignore:
+                func.append(f" if a.{ci.field.name} != b.{ci.field.name}: return False")
         func += [" return True"]
         exec("\n".join(func), env)
         return env["equal_ignoring"]
 
     @classmethod
     async def replace_multiple(
         cls: type[T],
@@ -599,17 +634,19 @@
         cls: type[T], ignore: FieldNamesSet = ()
     ) -> Callable[[T, T], list[str]]:
         env: dict[str, Any] = {}
         func = [
             "def differences_ignoring(a, b):",
             " diffs = []",
         ]
-        for f in cls._fields():
-            if f.name not in ignore:
-                func.append(f" if a.{f.name} != b.{f.name}: diffs.append({f.name!r})")
+        for ci in cls.column_info().values():
+            if ci.field.name not in ignore:
+                func.append(
+                    f" if a.{ci.field.name} != b.{ci.field.name}: diffs.append({ci.field.name!r})"
+                )
         func += [" return diffs"]
         exec("\n".join(func), env)
         return env["differences_ignoring"]
 
     @classmethod
     async def replace_multiple_reporting_differences(
         cls: type[T],
```

### Comparing `sql_athame-0.4.0a8/sql_athame/escape.py` & `sql_athame-0.4.0a9/sql_athame/escape.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a8/sql_athame/sqlalchemy.py` & `sql_athame-0.4.0a9/sql_athame/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a8/PKG-INFO` & `sql_athame-0.4.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-athame
-Version: 0.4.0a8
+Version: 0.4.0a9
 Summary: Python tool for slicing and dicing SQL
 Home-page: https://github.com/bdowning/sql-athame
 License: MIT
 Author: Brian Downing
 Author-email: bdowning@lavos.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

