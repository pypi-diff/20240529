# Comparing `tmp/vxutils-20240528.tar.gz` & `tmp/vxutils-20240529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vxutils-20240528.tar", max compression
+gzip compressed data, was "vxutils-20240529.tar", max compression
```

## Comparing `vxutils-20240528.tar` & `vxutils-20240529.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2044 2024-05-28 04:35:03.758634 vxutils-20240528/pyproject.toml
--rw-r--r--   0        0        0       24 2024-02-28 02:40:58.487414 vxutils-20240528/README.md
--rw-r--r--   0        0        0      387 2024-04-30 07:57:04.146601 vxutils-20240528/src/vxsched/__init__.py
--rw-r--r--   0        0        0     1374 2024-04-14 08:23:52.813822 vxutils-20240528/src/vxsched/__main__.py
--rw-r--r--   0        0        0     1325 2024-04-30 07:48:16.967272 vxutils-20240528/src/vxsched/__subpubs.py
--rw-r--r--   0        0        0     9403 2024-04-30 08:01:53.820604 vxutils-20240528/src/vxsched/core.py
--rw-r--r--   0        0        0    11734 2024-03-07 05:59:56.919198 vxutils-20240528/src/vxsched/event.py
--rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxutils-20240528/src/vxsched/py.typed
--rw-r--r--   0        0        0        0 2024-04-30 08:02:48.493272 vxutils-20240528/src/vxsched/subpubs/__init__.py
--rw-r--r--   0        0        0     3162 2024-04-30 09:13:45.564793 vxutils-20240528/src/vxsched/subpubs/mqtt.py
--rw-r--r--   0        0        0     3950 2024-04-30 09:12:29.598846 vxutils-20240528/src/vxsched/subpubs/tt.py
--rw-r--r--   0        0        0     1375 2024-04-03 04:23:00.014767 vxutils-20240528/src/vxutils/__init__.py
--rw-r--r--   0        0        0     3738 2024-05-22 11:03:46.262964 vxutils-20240528/src/vxutils/context.py
--rw-r--r--   0        0        0     9225 2024-02-20 02:25:26.235753 vxutils-20240528/src/vxutils/convertors.py
--rw-r--r--   0        0        0      263 2024-05-23 06:52:47.629334 vxutils-20240528/src/vxutils/datamodel/__init__.py
--rw-r--r--   0        0        0     4633 2024-04-25 04:13:01.084260 vxutils-20240528/src/vxutils/datamodel/adapter.py
--rw-r--r--   0        0        0     2536 2024-04-24 08:08:56.901548 vxutils-20240528/src/vxutils/datamodel/core.py
--rw-r--r--   0        0        0    14691 2024-05-28 04:34:45.612248 vxutils-20240528/src/vxutils/datamodel/dborm.py
--rw-r--r--   0        0        0     9071 2024-04-07 01:14:57.773870 vxutils-20240528/src/vxutils/decorators.py
--rw-r--r--   0        0        0     9568 2024-04-07 01:16:17.431751 vxutils-20240528/src/vxutils/dtutils.py
--rw-r--r--   0        0        0     7430 2024-04-10 02:46:27.989670 vxutils-20240528/src/vxutils/logger.py
--rw-r--r--   0        0        0    14529 2024-02-20 08:56:31.979240 vxutils-20240528/src/vxutils/networking/requests.py
--rw-r--r--   0        0        0     7999 2024-05-23 06:50:24.656143 vxutils-20240528/src/vxutils/networking/wechat.py
--rw-r--r--   0        0        0     6161 2024-04-24 04:51:26.814405 vxutils-20240528/src/vxutils/provider.py
--rw-r--r--   0        0        0        0 2024-02-15 15:46:34.000000 vxutils-20240528/src/vxutils/py.typed
--rw-r--r--   0        0        0      446 2024-03-10 03:13:04.515372 vxutils-20240528/src/vxutils/typehints.py
--rw-r--r--   0        0        0     1092 1970-01-01 00:00:00.000000 vxutils-20240528/PKG-INFO
+-rw-r--r--   0        0        0     2044 2024-05-29 03:18:48.055067 vxutils-20240529/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-02-28 02:40:58.487414 vxutils-20240529/README.md
+-rw-r--r--   0        0        0      387 2024-04-30 07:57:04.146601 vxutils-20240529/src/vxsched/__init__.py
+-rw-r--r--   0        0        0     1374 2024-04-14 08:23:52.813822 vxutils-20240529/src/vxsched/__main__.py
+-rw-r--r--   0        0        0     1325 2024-04-30 07:48:16.967272 vxutils-20240529/src/vxsched/__subpubs.py
+-rw-r--r--   0        0        0     9403 2024-04-30 08:01:53.820604 vxutils-20240529/src/vxsched/core.py
+-rw-r--r--   0        0        0    11734 2024-03-07 05:59:56.919198 vxutils-20240529/src/vxsched/event.py
+-rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxutils-20240529/src/vxsched/py.typed
+-rw-r--r--   0        0        0        0 2024-04-30 08:02:48.493272 vxutils-20240529/src/vxsched/subpubs/__init__.py
+-rw-r--r--   0        0        0     3162 2024-04-30 09:13:45.564793 vxutils-20240529/src/vxsched/subpubs/mqtt.py
+-rw-r--r--   0        0        0     3950 2024-04-30 09:12:29.598846 vxutils-20240529/src/vxsched/subpubs/tt.py
+-rw-r--r--   0        0        0     1375 2024-04-03 04:23:00.014767 vxutils-20240529/src/vxutils/__init__.py
+-rw-r--r--   0        0        0     3738 2024-05-22 11:03:46.262964 vxutils-20240529/src/vxutils/context.py
+-rw-r--r--   0        0        0     9225 2024-02-20 02:25:26.235753 vxutils-20240529/src/vxutils/convertors.py
+-rw-r--r--   0        0        0      263 2024-05-23 06:52:47.629334 vxutils-20240529/src/vxutils/datamodel/__init__.py
+-rw-r--r--   0        0        0     4633 2024-04-25 04:13:01.084260 vxutils-20240529/src/vxutils/datamodel/adapter.py
+-rw-r--r--   0        0        0     2536 2024-04-24 08:08:56.901548 vxutils-20240529/src/vxutils/datamodel/core.py
+-rw-r--r--   0        0        0    13907 2024-05-29 03:18:30.596336 vxutils-20240529/src/vxutils/datamodel/dborm.py
+-rw-r--r--   0        0        0     9071 2024-04-07 01:14:57.773870 vxutils-20240529/src/vxutils/decorators.py
+-rw-r--r--   0        0        0     9568 2024-04-07 01:16:17.431751 vxutils-20240529/src/vxutils/dtutils.py
+-rw-r--r--   0        0        0     7430 2024-04-10 02:46:27.989670 vxutils-20240529/src/vxutils/logger.py
+-rw-r--r--   0        0        0    14529 2024-02-20 08:56:31.979240 vxutils-20240529/src/vxutils/networking/requests.py
+-rw-r--r--   0        0        0     7999 2024-05-23 06:50:24.656143 vxutils-20240529/src/vxutils/networking/wechat.py
+-rw-r--r--   0        0        0     6161 2024-04-24 04:51:26.814405 vxutils-20240529/src/vxutils/provider.py
+-rw-r--r--   0        0        0        0 2024-02-15 15:46:34.000000 vxutils-20240529/src/vxutils/py.typed
+-rw-r--r--   0        0        0      446 2024-03-10 03:13:04.515372 vxutils-20240529/src/vxutils/typehints.py
+-rw-r--r--   0        0        0     1092 1970-01-01 00:00:00.000000 vxutils-20240529/PKG-INFO
```

### Comparing `vxutils-20240528/pyproject.toml` & `vxutils-20240529/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vxutils"
-version = "20240528"
+version = "20240529"
 description = "python 常用工具箱"
 license = "MIT"
 authors = ["vex1023 <vex1023@qq.com>"]
 homepage = "https://gitee.com/vxquant/vxutils"
 keywords = ["quant", "tools"]
 readme = "README.md"
