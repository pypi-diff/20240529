# Comparing `tmp/sql_athame-0.4.0a7.tar.gz` & `tmp/sql_athame-0.4.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_athame-0.4.0a7.tar", max compression
+gzip compressed data, was "sql_athame-0.4.0a8.tar", max compression
```

## Comparing `sql_athame-0.4.0a7.tar` & `sql_athame-0.4.0a8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/LICENSE
--rw-r--r--   0        0        0    12086 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/README.md
--rw-r--r--   0        0        0     2067 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/pyproject.toml
--rw-r--r--   0        0        0       79 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/__init__.py
--rw-r--r--   0        0        0    10293 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/base.py
--rw-r--r--   0        0        0    22193 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/dataclasses.py
--rw-r--r--   0        0        0      758 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/escape.py
--rw-r--r--   0        0        0        0 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/py.typed
--rw-r--r--   0        0        0     1293 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/sqlalchemy.py
--rw-r--r--   0        0        0      475 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/types.py
--rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a7/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/LICENSE
+-rw-r--r--   0        0        0    12086 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/README.md
+-rw-r--r--   0        0        0     2067 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/pyproject.toml
+-rw-r--r--   0        0        0       79 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/__init__.py
+-rw-r--r--   0        0        0    10293 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/base.py
+-rw-r--r--   0        0        0    22167 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/dataclasses.py
+-rw-r--r--   0        0        0      758 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/escape.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/py.typed
+-rw-r--r--   0        0        0     1293 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/sqlalchemy.py
+-rw-r--r--   0        0        0      475 2024-05-28 17:00:39.393818 sql_athame-0.4.0a8/sql_athame/types.py
+-rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a8/PKG-INFO
```

### Comparing `sql_athame-0.4.0a7/LICENSE` & `sql_athame-0.4.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a7/README.md` & `sql_athame-0.4.0a8/README.md`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a7/pyproject.toml` & `sql_athame-0.4.0a8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-athame"
-version = "0.4.0-alpha-7"
+version = "0.4.0-alpha-8"
 description = "Python tool for slicing and dicing SQL"
 authors = ["Brian Downing <bdowning@lavos.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bdowning/sql-athame"
 repository = "https://github.com/bdowning/sql-athame"
```

### Comparing `sql_athame-0.4.0a7/sql_athame/base.py` & `sql_athame-0.4.0a8/sql_athame/base.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a7/sql_athame/dataclasses.py` & `sql_athame-0.4.0a8/sql_athame/dataclasses.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import (
     Annotated,
     Any,
     Callable,
     Optional,
     TypeVar,
     Union,
+    get_args,
     get_origin,
     get_type_hints,
 )
 
 from typing_extensions import TypeAlias
 
 from .base import Fragment, sql
@@ -80,38 +81,46 @@
             self.create_type,
             *(() if self.nullable else ("NOT NULL",)),
             *self.constraints,
         )
         return " ".join(parts)
 
 
+NULLABLE_TYPES = (type(None), Any, object)
+
+
+def split_nullable(typ: type) -> tuple[bool, type]:
+    nullable = typ in NULLABLE_TYPES
+    if get_origin(typ) is Union:
+        args = []
+        for arg in get_args(typ):
+            if arg in NULLABLE_TYPES:
+                nullable = True
+            else:
+                args.append(arg)
+        return nullable, Union[tuple(args)]  # type: ignore
+    return nullable, typ
+
+
 sql_create_type_map = {
     "BIGSERIAL": "BIGINT",
     "SERIAL": "INTEGER",
     "SMALLSERIAL": "SMALLINT",
 }
 
 
-sql_type_map: dict[Any, tuple[str, bool]] = {
-    Optional[bool]: ("BOOLEAN", True),
-    Optional[bytes]: ("BYTEA", True),
-    Optional[datetime.date]: ("DATE", True),
-    Optional[datetime.datetime]: ("TIMESTAMP", True),
-    Optional[float]: ("DOUBLE PRECISION", True),
-    Optional[int]: ("INTEGER", True),
-    Optional[str]: ("TEXT", True),
-    Optional[uuid.UUID]: ("UUID", True),
-    bool: ("BOOLEAN", False),
-    bytes: ("BYTEA", False),
-    datetime.date: ("DATE", False),
-    datetime.datetime: ("TIMESTAMP", False),
-    float: ("DOUBLE PRECISION", False),
-    int: ("INTEGER", False),
-    str: ("TEXT", False),
-    uuid.UUID: ("UUID", False),
+sql_type_map: dict[Any, str] = {
+    bool: "BOOLEAN",
+    bytes: "BYTEA",
+    datetime.date: "DATE",
+    datetime.datetime: "TIMESTAMP",
+    float: "DOUBLE PRECISION",
+    int: "INTEGER",
+    str: "TEXT",
+    uuid.UUID: "UUID",
 }
 
 
 T = TypeVar("T", bound="ModelBase")
 U = TypeVar("U")
 
 
@@ -167,24 +176,24 @@
             cls._type_hints = get_type_hints(cls, include_extras=True)
             return cls._type_hints
 
     @classmethod
     def column_info_for_field(cls, field: Field) -> ConcreteColumnInfo:
         type_info = cls.type_hints()[field.name]
         base_type = type_info
+        metadata = []
         if get_origin(type_info) is Annotated:
-            base_type = type_info.__origin__  # type: ignore
-        info = []
+            base_type, *metadata = get_args(type_info)
+        nullable, base_type = split_nullable(base_type)
+        info = [ColumnInfo(nullable=nullable)]
         if base_type in sql_type_map:
-            _type, nullable = sql_type_map[base_type]
-            info.append(ColumnInfo(type=_type, nullable=nullable))
-        if get_origin(type_info) is Annotated:
-            for md in type_info.__metadata__:  # type: ignore
-                if isinstance(md, ColumnInfo):
-                    info.append(md)
+            info.append(ColumnInfo(type=sql_type_map[base_type]))
+        for md in metadata:
+            if isinstance(md, ColumnInfo):
+                info.append(md)
         return ConcreteColumnInfo.from_column_info(field.name, *info)
 
     @classmethod
     def column_info(cls, column: str) -> ConcreteColumnInfo:
         try:
             return cls._column_info[column]  # type: ignore
         except AttributeError:
```

### Comparing `sql_athame-0.4.0a7/sql_athame/escape.py` & `sql_athame-0.4.0a8/sql_athame/escape.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a7/sql_athame/sqlalchemy.py` & `sql_athame-0.4.0a8/sql_athame/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a7/PKG-INFO` & `sql_athame-0.4.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-athame
-Version: 0.4.0a7
+Version: 0.4.0a8
 Summary: Python tool for slicing and dicing SQL
 Home-page: https://github.com/bdowning/sql-athame
 License: MIT
 Author: Brian Downing
 Author-email: bdowning@lavos.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