```

### Comparing `vxutils-20240528/src/vxsched/__main__.py` & `vxutils-20240529/src/vxsched/__main__.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxsched/__subpubs.py` & `vxutils-20240529/src/vxsched/__subpubs.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxsched/core.py` & `vxutils-20240529/src/vxsched/core.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxsched/event.py` & `vxutils-20240529/src/vxsched/event.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxsched/subpubs/mqtt.py` & `vxutils-20240529/src/vxsched/subpubs/mqtt.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxsched/subpubs/tt.py` & `vxutils-20240529/src/vxsched/subpubs/tt.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxutils/__init__.py` & `vxutils-20240529/src/vxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxutils/context.py` & `vxutils-20240529/src/vxutils/context.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxutils/convertors.py` & `vxutils-20240529/src/vxutils/convertors.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxutils/datamodel/adapter.py` & `vxutils-20240529/src/vxutils/datamodel/adapter.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxutils/datamodel/core.py` & `vxutils-20240529/src/vxutils/datamodel/core.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxutils/datamodel/dborm.py` & `vxutils-20240529/src/vxutils/datamodel/dborm.py`

 * *Files 7% similar despite different names*

```diff
@@ -141,41 +141,41 @@
                 nullable=(name in primary_keys),
             )
             for name, field_info in vxdatacls.model_fields.items()
         ]
 
         if table_name in self._metadata.tables.keys():
             if if_exists == "ignore":
-                logging.warning("Table %s already exists", table_name)
+                logging.debug("Table %s already exists", table_name)
                 return self
             elif if_exists == "replace":
                 tbl = self._metadata.tables[table_name]
                 tbl.drop(bind=self._dbengine, checkfirst=True)
-                logging.warning("Table %s already exists, replace it", table_name)
+                logging.info("Table %s already exists, replace it", table_name)
                 self._metadata.remove(self._metadata.tables[table_name])
 
         tbl = Table(table_name, self._metadata, *column_defs)
         self._tblmapping[table_name] = vxdatacls
         tbl.create(bind=self._dbengine, checkfirst=True)
-        logging.warning("Table: %s ==> %s", table_name, vxdatacls)
+        logging.debug("Create Table: [%s] ==> %s", table_name, vxdatacls)
         return self
 
     def drop_table(self, table_name: str) -> "VXDataBase":
         """删除数据表
 
         Arguments:
             table_name {str} -- 数据表名称
 
         Returns:
             vxDataBase -- 返回数据表格实例
         """
         if table_name in self._metadata.tables.keys():
             tbl = self._metadata.tables[table_name]
             tbl.drop(bind=self._dbengine, checkfirst=True)
-            logging.warning("Table %s dropped", table_name)
+            logging.info("Table %s dropped", table_name)
             self._metadata.remove(self._metadata.tables[table_name])
 
         if table_name in self._tblmapping.keys():
             self._tblmapping.pop(table_name)
 
         return self
 
@@ -243,15 +243,15 @@
             set_={
                 k: v
                 for k, v in vxdataobjs[0].model_dump().items()
                 if k not in tbl.primary_key
             },
         )
         self._conn.execute(insert_stmt)
-        logging.warning("Table %s saved, %s", table_name, insert_stmt.compile())
+        logging.debug("Table %s saved, %s", table_name, insert_stmt.compile())
         return self
 
     def remove(self, table_name: str, *vxdataobjs: VXDataModel) -> "VXDBSession":
         """删除数据
 
         Arguments:
             table_name {str} -- 表格名称
@@ -259,15 +259,15 @@
         """
         tbl = self._metadata.tables[table_name]
         delete_stmt = tbl.delete().where(
             tbl.c[tbl.primary_key.columns.keys()[0]]
             == vxdataobjs[0].model_dump()[tbl.primary_key.columns.keys()[0]]
         )
         self._conn.execute(delete_stmt)
-        logging.warning("Table %s deleted, %s", table_name, delete_stmt)
+        logging.debug("Table %s deleted, %s", table_name, delete_stmt)
         return self
 
     def delete(self, table_name: str, *exprs: str, **options: Any) -> "VXDBSession":
         """删除数据
 
         Arguments:
             table_name {str} -- 表格名称
@@ -282,15 +282,15 @@
         delete_stmt = (
             f"delete from {table_name} where {' and '.join(query)};"
             if query
             else f"delete from {table_name} ; "
         )
 
         result = self._conn.execute(text(delete_stmt))
-        logging.warning("Table %s deleted  %s rows", table_name, result.rowcount)
+        logging.debug("Table %s deleted  %s rows", table_name, result.rowcount)
         return self
 
     def find(
         self,
         table_name: str,
         *exprs: str,
         **options: Any,
@@ -337,17 +337,18 @@
         query_stmt = text(
             f"select * from {table_name} where {' and '.join(query)};"
             if query
             else f"select * from {table_name};"
         )
         result = self._conn.execute(query_stmt)
         row = result.fetchone()
-        if row:
-            return self._tblmapping[table_name](**dict(zip(row._fields, row)))
-        return None
+
+        return (
+            self._tblmapping[table_name](**dict(zip(row._fields, row))) if row else None
+        )
 
     def distinct(self, table_name: str, column: str) -> List[VXDataModel]:
         """查询数据
 
         Arguments:
             table_name {str} -- 表格名称
 
@@ -443,40 +444,15 @@
         return row[0]
 
     def execute(
         self, sql: str, params: Optional[Union[Tuple, Dict, List]] = None
     ) -> Any:
         return self._conn.execute(text(sql), params)
 
-    def commit(self) -> None:
+    def commit(self) -> Any:
         return self._conn.commit()
 
-    def rollback(self) -> None:
+    def rollback(self) -> Any:
         return self._conn.rollback()
 
-    def __enter__(self) -> None:
+    def __enter__(self) -> Any:
         pass
-
-
-if __name__ == "__main__":
-
-    class Test(VXDataModel):
-        a: int
-        b: float
-        c: str
-
-    db = VXDataBase()
-    db.create_table("test", ["a"], Test)
-    db.create_table("test", ["b"], Test, if_exists="replace")
-    db.create_table("test", ["a"], Test)
-    print(db._metadata.tables)
-    test1 = Test(a=1, b=2.0, c="3")
-    test2 = Test(a=2, b=3.0, c="4")
-    test3 = Test(a=1, b=4.0, c="5")
-    with db.start_session() as session:
-        session.save("test", test1, test2, test3)
-        print(list(session.find("test", "b>2")))
-        session.delete("test", "a>1", b=3)
-        print(session.count("test"))
-        print(session.max("test", "b"))
-        print(session.min("test", "b"))
-        print(session.mean("test", "b"))
```

### Comparing `vxutils-20240528/src/vxutils/decorators.py` & `vxutils-20240529/src/vxutils/decorators.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxutils/dtutils.py` & `vxutils-20240529/src/vxutils/dtutils.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxutils/logger.py` & `vxutils-20240529/src/vxutils/logger.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxutils/networking/requests.py` & `vxutils-20240529/src/vxutils/networking/requests.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxutils/networking/wechat.py` & `vxutils-20240529/src/vxutils/networking/wechat.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/src/vxutils/provider.py` & `vxutils-20240529/src/vxutils/provider.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240528/PKG-INFO` & `vxutils-20240529/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vxutils
-Version: 20240528
+Version: 20240529
 Summary: python 常用工具箱
 Home-page: https://gitee.com/vxquant/vxutils
 License: MIT
 Keywords: quant,tools
 Author: vex1023
 Author-email: vex1023@qq.com
 Requires-Python: >=3.8,<4.0
```

